# Comparing `tmp/ms-swift-2.0.4.tar.gz` & `tmp/ms-swift-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ms-swift-2.0.4.tar", last modified: Wed May  1 05:20:13 2024, max compression
+gzip compressed data, was "dist/ms-swift-2.0.5.tar", last modified: Wed May 22 10:57:00 2024, max compression
```

## Comparing `ms-swift-2.0.4.tar` & `ms-swift-2.0.5.tar`

### file list

```diff
@@ -1,229 +1,238 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-01 05:20:08.000000 ms-swift-2.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    60642 2024-05-01 05:20:13.000000 ms-swift-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    54690 2024-05-01 05:20:08.000000 ms-swift-2.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/ms_swift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    60642 2024-05-01 05:20:12.000000 ms-swift-2.0.4/ms_swift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5609 2024-05-01 05:20:13.000000 ms-swift-2.0.4/ms_swift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 05:20:12.000000 ms-swift-2.0.4/ms_swift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-01 05:20:12.000000 ms-swift-2.0.4/ms_swift.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 05:20:12.000000 ms-swift-2.0.4/ms_swift.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-01 05:20:12.000000 ms-swift-2.0.4/ms_swift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-01 05:20:12.000000 ms-swift-2.0.4/ms_swift.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-01 05:20:08.000000 ms-swift-2.0.4/requirements/aigc.txt
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-01 05:20:08.000000 ms-swift-2.0.4/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 05:20:08.000000 ms-swift-2.0.4/requirements/eval.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-01 05:20:08.000000 ms-swift-2.0.4/requirements/framework.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-01 05:20:08.000000 ms-swift-2.0.4/requirements/llm.txt
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-01 05:20:08.000000 ms-swift-2.0.4/requirements/tests.txt
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-01 05:20:13.000000 ms-swift-2.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6181 2024-05-01 05:20:08.000000 ms-swift-2.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/aigc/
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21701 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/animatediff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/animatediff_infer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/aigc/diffusers/
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/diffusers/infer_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/diffusers/infer_controlnet_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/diffusers/infer_dreambooth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/diffusers/infer_dreambooth_lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/diffusers/infer_dreambooth_lora_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/diffusers/infer_text_to_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/diffusers/infer_text_to_image_lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/diffusers/infer_text_to_image_lora_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/diffusers/infer_text_to_image_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)    45735 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/diffusers/train_controlnet.py
--rw-r--r--   0 runner    (1001) docker     (127)    51223 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/diffusers/train_controlnet_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)    56676 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/diffusers/train_dreambooth.py
--rw-r--r--   0 runner    (1001) docker     (127)    54718 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/diffusers/train_dreambooth_lora.py
--rw-r--r--   0 runner    (1001) docker     (127)    67404 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/diffusers/train_dreambooth_lora_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)    44087 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/diffusers/train_text_to_image.py
--rw-r--r--   0 runner    (1001) docker     (127)    39653 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/diffusers/train_text_to_image_lora.py
--rw-r--r--   0 runner    (1001) docker     (127)    50800 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/diffusers/train_text_to_image_lora_sdxl.py
--rw-r--r--   0 runner    (1001) docker     (127)    54357 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/diffusers/train_text_to_image_sdxl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/aigc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/aigc/utils/argument.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/cli/app_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/cli/dpo.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/cli/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/cli/export.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/cli/infer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/cli/merge_lora.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/cli/sft.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/cli/web_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/hub/
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30386 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/hub/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/hub/check_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/hub/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/hub/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    12118 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/hub/file_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/hub/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/hub/push_to_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/hub/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/hub/snapshot_download.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/hub/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/hub/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/hub/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/hub/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/llm/
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/accelerator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/llm/agent/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/agent/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/app_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/llm/data/
--rw-r--r--   0 runner    (1001) docker     (127)    27215 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/data/self_cognition.jsonl
--rw-r--r--   0 runner    (1001) docker     (127)    18965 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     8241 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/dpo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/llm/ds_config/
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/ds_config/zero2.json
--rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/ds_config/zero3.json
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/ds_config/zero3_offload.json
--rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5782 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/export.py
--rw-r--r--   0 runner    (1001) docker     (127)    19178 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/infer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/rome.py
--rw-r--r--   0 runner    (1001) docker     (127)    12450 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/sft.py
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/tuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/llm/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51785 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/utils/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)     3148 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/utils/client_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    58552 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/utils/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)   141321 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/utils/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/utils/protocol.py
--rw-r--r--   0 runner    (1001) docker     (127)    60732 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/utils/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    30852 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/utils/vision_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17049 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/llm/utils/vllm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/torchacc_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/trainers/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/trainers/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/trainers/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)    13725 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/trainers/dpo_trainers.py
--rw-r--r--   0 runner    (1001) docker     (127)    28140 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/trainers/mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/trainers/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/trainers/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/trainers/optimizers/galore/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/trainers/optimizers/galore/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10785 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/trainers/optimizers/galore/adafactor.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6011 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/trainers/optimizers/galore/adamw.py
--rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/trainers/optimizers/galore/adamw8bit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5176 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/trainers/optimizers/galore/galore_projector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/trainers/optimizers/galore/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13289 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/trainers/trainers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/trainers/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/tuners/
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    41066 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/llamapro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/tuners/longlora/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/longlora/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17854 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/longlora/llama.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/longlora/longlora.py
--rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)    38224 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/lora_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/module_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/neftune.py
--rw-r--r--   0 runner    (1001) docker     (127)    13430 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/peft.py
--rw-r--r--   0 runner    (1001) docker     (127)     9211 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)    15748 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/restuning.py
--rw-r--r--   0 runner    (1001) docker     (127)    12682 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/restuning_components.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/tuners/rome/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/rome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/rome/compute_u.py
--rw-r--r--   0 runner    (1001) docker     (127)     9319 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/rome/compute_v.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/rome/context_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/rome/hparams.py
--rw-r--r--   0 runner    (1001) docker     (127)    15391 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/rome/nethook.py
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/rome/repr_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/rome/rome.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/rome/rome_hparams.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/tuners/scetuning/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/scetuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/scetuning/scetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/scetuning/scetuning_components.py
--rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/side.py
--rw-r--r--   0 runner    (1001) docker     (127)    14976 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/tuners/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1598 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/ui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5878 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/ui/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/ui/llm_infer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/ui/llm_infer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/ui/llm_infer/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)    17439 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/ui/llm_infer/llm_infer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/ui/llm_infer/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/ui/llm_infer/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/ui/llm_train/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/ui/llm_train/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/ui/llm_train/advanced.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/ui/llm_train/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/ui/llm_train/hyper.py
--rw-r--r--   0 runner    (1001) docker     (127)    14491 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/ui/llm_train/llm_train.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/ui/llm_train/lora.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/ui/llm_train/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/ui/llm_train/quantization.py
--rw-r--r--   0 runner    (1001) docker     (127)    16132 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/ui/llm_train/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/ui/llm_train/save.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/ui/llm_train/self_cog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/ui/llm_train/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/swift/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/utils/hub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/utils/io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/utils/np_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/utils/run_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/utils/tb_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5419 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/utils/torch_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-01 05:20:08.000000 ms-swift-2.0.4/swift/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/tests/hub/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/hub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/hub/test_check_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/tests/llm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/llm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/llm/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    20012 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/llm/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    26506 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/llm/test_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/llm/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/llm/test_vllm_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/model_tag.py
--rw-r--r--   0 runner    (1001) docker     (127)    22281 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/run.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/tests/tuners/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/tuners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/tuners/test_extra_state_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/tuners/test_merged_linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/tuners/test_neft.py
--rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/tuners/test_peft.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/tuners/test_rome.py
--rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/tuners/test_scetuning.py
--rw-r--r--   0 runner    (1001) docker     (127)    21850 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/tuners/test_swift_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/tuners/test_swift_device_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/tuners/test_swift_restuning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:13.000000 ms-swift-2.0.4/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/utils/test_io_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-01 05:20:08.000000 ms-swift-2.0.4/tests/utils/test_torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-22 10:56:58.000000 ms-swift-2.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    62031 2024-05-22 10:57:00.000000 ms-swift-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    55730 2024-05-22 10:56:58.000000 ms-swift-2.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/ms_swift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    62031 2024-05-22 10:57:00.000000 ms-swift-2.0.5/ms_swift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-05-22 10:57:00.000000 ms-swift-2.0.5/ms_swift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:57:00.000000 ms-swift-2.0.5/ms_swift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-22 10:57:00.000000 ms-swift-2.0.5/ms_swift.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:57:00.000000 ms-swift-2.0.5/ms_swift.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-05-22 10:57:00.000000 ms-swift-2.0.5/ms_swift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-22 10:57:00.000000 ms-swift-2.0.5/ms_swift.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-22 10:56:58.000000 ms-swift-2.0.5/requirements/aigc.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-22 10:56:58.000000 ms-swift-2.0.5/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-22 10:56:58.000000 ms-swift-2.0.5/requirements/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-22 10:56:58.000000 ms-swift-2.0.5/requirements/framework.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-22 10:56:58.000000 ms-swift-2.0.5/requirements/llm.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 10:56:58.000000 ms-swift-2.0.5/requirements/seq_parallel.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-22 10:56:58.000000 ms-swift-2.0.5/requirements/tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-22 10:57:00.000000 ms-swift-2.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-22 10:56:58.000000 ms-swift-2.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/aigc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21701 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/animatediff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/animatediff_infer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/aigc/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/diffusers/infer_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/diffusers/infer_controlnet_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/diffusers/infer_dreambooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/diffusers/infer_dreambooth_lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/diffusers/infer_dreambooth_lora_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/diffusers/infer_text_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/diffusers/infer_text_to_image_lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/diffusers/infer_text_to_image_lora_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/diffusers/infer_text_to_image_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45624 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/diffusers/train_controlnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51112 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/diffusers/train_controlnet_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56676 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/diffusers/train_dreambooth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54718 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/diffusers/train_dreambooth_lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67404 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/diffusers/train_dreambooth_lora_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43976 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/diffusers/train_text_to_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39542 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/diffusers/train_text_to_image_lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50689 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/diffusers/train_text_to_image_lora_sdxl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54246 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/diffusers/train_text_to_image_sdxl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/aigc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/aigc/utils/argument.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/cli/app_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/cli/dpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/cli/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/cli/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/cli/infer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/cli/merge_lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/cli/orpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/cli/sft.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/cli/web_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30190 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/hub/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3666 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/hub/check_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/hub/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/hub/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12118 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/hub/file_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/hub/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/hub/push_to_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/hub/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6593 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/hub/snapshot_download.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/hub/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/hub/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/hub/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/hub/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/accelerator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/llm/agent/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/agent/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/app_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/llm/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     7808 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/data/dataset_info.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27215 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/data/self_cognition.jsonl
+-rw-r--r--   0 runner    (1001) docker     (127)    19413 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9932 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/dpo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/llm/ds_config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/ds_config/zero2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1545 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/ds_config/zero3.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/ds_config/zero3_offload.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7721 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23190 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/infer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10361 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/orpo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/rome.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14853 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/sft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17274 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/tuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/llm/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62117 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/utils/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3194 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/utils/client_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49694 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/utils/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)   156706 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9196 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/utils/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3785 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/utils/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65722 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/utils/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35201 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/utils/vision_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17195 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/llm/utils/vllm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11181 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/torchacc_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/trainers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/trainers/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/trainers/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13725 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/trainers/dpo_trainers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29196 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/trainers/mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/trainers/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/trainers/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/trainers/optimizers/galore/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/trainers/optimizers/galore/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10785 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/trainers/optimizers/galore/adafactor.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6011 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/trainers/optimizers/galore/adamw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3819 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/trainers/optimizers/galore/adamw8bit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5176 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/trainers/optimizers/galore/galore_projector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/trainers/optimizers/galore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8402 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/trainers/orpo_trainers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13779 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/trainers/trainers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/trainers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/trainers/xtuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/tuners/
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7604 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42757 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7598 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/llamapro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/tuners/longlora/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/longlora/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17854 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/longlora/llama.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/longlora/longlora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7921 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40406 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/lora_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4949 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/module_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/neftune.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13718 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/peft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9211 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15748 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/restuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12682 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/restuning_components.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/tuners/rome/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/rome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/rome/compute_u.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9319 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/rome/compute_v.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/rome/context_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/rome/hparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15391 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/rome/nethook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/rome/repr_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7284 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/rome/rome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/rome/rome_hparams.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/tuners/scetuning/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/scetuning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10531 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/scetuning/scetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/scetuning/scetuning_components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9442 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/side.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15140 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/tuners/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6026 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/ui/llm_infer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/llm_infer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/llm_infer/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17981 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/llm_infer/llm_infer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/llm_infer/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10665 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/llm_infer/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/ui/llm_train/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/llm_train/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/llm_train/advanced.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/llm_train/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/llm_train/galore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4903 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/llm_train/hyper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/llm_train/lisa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/llm_train/llamapro.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15069 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/llm_train/llm_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/llm_train/lora.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/llm_train/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/llm_train/quantization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16577 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/llm_train/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/llm_train/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/llm_train/self_cog.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/ui/llm_train/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/swift/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3229 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/utils/hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/utils/io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2768 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/utils/np_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/utils/run_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/utils/tb_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/utils/torch_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6248 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-22 10:56:58.000000 ms-swift-2.0.5/swift/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/tests/hub/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/hub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/hub/test_check_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/tests/llm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/llm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/llm/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21590 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/llm/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26506 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/llm/test_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/llm/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/llm/test_vllm_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/model_tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22281 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/tests/tuners/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/tuners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3452 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/tuners/test_extra_state_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/tuners/test_merged_linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/tuners/test_neft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/tuners/test_peft.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/tuners/test_rome.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4202 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/tuners/test_scetuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21850 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/tuners/test_swift_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/tuners/test_swift_device_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/tuners/test_swift_restuning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:57:00.000000 ms-swift-2.0.5/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/utils/test_io_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-22 10:56:58.000000 ms-swift-2.0.5/tests/utils/test_torch_utils.py
```

### Comparing `ms-swift-2.0.4/PKG-INFO` & `ms-swift-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-swift
-Version: 2.0.4
+Version: 2.0.5
 Summary: Swift: Scalable lightWeight Infrastructure for Fine-Tuning
 Home-page: https://github.com/modelscope/swift
 Author: DAMO ModelScope teams
 Author-email: contact@modelscope.cn
 License: Apache License 2.0
 Description: # SWIFT (Scalable lightWeight Infrastructure for Fine-Tuning)
         
@@ -25,41 +25,63 @@
         <a href="https://github.com/modelscope/modelscope/"><img src="https://img.shields.io/badge/modelscope-%E2%89%A51.9.5-5D91D4.svg"></a>
         <a href="https://pypi.org/project/ms-swift/"><img src="https://badge.fury.io/py/ms-swift.svg"></a>
         <a href="https://github.com/modelscope/swift/blob/main/LICENSE"><img src="https://img.shields.io/github/license/modelscope/swift"></a>
         <a href="https://pepy.tech/project/ms-swift"><img src="https://pepy.tech/badge/ms-swift"></a>
         <a href="https://github.com/modelscope/swift/pulls"><img src="https://img.shields.io/badge/PR-welcome-55EB99.svg"></a>
         </p>
         
+        <p align="center">
+        <a href="https://trendshift.io/repositories/6427" target="_blank"><img src="https://trendshift.io/api/badge/repositories/6427" alt="modelscope%2Fswift | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>
+        </p>
+        
         ## 📖 Table of Contents
         - [Introduction](#-introduction)
         - [News](#-news)
         - [Installation](#%EF%B8%8F-installation)
         - [Getting Started](#-getting-started)
         - [Documentation](#-documentation)
         - [License](#-License)
         - [Citation](#-citation)
-        - [Contact Us](#-contact-us)
+        - [WeChat Group](#-Wechat-Group)
         
         ## 📝 Introduction
         SWIFT supports training, inference, evaluation and deployment of nearly **200 LLMs and MLLMs** (multimodal large models). Developers can directly apply our framework to their own research and production environments to realize the complete workflow from model training and evaluation to application. In addition to supporting the lightweight training solutions provided by [PEFT](https://github.com/huggingface/peft), we also provide a complete **Adapters library** to support the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This adapter library can be used directly in your own custom workflow without our training scripts.
         
         To facilitate use by users unfamiliar with deep learning, we provide a Gradio web-ui for controlling training and inference, as well as accompanying deep learning courses and best practices for beginners.
         
         Additionally, we are expanding capabilities for other modalities. Currently, we support full-parameter training and LoRA training for AnimateDiff.
         
+        SWIFT has rich documentations for users, please check [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM).
+        
+        SWIFT web-ui is available both on [Huggingface space](https://huggingface.co/spaces/tastelikefeet/swift) and [ModelScope studio](https://www.modelscope.cn/studios/iic/Scalable-lightWeight-Infrastructure-for-Fine-Tuning/summary), please feel free to try!
+        
         ## 🎉 News
+        - 2024.05.22: Supports DeepSeek-V2-Lite series models, model_type are `deepseek-v2-lite` and `deepseek-v2-lite-chat`
+        - 2024.05.22: Supports TeleChat-12B-v2 model with quantized version, model_type are `telechat-12b-v2` and `telechat-12b-v2-gptq-int4`
+        - 🔥2024.05.21: Inference and fine-tuning support for MiniCPM-Llama3-V-2_5 are now available. For more details, please refer to [minicpm-v-2.5 Best Practice](docs/source/Multi-Modal/minicpm-v-2.5最佳实践.md).
+        - 🔥2024.05.20: Support for inferencing and fine-tuning cogvlm2-llama3-chinese-chat-19B, cogvlm2-llama3-chat-19B. you can refer to [cogvlm2 Best Practice](docs/source_en/Multi-Modal/cogvlm2-best-practice.md).
+        - 🔥2024.05.17: Support peft=0.11.0. Meanwhile support 3 new tuners: `BOFT`, `Vera` and `Pissa`. use `--sft_type boft/vera` to use BOFT or Vera, use `--init_lora_weights pissa` with `--sft_type lora` to use Pissa.
+        - 2024.05.16: Supports Llava-Next (Stronger) series models. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-practice.md).
+        - 🔥2024.05.13: Support Yi-1.5 series models，use `--model_type yi-1_5-9b-chat` to begin!
+        - 2024.05.11: Support for qlora training and quantized inference using [hqq](https://github.com/mobiusml/hqq) and [eetq](https://github.com/NetEase-FuXi/EETQ). For more information, see the [LLM Quantization Documentation](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/LLM-quantization.md).
+        - 2024.05.10: Support split a sequence to multiple GPUs to reduce memory usage. Use this feature by `pip install .[seq_parallel]`, then add `--sequence_parallel_size n` to your DDP script to begin!
+        - 2024.05.08: Support DeepSeek-V2-Chat model, you can refer to [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/deepseek-v2-chat/lora_ddp_ds3/sft.sh).Support InternVL-Chat-V1.5-Int8 model, for best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/internvl-best-practice.md).
+        - 🔥2024.05.07: Supoprts **ORPO** training! See [document](https://github.com/modelscope/swift/blob/main/docs/source_en/LLM/ORPO.md) to start training!
+        - 2024.05.07: Supports Llava-Llama3 model from xtuner，model_type is `llava-llama-3-8b-v1_1`.
         - 2024.04.29: Supports inference and fine-tuning of InternVL-Chat-V1.5 model. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/internvl-best-practice.md).
         - 🔥2024.04.26: Support **LISA** and **unsloth** training! Specify `--lisa_activated_layers=2` to use LISA(to reduce the memory cost to 30 percent!), specify `--tuner_backend unsloth` to use unsloth to train a huge model(full or lora) with lesser memory(30 percent or lesser) and faster speed(5x)!
         - 🔥2024.04.26: Support the fine-tuning and inference of Qwen1.5-110B and Qwen1.5-110B-Chat model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_110b_chat/lora_ddp_ds/sft.sh) to start training!
         - 2024.04.24: Support for inference and fine-tuning of Phi3 series models. Including: [phi3-4b-4k-instruct](examples/pytorch/llm/scripts/phi3_4b_4k_instruct/lora), phi3-4b-128k-instruct.
         - 2024.04.22: Support for inference, fine-tuning, and deployment of **chinese-llama-alpaca-2** series models. This includes：chinese-llama-2-1.3b, chinese-llama-2-7b, chinese-llama-2-13b, chinese-alpaca-2-1.3b, chinese-alpaca-2-7b and chinese-alpaca-2-13b along with their corresponding 16k and 64k long text versions.
         - 2024.04.22: Support for inference and fine-tuning of Llama3 GPTQ-Int4, GPTQ-Int8, and AWQ series models. Support for inference and fine-tuning of chatglm3-6b-128k, Openbuddy-Llama3.
         - 2024.04.20: Support for inference, fine-tuning, and deployment of **Atom** series models. This includes: Atom-7B and Atom-7B-Chat. use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/atom_7b_chat/lora/sft.sh) to train.
-        - 2024.04.19: Support for single-card, DDP, ZeRO2, and ZeRO3 training and inference with NPU, please refer to [NPU Inference and Fine-tuning Best Practices](docs/source_en/LLM/NPU-best-practice.md).
+        - 2024.04.19: Support for single-card, DDP, ZeRO2, and ZeRO3 training and inference with NPU, please refer to [NPU Inference and Fine-tuning Best Practice](docs/source_en/LLM/NPU-best-practice.md).
         - 2024.04.19: Support for inference, fine-tuning, and deployment of **Llama3** series models. This includes: Llama-3-8B, Llama-3-8B-Instruct, Llama-3-70B, and Llama-3-70B-Instruct. use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama3_8b_instruct/lora/sft.sh) to train.
+        <details><summary>More</summary>
+        
         - 2024.04.18: Supported models: wizardlm2-7b-awq, wizardlm2-8x22b, yi-6b-chat-awq, yi-6b-chat-int8, yi-34b-chat-awq, yi-34b-chat-int8. Supported `--deepspeed zero3-offload` and provided default zero3-offload configuration file for zero3+cpu offload usage.
         - 2024.04.18: Supported compatibility with HuggingFace ecosystem using the environment variable `USE_HF`, switching to use models and datasets from HF. Please refer to the [HuggingFace ecosystem compatibility documentation](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Compat-HF.md).
         - 2024.04.17: Support the evaluation for OpenAI standard interfaces. Check the [parameter documentation](docs/source_en/LLM/Command-line-parameters.md#eval-parameters) for details.
         - 🔥2024.04.17: Support **CodeQwen1.5-7B** series: CodeQwen1.5-7B, CodeQwen1.5-7B-Chat,CodeQwen1.5-7B-Chat-AWQ, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/codeqwen1half_7b_chat/lora/sft.sh) to train.
         - 2024.04.16: Supports inference and fine-tuning of llava-v1.6-34b model. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-practice.md).
         - 2024.04.13: Support the fine-tuning and inference of Mixtral-8x22B-v0.1 model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/lora_ddp_ds/sft.sh) to start training!
         - 2024.04.13: Support the newly launched **MiniCPM** series: MiniCPM-V-2.0、MiniCPM-2B-128k、MiniCPM-MoE-8x2B and MiniCPM-1B.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/minicpm_moe_8x2b/lora_ddp/sft.sh) to start training!
@@ -72,16 +94,14 @@
         - 🔥2024.04.03: Support **Qwen1.5-32B** series: Qwen1.5-32B, Qwen1.5-32B-Chat, Qwen1.5-32B-Chat-GPTQ-Int4.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_32b_chat/lora_mp/sft.sh) to start training!
         - 🔥2024.04.02: Support the fine-tuning and inference of Mengzi3-13B-Base model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mengzi3_13b_base/lora_ddp_ds/sft.sh) to start training!
         - 🔥2024.04.01: Support **dbrx** series: dbrx-base and dbrx-instruct, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/dbrx-instruct/lora_mp/sft.sh) to start training!
         - 🔥2024.03.29: Support **Qwen1.5-MoE** series: Qwen1.5-MoE-A2.7B, Qwen1.5-MoE-A2.7B-Chat, Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4.
         - 🔥2024.03.29: Support the fine-tuning and inference of **Grok-1** 300B MoE, please view details [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-practice.md).
         - 🔥2024.03.25: Supports inference and fine-tuning of TeleChat-7b and TeleChat-12b model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start training!
         - 🔥2024.03.20: Supports inference and fine-tuning for the **llava** series. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-practice.md).
-        <details><summary>More</summary>
-        
         - 🔥2024.03.12: Support inference and fine-tuning for **deepseek-vl** series. Best practices can be found [here](docs/source_en/Multi-Modal/deepseek-vl-best-practice.md).
         - 🔥2024.03.11: Support [GaLore](https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/2 of the original in full-parameter training.
         - 🔥2024.03.10: [End-to-end best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat.
         - 🔥2024.03.09: Support training and inference of MAMBA model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mamba-1.4b/lora/sft.sh) to start training!
         - 2024.03.09: Support training and inference of AQLM quantized model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama2_7b_aqlm_2bit_1x16/lora/sft.sh) to start training!
         - 2024.03.06: Support training and inference of AWQ quantized model, use [this Qwen1.5-AWQ model script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_awq/lora/sft.sh) to start training, and support training and inference of [yi-9b](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_9b/lora_zero3).
         - 🔥2024.02.29: Support [LLaMA PRO](https://arxiv.org/pdf/2401.02415.pdf), simply use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/llamapro/sft.sh) to start training.
@@ -104,18 +124,17 @@
         - 2024.01.24: Support codefuse-codegeex2-6b-chat, codefuse-qwen-14b-chat.
         - 2024.01.23: Support orion series: orion-14b, [orion-14b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/orion_14b_chat).
         - 2024.01.20: Support [xverse-13b-256k](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/xverse_13b_256k), xverse-65b-v2, xverse-65b-chat.
         - 🔥2024.01.17: Support internlm2 series: internlm2-7b-base, internlm2-7b, [internlm2-7b-sft-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/internlm2_7b_sft_chat), internlm2-7b-chat, internlm2-20b-base, internlm2-20b, internlm2-20b-sft-chat, internlm2-20b-chat.
         - 2024.01.15: Support yuan series: yuan2-2b-instruct, [yuan2-2b-janus-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yuan2_2b_janus_instruct), yuan2-51b-instruct, yuan2-102b-instruct.
         - 🔥2024.01.12: Support **deepseek-moe** series: deepseek-moe-16b, [deepseek-moe-16b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/deepseek_moe_16b_chat).
         - 🔥2024.01.04: Support **VLLM deployment**, compatible with **OpenAI API** style, see [VLLM Inference Acceleration and Deployment](https://github.com/modelscope/swift/blob/main/docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md#Deployment) for details.
-        
         - 2024.01.04: Update [Benchmark](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) for convenient viewing of training speed and memory usage of different models.
         - 🔥2023.12.29: Support web-ui for sft training and inference, use `swift web-ui` after installing ms-swift to start.
-        - 🔥2023.12.29: Support DPO RLHF (Reinforcement Learning from Human Feedback) and three datasets for this task: AI-ModelScope/stack-exchange-paired, AI-ModelScope/hh-rlhf and AI-ModelScope/hh_rlhf_cn. See [documentation](https://github.com/modelscope/swift/blob/main/docs/source/LLM/LLM%E4%BA%BA%E7%B1%BB%E5%AF%B9%E9%BD%90%E8%AE%AD%E7%BB%83%E6%96%87%E6%A1%A3.md) to start training!
+        - 🔥2023.12.29: Support DPO RLHF (Reinforcement Learning from Human Feedback) and three datasets for this task: AI-ModelScope/stack-exchange-paired, AI-ModelScope/hh-rlhf and AI-ModelScope/hh_rlhf_cn. See [documentation](https://github.com/modelscope/swift/blob/main/docs/source_en/LLM/DPO.md) to start training!
         - 🔥2023.12.28: Support SCEdit! This tuner can significantly reduce memory usage in U-Net and support low-memory controllable image generation (replacing ControlNet), read the section below to learn more.
         - 2023.12.23: Support [codegeex2-6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/codegeex2_6b).
         - 2023.12.19: Support [phi2-3b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/phi2_3b).
         - 2023.12.18: Support VLLM for inference acceleration.
         - 2023.12.15: Support deepseek, deepseek-coder series: deepseek-7b, deepseek-7b-chat, deepseek-67b, deepseek-67b-chat, openbuddy-deepseek-67b-chat, deepseek-coder-1_3b, deepseek-coder-1_3b-instruct, deepseek-coder-6_7b, deepseek-coder-6_7b-instruct, deepseek-coder-33b, deepseek-coder-33b-instruct.
         - 2023.12.13: Support mistral-7b-instruct-v2, [mixtral-moe-7b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/mixtral_7b_moe), [mixtral-moe-7b-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/mixtral_7b_moe_instruct).
         - 2023.12.09: Support `freeze_parameters` parameter as a compromise between lora and full-parameter training. Corresponding sh can be found in [full_freeze_ddp](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/full_freeze_ddp). Support `disable_tqdm`, `lazy_tokenize`, `preprocess_num_proc` parameters, see [command line arguments](https://github.com/modelscope/swift/blob/main/docs/source/LLM/%E5%91%BD%E4%BB%A4%E8%A1%8C%E5%8F%82%E6%95%B0.md) for details.
@@ -187,18 +206,22 @@
         
         ## 🚀 Getting Started
         
         This section introduces basic usage, see the [Documentation](#-documentation) section for more ways to use.
         
         ### Web-UI
         
+        Web-UI is a gradio-based interface for **zero-threshold** training and deployment. It is easy to use and perfectly supports multi-GPU training and deployment:
+        
         ```shell
-        swift web-ui
+        SWIFT_UI_LANG=en swift web-ui
         ```
         
+        ![image.png](./docs/resources/web-ui-en.jpg)
+        
         ### Training
         
         #### Training Scripts
         You can refer to the following scripts to customize your own training script.
         
         - full: [qwen1half-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat/full) (A100), [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/full_mp) (2\*A100)
         - full+ddp+zero2: [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/full_ddp_zero2) (4\*A100)
@@ -213,15 +236,15 @@
         
         #### Supported Training Processes
         
         | Training Process | Training Method                                                               |
         |------------------|-------------------------------------------------------------------------------|
         | Pretraining      | Text Generation                                                               |
         | Fine-tuning      | Single-turn/Multi-turn<br>Agent Training/Self-cognition<br>Multi-modal Vision/Multi-modal Speech|
-        | Human Alignment  | DPO                                                                           |
+        | Human Alignment  | DPO<br>ORPO                                                                   |
         | Text-to-Image    | DreamBooth, etc.                                                              |
         | Text-to-Video    | -                                                                             |
         
         #### Single GPU Training
         
         Start single GPU fine-tuning with the following command:
         
@@ -380,14 +403,28 @@
             --model_id_or_path qwen1half-32b-chat \
             --sft_type full \
             --dataset blossom-math-zh \
             --output_dir output \
             --deepspeed default-zero3 \
         ```
         
+        ##### AliYun-DLC multi-node training
+        In DLC product, WORLD_SIZE is the node number, RANK is the node index, this is different from the definition of torchrun.
+        
+        ```shell
+        NNODES=$WORLD_SIZE \
+        NODE_RANK=$RANK \
+        swift sft \
+            --model_id_or_path qwen1half-32b-chat \
+            --sft_type full \
+            --dataset blossom-math-zh \
+            --output_dir output \
+            --deepspeed default-zero3
+        ```
+        
         
         ### Inference
         Original model:
         ```shell
         CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat
         # use VLLM
         CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat \
@@ -455,17 +492,17 @@
         | ChatGLM2<br>ChatGLM3<br>Codegeex2                    | [Zhipu ChatGLM series models](https://github.com/THUDM)               | Chinese<br>English    | 6B                                     | base model<br>chat model<br>code model<br>long text model  |
         | Baichuan/Baichuan2                             | [Baichuan 1 and Baichuan 2](https://github.com/baichuan-inc)           | Chinese<br>English    | 7B-13B<br>including quantized versions             | base model<br>chat model                       |
         | Yuan2                                          | [Langchao Yuan series models](https://github.com/IEIT-Yuan)             | Chinese<br>English    | 2B-102B                                | instruct model                                 |
         | XVerse                                         | [XVerse series models](https://github.com/xverse-ai)                    | Chinese<br>English    | 7B-65B                                 | base model<br>chat model<br>long text model<br>MoE model                |
         | LLaMA2                                         | [LLaMA2 series models](https://github.com/facebookresearch/llama)       | English            | 7B-70B<br>including quantized versions   | base model<br>chat model                       |
         | LLaMA3                   | [LLaMA3 series models](https://github.com/meta-llama/llama3)  | English       | 8B-70B<br>including quantized versions      | base model<br>chat model              |
         | Mistral<br>Mixtral                            | [Mistral series models](https://github.com/mistralai/mistral-src)       | English            | 7B-22B     | base model<br>instruct model<br>MoE model                     |
-        | YI                                             | [01AI's YI series models](https://github.com/01-ai)                     | Chinese<br>English    | 6B-34B<br>including quantized             | base model<br>chat model<br>long text model            |
+        | Yi<br>Yi1.5                                      | [01AI's YI series models](https://github.com/01-ai)                     | Chinese<br>English    | 6B-34B<br>including quantized             | base model<br>chat model<br>long text model            |
         | InternLM<br>InternLM2<br>InternLM2-Math              | [Pujiang AI Lab InternLM series models](https://github.com/InternLM/InternLM) | Chinese<br>English | 1.8B-20B                            | base model<br>chat model<br>math model            |
-        | DeepSeek<br>DeepSeek-MoE<br>DeepSeek-Coder<br>DeepSeek-Math          | [DeepSeek series models](https://github.com/deepseek-ai)       | Chinese<br>English    | 1.3B-67B                               | base model<br>chat model<br>MoE model<br>code model<br>math model |
+        | DeepSeek<br>DeepSeek-MoE<br>DeepSeek-Coder<br>DeepSeek-Math<br>DeepSeek-V2          | [DeepSeek series models](https://github.com/deepseek-ai)       | Chinese<br>English    | 1.3B-236B                               | base model<br>chat model<br>MoE model<br>code model<br>math model |
         | MAMBA                                          | [MAMBA temporal convolution model](https://github.com/state-spaces/mamba) | English          | 130M-2.8B                              | base model                                 |
         | Gemma                                          | [Google Gemma series models](https://github.com/google/gemma_pytorch)   | English            | 2B-7B                                  | base model<br>instruct model                       |
         | MiniCPM                                        | [OpenBmB MiniCPM series models](https://github.com/OpenBMB/MiniCPM)     | Chinese<br>English    | 2B-3B                                  | chat model<br>MoE model                                 |
         | OpenBuddy                                      | [OpenBuddy series models](https://github.com/OpenBuddy/OpenBuddy)       | Chinese<br>English    | 7B-67B                                 | base model<br>chat model                       |
         | Orion                                          | [OrionStar AI series models](https://github.com/OrionStarAI)            | Chinese<br>English    | 14B                                    | base model<br>chat model                       |
         | BlueLM                                         | [VIVO BlueLM large model](https://github.com/vivo-ai-lab/BlueLM)        | Chinese<br>English    | 7B                                     | base model<br>chat model                       |
         | Ziya2                                          | [Fengshenbang series models](https://github.com/IDEA-CCNL/Fengshenbang-LM) | Chinese<br>English  | 13B                                    | base model<br>chat model                       |
@@ -486,52 +523,54 @@
         | Atom | [Atom](https://github.com/LlamaFamily/Llama-Chinese) | Chinese | 7B| base model<br>chat model|
         | Chinese-LLaMA-Alpaca-2 | [Chinese-LLaMA-Alpaca-2](https://github.com/ymcui/Chinese-LLaMA-Alpaca-2) | Chinese | 1.3B-13B| base model<br>chat model<br>long text model |
         | Chinese-LLaMA-Alpaca-3 | [Chinese-LLaMA-Alpaca-3](https://github.com/ymcui/Chinese-LLaMA-Alpaca-3) | Chinese | 8B| base model<br>chat model|
         | ModelScope-Agent | [ModelScope Agent series models](https://github.com/modelscope/modelscope-agent) | Chinese | 7B-14B| agent model |
         
         #### MLLMs
         
-        | Model Type       | Model Introduction                                                     | Language           | Model Size        | Model Type         |
+        | Model Type         | Model Introduction                                                           | Language           | Model Size                         | Model Type         |
         |------------------|------------------------------------------------------------------------|--------------------|-------------------|------------------- |
-        | Qwen-VL          | [Tongyi Qwen vision model](https://github.com/QwenLM)               | Chinese<br>English    | 7B<br>including quantized versions | base model<br>chat model |
-        | Qwen-Audio       | [Tongyi Qwen speech model](https://github.com/QwenLM)               | Chinese<br>English    | 7B                | base model<br>chat model |
-        | YI-VL            | [01AI's YI series vision models](https://github.com/01-ai)             | Chinese<br>English    | 6B-34B            | chat model         |
-        | XComposer2       | [Pujiang AI Lab InternLM vision model](https://github.com/InternLM/InternLM) | Chinese<br>English | 7B              | chat model         |
-        | DeepSeek-VL      | [DeepSeek series vision models](https://github.com/deepseek-ai) | Chinese<br>English    | 1.3B-7B           | chat model         |
-        | MiniCPM-V       | [OpenBmB MiniCPM vision model](https://github.com/OpenBMB/MiniCPM)     | Chinese<br>English    | 3B                | chat model         |
-        | CogVLM<br>CogAgent  | [Zhipu ChatGLM visual QA and Agent model](https://github.com/THUDM/)   | English    | 17B-18B           | chat model         |
-        | Llava      | [Llava series models](https://github.com/haotian-liu/LLaVA)                | English | 7B-34B               | chat model |
-        | mPLUG-Owl      | [mPLUG-Owl series models](https://github.com/X-PLUG/mPLUG-Owl)         | English | 11B               | chat model |
-        | InternVL         | [InternVL](https://github.com/OpenGVLab/InternVL)                | Chinese<br>English | 25.5B | chat model |
+        | Qwen-VL            | [Tongyi Qwen vision model](https://github.com/QwenLM)                        | Chinese<br>English    | 7B<br>including quantized versions | base model<br>chat model |
+        | Qwen-Audio         | [Tongyi Qwen speech model](https://github.com/QwenLM)                        | Chinese<br>English    | 7B                                 | base model<br>chat model |
+        | YI-VL              | [01AI's YI series vision models](https://github.com/01-ai)                   | Chinese<br>English    | 6B-34B                             | chat model         |
+        | XComposer2         | [Pujiang AI Lab InternLM vision model](https://github.com/InternLM/InternLM) | Chinese<br>English | 7B                                 | chat model         |
+        | DeepSeek-VL        | [DeepSeek series vision models](https://github.com/deepseek-ai)              | Chinese<br>English    | 1.3B-7B                            | chat model         |
+        | MiniCPM-V<br>MiniCPM-V-2<br>MiniCPM-V-2_5  | [OpenBmB MiniCPM vision model](https://github.com/OpenBMB/MiniCPM) | Chinese<br>English | 3B-9B            | chat model          |
+        | CogVLM<br>CogVLM2<br>CogAgent | [Zhipu ChatGLM visual QA and Agent model](https://github.com/THUDM/)         | Chinese<br>English    | 17B-19B                            | chat model         |
+        | Llava              | [Llava series models](https://github.com/haotian-liu/LLaVA)                  | English | 7B-34B                             | chat model |
+        | Llava-Next              | [Llava-Next series models](https://github.com/LLaVA-VL/LLaVA-NeXT)                  | Chinese<br>English | 8B-110B                             | chat model |
+        | mPLUG-Owl          | [mPLUG-Owl series models](https://github.com/X-PLUG/mPLUG-Owl)               | English | 11B                                | chat model |
+        | InternVL           | [InternVL](https://github.com/OpenGVLab/InternVL)                            | Chinese<br>English | 25.5B<br>including quantized version                              | chat model |
+        | Llava-llama3       | [xtuner](https://huggingface.co/xtuner/llava-llama-3-8b-v1_1-transformers)   | English | 8B                                 | chat model |
         
         #### Diffusion Models
         
         | Model Type          | Model Introduction                                                    | Language | Model Type        |
         |---------------------|----------------------------------------------------------------------|----------|------------------ |
         | AnimateDiff         | [AnimateDiff animation model](https://github.com/guoyww/AnimateDiff) | English  | text-to-video     |
         | SD1.5/SD2.0/SDXL    | [StabilityAI series diffusion models](https://github.com/Stability-AI) | English | text-to-image    |
         
         ### Supported Open Source Datasets
         
         | Dataset Type | Training Task  | Documentation                                                                                                                                                                                                                                                                                                        |
         |--------------|:---------------|--------------------------------------------------------------- |
-        | General      | Fine-tuning    | 🔥ruozhiba, 🔥ms-bench, 🔥ms-bench-mini, 🔥alpaca-en(gpt4), 🔥alpaca-zh(gpt4), multi-alpaca-all, instinwild-en, instinwild-zh, cot-en, cot-zh, firefly-all-zh, instruct-en, gpt4all-en, sharegpt-en, sharegpt-zh, tulu-v2-sft-mixture, wikipedia-zh, open-orca, open-orca-gpt4, sharegpt-gpt4, 🔥sharegpt-gpt4-mini. |
-        | Agent        | Fine-tuning    | 🔥ms-agent, ms-agent-for-agentfabric-default, ms-agent-for-agentfabric-addition, damo-mini-agent-zh, damo-agent-zh, agent-instruct-all-en.                                                                                                                                                                                                                                                |
-        | General      | Human Alignment | 🔥hh-rlhf-cn, stack-exchange-paired, hh-rlhf-harmless-base, hh-rlhf-helpful-base, hh-rlhf-helpful-online, hh-rlhf-helpful-rejection-sampled, hh-rlhf-red-team-attempts, hh-rlhf-cn-harmless-base-cn, hh-rlhf-cn-helpful-base-cn, hh-rlhf-cn-harmless-base-en, hh-rlhf-cn-helpful-base-en.                            |
-        | Code         | Fine-tuning    | code-alpaca-en, 🔥leetcode-python-en, 🔥codefuse-python-en, 🔥codefuse-evol-instruction-zh.                                                                                                                                                                                                                          |
-        | Medical      | Fine-tuning    | medical-en, medical-zh, medical-mini-zh, 🔥disc-med-sft-zh.                                                                                                                                                                                                                                                          |
-        | Legal        | Fine-tuning    | lawyer-llama-zh, tigerbot-law-zh, 🔥disc-law-sft-zh.                                                                                                                                                                                                                                                                 |
-        | Math         | Fine-tuning    | 🔥blossom-math-zh, school-math-zh, open-platypus-en.                                                                                                                                                                                                                                                                 |
-        | SQL          | Fine-tuning    | text2sql-en, 🔥sql-create-context-en.                                                                                                                                                                                                                                                                                |
-        | Text Generation | Fine-tuning | 🔥advertise-gen-zh, 🔥dureader-robust-zh.                                                                                                                                                                                                                                                                            |
-        | Classification | Fine-tuning  | cmnli-zh, 🔥cmnli-mini-zh, 🔥jd-sentiment-zh, 🔥hc3-zh, 🔥hc3-en.                                                                                                                                                                                                                                                    |
-        | Quantization Assist | Quantization | pileval.                                                                                                                                                                                                                                                                                                             |
-        | Other        | Fine-tuning    | finance-en, poetry-zh, webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-jave-zh.                                                                                                                                                                                                                               |
-        | Vision       | Fine-tuning    | coco-en, 🔥coco-mini-en, coco-mini-en-2, capcha-images.                                                                                                                                                                                                                                                              |
-        | Audio        | Fine-tuning    | aishell1-zh, 🔥aishell1-mini-zh.                                                                                                                                                                                                                                                                                     |
+        | General      | Fine-tuning    | 🔥ruozhiba, 🔥ms-bench, 🔥alpaca-en(gpt4), 🔥alpaca-zh(gpt4), multi-alpaca, instinwild, cot-en, cot-zh, firefly-zh, instruct-en, gpt4all-en, sharegpt, tulu-v2-sft-mixture, wikipedia-zh, open-orca, sharegpt-gpt4, deepctrl-sft, coig-cqia. |
+        | Agent        | Fine-tuning    | 🔥ms-agent, 🔥ms-agent-for-agentfabric, ms-agent-multirole, 🔥toolbench-for-alpha-umi, damo-agent-zh, damo-agent-zh-mini, agent-instruct-all-en.                    |
+        | General      | Human Alignment | hh-rlhf, 🔥hh-rlhf-cn, stack-exchange-paired.                            |
+        | Code         | Fine-tuning    | code-alpaca-en, 🔥leetcode-python-en, 🔥codefuse-python-en, 🔥codefuse-evol-instruction-zh.    |
+        | Medical      | Fine-tuning    | medical-en, medical-zh, 🔥disc-med-sft-zh.               |
+        | Legal        | Fine-tuning    | lawyer-llama-zh, tigerbot-law-zh, 🔥disc-law-sft-zh.               |
+        | Math         | Fine-tuning    | 🔥blossom-math-zh, school-math-zh, open-platypus-en.                      |
+        | SQL          | Fine-tuning    | text2sql-en, 🔥sql-create-context-en.                                    |
+        | Text Generation | Fine-tuning | 🔥advertise-gen-zh, 🔥dureader-robust-zh.                            |
+        | Classification | Fine-tuning  | cmnli-zh, 🔥jd-sentiment-zh, 🔥hc3-zh, 🔥hc3-en.           |
+        | Quantization Assist | Quantization | pileval.  |
+        | Other        | Fine-tuning    | finance-en, poetry-zh, webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-jave-zh.   |
+        | Vision       | Fine-tuning    | coco-en, 🔥coco-en-mini, coco-en-2, coco-en-2-mini, capcha-images.         |
+        | Audio        | Fine-tuning    | aishell1-zh, 🔥aishell1-zh-mini.       |
         
         ### Supported Technologies
         
         | Technology Name                                              |
         | ------------------------------------------------------------ |
         | 🔥LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE MODELS](https://arxiv.org/abs/2106.09685) |
         | 🔥LoRA+: [LoRA+: Efficient Low Rank Adaptation of Large Models](https://arxiv.org/pdf/2402.12354.pdf) |
@@ -574,15 +613,16 @@
         | [Using Web-UI](docs/source_en/GetStarted/Web-ui.md)          |
         | [Using Tuners](docs/source_en/GetStarted/Tuners.md)          |
         | [LLM Inference](docs/source_en/LLM/LLM-inference.md)         |
         | [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-tuning.md)     |
         | [LLM Evaluation](docs/source_en/LLM/LLM-eval.md)     |
         | [LLM Quantization](docs/source_en/LLM/LLM-quantization.md)   |
         | [LLM Deployment](docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md) |
-        | [DPO Human Alignment Training](docs/source_en/LLM/RLHF.md)   |
+        | [DPO Human Alignment Training](docs/source_en/LLM/DPO.md)   |
+        | [ORPO Human Alignment Training](docs/source_en/LLM/ORPO.md)   |
         | [AnimateDiff Training](docs/source_en/AIGC/AnimateDiff-train-infer.md) |
         
         ### Reference Documentation
         | Document Name                                                |
         | ------------------------------------------------------------ |
         | [Command Line Arguments](docs/source_en/LLM/Command-line-parameters.md) |
         | [Supported Models and Datasets List](docs/source_en/LLM/Supported-models-datasets.md) |
@@ -628,15 +668,15 @@
           title = {SWIFT:Scalable lightWeight Infrastructure for Fine-Tuning},
           author = {The ModelScope Team},
           howpublished = {\url{https://github.com/modelscope/swift}},
           year = {2024}
         }
         ```
         
-        ## ☎ Contact Us
+        ## ☎ Wechat Group
         
         You can contact us and communicate with us by adding our WeChat group:
         
         <p align="left">
         <img src="asset/wechat.png" width="250" style="display: inline-block;">
         </p>
         
@@ -654,8 +694,9 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: llm
 Provides-Extra: aigc
 Provides-Extra: eval
+Provides-Extra: seq_parallel
 Provides-Extra: all
```

#### html2text {}

```diff
@@ -1,69 +1,106 @@
-Metadata-Version: 2.1 Name: ms-swift Version: 2.0.4 Summary: Swift: Scalable
+Metadata-Version: 2.1 Name: ms-swift Version: 2.0.5 Summary: Swift: Scalable
 lightWeight Infrastructure for Fine-Tuning Home-page: https://github.com/
 modelscope/swift Author: DAMO ModelScope teams Author-email:
 contact@modelscope.cn License: Apache License 2.0 Description: # SWIFT
 (Scalable lightWeight Infrastructure for Fine-Tuning)
 
                             [resources/banner.png]
                          _M_o_d_e_l_S_c_o_p_e_ _C_o_m_m_u_n_i_t_y_ _W_e_b_s_i_t_e
                            _ä_¸_­_æ__   ï½   English  
       [https://img.shields.io/badge/python-%E2%89%A53.8-5be.svg][https://
   img.shields.io/badge/pytorch-%E2%89%A51.12%20%7C%20%E2%89%A52.0-orange.svg]
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_m_o_d_e_l_s_c_o_p_e_-_%_E_2_%_8_9_%_A_5_1_._9_._5_-_5_D_9_1_D_4_._s_v_g_]_[_h_t_t_p_s_:_/_/
      _b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_m_s_-_s_w_i_f_t_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/
   _m_o_d_e_l_s_c_o_p_e_/_s_w_i_f_t_]_[_h_t_t_p_s_:_/_/_p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_m_s_-_s_w_i_f_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
                          _b_a_d_g_e_/_P_R_-_w_e_l_c_o_m_e_-_5_5_E_B_9_9_._s_v_g_]
+                       _[_m_o_d_e_l_s_c_o_p_e_%_2_F_s_w_i_f_t_ _|_ _T_r_e_n_d_s_h_i_f_t_]
 ## ð Table of Contents - [Introduction](#-introduction) - [News](#-news) -
 [Installation](#%EF%B8%8F-installation) - [Getting Started](#-getting-started)
 - [Documentation](#-documentation) - [License](#-License) - [Citation](#-
-citation) - [Contact Us](#-contact-us) ## ð Introduction SWIFT supports
+citation) - [WeChat Group](#-Wechat-Group) ## ð Introduction SWIFT supports
 training, inference, evaluation and deployment of nearly **200 LLMs and MLLMs**
 (multimodal large models). Developers can directly apply our framework to their
 own research and production environments to realize the complete workflow from
 model training and evaluation to application. In addition to supporting the
 lightweight training solutions provided by [PEFT](https://github.com/
 huggingface/peft), we also provide a complete **Adapters library** to support
 the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This
 adapter library can be used directly in your own custom workflow without our
 training scripts. To facilitate use by users unfamiliar with deep learning, we
 provide a Gradio web-ui for controlling training and inference, as well as
 accompanying deep learning courses and best practices for beginners.
 Additionally, we are expanding capabilities for other modalities. Currently, we
-support full-parameter training and LoRA training for AnimateDiff. ## ð News
-- 2024.04.29: Supports inference and fine-tuning of InternVL-Chat-V1.5 model.
-For best practice, you can refer to [here](https://github.com/modelscope/swift/
-tree/main/docs/source_en/Multi-Modal/internvl-best-practice.md). -
-ð¥2024.04.26: Support **LISA** and **unsloth** training! Specify `--
-lisa_activated_layers=2` to use LISA(to reduce the memory cost to 30 percent!),
-specify `--tuner_backend unsloth` to use unsloth to train a huge model(full or
-lora) with lesser memory(30 percent or lesser) and faster speed(5x)! -
-ð¥2024.04.26: Support the fine-tuning and inference of Qwen1.5-110B and
-Qwen1.5-110B-Chat model, use [this script](https://github.com/modelscope/swift/
-blob/main/examples/pytorch/llm/scripts/qwen1half_110b_chat/lora_ddp_ds/sft.sh)
-to start training! - 2024.04.24: Support for inference and fine-tuning of Phi3
-series models. Including: [phi3-4b-4k-instruct](examples/pytorch/llm/scripts/
+support full-parameter training and LoRA training for AnimateDiff. SWIFT has
+rich documentations for users, please check [here](https://github.com/
+modelscope/swift/tree/main/docs/source_en/LLM). SWIFT web-ui is available both
+on [Huggingface space](https://huggingface.co/spaces/tastelikefeet/swift) and
+[ModelScope studio](https://www.modelscope.cn/studios/iic/Scalable-lightWeight-
+Infrastructure-for-Fine-Tuning/summary), please feel free to try! ## ð News
+- 2024.05.22: Supports DeepSeek-V2-Lite series models, model_type are
+`deepseek-v2-lite` and `deepseek-v2-lite-chat` - 2024.05.22: Supports TeleChat-
+12B-v2 model with quantized version, model_type are `telechat-12b-v2` and
+`telechat-12b-v2-gptq-int4` - ð¥2024.05.21: Inference and fine-tuning support
+for MiniCPM-Llama3-V-2_5 are now available. For more details, please refer to
+[minicpm-v-2.5 Best Practice](docs/source/Multi-Modal/minicpm-v-
+2.5æä½³å®è·µ.md). - ð¥2024.05.20: Support for inferencing and fine-tuning
+cogvlm2-llama3-chinese-chat-19B, cogvlm2-llama3-chat-19B. you can refer to
+[cogvlm2 Best Practice](docs/source_en/Multi-Modal/cogvlm2-best-practice.md). -
+ð¥2024.05.17: Support peft=0.11.0. Meanwhile support 3 new tuners: `BOFT`,
+`Vera` and `Pissa`. use `--sft_type boft/vera` to use BOFT or Vera, use `--
+init_lora_weights pissa` with `--sft_type lora` to use Pissa. - 2024.05.16:
+Supports Llava-Next (Stronger) series models. For best practice, you can refer
+to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-
+Modal/llava-best-practice.md). - ð¥2024.05.13: Support Yi-1.5 series
+modelsï¼use `--model_type yi-1_5-9b-chat` to begin! - 2024.05.11: Support for
+qlora training and quantized inference using [hqq](https://github.com/mobiusml/
+hqq) and [eetq](https://github.com/NetEase-FuXi/EETQ). For more information,
+see the [LLM Quantization Documentation](https://github.com/modelscope/swift/
+tree/main/docs/source_en/LLM/LLM-quantization.md). - 2024.05.10: Support split
+a sequence to multiple GPUs to reduce memory usage. Use this feature by `pip
+install .[seq_parallel]`, then add `--sequence_parallel_size n` to your DDP
+script to begin! - 2024.05.08: Support DeepSeek-V2-Chat model, you can refer to
+[this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/
+llm/scripts/deepseek-v2-chat/lora_ddp_ds3/sft.sh).Support InternVL-Chat-V1.5-
+Int8 model, for best practice, you can refer to [here](https://github.com/
+modelscope/swift/tree/main/docs/source_en/Multi-Modal/internvl-best-
+practice.md). - ð¥2024.05.07: Supoprts **ORPO** training! See [document]
+(https://github.com/modelscope/swift/blob/main/docs/source_en/LLM/ORPO.md) to
+start training! - 2024.05.07: Supports Llava-Llama3 model from
+xtunerï¼model_type is `llava-llama-3-8b-v1_1`. - 2024.04.29: Supports
+inference and fine-tuning of InternVL-Chat-V1.5 model. For best practice, you
+can refer to [here](https://github.com/modelscope/swift/tree/main/docs/
+source_en/Multi-Modal/internvl-best-practice.md). - ð¥2024.04.26: Support
+**LISA** and **unsloth** training! Specify `--lisa_activated_layers=2` to use
+LISA(to reduce the memory cost to 30 percent!), specify `--tuner_backend
+unsloth` to use unsloth to train a huge model(full or lora) with lesser memory
+(30 percent or lesser) and faster speed(5x)! - ð¥2024.04.26: Support the
+fine-tuning and inference of Qwen1.5-110B and Qwen1.5-110B-Chat model, use
+[this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/
+llm/scripts/qwen1half_110b_chat/lora_ddp_ds/sft.sh) to start training! -
+2024.04.24: Support for inference and fine-tuning of Phi3 series models.
+Including: [phi3-4b-4k-instruct](examples/pytorch/llm/scripts/
 phi3_4b_4k_instruct/lora), phi3-4b-128k-instruct. - 2024.04.22: Support for
 inference, fine-tuning, and deployment of **chinese-llama-alpaca-2** series
 models. This includesï¼chinese-llama-2-1.3b, chinese-llama-2-7b, chinese-
 llama-2-13b, chinese-alpaca-2-1.3b, chinese-alpaca-2-7b and chinese-alpaca-2-
 13b along with their corresponding 16k and 64k long text versions. -
 2024.04.22: Support for inference and fine-tuning of Llama3 GPTQ-Int4, GPTQ-
 Int8, and AWQ series models. Support for inference and fine-tuning of chatglm3-
 6b-128k, Openbuddy-Llama3. - 2024.04.20: Support for inference, fine-tuning,
 and deployment of **Atom** series models. This includes: Atom-7B and Atom-7B-
 Chat. use [this script](https://github.com/modelscope/swift/blob/main/examples/
 pytorch/llm/scripts/atom_7b_chat/lora/sft.sh) to train. - 2024.04.19: Support
 for single-card, DDP, ZeRO2, and ZeRO3 training and inference with NPU, please
-refer to [NPU Inference and Fine-tuning Best Practices](docs/source_en/LLM/NPU-
+refer to [NPU Inference and Fine-tuning Best Practice](docs/source_en/LLM/NPU-
 best-practice.md). - 2024.04.19: Support for inference, fine-tuning, and
 deployment of **Llama3** series models. This includes: Llama-3-8B, Llama-3-8B-
 Instruct, Llama-3-70B, and Llama-3-70B-Instruct. use [this script](https://
 github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
-llama3_8b_instruct/lora/sft.sh) to train. - 2024.04.18: Supported models:
+llama3_8b_instruct/lora/sft.sh) to train. More - 2024.04.18: Supported models:
 wizardlm2-7b-awq, wizardlm2-8x22b, yi-6b-chat-awq, yi-6b-chat-int8, yi-34b-
 chat-awq, yi-34b-chat-int8. Supported `--deepspeed zero3-offload` and provided
 default zero3-offload configuration file for zero3+cpu offload usage. -
 2024.04.18: Supported compatibility with HuggingFace ecosystem using the
 environment variable `USE_HF`, switching to use models and datasets from HF.
 Please refer to the [HuggingFace ecosystem compatibility documentation](https:/
 /github.com/modelscope/swift/tree/main/docs/source_en/LLM/Compat-HF.md). -
@@ -118,15 +155,15 @@
 (https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-
 practice.md). - ð¥2024.03.25: Supports inference and fine-tuning of TeleChat-
 7b and TeleChat-12b model, use [this script](https://github.com/modelscope/
 swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start
 training! - ð¥2024.03.20: Supports inference and fine-tuning for the
 **llava** series. For best practice, you can refer to [here](https://
 github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-
-practice.md). More - ð¥2024.03.12: Support inference and fine-tuning for
+practice.md). - ð¥2024.03.12: Support inference and fine-tuning for
 **deepseek-vl** series. Best practices can be found [here](docs/source_en/
 Multi-Modal/deepseek-vl-best-practice.md). - ð¥2024.03.11: Support [GaLore]
 (https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/
 2 of the original in full-parameter training. - ð¥2024.03.10: [End-to-end
 best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning
 to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat. - ð¥2024.03.09:
 Support training and inference of MAMBA model, use [this script](https://
@@ -207,35 +244,33 @@
 /github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) for
 convenient viewing of training speed and memory usage of different models. -
 ð¥2023.12.29: Support web-ui for sft training and inference, use `swift web-
 ui` after installing ms-swift to start. - ð¥2023.12.29: Support DPO RLHF
 (Reinforcement Learning from Human Feedback) and three datasets for this task:
 AI-ModelScope/stack-exchange-paired, AI-ModelScope/hh-rlhf and AI-ModelScope/
 hh_rlhf_cn. See [documentation](https://github.com/modelscope/swift/blob/main/
-docs/source/LLM/
-LLM%E4%BA%BA%E7%B1%BB%E5%AF%B9%E9%BD%90%E8%AE%AD%E7%BB%83%E6%96%87%E6%A1%A3.md)
-to start training! - ð¥2023.12.28: Support SCEdit! This tuner can
-significantly reduce memory usage in U-Net and support low-memory controllable
-image generation (replacing ControlNet), read the section below to learn more.
-- 2023.12.23: Support [codegeex2-6b](https://github.com/modelscope/swift/tree/
-main/examples/pytorch/llm/scripts/codegeex2_6b). - 2023.12.19: Support [phi2-
-3b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
-phi2_3b). - 2023.12.18: Support VLLM for inference acceleration. - 2023.12.15:
-Support deepseek, deepseek-coder series: deepseek-7b, deepseek-7b-chat,
-deepseek-67b, deepseek-67b-chat, openbuddy-deepseek-67b-chat, deepseek-coder-
-1_3b, deepseek-coder-1_3b-instruct, deepseek-coder-6_7b, deepseek-coder-6_7b-
-instruct, deepseek-coder-33b, deepseek-coder-33b-instruct. - 2023.12.13:
-Support mistral-7b-instruct-v2, [mixtral-moe-7b](https://github.com/modelscope/
-swift/tree/main/examples/pytorch/llm/scripts/mixtral_7b_moe), [mixtral-moe-7b-
-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
-scripts/mixtral_7b_moe_instruct). - 2023.12.09: Support `freeze_parameters`
-parameter as a compromise between lora and full-parameter training.
-Corresponding sh can be found in [full_freeze_ddp](https://github.com/
-modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/
-full_freeze_ddp). Support `disable_tqdm`, `lazy_tokenize`,
+docs/source_en/LLM/DPO.md) to start training! - ð¥2023.12.28: Support SCEdit!
+This tuner can significantly reduce memory usage in U-Net and support low-
+memory controllable image generation (replacing ControlNet), read the section
+below to learn more. - 2023.12.23: Support [codegeex2-6b](https://github.com/
+modelscope/swift/tree/main/examples/pytorch/llm/scripts/codegeex2_6b). -
+2023.12.19: Support [phi2-3b](https://github.com/modelscope/swift/tree/main/
+examples/pytorch/llm/scripts/phi2_3b). - 2023.12.18: Support VLLM for inference
+acceleration. - 2023.12.15: Support deepseek, deepseek-coder series: deepseek-
+7b, deepseek-7b-chat, deepseek-67b, deepseek-67b-chat, openbuddy-deepseek-67b-
+chat, deepseek-coder-1_3b, deepseek-coder-1_3b-instruct, deepseek-coder-6_7b,
+deepseek-coder-6_7b-instruct, deepseek-coder-33b, deepseek-coder-33b-instruct.
+- 2023.12.13: Support mistral-7b-instruct-v2, [mixtral-moe-7b](https://
+github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
+mixtral_7b_moe), [mixtral-moe-7b-instruct](https://github.com/modelscope/swift/
+tree/main/examples/pytorch/llm/scripts/mixtral_7b_moe_instruct). - 2023.12.09:
+Support `freeze_parameters` parameter as a compromise between lora and full-
+parameter training. Corresponding sh can be found in [full_freeze_ddp](https://
+github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
+qwen_7b_chat/full_freeze_ddp). Support `disable_tqdm`, `lazy_tokenize`,
 `preprocess_num_proc` parameters, see [command line arguments](https://
 github.com/modelscope/swift/blob/main/docs/source/LLM/
 %E5%91%BD%E4%BB%A4%E8%A1%8C%E5%8F%82%E6%95%B0.md) for details. - 2023.12.08:
 Support [sus-34b-chat](https://github.com/modelscope/swift/tree/main/examples/
 pytorch/llm/scripts/sus_34b_chat), support yi-6b-200k, yi-34b-200k. -
 2023.12.07: Support [Multi-Node DDP training](https://github.com/modelscope/
 swift/blob/main/docs/source/LLM/
@@ -310,17 +345,20 @@
 [llm]' ``` SWIFT depends on torch>=1.13, recommend torch>=2.0.0. - Method 3:
 Use SWIFT in our Docker image ```shell # China-Hangzhou image docker pull
 registry.cn-hangzhou.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-
 cuda12.1.0-py310-torch2.1.2-tf2.14.0-1.13.1 # US-west image docker pull
 registry.us-west-1.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-
 cuda12.1.0-py310-torch2.1.2-tf2.14.0-1.13.1 ``` ## ð Getting Started This
 section introduces basic usage, see the [Documentation](#-documentation)
-section for more ways to use. ### Web-UI ```shell swift web-ui ``` ### Training
-#### Training Scripts You can refer to the following scripts to customize your
-own training script. - full: [qwen1half-7b-chat](https://github.com/modelscope/
+section for more ways to use. ### Web-UI Web-UI is a gradio-based interface for
+**zero-threshold** training and deployment. It is easy to use and perfectly
+supports multi-GPU training and deployment: ```shell SWIFT_UI_LANG=en swift
+web-ui ``` ![image.png](./docs/resources/web-ui-en.jpg) ### Training ####
+Training Scripts You can refer to the following scripts to customize your own
+training script. - full: [qwen1half-7b-chat](https://github.com/modelscope/
 swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat/full) (A100),
 [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/
 llm/scripts/qwen_7b_chat/full_mp) (2\*A100) - full+ddp+zero2: [qwen-7b-chat]
 (https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
 qwen_7b_chat/full_ddp_zero2) (4\*A100) - full+ddp+zero3: [qwen-14b-chat](https:
 //github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
 qwen_14b_chat/full_ddp_zero3) (4\*A100) - lora: [chatglm3-6b](https://
@@ -342,86 +380,91 @@
 scripts/qwen1half_7b_chat_int8/qlora) (3090) - qlora(bnb-int4): [qwen-7b-chat]
 (https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
 qwen_7b_chat/qlora) (3090) #### Supported Training Processes | Training Process
 | Training Method | |------------------|---------------------------------------
 ----------------------------------------| | Pretraining | Text Generation | |
 Fine-tuning | Single-turn/Multi-turn
 Agent Training/Self-cognition
-Multi-modal Vision/Multi-modal Speech| | Human Alignment | DPO | | Text-to-
-Image | DreamBooth, etc. | | Text-to-Video | - | #### Single GPU Training Start
-single GPU fine-tuning with the following command: LoRA: ```shell #
-Experimental Environment: A100 # GPU Memory Requirement: 20GB # Runtime: 3.1
+Multi-modal Vision/Multi-modal Speech| | Human Alignment | DPO
+ORPO | | Text-to-Image | DreamBooth, etc. | | Text-to-Video | - | #### Single
+GPU Training Start single GPU fine-tuning with the following command: LoRA:
+```shell # Experimental Environment: A100 # GPU Memory Requirement: 20GB #
+Runtime: 3.1 hours CUDA_VISIBLE_DEVICES=0 \ swift sft \ --model_type qwen1half-
+7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \
+--output_dir output \ --eval_steps 200 \ ``` Full-parameter: ```shell #
+Experimental Environment: A100 # GPU Memory Requirement: 80GB # Runtime: 2.5
 hours CUDA_VISIBLE_DEVICES=0 \ swift sft \ --model_type qwen1half-7b-chat \ --
-dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --output_dir
-output \ --eval_steps 200 \ ``` Full-parameter: ```shell # Experimental
-Environment: A100 # GPU Memory Requirement: 80GB # Runtime: 2.5 hours
-CUDA_VISIBLE_DEVICES=0 \ swift sft \ --model_type qwen1half-7b-chat \ --dataset
-blossom-math-zh \ --num_train_epochs 5 \ --sft_type full \ --output_dir output
-\ --eval_steps 500 \ ``` #### Model Parallel Training ```shell # Experimental
-Environment: 2 * A100 # GPU Memory Requirement: 10GB + 13GB # Runtime: 3.4
-hours CUDA_VISIBLE_DEVICES=0,1 \ swift sft \ --model_type qwen1half-7b-chat \ -
--dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --
-output_dir output \ ``` #### Data Parallel Training ```shell # Experimental
-Environment: 4 * A100 # GPU Memory Requirement: 4 * 30GB # Runtime: 0.8 hours
-NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type
+dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type full \ --output_dir
+output \ --eval_steps 500 \ ``` #### Model Parallel Training ```shell #
+Experimental Environment: 2 * A100 # GPU Memory Requirement: 10GB + 13GB #
+Runtime: 3.4 hours CUDA_VISIBLE_DEVICES=0,1 \ swift sft \ --model_type
 qwen1half-7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
-sft_type lora \ --output_dir output \ ``` Combining Model Parallelism and Data
-Parallelism: ```shell # Experimental Environment: 4 * A100 # GPU Memory
-Requirement: 2*14GB + 2*18GB # Runtime: 1.7 hours NPROC_PER_NODE=2 \
-CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type qwen1half-7b-chat \ --
-dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --output_dir
-output \ ``` #### Deepspeed Training Deepspeed supports training of quantized
-GPTQ and AWQ models. ZeRO2: ```shell # Experimental Environment: 4 * A100 # GPU
-Memory Requirement: 4 * 21GB # Runtime: 0.9 hours NPROC_PER_NODE=4 \
+sft_type lora \ --output_dir output \ ``` #### Data Parallel Training ```shell
+# Experimental Environment: 4 * A100 # GPU Memory Requirement: 4 * 30GB #
+Runtime: 0.8 hours NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft
+\ --model_type qwen1half-7b-chat \ --dataset blossom-math-zh \ --
+num_train_epochs 5 \ --sft_type lora \ --output_dir output \ ``` Combining
+Model Parallelism and Data Parallelism: ```shell # Experimental Environment: 4
+* A100 # GPU Memory Requirement: 2*14GB + 2*18GB # Runtime: 1.7 hours
+NPROC_PER_NODE=2 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type
+qwen1half-7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
+sft_type lora \ --output_dir output \ ``` #### Deepspeed Training Deepspeed
+supports training of quantized GPTQ and AWQ models. ZeRO2: ```shell #
+Experimental Environment: 4 * A100 # GPU Memory Requirement: 4 * 21GB #
+Runtime: 0.9 hours NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft
+\ --model_type qwen1half-7b-chat \ --dataset blossom-math-zh \ --
+num_train_epochs 5 \ --sft_type lora \ --output_dir output \ --deepspeed
+default-zero2 \ ``` ZeRO3: ```shell # Experimental Environment: 4 * A100 # GPU
+Memory Requirement: 4 * 19GB # Runtime: 3.2 hours NPROC_PER_NODE=4 \
 CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type qwen1half-7b-chat \ --
 dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --output_dir
-output \ --deepspeed default-zero2 \ ``` ZeRO3: ```shell # Experimental
-Environment: 4 * A100 # GPU Memory Requirement: 4 * 19GB # Runtime: 3.2 hours
-NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type
-qwen1half-7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
-sft_type lora \ --output_dir output \ --deepspeed default-zero3 \ ``` ZeRO3-
-Offload: ```shell # Experimental Environment: 4 * A100 # GPU Memory
-Requirement: 4 * 12GB # Runtime: 60 hours NPROC_PER_NODE=4 \
-CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_id_or_path AI-ModelScope/
-WizardLM-2-8x22B \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
-sft_type lora \ --output_dir output \ --deepspeed zero3-offload \ ``` ####
-Multi-node Multi-GPU ```shell # node0 CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 \
-NNODES=2 \ NODE_RANK=0 \ MASTER_ADDR=127.0.0.1 \ NPROC_PER_NODE=8 \ swift sft \
---model_id_or_path qwen1half-32b-chat \ --sft_type full \ --dataset blossom-
-math-zh \ --output_dir output \ --deepspeed default-zero3 \ # node1
+output \ --deepspeed default-zero3 \ ``` ZeRO3-Offload: ```shell # Experimental
+Environment: 4 * A100 # GPU Memory Requirement: 4 * 12GB # Runtime: 60 hours
+NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --
+model_id_or_path AI-ModelScope/WizardLM-2-8x22B \ --dataset blossom-math-zh \ -
+-num_train_epochs 5 \ --sft_type lora \ --output_dir output \ --deepspeed
+zero3-offload \ ``` #### Multi-node Multi-GPU ```shell # node0
+CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 \ NNODES=2 \ NODE_RANK=0 \
+MASTER_ADDR=127.0.0.1 \ NPROC_PER_NODE=8 \ swift sft \ --model_id_or_path
+qwen1half-32b-chat \ --sft_type full \ --dataset blossom-math-zh \ --output_dir
+output \ --deepspeed default-zero3 \ # node1
 CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 \ NNODES=2 \ NODE_RANK=1 \
 MASTER_ADDR=xxx.xxx.xxx.xxx \ NPROC_PER_NODE=8 \ swift sft \ --model_id_or_path
 qwen1half-32b-chat \ --sft_type full \ --dataset blossom-math-zh \ --output_dir
-output \ --deepspeed default-zero3 \ ``` ### Inference Original model: ```shell
-CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat # use VLLM
-CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat \ --
-infer_backend vllm --max_model_len 8192 ``` LoRA fine-tuned: ```shell
-CUDA_VISIBLE_DEVICES=0 swift infer --ckpt_dir xxx/checkpoint-xxx --
-load_dataset_config true # use VLLM CUDA_VISIBLE_DEVICES=0 swift infer \ --
-ckpt_dir xxx/checkpoint-xxx --load_dataset_config true \ --merge_lora true --
-infer_backend vllm --max_model_len 8192 ``` ### Evaluation ```shell
-CUDA_VISIBLE_DEVICES=0 swift eval --model_type qwen1half-7b-chat --eval_dataset
-mmlu ceval ``` ### Export Original model: ```shell CUDA_VISIBLE_DEVICES=0 swift
-export --model_type qwen1half-7b-chat \ --quant_bits 4 --quant_method awq ```
-LoRA fine-tuned: ```shell CUDA_VISIBLE_DEVICES=0 swift export \ --ckpt_dir xxx/
-checkpoint-xxx --load_dataset_config true \ --quant_method awq --quant_bits 4 \
---merge_lora true \ ``` ### Deployment Original model: ```shell
-CUDA_VISIBLE_DEVICES=0 swift deploy --model_type qwen1half-7b-chat #
-ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0 swift deploy --model_type qwen1half-7b-
-chat \ --infer_backend vllm --max_model_len 8192 ``` LoRA fine-tuned: ```shell
-CUDA_VISIBLE_DEVICES=0 swift deploy --ckpt_dir xxx/checkpoint-xxx #
-ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0 swift deploy \ --ckpt_dir xxx/
-checkpoint-xxx --merge_lora true \ --infer_backend vllm --max_model_len 8192
-``` ### Supported Models The complete list of supported models and datasets can
-be found at [Supported Models and Datasets List](docs/source_en/LLM/Supported-
-models-datasets.md). #### LLMs | Model Type | Model Introduction | Language |
-Model Size | Model Type | |------------------------------------------------|---
----------------------------------------------------------------------|---------
------------|----------------------------------------|--------------------------
------------------ | | Qwen
+output \ --deepspeed default-zero3 \ ``` ##### AliYun-DLC multi-node training
+In DLC product, WORLD_SIZE is the node number, RANK is the node index, this is
+different from the definition of torchrun. ```shell NNODES=$WORLD_SIZE \
+NODE_RANK=$RANK \ swift sft \ --model_id_or_path qwen1half-32b-chat \ --
+sft_type full \ --dataset blossom-math-zh \ --output_dir output \ --deepspeed
+default-zero3 ``` ### Inference Original model: ```shell CUDA_VISIBLE_DEVICES=0
+swift infer --model_type qwen1half-7b-chat # use VLLM CUDA_VISIBLE_DEVICES=0
+swift infer --model_type qwen1half-7b-chat \ --infer_backend vllm --
+max_model_len 8192 ``` LoRA fine-tuned: ```shell CUDA_VISIBLE_DEVICES=0 swift
+infer --ckpt_dir xxx/checkpoint-xxx --load_dataset_config true # use VLLM
+CUDA_VISIBLE_DEVICES=0 swift infer \ --ckpt_dir xxx/checkpoint-xxx --
+load_dataset_config true \ --merge_lora true --infer_backend vllm --
+max_model_len 8192 ``` ### Evaluation ```shell CUDA_VISIBLE_DEVICES=0 swift
+eval --model_type qwen1half-7b-chat --eval_dataset mmlu ceval ``` ### Export
+Original model: ```shell CUDA_VISIBLE_DEVICES=0 swift export --model_type
+qwen1half-7b-chat \ --quant_bits 4 --quant_method awq ``` LoRA fine-tuned:
+```shell CUDA_VISIBLE_DEVICES=0 swift export \ --ckpt_dir xxx/checkpoint-xxx --
+load_dataset_config true \ --quant_method awq --quant_bits 4 \ --merge_lora
+true \ ``` ### Deployment Original model: ```shell CUDA_VISIBLE_DEVICES=0 swift
+deploy --model_type qwen1half-7b-chat # ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0
+swift deploy --model_type qwen1half-7b-chat \ --infer_backend vllm --
+max_model_len 8192 ``` LoRA fine-tuned: ```shell CUDA_VISIBLE_DEVICES=0 swift
+deploy --ckpt_dir xxx/checkpoint-xxx # ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0
+swift deploy \ --ckpt_dir xxx/checkpoint-xxx --merge_lora true \ --
+infer_backend vllm --max_model_len 8192 ``` ### Supported Models The complete
+list of supported models and datasets can be found at [Supported Models and
+Datasets List](docs/source_en/LLM/Supported-models-datasets.md). #### LLMs |
+Model Type | Model Introduction | Language | Model Size | Model Type | |-------
+-----------------------------------------|-------------------------------------
+-----------------------------------|--------------------|----------------------
+------------------|------------------------------------------- | | Qwen
 Qwen1.5 | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM) |
 Chinese
 English | 0.5B-110B
 including quantized versions | base model
 chat model
 MoE model
 code model | | ChatGLM2
@@ -447,31 +490,32 @@
 chat model | | LLaMA3 | [LLaMA3 series models](https://github.com/meta-llama/
 llama3) | English | 8B-70B
 including quantized versions | base model
 chat model | | Mistral
 Mixtral | [Mistral series models](https://github.com/mistralai/mistral-src) |
 English | 7B-22B | base model
 instruct model
-MoE model | | YI | [01AI's YI series models](https://github.com/01-ai) |
-Chinese
+MoE model | | Yi
+Yi1.5 | [01AI's YI series models](https://github.com/01-ai) | Chinese
 English | 6B-34B
 including quantized | base model
 chat model
 long text model | | InternLM
 InternLM2
 InternLM2-Math | [Pujiang AI Lab InternLM series models](https://github.com/
 InternLM/InternLM) | Chinese
 English | 1.8B-20B | base model
 chat model
 math model | | DeepSeek
 DeepSeek-MoE
 DeepSeek-Coder
-DeepSeek-Math | [DeepSeek series models](https://github.com/deepseek-ai) |
+DeepSeek-Math
+DeepSeek-V2 | [DeepSeek series models](https://github.com/deepseek-ai) |
 Chinese
-English | 1.3B-67B | base model
+English | 1.3B-236B | base model
 chat model
 MoE model
 code model
 math model | | MAMBA | [MAMBA temporal convolution model](https://github.com/
 state-spaces/mamba) | English | 130M-2.8B | base model | | Gemma | [Google
 Gemma series models](https://github.com/google/gemma_pytorch) | English | 2B-7B
 | base model
@@ -544,109 +588,113 @@
 English | 7B | base model
 chat model | | YI-VL | [01AI's YI series vision models](https://github.com/01-
 ai) | Chinese
 English | 6B-34B | chat model | | XComposer2 | [Pujiang AI Lab InternLM vision
 model](https://github.com/InternLM/InternLM) | Chinese
 English | 7B | chat model | | DeepSeek-VL | [DeepSeek series vision models]
 (https://github.com/deepseek-ai) | Chinese
-English | 1.3B-7B | chat model | | MiniCPM-V | [OpenBmB MiniCPM vision model]
-(https://github.com/OpenBMB/MiniCPM) | Chinese
-English | 3B | chat model | | CogVLM
+English | 1.3B-7B | chat model | | MiniCPM-V
+MiniCPM-V-2
+MiniCPM-V-2_5 | [OpenBmB MiniCPM vision model](https://github.com/OpenBMB/
+MiniCPM) | Chinese
+English | 3B-9B | chat model | | CogVLM
+CogVLM2
 CogAgent | [Zhipu ChatGLM visual QA and Agent model](https://github.com/THUDM/
-) | English | 17B-18B | chat model | | Llava | [Llava series models](https://
-github.com/haotian-liu/LLaVA) | English | 7B-34B | chat model | | mPLUG-Owl |
-[mPLUG-Owl series models](https://github.com/X-PLUG/mPLUG-Owl) | English | 11B
-| chat model | | InternVL | [InternVL](https://github.com/OpenGVLab/InternVL) |
-Chinese
-English | 25.5B | chat model | #### Diffusion Models | Model Type | Model
-Introduction | Language | Model Type | |---------------------|-----------------
------------------------------------------------------|----------|--------------
----- | | AnimateDiff | [AnimateDiff animation model](https://github.com/guoyww/
-AnimateDiff) | English | text-to-video | | SD1.5/SD2.0/SDXL | [StabilityAI
-series diffusion models](https://github.com/Stability-AI) | English | text-to-
-image | ### Supported Open Source Datasets | Dataset Type | Training Task |
-Documentation | |--------------|:---------------|------------------------------
---------------------------------- | | General | Fine-tuning | ð¥ruozhiba,
-ð¥ms-bench, ð¥ms-bench-mini, ð¥alpaca-en(gpt4), ð¥alpaca-zh(gpt4),
-multi-alpaca-all, instinwild-en, instinwild-zh, cot-en, cot-zh, firefly-all-zh,
-instruct-en, gpt4all-en, sharegpt-en, sharegpt-zh, tulu-v2-sft-mixture,
-wikipedia-zh, open-orca, open-orca-gpt4, sharegpt-gpt4, ð¥sharegpt-gpt4-mini.
-| | Agent | Fine-tuning | ð¥ms-agent, ms-agent-for-agentfabric-default, ms-
-agent-for-agentfabric-addition, damo-mini-agent-zh, damo-agent-zh, agent-
-instruct-all-en. | | General | Human Alignment | ð¥hh-rlhf-cn, stack-
-exchange-paired, hh-rlhf-harmless-base, hh-rlhf-helpful-base, hh-rlhf-helpful-
-online, hh-rlhf-helpful-rejection-sampled, hh-rlhf-red-team-attempts, hh-rlhf-
-cn-harmless-base-cn, hh-rlhf-cn-helpful-base-cn, hh-rlhf-cn-harmless-base-en,
-hh-rlhf-cn-helpful-base-en. | | Code | Fine-tuning | code-alpaca-en,
-ð¥leetcode-python-en, ð¥codefuse-python-en, ð¥codefuse-evol-instruction-
-zh. | | Medical | Fine-tuning | medical-en, medical-zh, medical-mini-zh,
-ð¥disc-med-sft-zh. | | Legal | Fine-tuning | lawyer-llama-zh, tigerbot-law-
-zh, ð¥disc-law-sft-zh. | | Math | Fine-tuning | ð¥blossom-math-zh, school-
-math-zh, open-platypus-en. | | SQL | Fine-tuning | text2sql-en, ð¥sql-create-
-context-en. | | Text Generation | Fine-tuning | ð¥advertise-gen-zh,
-ð¥dureader-robust-zh. | | Classification | Fine-tuning | cmnli-zh, ð¥cmnli-
-mini-zh, ð¥jd-sentiment-zh, ð¥hc3-zh, ð¥hc3-en. | | Quantization Assist |
-Quantization | pileval. | | Other | Fine-tuning | finance-en, poetry-zh,
-webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-jave-zh. | | Vision |
-Fine-tuning | coco-en, ð¥coco-mini-en, coco-mini-en-2, capcha-images. | |
-Audio | Fine-tuning | aishell1-zh, ð¥aishell1-mini-zh. | ### Supported
-Technologies | Technology Name | | --------------------------------------------
----------------- | | ð¥LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE
-MODELS](https://arxiv.org/abs/2106.09685) | | ð¥LoRA+: [LoRA+: Efficient Low
-Rank Adaptation of Large Models](https://arxiv.org/pdf/2402.12354.pdf) | |
-ð¥GaLore:[GaLore: Memory-Efficient LLM Training by Gradient Low-Rank
-Projection](https://arxiv.org/abs/2403.03507) | | ð¥LISA: [LISA: Layerwise
-Importance Sampling for Memory-Efficient Large Language Model Fine-Tuning]
-(https://arxiv.org/abs/2403.17919) | | ð¥UnSloth: https://github.com/
-unslothai/unsloth | | ð¥LLaMA PRO: [LLAMA PRO: Progressive LLaMA with Block
-Expansion](https://arxiv.org/pdf/2401.02415.pdf) | | ð¥SCEdit: [SCEdit:
-Efficient and Controllable Image Diffusion Generation via Skip Connection
-Editing](https://arxiv.org/abs/2312.11392) < [arXiv](https://arxiv.org/abs/
-2312.11392) \ | | ð¥NEFTune: [Noisy Embeddings Improve Instruction
-Finetuning](https://arxiv.org/abs/2310.05914) | | LongLoRA: [Efficient Fine-
-tuning of Long-Context Large Language Models](https://arxiv.org/abs/2309.12307)
-| | Adapter: [Parameter-Efficient Transfer Learning for NLP](http://arxiv.org/
-abs/1902.00751) | | Vision Prompt Tuning: [Visual Prompt Tuning](https://
-arxiv.org/abs/2203.12119) | | Side: [Side-Tuning: A Baseline for Network
-Adaptation via Additive Side Networks](https://arxiv.org/abs/1912.13503) | |
-Res-Tuning: [Res-Tuning: A Flexible and Efficient Tuning Paradigm via Unbinding
-Tuner from Backbone](https://arxiv.org/abs/2310.19859) < [arXiv](https://
-arxiv.org/abs/2310.19859) \ | | Tuners provided by [PEFT](https://github.com/
-huggingface/peft), such as IA3, AdaLoRA, etc. | ### Supported Hardware |
-Hardware Environment | Notes | |--------------------------------|--------------
------------------------------------| | CPU | | | RTX 20/30/40 series, etc. |
-After 30 series, BF16 and FlashAttn can be used | | Computing cards T4/V100,
-etc. | BF16 and FlashAttn not supported | | Computing cards A10/A100, etc. |
-Support BF16 and FlashAttn | | Huawei Ascend NPU | | ## ð Documentation ###
-Documentation Compiling ```shell make docs # Check docs/build/html/index.html
-in web-browser ``` ### User Guide | Document Name | | -------------------------
------------------------------------ | | [Using Web-UI](docs/source_en/
-GetStarted/Web-ui.md) | | [Using Tuners](docs/source_en/GetStarted/Tuners.md) |
-| [LLM Inference](docs/source_en/LLM/LLM-inference.md) | | [LLM Fine-tuning]
-(docs/source_en/LLM/LLM-fine-tuning.md) | | [LLM Evaluation](docs/source_en/
-LLM/LLM-eval.md) | | [LLM Quantization](docs/source_en/LLM/LLM-quantization.md)
-| | [LLM Deployment](docs/source_en/LLM/VLLM-inference-acceleration-and-
-deployment.md) | | [DPO Human Alignment Training](docs/source_en/LLM/RLHF.md) |
-| [AnimateDiff Training](docs/source_en/AIGC/AnimateDiff-train-infer.md) | ###
-Reference Documentation | Document Name | | -----------------------------------
-------------------------- | | [Command Line Arguments](docs/source_en/LLM/
-Command-line-parameters.md) | | [Supported Models and Datasets List](docs/
-source_en/LLM/Supported-models-datasets.md) | | [Customizing New Models and
-Datasets](docs/source_en/LLM/Customization.md) | | [Runtime Speed and Memory
-Benchmark](docs/source_en/LLM/Benchmark.md) | ### Best Practices | Best
-Practices Name | | -----------------------------------------------------------
-- | | [Agent Fine-Tuning Best Practice](docs/source_en/LLM/Agent-best-
-practice.md) | | [Self-Cognition Fine-Tuning Best Practice](docs/source_en/LLM/
-Self-cognition-best-practice.md) | | [Qwen1.5 Best Practice](docs/source_en/
-LLM/Qwen1.5-best-practice.md) | | [Multi-Modal Model Training Best Practice]
-(docs/source_en/Multi-Modal/index.md) | | [NPU Best Practice](docs/source_en/
-LLM/NPU-best-practice.md) | ### Deep Learning Tutorials | Tutorial Name | |----
----------------------------------------------------------- | | [Introduction to
-Deep Learning](https://github.com/modelscope/modelscope-classroom/blob/main/
-LLM-tutorial/
+) | Chinese
+English | 17B-19B | chat model | | Llava | [Llava series models](https://
+github.com/haotian-liu/LLaVA) | English | 7B-34B | chat model | | Llava-Next |
+[Llava-Next series models](https://github.com/LLaVA-VL/LLaVA-NeXT) | Chinese
+English | 8B-110B | chat model | | mPLUG-Owl | [mPLUG-Owl series models](https:
+//github.com/X-PLUG/mPLUG-Owl) | English | 11B | chat model | | InternVL |
+[InternVL](https://github.com/OpenGVLab/InternVL) | Chinese
+English | 25.5B
+including quantized version | chat model | | Llava-llama3 | [xtuner](https://
+huggingface.co/xtuner/llava-llama-3-8b-v1_1-transformers) | English | 8B | chat
+model | #### Diffusion Models | Model Type | Model Introduction | Language |
+Model Type | |---------------------|-------------------------------------------
+---------------------------|----------|------------------ | | AnimateDiff |
+[AnimateDiff animation model](https://github.com/guoyww/AnimateDiff) | English
+| text-to-video | | SD1.5/SD2.0/SDXL | [StabilityAI series diffusion models]
+(https://github.com/Stability-AI) | English | text-to-image | ### Supported
+Open Source Datasets | Dataset Type | Training Task | Documentation | |--------
+------|:---------------|-------------------------------------------------------
+-------- | | General | Fine-tuning | ð¥ruozhiba, ð¥ms-bench, ð¥alpaca-en
+(gpt4), ð¥alpaca-zh(gpt4), multi-alpaca, instinwild, cot-en, cot-zh, firefly-
+zh, instruct-en, gpt4all-en, sharegpt, tulu-v2-sft-mixture, wikipedia-zh, open-
+orca, sharegpt-gpt4, deepctrl-sft, coig-cqia. | | Agent | Fine-tuning | ð¥ms-
+agent, ð¥ms-agent-for-agentfabric, ms-agent-multirole, ð¥toolbench-for-
+alpha-umi, damo-agent-zh, damo-agent-zh-mini, agent-instruct-all-en. | |
+General | Human Alignment | hh-rlhf, ð¥hh-rlhf-cn, stack-exchange-paired. | |
+Code | Fine-tuning | code-alpaca-en, ð¥leetcode-python-en, ð¥codefuse-
+python-en, ð¥codefuse-evol-instruction-zh. | | Medical | Fine-tuning |
+medical-en, medical-zh, ð¥disc-med-sft-zh. | | Legal | Fine-tuning | lawyer-
+llama-zh, tigerbot-law-zh, ð¥disc-law-sft-zh. | | Math | Fine-tuning |
+ð¥blossom-math-zh, school-math-zh, open-platypus-en. | | SQL | Fine-tuning |
+text2sql-en, ð¥sql-create-context-en. | | Text Generation | Fine-tuning |
+ð¥advertise-gen-zh, ð¥dureader-robust-zh. | | Classification | Fine-tuning
+| cmnli-zh, ð¥jd-sentiment-zh, ð¥hc3-zh, ð¥hc3-en. | | Quantization
+Assist | Quantization | pileval. | | Other | Fine-tuning | finance-en, poetry-
+zh, webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-jave-zh. | | Vision
+| Fine-tuning | coco-en, ð¥coco-en-mini, coco-en-2, coco-en-2-mini, capcha-
+images. | | Audio | Fine-tuning | aishell1-zh, ð¥aishell1-zh-mini. | ###
+Supported Technologies | Technology Name | | ----------------------------------
+-------------------------- | | ð¥LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE
+LANGUAGE MODELS](https://arxiv.org/abs/2106.09685) | | ð¥LoRA+: [LoRA+:
+Efficient Low Rank Adaptation of Large Models](https://arxiv.org/pdf/
+2402.12354.pdf) | | ð¥GaLore:[GaLore: Memory-Efficient LLM Training by
+Gradient Low-Rank Projection](https://arxiv.org/abs/2403.03507) | | ð¥LISA:
+[LISA: Layerwise Importance Sampling for Memory-Efficient Large Language Model
+Fine-Tuning](https://arxiv.org/abs/2403.17919) | | ð¥UnSloth: https://
+github.com/unslothai/unsloth | | ð¥LLaMA PRO: [LLAMA PRO: Progressive LLaMA
+with Block Expansion](https://arxiv.org/pdf/2401.02415.pdf) | | ð¥SCEdit:
+[SCEdit: Efficient and Controllable Image Diffusion Generation via Skip
+Connection Editing](https://arxiv.org/abs/2312.11392) < [arXiv](https://
+arxiv.org/abs/2312.11392) \ | | ð¥NEFTune: [Noisy Embeddings Improve
+Instruction Finetuning](https://arxiv.org/abs/2310.05914) | | LongLoRA:
+[Efficient Fine-tuning of Long-Context Large Language Models](https://
+arxiv.org/abs/2309.12307) | | Adapter: [Parameter-Efficient Transfer Learning
+for NLP](http://arxiv.org/abs/1902.00751) | | Vision Prompt Tuning: [Visual
+Prompt Tuning](https://arxiv.org/abs/2203.12119) | | Side: [Side-Tuning: A
+Baseline for Network Adaptation via Additive Side Networks](https://arxiv.org/
+abs/1912.13503) | | Res-Tuning: [Res-Tuning: A Flexible and Efficient Tuning
+Paradigm via Unbinding Tuner from Backbone](https://arxiv.org/abs/2310.19859) <
+[arXiv](https://arxiv.org/abs/2310.19859) \ | | Tuners provided by [PEFT]
+(https://github.com/huggingface/peft), such as IA3, AdaLoRA, etc. | ###
+Supported Hardware | Hardware Environment | Notes | |--------------------------
+------|-------------------------------------------------| | CPU | | | RTX 20/
+30/40 series, etc. | After 30 series, BF16 and FlashAttn can be used | |
+Computing cards T4/V100, etc. | BF16 and FlashAttn not supported | | Computing
+cards A10/A100, etc. | Support BF16 and FlashAttn | | Huawei Ascend NPU | | ##
+ð Documentation ### Documentation Compiling ```shell make docs # Check docs/
+build/html/index.html in web-browser ``` ### User Guide | Document Name | | ---
+--------------------------------------------------------- | | [Using Web-UI]
+(docs/source_en/GetStarted/Web-ui.md) | | [Using Tuners](docs/source_en/
+GetStarted/Tuners.md) | | [LLM Inference](docs/source_en/LLM/LLM-inference.md)
+| | [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-tuning.md) | | [LLM
+Evaluation](docs/source_en/LLM/LLM-eval.md) | | [LLM Quantization](docs/
+source_en/LLM/LLM-quantization.md) | | [LLM Deployment](docs/source_en/LLM/
+VLLM-inference-acceleration-and-deployment.md) | | [DPO Human Alignment
+Training](docs/source_en/LLM/DPO.md) | | [ORPO Human Alignment Training](docs/
+source_en/LLM/ORPO.md) | | [AnimateDiff Training](docs/source_en/AIGC/
+AnimateDiff-train-infer.md) | ### Reference Documentation | Document Name | | -
+----------------------------------------------------------- | | [Command Line
+Arguments](docs/source_en/LLM/Command-line-parameters.md) | | [Supported Models
+and Datasets List](docs/source_en/LLM/Supported-models-datasets.md) | |
+[Customizing New Models and Datasets](docs/source_en/LLM/Customization.md) | |
+[Runtime Speed and Memory Benchmark](docs/source_en/LLM/Benchmark.md) | ###
+Best Practices | Best Practices Name | | --------------------------------------
+---------------------- | | [Agent Fine-Tuning Best Practice](docs/source_en/
+LLM/Agent-best-practice.md) | | [Self-Cognition Fine-Tuning Best Practice]
+(docs/source_en/LLM/Self-cognition-best-practice.md) | | [Qwen1.5 Best
+Practice](docs/source_en/LLM/Qwen1.5-best-practice.md) | | [Multi-Modal Model
+Training Best Practice](docs/source_en/Multi-Modal/index.md) | | [NPU Best
+Practice](docs/source_en/LLM/NPU-best-practice.md) | ### Deep Learning
+Tutorials | Tutorial Name | |--------------------------------------------------
+------------ | | [Introduction to Deep Learning](https://github.com/modelscope/
+modelscope-classroom/blob/main/LLM-tutorial/
 A.%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0%E5%85%A5%E9%97%A8%E4%BB%8B%E7%BB%8D.md)
 | | [Large Model Basics](https://github.com/modelscope/modelscope-classroom/
 blob/main/LLM-tutorial/
 B.%E9%AD%94%E6%90%AD%E7%A4%BE%E5%8C%BA%E5%92%8CLLM%E5%A4%A7%E6%A8%A1%E5%9E%8B%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md)
 | | [Prompt Engineering](https://github.com/modelscope/modelscope-classroom/
 blob/main/LLM-tutorial/C.%E6%8F%90%E7%A4%BA%E8%AF%8D%E5%B7%A5%E7%A8%8B-
 prompt%20engineering.md) | | [Transformer Architecture Introduction](https://
@@ -668,20 +716,21 @@
 K.%E5%A4%A7%E6%A8%A1%E5%9E%8B%E8%87%AA%E5%8A%A8%E8%AF%84%E4%BC%B0%E7%90%86%E8%AE%BA%E5%92%8C%E5%AE%9E%E6%88%98-
 -LLM%20Automatic%20Evaluation.md) | ## ð License This framework is licensed
 under the [Apache License (Version 2.0)](https://github.com/modelscope/
 modelscope/blob/master/LICENSE). For models and datasets, please refer to the
 original resource page and follow the corresponding License. ## ð Citation
 ```bibtex @Misc{swift, title = {SWIFT:Scalable lightWeight Infrastructure for
 Fine-Tuning}, author = {The ModelScope Team}, howpublished = {\url{https://
-github.com/modelscope/swift}}, year = {2024} } ``` ## â Contact Us You can
+github.com/modelscope/swift}}, year = {2024} } ``` ## â Wechat Group You can
 contact us and communicate with us by adding our WeChat group:
 [asset/wechat.png]
 ## Star History [![Star History Chart](https://api.star-history.com/
 svg?repos=modelscope/swift&type=Date)](https://star-history.com/#modelscope/
 swift&Date) Keywords: python,petl,efficient tuners Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown Provides-
-Extra: llm Provides-Extra: aigc Provides-Extra: eval Provides-Extra: all
+Extra: llm Provides-Extra: aigc Provides-Extra: eval Provides-Extra:
+seq_parallel Provides-Extra: all
```

### Comparing `ms-swift-2.0.4/README.md` & `ms-swift-2.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -17,41 +17,63 @@
 <a href="https://github.com/modelscope/modelscope/"><img src="https://img.shields.io/badge/modelscope-%E2%89%A51.9.5-5D91D4.svg"></a>
 <a href="https://pypi.org/project/ms-swift/"><img src="https://badge.fury.io/py/ms-swift.svg"></a>
 <a href="https://github.com/modelscope/swift/blob/main/LICENSE"><img src="https://img.shields.io/github/license/modelscope/swift"></a>
 <a href="https://pepy.tech/project/ms-swift"><img src="https://pepy.tech/badge/ms-swift"></a>
 <a href="https://github.com/modelscope/swift/pulls"><img src="https://img.shields.io/badge/PR-welcome-55EB99.svg"></a>
 </p>
 
+<p align="center">
+<a href="https://trendshift.io/repositories/6427" target="_blank"><img src="https://trendshift.io/api/badge/repositories/6427" alt="modelscope%2Fswift | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>
+</p>
+
 ## 📖 Table of Contents
 - [Introduction](#-introduction)
 - [News](#-news)
 - [Installation](#%EF%B8%8F-installation)
 - [Getting Started](#-getting-started)
 - [Documentation](#-documentation)
 - [License](#-License)
 - [Citation](#-citation)
-- [Contact Us](#-contact-us)
+- [WeChat Group](#-Wechat-Group)
 
 ## 📝 Introduction
 SWIFT supports training, inference, evaluation and deployment of nearly **200 LLMs and MLLMs** (multimodal large models). Developers can directly apply our framework to their own research and production environments to realize the complete workflow from model training and evaluation to application. In addition to supporting the lightweight training solutions provided by [PEFT](https://github.com/huggingface/peft), we also provide a complete **Adapters library** to support the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This adapter library can be used directly in your own custom workflow without our training scripts.
 
 To facilitate use by users unfamiliar with deep learning, we provide a Gradio web-ui for controlling training and inference, as well as accompanying deep learning courses and best practices for beginners.
 
 Additionally, we are expanding capabilities for other modalities. Currently, we support full-parameter training and LoRA training for AnimateDiff.
 
+SWIFT has rich documentations for users, please check [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM).
+
+SWIFT web-ui is available both on [Huggingface space](https://huggingface.co/spaces/tastelikefeet/swift) and [ModelScope studio](https://www.modelscope.cn/studios/iic/Scalable-lightWeight-Infrastructure-for-Fine-Tuning/summary), please feel free to try!
+
 ## 🎉 News
+- 2024.05.22: Supports DeepSeek-V2-Lite series models, model_type are `deepseek-v2-lite` and `deepseek-v2-lite-chat`
+- 2024.05.22: Supports TeleChat-12B-v2 model with quantized version, model_type are `telechat-12b-v2` and `telechat-12b-v2-gptq-int4`
+- 🔥2024.05.21: Inference and fine-tuning support for MiniCPM-Llama3-V-2_5 are now available. For more details, please refer to [minicpm-v-2.5 Best Practice](docs/source/Multi-Modal/minicpm-v-2.5最佳实践.md).
+- 🔥2024.05.20: Support for inferencing and fine-tuning cogvlm2-llama3-chinese-chat-19B, cogvlm2-llama3-chat-19B. you can refer to [cogvlm2 Best Practice](docs/source_en/Multi-Modal/cogvlm2-best-practice.md).
+- 🔥2024.05.17: Support peft=0.11.0. Meanwhile support 3 new tuners: `BOFT`, `Vera` and `Pissa`. use `--sft_type boft/vera` to use BOFT or Vera, use `--init_lora_weights pissa` with `--sft_type lora` to use Pissa.
+- 2024.05.16: Supports Llava-Next (Stronger) series models. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-practice.md).
+- 🔥2024.05.13: Support Yi-1.5 series models，use `--model_type yi-1_5-9b-chat` to begin!
+- 2024.05.11: Support for qlora training and quantized inference using [hqq](https://github.com/mobiusml/hqq) and [eetq](https://github.com/NetEase-FuXi/EETQ). For more information, see the [LLM Quantization Documentation](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/LLM-quantization.md).
+- 2024.05.10: Support split a sequence to multiple GPUs to reduce memory usage. Use this feature by `pip install .[seq_parallel]`, then add `--sequence_parallel_size n` to your DDP script to begin!
+- 2024.05.08: Support DeepSeek-V2-Chat model, you can refer to [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/deepseek-v2-chat/lora_ddp_ds3/sft.sh).Support InternVL-Chat-V1.5-Int8 model, for best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/internvl-best-practice.md).
+- 🔥2024.05.07: Supoprts **ORPO** training! See [document](https://github.com/modelscope/swift/blob/main/docs/source_en/LLM/ORPO.md) to start training!
+- 2024.05.07: Supports Llava-Llama3 model from xtuner，model_type is `llava-llama-3-8b-v1_1`.
 - 2024.04.29: Supports inference and fine-tuning of InternVL-Chat-V1.5 model. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/internvl-best-practice.md).
 - 🔥2024.04.26: Support **LISA** and **unsloth** training! Specify `--lisa_activated_layers=2` to use LISA(to reduce the memory cost to 30 percent!), specify `--tuner_backend unsloth` to use unsloth to train a huge model(full or lora) with lesser memory(30 percent or lesser) and faster speed(5x)!
 - 🔥2024.04.26: Support the fine-tuning and inference of Qwen1.5-110B and Qwen1.5-110B-Chat model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_110b_chat/lora_ddp_ds/sft.sh) to start training!
 - 2024.04.24: Support for inference and fine-tuning of Phi3 series models. Including: [phi3-4b-4k-instruct](examples/pytorch/llm/scripts/phi3_4b_4k_instruct/lora), phi3-4b-128k-instruct.
 - 2024.04.22: Support for inference, fine-tuning, and deployment of **chinese-llama-alpaca-2** series models. This includes：chinese-llama-2-1.3b, chinese-llama-2-7b, chinese-llama-2-13b, chinese-alpaca-2-1.3b, chinese-alpaca-2-7b and chinese-alpaca-2-13b along with their corresponding 16k and 64k long text versions.
 - 2024.04.22: Support for inference and fine-tuning of Llama3 GPTQ-Int4, GPTQ-Int8, and AWQ series models. Support for inference and fine-tuning of chatglm3-6b-128k, Openbuddy-Llama3.
 - 2024.04.20: Support for inference, fine-tuning, and deployment of **Atom** series models. This includes: Atom-7B and Atom-7B-Chat. use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/atom_7b_chat/lora/sft.sh) to train.
-- 2024.04.19: Support for single-card, DDP, ZeRO2, and ZeRO3 training and inference with NPU, please refer to [NPU Inference and Fine-tuning Best Practices](docs/source_en/LLM/NPU-best-practice.md).
+- 2024.04.19: Support for single-card, DDP, ZeRO2, and ZeRO3 training and inference with NPU, please refer to [NPU Inference and Fine-tuning Best Practice](docs/source_en/LLM/NPU-best-practice.md).
 - 2024.04.19: Support for inference, fine-tuning, and deployment of **Llama3** series models. This includes: Llama-3-8B, Llama-3-8B-Instruct, Llama-3-70B, and Llama-3-70B-Instruct. use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama3_8b_instruct/lora/sft.sh) to train.
+<details><summary>More</summary>
+
 - 2024.04.18: Supported models: wizardlm2-7b-awq, wizardlm2-8x22b, yi-6b-chat-awq, yi-6b-chat-int8, yi-34b-chat-awq, yi-34b-chat-int8. Supported `--deepspeed zero3-offload` and provided default zero3-offload configuration file for zero3+cpu offload usage.
 - 2024.04.18: Supported compatibility with HuggingFace ecosystem using the environment variable `USE_HF`, switching to use models and datasets from HF. Please refer to the [HuggingFace ecosystem compatibility documentation](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Compat-HF.md).
 - 2024.04.17: Support the evaluation for OpenAI standard interfaces. Check the [parameter documentation](docs/source_en/LLM/Command-line-parameters.md#eval-parameters) for details.
 - 🔥2024.04.17: Support **CodeQwen1.5-7B** series: CodeQwen1.5-7B, CodeQwen1.5-7B-Chat,CodeQwen1.5-7B-Chat-AWQ, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/codeqwen1half_7b_chat/lora/sft.sh) to train.
 - 2024.04.16: Supports inference and fine-tuning of llava-v1.6-34b model. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-practice.md).
 - 2024.04.13: Support the fine-tuning and inference of Mixtral-8x22B-v0.1 model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/lora_ddp_ds/sft.sh) to start training!
 - 2024.04.13: Support the newly launched **MiniCPM** series: MiniCPM-V-2.0、MiniCPM-2B-128k、MiniCPM-MoE-8x2B and MiniCPM-1B.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/minicpm_moe_8x2b/lora_ddp/sft.sh) to start training!
@@ -64,16 +86,14 @@
 - 🔥2024.04.03: Support **Qwen1.5-32B** series: Qwen1.5-32B, Qwen1.5-32B-Chat, Qwen1.5-32B-Chat-GPTQ-Int4.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_32b_chat/lora_mp/sft.sh) to start training!
 - 🔥2024.04.02: Support the fine-tuning and inference of Mengzi3-13B-Base model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mengzi3_13b_base/lora_ddp_ds/sft.sh) to start training!
 - 🔥2024.04.01: Support **dbrx** series: dbrx-base and dbrx-instruct, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/dbrx-instruct/lora_mp/sft.sh) to start training!
 - 🔥2024.03.29: Support **Qwen1.5-MoE** series: Qwen1.5-MoE-A2.7B, Qwen1.5-MoE-A2.7B-Chat, Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4.
 - 🔥2024.03.29: Support the fine-tuning and inference of **Grok-1** 300B MoE, please view details [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-practice.md).
 - 🔥2024.03.25: Supports inference and fine-tuning of TeleChat-7b and TeleChat-12b model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start training!
 - 🔥2024.03.20: Supports inference and fine-tuning for the **llava** series. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-practice.md).
-<details><summary>More</summary>
-
 - 🔥2024.03.12: Support inference and fine-tuning for **deepseek-vl** series. Best practices can be found [here](docs/source_en/Multi-Modal/deepseek-vl-best-practice.md).
 - 🔥2024.03.11: Support [GaLore](https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/2 of the original in full-parameter training.
 - 🔥2024.03.10: [End-to-end best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat.
 - 🔥2024.03.09: Support training and inference of MAMBA model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mamba-1.4b/lora/sft.sh) to start training!
 - 2024.03.09: Support training and inference of AQLM quantized model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama2_7b_aqlm_2bit_1x16/lora/sft.sh) to start training!
 - 2024.03.06: Support training and inference of AWQ quantized model, use [this Qwen1.5-AWQ model script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_awq/lora/sft.sh) to start training, and support training and inference of [yi-9b](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_9b/lora_zero3).
 - 🔥2024.02.29: Support [LLaMA PRO](https://arxiv.org/pdf/2401.02415.pdf), simply use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/llamapro/sft.sh) to start training.
@@ -96,18 +116,17 @@
 - 2024.01.24: Support codefuse-codegeex2-6b-chat, codefuse-qwen-14b-chat.
 - 2024.01.23: Support orion series: orion-14b, [orion-14b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/orion_14b_chat).
 - 2024.01.20: Support [xverse-13b-256k](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/xverse_13b_256k), xverse-65b-v2, xverse-65b-chat.
 - 🔥2024.01.17: Support internlm2 series: internlm2-7b-base, internlm2-7b, [internlm2-7b-sft-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/internlm2_7b_sft_chat), internlm2-7b-chat, internlm2-20b-base, internlm2-20b, internlm2-20b-sft-chat, internlm2-20b-chat.
 - 2024.01.15: Support yuan series: yuan2-2b-instruct, [yuan2-2b-janus-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yuan2_2b_janus_instruct), yuan2-51b-instruct, yuan2-102b-instruct.
 - 🔥2024.01.12: Support **deepseek-moe** series: deepseek-moe-16b, [deepseek-moe-16b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/deepseek_moe_16b_chat).
 - 🔥2024.01.04: Support **VLLM deployment**, compatible with **OpenAI API** style, see [VLLM Inference Acceleration and Deployment](https://github.com/modelscope/swift/blob/main/docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md#Deployment) for details.
-
 - 2024.01.04: Update [Benchmark](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) for convenient viewing of training speed and memory usage of different models.
 - 🔥2023.12.29: Support web-ui for sft training and inference, use `swift web-ui` after installing ms-swift to start.
-- 🔥2023.12.29: Support DPO RLHF (Reinforcement Learning from Human Feedback) and three datasets for this task: AI-ModelScope/stack-exchange-paired, AI-ModelScope/hh-rlhf and AI-ModelScope/hh_rlhf_cn. See [documentation](https://github.com/modelscope/swift/blob/main/docs/source/LLM/LLM%E4%BA%BA%E7%B1%BB%E5%AF%B9%E9%BD%90%E8%AE%AD%E7%BB%83%E6%96%87%E6%A1%A3.md) to start training!
+- 🔥2023.12.29: Support DPO RLHF (Reinforcement Learning from Human Feedback) and three datasets for this task: AI-ModelScope/stack-exchange-paired, AI-ModelScope/hh-rlhf and AI-ModelScope/hh_rlhf_cn. See [documentation](https://github.com/modelscope/swift/blob/main/docs/source_en/LLM/DPO.md) to start training!
 - 🔥2023.12.28: Support SCEdit! This tuner can significantly reduce memory usage in U-Net and support low-memory controllable image generation (replacing ControlNet), read the section below to learn more.
 - 2023.12.23: Support [codegeex2-6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/codegeex2_6b).
 - 2023.12.19: Support [phi2-3b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/phi2_3b).
 - 2023.12.18: Support VLLM for inference acceleration.
 - 2023.12.15: Support deepseek, deepseek-coder series: deepseek-7b, deepseek-7b-chat, deepseek-67b, deepseek-67b-chat, openbuddy-deepseek-67b-chat, deepseek-coder-1_3b, deepseek-coder-1_3b-instruct, deepseek-coder-6_7b, deepseek-coder-6_7b-instruct, deepseek-coder-33b, deepseek-coder-33b-instruct.
 - 2023.12.13: Support mistral-7b-instruct-v2, [mixtral-moe-7b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/mixtral_7b_moe), [mixtral-moe-7b-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/mixtral_7b_moe_instruct).
 - 2023.12.09: Support `freeze_parameters` parameter as a compromise between lora and full-parameter training. Corresponding sh can be found in [full_freeze_ddp](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/full_freeze_ddp). Support `disable_tqdm`, `lazy_tokenize`, `preprocess_num_proc` parameters, see [command line arguments](https://github.com/modelscope/swift/blob/main/docs/source/LLM/%E5%91%BD%E4%BB%A4%E8%A1%8C%E5%8F%82%E6%95%B0.md) for details.
@@ -179,18 +198,22 @@
 
 ## 🚀 Getting Started
 
 This section introduces basic usage, see the [Documentation](#-documentation) section for more ways to use.
 
 ### Web-UI
 
+Web-UI is a gradio-based interface for **zero-threshold** training and deployment. It is easy to use and perfectly supports multi-GPU training and deployment:
+
 ```shell
-swift web-ui
+SWIFT_UI_LANG=en swift web-ui
 ```
 
+![image.png](./docs/resources/web-ui-en.jpg)
+
 ### Training
 
 #### Training Scripts
 You can refer to the following scripts to customize your own training script.
 
 - full: [qwen1half-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat/full) (A100), [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/full_mp) (2\*A100)
 - full+ddp+zero2: [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/full_ddp_zero2) (4\*A100)
@@ -205,15 +228,15 @@
 
 #### Supported Training Processes
 
 | Training Process | Training Method                                                               |
 |------------------|-------------------------------------------------------------------------------|
 | Pretraining      | Text Generation                                                               |
 | Fine-tuning      | Single-turn/Multi-turn<br>Agent Training/Self-cognition<br>Multi-modal Vision/Multi-modal Speech|
-| Human Alignment  | DPO                                                                           |
+| Human Alignment  | DPO<br>ORPO                                                                   |
 | Text-to-Image    | DreamBooth, etc.                                                              |
 | Text-to-Video    | -                                                                             |
 
 #### Single GPU Training
 
 Start single GPU fine-tuning with the following command:
 
@@ -372,14 +395,28 @@
     --model_id_or_path qwen1half-32b-chat \
     --sft_type full \
     --dataset blossom-math-zh \
     --output_dir output \
     --deepspeed default-zero3 \
 ```
 
+##### AliYun-DLC multi-node training
+In DLC product, WORLD_SIZE is the node number, RANK is the node index, this is different from the definition of torchrun.
+
+```shell
+NNODES=$WORLD_SIZE \
+NODE_RANK=$RANK \
+swift sft \
+    --model_id_or_path qwen1half-32b-chat \
+    --sft_type full \
+    --dataset blossom-math-zh \
+    --output_dir output \
+    --deepspeed default-zero3
+```
+
 
 ### Inference
 Original model:
 ```shell
 CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat
 # use VLLM
 CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat \
@@ -447,17 +484,17 @@
 | ChatGLM2<br>ChatGLM3<br>Codegeex2                    | [Zhipu ChatGLM series models](https://github.com/THUDM)               | Chinese<br>English    | 6B                                     | base model<br>chat model<br>code model<br>long text model  |
 | Baichuan/Baichuan2                             | [Baichuan 1 and Baichuan 2](https://github.com/baichuan-inc)           | Chinese<br>English    | 7B-13B<br>including quantized versions             | base model<br>chat model                       |
 | Yuan2                                          | [Langchao Yuan series models](https://github.com/IEIT-Yuan)             | Chinese<br>English    | 2B-102B                                | instruct model                                 |
 | XVerse                                         | [XVerse series models](https://github.com/xverse-ai)                    | Chinese<br>English    | 7B-65B                                 | base model<br>chat model<br>long text model<br>MoE model                |
 | LLaMA2                                         | [LLaMA2 series models](https://github.com/facebookresearch/llama)       | English            | 7B-70B<br>including quantized versions   | base model<br>chat model                       |
 | LLaMA3                   | [LLaMA3 series models](https://github.com/meta-llama/llama3)  | English       | 8B-70B<br>including quantized versions      | base model<br>chat model              |
 | Mistral<br>Mixtral                            | [Mistral series models](https://github.com/mistralai/mistral-src)       | English            | 7B-22B     | base model<br>instruct model<br>MoE model                     |
-| YI                                             | [01AI's YI series models](https://github.com/01-ai)                     | Chinese<br>English    | 6B-34B<br>including quantized             | base model<br>chat model<br>long text model            |
+| Yi<br>Yi1.5                                      | [01AI's YI series models](https://github.com/01-ai)                     | Chinese<br>English    | 6B-34B<br>including quantized             | base model<br>chat model<br>long text model            |
 | InternLM<br>InternLM2<br>InternLM2-Math              | [Pujiang AI Lab InternLM series models](https://github.com/InternLM/InternLM) | Chinese<br>English | 1.8B-20B                            | base model<br>chat model<br>math model            |
-| DeepSeek<br>DeepSeek-MoE<br>DeepSeek-Coder<br>DeepSeek-Math          | [DeepSeek series models](https://github.com/deepseek-ai)       | Chinese<br>English    | 1.3B-67B                               | base model<br>chat model<br>MoE model<br>code model<br>math model |
+| DeepSeek<br>DeepSeek-MoE<br>DeepSeek-Coder<br>DeepSeek-Math<br>DeepSeek-V2          | [DeepSeek series models](https://github.com/deepseek-ai)       | Chinese<br>English    | 1.3B-236B                               | base model<br>chat model<br>MoE model<br>code model<br>math model |
 | MAMBA                                          | [MAMBA temporal convolution model](https://github.com/state-spaces/mamba) | English          | 130M-2.8B                              | base model                                 |
 | Gemma                                          | [Google Gemma series models](https://github.com/google/gemma_pytorch)   | English            | 2B-7B                                  | base model<br>instruct model                       |
 | MiniCPM                                        | [OpenBmB MiniCPM series models](https://github.com/OpenBMB/MiniCPM)     | Chinese<br>English    | 2B-3B                                  | chat model<br>MoE model                                 |
 | OpenBuddy                                      | [OpenBuddy series models](https://github.com/OpenBuddy/OpenBuddy)       | Chinese<br>English    | 7B-67B                                 | base model<br>chat model                       |
 | Orion                                          | [OrionStar AI series models](https://github.com/OrionStarAI)            | Chinese<br>English    | 14B                                    | base model<br>chat model                       |
 | BlueLM                                         | [VIVO BlueLM large model](https://github.com/vivo-ai-lab/BlueLM)        | Chinese<br>English    | 7B                                     | base model<br>chat model                       |
 | Ziya2                                          | [Fengshenbang series models](https://github.com/IDEA-CCNL/Fengshenbang-LM) | Chinese<br>English  | 13B                                    | base model<br>chat model                       |
@@ -478,52 +515,54 @@
 | Atom | [Atom](https://github.com/LlamaFamily/Llama-Chinese) | Chinese | 7B| base model<br>chat model|
 | Chinese-LLaMA-Alpaca-2 | [Chinese-LLaMA-Alpaca-2](https://github.com/ymcui/Chinese-LLaMA-Alpaca-2) | Chinese | 1.3B-13B| base model<br>chat model<br>long text model |
 | Chinese-LLaMA-Alpaca-3 | [Chinese-LLaMA-Alpaca-3](https://github.com/ymcui/Chinese-LLaMA-Alpaca-3) | Chinese | 8B| base model<br>chat model|
 | ModelScope-Agent | [ModelScope Agent series models](https://github.com/modelscope/modelscope-agent) | Chinese | 7B-14B| agent model |
 
 #### MLLMs
 
-| Model Type       | Model Introduction                                                     | Language           | Model Size        | Model Type         |
+| Model Type         | Model Introduction                                                           | Language           | Model Size                         | Model Type         |
 |------------------|------------------------------------------------------------------------|--------------------|-------------------|------------------- |
-| Qwen-VL          | [Tongyi Qwen vision model](https://github.com/QwenLM)               | Chinese<br>English    | 7B<br>including quantized versions | base model<br>chat model |
-| Qwen-Audio       | [Tongyi Qwen speech model](https://github.com/QwenLM)               | Chinese<br>English    | 7B                | base model<br>chat model |
-| YI-VL            | [01AI's YI series vision models](https://github.com/01-ai)             | Chinese<br>English    | 6B-34B            | chat model         |
-| XComposer2       | [Pujiang AI Lab InternLM vision model](https://github.com/InternLM/InternLM) | Chinese<br>English | 7B              | chat model         |
-| DeepSeek-VL      | [DeepSeek series vision models](https://github.com/deepseek-ai) | Chinese<br>English    | 1.3B-7B           | chat model         |
-| MiniCPM-V       | [OpenBmB MiniCPM vision model](https://github.com/OpenBMB/MiniCPM)     | Chinese<br>English    | 3B                | chat model         |
-| CogVLM<br>CogAgent  | [Zhipu ChatGLM visual QA and Agent model](https://github.com/THUDM/)   | English    | 17B-18B           | chat model         |
-| Llava      | [Llava series models](https://github.com/haotian-liu/LLaVA)                | English | 7B-34B               | chat model |
-| mPLUG-Owl      | [mPLUG-Owl series models](https://github.com/X-PLUG/mPLUG-Owl)         | English | 11B               | chat model |
-| InternVL         | [InternVL](https://github.com/OpenGVLab/InternVL)                | Chinese<br>English | 25.5B | chat model |
+| Qwen-VL            | [Tongyi Qwen vision model](https://github.com/QwenLM)                        | Chinese<br>English    | 7B<br>including quantized versions | base model<br>chat model |
+| Qwen-Audio         | [Tongyi Qwen speech model](https://github.com/QwenLM)                        | Chinese<br>English    | 7B                                 | base model<br>chat model |
+| YI-VL              | [01AI's YI series vision models](https://github.com/01-ai)                   | Chinese<br>English    | 6B-34B                             | chat model         |
+| XComposer2         | [Pujiang AI Lab InternLM vision model](https://github.com/InternLM/InternLM) | Chinese<br>English | 7B                                 | chat model         |
+| DeepSeek-VL        | [DeepSeek series vision models](https://github.com/deepseek-ai)              | Chinese<br>English    | 1.3B-7B                            | chat model         |
+| MiniCPM-V<br>MiniCPM-V-2<br>MiniCPM-V-2_5  | [OpenBmB MiniCPM vision model](https://github.com/OpenBMB/MiniCPM) | Chinese<br>English | 3B-9B            | chat model          |
+| CogVLM<br>CogVLM2<br>CogAgent | [Zhipu ChatGLM visual QA and Agent model](https://github.com/THUDM/)         | Chinese<br>English    | 17B-19B                            | chat model         |
+| Llava              | [Llava series models](https://github.com/haotian-liu/LLaVA)                  | English | 7B-34B                             | chat model |
+| Llava-Next              | [Llava-Next series models](https://github.com/LLaVA-VL/LLaVA-NeXT)                  | Chinese<br>English | 8B-110B                             | chat model |
+| mPLUG-Owl          | [mPLUG-Owl series models](https://github.com/X-PLUG/mPLUG-Owl)               | English | 11B                                | chat model |
+| InternVL           | [InternVL](https://github.com/OpenGVLab/InternVL)                            | Chinese<br>English | 25.5B<br>including quantized version                              | chat model |
+| Llava-llama3       | [xtuner](https://huggingface.co/xtuner/llava-llama-3-8b-v1_1-transformers)   | English | 8B                                 | chat model |
 
 #### Diffusion Models
 
 | Model Type          | Model Introduction                                                    | Language | Model Type        |
 |---------------------|----------------------------------------------------------------------|----------|------------------ |
 | AnimateDiff         | [AnimateDiff animation model](https://github.com/guoyww/AnimateDiff) | English  | text-to-video     |
 | SD1.5/SD2.0/SDXL    | [StabilityAI series diffusion models](https://github.com/Stability-AI) | English | text-to-image    |
 
 ### Supported Open Source Datasets
 
 | Dataset Type | Training Task  | Documentation                                                                                                                                                                                                                                                                                                        |
 |--------------|:---------------|--------------------------------------------------------------- |
-| General      | Fine-tuning    | 🔥ruozhiba, 🔥ms-bench, 🔥ms-bench-mini, 🔥alpaca-en(gpt4), 🔥alpaca-zh(gpt4), multi-alpaca-all, instinwild-en, instinwild-zh, cot-en, cot-zh, firefly-all-zh, instruct-en, gpt4all-en, sharegpt-en, sharegpt-zh, tulu-v2-sft-mixture, wikipedia-zh, open-orca, open-orca-gpt4, sharegpt-gpt4, 🔥sharegpt-gpt4-mini. |
-| Agent        | Fine-tuning    | 🔥ms-agent, ms-agent-for-agentfabric-default, ms-agent-for-agentfabric-addition, damo-mini-agent-zh, damo-agent-zh, agent-instruct-all-en.                                                                                                                                                                                                                                                |
-| General      | Human Alignment | 🔥hh-rlhf-cn, stack-exchange-paired, hh-rlhf-harmless-base, hh-rlhf-helpful-base, hh-rlhf-helpful-online, hh-rlhf-helpful-rejection-sampled, hh-rlhf-red-team-attempts, hh-rlhf-cn-harmless-base-cn, hh-rlhf-cn-helpful-base-cn, hh-rlhf-cn-harmless-base-en, hh-rlhf-cn-helpful-base-en.                            |
-| Code         | Fine-tuning    | code-alpaca-en, 🔥leetcode-python-en, 🔥codefuse-python-en, 🔥codefuse-evol-instruction-zh.                                                                                                                                                                                                                          |
-| Medical      | Fine-tuning    | medical-en, medical-zh, medical-mini-zh, 🔥disc-med-sft-zh.                                                                                                                                                                                                                                                          |
-| Legal        | Fine-tuning    | lawyer-llama-zh, tigerbot-law-zh, 🔥disc-law-sft-zh.                                                                                                                                                                                                                                                                 |
-| Math         | Fine-tuning    | 🔥blossom-math-zh, school-math-zh, open-platypus-en.                                                                                                                                                                                                                                                                 |
-| SQL          | Fine-tuning    | text2sql-en, 🔥sql-create-context-en.                                                                                                                                                                                                                                                                                |
-| Text Generation | Fine-tuning | 🔥advertise-gen-zh, 🔥dureader-robust-zh.                                                                                                                                                                                                                                                                            |
-| Classification | Fine-tuning  | cmnli-zh, 🔥cmnli-mini-zh, 🔥jd-sentiment-zh, 🔥hc3-zh, 🔥hc3-en.                                                                                                                                                                                                                                                    |
-| Quantization Assist | Quantization | pileval.                                                                                                                                                                                                                                                                                                             |
-| Other        | Fine-tuning    | finance-en, poetry-zh, webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-jave-zh.                                                                                                                                                                                                                               |
-| Vision       | Fine-tuning    | coco-en, 🔥coco-mini-en, coco-mini-en-2, capcha-images.                                                                                                                                                                                                                                                              |
-| Audio        | Fine-tuning    | aishell1-zh, 🔥aishell1-mini-zh.                                                                                                                                                                                                                                                                                     |
+| General      | Fine-tuning    | 🔥ruozhiba, 🔥ms-bench, 🔥alpaca-en(gpt4), 🔥alpaca-zh(gpt4), multi-alpaca, instinwild, cot-en, cot-zh, firefly-zh, instruct-en, gpt4all-en, sharegpt, tulu-v2-sft-mixture, wikipedia-zh, open-orca, sharegpt-gpt4, deepctrl-sft, coig-cqia. |
+| Agent        | Fine-tuning    | 🔥ms-agent, 🔥ms-agent-for-agentfabric, ms-agent-multirole, 🔥toolbench-for-alpha-umi, damo-agent-zh, damo-agent-zh-mini, agent-instruct-all-en.                    |
+| General      | Human Alignment | hh-rlhf, 🔥hh-rlhf-cn, stack-exchange-paired.                            |
+| Code         | Fine-tuning    | code-alpaca-en, 🔥leetcode-python-en, 🔥codefuse-python-en, 🔥codefuse-evol-instruction-zh.    |
+| Medical      | Fine-tuning    | medical-en, medical-zh, 🔥disc-med-sft-zh.               |
+| Legal        | Fine-tuning    | lawyer-llama-zh, tigerbot-law-zh, 🔥disc-law-sft-zh.               |
+| Math         | Fine-tuning    | 🔥blossom-math-zh, school-math-zh, open-platypus-en.                      |
+| SQL          | Fine-tuning    | text2sql-en, 🔥sql-create-context-en.                                    |
+| Text Generation | Fine-tuning | 🔥advertise-gen-zh, 🔥dureader-robust-zh.                            |
+| Classification | Fine-tuning  | cmnli-zh, 🔥jd-sentiment-zh, 🔥hc3-zh, 🔥hc3-en.           |
+| Quantization Assist | Quantization | pileval.  |
+| Other        | Fine-tuning    | finance-en, poetry-zh, webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-jave-zh.   |
+| Vision       | Fine-tuning    | coco-en, 🔥coco-en-mini, coco-en-2, coco-en-2-mini, capcha-images.         |
+| Audio        | Fine-tuning    | aishell1-zh, 🔥aishell1-zh-mini.       |
 
 ### Supported Technologies
 
 | Technology Name                                              |
 | ------------------------------------------------------------ |
 | 🔥LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE MODELS](https://arxiv.org/abs/2106.09685) |
 | 🔥LoRA+: [LoRA+: Efficient Low Rank Adaptation of Large Models](https://arxiv.org/pdf/2402.12354.pdf) |
@@ -566,15 +605,16 @@
 | [Using Web-UI](docs/source_en/GetStarted/Web-ui.md)          |
 | [Using Tuners](docs/source_en/GetStarted/Tuners.md)          |
 | [LLM Inference](docs/source_en/LLM/LLM-inference.md)         |
 | [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-tuning.md)     |
 | [LLM Evaluation](docs/source_en/LLM/LLM-eval.md)     |
 | [LLM Quantization](docs/source_en/LLM/LLM-quantization.md)   |
 | [LLM Deployment](docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md) |
-| [DPO Human Alignment Training](docs/source_en/LLM/RLHF.md)   |
+| [DPO Human Alignment Training](docs/source_en/LLM/DPO.md)   |
+| [ORPO Human Alignment Training](docs/source_en/LLM/ORPO.md)   |
 | [AnimateDiff Training](docs/source_en/AIGC/AnimateDiff-train-infer.md) |
 
 ### Reference Documentation
 | Document Name                                                |
 | ------------------------------------------------------------ |
 | [Command Line Arguments](docs/source_en/LLM/Command-line-parameters.md) |
 | [Supported Models and Datasets List](docs/source_en/LLM/Supported-models-datasets.md) |
@@ -620,15 +660,15 @@
   title = {SWIFT:Scalable lightWeight Infrastructure for Fine-Tuning},
   author = {The ModelScope Team},
   howpublished = {\url{https://github.com/modelscope/swift}},
   year = {2024}
 }
 ```
 
-## ☎ Contact Us
+## ☎ Wechat Group
 
 You can contact us and communicate with us by adding our WeChat group:
 
 <p align="left">
 <img src="asset/wechat.png" width="250" style="display: inline-block;">
 </p>
```

#### html2text {}

```diff
@@ -5,61 +5,98 @@
                            _ä_¸_­_æ__   ï½   English  
       [https://img.shields.io/badge/python-%E2%89%A53.8-5be.svg][https://
   img.shields.io/badge/pytorch-%E2%89%A51.12%20%7C%20%E2%89%A52.0-orange.svg]
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_m_o_d_e_l_s_c_o_p_e_-_%_E_2_%_8_9_%_A_5_1_._9_._5_-_5_D_9_1_D_4_._s_v_g_]_[_h_t_t_p_s_:_/_/
      _b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_m_s_-_s_w_i_f_t_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/
   _m_o_d_e_l_s_c_o_p_e_/_s_w_i_f_t_]_[_h_t_t_p_s_:_/_/_p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_m_s_-_s_w_i_f_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
                          _b_a_d_g_e_/_P_R_-_w_e_l_c_o_m_e_-_5_5_E_B_9_9_._s_v_g_]
+                       _[_m_o_d_e_l_s_c_o_p_e_%_2_F_s_w_i_f_t_ _|_ _T_r_e_n_d_s_h_i_f_t_]
 ## ð Table of Contents - [Introduction](#-introduction) - [News](#-news) -
 [Installation](#%EF%B8%8F-installation) - [Getting Started](#-getting-started)
 - [Documentation](#-documentation) - [License](#-License) - [Citation](#-
-citation) - [Contact Us](#-contact-us) ## ð Introduction SWIFT supports
+citation) - [WeChat Group](#-Wechat-Group) ## ð Introduction SWIFT supports
 training, inference, evaluation and deployment of nearly **200 LLMs and MLLMs**
 (multimodal large models). Developers can directly apply our framework to their
 own research and production environments to realize the complete workflow from
 model training and evaluation to application. In addition to supporting the
 lightweight training solutions provided by [PEFT](https://github.com/
 huggingface/peft), we also provide a complete **Adapters library** to support
 the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This
 adapter library can be used directly in your own custom workflow without our
 training scripts. To facilitate use by users unfamiliar with deep learning, we
 provide a Gradio web-ui for controlling training and inference, as well as
 accompanying deep learning courses and best practices for beginners.
 Additionally, we are expanding capabilities for other modalities. Currently, we
-support full-parameter training and LoRA training for AnimateDiff. ## ð News
-- 2024.04.29: Supports inference and fine-tuning of InternVL-Chat-V1.5 model.
-For best practice, you can refer to [here](https://github.com/modelscope/swift/
-tree/main/docs/source_en/Multi-Modal/internvl-best-practice.md). -
-ð¥2024.04.26: Support **LISA** and **unsloth** training! Specify `--
-lisa_activated_layers=2` to use LISA(to reduce the memory cost to 30 percent!),
-specify `--tuner_backend unsloth` to use unsloth to train a huge model(full or
-lora) with lesser memory(30 percent or lesser) and faster speed(5x)! -
-ð¥2024.04.26: Support the fine-tuning and inference of Qwen1.5-110B and
-Qwen1.5-110B-Chat model, use [this script](https://github.com/modelscope/swift/
-blob/main/examples/pytorch/llm/scripts/qwen1half_110b_chat/lora_ddp_ds/sft.sh)
-to start training! - 2024.04.24: Support for inference and fine-tuning of Phi3
-series models. Including: [phi3-4b-4k-instruct](examples/pytorch/llm/scripts/
+support full-parameter training and LoRA training for AnimateDiff. SWIFT has
+rich documentations for users, please check [here](https://github.com/
+modelscope/swift/tree/main/docs/source_en/LLM). SWIFT web-ui is available both
+on [Huggingface space](https://huggingface.co/spaces/tastelikefeet/swift) and
+[ModelScope studio](https://www.modelscope.cn/studios/iic/Scalable-lightWeight-
+Infrastructure-for-Fine-Tuning/summary), please feel free to try! ## ð News
+- 2024.05.22: Supports DeepSeek-V2-Lite series models, model_type are
+`deepseek-v2-lite` and `deepseek-v2-lite-chat` - 2024.05.22: Supports TeleChat-
+12B-v2 model with quantized version, model_type are `telechat-12b-v2` and
+`telechat-12b-v2-gptq-int4` - ð¥2024.05.21: Inference and fine-tuning support
+for MiniCPM-Llama3-V-2_5 are now available. For more details, please refer to
+[minicpm-v-2.5 Best Practice](docs/source/Multi-Modal/minicpm-v-
+2.5æä½³å®è·µ.md). - ð¥2024.05.20: Support for inferencing and fine-tuning
+cogvlm2-llama3-chinese-chat-19B, cogvlm2-llama3-chat-19B. you can refer to
+[cogvlm2 Best Practice](docs/source_en/Multi-Modal/cogvlm2-best-practice.md). -
+ð¥2024.05.17: Support peft=0.11.0. Meanwhile support 3 new tuners: `BOFT`,
+`Vera` and `Pissa`. use `--sft_type boft/vera` to use BOFT or Vera, use `--
+init_lora_weights pissa` with `--sft_type lora` to use Pissa. - 2024.05.16:
+Supports Llava-Next (Stronger) series models. For best practice, you can refer
+to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-
+Modal/llava-best-practice.md). - ð¥2024.05.13: Support Yi-1.5 series
+modelsï¼use `--model_type yi-1_5-9b-chat` to begin! - 2024.05.11: Support for
+qlora training and quantized inference using [hqq](https://github.com/mobiusml/
+hqq) and [eetq](https://github.com/NetEase-FuXi/EETQ). For more information,
+see the [LLM Quantization Documentation](https://github.com/modelscope/swift/
+tree/main/docs/source_en/LLM/LLM-quantization.md). - 2024.05.10: Support split
+a sequence to multiple GPUs to reduce memory usage. Use this feature by `pip
+install .[seq_parallel]`, then add `--sequence_parallel_size n` to your DDP
+script to begin! - 2024.05.08: Support DeepSeek-V2-Chat model, you can refer to
+[this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/
+llm/scripts/deepseek-v2-chat/lora_ddp_ds3/sft.sh).Support InternVL-Chat-V1.5-
+Int8 model, for best practice, you can refer to [here](https://github.com/
+modelscope/swift/tree/main/docs/source_en/Multi-Modal/internvl-best-
+practice.md). - ð¥2024.05.07: Supoprts **ORPO** training! See [document]
+(https://github.com/modelscope/swift/blob/main/docs/source_en/LLM/ORPO.md) to
+start training! - 2024.05.07: Supports Llava-Llama3 model from
+xtunerï¼model_type is `llava-llama-3-8b-v1_1`. - 2024.04.29: Supports
+inference and fine-tuning of InternVL-Chat-V1.5 model. For best practice, you
+can refer to [here](https://github.com/modelscope/swift/tree/main/docs/
+source_en/Multi-Modal/internvl-best-practice.md). - ð¥2024.04.26: Support
+**LISA** and **unsloth** training! Specify `--lisa_activated_layers=2` to use
+LISA(to reduce the memory cost to 30 percent!), specify `--tuner_backend
+unsloth` to use unsloth to train a huge model(full or lora) with lesser memory
+(30 percent or lesser) and faster speed(5x)! - ð¥2024.04.26: Support the
+fine-tuning and inference of Qwen1.5-110B and Qwen1.5-110B-Chat model, use
+[this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/
+llm/scripts/qwen1half_110b_chat/lora_ddp_ds/sft.sh) to start training! -
+2024.04.24: Support for inference and fine-tuning of Phi3 series models.
+Including: [phi3-4b-4k-instruct](examples/pytorch/llm/scripts/
 phi3_4b_4k_instruct/lora), phi3-4b-128k-instruct. - 2024.04.22: Support for
 inference, fine-tuning, and deployment of **chinese-llama-alpaca-2** series
 models. This includesï¼chinese-llama-2-1.3b, chinese-llama-2-7b, chinese-
 llama-2-13b, chinese-alpaca-2-1.3b, chinese-alpaca-2-7b and chinese-alpaca-2-
 13b along with their corresponding 16k and 64k long text versions. -
 2024.04.22: Support for inference and fine-tuning of Llama3 GPTQ-Int4, GPTQ-
 Int8, and AWQ series models. Support for inference and fine-tuning of chatglm3-
 6b-128k, Openbuddy-Llama3. - 2024.04.20: Support for inference, fine-tuning,
 and deployment of **Atom** series models. This includes: Atom-7B and Atom-7B-
 Chat. use [this script](https://github.com/modelscope/swift/blob/main/examples/
 pytorch/llm/scripts/atom_7b_chat/lora/sft.sh) to train. - 2024.04.19: Support
 for single-card, DDP, ZeRO2, and ZeRO3 training and inference with NPU, please
-refer to [NPU Inference and Fine-tuning Best Practices](docs/source_en/LLM/NPU-
+refer to [NPU Inference and Fine-tuning Best Practice](docs/source_en/LLM/NPU-
 best-practice.md). - 2024.04.19: Support for inference, fine-tuning, and
 deployment of **Llama3** series models. This includes: Llama-3-8B, Llama-3-8B-
 Instruct, Llama-3-70B, and Llama-3-70B-Instruct. use [this script](https://
 github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
-llama3_8b_instruct/lora/sft.sh) to train. - 2024.04.18: Supported models:
+llama3_8b_instruct/lora/sft.sh) to train. More - 2024.04.18: Supported models:
 wizardlm2-7b-awq, wizardlm2-8x22b, yi-6b-chat-awq, yi-6b-chat-int8, yi-34b-
 chat-awq, yi-34b-chat-int8. Supported `--deepspeed zero3-offload` and provided
 default zero3-offload configuration file for zero3+cpu offload usage. -
 2024.04.18: Supported compatibility with HuggingFace ecosystem using the
 environment variable `USE_HF`, switching to use models and datasets from HF.
 Please refer to the [HuggingFace ecosystem compatibility documentation](https:/
 /github.com/modelscope/swift/tree/main/docs/source_en/LLM/Compat-HF.md). -
@@ -114,15 +151,15 @@
 (https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-
 practice.md). - ð¥2024.03.25: Supports inference and fine-tuning of TeleChat-
 7b and TeleChat-12b model, use [this script](https://github.com/modelscope/
 swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start
 training! - ð¥2024.03.20: Supports inference and fine-tuning for the
 **llava** series. For best practice, you can refer to [here](https://
 github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-
-practice.md). More - ð¥2024.03.12: Support inference and fine-tuning for
+practice.md). - ð¥2024.03.12: Support inference and fine-tuning for
 **deepseek-vl** series. Best practices can be found [here](docs/source_en/
 Multi-Modal/deepseek-vl-best-practice.md). - ð¥2024.03.11: Support [GaLore]
 (https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/
 2 of the original in full-parameter training. - ð¥2024.03.10: [End-to-end
 best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning
 to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat. - ð¥2024.03.09:
 Support training and inference of MAMBA model, use [this script](https://
@@ -203,35 +240,33 @@
 /github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) for
 convenient viewing of training speed and memory usage of different models. -
 ð¥2023.12.29: Support web-ui for sft training and inference, use `swift web-
 ui` after installing ms-swift to start. - ð¥2023.12.29: Support DPO RLHF
 (Reinforcement Learning from Human Feedback) and three datasets for this task:
 AI-ModelScope/stack-exchange-paired, AI-ModelScope/hh-rlhf and AI-ModelScope/
 hh_rlhf_cn. See [documentation](https://github.com/modelscope/swift/blob/main/
-docs/source/LLM/
-LLM%E4%BA%BA%E7%B1%BB%E5%AF%B9%E9%BD%90%E8%AE%AD%E7%BB%83%E6%96%87%E6%A1%A3.md)
-to start training! - ð¥2023.12.28: Support SCEdit! This tuner can
-significantly reduce memory usage in U-Net and support low-memory controllable
-image generation (replacing ControlNet), read the section below to learn more.
-- 2023.12.23: Support [codegeex2-6b](https://github.com/modelscope/swift/tree/
-main/examples/pytorch/llm/scripts/codegeex2_6b). - 2023.12.19: Support [phi2-
-3b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
-phi2_3b). - 2023.12.18: Support VLLM for inference acceleration. - 2023.12.15:
-Support deepseek, deepseek-coder series: deepseek-7b, deepseek-7b-chat,
-deepseek-67b, deepseek-67b-chat, openbuddy-deepseek-67b-chat, deepseek-coder-
-1_3b, deepseek-coder-1_3b-instruct, deepseek-coder-6_7b, deepseek-coder-6_7b-
-instruct, deepseek-coder-33b, deepseek-coder-33b-instruct. - 2023.12.13:
-Support mistral-7b-instruct-v2, [mixtral-moe-7b](https://github.com/modelscope/
-swift/tree/main/examples/pytorch/llm/scripts/mixtral_7b_moe), [mixtral-moe-7b-
-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
-scripts/mixtral_7b_moe_instruct). - 2023.12.09: Support `freeze_parameters`
-parameter as a compromise between lora and full-parameter training.
-Corresponding sh can be found in [full_freeze_ddp](https://github.com/
-modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/
-full_freeze_ddp). Support `disable_tqdm`, `lazy_tokenize`,
+docs/source_en/LLM/DPO.md) to start training! - ð¥2023.12.28: Support SCEdit!
+This tuner can significantly reduce memory usage in U-Net and support low-
+memory controllable image generation (replacing ControlNet), read the section
+below to learn more. - 2023.12.23: Support [codegeex2-6b](https://github.com/
+modelscope/swift/tree/main/examples/pytorch/llm/scripts/codegeex2_6b). -
+2023.12.19: Support [phi2-3b](https://github.com/modelscope/swift/tree/main/
+examples/pytorch/llm/scripts/phi2_3b). - 2023.12.18: Support VLLM for inference
+acceleration. - 2023.12.15: Support deepseek, deepseek-coder series: deepseek-
+7b, deepseek-7b-chat, deepseek-67b, deepseek-67b-chat, openbuddy-deepseek-67b-
+chat, deepseek-coder-1_3b, deepseek-coder-1_3b-instruct, deepseek-coder-6_7b,
+deepseek-coder-6_7b-instruct, deepseek-coder-33b, deepseek-coder-33b-instruct.
+- 2023.12.13: Support mistral-7b-instruct-v2, [mixtral-moe-7b](https://
+github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
+mixtral_7b_moe), [mixtral-moe-7b-instruct](https://github.com/modelscope/swift/
+tree/main/examples/pytorch/llm/scripts/mixtral_7b_moe_instruct). - 2023.12.09:
+Support `freeze_parameters` parameter as a compromise between lora and full-
+parameter training. Corresponding sh can be found in [full_freeze_ddp](https://
+github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
+qwen_7b_chat/full_freeze_ddp). Support `disable_tqdm`, `lazy_tokenize`,
 `preprocess_num_proc` parameters, see [command line arguments](https://
 github.com/modelscope/swift/blob/main/docs/source/LLM/
 %E5%91%BD%E4%BB%A4%E8%A1%8C%E5%8F%82%E6%95%B0.md) for details. - 2023.12.08:
 Support [sus-34b-chat](https://github.com/modelscope/swift/tree/main/examples/
 pytorch/llm/scripts/sus_34b_chat), support yi-6b-200k, yi-34b-200k. -
 2023.12.07: Support [Multi-Node DDP training](https://github.com/modelscope/
 swift/blob/main/docs/source/LLM/
@@ -306,17 +341,20 @@
 [llm]' ``` SWIFT depends on torch>=1.13, recommend torch>=2.0.0. - Method 3:
 Use SWIFT in our Docker image ```shell # China-Hangzhou image docker pull
 registry.cn-hangzhou.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-
 cuda12.1.0-py310-torch2.1.2-tf2.14.0-1.13.1 # US-west image docker pull
 registry.us-west-1.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-
 cuda12.1.0-py310-torch2.1.2-tf2.14.0-1.13.1 ``` ## ð Getting Started This
 section introduces basic usage, see the [Documentation](#-documentation)
-section for more ways to use. ### Web-UI ```shell swift web-ui ``` ### Training
-#### Training Scripts You can refer to the following scripts to customize your
-own training script. - full: [qwen1half-7b-chat](https://github.com/modelscope/
+section for more ways to use. ### Web-UI Web-UI is a gradio-based interface for
+**zero-threshold** training and deployment. It is easy to use and perfectly
+supports multi-GPU training and deployment: ```shell SWIFT_UI_LANG=en swift
+web-ui ``` ![image.png](./docs/resources/web-ui-en.jpg) ### Training ####
+Training Scripts You can refer to the following scripts to customize your own
+training script. - full: [qwen1half-7b-chat](https://github.com/modelscope/
 swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat/full) (A100),
 [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/
 llm/scripts/qwen_7b_chat/full_mp) (2\*A100) - full+ddp+zero2: [qwen-7b-chat]
 (https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
 qwen_7b_chat/full_ddp_zero2) (4\*A100) - full+ddp+zero3: [qwen-14b-chat](https:
 //github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
 qwen_14b_chat/full_ddp_zero3) (4\*A100) - lora: [chatglm3-6b](https://
@@ -338,86 +376,91 @@
 scripts/qwen1half_7b_chat_int8/qlora) (3090) - qlora(bnb-int4): [qwen-7b-chat]
 (https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
 qwen_7b_chat/qlora) (3090) #### Supported Training Processes | Training Process
 | Training Method | |------------------|---------------------------------------
 ----------------------------------------| | Pretraining | Text Generation | |
 Fine-tuning | Single-turn/Multi-turn
 Agent Training/Self-cognition
-Multi-modal Vision/Multi-modal Speech| | Human Alignment | DPO | | Text-to-
-Image | DreamBooth, etc. | | Text-to-Video | - | #### Single GPU Training Start
-single GPU fine-tuning with the following command: LoRA: ```shell #
-Experimental Environment: A100 # GPU Memory Requirement: 20GB # Runtime: 3.1
+Multi-modal Vision/Multi-modal Speech| | Human Alignment | DPO
+ORPO | | Text-to-Image | DreamBooth, etc. | | Text-to-Video | - | #### Single
+GPU Training Start single GPU fine-tuning with the following command: LoRA:
+```shell # Experimental Environment: A100 # GPU Memory Requirement: 20GB #
+Runtime: 3.1 hours CUDA_VISIBLE_DEVICES=0 \ swift sft \ --model_type qwen1half-
+7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \
+--output_dir output \ --eval_steps 200 \ ``` Full-parameter: ```shell #
+Experimental Environment: A100 # GPU Memory Requirement: 80GB # Runtime: 2.5
 hours CUDA_VISIBLE_DEVICES=0 \ swift sft \ --model_type qwen1half-7b-chat \ --
-dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --output_dir
-output \ --eval_steps 200 \ ``` Full-parameter: ```shell # Experimental
-Environment: A100 # GPU Memory Requirement: 80GB # Runtime: 2.5 hours
-CUDA_VISIBLE_DEVICES=0 \ swift sft \ --model_type qwen1half-7b-chat \ --dataset
-blossom-math-zh \ --num_train_epochs 5 \ --sft_type full \ --output_dir output
-\ --eval_steps 500 \ ``` #### Model Parallel Training ```shell # Experimental
-Environment: 2 * A100 # GPU Memory Requirement: 10GB + 13GB # Runtime: 3.4
-hours CUDA_VISIBLE_DEVICES=0,1 \ swift sft \ --model_type qwen1half-7b-chat \ -
--dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --
-output_dir output \ ``` #### Data Parallel Training ```shell # Experimental
-Environment: 4 * A100 # GPU Memory Requirement: 4 * 30GB # Runtime: 0.8 hours
-NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type
+dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type full \ --output_dir
+output \ --eval_steps 500 \ ``` #### Model Parallel Training ```shell #
+Experimental Environment: 2 * A100 # GPU Memory Requirement: 10GB + 13GB #
+Runtime: 3.4 hours CUDA_VISIBLE_DEVICES=0,1 \ swift sft \ --model_type
 qwen1half-7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
-sft_type lora \ --output_dir output \ ``` Combining Model Parallelism and Data
-Parallelism: ```shell # Experimental Environment: 4 * A100 # GPU Memory
-Requirement: 2*14GB + 2*18GB # Runtime: 1.7 hours NPROC_PER_NODE=2 \
-CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type qwen1half-7b-chat \ --
-dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --output_dir
-output \ ``` #### Deepspeed Training Deepspeed supports training of quantized
-GPTQ and AWQ models. ZeRO2: ```shell # Experimental Environment: 4 * A100 # GPU
-Memory Requirement: 4 * 21GB # Runtime: 0.9 hours NPROC_PER_NODE=4 \
+sft_type lora \ --output_dir output \ ``` #### Data Parallel Training ```shell
+# Experimental Environment: 4 * A100 # GPU Memory Requirement: 4 * 30GB #
+Runtime: 0.8 hours NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft
+\ --model_type qwen1half-7b-chat \ --dataset blossom-math-zh \ --
+num_train_epochs 5 \ --sft_type lora \ --output_dir output \ ``` Combining
+Model Parallelism and Data Parallelism: ```shell # Experimental Environment: 4
+* A100 # GPU Memory Requirement: 2*14GB + 2*18GB # Runtime: 1.7 hours
+NPROC_PER_NODE=2 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type
+qwen1half-7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
+sft_type lora \ --output_dir output \ ``` #### Deepspeed Training Deepspeed
+supports training of quantized GPTQ and AWQ models. ZeRO2: ```shell #
+Experimental Environment: 4 * A100 # GPU Memory Requirement: 4 * 21GB #
+Runtime: 0.9 hours NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft
+\ --model_type qwen1half-7b-chat \ --dataset blossom-math-zh \ --
+num_train_epochs 5 \ --sft_type lora \ --output_dir output \ --deepspeed
+default-zero2 \ ``` ZeRO3: ```shell # Experimental Environment: 4 * A100 # GPU
+Memory Requirement: 4 * 19GB # Runtime: 3.2 hours NPROC_PER_NODE=4 \
 CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type qwen1half-7b-chat \ --
 dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --output_dir
-output \ --deepspeed default-zero2 \ ``` ZeRO3: ```shell # Experimental
-Environment: 4 * A100 # GPU Memory Requirement: 4 * 19GB # Runtime: 3.2 hours
-NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type
-qwen1half-7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
-sft_type lora \ --output_dir output \ --deepspeed default-zero3 \ ``` ZeRO3-
-Offload: ```shell # Experimental Environment: 4 * A100 # GPU Memory
-Requirement: 4 * 12GB # Runtime: 60 hours NPROC_PER_NODE=4 \
-CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_id_or_path AI-ModelScope/
-WizardLM-2-8x22B \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
-sft_type lora \ --output_dir output \ --deepspeed zero3-offload \ ``` ####
-Multi-node Multi-GPU ```shell # node0 CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 \
-NNODES=2 \ NODE_RANK=0 \ MASTER_ADDR=127.0.0.1 \ NPROC_PER_NODE=8 \ swift sft \
---model_id_or_path qwen1half-32b-chat \ --sft_type full \ --dataset blossom-
-math-zh \ --output_dir output \ --deepspeed default-zero3 \ # node1
+output \ --deepspeed default-zero3 \ ``` ZeRO3-Offload: ```shell # Experimental
+Environment: 4 * A100 # GPU Memory Requirement: 4 * 12GB # Runtime: 60 hours
+NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --
+model_id_or_path AI-ModelScope/WizardLM-2-8x22B \ --dataset blossom-math-zh \ -
+-num_train_epochs 5 \ --sft_type lora \ --output_dir output \ --deepspeed
+zero3-offload \ ``` #### Multi-node Multi-GPU ```shell # node0
+CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 \ NNODES=2 \ NODE_RANK=0 \
+MASTER_ADDR=127.0.0.1 \ NPROC_PER_NODE=8 \ swift sft \ --model_id_or_path
+qwen1half-32b-chat \ --sft_type full \ --dataset blossom-math-zh \ --output_dir
+output \ --deepspeed default-zero3 \ # node1
 CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 \ NNODES=2 \ NODE_RANK=1 \
 MASTER_ADDR=xxx.xxx.xxx.xxx \ NPROC_PER_NODE=8 \ swift sft \ --model_id_or_path
 qwen1half-32b-chat \ --sft_type full \ --dataset blossom-math-zh \ --output_dir
-output \ --deepspeed default-zero3 \ ``` ### Inference Original model: ```shell
-CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat # use VLLM
-CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat \ --
-infer_backend vllm --max_model_len 8192 ``` LoRA fine-tuned: ```shell
-CUDA_VISIBLE_DEVICES=0 swift infer --ckpt_dir xxx/checkpoint-xxx --
-load_dataset_config true # use VLLM CUDA_VISIBLE_DEVICES=0 swift infer \ --
-ckpt_dir xxx/checkpoint-xxx --load_dataset_config true \ --merge_lora true --
-infer_backend vllm --max_model_len 8192 ``` ### Evaluation ```shell
-CUDA_VISIBLE_DEVICES=0 swift eval --model_type qwen1half-7b-chat --eval_dataset
-mmlu ceval ``` ### Export Original model: ```shell CUDA_VISIBLE_DEVICES=0 swift
-export --model_type qwen1half-7b-chat \ --quant_bits 4 --quant_method awq ```
-LoRA fine-tuned: ```shell CUDA_VISIBLE_DEVICES=0 swift export \ --ckpt_dir xxx/
-checkpoint-xxx --load_dataset_config true \ --quant_method awq --quant_bits 4 \
---merge_lora true \ ``` ### Deployment Original model: ```shell
-CUDA_VISIBLE_DEVICES=0 swift deploy --model_type qwen1half-7b-chat #
-ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0 swift deploy --model_type qwen1half-7b-
-chat \ --infer_backend vllm --max_model_len 8192 ``` LoRA fine-tuned: ```shell
-CUDA_VISIBLE_DEVICES=0 swift deploy --ckpt_dir xxx/checkpoint-xxx #
-ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0 swift deploy \ --ckpt_dir xxx/
-checkpoint-xxx --merge_lora true \ --infer_backend vllm --max_model_len 8192
-``` ### Supported Models The complete list of supported models and datasets can
-be found at [Supported Models and Datasets List](docs/source_en/LLM/Supported-
-models-datasets.md). #### LLMs | Model Type | Model Introduction | Language |
-Model Size | Model Type | |------------------------------------------------|---
----------------------------------------------------------------------|---------
------------|----------------------------------------|--------------------------
------------------ | | Qwen
+output \ --deepspeed default-zero3 \ ``` ##### AliYun-DLC multi-node training
+In DLC product, WORLD_SIZE is the node number, RANK is the node index, this is
+different from the definition of torchrun. ```shell NNODES=$WORLD_SIZE \
+NODE_RANK=$RANK \ swift sft \ --model_id_or_path qwen1half-32b-chat \ --
+sft_type full \ --dataset blossom-math-zh \ --output_dir output \ --deepspeed
+default-zero3 ``` ### Inference Original model: ```shell CUDA_VISIBLE_DEVICES=0
+swift infer --model_type qwen1half-7b-chat # use VLLM CUDA_VISIBLE_DEVICES=0
+swift infer --model_type qwen1half-7b-chat \ --infer_backend vllm --
+max_model_len 8192 ``` LoRA fine-tuned: ```shell CUDA_VISIBLE_DEVICES=0 swift
+infer --ckpt_dir xxx/checkpoint-xxx --load_dataset_config true # use VLLM
+CUDA_VISIBLE_DEVICES=0 swift infer \ --ckpt_dir xxx/checkpoint-xxx --
+load_dataset_config true \ --merge_lora true --infer_backend vllm --
+max_model_len 8192 ``` ### Evaluation ```shell CUDA_VISIBLE_DEVICES=0 swift
+eval --model_type qwen1half-7b-chat --eval_dataset mmlu ceval ``` ### Export
+Original model: ```shell CUDA_VISIBLE_DEVICES=0 swift export --model_type
+qwen1half-7b-chat \ --quant_bits 4 --quant_method awq ``` LoRA fine-tuned:
+```shell CUDA_VISIBLE_DEVICES=0 swift export \ --ckpt_dir xxx/checkpoint-xxx --
+load_dataset_config true \ --quant_method awq --quant_bits 4 \ --merge_lora
+true \ ``` ### Deployment Original model: ```shell CUDA_VISIBLE_DEVICES=0 swift
+deploy --model_type qwen1half-7b-chat # ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0
+swift deploy --model_type qwen1half-7b-chat \ --infer_backend vllm --
+max_model_len 8192 ``` LoRA fine-tuned: ```shell CUDA_VISIBLE_DEVICES=0 swift
+deploy --ckpt_dir xxx/checkpoint-xxx # ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0
+swift deploy \ --ckpt_dir xxx/checkpoint-xxx --merge_lora true \ --
+infer_backend vllm --max_model_len 8192 ``` ### Supported Models The complete
+list of supported models and datasets can be found at [Supported Models and
+Datasets List](docs/source_en/LLM/Supported-models-datasets.md). #### LLMs |
+Model Type | Model Introduction | Language | Model Size | Model Type | |-------
+-----------------------------------------|-------------------------------------
+-----------------------------------|--------------------|----------------------
+------------------|------------------------------------------- | | Qwen
 Qwen1.5 | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM) |
 Chinese
 English | 0.5B-110B
 including quantized versions | base model
 chat model
 MoE model
 code model | | ChatGLM2
@@ -443,31 +486,32 @@
 chat model | | LLaMA3 | [LLaMA3 series models](https://github.com/meta-llama/
 llama3) | English | 8B-70B
 including quantized versions | base model
 chat model | | Mistral
 Mixtral | [Mistral series models](https://github.com/mistralai/mistral-src) |
 English | 7B-22B | base model
 instruct model
-MoE model | | YI | [01AI's YI series models](https://github.com/01-ai) |
-Chinese
+MoE model | | Yi
+Yi1.5 | [01AI's YI series models](https://github.com/01-ai) | Chinese
 English | 6B-34B
 including quantized | base model
 chat model
 long text model | | InternLM
 InternLM2
 InternLM2-Math | [Pujiang AI Lab InternLM series models](https://github.com/
 InternLM/InternLM) | Chinese
 English | 1.8B-20B | base model
 chat model
 math model | | DeepSeek
 DeepSeek-MoE
 DeepSeek-Coder
-DeepSeek-Math | [DeepSeek series models](https://github.com/deepseek-ai) |
+DeepSeek-Math
+DeepSeek-V2 | [DeepSeek series models](https://github.com/deepseek-ai) |
 Chinese
-English | 1.3B-67B | base model
+English | 1.3B-236B | base model
 chat model
 MoE model
 code model
 math model | | MAMBA | [MAMBA temporal convolution model](https://github.com/
 state-spaces/mamba) | English | 130M-2.8B | base model | | Gemma | [Google
 Gemma series models](https://github.com/google/gemma_pytorch) | English | 2B-7B
 | base model
@@ -540,109 +584,113 @@
 English | 7B | base model
 chat model | | YI-VL | [01AI's YI series vision models](https://github.com/01-
 ai) | Chinese
 English | 6B-34B | chat model | | XComposer2 | [Pujiang AI Lab InternLM vision
 model](https://github.com/InternLM/InternLM) | Chinese
 English | 7B | chat model | | DeepSeek-VL | [DeepSeek series vision models]
 (https://github.com/deepseek-ai) | Chinese
-English | 1.3B-7B | chat model | | MiniCPM-V | [OpenBmB MiniCPM vision model]
-(https://github.com/OpenBMB/MiniCPM) | Chinese
-English | 3B | chat model | | CogVLM
+English | 1.3B-7B | chat model | | MiniCPM-V
+MiniCPM-V-2
+MiniCPM-V-2_5 | [OpenBmB MiniCPM vision model](https://github.com/OpenBMB/
+MiniCPM) | Chinese
+English | 3B-9B | chat model | | CogVLM
+CogVLM2
 CogAgent | [Zhipu ChatGLM visual QA and Agent model](https://github.com/THUDM/
-) | English | 17B-18B | chat model | | Llava | [Llava series models](https://
-github.com/haotian-liu/LLaVA) | English | 7B-34B | chat model | | mPLUG-Owl |
-[mPLUG-Owl series models](https://github.com/X-PLUG/mPLUG-Owl) | English | 11B
-| chat model | | InternVL | [InternVL](https://github.com/OpenGVLab/InternVL) |
-Chinese
-English | 25.5B | chat model | #### Diffusion Models | Model Type | Model
-Introduction | Language | Model Type | |---------------------|-----------------
------------------------------------------------------|----------|--------------
----- | | AnimateDiff | [AnimateDiff animation model](https://github.com/guoyww/
-AnimateDiff) | English | text-to-video | | SD1.5/SD2.0/SDXL | [StabilityAI
-series diffusion models](https://github.com/Stability-AI) | English | text-to-
-image | ### Supported Open Source Datasets | Dataset Type | Training Task |
-Documentation | |--------------|:---------------|------------------------------
---------------------------------- | | General | Fine-tuning | ð¥ruozhiba,
-ð¥ms-bench, ð¥ms-bench-mini, ð¥alpaca-en(gpt4), ð¥alpaca-zh(gpt4),
-multi-alpaca-all, instinwild-en, instinwild-zh, cot-en, cot-zh, firefly-all-zh,
-instruct-en, gpt4all-en, sharegpt-en, sharegpt-zh, tulu-v2-sft-mixture,
-wikipedia-zh, open-orca, open-orca-gpt4, sharegpt-gpt4, ð¥sharegpt-gpt4-mini.
-| | Agent | Fine-tuning | ð¥ms-agent, ms-agent-for-agentfabric-default, ms-
-agent-for-agentfabric-addition, damo-mini-agent-zh, damo-agent-zh, agent-
-instruct-all-en. | | General | Human Alignment | ð¥hh-rlhf-cn, stack-
-exchange-paired, hh-rlhf-harmless-base, hh-rlhf-helpful-base, hh-rlhf-helpful-
-online, hh-rlhf-helpful-rejection-sampled, hh-rlhf-red-team-attempts, hh-rlhf-
-cn-harmless-base-cn, hh-rlhf-cn-helpful-base-cn, hh-rlhf-cn-harmless-base-en,
-hh-rlhf-cn-helpful-base-en. | | Code | Fine-tuning | code-alpaca-en,
-ð¥leetcode-python-en, ð¥codefuse-python-en, ð¥codefuse-evol-instruction-
-zh. | | Medical | Fine-tuning | medical-en, medical-zh, medical-mini-zh,
-ð¥disc-med-sft-zh. | | Legal | Fine-tuning | lawyer-llama-zh, tigerbot-law-
-zh, ð¥disc-law-sft-zh. | | Math | Fine-tuning | ð¥blossom-math-zh, school-
-math-zh, open-platypus-en. | | SQL | Fine-tuning | text2sql-en, ð¥sql-create-
-context-en. | | Text Generation | Fine-tuning | ð¥advertise-gen-zh,
-ð¥dureader-robust-zh. | | Classification | Fine-tuning | cmnli-zh, ð¥cmnli-
-mini-zh, ð¥jd-sentiment-zh, ð¥hc3-zh, ð¥hc3-en. | | Quantization Assist |
-Quantization | pileval. | | Other | Fine-tuning | finance-en, poetry-zh,
-webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-jave-zh. | | Vision |
-Fine-tuning | coco-en, ð¥coco-mini-en, coco-mini-en-2, capcha-images. | |
-Audio | Fine-tuning | aishell1-zh, ð¥aishell1-mini-zh. | ### Supported
-Technologies | Technology Name | | --------------------------------------------
----------------- | | ð¥LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE
-MODELS](https://arxiv.org/abs/2106.09685) | | ð¥LoRA+: [LoRA+: Efficient Low
-Rank Adaptation of Large Models](https://arxiv.org/pdf/2402.12354.pdf) | |
-ð¥GaLore:[GaLore: Memory-Efficient LLM Training by Gradient Low-Rank
-Projection](https://arxiv.org/abs/2403.03507) | | ð¥LISA: [LISA: Layerwise
-Importance Sampling for Memory-Efficient Large Language Model Fine-Tuning]
-(https://arxiv.org/abs/2403.17919) | | ð¥UnSloth: https://github.com/
-unslothai/unsloth | | ð¥LLaMA PRO: [LLAMA PRO: Progressive LLaMA with Block
-Expansion](https://arxiv.org/pdf/2401.02415.pdf) | | ð¥SCEdit: [SCEdit:
-Efficient and Controllable Image Diffusion Generation via Skip Connection
-Editing](https://arxiv.org/abs/2312.11392) < [arXiv](https://arxiv.org/abs/
-2312.11392) \ | | ð¥NEFTune: [Noisy Embeddings Improve Instruction
-Finetuning](https://arxiv.org/abs/2310.05914) | | LongLoRA: [Efficient Fine-
-tuning of Long-Context Large Language Models](https://arxiv.org/abs/2309.12307)
-| | Adapter: [Parameter-Efficient Transfer Learning for NLP](http://arxiv.org/
-abs/1902.00751) | | Vision Prompt Tuning: [Visual Prompt Tuning](https://
-arxiv.org/abs/2203.12119) | | Side: [Side-Tuning: A Baseline for Network
-Adaptation via Additive Side Networks](https://arxiv.org/abs/1912.13503) | |
-Res-Tuning: [Res-Tuning: A Flexible and Efficient Tuning Paradigm via Unbinding
-Tuner from Backbone](https://arxiv.org/abs/2310.19859) < [arXiv](https://
-arxiv.org/abs/2310.19859) \ | | Tuners provided by [PEFT](https://github.com/
-huggingface/peft), such as IA3, AdaLoRA, etc. | ### Supported Hardware |
-Hardware Environment | Notes | |--------------------------------|--------------
------------------------------------| | CPU | | | RTX 20/30/40 series, etc. |
-After 30 series, BF16 and FlashAttn can be used | | Computing cards T4/V100,
-etc. | BF16 and FlashAttn not supported | | Computing cards A10/A100, etc. |
-Support BF16 and FlashAttn | | Huawei Ascend NPU | | ## ð Documentation ###
-Documentation Compiling ```shell make docs # Check docs/build/html/index.html
-in web-browser ``` ### User Guide | Document Name | | -------------------------
------------------------------------ | | [Using Web-UI](docs/source_en/
-GetStarted/Web-ui.md) | | [Using Tuners](docs/source_en/GetStarted/Tuners.md) |
-| [LLM Inference](docs/source_en/LLM/LLM-inference.md) | | [LLM Fine-tuning]
-(docs/source_en/LLM/LLM-fine-tuning.md) | | [LLM Evaluation](docs/source_en/
-LLM/LLM-eval.md) | | [LLM Quantization](docs/source_en/LLM/LLM-quantization.md)
-| | [LLM Deployment](docs/source_en/LLM/VLLM-inference-acceleration-and-
-deployment.md) | | [DPO Human Alignment Training](docs/source_en/LLM/RLHF.md) |
-| [AnimateDiff Training](docs/source_en/AIGC/AnimateDiff-train-infer.md) | ###
-Reference Documentation | Document Name | | -----------------------------------
-------------------------- | | [Command Line Arguments](docs/source_en/LLM/
-Command-line-parameters.md) | | [Supported Models and Datasets List](docs/
-source_en/LLM/Supported-models-datasets.md) | | [Customizing New Models and
-Datasets](docs/source_en/LLM/Customization.md) | | [Runtime Speed and Memory
-Benchmark](docs/source_en/LLM/Benchmark.md) | ### Best Practices | Best
-Practices Name | | -----------------------------------------------------------
-- | | [Agent Fine-Tuning Best Practice](docs/source_en/LLM/Agent-best-
-practice.md) | | [Self-Cognition Fine-Tuning Best Practice](docs/source_en/LLM/
-Self-cognition-best-practice.md) | | [Qwen1.5 Best Practice](docs/source_en/
-LLM/Qwen1.5-best-practice.md) | | [Multi-Modal Model Training Best Practice]
-(docs/source_en/Multi-Modal/index.md) | | [NPU Best Practice](docs/source_en/
-LLM/NPU-best-practice.md) | ### Deep Learning Tutorials | Tutorial Name | |----
----------------------------------------------------------- | | [Introduction to
-Deep Learning](https://github.com/modelscope/modelscope-classroom/blob/main/
-LLM-tutorial/
+) | Chinese
+English | 17B-19B | chat model | | Llava | [Llava series models](https://
+github.com/haotian-liu/LLaVA) | English | 7B-34B | chat model | | Llava-Next |
+[Llava-Next series models](https://github.com/LLaVA-VL/LLaVA-NeXT) | Chinese
+English | 8B-110B | chat model | | mPLUG-Owl | [mPLUG-Owl series models](https:
+//github.com/X-PLUG/mPLUG-Owl) | English | 11B | chat model | | InternVL |
+[InternVL](https://github.com/OpenGVLab/InternVL) | Chinese
+English | 25.5B
+including quantized version | chat model | | Llava-llama3 | [xtuner](https://
+huggingface.co/xtuner/llava-llama-3-8b-v1_1-transformers) | English | 8B | chat
+model | #### Diffusion Models | Model Type | Model Introduction | Language |
+Model Type | |---------------------|-------------------------------------------
+---------------------------|----------|------------------ | | AnimateDiff |
+[AnimateDiff animation model](https://github.com/guoyww/AnimateDiff) | English
+| text-to-video | | SD1.5/SD2.0/SDXL | [StabilityAI series diffusion models]
+(https://github.com/Stability-AI) | English | text-to-image | ### Supported
+Open Source Datasets | Dataset Type | Training Task | Documentation | |--------
+------|:---------------|-------------------------------------------------------
+-------- | | General | Fine-tuning | ð¥ruozhiba, ð¥ms-bench, ð¥alpaca-en
+(gpt4), ð¥alpaca-zh(gpt4), multi-alpaca, instinwild, cot-en, cot-zh, firefly-
+zh, instruct-en, gpt4all-en, sharegpt, tulu-v2-sft-mixture, wikipedia-zh, open-
+orca, sharegpt-gpt4, deepctrl-sft, coig-cqia. | | Agent | Fine-tuning | ð¥ms-
+agent, ð¥ms-agent-for-agentfabric, ms-agent-multirole, ð¥toolbench-for-
+alpha-umi, damo-agent-zh, damo-agent-zh-mini, agent-instruct-all-en. | |
+General | Human Alignment | hh-rlhf, ð¥hh-rlhf-cn, stack-exchange-paired. | |
+Code | Fine-tuning | code-alpaca-en, ð¥leetcode-python-en, ð¥codefuse-
+python-en, ð¥codefuse-evol-instruction-zh. | | Medical | Fine-tuning |
+medical-en, medical-zh, ð¥disc-med-sft-zh. | | Legal | Fine-tuning | lawyer-
+llama-zh, tigerbot-law-zh, ð¥disc-law-sft-zh. | | Math | Fine-tuning |
+ð¥blossom-math-zh, school-math-zh, open-platypus-en. | | SQL | Fine-tuning |
+text2sql-en, ð¥sql-create-context-en. | | Text Generation | Fine-tuning |
+ð¥advertise-gen-zh, ð¥dureader-robust-zh. | | Classification | Fine-tuning
+| cmnli-zh, ð¥jd-sentiment-zh, ð¥hc3-zh, ð¥hc3-en. | | Quantization
+Assist | Quantization | pileval. | | Other | Fine-tuning | finance-en, poetry-
+zh, webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-jave-zh. | | Vision
+| Fine-tuning | coco-en, ð¥coco-en-mini, coco-en-2, coco-en-2-mini, capcha-
+images. | | Audio | Fine-tuning | aishell1-zh, ð¥aishell1-zh-mini. | ###
+Supported Technologies | Technology Name | | ----------------------------------
+-------------------------- | | ð¥LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE
+LANGUAGE MODELS](https://arxiv.org/abs/2106.09685) | | ð¥LoRA+: [LoRA+:
+Efficient Low Rank Adaptation of Large Models](https://arxiv.org/pdf/
+2402.12354.pdf) | | ð¥GaLore:[GaLore: Memory-Efficient LLM Training by
+Gradient Low-Rank Projection](https://arxiv.org/abs/2403.03507) | | ð¥LISA:
+[LISA: Layerwise Importance Sampling for Memory-Efficient Large Language Model
+Fine-Tuning](https://arxiv.org/abs/2403.17919) | | ð¥UnSloth: https://
+github.com/unslothai/unsloth | | ð¥LLaMA PRO: [LLAMA PRO: Progressive LLaMA
+with Block Expansion](https://arxiv.org/pdf/2401.02415.pdf) | | ð¥SCEdit:
+[SCEdit: Efficient and Controllable Image Diffusion Generation via Skip
+Connection Editing](https://arxiv.org/abs/2312.11392) < [arXiv](https://
+arxiv.org/abs/2312.11392) \ | | ð¥NEFTune: [Noisy Embeddings Improve
+Instruction Finetuning](https://arxiv.org/abs/2310.05914) | | LongLoRA:
+[Efficient Fine-tuning of Long-Context Large Language Models](https://
+arxiv.org/abs/2309.12307) | | Adapter: [Parameter-Efficient Transfer Learning
+for NLP](http://arxiv.org/abs/1902.00751) | | Vision Prompt Tuning: [Visual
+Prompt Tuning](https://arxiv.org/abs/2203.12119) | | Side: [Side-Tuning: A
+Baseline for Network Adaptation via Additive Side Networks](https://arxiv.org/
+abs/1912.13503) | | Res-Tuning: [Res-Tuning: A Flexible and Efficient Tuning
+Paradigm via Unbinding Tuner from Backbone](https://arxiv.org/abs/2310.19859) <
+[arXiv](https://arxiv.org/abs/2310.19859) \ | | Tuners provided by [PEFT]
+(https://github.com/huggingface/peft), such as IA3, AdaLoRA, etc. | ###
+Supported Hardware | Hardware Environment | Notes | |--------------------------
+------|-------------------------------------------------| | CPU | | | RTX 20/
+30/40 series, etc. | After 30 series, BF16 and FlashAttn can be used | |
+Computing cards T4/V100, etc. | BF16 and FlashAttn not supported | | Computing
+cards A10/A100, etc. | Support BF16 and FlashAttn | | Huawei Ascend NPU | | ##
+ð Documentation ### Documentation Compiling ```shell make docs # Check docs/
+build/html/index.html in web-browser ``` ### User Guide | Document Name | | ---
+--------------------------------------------------------- | | [Using Web-UI]
+(docs/source_en/GetStarted/Web-ui.md) | | [Using Tuners](docs/source_en/
+GetStarted/Tuners.md) | | [LLM Inference](docs/source_en/LLM/LLM-inference.md)
+| | [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-tuning.md) | | [LLM
+Evaluation](docs/source_en/LLM/LLM-eval.md) | | [LLM Quantization](docs/
+source_en/LLM/LLM-quantization.md) | | [LLM Deployment](docs/source_en/LLM/
+VLLM-inference-acceleration-and-deployment.md) | | [DPO Human Alignment
+Training](docs/source_en/LLM/DPO.md) | | [ORPO Human Alignment Training](docs/
+source_en/LLM/ORPO.md) | | [AnimateDiff Training](docs/source_en/AIGC/
+AnimateDiff-train-infer.md) | ### Reference Documentation | Document Name | | -
+----------------------------------------------------------- | | [Command Line
+Arguments](docs/source_en/LLM/Command-line-parameters.md) | | [Supported Models
+and Datasets List](docs/source_en/LLM/Supported-models-datasets.md) | |
+[Customizing New Models and Datasets](docs/source_en/LLM/Customization.md) | |
+[Runtime Speed and Memory Benchmark](docs/source_en/LLM/Benchmark.md) | ###
+Best Practices | Best Practices Name | | --------------------------------------
+---------------------- | | [Agent Fine-Tuning Best Practice](docs/source_en/
+LLM/Agent-best-practice.md) | | [Self-Cognition Fine-Tuning Best Practice]
+(docs/source_en/LLM/Self-cognition-best-practice.md) | | [Qwen1.5 Best
+Practice](docs/source_en/LLM/Qwen1.5-best-practice.md) | | [Multi-Modal Model
+Training Best Practice](docs/source_en/Multi-Modal/index.md) | | [NPU Best
+Practice](docs/source_en/LLM/NPU-best-practice.md) | ### Deep Learning
+Tutorials | Tutorial Name | |--------------------------------------------------
+------------ | | [Introduction to Deep Learning](https://github.com/modelscope/
+modelscope-classroom/blob/main/LLM-tutorial/
 A.%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0%E5%85%A5%E9%97%A8%E4%BB%8B%E7%BB%8D.md)
 | | [Large Model Basics](https://github.com/modelscope/modelscope-classroom/
 blob/main/LLM-tutorial/
 B.%E9%AD%94%E6%90%AD%E7%A4%BE%E5%8C%BA%E5%92%8CLLM%E5%A4%A7%E6%A8%A1%E5%9E%8B%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md)
 | | [Prompt Engineering](https://github.com/modelscope/modelscope-classroom/
 blob/main/LLM-tutorial/C.%E6%8F%90%E7%A4%BA%E8%AF%8D%E5%B7%A5%E7%A8%8B-
 prompt%20engineering.md) | | [Transformer Architecture Introduction](https://
@@ -664,13 +712,13 @@
 K.%E5%A4%A7%E6%A8%A1%E5%9E%8B%E8%87%AA%E5%8A%A8%E8%AF%84%E4%BC%B0%E7%90%86%E8%AE%BA%E5%92%8C%E5%AE%9E%E6%88%98-
 -LLM%20Automatic%20Evaluation.md) | ## ð License This framework is licensed
 under the [Apache License (Version 2.0)](https://github.com/modelscope/
 modelscope/blob/master/LICENSE). For models and datasets, please refer to the
 original resource page and follow the corresponding License. ## ð Citation
 ```bibtex @Misc{swift, title = {SWIFT:Scalable lightWeight Infrastructure for
 Fine-Tuning}, author = {The ModelScope Team}, howpublished = {\url{https://
-github.com/modelscope/swift}}, year = {2024} } ``` ## â Contact Us You can
+github.com/modelscope/swift}}, year = {2024} } ``` ## â Wechat Group You can
 contact us and communicate with us by adding our WeChat group:
 [asset/wechat.png]
 ## Star History [![Star History Chart](https://api.star-history.com/
 svg?repos=modelscope/swift&type=Date)](https://star-history.com/#modelscope/
 swift&Date)
```

### Comparing `ms-swift-2.0.4/ms_swift.egg-info/PKG-INFO` & `ms-swift-2.0.5/ms_swift.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-swift
-Version: 2.0.4
+Version: 2.0.5
 Summary: Swift: Scalable lightWeight Infrastructure for Fine-Tuning
 Home-page: https://github.com/modelscope/swift
 Author: DAMO ModelScope teams
 Author-email: contact@modelscope.cn
 License: Apache License 2.0
 Description: # SWIFT (Scalable lightWeight Infrastructure for Fine-Tuning)
         
@@ -25,41 +25,63 @@
         <a href="https://github.com/modelscope/modelscope/"><img src="https://img.shields.io/badge/modelscope-%E2%89%A51.9.5-5D91D4.svg"></a>
         <a href="https://pypi.org/project/ms-swift/"><img src="https://badge.fury.io/py/ms-swift.svg"></a>
         <a href="https://github.com/modelscope/swift/blob/main/LICENSE"><img src="https://img.shields.io/github/license/modelscope/swift"></a>
         <a href="https://pepy.tech/project/ms-swift"><img src="https://pepy.tech/badge/ms-swift"></a>
         <a href="https://github.com/modelscope/swift/pulls"><img src="https://img.shields.io/badge/PR-welcome-55EB99.svg"></a>
         </p>
         
+        <p align="center">
+        <a href="https://trendshift.io/repositories/6427" target="_blank"><img src="https://trendshift.io/api/badge/repositories/6427" alt="modelscope%2Fswift | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>
+        </p>
+        
         ## 📖 Table of Contents
         - [Introduction](#-introduction)
         - [News](#-news)
         - [Installation](#%EF%B8%8F-installation)
         - [Getting Started](#-getting-started)
         - [Documentation](#-documentation)
         - [License](#-License)
         - [Citation](#-citation)
-        - [Contact Us](#-contact-us)
+        - [WeChat Group](#-Wechat-Group)
         
         ## 📝 Introduction
         SWIFT supports training, inference, evaluation and deployment of nearly **200 LLMs and MLLMs** (multimodal large models). Developers can directly apply our framework to their own research and production environments to realize the complete workflow from model training and evaluation to application. In addition to supporting the lightweight training solutions provided by [PEFT](https://github.com/huggingface/peft), we also provide a complete **Adapters library** to support the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This adapter library can be used directly in your own custom workflow without our training scripts.
         
         To facilitate use by users unfamiliar with deep learning, we provide a Gradio web-ui for controlling training and inference, as well as accompanying deep learning courses and best practices for beginners.
         
         Additionally, we are expanding capabilities for other modalities. Currently, we support full-parameter training and LoRA training for AnimateDiff.
         
+        SWIFT has rich documentations for users, please check [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM).
+        
+        SWIFT web-ui is available both on [Huggingface space](https://huggingface.co/spaces/tastelikefeet/swift) and [ModelScope studio](https://www.modelscope.cn/studios/iic/Scalable-lightWeight-Infrastructure-for-Fine-Tuning/summary), please feel free to try!
+        
         ## 🎉 News
+        - 2024.05.22: Supports DeepSeek-V2-Lite series models, model_type are `deepseek-v2-lite` and `deepseek-v2-lite-chat`
+        - 2024.05.22: Supports TeleChat-12B-v2 model with quantized version, model_type are `telechat-12b-v2` and `telechat-12b-v2-gptq-int4`
+        - 🔥2024.05.21: Inference and fine-tuning support for MiniCPM-Llama3-V-2_5 are now available. For more details, please refer to [minicpm-v-2.5 Best Practice](docs/source/Multi-Modal/minicpm-v-2.5最佳实践.md).
+        - 🔥2024.05.20: Support for inferencing and fine-tuning cogvlm2-llama3-chinese-chat-19B, cogvlm2-llama3-chat-19B. you can refer to [cogvlm2 Best Practice](docs/source_en/Multi-Modal/cogvlm2-best-practice.md).
+        - 🔥2024.05.17: Support peft=0.11.0. Meanwhile support 3 new tuners: `BOFT`, `Vera` and `Pissa`. use `--sft_type boft/vera` to use BOFT or Vera, use `--init_lora_weights pissa` with `--sft_type lora` to use Pissa.
+        - 2024.05.16: Supports Llava-Next (Stronger) series models. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-practice.md).
+        - 🔥2024.05.13: Support Yi-1.5 series models，use `--model_type yi-1_5-9b-chat` to begin!
+        - 2024.05.11: Support for qlora training and quantized inference using [hqq](https://github.com/mobiusml/hqq) and [eetq](https://github.com/NetEase-FuXi/EETQ). For more information, see the [LLM Quantization Documentation](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/LLM-quantization.md).
+        - 2024.05.10: Support split a sequence to multiple GPUs to reduce memory usage. Use this feature by `pip install .[seq_parallel]`, then add `--sequence_parallel_size n` to your DDP script to begin!
+        - 2024.05.08: Support DeepSeek-V2-Chat model, you can refer to [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/deepseek-v2-chat/lora_ddp_ds3/sft.sh).Support InternVL-Chat-V1.5-Int8 model, for best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/internvl-best-practice.md).
+        - 🔥2024.05.07: Supoprts **ORPO** training! See [document](https://github.com/modelscope/swift/blob/main/docs/source_en/LLM/ORPO.md) to start training!
+        - 2024.05.07: Supports Llava-Llama3 model from xtuner，model_type is `llava-llama-3-8b-v1_1`.
         - 2024.04.29: Supports inference and fine-tuning of InternVL-Chat-V1.5 model. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/internvl-best-practice.md).
         - 🔥2024.04.26: Support **LISA** and **unsloth** training! Specify `--lisa_activated_layers=2` to use LISA(to reduce the memory cost to 30 percent!), specify `--tuner_backend unsloth` to use unsloth to train a huge model(full or lora) with lesser memory(30 percent or lesser) and faster speed(5x)!
         - 🔥2024.04.26: Support the fine-tuning and inference of Qwen1.5-110B and Qwen1.5-110B-Chat model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_110b_chat/lora_ddp_ds/sft.sh) to start training!
         - 2024.04.24: Support for inference and fine-tuning of Phi3 series models. Including: [phi3-4b-4k-instruct](examples/pytorch/llm/scripts/phi3_4b_4k_instruct/lora), phi3-4b-128k-instruct.
         - 2024.04.22: Support for inference, fine-tuning, and deployment of **chinese-llama-alpaca-2** series models. This includes：chinese-llama-2-1.3b, chinese-llama-2-7b, chinese-llama-2-13b, chinese-alpaca-2-1.3b, chinese-alpaca-2-7b and chinese-alpaca-2-13b along with their corresponding 16k and 64k long text versions.
         - 2024.04.22: Support for inference and fine-tuning of Llama3 GPTQ-Int4, GPTQ-Int8, and AWQ series models. Support for inference and fine-tuning of chatglm3-6b-128k, Openbuddy-Llama3.
         - 2024.04.20: Support for inference, fine-tuning, and deployment of **Atom** series models. This includes: Atom-7B and Atom-7B-Chat. use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/atom_7b_chat/lora/sft.sh) to train.
-        - 2024.04.19: Support for single-card, DDP, ZeRO2, and ZeRO3 training and inference with NPU, please refer to [NPU Inference and Fine-tuning Best Practices](docs/source_en/LLM/NPU-best-practice.md).
+        - 2024.04.19: Support for single-card, DDP, ZeRO2, and ZeRO3 training and inference with NPU, please refer to [NPU Inference and Fine-tuning Best Practice](docs/source_en/LLM/NPU-best-practice.md).
         - 2024.04.19: Support for inference, fine-tuning, and deployment of **Llama3** series models. This includes: Llama-3-8B, Llama-3-8B-Instruct, Llama-3-70B, and Llama-3-70B-Instruct. use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama3_8b_instruct/lora/sft.sh) to train.
+        <details><summary>More</summary>
+        
         - 2024.04.18: Supported models: wizardlm2-7b-awq, wizardlm2-8x22b, yi-6b-chat-awq, yi-6b-chat-int8, yi-34b-chat-awq, yi-34b-chat-int8. Supported `--deepspeed zero3-offload` and provided default zero3-offload configuration file for zero3+cpu offload usage.
         - 2024.04.18: Supported compatibility with HuggingFace ecosystem using the environment variable `USE_HF`, switching to use models and datasets from HF. Please refer to the [HuggingFace ecosystem compatibility documentation](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Compat-HF.md).
         - 2024.04.17: Support the evaluation for OpenAI standard interfaces. Check the [parameter documentation](docs/source_en/LLM/Command-line-parameters.md#eval-parameters) for details.
         - 🔥2024.04.17: Support **CodeQwen1.5-7B** series: CodeQwen1.5-7B, CodeQwen1.5-7B-Chat,CodeQwen1.5-7B-Chat-AWQ, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/codeqwen1half_7b_chat/lora/sft.sh) to train.
         - 2024.04.16: Supports inference and fine-tuning of llava-v1.6-34b model. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-practice.md).
         - 2024.04.13: Support the fine-tuning and inference of Mixtral-8x22B-v0.1 model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mixtral_moe_8x22b_v1/lora_ddp_ds/sft.sh) to start training!
         - 2024.04.13: Support the newly launched **MiniCPM** series: MiniCPM-V-2.0、MiniCPM-2B-128k、MiniCPM-MoE-8x2B and MiniCPM-1B.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/minicpm_moe_8x2b/lora_ddp/sft.sh) to start training!
@@ -72,16 +94,14 @@
         - 🔥2024.04.03: Support **Qwen1.5-32B** series: Qwen1.5-32B, Qwen1.5-32B-Chat, Qwen1.5-32B-Chat-GPTQ-Int4.use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_32b_chat/lora_mp/sft.sh) to start training!
         - 🔥2024.04.02: Support the fine-tuning and inference of Mengzi3-13B-Base model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mengzi3_13b_base/lora_ddp_ds/sft.sh) to start training!
         - 🔥2024.04.01: Support **dbrx** series: dbrx-base and dbrx-instruct, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/dbrx-instruct/lora_mp/sft.sh) to start training!
         - 🔥2024.03.29: Support **Qwen1.5-MoE** series: Qwen1.5-MoE-A2.7B, Qwen1.5-MoE-A2.7B-Chat, Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4.
         - 🔥2024.03.29: Support the fine-tuning and inference of **Grok-1** 300B MoE, please view details [here](https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-practice.md).
         - 🔥2024.03.25: Supports inference and fine-tuning of TeleChat-7b and TeleChat-12b model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start training!
         - 🔥2024.03.20: Supports inference and fine-tuning for the **llava** series. For best practice, you can refer to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-practice.md).
-        <details><summary>More</summary>
-        
         - 🔥2024.03.12: Support inference and fine-tuning for **deepseek-vl** series. Best practices can be found [here](docs/source_en/Multi-Modal/deepseek-vl-best-practice.md).
         - 🔥2024.03.11: Support [GaLore](https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/2 of the original in full-parameter training.
         - 🔥2024.03.10: [End-to-end best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat.
         - 🔥2024.03.09: Support training and inference of MAMBA model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/mamba-1.4b/lora/sft.sh) to start training!
         - 2024.03.09: Support training and inference of AQLM quantized model, use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/llama2_7b_aqlm_2bit_1x16/lora/sft.sh) to start training!
         - 2024.03.06: Support training and inference of AWQ quantized model, use [this Qwen1.5-AWQ model script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/qwen1half_7b_chat_awq/lora/sft.sh) to start training, and support training and inference of [yi-9b](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_9b/lora_zero3).
         - 🔥2024.02.29: Support [LLaMA PRO](https://arxiv.org/pdf/2401.02415.pdf), simply use [this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/yi_6b_chat/llamapro/sft.sh) to start training.
@@ -104,18 +124,17 @@
         - 2024.01.24: Support codefuse-codegeex2-6b-chat, codefuse-qwen-14b-chat.
         - 2024.01.23: Support orion series: orion-14b, [orion-14b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/orion_14b_chat).
         - 2024.01.20: Support [xverse-13b-256k](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/xverse_13b_256k), xverse-65b-v2, xverse-65b-chat.
         - 🔥2024.01.17: Support internlm2 series: internlm2-7b-base, internlm2-7b, [internlm2-7b-sft-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/internlm2_7b_sft_chat), internlm2-7b-chat, internlm2-20b-base, internlm2-20b, internlm2-20b-sft-chat, internlm2-20b-chat.
         - 2024.01.15: Support yuan series: yuan2-2b-instruct, [yuan2-2b-janus-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/yuan2_2b_janus_instruct), yuan2-51b-instruct, yuan2-102b-instruct.
         - 🔥2024.01.12: Support **deepseek-moe** series: deepseek-moe-16b, [deepseek-moe-16b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/deepseek_moe_16b_chat).
         - 🔥2024.01.04: Support **VLLM deployment**, compatible with **OpenAI API** style, see [VLLM Inference Acceleration and Deployment](https://github.com/modelscope/swift/blob/main/docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md#Deployment) for details.
-        
         - 2024.01.04: Update [Benchmark](https://github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) for convenient viewing of training speed and memory usage of different models.
         - 🔥2023.12.29: Support web-ui for sft training and inference, use `swift web-ui` after installing ms-swift to start.
-        - 🔥2023.12.29: Support DPO RLHF (Reinforcement Learning from Human Feedback) and three datasets for this task: AI-ModelScope/stack-exchange-paired, AI-ModelScope/hh-rlhf and AI-ModelScope/hh_rlhf_cn. See [documentation](https://github.com/modelscope/swift/blob/main/docs/source/LLM/LLM%E4%BA%BA%E7%B1%BB%E5%AF%B9%E9%BD%90%E8%AE%AD%E7%BB%83%E6%96%87%E6%A1%A3.md) to start training!
+        - 🔥2023.12.29: Support DPO RLHF (Reinforcement Learning from Human Feedback) and three datasets for this task: AI-ModelScope/stack-exchange-paired, AI-ModelScope/hh-rlhf and AI-ModelScope/hh_rlhf_cn. See [documentation](https://github.com/modelscope/swift/blob/main/docs/source_en/LLM/DPO.md) to start training!
         - 🔥2023.12.28: Support SCEdit! This tuner can significantly reduce memory usage in U-Net and support low-memory controllable image generation (replacing ControlNet), read the section below to learn more.
         - 2023.12.23: Support [codegeex2-6b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/codegeex2_6b).
         - 2023.12.19: Support [phi2-3b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/phi2_3b).
         - 2023.12.18: Support VLLM for inference acceleration.
         - 2023.12.15: Support deepseek, deepseek-coder series: deepseek-7b, deepseek-7b-chat, deepseek-67b, deepseek-67b-chat, openbuddy-deepseek-67b-chat, deepseek-coder-1_3b, deepseek-coder-1_3b-instruct, deepseek-coder-6_7b, deepseek-coder-6_7b-instruct, deepseek-coder-33b, deepseek-coder-33b-instruct.
         - 2023.12.13: Support mistral-7b-instruct-v2, [mixtral-moe-7b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/mixtral_7b_moe), [mixtral-moe-7b-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/mixtral_7b_moe_instruct).
         - 2023.12.09: Support `freeze_parameters` parameter as a compromise between lora and full-parameter training. Corresponding sh can be found in [full_freeze_ddp](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/full_freeze_ddp). Support `disable_tqdm`, `lazy_tokenize`, `preprocess_num_proc` parameters, see [command line arguments](https://github.com/modelscope/swift/blob/main/docs/source/LLM/%E5%91%BD%E4%BB%A4%E8%A1%8C%E5%8F%82%E6%95%B0.md) for details.
@@ -187,18 +206,22 @@
         
         ## 🚀 Getting Started
         
         This section introduces basic usage, see the [Documentation](#-documentation) section for more ways to use.
         
         ### Web-UI
         
+        Web-UI is a gradio-based interface for **zero-threshold** training and deployment. It is easy to use and perfectly supports multi-GPU training and deployment:
+        
         ```shell
-        swift web-ui
+        SWIFT_UI_LANG=en swift web-ui
         ```
         
+        ![image.png](./docs/resources/web-ui-en.jpg)
+        
         ### Training
         
         #### Training Scripts
         You can refer to the following scripts to customize your own training script.
         
         - full: [qwen1half-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat/full) (A100), [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/full_mp) (2\*A100)
         - full+ddp+zero2: [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/full_ddp_zero2) (4\*A100)
@@ -213,15 +236,15 @@
         
         #### Supported Training Processes
         
         | Training Process | Training Method                                                               |
         |------------------|-------------------------------------------------------------------------------|
         | Pretraining      | Text Generation                                                               |
         | Fine-tuning      | Single-turn/Multi-turn<br>Agent Training/Self-cognition<br>Multi-modal Vision/Multi-modal Speech|
-        | Human Alignment  | DPO                                                                           |
+        | Human Alignment  | DPO<br>ORPO                                                                   |
         | Text-to-Image    | DreamBooth, etc.                                                              |
         | Text-to-Video    | -                                                                             |
         
         #### Single GPU Training
         
         Start single GPU fine-tuning with the following command:
         
@@ -380,14 +403,28 @@
             --model_id_or_path qwen1half-32b-chat \
             --sft_type full \
             --dataset blossom-math-zh \
             --output_dir output \
             --deepspeed default-zero3 \
         ```
         
+        ##### AliYun-DLC multi-node training
+        In DLC product, WORLD_SIZE is the node number, RANK is the node index, this is different from the definition of torchrun.
+        
+        ```shell
+        NNODES=$WORLD_SIZE \
+        NODE_RANK=$RANK \
+        swift sft \
+            --model_id_or_path qwen1half-32b-chat \
+            --sft_type full \
+            --dataset blossom-math-zh \
+            --output_dir output \
+            --deepspeed default-zero3
+        ```
+        
         
         ### Inference
         Original model:
         ```shell
         CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat
         # use VLLM
         CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat \
@@ -455,17 +492,17 @@
         | ChatGLM2<br>ChatGLM3<br>Codegeex2                    | [Zhipu ChatGLM series models](https://github.com/THUDM)               | Chinese<br>English    | 6B                                     | base model<br>chat model<br>code model<br>long text model  |
         | Baichuan/Baichuan2                             | [Baichuan 1 and Baichuan 2](https://github.com/baichuan-inc)           | Chinese<br>English    | 7B-13B<br>including quantized versions             | base model<br>chat model                       |
         | Yuan2                                          | [Langchao Yuan series models](https://github.com/IEIT-Yuan)             | Chinese<br>English    | 2B-102B                                | instruct model                                 |
         | XVerse                                         | [XVerse series models](https://github.com/xverse-ai)                    | Chinese<br>English    | 7B-65B                                 | base model<br>chat model<br>long text model<br>MoE model                |
         | LLaMA2                                         | [LLaMA2 series models](https://github.com/facebookresearch/llama)       | English            | 7B-70B<br>including quantized versions   | base model<br>chat model                       |
         | LLaMA3                   | [LLaMA3 series models](https://github.com/meta-llama/llama3)  | English       | 8B-70B<br>including quantized versions      | base model<br>chat model              |
         | Mistral<br>Mixtral                            | [Mistral series models](https://github.com/mistralai/mistral-src)       | English            | 7B-22B     | base model<br>instruct model<br>MoE model                     |
-        | YI                                             | [01AI's YI series models](https://github.com/01-ai)                     | Chinese<br>English    | 6B-34B<br>including quantized             | base model<br>chat model<br>long text model            |
+        | Yi<br>Yi1.5                                      | [01AI's YI series models](https://github.com/01-ai)                     | Chinese<br>English    | 6B-34B<br>including quantized             | base model<br>chat model<br>long text model            |
         | InternLM<br>InternLM2<br>InternLM2-Math              | [Pujiang AI Lab InternLM series models](https://github.com/InternLM/InternLM) | Chinese<br>English | 1.8B-20B                            | base model<br>chat model<br>math model            |
-        | DeepSeek<br>DeepSeek-MoE<br>DeepSeek-Coder<br>DeepSeek-Math          | [DeepSeek series models](https://github.com/deepseek-ai)       | Chinese<br>English    | 1.3B-67B                               | base model<br>chat model<br>MoE model<br>code model<br>math model |
+        | DeepSeek<br>DeepSeek-MoE<br>DeepSeek-Coder<br>DeepSeek-Math<br>DeepSeek-V2          | [DeepSeek series models](https://github.com/deepseek-ai)       | Chinese<br>English    | 1.3B-236B                               | base model<br>chat model<br>MoE model<br>code model<br>math model |
         | MAMBA                                          | [MAMBA temporal convolution model](https://github.com/state-spaces/mamba) | English          | 130M-2.8B                              | base model                                 |
         | Gemma                                          | [Google Gemma series models](https://github.com/google/gemma_pytorch)   | English            | 2B-7B                                  | base model<br>instruct model                       |
         | MiniCPM                                        | [OpenBmB MiniCPM series models](https://github.com/OpenBMB/MiniCPM)     | Chinese<br>English    | 2B-3B                                  | chat model<br>MoE model                                 |
         | OpenBuddy                                      | [OpenBuddy series models](https://github.com/OpenBuddy/OpenBuddy)       | Chinese<br>English    | 7B-67B                                 | base model<br>chat model                       |
         | Orion                                          | [OrionStar AI series models](https://github.com/OrionStarAI)            | Chinese<br>English    | 14B                                    | base model<br>chat model                       |
         | BlueLM                                         | [VIVO BlueLM large model](https://github.com/vivo-ai-lab/BlueLM)        | Chinese<br>English    | 7B                                     | base model<br>chat model                       |
         | Ziya2                                          | [Fengshenbang series models](https://github.com/IDEA-CCNL/Fengshenbang-LM) | Chinese<br>English  | 13B                                    | base model<br>chat model                       |
@@ -486,52 +523,54 @@
         | Atom | [Atom](https://github.com/LlamaFamily/Llama-Chinese) | Chinese | 7B| base model<br>chat model|
         | Chinese-LLaMA-Alpaca-2 | [Chinese-LLaMA-Alpaca-2](https://github.com/ymcui/Chinese-LLaMA-Alpaca-2) | Chinese | 1.3B-13B| base model<br>chat model<br>long text model |
         | Chinese-LLaMA-Alpaca-3 | [Chinese-LLaMA-Alpaca-3](https://github.com/ymcui/Chinese-LLaMA-Alpaca-3) | Chinese | 8B| base model<br>chat model|
         | ModelScope-Agent | [ModelScope Agent series models](https://github.com/modelscope/modelscope-agent) | Chinese | 7B-14B| agent model |
         
         #### MLLMs
         
-        | Model Type       | Model Introduction                                                     | Language           | Model Size        | Model Type         |
+        | Model Type         | Model Introduction                                                           | Language           | Model Size                         | Model Type         |
         |------------------|------------------------------------------------------------------------|--------------------|-------------------|------------------- |
-        | Qwen-VL          | [Tongyi Qwen vision model](https://github.com/QwenLM)               | Chinese<br>English    | 7B<br>including quantized versions | base model<br>chat model |
-        | Qwen-Audio       | [Tongyi Qwen speech model](https://github.com/QwenLM)               | Chinese<br>English    | 7B                | base model<br>chat model |
-        | YI-VL            | [01AI's YI series vision models](https://github.com/01-ai)             | Chinese<br>English    | 6B-34B            | chat model         |
-        | XComposer2       | [Pujiang AI Lab InternLM vision model](https://github.com/InternLM/InternLM) | Chinese<br>English | 7B              | chat model         |
-        | DeepSeek-VL      | [DeepSeek series vision models](https://github.com/deepseek-ai) | Chinese<br>English    | 1.3B-7B           | chat model         |
-        | MiniCPM-V       | [OpenBmB MiniCPM vision model](https://github.com/OpenBMB/MiniCPM)     | Chinese<br>English    | 3B                | chat model         |
-        | CogVLM<br>CogAgent  | [Zhipu ChatGLM visual QA and Agent model](https://github.com/THUDM/)   | English    | 17B-18B           | chat model         |
-        | Llava      | [Llava series models](https://github.com/haotian-liu/LLaVA)                | English | 7B-34B               | chat model |
-        | mPLUG-Owl      | [mPLUG-Owl series models](https://github.com/X-PLUG/mPLUG-Owl)         | English | 11B               | chat model |
-        | InternVL         | [InternVL](https://github.com/OpenGVLab/InternVL)                | Chinese<br>English | 25.5B | chat model |
+        | Qwen-VL            | [Tongyi Qwen vision model](https://github.com/QwenLM)                        | Chinese<br>English    | 7B<br>including quantized versions | base model<br>chat model |
+        | Qwen-Audio         | [Tongyi Qwen speech model](https://github.com/QwenLM)                        | Chinese<br>English    | 7B                                 | base model<br>chat model |
+        | YI-VL              | [01AI's YI series vision models](https://github.com/01-ai)                   | Chinese<br>English    | 6B-34B                             | chat model         |
+        | XComposer2         | [Pujiang AI Lab InternLM vision model](https://github.com/InternLM/InternLM) | Chinese<br>English | 7B                                 | chat model         |
+        | DeepSeek-VL        | [DeepSeek series vision models](https://github.com/deepseek-ai)              | Chinese<br>English    | 1.3B-7B                            | chat model         |
+        | MiniCPM-V<br>MiniCPM-V-2<br>MiniCPM-V-2_5  | [OpenBmB MiniCPM vision model](https://github.com/OpenBMB/MiniCPM) | Chinese<br>English | 3B-9B            | chat model          |
+        | CogVLM<br>CogVLM2<br>CogAgent | [Zhipu ChatGLM visual QA and Agent model](https://github.com/THUDM/)         | Chinese<br>English    | 17B-19B                            | chat model         |
+        | Llava              | [Llava series models](https://github.com/haotian-liu/LLaVA)                  | English | 7B-34B                             | chat model |
+        | Llava-Next              | [Llava-Next series models](https://github.com/LLaVA-VL/LLaVA-NeXT)                  | Chinese<br>English | 8B-110B                             | chat model |
+        | mPLUG-Owl          | [mPLUG-Owl series models](https://github.com/X-PLUG/mPLUG-Owl)               | English | 11B                                | chat model |
+        | InternVL           | [InternVL](https://github.com/OpenGVLab/InternVL)                            | Chinese<br>English | 25.5B<br>including quantized version                              | chat model |
+        | Llava-llama3       | [xtuner](https://huggingface.co/xtuner/llava-llama-3-8b-v1_1-transformers)   | English | 8B                                 | chat model |
         
         #### Diffusion Models
         
         | Model Type          | Model Introduction                                                    | Language | Model Type        |
         |---------------------|----------------------------------------------------------------------|----------|------------------ |
         | AnimateDiff         | [AnimateDiff animation model](https://github.com/guoyww/AnimateDiff) | English  | text-to-video     |
         | SD1.5/SD2.0/SDXL    | [StabilityAI series diffusion models](https://github.com/Stability-AI) | English | text-to-image    |
         
         ### Supported Open Source Datasets
         
         | Dataset Type | Training Task  | Documentation                                                                                                                                                                                                                                                                                                        |
         |--------------|:---------------|--------------------------------------------------------------- |
-        | General      | Fine-tuning    | 🔥ruozhiba, 🔥ms-bench, 🔥ms-bench-mini, 🔥alpaca-en(gpt4), 🔥alpaca-zh(gpt4), multi-alpaca-all, instinwild-en, instinwild-zh, cot-en, cot-zh, firefly-all-zh, instruct-en, gpt4all-en, sharegpt-en, sharegpt-zh, tulu-v2-sft-mixture, wikipedia-zh, open-orca, open-orca-gpt4, sharegpt-gpt4, 🔥sharegpt-gpt4-mini. |
-        | Agent        | Fine-tuning    | 🔥ms-agent, ms-agent-for-agentfabric-default, ms-agent-for-agentfabric-addition, damo-mini-agent-zh, damo-agent-zh, agent-instruct-all-en.                                                                                                                                                                                                                                                |
-        | General      | Human Alignment | 🔥hh-rlhf-cn, stack-exchange-paired, hh-rlhf-harmless-base, hh-rlhf-helpful-base, hh-rlhf-helpful-online, hh-rlhf-helpful-rejection-sampled, hh-rlhf-red-team-attempts, hh-rlhf-cn-harmless-base-cn, hh-rlhf-cn-helpful-base-cn, hh-rlhf-cn-harmless-base-en, hh-rlhf-cn-helpful-base-en.                            |
-        | Code         | Fine-tuning    | code-alpaca-en, 🔥leetcode-python-en, 🔥codefuse-python-en, 🔥codefuse-evol-instruction-zh.                                                                                                                                                                                                                          |
-        | Medical      | Fine-tuning    | medical-en, medical-zh, medical-mini-zh, 🔥disc-med-sft-zh.                                                                                                                                                                                                                                                          |
-        | Legal        | Fine-tuning    | lawyer-llama-zh, tigerbot-law-zh, 🔥disc-law-sft-zh.                                                                                                                                                                                                                                                                 |
-        | Math         | Fine-tuning    | 🔥blossom-math-zh, school-math-zh, open-platypus-en.                                                                                                                                                                                                                                                                 |
-        | SQL          | Fine-tuning    | text2sql-en, 🔥sql-create-context-en.                                                                                                                                                                                                                                                                                |
-        | Text Generation | Fine-tuning | 🔥advertise-gen-zh, 🔥dureader-robust-zh.                                                                                                                                                                                                                                                                            |
-        | Classification | Fine-tuning  | cmnli-zh, 🔥cmnli-mini-zh, 🔥jd-sentiment-zh, 🔥hc3-zh, 🔥hc3-en.                                                                                                                                                                                                                                                    |
-        | Quantization Assist | Quantization | pileval.                                                                                                                                                                                                                                                                                                             |
-        | Other        | Fine-tuning    | finance-en, poetry-zh, webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-jave-zh.                                                                                                                                                                                                                               |
-        | Vision       | Fine-tuning    | coco-en, 🔥coco-mini-en, coco-mini-en-2, capcha-images.                                                                                                                                                                                                                                                              |
-        | Audio        | Fine-tuning    | aishell1-zh, 🔥aishell1-mini-zh.                                                                                                                                                                                                                                                                                     |
+        | General      | Fine-tuning    | 🔥ruozhiba, 🔥ms-bench, 🔥alpaca-en(gpt4), 🔥alpaca-zh(gpt4), multi-alpaca, instinwild, cot-en, cot-zh, firefly-zh, instruct-en, gpt4all-en, sharegpt, tulu-v2-sft-mixture, wikipedia-zh, open-orca, sharegpt-gpt4, deepctrl-sft, coig-cqia. |
+        | Agent        | Fine-tuning    | 🔥ms-agent, 🔥ms-agent-for-agentfabric, ms-agent-multirole, 🔥toolbench-for-alpha-umi, damo-agent-zh, damo-agent-zh-mini, agent-instruct-all-en.                    |
+        | General      | Human Alignment | hh-rlhf, 🔥hh-rlhf-cn, stack-exchange-paired.                            |
+        | Code         | Fine-tuning    | code-alpaca-en, 🔥leetcode-python-en, 🔥codefuse-python-en, 🔥codefuse-evol-instruction-zh.    |
+        | Medical      | Fine-tuning    | medical-en, medical-zh, 🔥disc-med-sft-zh.               |
+        | Legal        | Fine-tuning    | lawyer-llama-zh, tigerbot-law-zh, 🔥disc-law-sft-zh.               |
+        | Math         | Fine-tuning    | 🔥blossom-math-zh, school-math-zh, open-platypus-en.                      |
+        | SQL          | Fine-tuning    | text2sql-en, 🔥sql-create-context-en.                                    |
+        | Text Generation | Fine-tuning | 🔥advertise-gen-zh, 🔥dureader-robust-zh.                            |
+        | Classification | Fine-tuning  | cmnli-zh, 🔥jd-sentiment-zh, 🔥hc3-zh, 🔥hc3-en.           |
+        | Quantization Assist | Quantization | pileval.  |
+        | Other        | Fine-tuning    | finance-en, poetry-zh, webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-jave-zh.   |
+        | Vision       | Fine-tuning    | coco-en, 🔥coco-en-mini, coco-en-2, coco-en-2-mini, capcha-images.         |
+        | Audio        | Fine-tuning    | aishell1-zh, 🔥aishell1-zh-mini.       |
         
         ### Supported Technologies
         
         | Technology Name                                              |
         | ------------------------------------------------------------ |
         | 🔥LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE MODELS](https://arxiv.org/abs/2106.09685) |
         | 🔥LoRA+: [LoRA+: Efficient Low Rank Adaptation of Large Models](https://arxiv.org/pdf/2402.12354.pdf) |
@@ -574,15 +613,16 @@
         | [Using Web-UI](docs/source_en/GetStarted/Web-ui.md)          |
         | [Using Tuners](docs/source_en/GetStarted/Tuners.md)          |
         | [LLM Inference](docs/source_en/LLM/LLM-inference.md)         |
         | [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-tuning.md)     |
         | [LLM Evaluation](docs/source_en/LLM/LLM-eval.md)     |
         | [LLM Quantization](docs/source_en/LLM/LLM-quantization.md)   |
         | [LLM Deployment](docs/source_en/LLM/VLLM-inference-acceleration-and-deployment.md) |
-        | [DPO Human Alignment Training](docs/source_en/LLM/RLHF.md)   |
+        | [DPO Human Alignment Training](docs/source_en/LLM/DPO.md)   |
+        | [ORPO Human Alignment Training](docs/source_en/LLM/ORPO.md)   |
         | [AnimateDiff Training](docs/source_en/AIGC/AnimateDiff-train-infer.md) |
         
         ### Reference Documentation
         | Document Name                                                |
         | ------------------------------------------------------------ |
         | [Command Line Arguments](docs/source_en/LLM/Command-line-parameters.md) |
         | [Supported Models and Datasets List](docs/source_en/LLM/Supported-models-datasets.md) |
@@ -628,15 +668,15 @@
           title = {SWIFT:Scalable lightWeight Infrastructure for Fine-Tuning},
           author = {The ModelScope Team},
           howpublished = {\url{https://github.com/modelscope/swift}},
           year = {2024}
         }
         ```
         
-        ## ☎ Contact Us
+        ## ☎ Wechat Group
         
         You can contact us and communicate with us by adding our WeChat group:
         
         <p align="left">
         <img src="asset/wechat.png" width="250" style="display: inline-block;">
         </p>
         
@@ -654,8 +694,9 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 Provides-Extra: llm
 Provides-Extra: aigc
 Provides-Extra: eval
+Provides-Extra: seq_parallel
 Provides-Extra: all
```

#### html2text {}

```diff
@@ -1,69 +1,106 @@
-Metadata-Version: 2.1 Name: ms-swift Version: 2.0.4 Summary: Swift: Scalable
+Metadata-Version: 2.1 Name: ms-swift Version: 2.0.5 Summary: Swift: Scalable
 lightWeight Infrastructure for Fine-Tuning Home-page: https://github.com/
 modelscope/swift Author: DAMO ModelScope teams Author-email:
 contact@modelscope.cn License: Apache License 2.0 Description: # SWIFT
 (Scalable lightWeight Infrastructure for Fine-Tuning)
 
                             [resources/banner.png]
                          _M_o_d_e_l_S_c_o_p_e_ _C_o_m_m_u_n_i_t_y_ _W_e_b_s_i_t_e
                            _ä_¸_­_æ__   ï½   English  
       [https://img.shields.io/badge/python-%E2%89%A53.8-5be.svg][https://
   img.shields.io/badge/pytorch-%E2%89%A51.12%20%7C%20%E2%89%A52.0-orange.svg]
  _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_m_o_d_e_l_s_c_o_p_e_-_%_E_2_%_8_9_%_A_5_1_._9_._5_-_5_D_9_1_D_4_._s_v_g_]_[_h_t_t_p_s_:_/_/
      _b_a_d_g_e_._f_u_r_y_._i_o_/_p_y_/_m_s_-_s_w_i_f_t_._s_v_g_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/
   _m_o_d_e_l_s_c_o_p_e_/_s_w_i_f_t_]_[_h_t_t_p_s_:_/_/_p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_m_s_-_s_w_i_f_t_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
                          _b_a_d_g_e_/_P_R_-_w_e_l_c_o_m_e_-_5_5_E_B_9_9_._s_v_g_]
+                       _[_m_o_d_e_l_s_c_o_p_e_%_2_F_s_w_i_f_t_ _|_ _T_r_e_n_d_s_h_i_f_t_]
 ## ð Table of Contents - [Introduction](#-introduction) - [News](#-news) -
 [Installation](#%EF%B8%8F-installation) - [Getting Started](#-getting-started)
 - [Documentation](#-documentation) - [License](#-License) - [Citation](#-
-citation) - [Contact Us](#-contact-us) ## ð Introduction SWIFT supports
+citation) - [WeChat Group](#-Wechat-Group) ## ð Introduction SWIFT supports
 training, inference, evaluation and deployment of nearly **200 LLMs and MLLMs**
 (multimodal large models). Developers can directly apply our framework to their
 own research and production environments to realize the complete workflow from
 model training and evaluation to application. In addition to supporting the
 lightweight training solutions provided by [PEFT](https://github.com/
 huggingface/peft), we also provide a complete **Adapters library** to support
 the latest training techniques such as NEFTune, LoRA+, LLaMA-PRO, etc. This
 adapter library can be used directly in your own custom workflow without our
 training scripts. To facilitate use by users unfamiliar with deep learning, we
 provide a Gradio web-ui for controlling training and inference, as well as
 accompanying deep learning courses and best practices for beginners.
 Additionally, we are expanding capabilities for other modalities. Currently, we
-support full-parameter training and LoRA training for AnimateDiff. ## ð News
-- 2024.04.29: Supports inference and fine-tuning of InternVL-Chat-V1.5 model.
-For best practice, you can refer to [here](https://github.com/modelscope/swift/
-tree/main/docs/source_en/Multi-Modal/internvl-best-practice.md). -
-ð¥2024.04.26: Support **LISA** and **unsloth** training! Specify `--
-lisa_activated_layers=2` to use LISA(to reduce the memory cost to 30 percent!),
-specify `--tuner_backend unsloth` to use unsloth to train a huge model(full or
-lora) with lesser memory(30 percent or lesser) and faster speed(5x)! -
-ð¥2024.04.26: Support the fine-tuning and inference of Qwen1.5-110B and
-Qwen1.5-110B-Chat model, use [this script](https://github.com/modelscope/swift/
-blob/main/examples/pytorch/llm/scripts/qwen1half_110b_chat/lora_ddp_ds/sft.sh)
-to start training! - 2024.04.24: Support for inference and fine-tuning of Phi3
-series models. Including: [phi3-4b-4k-instruct](examples/pytorch/llm/scripts/
+support full-parameter training and LoRA training for AnimateDiff. SWIFT has
+rich documentations for users, please check [here](https://github.com/
+modelscope/swift/tree/main/docs/source_en/LLM). SWIFT web-ui is available both
+on [Huggingface space](https://huggingface.co/spaces/tastelikefeet/swift) and
+[ModelScope studio](https://www.modelscope.cn/studios/iic/Scalable-lightWeight-
+Infrastructure-for-Fine-Tuning/summary), please feel free to try! ## ð News
+- 2024.05.22: Supports DeepSeek-V2-Lite series models, model_type are
+`deepseek-v2-lite` and `deepseek-v2-lite-chat` - 2024.05.22: Supports TeleChat-
+12B-v2 model with quantized version, model_type are `telechat-12b-v2` and
+`telechat-12b-v2-gptq-int4` - ð¥2024.05.21: Inference and fine-tuning support
+for MiniCPM-Llama3-V-2_5 are now available. For more details, please refer to
+[minicpm-v-2.5 Best Practice](docs/source/Multi-Modal/minicpm-v-
+2.5æä½³å®è·µ.md). - ð¥2024.05.20: Support for inferencing and fine-tuning
+cogvlm2-llama3-chinese-chat-19B, cogvlm2-llama3-chat-19B. you can refer to
+[cogvlm2 Best Practice](docs/source_en/Multi-Modal/cogvlm2-best-practice.md). -
+ð¥2024.05.17: Support peft=0.11.0. Meanwhile support 3 new tuners: `BOFT`,
+`Vera` and `Pissa`. use `--sft_type boft/vera` to use BOFT or Vera, use `--
+init_lora_weights pissa` with `--sft_type lora` to use Pissa. - 2024.05.16:
+Supports Llava-Next (Stronger) series models. For best practice, you can refer
+to [here](https://github.com/modelscope/swift/tree/main/docs/source_en/Multi-
+Modal/llava-best-practice.md). - ð¥2024.05.13: Support Yi-1.5 series
+modelsï¼use `--model_type yi-1_5-9b-chat` to begin! - 2024.05.11: Support for
+qlora training and quantized inference using [hqq](https://github.com/mobiusml/
+hqq) and [eetq](https://github.com/NetEase-FuXi/EETQ). For more information,
+see the [LLM Quantization Documentation](https://github.com/modelscope/swift/
+tree/main/docs/source_en/LLM/LLM-quantization.md). - 2024.05.10: Support split
+a sequence to multiple GPUs to reduce memory usage. Use this feature by `pip
+install .[seq_parallel]`, then add `--sequence_parallel_size n` to your DDP
+script to begin! - 2024.05.08: Support DeepSeek-V2-Chat model, you can refer to
+[this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/
+llm/scripts/deepseek-v2-chat/lora_ddp_ds3/sft.sh).Support InternVL-Chat-V1.5-
+Int8 model, for best practice, you can refer to [here](https://github.com/
+modelscope/swift/tree/main/docs/source_en/Multi-Modal/internvl-best-
+practice.md). - ð¥2024.05.07: Supoprts **ORPO** training! See [document]
+(https://github.com/modelscope/swift/blob/main/docs/source_en/LLM/ORPO.md) to
+start training! - 2024.05.07: Supports Llava-Llama3 model from
+xtunerï¼model_type is `llava-llama-3-8b-v1_1`. - 2024.04.29: Supports
+inference and fine-tuning of InternVL-Chat-V1.5 model. For best practice, you
+can refer to [here](https://github.com/modelscope/swift/tree/main/docs/
+source_en/Multi-Modal/internvl-best-practice.md). - ð¥2024.04.26: Support
+**LISA** and **unsloth** training! Specify `--lisa_activated_layers=2` to use
+LISA(to reduce the memory cost to 30 percent!), specify `--tuner_backend
+unsloth` to use unsloth to train a huge model(full or lora) with lesser memory
+(30 percent or lesser) and faster speed(5x)! - ð¥2024.04.26: Support the
+fine-tuning and inference of Qwen1.5-110B and Qwen1.5-110B-Chat model, use
+[this script](https://github.com/modelscope/swift/blob/main/examples/pytorch/
+llm/scripts/qwen1half_110b_chat/lora_ddp_ds/sft.sh) to start training! -
+2024.04.24: Support for inference and fine-tuning of Phi3 series models.
+Including: [phi3-4b-4k-instruct](examples/pytorch/llm/scripts/
 phi3_4b_4k_instruct/lora), phi3-4b-128k-instruct. - 2024.04.22: Support for
 inference, fine-tuning, and deployment of **chinese-llama-alpaca-2** series
 models. This includesï¼chinese-llama-2-1.3b, chinese-llama-2-7b, chinese-
 llama-2-13b, chinese-alpaca-2-1.3b, chinese-alpaca-2-7b and chinese-alpaca-2-
 13b along with their corresponding 16k and 64k long text versions. -
 2024.04.22: Support for inference and fine-tuning of Llama3 GPTQ-Int4, GPTQ-
 Int8, and AWQ series models. Support for inference and fine-tuning of chatglm3-
 6b-128k, Openbuddy-Llama3. - 2024.04.20: Support for inference, fine-tuning,
 and deployment of **Atom** series models. This includes: Atom-7B and Atom-7B-
 Chat. use [this script](https://github.com/modelscope/swift/blob/main/examples/
 pytorch/llm/scripts/atom_7b_chat/lora/sft.sh) to train. - 2024.04.19: Support
 for single-card, DDP, ZeRO2, and ZeRO3 training and inference with NPU, please
-refer to [NPU Inference and Fine-tuning Best Practices](docs/source_en/LLM/NPU-
+refer to [NPU Inference and Fine-tuning Best Practice](docs/source_en/LLM/NPU-
 best-practice.md). - 2024.04.19: Support for inference, fine-tuning, and
 deployment of **Llama3** series models. This includes: Llama-3-8B, Llama-3-8B-
 Instruct, Llama-3-70B, and Llama-3-70B-Instruct. use [this script](https://
 github.com/modelscope/swift/blob/main/examples/pytorch/llm/scripts/
-llama3_8b_instruct/lora/sft.sh) to train. - 2024.04.18: Supported models:
+llama3_8b_instruct/lora/sft.sh) to train. More - 2024.04.18: Supported models:
 wizardlm2-7b-awq, wizardlm2-8x22b, yi-6b-chat-awq, yi-6b-chat-int8, yi-34b-
 chat-awq, yi-34b-chat-int8. Supported `--deepspeed zero3-offload` and provided
 default zero3-offload configuration file for zero3+cpu offload usage. -
 2024.04.18: Supported compatibility with HuggingFace ecosystem using the
 environment variable `USE_HF`, switching to use models and datasets from HF.
 Please refer to the [HuggingFace ecosystem compatibility documentation](https:/
 /github.com/modelscope/swift/tree/main/docs/source_en/LLM/Compat-HF.md). -
@@ -118,15 +155,15 @@
 (https://github.com/modelscope/swift/tree/main/docs/source_en/LLM/Grok-1-best-
 practice.md). - ð¥2024.03.25: Supports inference and fine-tuning of TeleChat-
 7b and TeleChat-12b model, use [this script](https://github.com/modelscope/
 swift/blob/main/examples/pytorch/llm/scripts/telechat_12b/lora/sft.sh) to start
 training! - ð¥2024.03.20: Supports inference and fine-tuning for the
 **llava** series. For best practice, you can refer to [here](https://
 github.com/modelscope/swift/tree/main/docs/source_en/Multi-Modal/llava-best-
-practice.md). More - ð¥2024.03.12: Support inference and fine-tuning for
+practice.md). - ð¥2024.03.12: Support inference and fine-tuning for
 **deepseek-vl** series. Best practices can be found [here](docs/source_en/
 Multi-Modal/deepseek-vl-best-practice.md). - ð¥2024.03.11: Support [GaLore]
 (https://arxiv.org/abs/2403.03507) for effectively reducing memory usage to 1/
 2 of the original in full-parameter training. - ð¥2024.03.10: [End-to-end
 best practices](docs/source_en/LLM/Qwen1.5-best-practice.md) from fine-tuning
 to deployment for Qwen1.5-7B-Chat and Qwen1.5-72B-Chat. - ð¥2024.03.09:
 Support training and inference of MAMBA model, use [this script](https://
@@ -207,35 +244,33 @@
 /github.com/modelscope/swift/blob/main/docs/source/LLM/Benchmark.md) for
 convenient viewing of training speed and memory usage of different models. -
 ð¥2023.12.29: Support web-ui for sft training and inference, use `swift web-
 ui` after installing ms-swift to start. - ð¥2023.12.29: Support DPO RLHF
 (Reinforcement Learning from Human Feedback) and three datasets for this task:
 AI-ModelScope/stack-exchange-paired, AI-ModelScope/hh-rlhf and AI-ModelScope/
 hh_rlhf_cn. See [documentation](https://github.com/modelscope/swift/blob/main/
-docs/source/LLM/
-LLM%E4%BA%BA%E7%B1%BB%E5%AF%B9%E9%BD%90%E8%AE%AD%E7%BB%83%E6%96%87%E6%A1%A3.md)
-to start training! - ð¥2023.12.28: Support SCEdit! This tuner can
-significantly reduce memory usage in U-Net and support low-memory controllable
-image generation (replacing ControlNet), read the section below to learn more.
-- 2023.12.23: Support [codegeex2-6b](https://github.com/modelscope/swift/tree/
-main/examples/pytorch/llm/scripts/codegeex2_6b). - 2023.12.19: Support [phi2-
-3b](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
-phi2_3b). - 2023.12.18: Support VLLM for inference acceleration. - 2023.12.15:
-Support deepseek, deepseek-coder series: deepseek-7b, deepseek-7b-chat,
-deepseek-67b, deepseek-67b-chat, openbuddy-deepseek-67b-chat, deepseek-coder-
-1_3b, deepseek-coder-1_3b-instruct, deepseek-coder-6_7b, deepseek-coder-6_7b-
-instruct, deepseek-coder-33b, deepseek-coder-33b-instruct. - 2023.12.13:
-Support mistral-7b-instruct-v2, [mixtral-moe-7b](https://github.com/modelscope/
-swift/tree/main/examples/pytorch/llm/scripts/mixtral_7b_moe), [mixtral-moe-7b-
-instruct](https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/
-scripts/mixtral_7b_moe_instruct). - 2023.12.09: Support `freeze_parameters`
-parameter as a compromise between lora and full-parameter training.
-Corresponding sh can be found in [full_freeze_ddp](https://github.com/
-modelscope/swift/tree/main/examples/pytorch/llm/scripts/qwen_7b_chat/
-full_freeze_ddp). Support `disable_tqdm`, `lazy_tokenize`,
+docs/source_en/LLM/DPO.md) to start training! - ð¥2023.12.28: Support SCEdit!
+This tuner can significantly reduce memory usage in U-Net and support low-
+memory controllable image generation (replacing ControlNet), read the section
+below to learn more. - 2023.12.23: Support [codegeex2-6b](https://github.com/
+modelscope/swift/tree/main/examples/pytorch/llm/scripts/codegeex2_6b). -
+2023.12.19: Support [phi2-3b](https://github.com/modelscope/swift/tree/main/
+examples/pytorch/llm/scripts/phi2_3b). - 2023.12.18: Support VLLM for inference
+acceleration. - 2023.12.15: Support deepseek, deepseek-coder series: deepseek-
+7b, deepseek-7b-chat, deepseek-67b, deepseek-67b-chat, openbuddy-deepseek-67b-
+chat, deepseek-coder-1_3b, deepseek-coder-1_3b-instruct, deepseek-coder-6_7b,
+deepseek-coder-6_7b-instruct, deepseek-coder-33b, deepseek-coder-33b-instruct.
+- 2023.12.13: Support mistral-7b-instruct-v2, [mixtral-moe-7b](https://
+github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
+mixtral_7b_moe), [mixtral-moe-7b-instruct](https://github.com/modelscope/swift/
+tree/main/examples/pytorch/llm/scripts/mixtral_7b_moe_instruct). - 2023.12.09:
+Support `freeze_parameters` parameter as a compromise between lora and full-
+parameter training. Corresponding sh can be found in [full_freeze_ddp](https://
+github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
+qwen_7b_chat/full_freeze_ddp). Support `disable_tqdm`, `lazy_tokenize`,
 `preprocess_num_proc` parameters, see [command line arguments](https://
 github.com/modelscope/swift/blob/main/docs/source/LLM/
 %E5%91%BD%E4%BB%A4%E8%A1%8C%E5%8F%82%E6%95%B0.md) for details. - 2023.12.08:
 Support [sus-34b-chat](https://github.com/modelscope/swift/tree/main/examples/
 pytorch/llm/scripts/sus_34b_chat), support yi-6b-200k, yi-34b-200k. -
 2023.12.07: Support [Multi-Node DDP training](https://github.com/modelscope/
 swift/blob/main/docs/source/LLM/
@@ -310,17 +345,20 @@
 [llm]' ``` SWIFT depends on torch>=1.13, recommend torch>=2.0.0. - Method 3:
 Use SWIFT in our Docker image ```shell # China-Hangzhou image docker pull
 registry.cn-hangzhou.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-
 cuda12.1.0-py310-torch2.1.2-tf2.14.0-1.13.1 # US-west image docker pull
 registry.us-west-1.aliyuncs.com/modelscope-repo/modelscope:ubuntu22.04-
 cuda12.1.0-py310-torch2.1.2-tf2.14.0-1.13.1 ``` ## ð Getting Started This
 section introduces basic usage, see the [Documentation](#-documentation)
-section for more ways to use. ### Web-UI ```shell swift web-ui ``` ### Training
-#### Training Scripts You can refer to the following scripts to customize your
-own training script. - full: [qwen1half-7b-chat](https://github.com/modelscope/
+section for more ways to use. ### Web-UI Web-UI is a gradio-based interface for
+**zero-threshold** training and deployment. It is easy to use and perfectly
+supports multi-GPU training and deployment: ```shell SWIFT_UI_LANG=en swift
+web-ui ``` ![image.png](./docs/resources/web-ui-en.jpg) ### Training ####
+Training Scripts You can refer to the following scripts to customize your own
+training script. - full: [qwen1half-7b-chat](https://github.com/modelscope/
 swift/tree/main/examples/pytorch/llm/scripts/qwen1half_7b_chat/full) (A100),
 [qwen-7b-chat](https://github.com/modelscope/swift/tree/main/examples/pytorch/
 llm/scripts/qwen_7b_chat/full_mp) (2\*A100) - full+ddp+zero2: [qwen-7b-chat]
 (https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
 qwen_7b_chat/full_ddp_zero2) (4\*A100) - full+ddp+zero3: [qwen-14b-chat](https:
 //github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
 qwen_14b_chat/full_ddp_zero3) (4\*A100) - lora: [chatglm3-6b](https://
@@ -342,86 +380,91 @@
 scripts/qwen1half_7b_chat_int8/qlora) (3090) - qlora(bnb-int4): [qwen-7b-chat]
 (https://github.com/modelscope/swift/tree/main/examples/pytorch/llm/scripts/
 qwen_7b_chat/qlora) (3090) #### Supported Training Processes | Training Process
 | Training Method | |------------------|---------------------------------------
 ----------------------------------------| | Pretraining | Text Generation | |
 Fine-tuning | Single-turn/Multi-turn
 Agent Training/Self-cognition
-Multi-modal Vision/Multi-modal Speech| | Human Alignment | DPO | | Text-to-
-Image | DreamBooth, etc. | | Text-to-Video | - | #### Single GPU Training Start
-single GPU fine-tuning with the following command: LoRA: ```shell #
-Experimental Environment: A100 # GPU Memory Requirement: 20GB # Runtime: 3.1
+Multi-modal Vision/Multi-modal Speech| | Human Alignment | DPO
+ORPO | | Text-to-Image | DreamBooth, etc. | | Text-to-Video | - | #### Single
+GPU Training Start single GPU fine-tuning with the following command: LoRA:
+```shell # Experimental Environment: A100 # GPU Memory Requirement: 20GB #
+Runtime: 3.1 hours CUDA_VISIBLE_DEVICES=0 \ swift sft \ --model_type qwen1half-
+7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \
+--output_dir output \ --eval_steps 200 \ ``` Full-parameter: ```shell #
+Experimental Environment: A100 # GPU Memory Requirement: 80GB # Runtime: 2.5
 hours CUDA_VISIBLE_DEVICES=0 \ swift sft \ --model_type qwen1half-7b-chat \ --
-dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --output_dir
-output \ --eval_steps 200 \ ``` Full-parameter: ```shell # Experimental
-Environment: A100 # GPU Memory Requirement: 80GB # Runtime: 2.5 hours
-CUDA_VISIBLE_DEVICES=0 \ swift sft \ --model_type qwen1half-7b-chat \ --dataset
-blossom-math-zh \ --num_train_epochs 5 \ --sft_type full \ --output_dir output
-\ --eval_steps 500 \ ``` #### Model Parallel Training ```shell # Experimental
-Environment: 2 * A100 # GPU Memory Requirement: 10GB + 13GB # Runtime: 3.4
-hours CUDA_VISIBLE_DEVICES=0,1 \ swift sft \ --model_type qwen1half-7b-chat \ -
--dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --
-output_dir output \ ``` #### Data Parallel Training ```shell # Experimental
-Environment: 4 * A100 # GPU Memory Requirement: 4 * 30GB # Runtime: 0.8 hours
-NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type
+dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type full \ --output_dir
+output \ --eval_steps 500 \ ``` #### Model Parallel Training ```shell #
+Experimental Environment: 2 * A100 # GPU Memory Requirement: 10GB + 13GB #
+Runtime: 3.4 hours CUDA_VISIBLE_DEVICES=0,1 \ swift sft \ --model_type
 qwen1half-7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
-sft_type lora \ --output_dir output \ ``` Combining Model Parallelism and Data
-Parallelism: ```shell # Experimental Environment: 4 * A100 # GPU Memory
-Requirement: 2*14GB + 2*18GB # Runtime: 1.7 hours NPROC_PER_NODE=2 \
-CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type qwen1half-7b-chat \ --
-dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --output_dir
-output \ ``` #### Deepspeed Training Deepspeed supports training of quantized
-GPTQ and AWQ models. ZeRO2: ```shell # Experimental Environment: 4 * A100 # GPU
-Memory Requirement: 4 * 21GB # Runtime: 0.9 hours NPROC_PER_NODE=4 \
+sft_type lora \ --output_dir output \ ``` #### Data Parallel Training ```shell
+# Experimental Environment: 4 * A100 # GPU Memory Requirement: 4 * 30GB #
+Runtime: 0.8 hours NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft
+\ --model_type qwen1half-7b-chat \ --dataset blossom-math-zh \ --
+num_train_epochs 5 \ --sft_type lora \ --output_dir output \ ``` Combining
+Model Parallelism and Data Parallelism: ```shell # Experimental Environment: 4
+* A100 # GPU Memory Requirement: 2*14GB + 2*18GB # Runtime: 1.7 hours
+NPROC_PER_NODE=2 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type
+qwen1half-7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
+sft_type lora \ --output_dir output \ ``` #### Deepspeed Training Deepspeed
+supports training of quantized GPTQ and AWQ models. ZeRO2: ```shell #
+Experimental Environment: 4 * A100 # GPU Memory Requirement: 4 * 21GB #
+Runtime: 0.9 hours NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft
+\ --model_type qwen1half-7b-chat \ --dataset blossom-math-zh \ --
+num_train_epochs 5 \ --sft_type lora \ --output_dir output \ --deepspeed
+default-zero2 \ ``` ZeRO3: ```shell # Experimental Environment: 4 * A100 # GPU
+Memory Requirement: 4 * 19GB # Runtime: 3.2 hours NPROC_PER_NODE=4 \
 CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type qwen1half-7b-chat \ --
 dataset blossom-math-zh \ --num_train_epochs 5 \ --sft_type lora \ --output_dir
-output \ --deepspeed default-zero2 \ ``` ZeRO3: ```shell # Experimental
-Environment: 4 * A100 # GPU Memory Requirement: 4 * 19GB # Runtime: 3.2 hours
-NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_type
-qwen1half-7b-chat \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
-sft_type lora \ --output_dir output \ --deepspeed default-zero3 \ ``` ZeRO3-
-Offload: ```shell # Experimental Environment: 4 * A100 # GPU Memory
-Requirement: 4 * 12GB # Runtime: 60 hours NPROC_PER_NODE=4 \
-CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --model_id_or_path AI-ModelScope/
-WizardLM-2-8x22B \ --dataset blossom-math-zh \ --num_train_epochs 5 \ --
-sft_type lora \ --output_dir output \ --deepspeed zero3-offload \ ``` ####
-Multi-node Multi-GPU ```shell # node0 CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 \
-NNODES=2 \ NODE_RANK=0 \ MASTER_ADDR=127.0.0.1 \ NPROC_PER_NODE=8 \ swift sft \
---model_id_or_path qwen1half-32b-chat \ --sft_type full \ --dataset blossom-
-math-zh \ --output_dir output \ --deepspeed default-zero3 \ # node1
+output \ --deepspeed default-zero3 \ ``` ZeRO3-Offload: ```shell # Experimental
+Environment: 4 * A100 # GPU Memory Requirement: 4 * 12GB # Runtime: 60 hours
+NPROC_PER_NODE=4 \ CUDA_VISIBLE_DEVICES=0,1,2,3 \ swift sft \ --
+model_id_or_path AI-ModelScope/WizardLM-2-8x22B \ --dataset blossom-math-zh \ -
+-num_train_epochs 5 \ --sft_type lora \ --output_dir output \ --deepspeed
+zero3-offload \ ``` #### Multi-node Multi-GPU ```shell # node0
+CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 \ NNODES=2 \ NODE_RANK=0 \
+MASTER_ADDR=127.0.0.1 \ NPROC_PER_NODE=8 \ swift sft \ --model_id_or_path
+qwen1half-32b-chat \ --sft_type full \ --dataset blossom-math-zh \ --output_dir
+output \ --deepspeed default-zero3 \ # node1
 CUDA_VISIBLE_DEVICES=0,1,2,3,4,5,6,7 \ NNODES=2 \ NODE_RANK=1 \
 MASTER_ADDR=xxx.xxx.xxx.xxx \ NPROC_PER_NODE=8 \ swift sft \ --model_id_or_path
 qwen1half-32b-chat \ --sft_type full \ --dataset blossom-math-zh \ --output_dir
-output \ --deepspeed default-zero3 \ ``` ### Inference Original model: ```shell
-CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat # use VLLM
-CUDA_VISIBLE_DEVICES=0 swift infer --model_type qwen1half-7b-chat \ --
-infer_backend vllm --max_model_len 8192 ``` LoRA fine-tuned: ```shell
-CUDA_VISIBLE_DEVICES=0 swift infer --ckpt_dir xxx/checkpoint-xxx --
-load_dataset_config true # use VLLM CUDA_VISIBLE_DEVICES=0 swift infer \ --
-ckpt_dir xxx/checkpoint-xxx --load_dataset_config true \ --merge_lora true --
-infer_backend vllm --max_model_len 8192 ``` ### Evaluation ```shell
-CUDA_VISIBLE_DEVICES=0 swift eval --model_type qwen1half-7b-chat --eval_dataset
-mmlu ceval ``` ### Export Original model: ```shell CUDA_VISIBLE_DEVICES=0 swift
-export --model_type qwen1half-7b-chat \ --quant_bits 4 --quant_method awq ```
-LoRA fine-tuned: ```shell CUDA_VISIBLE_DEVICES=0 swift export \ --ckpt_dir xxx/
-checkpoint-xxx --load_dataset_config true \ --quant_method awq --quant_bits 4 \
---merge_lora true \ ``` ### Deployment Original model: ```shell
-CUDA_VISIBLE_DEVICES=0 swift deploy --model_type qwen1half-7b-chat #
-ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0 swift deploy --model_type qwen1half-7b-
-chat \ --infer_backend vllm --max_model_len 8192 ``` LoRA fine-tuned: ```shell
-CUDA_VISIBLE_DEVICES=0 swift deploy --ckpt_dir xxx/checkpoint-xxx #
-ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0 swift deploy \ --ckpt_dir xxx/
-checkpoint-xxx --merge_lora true \ --infer_backend vllm --max_model_len 8192
-``` ### Supported Models The complete list of supported models and datasets can
-be found at [Supported Models and Datasets List](docs/source_en/LLM/Supported-
-models-datasets.md). #### LLMs | Model Type | Model Introduction | Language |
-Model Size | Model Type | |------------------------------------------------|---
----------------------------------------------------------------------|---------
------------|----------------------------------------|--------------------------
------------------ | | Qwen
+output \ --deepspeed default-zero3 \ ``` ##### AliYun-DLC multi-node training
+In DLC product, WORLD_SIZE is the node number, RANK is the node index, this is
+different from the definition of torchrun. ```shell NNODES=$WORLD_SIZE \
+NODE_RANK=$RANK \ swift sft \ --model_id_or_path qwen1half-32b-chat \ --
+sft_type full \ --dataset blossom-math-zh \ --output_dir output \ --deepspeed
+default-zero3 ``` ### Inference Original model: ```shell CUDA_VISIBLE_DEVICES=0
+swift infer --model_type qwen1half-7b-chat # use VLLM CUDA_VISIBLE_DEVICES=0
+swift infer --model_type qwen1half-7b-chat \ --infer_backend vllm --
+max_model_len 8192 ``` LoRA fine-tuned: ```shell CUDA_VISIBLE_DEVICES=0 swift
+infer --ckpt_dir xxx/checkpoint-xxx --load_dataset_config true # use VLLM
+CUDA_VISIBLE_DEVICES=0 swift infer \ --ckpt_dir xxx/checkpoint-xxx --
+load_dataset_config true \ --merge_lora true --infer_backend vllm --
+max_model_len 8192 ``` ### Evaluation ```shell CUDA_VISIBLE_DEVICES=0 swift
+eval --model_type qwen1half-7b-chat --eval_dataset mmlu ceval ``` ### Export
+Original model: ```shell CUDA_VISIBLE_DEVICES=0 swift export --model_type
+qwen1half-7b-chat \ --quant_bits 4 --quant_method awq ``` LoRA fine-tuned:
+```shell CUDA_VISIBLE_DEVICES=0 swift export \ --ckpt_dir xxx/checkpoint-xxx --
+load_dataset_config true \ --quant_method awq --quant_bits 4 \ --merge_lora
+true \ ``` ### Deployment Original model: ```shell CUDA_VISIBLE_DEVICES=0 swift
+deploy --model_type qwen1half-7b-chat # ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0
+swift deploy --model_type qwen1half-7b-chat \ --infer_backend vllm --
+max_model_len 8192 ``` LoRA fine-tuned: ```shell CUDA_VISIBLE_DEVICES=0 swift
+deploy --ckpt_dir xxx/checkpoint-xxx # ä½¿ç¨VLLMå é CUDA_VISIBLE_DEVICES=0
+swift deploy \ --ckpt_dir xxx/checkpoint-xxx --merge_lora true \ --
+infer_backend vllm --max_model_len 8192 ``` ### Supported Models The complete
+list of supported models and datasets can be found at [Supported Models and
+Datasets List](docs/source_en/LLM/Supported-models-datasets.md). #### LLMs |
+Model Type | Model Introduction | Language | Model Size | Model Type | |-------
+-----------------------------------------|-------------------------------------
+-----------------------------------|--------------------|----------------------
+------------------|------------------------------------------- | | Qwen
 Qwen1.5 | [Tongyi Qwen 1.0 and 1.5 series models](https://github.com/QwenLM) |
 Chinese
 English | 0.5B-110B
 including quantized versions | base model
 chat model
 MoE model
 code model | | ChatGLM2
@@ -447,31 +490,32 @@
 chat model | | LLaMA3 | [LLaMA3 series models](https://github.com/meta-llama/
 llama3) | English | 8B-70B
 including quantized versions | base model
 chat model | | Mistral
 Mixtral | [Mistral series models](https://github.com/mistralai/mistral-src) |
 English | 7B-22B | base model
 instruct model
-MoE model | | YI | [01AI's YI series models](https://github.com/01-ai) |
-Chinese
+MoE model | | Yi
+Yi1.5 | [01AI's YI series models](https://github.com/01-ai) | Chinese
 English | 6B-34B
 including quantized | base model
 chat model
 long text model | | InternLM
 InternLM2
 InternLM2-Math | [Pujiang AI Lab InternLM series models](https://github.com/
 InternLM/InternLM) | Chinese
 English | 1.8B-20B | base model
 chat model
 math model | | DeepSeek
 DeepSeek-MoE
 DeepSeek-Coder
-DeepSeek-Math | [DeepSeek series models](https://github.com/deepseek-ai) |
+DeepSeek-Math
+DeepSeek-V2 | [DeepSeek series models](https://github.com/deepseek-ai) |
 Chinese
-English | 1.3B-67B | base model
+English | 1.3B-236B | base model
 chat model
 MoE model
 code model
 math model | | MAMBA | [MAMBA temporal convolution model](https://github.com/
 state-spaces/mamba) | English | 130M-2.8B | base model | | Gemma | [Google
 Gemma series models](https://github.com/google/gemma_pytorch) | English | 2B-7B
 | base model
@@ -544,109 +588,113 @@
 English | 7B | base model
 chat model | | YI-VL | [01AI's YI series vision models](https://github.com/01-
 ai) | Chinese
 English | 6B-34B | chat model | | XComposer2 | [Pujiang AI Lab InternLM vision
 model](https://github.com/InternLM/InternLM) | Chinese
 English | 7B | chat model | | DeepSeek-VL | [DeepSeek series vision models]
 (https://github.com/deepseek-ai) | Chinese
-English | 1.3B-7B | chat model | | MiniCPM-V | [OpenBmB MiniCPM vision model]
-(https://github.com/OpenBMB/MiniCPM) | Chinese
-English | 3B | chat model | | CogVLM
+English | 1.3B-7B | chat model | | MiniCPM-V
+MiniCPM-V-2
+MiniCPM-V-2_5 | [OpenBmB MiniCPM vision model](https://github.com/OpenBMB/
+MiniCPM) | Chinese
+English | 3B-9B | chat model | | CogVLM
+CogVLM2
 CogAgent | [Zhipu ChatGLM visual QA and Agent model](https://github.com/THUDM/
-) | English | 17B-18B | chat model | | Llava | [Llava series models](https://
-github.com/haotian-liu/LLaVA) | English | 7B-34B | chat model | | mPLUG-Owl |
-[mPLUG-Owl series models](https://github.com/X-PLUG/mPLUG-Owl) | English | 11B
-| chat model | | InternVL | [InternVL](https://github.com/OpenGVLab/InternVL) |
-Chinese
-English | 25.5B | chat model | #### Diffusion Models | Model Type | Model
-Introduction | Language | Model Type | |---------------------|-----------------
------------------------------------------------------|----------|--------------
----- | | AnimateDiff | [AnimateDiff animation model](https://github.com/guoyww/
-AnimateDiff) | English | text-to-video | | SD1.5/SD2.0/SDXL | [StabilityAI
-series diffusion models](https://github.com/Stability-AI) | English | text-to-
-image | ### Supported Open Source Datasets | Dataset Type | Training Task |
-Documentation | |--------------|:---------------|------------------------------
---------------------------------- | | General | Fine-tuning | ð¥ruozhiba,
-ð¥ms-bench, ð¥ms-bench-mini, ð¥alpaca-en(gpt4), ð¥alpaca-zh(gpt4),
-multi-alpaca-all, instinwild-en, instinwild-zh, cot-en, cot-zh, firefly-all-zh,
-instruct-en, gpt4all-en, sharegpt-en, sharegpt-zh, tulu-v2-sft-mixture,
-wikipedia-zh, open-orca, open-orca-gpt4, sharegpt-gpt4, ð¥sharegpt-gpt4-mini.
-| | Agent | Fine-tuning | ð¥ms-agent, ms-agent-for-agentfabric-default, ms-
-agent-for-agentfabric-addition, damo-mini-agent-zh, damo-agent-zh, agent-
-instruct-all-en. | | General | Human Alignment | ð¥hh-rlhf-cn, stack-
-exchange-paired, hh-rlhf-harmless-base, hh-rlhf-helpful-base, hh-rlhf-helpful-
-online, hh-rlhf-helpful-rejection-sampled, hh-rlhf-red-team-attempts, hh-rlhf-
-cn-harmless-base-cn, hh-rlhf-cn-helpful-base-cn, hh-rlhf-cn-harmless-base-en,
-hh-rlhf-cn-helpful-base-en. | | Code | Fine-tuning | code-alpaca-en,
-ð¥leetcode-python-en, ð¥codefuse-python-en, ð¥codefuse-evol-instruction-
-zh. | | Medical | Fine-tuning | medical-en, medical-zh, medical-mini-zh,
-ð¥disc-med-sft-zh. | | Legal | Fine-tuning | lawyer-llama-zh, tigerbot-law-
-zh, ð¥disc-law-sft-zh. | | Math | Fine-tuning | ð¥blossom-math-zh, school-
-math-zh, open-platypus-en. | | SQL | Fine-tuning | text2sql-en, ð¥sql-create-
-context-en. | | Text Generation | Fine-tuning | ð¥advertise-gen-zh,
-ð¥dureader-robust-zh. | | Classification | Fine-tuning | cmnli-zh, ð¥cmnli-
-mini-zh, ð¥jd-sentiment-zh, ð¥hc3-zh, ð¥hc3-en. | | Quantization Assist |
-Quantization | pileval. | | Other | Fine-tuning | finance-en, poetry-zh,
-webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-jave-zh. | | Vision |
-Fine-tuning | coco-en, ð¥coco-mini-en, coco-mini-en-2, capcha-images. | |
-Audio | Fine-tuning | aishell1-zh, ð¥aishell1-mini-zh. | ### Supported
-Technologies | Technology Name | | --------------------------------------------
----------------- | | ð¥LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE LANGUAGE
-MODELS](https://arxiv.org/abs/2106.09685) | | ð¥LoRA+: [LoRA+: Efficient Low
-Rank Adaptation of Large Models](https://arxiv.org/pdf/2402.12354.pdf) | |
-ð¥GaLore:[GaLore: Memory-Efficient LLM Training by Gradient Low-Rank
-Projection](https://arxiv.org/abs/2403.03507) | | ð¥LISA: [LISA: Layerwise
-Importance Sampling for Memory-Efficient Large Language Model Fine-Tuning]
-(https://arxiv.org/abs/2403.17919) | | ð¥UnSloth: https://github.com/
-unslothai/unsloth | | ð¥LLaMA PRO: [LLAMA PRO: Progressive LLaMA with Block
-Expansion](https://arxiv.org/pdf/2401.02415.pdf) | | ð¥SCEdit: [SCEdit:
-Efficient and Controllable Image Diffusion Generation via Skip Connection
-Editing](https://arxiv.org/abs/2312.11392) < [arXiv](https://arxiv.org/abs/
-2312.11392) \ | | ð¥NEFTune: [Noisy Embeddings Improve Instruction
-Finetuning](https://arxiv.org/abs/2310.05914) | | LongLoRA: [Efficient Fine-
-tuning of Long-Context Large Language Models](https://arxiv.org/abs/2309.12307)
-| | Adapter: [Parameter-Efficient Transfer Learning for NLP](http://arxiv.org/
-abs/1902.00751) | | Vision Prompt Tuning: [Visual Prompt Tuning](https://
-arxiv.org/abs/2203.12119) | | Side: [Side-Tuning: A Baseline for Network
-Adaptation via Additive Side Networks](https://arxiv.org/abs/1912.13503) | |
-Res-Tuning: [Res-Tuning: A Flexible and Efficient Tuning Paradigm via Unbinding
-Tuner from Backbone](https://arxiv.org/abs/2310.19859) < [arXiv](https://
-arxiv.org/abs/2310.19859) \ | | Tuners provided by [PEFT](https://github.com/
-huggingface/peft), such as IA3, AdaLoRA, etc. | ### Supported Hardware |
-Hardware Environment | Notes | |--------------------------------|--------------
------------------------------------| | CPU | | | RTX 20/30/40 series, etc. |
-After 30 series, BF16 and FlashAttn can be used | | Computing cards T4/V100,
-etc. | BF16 and FlashAttn not supported | | Computing cards A10/A100, etc. |
-Support BF16 and FlashAttn | | Huawei Ascend NPU | | ## ð Documentation ###
-Documentation Compiling ```shell make docs # Check docs/build/html/index.html
-in web-browser ``` ### User Guide | Document Name | | -------------------------
------------------------------------ | | [Using Web-UI](docs/source_en/
-GetStarted/Web-ui.md) | | [Using Tuners](docs/source_en/GetStarted/Tuners.md) |
-| [LLM Inference](docs/source_en/LLM/LLM-inference.md) | | [LLM Fine-tuning]
-(docs/source_en/LLM/LLM-fine-tuning.md) | | [LLM Evaluation](docs/source_en/
-LLM/LLM-eval.md) | | [LLM Quantization](docs/source_en/LLM/LLM-quantization.md)
-| | [LLM Deployment](docs/source_en/LLM/VLLM-inference-acceleration-and-
-deployment.md) | | [DPO Human Alignment Training](docs/source_en/LLM/RLHF.md) |
-| [AnimateDiff Training](docs/source_en/AIGC/AnimateDiff-train-infer.md) | ###
-Reference Documentation | Document Name | | -----------------------------------
-------------------------- | | [Command Line Arguments](docs/source_en/LLM/
-Command-line-parameters.md) | | [Supported Models and Datasets List](docs/
-source_en/LLM/Supported-models-datasets.md) | | [Customizing New Models and
-Datasets](docs/source_en/LLM/Customization.md) | | [Runtime Speed and Memory
-Benchmark](docs/source_en/LLM/Benchmark.md) | ### Best Practices | Best
-Practices Name | | -----------------------------------------------------------
-- | | [Agent Fine-Tuning Best Practice](docs/source_en/LLM/Agent-best-
-practice.md) | | [Self-Cognition Fine-Tuning Best Practice](docs/source_en/LLM/
-Self-cognition-best-practice.md) | | [Qwen1.5 Best Practice](docs/source_en/
-LLM/Qwen1.5-best-practice.md) | | [Multi-Modal Model Training Best Practice]
-(docs/source_en/Multi-Modal/index.md) | | [NPU Best Practice](docs/source_en/
-LLM/NPU-best-practice.md) | ### Deep Learning Tutorials | Tutorial Name | |----
----------------------------------------------------------- | | [Introduction to
-Deep Learning](https://github.com/modelscope/modelscope-classroom/blob/main/
-LLM-tutorial/
+) | Chinese
+English | 17B-19B | chat model | | Llava | [Llava series models](https://
+github.com/haotian-liu/LLaVA) | English | 7B-34B | chat model | | Llava-Next |
+[Llava-Next series models](https://github.com/LLaVA-VL/LLaVA-NeXT) | Chinese
+English | 8B-110B | chat model | | mPLUG-Owl | [mPLUG-Owl series models](https:
+//github.com/X-PLUG/mPLUG-Owl) | English | 11B | chat model | | InternVL |
+[InternVL](https://github.com/OpenGVLab/InternVL) | Chinese
+English | 25.5B
+including quantized version | chat model | | Llava-llama3 | [xtuner](https://
+huggingface.co/xtuner/llava-llama-3-8b-v1_1-transformers) | English | 8B | chat
+model | #### Diffusion Models | Model Type | Model Introduction | Language |
+Model Type | |---------------------|-------------------------------------------
+---------------------------|----------|------------------ | | AnimateDiff |
+[AnimateDiff animation model](https://github.com/guoyww/AnimateDiff) | English
+| text-to-video | | SD1.5/SD2.0/SDXL | [StabilityAI series diffusion models]
+(https://github.com/Stability-AI) | English | text-to-image | ### Supported
+Open Source Datasets | Dataset Type | Training Task | Documentation | |--------
+------|:---------------|-------------------------------------------------------
+-------- | | General | Fine-tuning | ð¥ruozhiba, ð¥ms-bench, ð¥alpaca-en
+(gpt4), ð¥alpaca-zh(gpt4), multi-alpaca, instinwild, cot-en, cot-zh, firefly-
+zh, instruct-en, gpt4all-en, sharegpt, tulu-v2-sft-mixture, wikipedia-zh, open-
+orca, sharegpt-gpt4, deepctrl-sft, coig-cqia. | | Agent | Fine-tuning | ð¥ms-
+agent, ð¥ms-agent-for-agentfabric, ms-agent-multirole, ð¥toolbench-for-
+alpha-umi, damo-agent-zh, damo-agent-zh-mini, agent-instruct-all-en. | |
+General | Human Alignment | hh-rlhf, ð¥hh-rlhf-cn, stack-exchange-paired. | |
+Code | Fine-tuning | code-alpaca-en, ð¥leetcode-python-en, ð¥codefuse-
+python-en, ð¥codefuse-evol-instruction-zh. | | Medical | Fine-tuning |
+medical-en, medical-zh, ð¥disc-med-sft-zh. | | Legal | Fine-tuning | lawyer-
+llama-zh, tigerbot-law-zh, ð¥disc-law-sft-zh. | | Math | Fine-tuning |
+ð¥blossom-math-zh, school-math-zh, open-platypus-en. | | SQL | Fine-tuning |
+text2sql-en, ð¥sql-create-context-en. | | Text Generation | Fine-tuning |
+ð¥advertise-gen-zh, ð¥dureader-robust-zh. | | Classification | Fine-tuning
+| cmnli-zh, ð¥jd-sentiment-zh, ð¥hc3-zh, ð¥hc3-en. | | Quantization
+Assist | Quantization | pileval. | | Other | Fine-tuning | finance-en, poetry-
+zh, webnovel-zh, generated-chat-zh, cls-fudan-news-zh, ner-jave-zh. | | Vision
+| Fine-tuning | coco-en, ð¥coco-en-mini, coco-en-2, coco-en-2-mini, capcha-
+images. | | Audio | Fine-tuning | aishell1-zh, ð¥aishell1-zh-mini. | ###
+Supported Technologies | Technology Name | | ----------------------------------
+-------------------------- | | ð¥LoRA: [LORA: LOW-RANK ADAPTATION OF LARGE
+LANGUAGE MODELS](https://arxiv.org/abs/2106.09685) | | ð¥LoRA+: [LoRA+:
+Efficient Low Rank Adaptation of Large Models](https://arxiv.org/pdf/
+2402.12354.pdf) | | ð¥GaLore:[GaLore: Memory-Efficient LLM Training by
+Gradient Low-Rank Projection](https://arxiv.org/abs/2403.03507) | | ð¥LISA:
+[LISA: Layerwise Importance Sampling for Memory-Efficient Large Language Model
+Fine-Tuning](https://arxiv.org/abs/2403.17919) | | ð¥UnSloth: https://
+github.com/unslothai/unsloth | | ð¥LLaMA PRO: [LLAMA PRO: Progressive LLaMA
+with Block Expansion](https://arxiv.org/pdf/2401.02415.pdf) | | ð¥SCEdit:
+[SCEdit: Efficient and Controllable Image Diffusion Generation via Skip
+Connection Editing](https://arxiv.org/abs/2312.11392) < [arXiv](https://
+arxiv.org/abs/2312.11392) \ | | ð¥NEFTune: [Noisy Embeddings Improve
+Instruction Finetuning](https://arxiv.org/abs/2310.05914) | | LongLoRA:
+[Efficient Fine-tuning of Long-Context Large Language Models](https://
+arxiv.org/abs/2309.12307) | | Adapter: [Parameter-Efficient Transfer Learning
+for NLP](http://arxiv.org/abs/1902.00751) | | Vision Prompt Tuning: [Visual
+Prompt Tuning](https://arxiv.org/abs/2203.12119) | | Side: [Side-Tuning: A
+Baseline for Network Adaptation via Additive Side Networks](https://arxiv.org/
+abs/1912.13503) | | Res-Tuning: [Res-Tuning: A Flexible and Efficient Tuning
+Paradigm via Unbinding Tuner from Backbone](https://arxiv.org/abs/2310.19859) <
+[arXiv](https://arxiv.org/abs/2310.19859) \ | | Tuners provided by [PEFT]
+(https://github.com/huggingface/peft), such as IA3, AdaLoRA, etc. | ###
+Supported Hardware | Hardware Environment | Notes | |--------------------------
+------|-------------------------------------------------| | CPU | | | RTX 20/
+30/40 series, etc. | After 30 series, BF16 and FlashAttn can be used | |
+Computing cards T4/V100, etc. | BF16 and FlashAttn not supported | | Computing
+cards A10/A100, etc. | Support BF16 and FlashAttn | | Huawei Ascend NPU | | ##
+ð Documentation ### Documentation Compiling ```shell make docs # Check docs/
+build/html/index.html in web-browser ``` ### User Guide | Document Name | | ---
+--------------------------------------------------------- | | [Using Web-UI]
+(docs/source_en/GetStarted/Web-ui.md) | | [Using Tuners](docs/source_en/
+GetStarted/Tuners.md) | | [LLM Inference](docs/source_en/LLM/LLM-inference.md)
+| | [LLM Fine-tuning](docs/source_en/LLM/LLM-fine-tuning.md) | | [LLM
+Evaluation](docs/source_en/LLM/LLM-eval.md) | | [LLM Quantization](docs/
+source_en/LLM/LLM-quantization.md) | | [LLM Deployment](docs/source_en/LLM/
+VLLM-inference-acceleration-and-deployment.md) | | [DPO Human Alignment
+Training](docs/source_en/LLM/DPO.md) | | [ORPO Human Alignment Training](docs/
+source_en/LLM/ORPO.md) | | [AnimateDiff Training](docs/source_en/AIGC/
+AnimateDiff-train-infer.md) | ### Reference Documentation | Document Name | | -
+----------------------------------------------------------- | | [Command Line
+Arguments](docs/source_en/LLM/Command-line-parameters.md) | | [Supported Models
+and Datasets List](docs/source_en/LLM/Supported-models-datasets.md) | |
+[Customizing New Models and Datasets](docs/source_en/LLM/Customization.md) | |
+[Runtime Speed and Memory Benchmark](docs/source_en/LLM/Benchmark.md) | ###
+Best Practices | Best Practices Name | | --------------------------------------
+---------------------- | | [Agent Fine-Tuning Best Practice](docs/source_en/
+LLM/Agent-best-practice.md) | | [Self-Cognition Fine-Tuning Best Practice]
+(docs/source_en/LLM/Self-cognition-best-practice.md) | | [Qwen1.5 Best
+Practice](docs/source_en/LLM/Qwen1.5-best-practice.md) | | [Multi-Modal Model
+Training Best Practice](docs/source_en/Multi-Modal/index.md) | | [NPU Best
+Practice](docs/source_en/LLM/NPU-best-practice.md) | ### Deep Learning
+Tutorials | Tutorial Name | |--------------------------------------------------
+------------ | | [Introduction to Deep Learning](https://github.com/modelscope/
+modelscope-classroom/blob/main/LLM-tutorial/
 A.%E6%B7%B1%E5%BA%A6%E5%AD%A6%E4%B9%A0%E5%85%A5%E9%97%A8%E4%BB%8B%E7%BB%8D.md)
 | | [Large Model Basics](https://github.com/modelscope/modelscope-classroom/
 blob/main/LLM-tutorial/
 B.%E9%AD%94%E6%90%AD%E7%A4%BE%E5%8C%BA%E5%92%8CLLM%E5%A4%A7%E6%A8%A1%E5%9E%8B%E5%9F%BA%E7%A1%80%E7%9F%A5%E8%AF%86.md)
 | | [Prompt Engineering](https://github.com/modelscope/modelscope-classroom/
 blob/main/LLM-tutorial/C.%E6%8F%90%E7%A4%BA%E8%AF%8D%E5%B7%A5%E7%A8%8B-
 prompt%20engineering.md) | | [Transformer Architecture Introduction](https://
@@ -668,20 +716,21 @@
 K.%E5%A4%A7%E6%A8%A1%E5%9E%8B%E8%87%AA%E5%8A%A8%E8%AF%84%E4%BC%B0%E7%90%86%E8%AE%BA%E5%92%8C%E5%AE%9E%E6%88%98-
 -LLM%20Automatic%20Evaluation.md) | ## ð License This framework is licensed
 under the [Apache License (Version 2.0)](https://github.com/modelscope/
 modelscope/blob/master/LICENSE). For models and datasets, please refer to the
 original resource page and follow the corresponding License. ## ð Citation
 ```bibtex @Misc{swift, title = {SWIFT:Scalable lightWeight Infrastructure for
 Fine-Tuning}, author = {The ModelScope Team}, howpublished = {\url{https://
-github.com/modelscope/swift}}, year = {2024} } ``` ## â Contact Us You can
+github.com/modelscope/swift}}, year = {2024} } ``` ## â Wechat Group You can
 contact us and communicate with us by adding our WeChat group:
 [asset/wechat.png]
 ## Star History [![Star History Chart](https://api.star-history.com/
 svg?repos=modelscope/swift&type=Date)](https://star-history.com/#modelscope/
 swift&Date) Keywords: python,petl,efficient tuners Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Description-Content-Type: text/markdown Provides-
-Extra: llm Provides-Extra: aigc Provides-Extra: eval Provides-Extra: all
+Extra: llm Provides-Extra: aigc Provides-Extra: eval Provides-Extra:
+seq_parallel Provides-Extra: all
```

### Comparing `ms-swift-2.0.4/ms_swift.egg-info/SOURCES.txt` & `ms-swift-2.0.5/ms_swift.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 ms_swift.egg-info/requires.txt
 ms_swift.egg-info/top_level.txt
 requirements/aigc.txt
 requirements/docs.txt
 requirements/eval.txt
 requirements/framework.txt
 requirements/llm.txt
+requirements/seq_parallel.txt
 requirements/tests.txt
 swift/__init__.py
 swift/torchacc_utils.py
 swift/version.py
 swift/aigc/__init__.py
 swift/aigc/animatediff.py
 swift/aigc/animatediff_infer.py
@@ -47,14 +48,15 @@
 swift/cli/deploy.py
 swift/cli/dpo.py
 swift/cli/eval.py
 swift/cli/export.py
 swift/cli/infer.py
 swift/cli/main.py
 swift/cli/merge_lora.py
+swift/cli/orpo.py
 swift/cli/sft.py
 swift/cli/web_ui.py
 swift/hub/__init__.py
 swift/hub/api.py
 swift/hub/check_model.py
 swift/hub/constants.py
 swift/hub/errors.py
@@ -70,19 +72,21 @@
 swift/llm/accelerator.py
 swift/llm/app_ui.py
 swift/llm/deploy.py
 swift/llm/dpo.py
 swift/llm/eval.py
 swift/llm/export.py
 swift/llm/infer.py
+swift/llm/orpo.py
 swift/llm/rome.py
 swift/llm/sft.py
 swift/llm/tuner.py
 swift/llm/agent/__init__.py
 swift/llm/agent/utils.py
+swift/llm/data/dataset_info.json
 swift/llm/data/self_cognition.jsonl
 swift/llm/ds_config/zero2.json
 swift/llm/ds_config/zero3.json
 swift/llm/ds_config/zero3_offload.json
 swift/llm/utils/__init__.py
 swift/llm/utils/argument.py
 swift/llm/utils/client_utils.py
@@ -95,16 +99,18 @@
 swift/llm/utils/vision_utils.py
 swift/llm/utils/vllm_utils.py
 swift/trainers/__init__.py
 swift/trainers/arguments.py
 swift/trainers/callback.py
 swift/trainers/dpo_trainers.py
 swift/trainers/mixin.py
+swift/trainers/orpo_trainers.py
 swift/trainers/trainers.py
 swift/trainers/utils.py
+swift/trainers/xtuner.py
 swift/trainers/optimizers/__init__.py
 swift/trainers/optimizers/galore/__init__.py
 swift/trainers/optimizers/galore/adafactor.py
 swift/trainers/optimizers/galore/adamw.py
 swift/trainers/optimizers/galore/adamw8bit.py
 swift/trainers/optimizers/galore/galore_projector.py
 swift/trainers/optimizers/galore/utils.py
@@ -145,15 +151,18 @@
 swift/ui/llm_infer/generate.py
 swift/ui/llm_infer/llm_infer.py
 swift/ui/llm_infer/model.py
 swift/ui/llm_infer/runtime.py
 swift/ui/llm_train/__init__.py
 swift/ui/llm_train/advanced.py
 swift/ui/llm_train/dataset.py
+swift/ui/llm_train/galore.py
 swift/ui/llm_train/hyper.py
+swift/ui/llm_train/lisa.py
+swift/ui/llm_train/llamapro.py
 swift/ui/llm_train/llm_train.py
 swift/ui/llm_train/lora.py
 swift/ui/llm_train/model.py
 swift/ui/llm_train/quantization.py
 swift/ui/llm_train/runtime.py
 swift/ui/llm_train/save.py
 swift/ui/llm_train/self_cog.py
```

### Comparing `ms-swift-2.0.4/ms_swift.egg-info/requires.txt` & `ms-swift-2.0.5/ms_swift.egg-info/requires.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,79 @@
 accelerate
 dacite
-datasets<=2.18
 jieba
 matplotlib
-modelscope>=1.13.3
+modelscope>=1.14
 nltk
 numpy
 optimum>=1.17.0
 pandas
-peft<0.11.0,>=0.9.0
+peft<0.12.0,>=0.11.0
 requests
 rouge
 safetensors
 tensorboard
 tqdm
-transformers<4.41,>=4.33
+transformers<4.42,>=4.33
 transformers_stream_generator
-trl>=0.7.7
+trl>=0.8.2
 
 [aigc]
 decord
 diffusers==0.25.0
 einops
 torchvision
 
 [all]
 accelerate
 dacite
-datasets<=2.18
 jieba
 matplotlib
-modelscope>=1.13.3
+modelscope>=1.14
 nltk
 numpy
 optimum>=1.17.0
 pandas
-peft<0.11.0,>=0.9.0
+peft<0.12.0,>=0.11.0
 requests
 rouge
 safetensors
 tensorboard
 tqdm
-transformers<4.41,>=4.33
+transformers<4.42,>=4.33
 transformers_stream_generator
-trl>=0.7.7
+trl>=0.8.2
 charset_normalizer
 cpm_kernels
 fastapi
 gradio>=3.40.0
 sentencepiece
 tiktoken
 uvicorn
 decord
 diffusers==0.25.0
 einops
 torchvision
 llmuses>=0.3.0
+xtuner
 
 [eval]
 llmuses>=0.3.0
 
 [llm]
 charset_normalizer
 cpm_kernels
 fastapi
 gradio>=3.40.0
 sentencepiece
 tiktoken
 uvicorn
+
+[seq_parallel]
+xtuner
+charset_normalizer
+cpm_kernels
+fastapi
+gradio>=3.40.0
+sentencepiece
+tiktoken
+uvicorn
```

### Comparing `ms-swift-2.0.4/setup.cfg` & `ms-swift-2.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/setup.py` & `ms-swift-2.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,18 +118,21 @@
 if __name__ == '__main__':
     install_requires, deps_link = parse_requirements('requirements.txt')
     extra_requires = {}
     all_requires = []
     extra_requires['llm'], _ = parse_requirements('requirements/llm.txt')
     extra_requires['aigc'], _ = parse_requirements('requirements/aigc.txt')
     extra_requires['eval'], _ = parse_requirements('requirements/eval.txt')
+    extra_requires['seq_parallel'], _ = parse_requirements('requirements/seq_parallel.txt')
     all_requires.extend(install_requires)
     all_requires.extend(extra_requires['llm'])
     all_requires.extend(extra_requires['aigc'])
     all_requires.extend(extra_requires['eval'])
+    all_requires.extend(extra_requires['seq_parallel'])
+    extra_requires['seq_parallel'].extend(extra_requires['llm'])
     extra_requires['all'] = all_requires
 
     setup(
         name='ms-swift',
         version=get_version(),
         description='Swift: Scalable lightWeight Infrastructure for Fine-Tuning',
         long_description=readme(),
```

### Comparing `ms-swift-2.0.4/swift/__init__.py` & `ms-swift-2.0.5/swift/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/aigc/__init__.py` & `ms-swift-2.0.5/swift/aigc/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/aigc/animatediff.py` & `ms-swift-2.0.5/swift/aigc/animatediff.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/aigc/animatediff_infer.py` & `ms-swift-2.0.5/swift/aigc/animatediff_infer.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/aigc/diffusers/__init__.py` & `ms-swift-2.0.5/swift/aigc/diffusers/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/aigc/diffusers/infer_controlnet.py` & `ms-swift-2.0.5/swift/aigc/diffusers/infer_controlnet.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/aigc/diffusers/infer_controlnet_sdxl.py` & `ms-swift-2.0.5/swift/aigc/diffusers/infer_controlnet_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/aigc/diffusers/infer_dreambooth.py` & `ms-swift-2.0.5/swift/aigc/diffusers/infer_dreambooth.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/aigc/diffusers/infer_dreambooth_lora.py` & `ms-swift-2.0.5/swift/aigc/diffusers/infer_dreambooth_lora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/aigc/diffusers/infer_dreambooth_lora_sdxl.py` & `ms-swift-2.0.5/swift/aigc/diffusers/infer_dreambooth_lora_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/aigc/diffusers/infer_text_to_image.py` & `ms-swift-2.0.5/swift/aigc/diffusers/infer_text_to_image.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/aigc/diffusers/infer_text_to_image_lora.py` & `ms-swift-2.0.5/swift/aigc/diffusers/infer_text_to_image_lora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/aigc/diffusers/infer_text_to_image_lora_sdxl.py` & `ms-swift-2.0.5/swift/aigc/diffusers/infer_text_to_image_lora_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/aigc/diffusers/infer_text_to_image_sdxl.py` & `ms-swift-2.0.5/swift/aigc/diffusers/infer_text_to_image_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/aigc/diffusers/train_controlnet.py` & `ms-swift-2.0.5/swift/aigc/diffusers/train_controlnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -550,18 +550,16 @@
     # download the dataset.
     if args.dataset_name is not None:
         # Downloading and loading a dataset from the hub.
         dataset = MsDataset.load(
             args.dataset_name,
             args.dataset_config_name,
         )
-        if isinstance(dataset, dict):
-            dataset = {key: value.to_hf_dataset() for key, value in dataset.items()}
-        else:
-            dataset = {'train': dataset.to_hf_dataset()}
+        if not isinstance(dataset, dict):
+            dataset = {'train': dataset}
     else:
         if args.train_data_dir is not None:
             dataset = load_dataset(
                 args.train_data_dir,
                 cache_dir=args.cache_dir,
             )
         # See more about loading custom images at
```

### Comparing `ms-swift-2.0.4/swift/aigc/diffusers/train_controlnet_sdxl.py` & `ms-swift-2.0.5/swift/aigc/diffusers/train_controlnet_sdxl.py`

 * *Files 0% similar despite different names*

```diff
@@ -566,18 +566,16 @@
     # download the dataset.
     if args.dataset_name is not None:
         # Downloading and loading a dataset from the hub.
         dataset = MsDataset.load(
             args.dataset_name,
             args.dataset_config_name,
         )
-        if isinstance(dataset, dict):
-            dataset = {key: value.to_hf_dataset() for key, value in dataset.items()}
-        else:
-            dataset = {'train': dataset.to_hf_dataset()}
+        if not isinstance(dataset, dict):
+            dataset = {'train': dataset}
     else:
         if args.train_data_dir is not None:
             dataset = load_dataset(
                 args.train_data_dir,
                 cache_dir=args.cache_dir,
             )
         # See more about loading custom images at
```

### Comparing `ms-swift-2.0.4/swift/aigc/diffusers/train_dreambooth.py` & `ms-swift-2.0.5/swift/aigc/diffusers/train_dreambooth.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/aigc/diffusers/train_dreambooth_lora.py` & `ms-swift-2.0.5/swift/aigc/diffusers/train_dreambooth_lora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/aigc/diffusers/train_dreambooth_lora_sdxl.py` & `ms-swift-2.0.5/swift/aigc/diffusers/train_dreambooth_lora_sdxl.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/aigc/diffusers/train_text_to_image.py` & `ms-swift-2.0.5/swift/aigc/diffusers/train_text_to_image.py`

 * *Files 0% similar despite different names*

```diff
@@ -646,18 +646,16 @@
     if args.dataset_name is not None:
         # Downloading and loading a dataset from the hub.
         dataset = MsDataset.load(
             args.dataset_name,
             args.dataset_config_name,
             data_dir=args.train_data_dir,
         )
-        if isinstance(dataset, dict):
-            dataset = {key: value.to_hf_dataset() for key, value in dataset.items()}
-        else:
-            dataset = {'train': dataset.to_hf_dataset()}
+        if not isinstance(dataset, dict):
+            dataset = {'train': dataset}
     else:
         data_files = {}
         if args.train_data_dir is not None:
             data_files['train'] = os.path.join(args.train_data_dir, '**')
         dataset = load_dataset(
             'imagefolder',
             data_files=data_files,
```

### Comparing `ms-swift-2.0.4/swift/aigc/diffusers/train_text_to_image_lora.py` & `ms-swift-2.0.5/swift/aigc/diffusers/train_text_to_image_lora.py`

 * *Files 1% similar despite different names*

```diff
@@ -521,18 +521,16 @@
     if args.dataset_name is not None:
         # Downloading and loading a dataset from the hub.
         dataset = MsDataset.load(
             args.dataset_name,
             args.dataset_config_name,
             data_dir=args.train_data_dir,
         )
-        if isinstance(dataset, dict):
-            dataset = {key: value.to_hf_dataset() for key, value in dataset.items()}
-        else:
-            dataset = {'train': dataset.to_hf_dataset()}
+        if not isinstance(dataset, dict):
+            dataset = {'train': dataset}
     else:
         data_files = {}
         if args.train_data_dir is not None:
             data_files['train'] = os.path.join(args.train_data_dir, '**')
         dataset = load_dataset(
             'imagefolder',
             data_files=data_files,
```

### Comparing `ms-swift-2.0.4/swift/aigc/diffusers/train_text_to_image_lora_sdxl.py` & `ms-swift-2.0.5/swift/aigc/diffusers/train_text_to_image_lora_sdxl.py`

 * *Files 0% similar despite different names*

```diff
@@ -683,18 +683,16 @@
     if args.dataset_name is not None:
         # Downloading and loading a dataset from the hub.
         dataset = MsDataset.load(
             args.dataset_name,
             args.dataset_config_name,
             data_dir=args.train_data_dir,
         )
-        if isinstance(dataset, dict):
-            dataset = {key: value.to_hf_dataset() for key, value in dataset.items()}
-        else:
-            dataset = {'train': dataset.to_hf_dataset()}
+        if not isinstance(dataset, dict):
+            dataset = {'train': dataset}
     else:
         data_files = {}
         if args.train_data_dir is not None:
             data_files['train'] = os.path.join(args.train_data_dir, '**')
         dataset = load_dataset(
             'imagefolder',
             data_files=data_files,
```

### Comparing `ms-swift-2.0.4/swift/aigc/diffusers/train_text_to_image_sdxl.py` & `ms-swift-2.0.5/swift/aigc/diffusers/train_text_to_image_sdxl.py`

 * *Files 0% similar despite different names*

```diff
@@ -741,18 +741,16 @@
     if args.dataset_name is not None:
         # Downloading and loading a dataset from the hub.
         dataset = MsDataset.load(
             args.dataset_name,
             args.dataset_config_name,
             data_dir=args.train_data_dir,
         )
-        if isinstance(dataset, dict):
-            dataset = {key: value.to_hf_dataset() for key, value in dataset.items()}
-        else:
-            dataset = {'train': dataset.to_hf_dataset()}
+        if not isinstance(dataset, dict):
+            dataset = {'train': dataset}
     else:
         data_files = {}
         if args.train_data_dir is not None:
             data_files['train'] = os.path.join(args.train_data_dir, '**')
         dataset = load_dataset(
             'imagefolder',
             data_files=data_files,
```

### Comparing `ms-swift-2.0.4/swift/aigc/utils/argument.py` & `ms-swift-2.0.5/swift/aigc/utils/argument.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/cli/main.py` & `ms-swift-2.0.5/swift/cli/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     'sft': 'swift.cli.sft',
     'infer': 'swift.cli.infer',
     'app-ui': 'swift.cli.app_ui',
     'merge-lora': 'swift.cli.merge_lora',
     'web-ui': 'swift.cli.web_ui',
     'deploy': 'swift.cli.deploy',
     'dpo': 'swift.cli.dpo',
+    'orpo': 'swift.cli.orpo',
     'export': 'swift.cli.export',
     'eval': 'swift.cli.eval'
 }
 
 ROUTE_MAPPING.update({k.replace('-', '_'): v for k, v in ROUTE_MAPPING.items()})
 
 
@@ -42,26 +43,28 @@
 
 def cli_main() -> None:
     argv = sys.argv[1:]
     method_name = argv[0]
     argv = argv[1:]
     file_path = importlib.util.find_spec(ROUTE_MAPPING[method_name]).origin
     torchrun_args = get_torchrun_args()
-    if torchrun_args is None or method_name not in ('sft', 'dpo'):
+    if torchrun_args is None or method_name not in ('sft', 'dpo', 'orpo'):
         try:
             python_cmd = 'python'
             subprocess.run(
                 [python_cmd, '--version'],
                 stdout=subprocess.PIPE,
                 stderr=subprocess.PIPE,
             )
         except FileNotFoundError:
             python_cmd = 'python3'
         args = [python_cmd, file_path, *argv]
     else:
         args = ['torchrun', *torchrun_args, file_path, *argv]
     print(f"run sh: `{' '.join(args)}`", flush=True)
-    subprocess.run(args)
+    result = subprocess.run(args)
+    if result.returncode != 0:
+        sys.exit(result.returncode)
 
 
 if __name__ == '__main__':
     cli_main()
```

### Comparing `ms-swift-2.0.4/swift/hub/api.py` & `ms-swift-2.0.5/swift/hub/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -620,17 +620,14 @@
         cookies_path = os.path.join(ModelScopeConfig.path_credential,
                                     ModelScopeConfig.COOKIES_FILE_NAME)
         if os.path.exists(cookies_path):
             with open(cookies_path, 'rb') as f:
                 cookies = pickle.load(f)
                 for cookie in cookies:
                     if cookie.is_expired():
-                        logger.warning(
-                            'Authentication has expired, '
-                            'please re-login if you need to access private models or datasets.')
                         return None
                 return cookies
         return None
 
     @staticmethod
     def get_user_session_id():
         session_path = os.path.join(ModelScopeConfig.path_credential,
```

### Comparing `ms-swift-2.0.4/swift/hub/check_model.py` & `ms-swift-2.0.5/swift/hub/check_model.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/hub/constants.py` & `ms-swift-2.0.5/swift/hub/constants.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/hub/errors.py` & `ms-swift-2.0.5/swift/hub/errors.py`

 * *Files 4% similar despite different names*

```diff
@@ -76,17 +76,15 @@
 
 
 def handle_http_response(response, logger, cookies, model_id):
     try:
         response.raise_for_status()
     except HTTPError as error:
         if cookies is None:  # code in [403] and
-            logger.error(
-                f'Authentication token does not exist, failed to access model {model_id} which may not exist or may be \
-                private. Please login first.')
+            pass
         message = _decode_response_error(response)
         raise HTTPError('Response details: %s' % message) from error
 
 
 def raise_on_error(rsp):
     """If response error, raise exception
```

### Comparing `ms-swift-2.0.4/swift/hub/file_download.py` & `ms-swift-2.0.5/swift/hub/file_download.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/hub/git.py` & `ms-swift-2.0.5/swift/hub/git.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/hub/push_to_hub.py` & `ms-swift-2.0.5/swift/hub/push_to_hub.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/hub/repository.py` & `ms-swift-2.0.5/swift/hub/repository.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/hub/snapshot_download.py` & `ms-swift-2.0.5/swift/hub/snapshot_download.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/hub/utils/caching.py` & `ms-swift-2.0.5/swift/hub/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/hub/utils/utils.py` & `ms-swift-2.0.5/swift/hub/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/llm/__init__.py` & `ms-swift-2.0.5/swift/llm/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,25 +5,27 @@
 from .utils import *
 
 if TYPE_CHECKING:
     # Recommend using `xxx_main`
     from .app_ui import gradio_chat_demo, gradio_generation_demo, app_ui_main
     from .deploy import deploy_main
     from .dpo import dpo_main
+    from .orpo import orpo_main
     from .infer import merge_lora, prepare_model_template, infer_main, merge_lora_main
     from .rome import rome_main
     from .sft import sft_main
     from .export import export_main
     from .eval import eval_main
 else:
     _extra_objects = {k: v for k, v in globals().items() if not k.startswith('_')}
     _import_structure = {
         'app_ui': ['gradio_chat_demo', 'gradio_generation_demo', 'app_ui_main'],
         'deploy': ['deploy_main'],
         'dpo': ['dpo_main'],
+        'orpo': ['orpo_main'],
         'infer': ['merge_lora', 'prepare_model_template', 'infer_main', 'merge_lora_main'],
         'rome': ['rome_main'],
         'sft': ['sft_main'],
         'export': ['export_main'],
         'eval': ['eval_main'],
     }
```

### Comparing `ms-swift-2.0.4/swift/llm/accelerator.py` & `ms-swift-2.0.5/swift/llm/accelerator.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/llm/agent/utils.py` & `ms-swift-2.0.5/swift/llm/agent/utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/llm/app_ui.py` & `ms-swift-2.0.5/swift/llm/app_ui.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/llm/data/self_cognition.jsonl` & `ms-swift-2.0.5/swift/llm/data/self_cognition.jsonl`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/llm/deploy.py` & `ms-swift-2.0.5/swift/llm/deploy.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 import logging
 import time
 from dataclasses import asdict
 from http import HTTPStatus
 from typing import List, Optional, Union
 
 import json
+import torch
 from fastapi import FastAPI, Request
 from fastapi.responses import JSONResponse, StreamingResponse
 from modelscope import GenerationConfig
+from peft import PeftModel
 
 from swift.utils import get_logger, get_main, seed_everything
 from .infer import merge_lora, prepare_model_template
 from .utils import ChatCompletionResponse  # noqa
 from .utils import (ChatCompletionRequest, ChatCompletionResponseChoice, ChatCompletionResponseStreamChoice,
                     ChatCompletionStreamResponse, ChatMessage, CompletionRequest, CompletionResponse,
                     CompletionResponseChoice, CompletionResponseStreamChoice, CompletionStreamResponse, DeltaMessage,
@@ -34,16 +36,16 @@
     return JSONResponse({'message': message, 'object': 'error'}, status_code)
 
 
 @app.get('/v1/models')
 async def get_available_models():
     global _args
     model_list = [_args.model_type]
-    if _args.vllm_lora_request_list is not None:
-        model_list += [lora_request.lora_name for lora_request in _args.vllm_lora_request_list]
+    if _args.lora_request_list is not None:
+        model_list += [lora_request.lora_name for lora_request in _args.lora_request_list]
     data = [Model(id=model_id) for model_id in model_list]
     return ModelList(data=data)
 
 
 async def check_length(request: Union[ChatCompletionRequest, CompletionRequest], input_ids: List[int]) -> Optional[str]:
     global llm_engine, model, _args
     if _args.infer_backend == 'vllm':
@@ -74,14 +76,15 @@
 def is_generation_template(template_type: str) -> bool:
     if 'generation' in template_type:
         return True
     else:
         return False
 
 
+@torch.inference_mode()
 async def inference_vllm_async(request: Union[ChatCompletionRequest, CompletionRequest], raw_request: Request):
     global llm_engine, template, _args
     from .utils import VllmGenerationConfig
     error_msg = await check_model(request)
     if error_msg is not None:
         return create_error_response(HTTPStatus.BAD_REQUEST, error_msg)
 
@@ -143,20 +146,19 @@
     request_info.update({'seed': request.seed, 'stream': request.stream})
     logger.info(request_info)
 
     created_time = int(time.time())
     generate_kwargs = {}
     if _args.vllm_enable_lora and request.model != _args.model_type:
         lora_request = None
-        for lora_req in _args.vllm_lora_request_list:
+        for lora_req in _args.lora_request_list:
             if lora_req.lora_name == request.model:
                 lora_request = lora_req
                 break
-        assert lora_request is not None, (f"request.model: '{request.model}', "
-                                          f'available_models: {await get_available_models()}')
+        assert lora_request is not None
         generate_kwargs['lora_request'] = lora_request
     result_generator = llm_engine.generate(None, generation_config, request_id, input_ids, **generate_kwargs)
 
     async def _generate_full():
         result = None
         async for result in result_generator:
             if await raw_request.is_disconnected():
@@ -247,14 +249,15 @@
         if 'ignore_metadata' in parameters:
             kwargs['ignore_metadata'] = True
         gen_kwargs = json.loads(self.to_json_string(**kwargs))
         gen_kwargs.pop('transformers_version', None)
         return f'GenerationConfig({gen_kwargs})'
 
 
+@torch.inference_mode()
 async def inference_pt_async(request: Union[ChatCompletionRequest, CompletionRequest], raw_request: Request):
     global model, template
     error_msg = await check_model(request)
     if error_msg is not None:
         return create_error_response(HTTPStatus.BAD_REQUEST, error_msg)
 
     if request.seed is not None:
@@ -308,24 +311,36 @@
 
     generation_config = _GenerationConfig(**kwargs)
     request_info['generation_config'] = generation_config
     request_info.update({'seed': request.seed, 'stop': request.stop, 'stream': request.stream})
     logger.info(request_info)
 
     created_time = int(time.time())
+    adapter_kwargs = {}
+    if request.model != _args.model_type:
+        adapter_names = None
+        for lora_req in _args.lora_request_list:
+            if lora_req.lora_name == request.model:
+                adapter_names = request.model
+                break
+        assert adapter_names is not None
+        adapter_kwargs['adapter_names'] = [adapter_names]
+    elif isinstance(model, PeftModel):
+        adapter_kwargs['adapter_names'] = ['-']
 
     async def _generate_full():
         generation_info = {}
         response, _ = inference(
             model,
             template,
             **example,
             stop_words=request.stop,
             generation_config=generation_config,
-            generation_info=generation_info)
+            generation_info=generation_info,
+            **adapter_kwargs)
         num_prompt_tokens = generation_info['num_prompt_tokens']
         num_generated_tokens = generation_info['num_generated_tokens']
         usage_info = UsageInfo(
             prompt_tokens=num_prompt_tokens,
             completion_tokens=num_generated_tokens,
             total_tokens=num_prompt_tokens + num_generated_tokens,
         )
@@ -353,15 +368,16 @@
         generation_info = {}
         gen = inference_stream(
             model,
             template,
             **example,
             stop_words=request.stop,
             generation_config=generation_config,
-            generation_info=generation_info)
+            generation_info=generation_info,
+            **adapter_kwargs)
 
         print_idx = 0
         for response, _ in gen:
             num_prompt_tokens = generation_info['num_prompt_tokens']
             num_generated_tokens = generation_info['num_generated_tokens']
             usage_info = UsageInfo(
                 prompt_tokens=num_prompt_tokens,
```

### Comparing `ms-swift-2.0.4/swift/llm/dpo.py` & `ms-swift-2.0.5/swift/llm/dpo.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import json
 import numpy as np
 import torch
 from modelscope import BitsAndBytesConfig, GenerationConfig
 from transformers import IntervalStrategy
 from transformers.integrations import is_deepspeed_zero3_enabled
+from transformers.utils import is_torch_npu_available
 
 from swift.trainers.dpo_trainers import DPOTrainer
 from swift.utils import (check_json_format, get_dist_setting, get_logger, get_main, get_model_info, is_ddp_plus_mp,
                          is_dist, is_master, plot_images, seed_everything, show_layers)
 from .tuner import prepare_model
 from .utils import (DPOArguments, Template, get_dataset, get_model_tokenizer, get_template, get_time_info,
                     set_generation_config)
@@ -18,28 +19,57 @@
 logger = get_logger()
 
 
 def llm_dpo(args: DPOArguments) -> str:
     logger.info(f'args: {args}')
     seed_everything(args.seed)
     training_args = args.training_args
-    print(f'device_count: {torch.cuda.device_count()}')
+    if is_torch_npu_available():
+        print(f'device_count: {torch.npu.device_count()}')
+    else:
+        print(f'device_count: {torch.cuda.device_count()}')
     rank, local_rank, world_size, local_world_size = get_dist_setting()
     print(f'rank: {rank}, local_rank: {local_rank}, ' f'world_size: {world_size}, local_world_size: {local_world_size}')
 
+    if args.gpu_memory_fraction is not None:
+        for device_id in range(torch.cuda.device_count()):
+            torch.cuda.set_per_process_memory_fraction(max(min(args.gpu_memory_fraction, 1.0), 0.01), device=device_id)
+
     # Loading Model and Tokenizer
     if is_deepspeed_zero3_enabled():
         model_kwargs = {'device_map': None}
+    elif is_torch_npu_available():
+        model_kwargs = {'device_map': local_rank if local_rank >= 0 else 0}
     else:
         model_kwargs = {'low_cpu_mem_usage': True}
         if is_dist() and not is_ddp_plus_mp():
             model_kwargs['device_map'] = {'': local_rank}
         else:
             model_kwargs['device_map'] = 'auto'
-    if args.load_in_8bit or args.load_in_4bit:
+    if args.quant_method == 'hqq':
+        from transformers import HqqConfig
+        if args.hqq_dynamic_config_path is not None:
+            cwd = os.getcwd()
+            config_path = args.hqq_dynamic_config_path if os.path.isabs(args.hqq_dynamic_config_path) else os.path.join(
+                cwd, args.hqq_dynamic_config_path)
+            with open(config_path, 'r') as json_file:
+                quantization_config = HqqConfig(dynamic_config=json.load(json_file))
+        else:
+            if args.quantization_bit == 0:
+                logger.info("You haven't set the quantization_bit parameter; set it to 8.")
+                args.quantization_bit = 8
+            quantization_config = HqqConfig(nbits=args.quantization_bit, axis=args.hqq_axis)
+        logger.info(f'quantization_config: {quantization_config.__dict__}')
+        model_kwargs['quantization_config'] = quantization_config
+    elif args.quant_method == 'eetq':
+        from transformers import EetqConfig
+        quantization_config = EetqConfig('int8')
+        logger.info(f'quantization_config: {quantization_config.__dict__}')
+        model_kwargs['quantization_config'] = quantization_config
+    elif args.load_in_8bit or args.load_in_4bit:
         quantization_config = BitsAndBytesConfig(
             args.load_in_8bit,
             args.load_in_4bit,
             bnb_4bit_compute_dtype=args.bnb_4bit_compute_dtype,
             bnb_4bit_quant_type=args.bnb_4bit_quant_type,
             bnb_4bit_use_double_quant=args.bnb_4bit_use_double_quant)
         logger.info(f'quantization_config: {quantization_config.__dict__}')
@@ -98,39 +128,46 @@
 
     if args.gradient_checkpointing:
         model.config.use_cache = False  # fix transformers==4.36
         logger.info('Setting model.config.use_cache: False')
         model.enable_input_require_grads()
 
     # Loading Dataset
-    random_state = np.random.RandomState(args.dataset_seed)
     train_dataset, val_dataset = get_dataset(
-        args.dataset, args.dataset_test_ratio, random_state, check_dataset_strategy=args.check_dataset_strategy)
-    val_dataset_sample = args.val_dataset_sample
-    if train_dataset is not None and args.train_dataset_sample >= 0:
-        train_dataset_sample = min(args.train_dataset_sample, train_dataset.shape[0])
-        if train_dataset.shape[0] > train_dataset_sample:
-            logger.info(f'train_dataset_sample: {train_dataset_sample}')
-            train_idxs = random_state.permutation(train_dataset_sample)
-            train_dataset = train_dataset.select(train_idxs)
-        if val_dataset_sample is None:
-            val_dataset_sample = max(int(train_dataset_sample * args.dataset_test_ratio), 1)
-    if val_dataset is not None and val_dataset_sample is not None and val_dataset_sample >= 0:
-        if val_dataset.shape[0] > val_dataset_sample:
-            logger.info(f'val_dataset_sample: {val_dataset_sample}')
-            val_idxs = random_state.permutation(val_dataset_sample)
-            val_dataset = val_dataset.select(val_idxs)
+        args.dataset,
+        args.dataset_test_ratio,
+        args.dataset_seed,
+        check_dataset_strategy=args.check_dataset_strategy,
+        model_name=args.model_name,
+        model_author=args.model_author)
+    if args.val_dataset is not None:
+        # Loading val dataset
+        _, val_dataset = get_dataset(
+            args.val_dataset,
+            1.0,
+            args.dataset_seed,
+            check_dataset_strategy=args.check_dataset_strategy,
+            model_name=args.model_name,
+            model_author=args.model_author)
+
+    train_dataset, val_dataset = args._handle_dataset_compat(train_dataset, val_dataset)
 
     if val_dataset is None:
         training_args.evaluation_strategy = IntervalStrategy.NO
         training_args.do_eval = False
     logger.info(f'train_dataset: {train_dataset}')
     logger.info(f'val_dataset: {val_dataset}')
     template: Template = get_template(
         args.template_type, tokenizer, args.system, args.max_length, args.truncation_strategy, model=model)
+    if not template.support_multi_round and 'history' in train_dataset[0]:
+        logger.info(
+            'The current template does not support multi-turn dialogue. The chatml template is used by default. \
+You can also use the --model_type parameter to specify the  template.')
+        template: Template = get_template(
+            'chatml', tokenizer, args.system, args.max_length, args.truncation_strategy, model=model)
     args.system = template.default_system
     logger.info(f'system: {args.system}')
 
     # Trainer
     logger.info(f'training_args: {training_args}')
 
     trainer_kwargs = {}
@@ -165,17 +202,18 @@
     trainer.train(training_args.resume_from_checkpoint)
     last_model_checkpoint = getattr(trainer.state, 'last_model_checkpoint', None)
     logger.info(f'last_model_checkpoint: {last_model_checkpoint}')
     logger.info(f'best_model_checkpoint: {trainer.state.best_model_checkpoint}')
     train_time = get_time_info(trainer.state.log_history, len(train_dataset))
     # Visualization
     if is_master():
-        images_dir = os.path.join(args.output_dir, 'images')
-        logger.info(f'images_dir: {images_dir}')
-        plot_images(images_dir, args.logging_dir, ['train/loss'], 0.9)
+        if 'tensorboard' in args.training_args.report_to:
+            images_dir = os.path.join(args.output_dir, 'images')
+            logger.info(f'images_dir: {images_dir}')
+            plot_images(images_dir, args.logging_dir, ['train/loss'], 0.9)
         if args.push_to_hub:
             trainer._add_patterns_to_gitignore(['images/'])
             trainer.push_to_hub()
     run_info = {
         'memory': trainer.perf['memory'],
         'train_time': train_time,
         'last_model_checkpoint': last_model_checkpoint,
```

### Comparing `ms-swift-2.0.4/swift/llm/ds_config/zero2.json` & `ms-swift-2.0.5/swift/llm/ds_config/zero2.json`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/llm/ds_config/zero3.json` & `ms-swift-2.0.5/swift/llm/ds_config/zero3.json`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/llm/ds_config/zero3_offload.json` & `ms-swift-2.0.5/swift/llm/ds_config/zero3_offload.json`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/llm/eval.py` & `ms-swift-2.0.5/swift/llm/eval.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/llm/export.py` & `ms-swift-2.0.5/swift/llm/export.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,21 @@
     assert _args is not None
     assert template is not None
     data = _args.dataset
     n_samples = _args.quant_n_samples
     block_size = _args.quant_seqlen
 
     # only use train_dataset
-    dataset = get_dataset(data)[0]
+    dataset = get_dataset(
+        data,
+        0,
+        _args.dataset_seed,
+        check_dataset_strategy=_args.check_dataset_strategy,
+        model_name=_args.model_name,
+        model_author=_args.model_author)[0]
     logger.info(f'quant_dataset: {dataset}')
     dataset = dataset.shuffle()
 
     samples = []
     n_run = 0
     for data in dataset:
         input_ids = template.encode(data)[0].get('input_ids')
@@ -92,43 +98,33 @@
         args.ckpt_dir = swift_to_peft_format(args.ckpt_dir)
     if args.merge_lora:
         merge_lora(args, device_map=args.merge_device_map)
     if args.quant_bits > 0:
         _args = args
         assert args.quantization_bit == 0
         assert args.sft_type == 'full', 'you need to merge lora'
-        if args.dtype == 'AUTO' and args.torch_dtype is None:
-            args.dtype, args.torch_dtype = 'fp16', torch.float16
-            logger.info(f'Setting args.torch_dtype: {args.torch_dtype}')
-        if args.ckpt_dir is None:
-            quant_path = f'{args.model_type}-{args.quant_method}-int{args.quant_bits}'
-        else:
-            ckpt_dir, ckpt_name = os.path.split(args.ckpt_dir)
-            quant_path = os.path.join(ckpt_dir, f'{ckpt_name}-{args.quant_method}-int{args.quant_bits}')
-        logger.info(f'Setting quant_path: {quant_path}')
-        assert not os.path.exists(quant_path), f'quant_path: {quant_path}'
         if args.quant_method == 'awq':
             from awq import AutoAWQForCausalLM
             model, template = prepare_model_template(
                 args, device_map=args.quant_device_map, verbose=False, automodel_class=AutoAWQForCausalLM)
             awq_model_quantize(model, template.tokenizer)
-            model.save_quantized(quant_path)
+            model.save_quantized(args.quant_output_dir)
         else:  # gptq
             model, template = prepare_model_template(args, device_map=args.quant_device_map, verbose=False)
             gptq_quantizer = gptq_model_quantize(model, template.tokenizer)
             model.config.quantization_config.pop('dataset', None)
-            gptq_quantizer.save(model, quant_path)
+            gptq_quantizer.save(model, args.quant_output_dir)
 
         logger.info(get_model_info(model))
         show_layers(model)
         logger.info('Saving quantized weights...')
         model_cache_dir = model.model_dir
-        save_checkpoint(None, template.tokenizer, model_cache_dir, args.ckpt_dir, quant_path)
-        logger.info(f'Successfully quantized the model and saved in {quant_path}.')
-        args.ckpt_dir = quant_path
+        save_checkpoint(None, template.tokenizer, model_cache_dir, args.ckpt_dir, args.quant_output_dir)
+        logger.info(f'Successfully quantized the model and saved in {args.quant_output_dir}.')
+        args.ckpt_dir = args.quant_output_dir
 
     if args.push_to_hub:
         ckpt_dir = args.ckpt_dir
         if ckpt_dir is None:
             ckpt_dir = args.model_id_or_path
         assert ckpt_dir is not None, 'You need to specify `ckpt_dir`.'
         push_to_ms_hub(ckpt_dir, args.hub_model_id, args.hub_token, args.hub_private_repo, args.commit_message)
```

### Comparing `ms-swift-2.0.4/swift/llm/infer.py` & `ms-swift-2.0.5/swift/llm/utils/vllm_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,436 +1,414 @@
-# Copyright (c) Alibaba, Inc. and its affiliates.
-import datetime as dt
+import asyncio
+import inspect
 import os
-import shutil
-from typing import Any, Dict, Literal, Optional, Tuple
+from copy import deepcopy
+from typing import Any, Dict, Iterator, List, Optional, Tuple
 
-import json
-import numpy as np
 import torch
-from modelscope import BitsAndBytesConfig, GenerationConfig
+import vllm
+from modelscope import GenerationConfig
+from packaging import version
+from torch import dtype as Dtype
 from tqdm import tqdm
-from transformers import PreTrainedModel, PreTrainedTokenizerBase
-from transformers.utils import is_torch_npu_available
+from transformers import PreTrainedTokenizerBase
+from vllm import AsyncEngineArgs, AsyncLLMEngine, EngineArgs, LLMEngine, SamplingParams
 
-from swift.tuners import Swift
-from swift.utils import (append_to_jsonl, get_logger, get_main, get_model_info, read_multi_line, seed_everything,
-                         show_layers)
-from .utils import (InferArguments, Template, get_additional_saved_files, get_dataset, get_model_tokenizer,
-                    get_template, inference, inference_stream, is_adapter, set_generation_config)
+from swift.utils import get_logger
+from .argument import InferArguments
+from .model import get_model_tokenizer
+from .template import Template, get_template
+
+try:
+    from vllm.lora.request import LoRARequest
+except ImportError:
+    pass
 
 logger = get_logger()
 
 
-def save_checkpoint(model: Optional[PreTrainedModel],
-                    tokenizer: PreTrainedTokenizerBase,
-                    model_cache_dir: str,
-                    ckpt_dir: Optional[str],
-                    target_dir: str,
+def get_vllm_engine(model_type: str,
+                    torch_dtype: Optional[Dtype] = None,
                     *,
-                    save_safetensors: bool = True) -> None:
-    if model is not None:
-        model.save_pretrained(target_dir, safe_serialization=save_safetensors)
-    tokenizer.save_pretrained(target_dir)
-    model_type = getattr(tokenizer, 'model_type')
-    fname_list = ['generation_config.json', 'preprocessor_config.json']
-    if model_type is not None:
-        fname_list += get_additional_saved_files(model_type)
-
-    for fname in fname_list:
-        tgt_path = os.path.join(target_dir, fname)
-        for model_dir in [ckpt_dir, model_cache_dir]:
-            if model_dir is None:
-                continue
-            src_path = os.path.join(model_dir, fname)
-            if os.path.isfile(src_path):
-                shutil.copy(src_path, tgt_path)
-                break
-            elif os.path.isdir(src_path):
-                shutil.copytree(src_path, tgt_path)
-                break
-    # configuration.json
-    configuration_fname = 'configuration.json'
-    new_configuration_path = os.path.join(target_dir, configuration_fname)
-    for model_dir in [ckpt_dir, model_cache_dir]:
-        if model_dir is None:
-            continue
-        old_configuration_path = os.path.join(model_dir, configuration_fname)
-        if os.path.exists(old_configuration_path):
-            with open(old_configuration_path, 'r', encoding='utf-8') as f:
-                res = json.load(f)
-            res.pop('adapter_cfg', None)
-            with open(new_configuration_path, 'w', encoding='utf-8') as f:
-                json.dump(res, f, ensure_ascii=False, indent=4)
-            break
-    if ckpt_dir is not None:
-        # sft_args.json
-        sft_args_fname = 'sft_args.json'
-        old_sft_args_path = os.path.join(ckpt_dir, sft_args_fname)
-        new_sft_args_path = os.path.join(target_dir, sft_args_fname)
-        if os.path.exists(old_sft_args_path):
-            with open(old_sft_args_path, 'r', encoding='utf-8') as f:
-                res = json.load(f)
-            res['sft_type'] = 'full'
-            with open(new_sft_args_path, 'w', encoding='utf-8') as f:
-                json.dump(res, f, ensure_ascii=False, indent=2)
-
-
-def merge_lora(args: InferArguments,
-               replace_if_exists=False,
-               device_map: Optional[str] = None,
-               **kwargs) -> Optional[str]:
-    logger.info(f'replace_if_exists: {replace_if_exists}')
-    assert args.ckpt_dir is not None, 'args.ckpt_dir is not specified.'
-    assert args.sft_type == 'lora', "Only supports sft_type == 'lora'"
-    for s in ['int4', 'int8', 'awq']:
-        assert s not in args.model_type, f'{s} model is not supported'
-    if args.quantization_bit != 0:
-        logger.warning('It is not recommended to merge quantized models, '
-                       'as this can result in performance degradation')
-    ckpt_dir, ckpt_name = os.path.split(args.ckpt_dir)
-    merged_lora_path = os.path.join(ckpt_dir, f'{ckpt_name}-merged')
-    logger.info(f'merged_lora_path: `{merged_lora_path}`')
-    if os.path.exists(merged_lora_path) and not replace_if_exists:
-        logger.info(f'The weight directory for the merged LoRA already exists in {args.ckpt_dir}, '
-                    'skipping the saving process. '
-                    'you can pass `replace_if_exists=True` to overwrite it.')
+                    model_id_or_path: Optional[str] = None,
+                    revision: Optional[str] = None,
+                    gpu_memory_utilization: float = 0.9,
+                    tensor_parallel_size: int = 1,
+                    max_model_len: Optional[int] = None,
+                    engine_kwargs: Optional[Dict[str, Any]] = None,
+                    use_async: bool = False,
+                    enable_lora: bool = False,
+                    max_loras: int = 1,
+                    max_lora_rank: int = 16,
+                    **kwargs) -> LLMEngine:
+    model_dir = kwargs.pop('model_dir', None)  # compat with swift<1.7
+    tokenizer = get_model_tokenizer(
+        model_type,
+        load_model=False,
+        model_id_or_path=model_id_or_path,
+        model_dir=model_dir,
+        revision=revision,
+        download_model=True)[1]
+    model_dir = tokenizer.model_dir
+
+    if engine_kwargs is None:
+        engine_kwargs = {}
+    dtype_mapping = {torch.float16: 'float16', torch.bfloat16: 'bfloat16', torch.float32: 'float32', None: 'auto'}
+    dtype = dtype_mapping[torch_dtype]
+    disable_log_stats = engine_kwargs.pop('disable_log_stats', True)
+
+    if use_async:
+        engine_args_cls = AsyncEngineArgs
+        llm_engine_cls = AsyncLLMEngine
+        engine_kwargs['disable_log_requests'] = True
+    else:
+        engine_args_cls = EngineArgs
+        llm_engine_cls = LLMEngine
+
+    parameters = inspect.signature(engine_args_cls.__init__).parameters
+    if 'enable_lora' in parameters and enable_lora:
+        engine_kwargs['enable_lora'] = enable_lora
+        engine_kwargs['max_loras'] = max_loras
+        engine_kwargs['max_lora_rank'] = max_lora_rank
+    else:
+        assert not enable_lora, ('The current version of VLLM does not support `enable_lora`. Please upgrade VLLM.')
+
+    engine_args = engine_args_cls(
+        model=model_dir,
+        trust_remote_code=True,
+        dtype=dtype,
+        gpu_memory_utilization=gpu_memory_utilization,
+        tensor_parallel_size=tensor_parallel_size,
+        max_model_len=max_model_len,
+        disable_log_stats=disable_log_stats,
+        **engine_kwargs)
+    try:
+        from vllm.model_executor.parallel_utils.parallel_state import destroy_model_parallel
+        destroy_model_parallel()
+    except ImportError:
+        pass
+    # fix HTTPError bug (use model_dir)
+    os.environ.pop('VLLM_USE_MODELSCOPE', None)
+    llm_engine = llm_engine_cls.from_engine_args(engine_args)
+    llm_engine.engine_args = engine_args
+    llm_engine.model_dir = model_dir
+    llm_engine.model_type = model_type
+
+    if use_async:
+        _engine = llm_engine.engine
+    else:
+        _engine = llm_engine
+    # compatible with vllm==0.3.*
+    if version.parse(vllm.__version__) >= version.parse('0.3'):
+        assert isinstance(_engine.tokenizer.tokenizer, PreTrainedTokenizerBase)
+        _engine.tokenizer.tokenizer = tokenizer
     else:
-        model, template = prepare_model_template(args, device_map=args.merge_device_map, verbose=False)
-        logger.info('Merge LoRA...')
-        Swift.merge_and_unload(model)
-        model = model.model
-        logger.info('Saving merged weights...')
-        save_checkpoint(
-            model,
-            template.tokenizer,
-            model.model_dir,
-            args.ckpt_dir,
-            merged_lora_path,
-            save_safetensors=args.save_safetensors)
-        logger.info(f'Successfully merged LoRA and saved in {merged_lora_path}.')
-    logger.info("Setting args.sft_type: 'full'")
-    logger.info(f'Setting args.ckpt_dir: {merged_lora_path}')
-    args.sft_type = 'full'
-    args.ckpt_dir = merged_lora_path
-    return merged_lora_path
-
-
-def prepare_model_template(args: InferArguments,
-                           *,
-                           device_map: Optional[str] = None,
-                           verbose: bool = True,
-                           automodel_class=None) -> Tuple[PreTrainedModel, Template]:
-
-    model_kwargs = {}
-    if is_torch_npu_available():
-        logger.info(f'device_count: {torch.npu.device_count()}')
-        if device_map is None:
-            device_map = 'npu:0'
+        assert isinstance(_engine.tokenizer, PreTrainedTokenizerBase)
+        _engine.tokenizer = tokenizer
+
+    llm_engine.hf_tokenizer = tokenizer
+    generation_config_path = os.path.join(model_dir, 'generation_config.json')
+    if os.path.isfile(generation_config_path):
+        generation_config = GenerationConfig.from_pretrained(model_dir)
+        kwargs = generation_config.to_dict()
+        parameters = inspect.signature(VllmGenerationConfig.__init__).parameters
+        for k in kwargs.copy().keys():
+            if k not in parameters:
+                kwargs.pop(k)
+        llm_engine.generation_config = VllmGenerationConfig(**kwargs)
     else:
-        logger.info(f'device_count: {torch.cuda.device_count()}')
-        if device_map is None:
-            device_map = 'auto'
-    if device_map == 'auto':
-        model_kwargs['low_cpu_mem_usage'] = True
-    model_kwargs['device_map'] = device_map
+        llm_engine.generation_config = VllmGenerationConfig()
+    return llm_engine
+
+
+class VllmGenerationConfig(SamplingParams):
+
+    def __init__(
+        self,
+        max_new_tokens: Optional[int] = 64,  # max_tokens
+        temperature: float = 1.,
+        top_k: int = 50,  # -1: all
+        top_p: float = 1.,
+        repetition_penalty: float = 1.,
+        num_beams: int = 1,
+        *,
+        n: int = 1,
+        length_penalty: float = 1.,
+        stop: Optional[List[str]] = None,
+        skip_special_tokens: bool = False,
+        **kwargs,
+    ) -> None:
+        # The parameter design is similar to transformers.GenerationConfig.
+        if max_new_tokens is None:
+            max_new_tokens = 64
+        if num_beams > 1:
+            top_k = -1
+            top_p = 1
+            temperature = 0
+            logger.warning(
+                'The output of num_beams in vllm may not be consistent with the output of num_beams in transformers.')
+        if top_k == 0:
+            top_k = -1
+        if stop is None:
+            stop = []
+        kwargs['max_tokens'] = max_new_tokens
+        kwargs['temperature'] = temperature
+        kwargs['top_k'] = top_k
+        kwargs['top_p'] = top_p
+        kwargs['repetition_penalty'] = repetition_penalty
+        if num_beams > 1:
+            best_of = kwargs.get('best_of')
+            assert 'use_beam_search' not in kwargs and best_of is None
+            kwargs['use_beam_search'] = True
+            kwargs['best_of'] = num_beams
+        kwargs['n'] = n
+        kwargs['length_penalty'] = length_penalty
+        kwargs['stop'] = stop
+        kwargs['skip_special_tokens'] = skip_special_tokens
+        parameters = inspect.signature(SamplingParams.__init__).parameters
+        for k in kwargs.copy().keys():
+            if k not in parameters:
+                logger.info(f'The VLLM version is too old and does not support the parameter: {k}.')
+                kwargs.pop(k)
+        self._temperature = temperature
+        super().__init__(**kwargs)
+
+    def __setattr__(self, key: str, value: str) -> None:
+        if key == 'max_new_tokens':
+            self.max_tokens = value
+        elif key == 'do_sample':
+            assert value in {True, False}
+            if value:
+                self.temperature = self._temperature
+            else:
+                self.temperature = 0.
+        elif key == 'max_length':
+            raise ValueError('`max_length` is not supported, please use `max_new_tokens` for setting.')
+        else:
+            super().__setattr__(key, value)
+
+
+@torch.inference_mode()
+def inference_stream_vllm(llm_engine: LLMEngine,
+                          template: Template,
+                          request_list: List[Dict[str, Any]],
+                          *,
+                          generation_config: Optional[VllmGenerationConfig] = None,
+                          lora_request: Optional['LoRARequest'] = None,
+                          use_tqdm: bool = False,
+                          **kwargs) -> Iterator[List[Dict[str, Any]]]:
+    """
+    request_list: e.g. [{'query': 'hello!'}].
+        The keys that can be included are: 'query', 'history', 'system'.
+    generation_config: Priority: generation_config > model.generation_config.
+    return: e.g. [{'response': 'hi!', 'history': [('hello!', 'hi!')]}].
+        The keys to be included will be: 'response', 'history'.
+    """
+    if generation_config is None:
+        generation_config = getattr(llm_engine, 'generation_config', VllmGenerationConfig())
+    assert isinstance(generation_config, VllmGenerationConfig)
+    request_list = deepcopy(request_list)
+    generation_config = deepcopy(generation_config)
+    if generation_config.use_beam_search is True:
+        error_msg = 'Streaming generation does not support beam search.'
+        raise ValueError(error_msg)
+
+    tokenizer = template.tokenizer
+    if tokenizer.eos_token is not None and tokenizer.eos_token not in generation_config.stop:
+        generation_config.stop.append(tokenizer.eos_token)
+    if isinstance(template.suffix[-1], str) and template.suffix[-1] not in generation_config.stop:
+        generation_config.stop.append(template.suffix[-1])
+    if isinstance(template.suffix[-1], list):
+        token_str = tokenizer.decode(template.suffix[-1])
+        if token_str not in generation_config.stop:
+            generation_config.stop.append(token_str)
+
+    parameters = inspect.signature(llm_engine.add_request).parameters
+    add_request_kwargs = {}
+    if 'lora_request' in parameters:
+        add_request_kwargs['lora_request'] = lora_request
+    else:
+        assert lora_request is None, (
+            'The current version of VLLM does not support `lora_request`. Please upgrade VLLM.')
+    request_temp = []
+    for i, request in enumerate(request_list):
+        history = request.get('history', None)
+        if history is None:
+            history = []
+
+        # agent support
+        is_observation = history[-1][-1].endswith('Observation:') if history and history[-1][-1] else False
+        act_length = None
+        if is_observation:
+            history[-1][-1] = history[-1][-1] + request['query']
+            act_length = len(history[-1][-1])
+            request['query'] = None
+        request_temp.append((is_observation, act_length))
+
+        request['history'] = history
+        inputs = template.encode(request)[0]
+        if len(inputs) == 0:
+            raise ValueError('input_ids exceeds `max_length`. Please increase the value of `max_length`.')
+        input_ids = inputs['input_ids']
+        llm_engine.add_request(str(i), None, generation_config, input_ids, **add_request_kwargs)
+
+    resp_list = [None] * len(request_list)
+    print_idx_list = [[0] for _ in range(len(request_list))]
+    prog_bar = tqdm(total=len(request_list), dynamic_ncols=True, disable=not use_tqdm)
+    while llm_engine.has_unfinished_requests():
+        step_outputs = llm_engine.step()
+        for output in step_outputs:
+            i = int(output.request_id)
+            request = request_list[i]
+            generate_ids = output.outputs[0].token_ids
+            safe_response = template.generate_ids_to_response(
+                generate_ids, output.finished, print_idx=print_idx_list[i])
+            query = request['query']
+            history = request['history']
+            if resp_list[i] is None and not request_temp[i][0]:
+                history.append(None)
+            if not request_temp[i][0]:
+                history[-1] = [query, safe_response]
+            else:
+                history[-1][-1] = history[-1][-1][:request_temp[i][1]] + safe_response
+            resp_list[i] = {'response': safe_response, 'history': history}
+            if output.finished:
+                prog_bar.update()
+        yield resp_list
+
+
+@torch.inference_mode()
+def inference_vllm(llm_engine: LLMEngine,
+                   template: Template,
+                   request_list: List[Dict[str, Any]],
+                   *,
+                   generation_config: Optional[VllmGenerationConfig] = None,
+                   lora_request: Optional['LoRARequest'] = None,
+                   use_tqdm: bool = False,
+                   verbose: bool = False,
+                   prompt_prefix: str = '[PROMPT]',
+                   output_prefix: str = '[OUTPUT]',
+                   **kwargs) -> List[Dict[str, Any]]:
+    """
+    request_list: e.g. [{'query': 'hello!'}].
+        The keys that can be included are: 'query', 'history', 'system'.
+    generation_config: Priority: generation_config > model.generation_config.
+    return: e.g. [{'response': 'hi!', 'history': [('hello!', 'hi!')]}].
+        The keys to be included will be: 'response', 'history'.
+    """
+    if generation_config is None:
+        generation_config = getattr(llm_engine, 'generation_config', VllmGenerationConfig())
+    assert isinstance(generation_config, VllmGenerationConfig)
+    request_list = deepcopy(request_list)
+    generation_config = deepcopy(generation_config)
+
+    tokenizer = template.tokenizer
+    if tokenizer.eos_token is not None and tokenizer.eos_token not in generation_config.stop:
+        generation_config.stop.append(tokenizer.eos_token)
+    if isinstance(template.suffix[-1], str) and template.suffix[-1] not in generation_config.stop:
+        generation_config.stop.append(template.suffix[-1])
+    if isinstance(template.suffix[-1], list):
+        token_str = tokenizer.decode(template.suffix[-1])
+        if token_str not in generation_config.stop:
+            generation_config.stop.append(token_str)
+
+    parameters = inspect.signature(llm_engine.add_request).parameters
+    add_request_kwargs = {}
+    if 'lora_request' in parameters:
+        add_request_kwargs['lora_request'] = lora_request
+    else:
+        assert lora_request is None, (
+            'The current version of VLLM does not support `lora_request`. Please upgrade VLLM.')
+
+    for i, request in enumerate(request_list):
+        history = request.get('history', None)
+        if history is None:
+            history = []
+
+        is_observation = history[-1][-1].endswith('Observation:') if history and history[-1][-1] else False
+        if is_observation:
+            history[-1][-1] = history[-1][-1] + request['query']
+            request['query'] = None
+        request['history'] = history
+        inputs = template.encode(request)[0]
+        if len(inputs) == 0:
+            raise ValueError('input_ids exceeds `max_length`. Please increase the value of `max_length`.')
+        input_ids = inputs['input_ids']
+        llm_engine.add_request(str(i), None, generation_config, input_ids, **add_request_kwargs)
+
+    if use_tqdm is True:
+        assert verbose is False
+    prog_bar = tqdm(total=len(request_list), dynamic_ncols=True, disable=not use_tqdm)
+    outputs = []
+    while llm_engine.has_unfinished_requests():
+        step_outputs = llm_engine.step()
+        for output in step_outputs:
+            if output.finished:
+                outputs.append(output)
+                prog_bar.update()
+
+    resp_list = [None] * len(request_list)
+    for output in outputs:
+        i = int(output.request_id)
+        request = request_list[i]
+        generate_ids = output.outputs[0].token_ids
+        response = template.generate_ids_to_response(generate_ids)
+        query = request['query']
+        history = request['history']
+        if not is_observation:
+            history.append([query, response])
+        else:
+            history[-1][-1] = history[-1][-1] + response
+        resp_list[i] = {'response': response, 'history': history}
+        if verbose:
+            print(f'{prompt_prefix}{tokenizer.decode(output.prompt_token_ids, False)}{output_prefix}', end='')
+            print(tokenizer.decode(output.outputs[0].token_ids, False))
+    return resp_list
+
+
+def prepare_vllm_engine_template(args: InferArguments, use_async: bool = False) -> Tuple[LLMEngine, Template]:
+    logger.info(f'device_count: {torch.cuda.device_count()}')
 
+    assert args.quantization_bit == 0, 'not support bnb'
+    assert not (args.sft_type == 'lora' and not args.vllm_enable_lora), 'you need to merge lora'
     # Loading Model and Tokenizer
-    if args.load_in_8bit or args.load_in_4bit:
-        quantization_config = BitsAndBytesConfig(
-            args.load_in_8bit,
-            args.load_in_4bit,
-            bnb_4bit_compute_dtype=args.bnb_4bit_compute_dtype,
-            bnb_4bit_quant_type=args.bnb_4bit_quant_type,
-            bnb_4bit_use_double_quant=args.bnb_4bit_use_double_quant)
-        if args.bnb_4bit_compute_dtype is None:
-            quantization_config.bnb_4bit_compute_dtype = None
-        logger.info(f'quantization_config: {quantization_config.__dict__}')
-        model_kwargs['quantization_config'] = quantization_config
-    kwargs = {}
-    if args.use_flash_attn is not None:
-        kwargs['use_flash_attn'] = args.use_flash_attn
     model_id_or_path = None
     if args.sft_type == 'full' and args.ckpt_dir is not None:
         model_id_or_path = args.ckpt_dir
     elif args.model_id_or_path is not None:
         model_id_or_path = args.model_id_or_path
-    if automodel_class is not None:
-        kwargs['automodel_class'] = automodel_class
-
-    model, tokenizer = get_model_tokenizer(
+    llm_engine = get_vllm_engine(
         args.model_type,
         args.torch_dtype,
-        model_kwargs,
+        gpu_memory_utilization=args.gpu_memory_utilization,
+        tensor_parallel_size=args.tensor_parallel_size,
+        max_model_len=args.max_model_len,
+        use_async=use_async,
         model_id_or_path=model_id_or_path,
-        revision=args.model_revision,
-        **kwargs)
-    if verbose:
-        logger.info(f'model_config: {model.config}')
+        enable_lora=args.vllm_enable_lora,
+        max_loras=min(len(args.lora_modules), 1),
+        max_lora_rank=args.vllm_max_lora_rank)
+    tokenizer = llm_engine.hf_tokenizer
+    if use_async:
+        model_config = asyncio.run(llm_engine.get_model_config())
+        llm_engine.model_config = model_config
+    else:
+        model_config = llm_engine.model_config
+    logger.info(f'model_config: {model_config.hf_config}')
 
-    generation_config = GenerationConfig(
+    if not args.do_sample:
+        args.temperature = 0
+    generation_config = VllmGenerationConfig(
         max_new_tokens=args.max_new_tokens,
         temperature=args.temperature,
         top_k=args.top_k,
         top_p=args.top_p,
-        do_sample=args.do_sample,
+        stop=args.stop_words,
         repetition_penalty=args.repetition_penalty,
-        num_beams=args.num_beams,
-        pad_token_id=tokenizer.pad_token_id,
-        eos_token_id=tokenizer.eos_token_id)
+        num_beams=args.num_beams)
     logger.info(f'generation_config: {generation_config}')
-    set_generation_config(model, generation_config)
-
-    if model.max_model_len is None:
-        model.max_model_len = args.max_model_len
-    elif args.max_model_len is not None:
-        if args.max_model_len <= model.max_model_len:
-            model.max_model_len = args.max_model_len
-        else:
-            raise ValueError('args.max_model_len exceeds the maximum max_model_len supported by the model.'
-                             f'args.max_model_len: {args.max_model_len}, model.max_model_len: {model.max_model_len}')
-    # Preparing LoRA
-    if is_adapter(args.sft_type) and args.ckpt_dir is not None:
-        model = Swift.from_pretrained(model, args.ckpt_dir, inference_mode=True)
-        model = model.to(model.dtype)
-
-    if verbose:
-        show_layers(model)
-        logger.info(model)
-    logger.info(get_model_info(model))
-
-    template: Template = get_template(
-        args.template_type, tokenizer, args.system, args.max_length, args.truncation_strategy, model=model)
+    llm_engine.generation_config = generation_config
+    template: Template = get_template(args.template_type, tokenizer, args.system, args.max_length,
+                                      args.truncation_strategy)
     args.system = template.default_system
     logger.info(f'system: {args.system}')
-    return model, template
-
-
-def read_media_file(infer_kwargs: Dict[str, Any], infer_media_type: Literal['none', 'round', 'dialogue']) -> None:
-    text = 'Input a media path or URL <<< '
-    images = infer_kwargs.get('images', [])
-    if infer_media_type == 'none':
-        return
-    if infer_media_type == 'round' or len(images) == 0:
-        image = input(text)
-        if len(image) > 0:
-            images += [image]
-    if len(images) > 0:
-        infer_kwargs['images'] = images
-
-
-def llm_infer(args: InferArguments) -> None:
-    logger.info(f'args: {args}')
-    seed_everything(args.seed)
-    if args.merge_lora:
-        merge_lora(args, device_map=args.merge_device_map)
-    if args.infer_backend == 'vllm':
-        from .utils import prepare_vllm_engine_template, inference_stream_vllm, inference_vllm
-        llm_engine, template = prepare_vllm_engine_template(args)
-    else:
-        model, template = prepare_model_template(args)
-        if args.overwrite_generation_config:
-            assert args.ckpt_dir is not None, 'args.ckpt_dir is not specified.'
-            model.generation_config.save_pretrained(args.ckpt_dir)
-    lora_request = None
-    if args.vllm_enable_lora:
-        assert len(args.vllm_lora_request_list) == 1
-        lora_request = args.vllm_lora_request_list[0]
-    # Inference
-    result = []
-    jsonl_path = None
-    if args.save_result:
-        result_dir = args.ckpt_dir
-        if result_dir is None:
-            result_dir = llm_engine.model_dir if args.infer_backend == 'vllm' else model.model_dir
-        if result_dir is not None:
-            result_dir = os.path.join(result_dir, 'infer_result')
-            os.makedirs(result_dir, exist_ok=True)
-            time = dt.datetime.now().strftime('%Y%m%d-%H%M%S')
-            jsonl_path = os.path.join(result_dir, f'{time}.jsonl')
-    if args.eval_human:
-        input_mode: Literal['S', 'M'] = 'S'
-        logger.info('Input `exit` or `quit` to exit the conversation.')
-        logger.info('Input `multi-line` to switch to multi-line input mode.')
-        logger.info('Input `reset-system` to reset the system and clear the history.')
-        if template.support_multi_round:
-            logger.info('Input `clear` to clear the history.')
-        else:
-            logger.info('The current template only supports single-round dialogues.')
-        history = []
-        infer_kwargs = {}
-        if args.infer_media_type != 'none':
-            logger.info('Please enter the conversation content first, ' 'followed by the path to the multimedia file.')
-        system = None
-        read_system = False
-        while True:
-            if input_mode == 'S':
-                addi_prompt = ''
-                if read_system:
-                    addi_prompt = '[S]'
-                query = input(f'<<<{addi_prompt} ')
-            else:
-                addi_prompt = '[M]'
-                if read_system:
-                    addi_prompt = '[MS]'
-                query = read_multi_line(addi_prompt)
-            if query.strip().lower() in {'exit', 'quit'}:
-                break
-            elif query.strip().lower() == 'clear':
-                history = []
-                infer_kwargs = {}
-                continue
-            elif query.strip() == '':
-                continue
-            elif query.strip().lower() == 'reset-system':
-                read_system = True
-                continue
-            if read_system:
-                system = query
-                read_system = False
-                continue
-            if input_mode == 'S' and query.strip().lower() == 'multi-line':
-                input_mode = 'M'
-                logger.info('End multi-line input with `#`.')
-                logger.info('Input `single-line` to switch to single-line input mode.')
-                continue
-            if input_mode == 'M' and query.strip().lower() == 'single-line':
-                input_mode = 'S'
-                continue
-            if not template.support_multi_round:
-                history = []
-                infer_kwargs = {}
-
-            read_media_file(infer_kwargs, args.infer_media_type)
-            if args.infer_backend == 'vllm':
-                request_list = [{'query': query, 'history': history, 'system': system}]
-                if args.stream:
-                    gen = inference_stream_vllm(llm_engine, template, request_list, lora_request=lora_request)
-                    print_idx = 0
-                    for resp_list in gen:
-                        response = resp_list[0]['response']
-                        new_history = resp_list[0]['history']
-                        if len(response) > print_idx:
-                            print(response[print_idx:], end='', flush=True)
-                            print_idx = len(response)
-                    print()
-                else:
-                    resp_list = inference_vllm(llm_engine, template, request_list, lora_request=lora_request)
-                    response = resp_list[0]['response']
-                    new_history = resp_list[0]['history']
-                    print(response)
-            else:
-                if args.stop_words:
-                    infer_kwargs['stop_words'] = args.stop_words
-                if args.stream:
-                    gen = inference_stream(model, template, query, history, system, **infer_kwargs)
-                    print_idx = 0
-                    for response, new_history in gen:
-                        if len(response) > print_idx:
-                            print(response[print_idx:], end='', flush=True)
-                            print_idx = len(response)
-                    print()
-                else:
-                    response, new_history = inference(model, template, query, history, system, **infer_kwargs)
-                    print(response)
-            print('-' * 50)
-            obj = {
-                'query': query,
-                'response': response,
-                'history': history,
-            }
-            history = new_history
-            if jsonl_path is not None:
-                append_to_jsonl(jsonl_path, obj)
-            result.append(obj)
-    else:
-        random_state = np.random.RandomState(args.dataset_seed)
-        _, val_dataset = get_dataset(
-            args.dataset, args.dataset_test_ratio, random_state, check_dataset_strategy=args.check_dataset_strategy)
-        if args.val_dataset_sample >= 0 and val_dataset.shape[0] > args.val_dataset_sample:
-            logger.info(f'val_dataset_sample: {args.val_dataset_sample}')
-            val_idxs = random_state.permutation(args.val_dataset_sample)
-            val_dataset = val_dataset.select(val_idxs)
-
-        logger.info(f'val_dataset: {val_dataset}')
-        if args.verbose is None:
-            if len(val_dataset) >= 100:
-                args.verbose = False
-            else:
-                args.verbose = True
-            logger.info(f'Setting args.verbose: {args.verbose}')
-        if not args.verbose and args.stream:
-            args.stream = False
-            logger.info(f'Setting args.stream: {args.stream}')
-
-        if args.infer_backend == 'vllm' and not args.stream:
-            if args.verbose:
-                args.verbose = False
-                logger.info('Setting args.verbose: False')
-            label_list = None
-            if 'response' in val_dataset.features:
-                label_list = val_dataset['response']
-            val_dataset = val_dataset.remove_columns('response')
-            request_list = val_dataset.to_list()
-            resp_list = inference_vllm(llm_engine, template, request_list, use_tqdm=True)
-            result = []
-            if label_list is not None:
-                for request, label in zip(request_list, label_list):
-                    request['label'] = label
-            for request, resp in zip(request_list, resp_list):
-                obj = {'response': resp['response'], **request}
-                if jsonl_path is not None:
-                    append_to_jsonl(jsonl_path, obj)
-                result.append(obj)
-        else:
-            if not args.verbose:
-                val_dataset = tqdm(val_dataset)
-            for data in val_dataset:
-                kwargs = {'query': data['query']}
-                history = data.get('history')
-                system = data.get('system')
-                images = data.get('images')
-                if args.verbose and system is not None:
-                    print(f'[SYSTEM]{system}')
-                if history is not None:
-                    kwargs['history'] = history
-                if system is not None:
-                    kwargs['system'] = system
-                if images is not None:
-                    kwargs['images'] = images
-                if args.infer_backend == 'vllm':
-                    assert args.stream is True
-                    if args.verbose:
-                        print(f"[QUERY]{data['query']}\n[RESPONSE]", end='')
-                    gen = inference_stream_vllm(llm_engine, template, [kwargs], lora_request=lora_request)
-                    print_idx = 0
-                    for resp_list in gen:
-                        response = resp_list[0]['response']
-                        if args.verbose and len(response) > print_idx:
-                            print(response[print_idx:], end='', flush=True)
-                            print_idx = len(response)
-                    print()
-                else:
-                    response, _ = inference(
-                        model, template, stream=args.stream and args.verbose, verbose=args.verbose, **kwargs)
-                label = data.pop('response')
-                if label is not None:
-                    kwargs['label'] = label
-                obj = {'response': response, **kwargs}
-                if jsonl_path is not None:
-                    append_to_jsonl(jsonl_path, obj)
-                result.append(obj)
-                if args.verbose:
-                    print()
-                    print(f'[LABELS]{label}')
-                    if images is not None:
-                        print(f'[IMAGES]{images}')
-                    print('-' * 50)
-    if jsonl_path is not None:
-        logger.info(f'save_result_path: {jsonl_path}')
-    if args.val_dataset_sample == 10:  # is default
-        logger.info('You can set `--val_dataset_sample -1` to perform inference on the entire dataset.')
-    return {'result': result}
-
-
-infer_main = get_main(InferArguments, llm_infer)
-merge_lora_main = get_main(InferArguments, merge_lora)
+    return llm_engine, template
```

### Comparing `ms-swift-2.0.4/swift/llm/rome.py` & `ms-swift-2.0.5/swift/llm/rome.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/llm/sft.py` & `ms-swift-2.0.5/swift/llm/sft.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 import os
 from functools import partial
 from typing import Any, Dict, Union
 
 import json
 import numpy as np
 import torch
+import torch.distributed as dist
+from datasets import Dataset
 from modelscope import BitsAndBytesConfig, GenerationConfig
 from transformers import IntervalStrategy
 from transformers.integrations import is_deepspeed_zero3_enabled
 from transformers.utils import is_torch_npu_available
 
 from swift.trainers import Seq2SeqTrainer
 from swift.trainers.utils import can_return_loss, find_labels
 from swift.utils import (check_json_format, compute_acc_metrics, compute_nlg_metrics, get_dist_setting, get_logger,
                          get_main, get_model_info, is_ddp_plus_mp, is_dist, is_master, plot_images,
                          preprocess_logits_for_metrics, seed_everything, show_layers, use_torchacc)
 from .accelerator import ta_accelerate
 from .tuner import prepare_model
-from .utils import (TEMPLATE_MAPPING, LazyLLMDataset, SftArguments, Template, add_self_cognition_dataset, dataset_map,
-                    get_dataset, get_model_tokenizer, get_template, get_time_info, print_example, set_generation_config,
+from .utils import (TEMPLATE_MAPPING, LazyLLMDataset, SftArguments, Template, dataset_map, get_dataset,
+                    get_model_tokenizer, get_template, get_time_info, print_example, set_generation_config,
                     sort_by_max_length, stat_dataset)
 
 logger = get_logger()
 
 
 def llm_sft(args: SftArguments) -> Dict[str, Union[str, Any]]:
     logger.info(f'args: {args}')
@@ -41,22 +43,48 @@
             torch.cuda.set_per_process_memory_fraction(max(min(args.gpu_memory_fraction, 1.0), 0.01), device=device_id)
 
     # Loading Model and Tokenizer
     if is_deepspeed_zero3_enabled():
         model_kwargs = {'device_map': None}
     elif is_torch_npu_available():
         model_kwargs = {'device_map': local_rank if local_rank >= 0 else 0}
+    elif args.device_map_config_path is not None:
+        cwd = os.getcwd()
+        config_path = args.device_map_config_path if os.path.isabs(args.device_map_config_path) else os.path.join(
+            cwd, args.device_map_config_path)
+        with open(config_path, 'r') as json_file:
+            model_kwargs['device_map'] = json.load(json_file)
     else:
         model_kwargs = {'low_cpu_mem_usage': True}
         if is_dist() and not is_ddp_plus_mp():
             model_kwargs['device_map'] = {'': local_rank}
         elif not use_torchacc():
             model_kwargs['device_map'] = 'auto'
 
-    if args.load_in_8bit or args.load_in_4bit:
+    if args.quant_method == 'hqq':
+        from transformers import HqqConfig
+        if args.hqq_dynamic_config_path is not None:
+            cwd = os.getcwd()
+            config_path = args.hqq_dynamic_config_path if os.path.isabs(args.hqq_dynamic_config_path) else os.path.join(
+                cwd, args.hqq_dynamic_config_path)
+            with open(config_path, 'r') as json_file:
+                quantization_config = HqqConfig(dynamic_config=json.load(json_file))
+        else:
+            if args.quantization_bit == 0:
+                logger.info("You haven't set the quantization_bit parameter; set it to 8.")
+                args.quantization_bit = 8
+            quantization_config = HqqConfig(nbits=args.quantization_bit, axis=args.hqq_axis)
+        logger.info(f'quantization_config: {quantization_config.__dict__}')
+        model_kwargs['quantization_config'] = quantization_config
+    elif args.quant_method == 'eetq':
+        from transformers import EetqConfig
+        quantization_config = EetqConfig('int8')
+        logger.info(f'quantization_config: {quantization_config.__dict__}')
+        model_kwargs['quantization_config'] = quantization_config
+    elif args.load_in_8bit or args.load_in_4bit:  # bnb
         quantization_config = BitsAndBytesConfig(
             args.load_in_8bit,
             args.load_in_4bit,
             bnb_4bit_compute_dtype=args.bnb_4bit_compute_dtype,
             bnb_4bit_quant_type=args.bnb_4bit_quant_type,
             bnb_4bit_use_double_quant=args.bnb_4bit_use_double_quant)
         logger.info(f'quantization_config: {quantization_config.__dict__}')
@@ -65,14 +93,16 @@
     kwargs = {
         'max_length': args.max_length,
         'use_unsloth': args.tuner_backend == 'unsloth',
         'load_in_4bit': args.quantization_bit == 4
     }
     if args.use_flash_attn is not None:
         kwargs['use_flash_attn'] = args.use_flash_attn
+    if args.local_repo_path:
+        kwargs['local_repo_path'] = args.local_repo_path
     model, tokenizer = get_model_tokenizer(
         args.model_type,
         args.torch_dtype,
         model_kwargs,
         model_id_or_path=args.model_id_or_path,
         revision=args.model_revision,
         is_training=True,
@@ -123,60 +153,77 @@
             args.model_layer_cls_name,
             args.bf16,
             args.fp16,
             gradient_checkpointing=True,
             fsdp_flatten_parameters=False)
 
     # Loading Dataset
-    random_state = np.random.RandomState(args.dataset_seed)
     train_dataset, val_dataset = get_dataset(
-        args.dataset, args.dataset_test_ratio, random_state, check_dataset_strategy=args.check_dataset_strategy)
-    val_dataset_sample = args.val_dataset_sample
-    if train_dataset is not None and args.train_dataset_sample >= 0:
-        train_dataset_sample = min(args.train_dataset_sample, train_dataset.shape[0])
-        if train_dataset.shape[0] > train_dataset_sample:
-            logger.info(f'train_dataset_sample: {train_dataset_sample}')
-            train_idxs = random_state.permutation(train_dataset_sample)
-            train_dataset = train_dataset.select(train_idxs)
-        if val_dataset_sample is None:
-            val_dataset_sample = max(int(train_dataset_sample * args.dataset_test_ratio), 1)
-    if val_dataset is not None and val_dataset_sample is not None and val_dataset_sample >= 0:
-        if val_dataset.shape[0] > val_dataset_sample:
-            logger.info(f'val_dataset_sample: {val_dataset_sample}')
-            val_idxs = random_state.permutation(val_dataset_sample)
-            val_dataset = val_dataset.select(val_idxs)
-
-    train_dataset = args.handle_dataset_mixture(train_dataset)
-
-    # add self-cognition dataset
-    if args.self_cognition_sample > 0:
-        train_dataset = add_self_cognition_dataset(train_dataset, args.self_cognition_sample, args.model_name,
-                                                   args.model_author)
+        args.dataset,
+        args.dataset_test_ratio,
+        args.dataset_seed,
+        check_dataset_strategy=args.check_dataset_strategy,
+        model_name=args.model_name,
+        model_author=args.model_author)
+    if args.val_dataset is not None:
+        # Loading val dataset
+        _, val_dataset = get_dataset(
+            args.val_dataset,
+            1.0,
+            args.dataset_seed,
+            check_dataset_strategy=args.check_dataset_strategy,
+            model_name=args.model_name,
+            model_author=args.model_author)
+
+    train_dataset, val_dataset = args._handle_dataset_compat(train_dataset, val_dataset)
     logger.info(f'train_dataset: {train_dataset}')
     logger.info(f'val_dataset: {val_dataset}')
     template_kwargs = {}
     template_info = TEMPLATE_MAPPING[args.template_type]
     use_model = template_info.get('use_model', False)
     if use_model:
         template_kwargs['model'] = model
     template_kwargs['use_loss_scale'] = args.use_loss_scale
+    if args.sequence_parallel_size and args.sequence_parallel_size > 1:
+        template_kwargs['sequence_parallel_size'] = args.sequence_parallel_size
     template: Template = get_template(args.template_type, tokenizer, args.system, args.max_length,
                                       args.truncation_strategy, **template_kwargs)
     args.system = template.default_system
     logger.info(f'system: {args.system}')
     logger.info(f'args.lazy_tokenize: {args.lazy_tokenize}')
-    if not args.lazy_tokenize:
+    if args.packing:
+        from swift.llm.utils.utils import ConstantLengthDataset
+        train_dataset = ConstantLengthDataset.get_packed_dataset(
+            template, train_dataset, args.max_length, lazy_tokenize=args.lazy_tokenize)
+        if val_dataset is not None:
+            val_dataset = ConstantLengthDataset.get_packed_dataset(
+                template, val_dataset, args.max_length, lazy_tokenize=args.lazy_tokenize)
+        dataset_info = {}
+        if not args.lazy_tokenize:
+            td0 = train_dataset[0]
+            print_example(td0, tokenizer, {})
+            dataset_info['train_dataset'] = stat_dataset(train_dataset)
+            if val_dataset is not None:
+                dataset_info['val_dataset'] = stat_dataset(val_dataset)
+    elif not args.lazy_tokenize:
         dataset_info = {}
         logger.info(f'Using num_proc: {args.preprocess_num_proc}')
         train_dataset = dataset_map(train_dataset, template.encode, args.preprocess_num_proc)
         if val_dataset is not None:
             val_dataset = dataset_map(val_dataset, template.encode, args.preprocess_num_proc)
         if args.test_oom_error:
             train_dataset = sort_by_max_length(train_dataset, 20000)
         # Data analysis
+        if train_dataset is None:
+            logger.error('Error accessing train_dataset properties. '
+                         'Please ensure that the dataset is properly initialized,'
+                         'and every sample of the train_dataset not empty.')
+            raise AttributeError('Failed to access dataset attributes,train_dataset is None. This might be because:\n'
+                                 '(1) The dataset contains None for input or labels;\n'
+                                 "(2) The 'max_length' setting is too short causing data truncation.")
         td0, tkwargs0 = train_dataset.data[0]
         print_example(td0, tokenizer, tkwargs0)
         dataset_info['train_dataset'] = stat_dataset(train_dataset)
         if val_dataset is not None:
             dataset_info['val_dataset'] = stat_dataset(val_dataset)
     else:
         dataset_info = None
@@ -218,14 +265,15 @@
         model=model,
         args=training_args,
         data_collator=data_collator,
         train_dataset=train_dataset,
         eval_dataset=val_dataset,
         tokenizer=tokenizer,
         callbacks=callbacks,
+        sequence_parallel_size=args.sequence_parallel_size,
         **trainer_kwargs)
     trainer.sft_args = args
     if use_torchacc():
         trainer.label_names = label_names
         trainer.can_return_loss = return_loss
     if is_master():
         for args_obj, fname in zip([args, training_args], ['sft_args.json', 'training_args.json']):
```

### Comparing `ms-swift-2.0.4/swift/llm/tuner.py` & `ms-swift-2.0.5/swift/llm/tuner.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,77 +5,119 @@
 import numpy as np
 import torch
 import transformers
 from packaging import version
 
 from swift.torchacc_utils import consolidate_checkpoint
 from swift.trainers import TrainerCallback
-from swift.tuners import (AdaLoraConfig, AdapterConfig, IA3Config, LongLoRAModelType, LoraConfig, LoRAConfig,
-                          NEFTuneConfig, Swift)
+from swift.tuners import (AdaLoraConfig, AdapterConfig, BOFTConfig, IA3Config, LongLoRAModelType, LoraConfig,
+                          LoRAConfig, NEFTuneConfig, Swift, VeraConfig)
 from swift.tuners.llamapro import LLaMAProConfig
 from swift.tuners.module_mapping import MODEL_KEYS_MAPPING
 from swift.utils import activate_model_parameters, freeze_model_parameters, get_logger, use_torchacc
 from .utils import SftArguments, find_all_linears, find_embedding, find_ln, is_adapter
 
 logger = get_logger()
 
 
 def handle_target_modules(model, args: SftArguments) -> None:
     if args.sft_type == 'ia3':
         target_modules = args.ia3_target_modules
         assert len(args.ia3_feedforward_modules) > 0, ('Setting ia3_target_modules to `ALL` '
                                                        'need to pass MLP linear names to `ia3_feedforward_modules`')
+    elif args.sft_type == 'vera':
+        target_modules = args.vera_target_modules
+    elif args.sft_type == 'boft':
+        target_modules = args.boft_target_modules
     else:
         target_modules = args.lora_target_modules
     if args.lora_use_embedding:
         target_modules += find_embedding(model)
     if args.lora_use_all:
         target_modules += find_all_linears(model, args.quantization_bit, args.model_type)
     if args.sft_type == 'ia3':
         args.ia3_target_modules = target_modules
         logger.info(f'ia3_target_modules: {args.ia3_target_modules}')
+    elif args.sft_type == 'vera':
+        args.vera_target_modules = target_modules
+        logger.info(f'vera_target_modules: {args.ia3_target_modules}')
+    elif args.sft_type == 'boft':
+        args.boft_target_modules = target_modules
+        logger.info(f'boft_target_modules: {args.boft_target_modules}')
     else:
         args.lora_target_modules = target_modules
         logger.info(f'lora_target_modules: {args.lora_target_modules}')
 
 
+def handle_same_dim_target_modules(model: torch.nn.Module, config: VeraConfig):
+    target_modules = config.target_modules
+    modules_dict = {
+        name: module.weight.shape
+        for name, module in model.named_modules()
+        if isinstance(module, torch.nn.Linear) and any([t in name for t in target_modules])
+    }  # only Linear for now
+    if len(set(modules_dict.values())) > 1:
+        v = [t for t in target_modules if 'v' in t]
+        if not v:
+            raise ValueError('Please manually pass in `vera_target_modules`, do not use `DEFAULT` or `ALL`,'
+                             'because Vera need all target linears to be the same size.')
+        v = v[0]
+        shape = [shape for name, shape in modules_dict.items() if v in name][0]
+        names = [_name for _name, _shape in modules_dict.items() if _shape == shape]
+        config.target_modules = [t for t in target_modules if any([t in name for name in names])]
+    return config
+
+
 def handle_modules_to_save(model, args: SftArguments) -> None:
     if args.sft_type == 'ia3':
         modules_to_save = args.ia3_modules_to_save
+    elif args.sft_type == 'vera':
+        modules_to_save = args.vera_modules_to_save
+    elif args.sft_type == 'boft':
+        modules_to_save = args.boft_modules_to_save
     else:
         modules_to_save = args.lora_modules_to_save
     if args.lora_m2s_use_embedding:
         modules_to_save += find_embedding(model)
     if args.lora_m2s_use_ln:
         modules_to_save += find_ln(model)
 
     if args.sft_type == 'ia3':
         args.ia3_modules_to_save = modules_to_save
         logger.info(f'ia3_modules_to_save: {args.ia3_modules_to_save}')
+    elif args.sft_type == 'vera':
+        args.vera_modules_to_save = modules_to_save
+        logger.info(f'vera_modules_to_save: {args.vera_modules_to_save}')
+    elif args.sft_type == 'boft':
+        args.boft_modules_to_save = modules_to_save
+        logger.info(f'boft_modules_to_save: {args.boft_modules_to_save}')
     else:
         args.lora_modules_to_save = modules_to_save
         logger.info(f'lora_modules_to_save: {args.lora_modules_to_save}')
 
 
 def prepare_model(model, args: SftArguments):
     # Preparing LoRA
     if is_adapter(args.sft_type):
         if args.resume_from_checkpoint is None:
             handle_target_modules(model, args)
             handle_modules_to_save(model, args)
+            if args.init_lora_weights and args.init_lora_weights.lower() in ('true', 'false'):
+                args.init_lora_weights = args.init_lora_weights.lower() in ('true', 'True')
             lora_kwargs = {
                 'r': args.lora_rank,
                 'target_modules': args.lora_target_modules,
                 'lora_alpha': args.lora_alpha,
                 'lora_dropout': args.lora_dropout_p,
                 'bias': args.lora_bias_trainable,
                 'modules_to_save': args.lora_modules_to_save,
                 'use_rslora': args.use_rslora,
                 'use_dora': args.use_dora,
                 'lorap_lr_ratio': args.lora_lr_ratio,
+                'init_lora_weights': args.init_lora_weights,
             }
             if args.sft_type in ('lora', 'longlora'):
                 if args.lora_dtype == 'AUTO':
                     args.lora_dtype = None
                 if args.tuner_backend == 'swift':
                     lora_config = LoRAConfig(lora_dtype=args.lora_dtype, **lora_kwargs)
                     model = Swift.prepare_model(model, lora_config)
@@ -154,14 +196,37 @@
                     dim=model.config.hidden_size,
                     target_modules=[mlp_key],
                     hidden_pos=0,
                     adapter_length=args.adapter_length,
                     act_layer=args.adapter_act)
                 model = Swift.prepare_model(model, adapter_config)
                 logger.info(f'adapter_config: {adapter_config}')
+            elif args.sft_type == 'vera':
+                vera_config = VeraConfig(
+                    r=args.vera_rank,
+                    target_modules=args.vera_target_modules,
+                    projection_prng_key=args.vera_projection_prng_key,
+                    vera_dropout=args.vera_dropout,
+                    d_initial=args.vera_d_initial,
+                    modules_to_save=args.vera_modules_to_save,
+                )
+                vera_config = handle_same_dim_target_modules(model, vera_config)
+                model = Swift.prepare_model(model, vera_config)
+                logger.info(f'vera_config: {vera_config}')
+            elif args.sft_type == 'boft':
+                boft_config = BOFTConfig(
+                    boft_block_size=args.boft_block_size,
+                    boft_block_num=args.boft_block_num,
+                    boft_n_butterfly_factor=args.boft_n_butterfly_factor,
+                    target_modules=args.boft_target_modules,
+                    boft_dropout=args.boft_dropout,
+                    modules_to_save=args.boft_modules_to_save,
+                )
+                model = Swift.prepare_model(model, boft_config)
+                logger.info(f'boft_config: {boft_config}')
         else:
             if use_torchacc():
                 consolidate_checkpoint(args.resume_from_checkpoint, 'adapter_model')
             model = Swift.from_pretrained(model, args.resume_from_checkpoint, is_trainable=True)
         # fix bug: Attempting to unscale FP16 gradients.
         #   peft: https://github.com/huggingface/peft/issues/1249
         #   modules_to_save + fp16
@@ -183,14 +248,17 @@
             state_dict = torch.load(weights_file, map_location='cpu')
             model.load_state_dict(state_dict, False)
             # release memory
             del state_dict
     else:
         raise ValueError(f'args.sft_type: {args.sft_type}')
 
+    if args.sequence_parallel_size > 1:
+        from swift.trainers.xtuner import dispatch_module_xtuner
+        dispatch_module_xtuner(model)
     if args.neftune_backend == 'swift' and args.neftune_noise_alpha not in {None, 0.}:
         neftune_config = NEFTuneConfig(noise_alpha=args.neftune_noise_alpha)
         model = Swift.prepare_model(model, {'neftune': neftune_config})
         logger.info(f'neftune_config: {neftune_config}')
 
     if args.use_galore:
         from swift.trainers.optimizers.galore import GaLoreConfig
@@ -252,19 +320,20 @@
                 layers = self.model.get_submodule(self.layers_attribute)
                 self.active_layers_indices = np.random.choice(range(self.total_layers), self.n_layers, replace=False)
                 # Enable gradients only for the selected layers
                 for idx in self.active_layers_indices:
                     for param in layers[idx].parameters():
                         param.requires_grad = True
 
-        callbacks.append(
-            DynamicLayerActivationCallback(
-                n_layers=args.lisa_activated_layers,  # Number of layers to activate
-                step_interval=args.lisa_step_interval,  # Step interval to update active layers
-                model=model))
+        lisa_callback = DynamicLayerActivationCallback(
+            n_layers=args.lisa_activated_layers,  # Number of layers to activate
+            step_interval=args.lisa_step_interval,  # Step interval to update active layers
+            model=model)
+        lisa_callback.switch_active_layers()  # Make trainable parameters printing a correct value
+        callbacks.append(lisa_callback)
 
     class TrainerAdapterCallback(TrainerCallback):
 
         def __init__(self):
             self.global_step = 0
 
         # offload original_modules to cpu, to save memory
```

### Comparing `ms-swift-2.0.4/swift/llm/utils/__init__.py` & `ms-swift-2.0.5/swift/llm/utils/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 from .argument import (AppUIArguments, DeployArguments, DPOArguments, EvalArguments, ExportArguments, InferArguments,
-                       RomeArguments, SftArguments, is_adapter, swift_to_peft_format)
+                       ORPOArguments, RomeArguments, SftArguments, is_adapter, swift_to_peft_format)
 from .client_utils import get_model_list_client, inference_client
-from .dataset import (DATASET_MAPPING, DatasetName, GetDatasetFunction, HfDataset, add_self_cognition_dataset,
-                      get_dataset, get_dataset_from_repo, load_dataset_from_local, load_ms_dataset, register_dataset)
+from .dataset import (DATASET_MAPPING, DatasetName, GetDatasetFunction, HfDataset, get_dataset, get_dataset_from_repo,
+                      load_dataset_from_local, load_ms_dataset, register_dataset, register_dataset_info,
+                      register_local_dataset, sample_dataset)
 from .model import (MODEL_MAPPING, GetModelTokenizerFunction, LoRATM, ModelType, get_additional_saved_files,
                     get_default_lora_target_modules, get_default_template_type, get_model_tokenizer,
                     get_model_tokenizer_from_repo, get_model_tokenizer_with_flash_attn, register_model)
 from .preprocess import (AlpacaPreprocessor, ClsPreprocessor, ComposePreprocessor, ConversationsPreprocessor,
                          PreprocessFunc, RenameColumnsPreprocessor, SmartPreprocessor, SwiftPreprocessor,
                          TextGenerationPreprocessor)
 from .protocol import ChatCompletionResponse  # noqa
```

### Comparing `ms-swift-2.0.4/swift/llm/utils/argument.py` & `ms-swift-2.0.5/swift/llm/utils/argument.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 import inspect
 import math
 import os
+import sys
 from dataclasses import dataclass, field
 from typing import List, Literal, Optional, Set, Tuple, Union
 
 import json
 import numpy as np
 import torch
 import transformers
@@ -17,63 +18,62 @@
 from transformers.utils.versions import require_version
 
 from swift.hub import HubApi, ModelScopeConfig
 from swift.trainers import Seq2SeqTrainingArguments
 from swift.tuners import Swift
 from swift.utils import (add_version_to_work_dir, get_dist_setting, get_logger, get_pai_tensorboard_dir, is_dist,
                          is_local_master, is_mp, is_pai_training_job)
-from .dataset import DATASET_MAPPING, get_custom_dataset, get_dataset, register_dataset
+from .dataset import DATASET_MAPPING, _dataset_name_exists, get_dataset, register_dataset_info_file, sample_dataset
 from .model import (MODEL_MAPPING, dtype_mapping, get_additional_saved_files, get_default_lora_target_modules,
                     get_default_template_type)
 from .template import TEMPLATE_MAPPING
 from .utils import is_vllm_available
 
 logger = get_logger()
 
 
 def is_adapter(sft_type: str) -> bool:
-    return sft_type in {'lora', 'longlora', 'adalora', 'ia3', 'llamapro', 'adapter'}
+    return sft_type in {'lora', 'longlora', 'adalora', 'ia3', 'llamapro', 'adapter', 'vera', 'boft'}
 
 
 class ArgumentsBase:
 
-    def register_custom_dataset(self: Union['SftArguments', 'InferArguments']) -> None:
-        dataset = []
-        for d in self.dataset:
-            if os.path.exists(d):
-                self.custom_train_dataset_path.append(d)
-            else:
-                dataset.append(d)
-        self.dataset = dataset
-
-        for key in ['custom_train_dataset_path', 'custom_val_dataset_path']:
-            value = getattr(self, key)
-            if isinstance(value, str):
-                setattr(self, key, [value])
-        if len(self.custom_train_dataset_path) == 0 and len(self.custom_val_dataset_path) == 0:
-            return
-
-        dataset_name = '_custom_dataset'
-        _register_local_dataset(dataset_name, self.custom_train_dataset_path, self.custom_val_dataset_path)
-        self.dataset.append(dataset_name)
+    @classmethod
+    def _check_path(cls, k: str, value: Union[str, List[str]],
+                    check_exist_path_set: Optional[Set[str]]) -> Union[str, List[str]]:
+        if isinstance(value, str):
+            value = os.path.expanduser(value)
+            value = os.path.abspath(value)
+            if k in check_exist_path_set and not os.path.exists(value):
+                raise FileNotFoundError(f"`{k}`: '{value}'")
+        elif isinstance(value, list):
+            res = []
+            for v in value:
+                res.append(cls._check_path(k, v, check_exist_path_set))
+            value = res
+        return value
 
     def handle_path(self: Union['SftArguments', 'InferArguments']) -> None:
-        check_exist_path = [
-            'ckpt_dir', 'resume_from_checkpoint', 'custom_train_dataset_path', 'custom_val_dataset_path'
-        ]
-        if self.model_id_or_path is not None and (self.model_id_or_path.startswith('~')
-                                                  or self.model_id_or_path.startswith('/')):
-            check_exist_path.append('model_id_or_path')
+        check_exist_path = ['ckpt_dir', 'resume_from_checkpoint', 'custom_register_path']
+        maybe_check_exist_path = ['model_id_or_path', 'custom_dataset_info']
+        if isinstance(self, SftArguments):
+            check_exist_path.append('deepspeed_config_path')
+            maybe_check_exist_path.append('deepspeed')
+
+        for k in maybe_check_exist_path:
+            v = getattr(self, k)
+            if isinstance(v, str) and v is not None and (v.startswith('~') or v.startswith('/') or os.path.exists(v)):
+                check_exist_path.append(k)
         check_exist_path_set = set(check_exist_path)
         other_path = ['output_dir', 'logging_dir']
         for k in check_exist_path + other_path:
             value = getattr(self, k, None)
             if value is None:
                 continue
-            value = _check_path(k, value, check_exist_path_set)
+            value = self._check_path(k, value, check_exist_path_set)
             setattr(self, k, value)
 
     def check_flash_attn(self: Union['SftArguments', 'InferArguments']) -> None:
         model_info = MODEL_MAPPING[self.model_type]
         support_flash_attn = model_info.get('support_flash_attn', False)
         if self.use_flash_attn and not support_flash_attn:
             logger.warning(f'use_flash_attn: {self.use_flash_attn}, ' f'but support_flash_attn: {support_flash_attn}')
@@ -140,76 +140,227 @@
 
         if self.bnb_4bit_comp_dtype != 'AUTO':
             bnb_4bit_compute_dtype = dtype_mapping_reversed[self.bnb_4bit_comp_dtype]
             assert bnb_4bit_compute_dtype in {torch.float16, torch.bfloat16, torch.float32}
         else:
             bnb_4bit_compute_dtype = None
         quantization_bit = self.quantization_bit
-        if quantization_bit == 4:
-            require_version('bitsandbytes')
-            load_in_4bit, load_in_8bit = True, False
-        elif quantization_bit == 8:
-            require_version('bitsandbytes')
-            load_in_4bit, load_in_8bit = False, True
+        if self.quant_method == 'bnb':
+            if quantization_bit == 4:
+                require_version('bitsandbytes')
+                load_in_4bit, load_in_8bit = True, False
+            elif quantization_bit == 8:
+                require_version('bitsandbytes')
+                load_in_4bit, load_in_8bit = False, True
         else:
             load_in_4bit, load_in_8bit = False, False
 
         return bnb_4bit_compute_dtype, load_in_4bit, load_in_8bit
 
+    def handle_custom_register(self: Union['SftArguments', 'InferArguments']) -> None:
+        if self.custom_register_path is None:
+            return
+        folder, fname = os.path.split(self.custom_register_path)
+        sys.path.append(folder)
+        __import__(fname.rstrip('.py'))
+
     def handle_compatibility(self: Union['SftArguments', 'InferArguments']) -> None:
         template_type_mapping = {'chatglm2-generation': 'chatglm-generation', 'chatml': 'qwen'}
         model_type_mapping = {
             'openbmb-minicpm-2b-sft-chat': 'minicpm-2b-sft-chat',
             'openbmb-minicpm-2b-chat': 'minicpm-2b-chat',
+            'cogvlm-17b-instruct': 'cogvlm-17b-chat',
+            'minicpm-v-v2': 'minicpm-v-v2-chat'
         }
-        for k, v in template_type_mapping.items():
-            if k == self.template_type:
-                self.template_type = v
-                break
-        for k, v in model_type_mapping.items():
-            if k == self.model_type:
-                self.model_type = v
+        dataset_name_mapping = {
+            'ms-bench-mini': 'ms-bench#20000',
+            'multi-alpaca-all': 'multi-alpaca',
+            'instinwild-en': 'instinwild:subset',
+            'instinwild-zh': 'instinwild:default',
+            'firefly-all-zh': 'firefly-zh',
+            'sharegpt-en': 'sharegpt:common-en/computer-en',
+            'sharegpt-zh': 'sharegpt:common-zh/computer-zh/unknow-zh',
+            'open-orca-gpt4': 'open-orca:default',
+            'sharegpt-gpt4-mini': 'sharegpt-gpt4:default',
+            'deepctrl-sft-zh': 'deepctrl-sft:default',
+            'deepctrl-sft-en': 'deepctrl-sft:en',
+            'ms-agent-for-agentfabric-default': 'ms-agent-for-agentfabric:default',
+            'ms-agent-for-agentfabric-addition': 'ms-agent-for-agentfabric:addition',
+            **{
+                f'toolbench-for-alpha-umi-{sn}': f'toolbench-for-alpha-umi:{sn}'
+                for sn in DATASET_MAPPING['toolbench-for-alpha-umi']['subsets']
+            },
+            'medical-mini-zh': 'medical-zh#50000',
+            'cmnli-mini-zh': 'cmnli-zh#20000/200',
+            'coco-mini-en': 'coco-en-mini',
+            'coco-mini-en-2': 'coco-en-2-mini',
+            'aishell1-mini-zh': 'aishell1-zh-mini',
+            **{f'hh-rlhf-{sn}': f'hh-rlhf:{sn}'
+               for sn in DATASET_MAPPING['hh-rlhf']['subsets']},
+            **{
+                f"hh-rlhf-cn-{sn.replace('_', '-')}": f'hh-rlhf-cn:{sn}'
+                for sn in DATASET_MAPPING['hh-rlhf-cn']['subsets']
+            },
+            **{
+                f"coig-cqia-{sn.replace('_', '-')}": f'coig-cqia:{sn}'
+                for sn in DATASET_MAPPING['coig-cqia']['subsets']
+            },
+            **{f'ruozhiba-{sn}': f'ruozhiba:{sn}'
+               for sn in DATASET_MAPPING['ruozhiba']['subsets']},
+        }
+        for _name, _mapping in [['template_type', template_type_mapping], ['model_type', model_type_mapping]]:
+            k = getattr(self, _name)
+            if k in _mapping:
+                v = _mapping[k]
+                setattr(self, _name, v)
                 break
-        if self.dataset is not None and len(self.dataset) == 1 and ',' in self.dataset[0]:
+        if isinstance(self.dataset, str):
+            self.dataset = [self.dataset]
+        if len(self.dataset) == 1 and ',' in self.dataset[0]:
             self.dataset = self.dataset[0].split(',')
+        for i, dataset in enumerate(self.dataset):
+            if dataset in dataset_name_mapping:
+                self.dataset[i] = dataset_name_mapping[dataset]
+        for d in self.dataset:
+            assert ',' not in d, f'dataset: {d}, please use `/`'
         if self.truncation_strategy == 'ignore':
             self.truncation_strategy = 'delete'
+        if self.safe_serialization is not None:
+            self.save_safetensors = self.safe_serialization
+        if len(self.custom_train_dataset_path) > 0:
+            self.dataset += self.custom_train_dataset_path
+        if len(self.custom_val_dataset_path) > 0:
+            self.dataset += self.custom_val_dataset_path
+
         if isinstance(self, InferArguments):
-            if self.show_dataset_sample != 10 and self.val_dataset_sample == 10:
-                # args.val_dataset_sample is the default value and args.show_dataset_sample is not the default value.
-                self.val_dataset_sample = self.show_dataset_sample
-            if self.safe_serialization is not None:
-                self.save_safetensors = self.safe_serialization
             if self.merge_lora_and_save is not None:
                 self.merge_lora = self.merge_lora_and_save
+            if self.vllm_lora_modules is not None:
+                self.lora_modules = self.vllm_lora_modules
+        if isinstance(self, AppUIArguments):
+            if self.server_name is not None:
+                self.host = self.server_name
+            if self.server_port is not None:
+                self.port = self.server_port
         if isinstance(self, SftArguments):
+            if isinstance(self.train_dataset_mix_ds, str):
+                self.train_dataset_mix_ds = [self.train_dataset_mix_ds]
             if self.only_save_model is not None:
                 self.save_only_model = self.only_save_model
             if self.neftune_alpha is not None:
                 self.neftune_noise_alpha = self.neftune_alpha
             if self.per_device_train_batch_size is not None:
                 self.batch_size = self.per_device_train_batch_size
             if self.per_device_eval_batch_size is not None:
                 self.eval_batch_size = self.per_device_eval_batch_size
             if self.deepspeed_config_path is not None:
                 self.deepspeed = self.deepspeed_config_path
 
+    def handle_custom_dataset_info(self):
+        if self.custom_dataset_info is None:
+            return
+        register_dataset_info_file(self.custom_dataset_info)
+
+    def _handle_dataset_sample(self):
+        # compatibility. (Deprecated)
+        # Avoid post-processing
+        if len(self.dataset) == 1 and '#' not in self.dataset[0] and self.train_dataset_sample >= 0:
+            self.dataset[0] = f'{self.dataset[0]}#{self.train_dataset_sample}'
+            self.train_dataset_sample = -1
+
+    def _register_self_cognition(self: Union['SftArguments', 'InferArguments']) -> None:
+
+        # compatibility. (Deprecated)
+        idx_list = _dataset_name_exists(self.dataset, 'self-cognition')
+        assert len(idx_list) <= 1
+        self.use_self_cognition = len(idx_list) == 1
+        if self.self_cognition_sample > 0:
+            d = f'self-cognition#{self.self_cognition_sample}'
+            if len(idx_list) == 1:
+                self.dataset[idx_list[0]] = d
+            else:
+                self.dataset.append(d)
+            self.use_self_cognition = True
+        # check
+        if self.use_self_cognition:
+            for k in ['model_name', 'model_author']:
+                v = getattr(self, k)
+                if isinstance(v, str):
+                    v = [v]
+                elif v is None:
+                    v = [None, None]
+                if len(v) == 1:
+                    v = v * 2
+                if v[0] is None and v[1] is None:
+                    raise ValueError('Please set self.model_name self.model_author. '
+                                     'For example: `--model_name 小黄 "Xiao Huang" --model_author 魔搭 ModelScope`. '
+                                     'Representing the model name and model author in Chinese and English.')
+                setattr(self, k, v)
+
+    def _handle_dataset_compat(self, train_dataset: HfDataset,
+                               val_dataset: Optional[HfDataset]) -> Tuple[HfDataset, Optional[HfDataset]]:
+        # compatibility. (Deprecated)
+        random_state = np.random.RandomState(self.dataset_seed)
+        val_dataset_sample = self.val_dataset_sample
+        if train_dataset is not None and self.train_dataset_sample >= 0:
+            train_dataset_sample = min(self.train_dataset_sample, train_dataset.shape[0])
+            if train_dataset.shape[0] > train_dataset_sample:
+                logger.info(f'train_dataset_sample: {train_dataset_sample}')
+                train_idxs = random_state.permutation(train_dataset_sample)
+                train_dataset = train_dataset.select(train_idxs)
+            if val_dataset_sample is None:
+                val_dataset_sample = max(int(train_dataset_sample * self.dataset_test_ratio), 1)
+        if val_dataset is not None and val_dataset_sample is not None and val_dataset_sample >= 0:
+            if val_dataset.shape[0] > val_dataset_sample:
+                logger.info(f'val_dataset_sample: {val_dataset_sample}')
+                val_idxs = random_state.permutation(val_dataset_sample)
+                val_dataset = val_dataset.select(val_idxs)
+
+        if (train_dataset is None or not hasattr(self, 'train_dataset_mix_ratio') or self.train_dataset_mix_ratio <= 0
+                or len(self.train_dataset_mix_ds) == 0):
+            return train_dataset, val_dataset
+
+        mix_dataset_sample = int(len(train_dataset) * self.train_dataset_mix_ratio)
+        logger.info(f'train_dataset_mix_ds: {self.train_dataset_mix_ds}')
+        logger.info(f'len(train_dataset): {len(train_dataset)}, mix_dataset_sample: {mix_dataset_sample}')
+        mixed_dataset = get_dataset(
+            self.train_dataset_mix_ds, 0.0, random_state, check_dataset_strategy=self.check_dataset_strategy)[0]
+        if len(mixed_dataset) < mix_dataset_sample:
+            logger.warn(f'The length of dataset used for mixin: {self.train_dataset_mix_ds} are '
+                        'lesser than the ratio required by the `train_dataset_mix_ratio` '
+                        f'argument: {self.train_dataset_mix_ratio}. '
+                        f'the actual ratio is: {len(mixed_dataset) / len(train_dataset):.6}.')
+        else:
+            mixed_dataset = sample_dataset(mixed_dataset, mix_dataset_sample, random_state)
+        train_dataset = concatenate_datasets([train_dataset, mixed_dataset])
+        return train_dataset, val_dataset
+
     def prepare_template(self):
         if self.template_type == 'AUTO':
             self.template_type = get_default_template_type(self.model_type)
             logger.info(f'Setting template_type: {self.template_type}')
 
     def set_model_type(self: Union['SftArguments', 'InferArguments']) -> None:
         # compat with swift<1.7
         if self.model_cache_dir is not None and self.model_id_or_path is None:
             self.model_id_or_path = self.model_cache_dir
             self.model_cache_dir = None
 
         if self.model_id_or_path is not None:
-            model_mapping_reversed = {v['model_id_or_path'].lower(): k for k, v in MODEL_MAPPING.items()}
+            use_hf = strtobool(os.environ.get('USE_HF', 'False'))
+            model_mapping_reversed = {}
+            for k, v in MODEL_MAPPING.items():
+                if use_hf:
+                    model_id = v.get('hf_model_id')
+                else:
+                    model_id = v.get('model_id_or_path')
+                if model_id is None:
+                    continue
+                model_id = model_id.lower()
+                model_mapping_reversed[model_id] = k
             model_id_or_path = self.model_id_or_path
             model_id_or_path_lower = model_id_or_path.lower()
             if model_id_or_path_lower not in model_mapping_reversed:
                 if (isinstance(self, InferArguments) and 'checkpoint' in model_id_or_path
                         and 'merged' not in model_id_or_path and self.ckpt_dir is None):
                     raise ValueError('Please use `--ckpt_dir vx-xxx/checkpoint-xxx` to use the checkpoint.')
                 if self.model_type is None:
@@ -247,19 +398,16 @@
 @dataclass
 class SftArguments(ArgumentsBase):
     # You can specify the model by either using the model_type or model_id_or_path.
     model_type: Optional[str] = field(
         default=None, metadata={'help': f'model_type choices: {list(MODEL_MAPPING.keys())}'})
     model_id_or_path: Optional[str] = None
     model_revision: Optional[str] = None
-    model_layer_cls_name: Optional[str] = field(
-        default=None,
-        metadata={'help': "Decoder Class name of model, e.g. 'QWenBlock' for QWen, 'LlamaDecoderLayer' for LLama"})
 
-    sft_type: Literal['lora', 'full', 'longlora', 'adalora', 'ia3', 'llamapro', 'adapter'] = 'lora'
+    sft_type: Literal['lora', 'full', 'longlora', 'adalora', 'ia3', 'llamapro', 'adapter', 'vera', 'boft'] = 'lora'
     freeze_parameters: float = 0.  # 0 ~ 1
     additional_trainable_parameters: List[str] = field(default_factory=list)
     tuner_backend: Literal['swift', 'peft', 'unsloth'] = 'peft'
     template_type: str = field(
         default='AUTO', metadata={'help': f"template_type choices: {list(TEMPLATE_MAPPING.keys()) + ['AUTO']}"})
     output_dir: str = 'output'
     add_output_dir_suffix: Optional[bool] = None
@@ -267,39 +415,35 @@
     ddp_find_unused_parameters: Optional[bool] = None
     ddp_broadcast_buffers: Optional[bool] = None
 
     seed: int = 42
     resume_from_checkpoint: Optional[str] = None
     ignore_data_skip: bool = False
     dtype: Literal['bf16', 'fp16', 'fp32', 'AUTO'] = 'AUTO'
+    packing: bool = False
 
     dataset: List[str] = field(
         default_factory=list, metadata={'help': f'dataset choices: {list(DATASET_MAPPING.keys())}'})
+    val_dataset: List[str] = field(default=None, metadata={'help': f'dataset choices: {list(DATASET_MAPPING.keys())}'})
     dataset_seed: int = 42
     dataset_test_ratio: float = 0.01
-    train_dataset_sample: int = -1  # -1: all dataset
-    train_dataset_mix_ratio: float = 0.
-    train_dataset_mix_ds: List[str] = field(default_factory=lambda: ['ms-bench'])
-    val_dataset_sample: Optional[int] = None  # -1: all dataset
-    use_loss_scale: bool = False
+    use_loss_scale: bool = False  # for agent
     system: Optional[str] = None
     max_length: int = 2048  # -1: no limit
     truncation_strategy: Literal['delete', 'truncation_left'] = 'delete'
     check_dataset_strategy: Literal['none', 'discard', 'error', 'warning'] = 'none'
-    custom_train_dataset_path: List[str] = field(default_factory=list)
-    custom_val_dataset_path: List[str] = field(default_factory=list)
-    self_cognition_sample: int = 0
     # Chinese name and English name
     model_name: List[str] = field(default_factory=lambda: [None, None], metadata={'help': "e.g. ['小黄', 'Xiao Huang']"})
     model_author: List[str] = field(
         default_factory=lambda: [None, None], metadata={'help': "e.g. ['魔搭', 'ModelScope']"})
-    # If you want to use qlora, set the quantization_bit to 8 or 4.
-    # And you need to install bitsandbytes: `pip install bitsandbytes -U`
     # note: bf16 and quantization have requirements for gpu architecture
-    quantization_bit: Literal[0, 4, 8] = 0
+    quant_method: Literal['bnb', 'hqq', 'eetq'] = None
+    quantization_bit: Literal[0, 1, 2, 3, 4, 8] = 0  # hqq: 1,2,3,4,8. bnb: 4,8
+    hqq_axis: Literal[0, 1] = 0
+    hqq_dynamic_config_path: Optional[str] = None
     bnb_4bit_comp_dtype: Literal['fp16', 'bf16', 'fp32', 'AUTO'] = 'AUTO'
     bnb_4bit_quant_type: Literal['fp4', 'nf4'] = 'nf4'
     bnb_4bit_use_double_quant: bool = True
     bnb_4bit_quant_storage: Optional[str] = None
     # lora
     lora_target_modules: List[str] = field(default_factory=lambda: ['DEFAULT'])
     lora_rank: int = 8
@@ -308,14 +452,31 @@
     lora_bias_trainable: Literal['none', 'all'] = 'none'
     # e.g. ['wte', 'ln_1', 'ln_2', 'ln_f', 'lm_head']
     lora_modules_to_save: List[str] = field(default_factory=list)
     lora_dtype: Literal['fp16', 'bf16', 'fp32', 'AUTO'] = 'AUTO'
     lora_lr_ratio: float = None
     use_rslora: bool = False
     use_dora: bool = False
+    init_lora_weights: Literal['gaussian', 'pissa', 'pissa_niter_[number of iters]', 'loftq', 'true', 'false'] = 'true'
+
+    # BOFT
+    boft_block_size: int = 4
+    boft_block_num: int = 0
+    boft_n_butterfly_factor: int = 1
+    boft_target_modules: List[str] = field(default_factory=lambda: ['DEFAULT'])
+    boft_dropout: float = 0.0
+    boft_modules_to_save: List[str] = field(default_factory=list)
+
+    # Vera
+    vera_rank: int = 256
+    vera_target_modules: List[str] = field(default_factory=lambda: ['DEFAULT'])
+    vera_projection_prng_key: int = 0
+    vera_dropout: float = 0.0
+    vera_d_initial: float = 0.1
+    vera_modules_to_save: List[str] = field(default_factory=list)
 
     # adapter
     adapter_act: str = 'gelu'
     adapter_length: int = 128
 
     # galore
     use_galore: bool = False
@@ -404,75 +565,62 @@
     ignore_args_error: bool = False  # True: notebook compatibility
     check_model_is_latest: bool = True
 
     logging_dir: Optional[str] = None
     report_to: List[str] = field(default_factory=lambda: ['tensorboard'])
     acc_strategy: Literal['token', 'sentence'] = 'token'
     save_on_each_node: bool = True
-    evaluation_strategy: Literal['steps', 'no'] = 'steps'
-    save_strategy: Literal['steps', 'no'] = 'steps'
+    evaluation_strategy: Literal['steps', 'epoch', 'no'] = 'steps'
+    save_strategy: Literal['steps', 'epoch', 'no'] = 'steps'
     save_safetensors: bool = True
     gpu_memory_fraction: Optional[float] = None
     include_num_input_tokens_seen: Optional[bool] = False
+    local_repo_path: Optional[str] = None
+    custom_register_path: Optional[str] = None  # .py
+    custom_dataset_info: Optional[str] = None  # .json
+
+    device_map_config_path: Optional[str] = None
 
     # generation config
     max_new_tokens: int = 2048
     do_sample: bool = True
     temperature: float = 0.3
     top_k: int = 20
     top_p: float = 0.7
     repetition_penalty: float = 1.
     num_beams: int = 1
+
+    # fsdp option
+    fsdp: Optional[str] = ''
+    # fsdp config file
+    fsdp_config: Optional[str] = None
+
+    sequence_parallel_size: int = 1
+    # for torchacc
+    model_layer_cls_name: Optional[str] = field(
+        default=None,
+        metadata={'help': "Decoder Class name of model, e.g. 'QWenBlock' for QWen, 'LlamaDecoderLayer' for LLama"})
+
     # compatibility hf
     per_device_train_batch_size: Optional[int] = None
     per_device_eval_batch_size: Optional[int] = None
     # compatibility. (Deprecated)
+    self_cognition_sample: int = 0
+    train_dataset_mix_ratio: float = 0.
+    train_dataset_mix_ds: List[str] = field(default_factory=lambda: ['ms-bench'])
+    train_dataset_sample: int = -1  # -1: all dataset
+    val_dataset_sample: Optional[int] = None  # -1: all dataset
+    safe_serialization: Optional[bool] = None
     only_save_model: Optional[bool] = None
     neftune_alpha: Optional[float] = None
     deepspeed_config_path: Optional[str] = None
     model_cache_dir: Optional[str] = None
 
-    # fsdp option
-    fsdp: Optional[str] = ''
-    # fsdp config file
-    fsdp_config: Optional[str] = None
-
-    def handle_dataset_mixture(self, train_dataset: HfDataset) -> None:
-        if train_dataset is None:
-            return train_dataset
-        if self.train_dataset_mix_ratio <= 0 or len(self.train_dataset_mix_ds) == 0:
-            return train_dataset
-
-        random_state = np.random.RandomState(self.dataset_seed)
-        train_dataset_mix_ds = []
-        custom_mix_ds = []
-        for mix_ds in self.train_dataset_mix_ds:
-            if os.path.exists(mix_ds):
-                custom_mix_ds.append(mix_ds)
-            else:
-                train_dataset_mix_ds.append(mix_ds)
-
-        if len(custom_mix_ds) > 0:
-            dataset_name = '_custom_mixture'
-            _register_local_dataset(dataset_name, custom_mix_ds, [])
-            train_dataset_mix_ds.append(dataset_name)
-        mix_dataset_sample = int(len(train_dataset) * self.train_dataset_mix_ratio)
-        logger.info(f'train_dataset_mix_ds: {train_dataset_mix_ds}')
-        logger.info(f'len(train_dataset): {len(train_dataset)}, mix_dataset_sample: {mix_dataset_sample}')
-        mixed_dataset = get_dataset(
-            train_dataset_mix_ds, 0.0, random_state, check_dataset_strategy=self.check_dataset_strategy)[0]
-        if len(mixed_dataset) < mix_dataset_sample:
-            logger.warn(f'The length of dataset used for mixin: {train_dataset_mix_ds} are '
-                        'lesser than the ratio required by the `train_dataset_mix_ratio` '
-                        f'argument: {self.train_dataset_mix_ratio}. '
-                        f'the actual ratio is: {len(mixed_dataset) / len(train_dataset):.6}.')
-        else:
-            train_idxs = random_state.permutation(mix_dataset_sample)
-            mixed_dataset = mixed_dataset.select(train_idxs)
-        return concatenate_datasets([train_dataset, mixed_dataset])
+    custom_train_dataset_path: List[str] = field(default_factory=list)
+    custom_val_dataset_path: List[str] = field(default_factory=list)
 
     def prepare_push_ms_hub(self) -> None:
         if not self.push_to_hub:
             return
         if self.hub_model_id is None:
             self.hub_model_id = f'{self.model_type}-{self.sft_type}'
             logger.info(f'Setting hub_model_id: {self.hub_model_id}')
@@ -519,67 +667,64 @@
         if 'LN' in modules_to_save:
             modules_to_save.remove('LN')
             self.lora_m2s_use_ln = True
         return modules_to_save
 
     def __post_init__(self) -> None:
         self.handle_compatibility()
+        self._register_self_cognition()
+        if self.val_dataset is not None:
+            self.dataset_test_ratio = 0.0 if self.val_dataset is not None else self.dataset_test_ratio
+            logger.info('Using val_dataset, ignoring dataset_test_ratio')
+        self._handle_dataset_sample()
         if is_pai_training_job():
             self._handle_pai_compat()
-        ds_config_folder = os.path.join(__file__, '..', '..', 'ds_config')
+        ds_config_folder = os.path.abspath(os.path.join(__file__, '..', '..', 'ds_config'))
         deepspeed_mapping = {
             'default-zero2': 'zero2.json',
             'default-zero3': 'zero3.json',
             'zero3-offload': 'zero3_offload.json'
         }
         for ds_name, ds_config in deepspeed_mapping.items():
             if self.deepspeed == ds_name:
-                self.deepspeed = os.path.abspath(os.path.join(ds_config_folder, ds_config))
+                self.deepspeed = os.path.join(ds_config_folder, ds_config)
                 break
 
         self.handle_path()
+        self.handle_custom_register()
+        self.handle_custom_dataset_info()
         self.set_model_type()
-        if isinstance(self.dataset, str):
-            self.dataset = [self.dataset]
-        if isinstance(self.train_dataset_mix_ds, str):
-            self.train_dataset_mix_ds = [self.train_dataset_mix_ds]
-        self.register_custom_dataset()
         self.check_flash_attn()
         self.handle_generation_config()
 
         self.lora_use_embedding = False
         self.lora_use_all = False
         self.lora_m2s_use_embedding = False
         self.lora_m2s_use_ln = False
         if self.sft_type == 'ia3':
             self.ia3_feedforward_modules = self._prepare_target_modules(self.ia3_feedforward_modules)
             self.ia3_target_modules = self._prepare_target_modules(self.ia3_target_modules)
             self.ia3_modules_to_save = self._prepare_modules_to_save(self.ia3_modules_to_save)
+        elif self.sft_type == 'vera':
+            self.vera_target_modules = self._prepare_target_modules(self.vera_target_modules)
+            self.vera_modules_to_save = self._prepare_modules_to_save(self.vera_modules_to_save)
+        elif self.sft_type == 'boft':
+            self.boft_target_modules = self._prepare_target_modules(self.boft_target_modules)
+            self.boft_modules_to_save = self._prepare_modules_to_save(self.boft_modules_to_save)
         else:
             self.lora_target_modules = self._prepare_target_modules(self.lora_target_modules)
             self.lora_modules_to_save = self._prepare_modules_to_save(self.lora_modules_to_save)
+        if self.use_self_cognition and self.sft_type == 'lora' and not self.lora_use_all:
+            logger.warning('Due to knowledge editing involved, it is recommended to add LoRA on MLP. '
+                           'For example: `--lora_target_modules ALL`. '
+                           'If you have already added LoRA on MLP, please ignore this warning.')
+
         if self.sft_type in {'adalora', 'ia3'} and self.lora_use_embedding:
             raise ValueError('`adalora` and `ia3` do not support setting embedding as target_modules.')
 
-        if self.self_cognition_sample > 0:
-            if self.model_name is None or self.model_author is None:
-                raise ValueError('Please enter self.model_name self.model_author. '
-                                 'For example: `--model_name 小黄 "Xiao Huang" --model_author 魔搭 ModelScope`. '
-                                 'Representing the model name and model author in Chinese and English.')
-            for k in ['model_name', 'model_author']:
-                v = getattr(self, k)
-                if len(v) == 1:
-                    v = v[0]
-                if isinstance(v, str):
-                    setattr(self, k, [v, v])
-            if self.sft_type == 'lora' and not self.lora_use_all:
-                logger.warning('Due to knowledge editing involved, it is recommended to add LoRA on MLP. '
-                               'For example: `--lora_target_modules ALL`. '
-                               'If you have already added LoRA on MLP, please ignore this warning.')
-
         self.torch_dtype, self.fp16, self.bf16 = self.select_dtype()
         world_size = 1
         if is_dist():
             rank, local_rank, world_size, _ = get_dist_setting()
             if is_torch_npu_available():
                 torch.npu.set_device(local_rank)
             else:
@@ -615,20 +760,31 @@
                 self.learning_rate = 1e-5
             if self.save_only_model is None:
                 self.save_only_model = True
         else:
             raise ValueError(f'sft_type: {self.sft_type}')
 
         self.prepare_template()
-        if len(self.dataset) == 0 and (len(self.custom_train_dataset_path) == 0
-                                       and len(self.custom_val_dataset_path) == 0 and self.self_cognition_sample == 0):
+        if len(self.dataset) == 0:
             raise ValueError(f'self.dataset: {self.dataset}, Please input the training dataset.')
 
         if self.save_steps is None:
             self.save_steps = self.eval_steps
+
+        # compatibility
+        if self.quantization_bit > 0 and self.quant_method is None:
+            if self.quantization_bit == 4 or self.quantization_bit == 8:
+                logger.info('Since you have specified quantization_bit as greater than 0 '
+                            "and have not designated a quant_method, quant_method will be set to 'bnb'.")
+                self.quant_method = 'bnb'
+            else:
+                self.quant_method = 'hqq'
+                logger.info('Since you have specified quantization_bit as greater than 0 '
+                            "and have not designated a quant_method, quant_method will be set to 'hqq'.")
+
         self.bnb_4bit_compute_dtype, self.load_in_4bit, self.load_in_8bit = self.select_bnb()
 
         if self.neftune_backend is None:
             self.neftune_backend = 'swift' if version.parse(transformers.__version__) < version.parse('4.35') \
                 else 'transformers'
 
         self.prepare_push_ms_hub()
@@ -792,40 +948,45 @@
 class InferArguments(ArgumentsBase):
     # You can specify the model by either using the model_type or model_id_or_path.
     model_type: Optional[str] = field(
         default=None, metadata={'help': f'model_type choices: {list(MODEL_MAPPING.keys())}'})
     model_id_or_path: Optional[str] = None
     model_revision: Optional[str] = None
 
-    sft_type: Literal['lora', 'longlora', 'full', 'adalora', 'ia3', 'llamapro'] = 'lora'
+    sft_type: Literal['lora', 'longlora', 'full', 'adalora', 'ia3', 'llamapro', 'vera', 'boft'] = 'lora'
     template_type: str = field(
         default='AUTO', metadata={'help': f"template_type choices: {list(TEMPLATE_MAPPING.keys()) + ['AUTO']}"})
     infer_backend: Literal['AUTO', 'vllm', 'pt'] = 'AUTO'
     ckpt_dir: Optional[str] = field(default=None, metadata={'help': '/path/to/your/vx-xxx/checkpoint-xxx'})
     load_args_from_ckpt_dir: bool = True
     load_dataset_config: bool = False
     eval_human: Optional[bool] = None
 
     seed: int = 42
     dtype: Literal['bf16', 'fp16', 'fp32', 'AUTO'] = 'AUTO'
 
     dataset: List[str] = field(
         default_factory=list, metadata={'help': f'dataset choices: {list(DATASET_MAPPING.keys())}'})
+    val_dataset: List[str] = field(default=None, metadata={'help': f'dataset choices: {list(DATASET_MAPPING.keys())}'})
     dataset_seed: int = 42
     dataset_test_ratio: float = 0.01
-    val_dataset_sample: int = 10  # -1: all dataset
+    show_dataset_sample: int = 10
     save_result: bool = True
     system: Optional[str] = None
     max_length: int = -1  # -1: no limit
     truncation_strategy: Literal['delete', 'truncation_left'] = 'delete'
     check_dataset_strategy: Literal['none', 'discard', 'error', 'warning'] = 'none'
-    custom_train_dataset_path: List[str] = field(default_factory=list)
-    custom_val_dataset_path: List[str] = field(default_factory=list)
-
-    quantization_bit: Literal[0, 4, 8] = 0
+    # Chinese name and English name
+    model_name: List[str] = field(default_factory=lambda: [None, None], metadata={'help': "e.g. ['小黄', 'Xiao Huang']"})
+    model_author: List[str] = field(
+        default_factory=lambda: [None, None], metadata={'help': "e.g. ['魔搭', 'ModelScope']"})
+    quant_method: Literal['bnb', 'hqq', 'eetq'] = None
+    quantization_bit: Literal[0, 1, 2, 3, 4, 8] = 0  # hqq: 1,2,3,4,8. bnb: 4,8
+    hqq_axis: Literal[0, 1] = 0
+    hqq_dynamic_config_path: Optional[str] = None
     bnb_4bit_comp_dtype: Literal['fp16', 'bf16', 'fp32', 'AUTO'] = 'AUTO'
     bnb_4bit_quant_type: Literal['fp4', 'nf4'] = 'nf4'
     bnb_4bit_use_double_quant: bool = True
     bnb_4bit_quant_storage: Optional[str] = None
 
     max_new_tokens: int = 2048
     do_sample: bool = True
@@ -841,80 +1002,105 @@
     ignore_args_error: bool = False  # True: notebook compatibility
     stream: bool = True
     merge_lora: bool = False
     merge_device_map: Optional[str] = None
     save_safetensors: bool = True
     overwrite_generation_config: Optional[bool] = None
     verbose: Optional[bool] = None
+    local_repo_path: Optional[str] = None
+    custom_register_path: Optional[str] = None  # .py
+    custom_dataset_info: Optional[str] = None  # .json
+    device_map_config_path: Optional[str] = None
+
     # vllm
     gpu_memory_utilization: float = 0.9
     tensor_parallel_size: int = 1
     max_model_len: Optional[int] = None
     vllm_enable_lora: bool = False
     vllm_max_lora_rank: int = 16
-    vllm_lora_modules: List[str] = field(default_factory=list)
+    lora_modules: List[str] = field(default_factory=list)
+
     # compatibility. (Deprecated)
-    show_dataset_sample: int = 10
+    self_cognition_sample: int = 0
+    train_dataset_sample: int = -1  # Used for splitting the validation set.
+    val_dataset_sample: Optional[int] = None  # -1: all dataset
     safe_serialization: Optional[bool] = None
     model_cache_dir: Optional[str] = None
     merge_lora_and_save: Optional[bool] = None
+    custom_train_dataset_path: List[str] = field(default_factory=list)
+    custom_val_dataset_path: List[str] = field(default_factory=list)
+    vllm_lora_modules: List[str] = None
 
     def __post_init__(self) -> None:
         if self.ckpt_dir is not None and not self.check_ckpt_dir_correct(self.ckpt_dir):
             logger.warning(f'The checkpoint dir {self.ckpt_dir} passed in is invalid, please make sure'
                            'the dir contains a `configuration.json` file.')
         self.handle_compatibility()
+        self._register_self_cognition()
+        if self.val_dataset is not None:
+            self.dataset_test_ratio = 0.0 if self.val_dataset is not None else self.dataset_test_ratio
+            logger.info('Using val_dataset, ignoring dataset_test_ratio')
         self.handle_path()
         logger.info(f'ckpt_dir: {self.ckpt_dir}')
         if self.ckpt_dir is None and self.load_args_from_ckpt_dir:
             self.load_args_from_ckpt_dir = False
             logger.info('Due to `ckpt_dir` being `None`, `load_args_from_ckpt_dir` is set to `False`.')
         if self.load_args_from_ckpt_dir:
             self.load_from_ckpt_dir()
         else:
             assert self.load_dataset_config is False, 'You need to first set `--load_args_from_ckpt_dir true`.'
+        self.handle_compatibility()
+        self._handle_dataset_sample()
+        self.handle_custom_register()
+        self.handle_custom_dataset_info()
         self.set_model_type()
-        if isinstance(self.dataset, str):
-            self.dataset = [self.dataset]
-        self.register_custom_dataset()
         self.check_flash_attn()
         self.handle_generation_config()
 
         self.torch_dtype, _, _ = self.select_dtype()
         self.prepare_template()
-        has_dataset = (
-            len(self.dataset) > 0 or len(self.custom_train_dataset_path) > 0 or len(self.custom_val_dataset_path) > 0)
         if self.eval_human is None:
-            if not has_dataset:
+            if not len(self.dataset) > 0:
                 self.eval_human = True
             else:
                 self.eval_human = False
             logger.info(f'Setting self.eval_human: {self.eval_human}')
-        elif self.eval_human is False and not has_dataset:
+        elif self.eval_human is False and not len(self.dataset) > 0:
             raise ValueError('Please provide the dataset or set `--load_dataset_config true`.')
 
+        # compatibility
+        if self.quantization_bit > 0 and self.quant_method is None:
+            if self.quantization_bit == 4 or self.quantization_bit == 8:
+                logger.info('Since you have specified quantization_bit as greater than 0 '
+                            "and have not designated a quant_method, quant_method will be set to 'bnb'.")
+                self.quant_method = 'bnb'
+            else:
+                self.quant_method = 'hqq'
+                logger.info('Since you have specified quantization_bit as greater than 0 '
+                            "and have not designated a quant_method, quant_method will be set to 'hqq'.")
+
         self.bnb_4bit_compute_dtype, self.load_in_4bit, self.load_in_8bit = self.select_bnb()
 
         if self.max_length == -1:
             self.max_length = None
         if self.overwrite_generation_config is None:
             if self.ckpt_dir is None:
                 self.overwrite_generation_config = False
             else:
                 self.overwrite_generation_config = True
             logger.info(f'Setting overwrite_generation_config: {self.overwrite_generation_config}')
         if self.ckpt_dir is None:
             self.sft_type = 'full'
 
-        self.prepare_vllm()
+        self.handle_infer_backend()
 
-    def prepare_vllm(self):
+    def handle_infer_backend(self):
         model_info = MODEL_MAPPING[self.model_type]
         support_vllm = model_info.get('support_vllm', False)
-        self.vllm_lora_request_list = None
+        self.lora_request_list = None
         if self.infer_backend == 'AUTO':
             self.infer_backend = 'pt'
             if is_vllm_available() and support_vllm:
                 if ((self.sft_type == 'full' or self.sft_type == 'lora' and self.merge_lora)
                         and self.quantization_bit == 0):
                     self.infer_backend = 'vllm'
                 if self.vllm_enable_lora:
@@ -923,18 +1109,21 @@
             require_version('vllm')
             assert self.quantization_bit == 0, 'VLLM does not support bnb.'
             if not support_vllm:
                 logger.warning(f'vllm not support `{self.model_type}`')
             if self.sft_type == 'lora' and not self.vllm_enable_lora:
                 assert self.merge_lora is True, ('To use VLLM, you need to provide the complete weight parameters. '
                                                  'Please set `--merge_lora true`.')
-            if self.vllm_enable_lora:
-                self.vllm_lora_modules.append(f'default-lora={self.ckpt_dir}')
-                self.vllm_lora_request_list = _parse_vllm_lora_modules(self.vllm_lora_modules)
-                logger.info(f'args.vllm_lora_request_list: {self.vllm_lora_request_list}')
+        if (self.infer_backend == 'vllm' and self.vllm_enable_lora
+                or self.infer_backend == 'pt' and isinstance(self, DeployArguments) and self.sft_type == 'lora'):
+            assert self.ckpt_dir is not None
+            self.lora_modules.append(f'default-lora={self.ckpt_dir}')
+            self.lora_request_list = _parse_lora_modules(self.lora_modules, True)
+            logger.info(f'args.lora_request_list: {self.lora_request_list}')
+
         template_info = TEMPLATE_MAPPING[self.template_type]
         if self.num_beams != 1:
             self.stream = False
             logger.info('Setting self.stream: False')
         self.infer_media_type = template_info.get('infer_media_type', 'none')
         if self.merge_device_map is None:
             self.merge_device_map = 'cpu'
@@ -948,25 +1137,29 @@
             sft_args = json.load(f)
         imported_keys = [
             'model_type', 'model_revision', 'sft_type', 'template_type', 'system', 'quantization_bit',
             'bnb_4bit_comp_dtype', 'bnb_4bit_quant_type', 'bnb_4bit_use_double_quant'
         ]
         if self.load_dataset_config:
             imported_keys += [
-                'dataset', 'dataset_seed', 'dataset_test_ratio', 'check_dataset_strategy', 'custom_train_dataset_path',
-                'custom_val_dataset_path'
+                'dataset', 'val_dataset', 'dataset_seed', 'dataset_test_ratio', 'check_dataset_strategy',
+                'self_cognition_sample', 'model_name', 'model_author', 'train_dataset_sample', 'val_dataset_sample'
             ]
         for key in imported_keys:
-            if (key in {'dataset', 'custom_train_dataset_path', 'custom_val_dataset_path'}
-                    and len(getattr(self, key)) > 0):
+            value = getattr(self, key)
+            if key == 'dataset' and len(value) > 0:
+                continue
+            if key in {'dataset_test_ratio', 'system'} and value is not None:
                 continue
             setattr(self, key, sft_args.get(key))
 
-        if self.model_id_or_path is None:
-            self.model_id_or_path = sft_args.get('model_id_or_path')
+        for k in ['model_id_or_path', 'custom_register_path', 'custom_dataset_info']:
+            if getattr(self, k) is None:
+                setattr(self, k, sft_args.get(k))
+
         if self.dtype == 'AUTO':
             self.dtype = sft_args.get('dtype')
 
     @staticmethod
     def check_ckpt_dir_correct(ckpt_dir) -> bool:
         """Check the checkpoint dir is correct, which means it must contains a `configuration.json` file.
         Args:
@@ -977,17 +1170,20 @@
         if not os.path.exists(ckpt_dir):
             return False
         return os.path.isfile(os.path.join(ckpt_dir, 'configuration.json'))
 
 
 @dataclass
 class AppUIArguments(InferArguments):
-    server_name: str = '127.0.0.1'
-    server_port: int = 7860
+    host: str = '127.0.0.1'
+    port: int = 7860
     share: bool = False
+    # compatibility. (Deprecated)
+    server_name: Optional[str] = None
+    server_port: Optional[int] = None
 
 
 @dataclass
 class DeployArguments(InferArguments):
     host: str = '127.0.0.1'
     port: int = 8000
     ssl_keyfile: Optional[str] = None
@@ -1018,61 +1214,78 @@
 
     eval_limit: Optional[int] = None
 
     custom_eval_config: Optional[str] = None
 
     eval_use_cache: Optional[bool] = False
 
+    def select_dtype(self):
+        if self.eval_url is None:
+            return super().select_dtype()
+        return None, None, None
+
     def set_model_type(self) -> None:
         if self.eval_url is None:
             super().set_model_type()
 
     def check_flash_attn(self) -> None:
         if self.eval_url is None:
             super().check_flash_attn()
 
     def prepare_template(self) -> None:
         if self.eval_url is None:
             super().prepare_template()
 
-    def prepare_vllm(self) -> None:
+    def handle_infer_backend(self) -> None:
         if self.eval_url is None:
-            super().prepare_vllm()
+            super().handle_infer_backend()
 
 
 @dataclass
 class ExportArguments(InferArguments):
     to_peft_format: bool = False
     # The parameter has been defined in InferArguments.
     # merge_lora: bool = False
 
     # awq: 4; gptq: 2, 3, 4, 8
     quant_bits: int = 0  # e.g. 4
     quant_method: Literal['awq', 'gptq'] = 'awq'
     quant_n_samples: int = 256
     quant_seqlen: int = 2048
     quant_device_map: str = 'cpu'  # e.g. 'cpu', 'auto'
+    quant_output_dir: Optional[str] = None
 
     # push to ms hub
     push_to_hub: bool = False
     # 'user_name/repo_name' or 'repo_name'
     hub_model_id: Optional[str] = None
     # None: use env var `MODELSCOPE_API_TOKEN`
     hub_token: Optional[str] = field(
         default=None, metadata={'help': 'SDK token can be found in https://modelscope.cn/my/myaccesstoken'})
     hub_private_repo: bool = False
     commit_message: str = 'update files'
 
     def __post_init__(self):
         if self.merge_device_map is None:
             self.merge_device_map = 'cpu' if self.quant_bits != 0 else 'auto'
+        if self.quant_bits > 0 and self.dtype == 'AUTO':
+            self.dtype = 'fp16'
+            logger.info(f'Setting args.dtype: {args.dtype}')
         super().__post_init__()
-        if len(self.dataset) == 0:
-            self.dataset = ['alpaca-zh', 'alpaca-en']
+        if len(self.dataset) == 0 and self.quant_bits > 0:
+            self.dataset = ['alpaca-zh#10000', 'alpaca-en#10000']
             logger.info(f'Setting args.dataset: {self.dataset}')
+        if self.quant_output_dir is None:
+            if self.ckpt_dir is None:
+                self.quant_output_dir = f'{self.model_type}-{self.quant_method}-int{self.quant_bits}'
+            else:
+                ckpt_dir, ckpt_name = os.path.split(self.ckpt_dir)
+                self.quant_output_dir = os.path.join(ckpt_dir, f'{ckpt_name}-{self.quant_method}-int{self.quant_bits}')
+            logger.info(f'Setting args.quant_output_dir: {self.quant_output_dir}')
+        assert not os.path.exists(self.quant_output_dir), f'args.quant_output_dir: {self.quant_output_dir}'
 
 
 @dataclass
 class DPOArguments(SftArguments):
 
     ref_model_type: Optional[str] = field(
         default=None, metadata={'help': f'model_type choices: {list(MODEL_MAPPING.keys())}'})
@@ -1083,14 +1296,20 @@
     beta: float = 0.1
     label_smoothing: float = 0.0
     loss_type: Literal['sigmoid', 'hinge', 'ipo', 'kto_pair'] = 'sigmoid'
     sft_beta: float = 0.1
 
 
 @dataclass
+class ORPOArguments(SftArguments):
+    max_prompt_length: int = 1024
+    beta: float = 0.1
+
+
+@dataclass
 class RomeArguments(InferArguments):
     rome_request_file: str = field(
         default=None, metadata={'help': 'The rome request file, please check the documentation '
                                 'to get the format'})
 
     def __post_init__(self) -> None:
         self.handle_compatibility()
@@ -1106,51 +1325,41 @@
         if self.max_length == -1:
             self.max_length = None
 
 
 dtype_mapping_reversed = {v: k for k, v in dtype_mapping.items()}
 
 
-def _check_path(k: str, value: Union[str, List[str]],
-                check_exist_path_set: Optional[Set[str]]) -> Union[str, List[str]]:
-    if isinstance(value, str):
-        value = os.path.expanduser(value)
-        value = os.path.abspath(value)
-        if k in check_exist_path_set and not os.path.exists(value):
-            raise FileNotFoundError(f"`{k}`: '{value}'")
-    elif isinstance(value, list):
-        res = []
-        for v in value:
-            res.append(_check_path(k, v, check_exist_path_set))
-        value = res
-    return value
-
-
-def _register_local_dataset(dataset_name: str, train_dataset_path: List[str], val_dataset_path: List[str]) -> None:
-    register_dataset(
-        dataset_name, '_', train_dataset_path, val_dataset_path, get_function=get_custom_dataset, exists_ok=True)
-
-
 def swift_to_peft_format(lora_checkpoint_path: str) -> str:
     if 'default' in os.listdir(lora_checkpoint_path):  # swift_backend
         new_lora_checkpoint_path = f'{lora_checkpoint_path}-peft'
         Swift.save_to_peft_format(lora_checkpoint_path, new_lora_checkpoint_path)
         lora_checkpoint_path = new_lora_checkpoint_path
         logger.info('Converting the swift format checkpoint to peft format, '
                     f"and saving it to: '{new_lora_checkpoint_path}'")
     else:
         logger.info('The format of the checkpoint is already in peft format.')
     return lora_checkpoint_path
 
 
-def _parse_vllm_lora_modules(vllm_lora_modules: List[str]) -> List['LoRARequest']:
-    try:
-        from .vllm_utils import LoRARequest
-    except ImportError:
-        logger.warning('The current version of VLLM does not support `enable_lora`. Please upgrade VLLM.')
-        raise
+def _parse_lora_modules(lora_modules: List[str], use_vllm: bool) -> List['LoRARequest']:
+    VllmLoRARequest = None
+    if use_vllm:
+        try:
+            from .vllm_utils import LoRARequest as VllmLoRARequest
+        except ImportError:
+            logger.warning('The current version of VLLM does not support `enable_lora`. Please upgrade VLLM.')
+            raise
+
+    @dataclass
+    class PtLoRARequest:
+        lora_name: str
+        lora_int_id: int
+        lora_local_path: str
+
+    LoRARequest = VllmLoRARequest if use_vllm else PtLoRARequest
     lora_request_list = []
-    for i, vllm_lora_module in enumerate(vllm_lora_modules):
-        lora_name, lora_local_path = vllm_lora_module.split('=')
+    for i, lora_module in enumerate(lora_modules):
+        lora_name, lora_local_path = lora_module.split('=')
         lora_local_path = swift_to_peft_format(lora_local_path)
         lora_request_list.append(LoRARequest(lora_name, i + 1, lora_local_path))
     return lora_request_list
```

### Comparing `ms-swift-2.0.4/swift/llm/utils/client_utils.py` & `ms-swift-2.0.5/swift/llm/utils/client_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,24 +32,25 @@
     query: str,
     history: Optional[History] = None,
     system: Optional[str] = None,
     *,
     request_config: Optional[XRequestConfig] = None,
     host: str = '127.0.0.1',
     port: str = '8000',
+    adapter_name: str = None,
     is_chat_request: Optional[bool] = None,
 ) -> Union[ChatCompletionResponse, CompletionResponse, Iterator[ChatCompletionStreamResponse],
            Iterator[CompletionStreamResponse]]:
     if request_config is None:
         request_config = XRequestConfig()
     if is_chat_request is None:
         template_type = get_default_template_type(model_type)
         is_chat_request = 'generation' not in template_type
     data = {k: v for k, v in request_config.__dict__.items() if not k.startswith('__')}
-    data['model'] = model_type
+    data['model'] = adapter_name or model_type
     if is_chat_request:
         data['messages'] = history_to_messages(history, query, system)
         url = f'http://{host}:{port}/v1/chat/completions'
     else:
         assert system is None and history is None, (
             'The chat template for text generation does not support system and history.')
         data['prompt'] = query
```

### Comparing `ms-swift-2.0.4/swift/llm/utils/dataset.py` & `ms-swift-2.0.5/swift/llm/utils/dataset.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 import ast
+import itertools
 import os
 import re
+from copy import deepcopy
 from functools import partial
 from typing import Any, Callable, Dict, List, Literal, Optional, Tuple, Union
 
 import json
 import numpy as np
 import pandas as pd
 from datasets import Dataset as HfDataset
-from datasets import concatenate_datasets, load_dataset
+from datasets import concatenate_datasets
+from datasets import load_dataset as load_hf_dataset
 from numpy.random import RandomState
 from pandas import DataFrame
 from tqdm.auto import tqdm
 from transformers.utils import strtobool
 
 from swift.utils import get_logger, get_seed, is_dist, is_local_master, read_from_jsonl, transform_jsonl_to_df
 from .preprocess import (AlpacaPreprocessor, ClsPreprocessor, ComposePreprocessor, ConversationsPreprocessor,
@@ -37,56 +40,50 @@
 
 logger = get_logger()
 
 
 class DatasetName:
     # general
     ms_bench = 'ms-bench'  # used for mixed training
-    ms_bench_mini = 'ms-bench-mini'
     alpaca_en = 'alpaca-en'
     alpaca_zh = 'alpaca-zh'
-    multi_alpaca_all = 'multi-alpaca-all'
-    instinwild_en = 'instinwild-en'
-    instinwild_zh = 'instinwild-zh'
+    multi_alpaca = 'multi-alpaca'
+    instinwild = 'instinwild'
     cot_en = 'cot-en'
     cot_zh = 'cot-zh'
-    firefly_all_zh = 'firefly-all-zh'
     instruct_en = 'instruct-en'
+    firefly_zh = 'firefly-zh'
     gpt4all_en = 'gpt4all-en'
-    sharegpt_en = 'sharegpt-en'
-    sharegpt_zh = 'sharegpt-zh'
+    sharegpt = 'sharegpt'
     tulu_v2_sft_mixture = 'tulu-v2-sft-mixture'
     wikipedia_zh = 'wikipedia-zh'
     open_orca = 'open-orca'
-    open_orca_gpt4 = 'open-orca-gpt4'
     sharegpt_gpt4 = 'sharegpt-gpt4'
-    sharegpt_gpt4_mini = 'sharegpt-gpt4-mini'
-    deepctrl_sft_zh = 'deepctrl-sft-zh'
-    deepctrl_sft_en = 'deepctrl-sft-en'
+    deepctrl_sft = 'deepctrl-sft'
+    coig_cqia = 'coig-cqia'
+    ruozhiba = 'ruozhiba'
+    long_alpaca_12k = 'long-alpaca-12k'
+
     # agent
     ms_agent = 'ms-agent'
-    ms_agent_for_agentfabric_default = 'ms-agent-for-agentfabric-default'
-    ms_agent_for_agentfabric_addition = 'ms-agent-for-agentfabric-addition'
+    ms_agent_for_agentfabric = 'ms-agent-for-agentfabric'
     ms_agent_multirole = 'ms-agent-multirole'
+    toolbench_for_alpha_umi = 'toolbench-for-alpha-umi'
     damo_agent_zh = 'damo-agent-zh'
-    damo_agent_mini_zh = 'damo-agent-mini-zh'
+    damo_agent_zh_mini = 'damo-agent-zh-mini'
     agent_instruct_all_en = 'agent-instruct-all-en'
-    toolbench_for_alpha_umi_backbone = 'toolbench-for-alpha-umi-backbone'
-    toolbench_for_alpha_umi_caller = 'toolbench-for-alpha-umi-caller'
-    toolbench_for_alpha_umi_planner = 'toolbench-for-alpha-umi-planner'
-    toolbench_for_alpha_umi_summarizer = 'toolbench-for-alpha-umi-summarizer'
+
     # coding
     code_alpaca_en = 'code-alpaca-en'
     leetcode_python_en = 'leetcode-python-en'
     codefuse_python_en = 'codefuse-python-en'
     codefuse_evol_instruction_zh = 'codefuse-evol-instruction-zh'
     # medical
     medical_en = 'medical-en'
     medical_zh = 'medical-zh'
-    medical_mini_zh = 'medical-mini-zh'
     disc_med_sft_zh = 'disc-med-sft-zh'
     # law
     lawyer_llama_zh = 'lawyer-llama-zh'
     tigerbot_law_zh = 'tigerbot-law-zh'
     disc_law_sft_zh = 'disc-law-sft-zh'
     # math
     blossom_math_zh = 'blossom-math-zh'
@@ -96,113 +93,89 @@
     text2sql_en = 'text2sql-en'
     sql_create_context_en = 'sql-create-context-en'
     # text-generation
     advertise_gen_zh = 'advertise-gen-zh'
     dureader_robust_zh = 'dureader-robust-zh'
     # classification
     cmnli_zh = 'cmnli-zh'
-    cmnli_mini_zh = 'cmnli-mini-zh'
     jd_sentiment_zh = 'jd-sentiment-zh'
     hc3_zh = 'hc3-zh'
     hc3_en = 'hc3-en'
     # other
     finance_en = 'finance-en'
     poetry_zh = 'poetry-zh'
     webnovel_zh = 'webnovel-zh'
     generated_chat_zh = 'generated-chat-zh'
+    self_cognition = 'self-cognition'
+
     # example dataset for specific model
     cls_fudan_news_zh = 'cls-fudan-news-zh'  # seqgpt-560m
     ner_java_zh = 'ner-jave-zh'  # seqgpt-560m
-    long_alpaca_12k = 'long-alpaca-12k'
 
     # multi-modal
-    # for qwen-vl
+    # <img></img>
     coco_en = 'coco-en'
-    coco_mini_en = 'coco-mini-en'
-    # for yi-vl, cogagnet
-    coco_mini_en_2 = 'coco-mini-en-2'
+    coco_en_mini = 'coco-en-mini'
+    # images
+    coco_en_2 = 'coco-en-2'
+    coco_en_2_mini = 'coco-en-2-mini'
     capcha_images = 'capcha-images'
     # for qwen-audio
     aishell1_zh = 'aishell1-zh'
-    aishell1_mini_zh = 'aishell1-mini-zh'
+    aishell1_zh_mini = 'aishell1-zh-mini'
 
     # dpo/hfrl dataset
-    hh_rlhf_harmless_base = 'hh-rlhf-harmless-base'
-    hh_rlhf_helpful_base = 'hh-rlhf-helpful-base'
-    hh_rlhf_helpful_online = 'hh-rlhf-helpful-online'
-    hh_rlhf_helpful_rejection_sampled = 'hh-rlhf-helpful-rejection-sampled'
-    hh_rlhf_red_team_attempts = 'hh-rlhf-red-team-attempts'
+    hh_rlhf = 'hh-rlhf'
     hh_rlhf_cn = 'hh-rlhf-cn'
-    hh_rlhf_cn_harmless_base_cn = 'hh-rlhf-cn-harmless-base-cn'
-    hh_rlhf_cn_helpful_base_cn = 'hh-rlhf-cn-helpful-base-cn'
-    hh_rlhf_cn_harmless_base_en = 'hh-rlhf-cn-harmless-base-en'
-    hh_rlhf_cn_helpful_base_en = 'hh-rlhf-cn-helpful-base-en'
     stack_exchange_paired = 'stack-exchange-paired'
+    shareai_llama3_dpo_zh_en_emoji = 'shareai-llama3-dpo-zh-en-emoji'
 
     # for awq
     pileval = 'pileval'
 
-    # COIG-CQIA
-    coig_cqia_chinese_traditional = 'coig-cqia-chinese-traditional'
-    coig_cqia_coig_pc = 'coig-cqia-coig-pc'
-    coig_cqia_exam = 'coig-cqia-exam'
-    coig_cqia_finance = 'coig-cqia-finance'
-    coig_cqia_douban = 'coig-cqia-douban'
-    coig_cqia_human_value = 'coig-cqia-human-value'
-    coig_cqia_logi_qa = 'coig-cqia-logi-qa'
-    coig_cqia_ruozhiba = 'coig-cqia-ruozhiba'
-    coig_cqia_segmentfault = 'coig-cqia-segmentfault'
-    coig_cqia_wiki = 'coig-cqia-wiki'
-    coig_cqia_wikihow = 'coig-cqia-wikihow'
-    coig_cqia_xhs = 'coig-cqia-xhs'
-    coig_cqia_zhihu = 'coig-cqia-zhihu'
-
-    # ruozhiba
-    ruozhiba_post_annual = 'ruozhiba-post-annual'
-    ruozhiba_title_good = 'ruozhiba-title-good'
-    ruozhiba_title_norm = 'ruozhiba-title-norm'
-
     @classmethod
     def get_dataset_name_list(cls) -> List[str]:
         res = []
         for k in cls.__dict__.keys():
             if k.startswith('__') or k == 'get_dataset_name_list':
                 continue
             res.append(cls.__dict__[k])
         return res
 
 
 def register_dataset(dataset_name: str,
-                     dataset_id_or_path: str,
-                     train_subset_split_list: Optional[List[SubsetSplit]] = None,
-                     val_subset_split_list: Optional[List[SubsetSplit]] = None,
+                     dataset_id_or_path: Optional[str] = None,
+                     subsets: Optional[List[str]] = None,
                      preprocess_func: Optional[PreprocessFunc] = None,
                      get_function: Optional[GetDatasetFunction] = None,
                      *,
+                     split: Optional[List[str]] = None,
                      hf_dataset_id: Optional[str] = None,
                      function_kwargs: Optional[Dict[str, Any]] = None,
-                     exists_ok: bool = False,
+                     exist_ok: bool = False,
+                     is_local: bool = False,
                      **kwargs) -> Optional[Callable[[GetDatasetFunction], GetDatasetFunction]]:
     if preprocess_func is None:
         preprocess_func = SmartPreprocessor()
-    if not exists_ok and dataset_name in DATASET_MAPPING:
+    if not exist_ok and dataset_name in DATASET_MAPPING:
         raise ValueError(f'The `{dataset_name}` has already been registered in the DATASET_MAPPING.')
-    if train_subset_split_list is None:
-        train_subset_split_list = []
-    if val_subset_split_list is None:
-        val_subset_split_list = []
+    if subsets is None:
+        subsets = []
+    if split is None:
+        split = ['train']
     if function_kwargs is None:
         function_kwargs = {}
 
     dataset_info = {
         'dataset_id_or_path': dataset_id_or_path,
-        'train_subset_split_list': train_subset_split_list,
-        'val_subset_split_list': val_subset_split_list,
+        'subsets': subsets,
         'preprocess_func': preprocess_func,
+        'split': split,
         'hf_dataset_id': hf_dataset_id,
+        'is_local': is_local,
         **kwargs
     }
     if get_function is not None:
         if len(function_kwargs) > 0:
             get_function = partial(get_function, **function_kwargs)
         dataset_info['get_function'] = get_function
         DATASET_MAPPING[dataset_name] = dataset_info
@@ -215,177 +188,176 @@
         dataset_info['get_function'] = get_function
         DATASET_MAPPING[dataset_name] = dataset_info
         return _old_get_function
 
     return _register_dataset
 
 
-def load_ms_dataset(dataset_id: str, subset_split_list: Optional[List[SubsetSplit]]) -> Optional[HfDataset]:
-    from modelscope import MsDataset
+def register_local_dataset(
+        dataset_name: str,
+        dataset_path: Optional[List[str]] = None,
+        # Convert relative path to absolute path
+        base_dir: Optional[str] = None,
+        **kwargs) -> None:
+    if dataset_path is None:
+        dataset_path = []
+    elif isinstance(dataset_path, str):
+        dataset_path = [dataset_path]
+    assert len(dataset_path) > 0
+    if base_dir is not None:
+        for i, path in enumerate(dataset_path):
+            if not os.path.isabs(path):
+                dataset_path[i] = os.path.join(base_dir, dataset_path[i])
+
+    register_dataset(
+        dataset_name, get_function=get_local_dataset, split=dataset_path, exist_ok=True, is_local=True, **kwargs)
+
+
+def register_dataset_info(dataset_name: str, d_info: Dict[str, Any], **kwargs) -> None:
+    if 'dataset_path' in d_info:
+        base_dir = kwargs.pop('base_dir', None)
+        register_local_dataset(dataset_name, d_info.pop('dataset_path', None), base_dir, **d_info)
+        return
+
+    assert 'dataset_id' in d_info or 'hf_dataset_id' in d_info
+    preprocess_func = None
+    if 'columns' in d_info:
+        preprocess_func = RenameColumnsPreprocessor(d_info['columns'])
+        d_info.pop('columns')
+    elif 'conversations' in d_info:
+        preprocess_func = ConversationsPreprocessor(**d_info['conversations'])
+        d_info.pop('conversations')
+    dataset_id = d_info.pop('dataset_id', None)
+    subsets = d_info.pop('subsets', None)
+    register_dataset(dataset_name, dataset_id, subsets, preprocess_func, get_dataset_from_repo, **d_info, exist_ok=True)
+
+
+def load_ms_dataset(dataset_id: str,
+                    subset_split_list: Optional[List[SubsetSplit]],
+                    use_hf: bool = False) -> Optional[HfDataset]:
+    if not use_hf:
+        from modelscope import MsDataset
+
     if subset_split_list is None or len(subset_split_list) == 0:
         return None
     dataset_list = []
     for subset_split in subset_split_list:
         if isinstance(subset_split, str):
             subset_split = ('default', subset_split)
         assert len(subset_split) == 2
         subset_name, split = subset_split
-        if is_dist() and not is_local_master():
-            force_redownload = False
+        if use_hf:
+            dataset = load_hf_dataset(dataset_id, name=subset_name, split=split)
         else:
-            force_redownload = strtobool(os.environ.get('FORCE_REDOWNLOAD', 'False'))
-        download_mode = 'force_redownload' if force_redownload else 'reuse_dataset_if_exists'
-        dataset = MsDataset.load(dataset_id, subset_name=subset_name, split=split, download_mode=download_mode)
-        if hasattr(dataset, 'to_hf_dataset'):
-            dataset = dataset.to_hf_dataset()
+            if is_dist() and not is_local_master():
+                force_redownload = False
+            else:
+                force_redownload = strtobool(os.environ.get('FORCE_REDOWNLOAD', 'False'))
+            download_mode = 'force_redownload' if force_redownload else 'reuse_dataset_if_exists'
+            dataset = MsDataset.load(dataset_id, subset_name=subset_name, split=split, download_mode=download_mode)
+            if hasattr(dataset, 'to_hf_dataset'):
+                dataset = dataset.to_hf_dataset()
         dataset_list.append(dataset)
     return concatenate_datasets(dataset_list)
 
 
-def load_hf_dataset(dataset_id: str, subset_split_list: Optional[List[SubsetSplit]]) -> Optional[HfDataset]:
-    if subset_split_list is None or len(subset_split_list) == 0:
-        return None
-    dataset_list = []
-    for subset_split in subset_split_list:
-        if isinstance(subset_split, str):
-            subset_split = (None, subset_split)
-        assert len(subset_split) == 2
-        subset_name, split = subset_split
-        dataset = load_dataset(dataset_id, name=subset_name, split=split)
-        dataset_list.append(dataset)
-    return concatenate_datasets(dataset_list)
+def sample_dataset(dataset: HfDataset, dataset_sample: int, random_state: Optional[RandomState] = None) -> HfDataset:
+    if dataset_sample in {None, -1, len(dataset)}:
+        return dataset
+    if random_state is None:
+        random_state = RandomState()
+    # Sample the part that exceeds the length of the dataset.
+    idx = random_state.permutation(len(dataset))[:dataset_sample]
+    dataset_sample -= len(idx)
+    if dataset_sample > 0:
+        idx2 = random_state.choice(len(dataset), dataset_sample)
+        idx = np.concatenate([idx, idx2], axis=0)
+    dataset = dataset.select(idx)
+    return dataset
 
 
-@register_dataset(
-    DatasetName.text2sql_en,
-    'AI-ModelScope/texttosqlv2_25000_v2', ['train'],
-    tags=['chat', 'sql'],
-    hf_dataset_id='Clinton/texttosqlv2_25000_v2')
-@register_dataset(
-    DatasetName.school_math_zh,
-    'AI-ModelScope/school_math_0.25M', ['train'],
-    tags=['chat', 'math'],
-    hf_dataset_id='BelleGroup/school_math_0.25M')
-@register_dataset(DatasetName.gpt4all_en, 'wyj123456/GPT4all', ['train'], tags=['chat', 'general'])
-@register_dataset(DatasetName.cot_zh, 'YorickHe/CoT_zh', ['train'], tags=['chat', 'general'])
-@register_dataset(DatasetName.cot_en, 'YorickHe/CoT', ['train'], tags=['chat', 'general'])
-@register_dataset(DatasetName.instinwild_en, 'wyj123456/instinwild', [('subset', 'train')], tags=['chat', 'general'])
-@register_dataset(DatasetName.instinwild_zh, 'wyj123456/instinwild', ['train'], tags=['chat', 'general'])
-@register_dataset(
-    DatasetName.code_alpaca_en,
-    'wyj123456/code_alpaca_en', ['train'],
-    tags=['chat', 'coding'],
-    hf_dataset_id='sahil2801/CodeAlpaca-20k')
-@register_dataset(
-    DatasetName.finance_en,
-    'wyj123456/finance_en', ['train'],
-    tags=['chat', 'financial'],
-    hf_dataset_id='ssbuild/alpaca_finance_en')
-@register_dataset(
-    DatasetName.alpaca_en,
-    'AI-ModelScope/alpaca-gpt4-data-en', ['train'],
-    tags=['chat', 'general', '🔥'],
-    hf_dataset_id='vicgalle/alpaca-gpt4')
-@register_dataset(
-    DatasetName.coig_cqia_chinese_traditional,
-    'AI-ModelScope/COIG-CQIA', [('chinese_traditional', 'train')],
-    tags=['general', '🔥'])
-@register_dataset(
-    DatasetName.coig_cqia_coig_pc, 'AI-ModelScope/COIG-CQIA', [('coig_pc', 'train')], tags=['general', '🔥'])
-@register_dataset(DatasetName.coig_cqia_exam, 'AI-ModelScope/COIG-CQIA', [('exam', 'train')], tags=['general', '🔥'])
-@register_dataset(
-    DatasetName.coig_cqia_finance, 'AI-ModelScope/COIG-CQIA', [('finance', 'train')], tags=['general', '🔥'])
-@register_dataset(DatasetName.coig_cqia_douban, 'AI-ModelScope/COIG-CQIA', [('douban', 'train')], tags=['general', '🔥'])
-@register_dataset(
-    DatasetName.coig_cqia_human_value, 'AI-ModelScope/COIG-CQIA', [('human_value', 'train')], tags=['general', '🔥'])
-@register_dataset(
-    DatasetName.coig_cqia_logi_qa, 'AI-ModelScope/COIG-CQIA', [('logi_qa', 'train')], tags=['general', '🔥'])
-@register_dataset(
-    DatasetName.coig_cqia_ruozhiba, 'AI-ModelScope/COIG-CQIA', [('ruozhiba', 'train')], tags=['general', '🔥'])
-@register_dataset(
-    DatasetName.coig_cqia_segmentfault, 'AI-ModelScope/COIG-CQIA', [('segmentfault', 'train')], tags=['general', '🔥'])
-@register_dataset(DatasetName.coig_cqia_wiki, 'AI-ModelScope/COIG-CQIA', [('wiki', 'train')], tags=['general', '🔥'])
-@register_dataset(
-    DatasetName.coig_cqia_wikihow, 'AI-ModelScope/COIG-CQIA', [('wikihow', 'train')], tags=['general', '🔥'])
-@register_dataset(DatasetName.coig_cqia_xhs, 'AI-ModelScope/COIG-CQIA', [('xhs', 'train')], tags=['general', '🔥'])
-@register_dataset(DatasetName.coig_cqia_zhihu, 'AI-ModelScope/COIG-CQIA', [('zhihu', 'train')], tags=['general', '🔥'])
-@register_dataset(
-    DatasetName.ms_agent_for_agentfabric_default,
-    'AI-ModelScope/ms_agent_for_agentfabric', [('default', 'train')],
-    tags=['chat', 'agent', 'multi-round'])
-@register_dataset(
-    DatasetName.ms_agent_for_agentfabric_addition,
-    'AI-ModelScope/ms_agent_for_agentfabric', [('addition', 'train')],
-    tags=['chat', 'agent', 'multi-round'])
-def get_dataset_from_repo(dataset_id: str,
-                          train_subset_split_list: List[SubsetSplit],
-                          val_subset_split_list: Optional[List[SubsetSplit]],
-                          preprocess_func: PreprocessFunc,
-                          remove_useless_columns: bool = True,
-                          train_dataset_sample: int = -1,
-                          val_dataset_sample: int = -1,
-                          use_hf: bool = False) -> Tuple[HfDataset, Optional[HfDataset]]:
-    dataset_list = []
-    _iter = zip([train_subset_split_list, val_subset_split_list], [train_dataset_sample, val_dataset_sample])
-    for subset_split_list, dataset_sample in _iter:
-        if use_hf:
-            dataset = load_hf_dataset(dataset_id, subset_split_list)
+def _post_preprocess(
+    train_dataset: HfDataset,
+    dataset_sample: int,
+    random_state: Optional[RandomState] = None,
+    preprocess_func: Optional[PreprocessFunc] = None,
+    dataset_test_ratio: float = 0.,
+    remove_useless_columns: bool = True,
+) -> Tuple[HfDataset, Optional[HfDataset]]:
+    assert train_dataset is not None
+    if dataset_sample == -1:
+        dataset_sample = len(train_dataset)
+    assert 0 <= dataset_test_ratio <= 1
+    if dataset_test_ratio == 1:
+        train_dataset, val_dataset = None, train_dataset
+        val_sample = dataset_sample
+        assert val_sample <= len(val_dataset), f'dataset_sample: {dataset_sample}, len(val_dataset): {len(val_dataset)}'
+        val_dataset = sample_dataset(val_dataset, val_sample, random_state)
+    else:
+        if dataset_test_ratio == 0:
+            train_sample = dataset_sample
+            val_dataset = None
         else:
-            dataset = load_ms_dataset(dataset_id, subset_split_list)
-        if dataset is not None:
-            if dataset_sample > 0 and len(dataset) > dataset_sample:
-                random_state = np.random.RandomState(42)
-                idxs = random_state.permutation(dataset_sample)
-                dataset = dataset.select(idxs)
+            # Avoid having a high train_sample causing a high val_sample.
+            _train_len = min(len(train_dataset), dataset_sample)
+            val_sample = max(int(_train_len * dataset_test_ratio), 1)
+            train_sample = dataset_sample - val_sample
+            assert isinstance(val_sample, int)
+            train_dataset, val_dataset = train_dataset.train_test_split(
+                test_size=val_sample, seed=get_seed(random_state)).values()
+
+        assert train_sample > 0
+        train_dataset = sample_dataset(train_dataset, train_sample, random_state)
+
+    res = []
+    for dataset in [train_dataset, val_dataset]:
+        if dataset is not None and preprocess_func is not None:
             dataset = preprocess_func(dataset)
-            if remove_useless_columns:
-                dataset = _remove_useless_columns(dataset)
-        dataset_list.append(dataset)
-    return tuple(dataset_list)
+        if dataset is not None and len(dataset) > 0 and remove_useless_columns:
+            dataset = _remove_useless_columns(dataset)
+        res.append(dataset)
+    return tuple(res)
 
 
-_multi_alpaca_subset_list = ['ar', 'de', 'es', 'fr', 'id', 'ja', 'ko', 'pt', 'ru', 'th', 'vi']
-
-register_dataset(
-    DatasetName.multi_alpaca_all,
-    'damo/nlp_polylm_multialpaca_sft', [(subset, 'train') for subset in _multi_alpaca_subset_list],
-    None,
-    None,
-    get_dataset_from_repo,
-    tags=['chat', 'general', 'multilingual'],
-    help="""language_list
-    Language-key	Language	# examples
-    ar	Arabic	14,671
-    de	German	9,515
-    es	Spanish	9,958
-    fr	France	11,332
-    id	Indonesian	12,117
-    ja	Japanese	10,191
-    ko	Korean	14,402
-    pt	Portuguese	10,825
-    ru	Russian	14,286
-    th	Thai	11,496
-    vi	Vietnamese	13,908
-""")
+def get_dataset_from_repo(dataset_id: str,
+                          subsets: Optional[List[str]],
+                          preprocess_func: PreprocessFunc,
+                          split: List[str],
+                          dataset_sample: int = -1,
+                          *,
+                          random_state: Optional[RandomState] = None,
+                          dataset_test_ratio: float = 0.,
+                          remove_useless_columns: bool = True,
+                          use_hf: bool = False) -> Tuple[HfDataset, Optional[HfDataset]]:
+    if subsets is None:
+        subsets = []
+    assert len(split) > 0
+    if len(subsets) == 0:
+        subset_split_list = split
+    else:
+        subset_split_list = list(itertools.product(subsets, split))
+    dataset = load_ms_dataset(dataset_id, subset_split_list, use_hf)
+    return _post_preprocess(dataset, dataset_sample, random_state, preprocess_func, dataset_test_ratio,
+                            remove_useless_columns)
 
 
 def _concat_inst_inp_alpaca_zh(inst: str, inp: str) -> str:
     if inp.startswith('输入：'):
         inp = inp[3:]
     return f'{inst}\n{inp}'
 
 
 register_dataset(
     DatasetName.alpaca_zh,
-    'AI-ModelScope/alpaca-gpt4-data-zh', ['train'],
+    'AI-ModelScope/alpaca-gpt4-data-zh',
     None,
     AlpacaPreprocessor(concat_inst_inp=_concat_inst_inp_alpaca_zh),
     get_dataset_from_repo,
     tags=['chat', 'general', '🔥'],
-    hf_dataset_id='c-s-ale/alpaca-gpt4-data-zh')
+    hf_dataset_id='llm-wizard/alpaca-gpt4-data-zh')
 
 
 def _preprocess_vision_dataset(dataset: HfDataset) -> HfDataset:
     prompt = 'please describe the image.'
     image_key = 'image'
     response_key = 'caption'
 
@@ -400,29 +372,29 @@
         response.append(d[response_key])
     dataset = HfDataset.from_dict({'query': query, 'response': response})
     return dataset
 
 
 register_dataset(
     DatasetName.coco_en,
-    'modelscope/coco_2014_caption', [('coco_2014_caption', 'train')], [('coco_2014_caption', 'validation')],
+    'modelscope/coco_2014_caption', ['coco_2014_caption'],
     _preprocess_vision_dataset,
     get_dataset_from_repo,
-    tags=['chat', 'multi-modal', 'vision'])
+    split=['train', 'validation'],
+    tags=['chat', 'multi-modal', 'vision'],
+    is_main=False)
 
 register_dataset(
-    DatasetName.coco_mini_en,
-    'modelscope/coco_2014_caption', [('coco_2014_caption', 'train')], [('coco_2014_caption', 'validation')],
+    DatasetName.coco_en_mini,
+    'modelscope/coco_2014_caption', ['coco_2014_caption'],
     _preprocess_vision_dataset,
     get_dataset_from_repo,
-    function_kwargs={
-        'train_dataset_sample': 20000,
-        'val_dataset_sample': 200
-    },
-    tags=['chat', 'multi-modal', 'vision', '🔥'])
+    split=['validation'],
+    tags=['chat', 'multi-modal', 'vision', '🔥'],
+    is_main=False)
 
 
 def _preprocess_vision_dataset2(dataset: HfDataset) -> HfDataset:
     query = 'please describe the image.'
     image_key = 'image'
     response_key = 'caption'
 
@@ -434,23 +406,30 @@
         if '&&' in d[response_key]:
             d[response_key] = d[response_key].split('&&')[0]
         response.append(d[response_key])
     return HfDataset.from_dict({'query': [query] * len(response), 'response': response, 'images': images})
 
 
 register_dataset(
-    DatasetName.coco_mini_en_2,
-    'modelscope/coco_2014_caption', [('coco_2014_caption', 'train')], [('coco_2014_caption', 'validation')],
+    DatasetName.coco_en_2,
+    'modelscope/coco_2014_caption', ['coco_2014_caption'],
+    _preprocess_vision_dataset2,
+    get_dataset_from_repo,
+    split=['train', 'validation'],
+    tags=['chat', 'multi-modal', 'vision'],
+    is_main=False)
+
+register_dataset(
+    DatasetName.coco_en_2_mini,
+    'modelscope/coco_2014_caption', ['coco_2014_caption'],
     _preprocess_vision_dataset2,
     get_dataset_from_repo,
-    function_kwargs={
-        'train_dataset_sample': 20000,
-        'val_dataset_sample': 200
-    },
-    tags=['chat', 'multi-modal', 'vision', '🔥'])
+    split=['validation'],
+    tags=['chat', 'multi-modal', 'vision', '🔥'],
+    is_main=False)
 
 
 def _preprocess_aishell1_dataset(dataset: HfDataset) -> HfDataset:
     prompt = '语音转文本'
     audio_key = 'Audio:FILE'
     response_key = 'Text:LABEL'
     query_format = f'Audio 1:<audio>{{audio_path}}</audio>\n{prompt}'
@@ -461,26 +440,30 @@
         response.append(d[response_key].replace(' ', ''))
     dataset = HfDataset.from_dict({'query': query, 'response': response})
     return dataset
 
 
 register_dataset(
     DatasetName.aishell1_zh,
-    'speech_asr/speech_asr_aishell1_trainsets', ['train', 'validation'], ['test'],
+    'speech_asr/speech_asr_aishell1_trainsets',
+    None,
     _preprocess_aishell1_dataset,
     get_dataset_from_repo,
+    split=['train', 'validation', 'test'],
     tags=['chat', 'multi-modal', 'audio'])
 
 register_dataset(
-    DatasetName.aishell1_mini_zh,
-    'speech_asr/speech_asr_aishell1_trainsets', ['validation'], ['test'],
+    DatasetName.aishell1_zh_mini,
+    'speech_asr/speech_asr_aishell1_trainsets',
+    None,
     _preprocess_aishell1_dataset,
     get_dataset_from_repo,
-    function_kwargs={'val_dataset_sample': 200},
-    tags=['chat', 'multi-modal', 'audio', '🔥'])
+    split=['validation', 'test'],
+    tags=['chat', 'multi-modal', 'audio', '🔥'],
+    is_main=False)
 
 
 def _repair_agent_conversations(conversations: str, use_mini: bool) -> List[Dict[str, str]]:
     if use_mini:
         pattern = r'\d\. {"plugin_name": "(.+?)"'
     else:
         pattern = r'\d\. {"(?:plugin_)?name": "(.+?)"'
@@ -515,126 +498,93 @@
 
 def long_alpaca_preprocessor(dataset: HfDataset):
 
     def map_row(row):
         response = row['response']
         if response and response.startswith('Answer:'):
             response = response[len('Answer:') + 1:].strip()
-        return {'query': row['query'], 'response': response}
+            row['response'] = response
+        return response
 
-    return dataset.rename_columns({'instruction': 'query', 'output': 'response'}) \
-        .remove_columns(['input', 'file']).map(map_row).filter(lambda row: row['response'] is not None)
+    dataset = AlpacaPreprocessor()(dataset)
+    return dataset.map(map_row)
 
 
 register_dataset(
     DatasetName.long_alpaca_12k,
-    'AI-ModelScope/LongAlpaca-12k', ['train'], [],
+    'AI-ModelScope/LongAlpaca-12k',
+    None,
     long_alpaca_preprocessor,
     get_dataset_from_repo,
     tags=['longlora', 'QA'],
     hf_dataset_id='Yukang/LongAlpaca-12k')
 
 
 def _preprocess_ruozhiba(dataset: HfDataset):
 
     def map_row(row):
-        title = row['title'] if 'title' in row else row['content']
+        title = row['title'] if row.get('title', None) is not None else row['content']
         abs = row['abs'] if 'abs' in row else None
         if abs and abs != title:
             title = title + '，' + abs
 
         pattern = r'\d+[\.,\s,\、](.+)'
         match = re.search(pattern, title)
         if match:
             title = match.group(1)
         return {'response': title}
 
     return dataset.map(map_row).filter(lambda row: row['response'])
 
 
 register_dataset(
-    DatasetName.ruozhiba_post_annual,
-    'AI-ModelScope/ruozhiba', [('post-annual', 'train')], [],
-    _preprocess_ruozhiba,
-    get_dataset_from_repo,
-    tags=['pretrain', '🔥'])
-register_dataset(
-    DatasetName.ruozhiba_title_good,
-    'AI-ModelScope/ruozhiba', [('title-good', 'train')], [],
-    _preprocess_ruozhiba,
-    get_dataset_from_repo,
-    tags=['pretrain', '🔥'])
-register_dataset(
-    DatasetName.ruozhiba_title_norm,
-    'AI-ModelScope/ruozhiba', [('title-norm', 'train')], [],
+    DatasetName.ruozhiba,
+    'AI-ModelScope/ruozhiba', ['post-annual', 'title-good', 'title-norm'],
     _preprocess_ruozhiba,
     get_dataset_from_repo,
     tags=['pretrain', '🔥'])
 
 register_dataset(
     DatasetName.ms_bench,
-    'iic/ms_bench', ['train'], [],
-    ConversationsPreprocessor(repair_conversations=_repair_ms_bench, error_strategy='delete'),
-    get_dataset_from_repo,
-    tags=['chat', 'general', 'multi-round', '🔥'])
-
-register_dataset(
-    DatasetName.ms_bench_mini,
-    'iic/ms_bench', ['train'], [],
+    'iic/ms_bench',
+    None,
     ConversationsPreprocessor(repair_conversations=_repair_ms_bench, error_strategy='delete'),
     get_dataset_from_repo,
-    function_kwargs={'train_dataset_sample': 20000},
     tags=['chat', 'general', 'multi-round', '🔥'])
 
 register_dataset(
-    DatasetName.ms_agent,
-    'iic/ms_agent', ['train'], [],
-    ConversationsPreprocessor(error_strategy='delete'),
-    get_dataset_from_repo,
-    tags=['chat', 'agent', 'multi-round', '🔥'])
-
-register_dataset(
-    DatasetName.damo_agent_mini_zh,
-    'damo/MSAgent-Bench', ['train'], ['validation'],
+    DatasetName.damo_agent_zh_mini,
+    'damo/MSAgent-Bench',
+    None,
     ConversationsPreprocessor(
         repair_conversations=partial(_repair_agent_conversations, use_mini=True), error_strategy='delete'),
     get_dataset_from_repo,
-    tags=['chat', 'agent', 'multi-round'])
+    split=['train', 'validation'],
+    tags=['chat', 'agent', 'multi-round'],
+    is_main=False)
 register_dataset(
     DatasetName.damo_agent_zh,
-    'damo/MSAgent-Bench', ['train'], ['validation'],
+    'damo/MSAgent-Bench',
+    None,
     ConversationsPreprocessor(
-        repair_conversations=partial(_repair_agent_conversations, use_mini=False, error_strategy='delete')),
+        repair_conversations=partial(_repair_agent_conversations, use_mini=False), error_strategy='delete'),
     get_dataset_from_repo,
+    split=['train', 'validation'],
     tags=['chat', 'agent', 'multi-round'])
 
-register_dataset(
-    DatasetName.deepctrl_sft_zh,
-    'AI-ModelScope/deepctrl-sft-data', [['default', 'train']],
-    None,
-    SmartPreprocessor(),
-    get_dataset_from_repo,
-    tags=['chat', 'general', 'sft', 'multi-round'])
-
-register_dataset(
-    DatasetName.deepctrl_sft_en,
-    'AI-ModelScope/deepctrl-sft-data', [['en', 'train']],
-    None,
-    SmartPreprocessor(),
-    get_dataset_from_repo,
-    tags=['chat', 'general', 'sft', 'multi-round'])
-
 advertise_gen_prompt = """Task: Generating advertisements based on keywords.
 Keywords: {query}
 Advertisements:"""
 register_dataset(
     DatasetName.advertise_gen_zh,
-    'lvjianjin/AdvertiseGen', ['train'], ['validation'],
+    'lvjianjin/AdvertiseGen',
+    None,
     TextGenerationPreprocessor(advertise_gen_prompt, 'content', 'summary'),
     get_dataset_from_repo,
+    split=['train', 'validation'],
     tags=['text-generation', '🔥'],
     hf_dataset_id='shibing624/AdvertiseGen')
 
 _firefly_kind_list = [
     'ProseGeneration', 'MRC', 'JinYongGeneration', 'TextCorrection', 'ClassicalChinese', 'BELLE', 'StoryGeneration',
     'Couplet', 'Cot', 'Dictionary', 'Translation', 'Program', 'SentimentAnalyze', 'OpenQA', 'AncientPoem',
     'TextMatching', 'NLI', 'Summary', 'KeywordRecognition', 'ProductDesc', 'LyricGeneration', 'Composition',
@@ -655,74 +605,49 @@
     return HfDataset.from_dict({
         'query': query,
         'response': response,
     })
 
 
 @register_dataset(
-    DatasetName.firefly_all_zh,
+    DatasetName.firefly_zh,
     'wyj123456/firefly',
-    preprocess_func=_preprocess_firefly,
+    None,
+    _preprocess_firefly,
     tags=['chat', 'general'],
     function_kwargs={'kind_list': _firefly_kind_list})
-def get_firefly_zh_dataset(dataset_id: str, preprocess_func, kind_list: List[str], **kwargs) -> HfDataset:
+def get_firefly_zh_dataset(dataset_id: str, _, preprocess_func: PreprocessFunc, *args, **kwargs) -> HfDataset:
+    kind_list = kwargs['kind_list']
     file = 'firefly-train-1.1M.jsonl'
     dataset_dir = download_dataset(dataset_id, [file])
     fpath = os.path.join(dataset_dir, file)
     with open(fpath, 'r', encoding='utf-8') as f:
         text = f.read()
         text = text.replace('}{', '},{')
         text = f'[{text}]'
         dataset = json.loads(text)
     return preprocess_func(dataset, kind_list)
 
 
 register_dataset(
-    DatasetName.poetry_zh,
-    'modelscope/chinese-poetry-collection', ['train'], ['test'],
-    RenameColumnsPreprocessor({'text1': 'response'}),
-    get_dataset_from_repo,
-    tags=['text-generation', 'poetry'])
-
-register_dataset(
-    DatasetName.instruct_en,
-    'wyj123456/instruct', ['train'],
-    None,
-    RenameColumnsPreprocessor({
-        'prompt': 'query',
-        'completion': 'response'
-    }),
-    get_dataset_from_repo,
-    tags=['chat', 'general'])
-
-register_dataset(
     DatasetName.cmnli_zh,
-    'clue', [('cmnli', 'train')], [('cmnli', 'validation')],
+    'modelscope/clue', ['cmnli'],
     ClsPreprocessor(['neutral', 'entailment', 'contradiction'], 'Natural Language Inference', True),
     get_dataset_from_repo,
+    split=['train', 'validation'],
     tags=['text-generation', 'classification'],
     hf_dataset_id='clue')
 
 register_dataset(
-    DatasetName.cmnli_mini_zh,
-    'clue', [('cmnli', 'train')], [('cmnli', 'validation')],
-    ClsPreprocessor(['neutral', 'entailment', 'contradiction'], 'Natural Language Inference', True),
-    get_dataset_from_repo,
-    function_kwargs={
-        'train_dataset_sample': 20000,
-        'val_dataset_sample': 200
-    },
-    tags=['text-generation', 'classification', '🔥'],
-    hf_dataset_id='clue')
-
-register_dataset(
     DatasetName.jd_sentiment_zh,
-    'DAMO_NLP/jd', ['train'], ['validation'],
+    'DAMO_NLP/jd',
+    None,
     ClsPreprocessor(['negative', 'positive'], 'Sentiment Classification', False),
     get_dataset_from_repo,
+    split=['train', 'validation'],
     tags=['text-generation', 'classification', '🔥'])
 
 
 def _preprocess_dureader_robust(dataset: HfDataset) -> HfDataset:
     prompt = """Task: Question Generation
 Context: {context}
 Answer: {answer}
@@ -735,59 +660,24 @@
         query.append(q)
         response.append(d['text2'])
     return HfDataset.from_dict({'query': query, 'response': response})
 
 
 register_dataset(
     DatasetName.dureader_robust_zh,
-    'modelscope/DuReader_robust-QG', ['train', 'validation'], ['test'],
+    'modelscope/DuReader_robust-QG',
+    None,
     _preprocess_dureader_robust,
     get_dataset_from_repo,
+    split=['train', 'validation', 'test'],
     tags=['text-generation', '🔥'])
 
-register_dataset(
-    DatasetName.medical_en,
-    'huangjintao/medical_zh', [('en', 'train'), ('en', 'val')], [('en', 'test')],
-    RenameColumnsPreprocessor({
-        'input': 'query',
-        'output': 'response'
-    }),
-    get_dataset_from_repo,
-    tags=['chat', 'medical'])
-
-register_dataset(
-    DatasetName.stack_exchange_paired,
-    'AI-ModelScope/stack-exchange-paired', [('default', 'train')],
-    None,
-    RenameColumnsPreprocessor({
-        'question': 'query',
-        'response_j': 'response',
-        'response_k': 'rejected_response',
-    }),
-    get_dataset_from_repo,
-    tags=['hfrl', 'dpo', 'pairwise'])
-
 
 def process_hh_rlhf(dataset):
 
-    def extract_anthropic_prompt(prompt_and_response):
-        """Extract the anthropic prompt from a prompt and response pair."""
-        search_term = '\n\nAssistant:'
-        search_term_idx = prompt_and_response.rfind(search_term)
-        assert search_term_idx != -1, f"Prompt and response does not contain '{search_term}'"
-        return prompt_and_response[:search_term_idx + len(search_term)]
-
-    def reorganize_row_simple(sample) -> Dict[str, str]:
-        prompt = extract_anthropic_prompt(sample['chosen'])
-        return {
-            'query': prompt,
-            'response': sample['chosen'][len(prompt):],
-            'rejected_response': sample['rejected'][len(prompt):],
-        }
-
     def reorganize_row(row):
         import re
         chosen = row['chosen'].strip()
         rejected = row['rejected'].strip()
         parts_chosen = [s.strip() for s in re.split('\n\nHuman:|\n\nAssistant:|\n\nHum:', chosen)]
         parts_rejected = [s.strip() for s in re.split('\n\nHuman:|\n\nAssistant:|\n\nHum:', rejected)]
         if parts_chosen[0].startswith('Human:'):
@@ -823,46 +713,19 @@
             'history': history,
         }
 
     return dataset.map(reorganize_row).filter(lambda row: row['query'] is not None)
 
 
 register_dataset(
-    DatasetName.hh_rlhf_harmless_base,
-    'AI-ModelScope/hh-rlhf', [('harmless-base', 'train')], [('harmless-base', 'test')],
-    process_hh_rlhf,
-    get_dataset_from_repo,
-    tags=['rlhf', 'dpo', 'pairwise'])
-
-register_dataset(
-    DatasetName.hh_rlhf_helpful_base,
-    'AI-ModelScope/hh-rlhf', [('helpful-base', 'train')], [('helpful-base', 'test')],
-    process_hh_rlhf,
-    get_dataset_from_repo,
-    tags=['rlhf', 'dpo', 'pairwise'])
-
-register_dataset(
-    DatasetName.hh_rlhf_helpful_online,
-    'AI-ModelScope/hh-rlhf', [('helpful-online', 'train')], [('helpful-online', 'test')],
-    process_hh_rlhf,
-    get_dataset_from_repo,
-    tags=['rlhf', 'dpo', 'pairwise'])
-
-register_dataset(
-    DatasetName.hh_rlhf_helpful_rejection_sampled,
-    'AI-ModelScope/hh-rlhf', [('helpful-rejection-sampled', 'train')], [('helpful-rejection-sampled', 'test')],
-    process_hh_rlhf,
-    get_dataset_from_repo,
-    tags=['rlhf', 'dpo', 'pairwise'])
-
-register_dataset(
-    DatasetName.hh_rlhf_red_team_attempts,
-    'AI-ModelScope/hh-rlhf', [('red-team-attempts', 'train')], [('red-team-attempts', 'test')],
+    DatasetName.hh_rlhf,
+    'AI-ModelScope/hh-rlhf', ['harmless-base', 'helpful-base', 'helpful-online', 'helpful-rejection-sampled'],
     process_hh_rlhf,
     get_dataset_from_repo,
+    split=['train', 'test'],
     tags=['rlhf', 'dpo', 'pairwise'])
 
 
 def process_hh_rlhf_cn(dataset):
 
     def reorganize_row(row):
         history = []
@@ -915,101 +778,64 @@
             return False
 
     return dataset.filter(row_can_be_parsed).map(reorganize_row).filter(lambda row: row['query'])
 
 
 register_dataset(
     DatasetName.hh_rlhf_cn,
-    'AI-ModelScope/hh_rlhf_cn', [('hh_rlhf', 'train')], [('hh_rlhf', 'test')],
+    'AI-ModelScope/hh_rlhf_cn',
+    ['hh_rlhf', 'harmless_base_cn', 'harmless_base_en', 'helpful_base_cn', 'helpful_base_en'],
     process_hh_rlhf_cn,
     get_dataset_from_repo,
+    split=['train', 'test'],
     tags=['rlhf', 'dpo', 'pairwise', '🔥'])
 
-register_dataset(
-    DatasetName.hh_rlhf_cn_harmless_base_cn,
-    'AI-ModelScope/hh_rlhf_cn', [('harmless_base_cn', 'train')], [('harmless_base_cn', 'test')],
-    process_hh_rlhf_cn,
-    get_dataset_from_repo,
-    tags=['rlhf', 'dpo', 'pairwise'])
 
-register_dataset(
-    DatasetName.hh_rlhf_cn_harmless_base_en,
-    'AI-ModelScope/hh_rlhf_cn', [('harmless_base_en', 'train')], [('harmless_base_en', 'test')],
-    process_hh_rlhf_cn,
-    get_dataset_from_repo,
-    tags=['rlhf', 'dpo', 'pairwise'])
+def process_shareai_dpo(dataset):
 
-register_dataset(
-    DatasetName.hh_rlhf_cn_helpful_base_cn,
-    'AI-ModelScope/hh_rlhf_cn', [('helpful_base_cn', 'train')], [('helpful_base_cn', 'test')],
-    process_hh_rlhf_cn,
-    get_dataset_from_repo,
-    tags=['rlhf', 'dpo', 'pairwise'])
+    def reorganize_row(row):
+        return {
+            'query': row['question'],
+            'response': row['answer_zh'],
+            'rejected_response': row['answer_en'],
+        }
+
+    return dataset.map(reorganize_row)
 
-register_dataset(
-    DatasetName.hh_rlhf_cn_helpful_base_en,
-    'AI-ModelScope/hh_rlhf_cn', [('helpful_base_en', 'train')], [('helpful_base_en', 'test')],
-    process_hh_rlhf_cn,
-    get_dataset_from_repo,
-    tags=['rlhf', 'dpo', 'pairwise'])
 
 register_dataset(
-    DatasetName.medical_zh,
-    'huangjintao/medical_zh', [('zh', 'train'), ('zh', 'val')], [('zh', 'test')],
-    RenameColumnsPreprocessor({
-        'instruction': 'query',
-        'output': 'response'
-    }),
-    get_dataset_from_repo,
-    tags=['chat', 'medical'])
-
-register_dataset(
-    DatasetName.medical_mini_zh,
-    'huangjintao/medical_zh', [('zh', 'train'), ('zh', 'val')], [('zh', 'test')],
-    RenameColumnsPreprocessor({
-        'instruction': 'query',
-        'output': 'response'
-    }),
+    DatasetName.shareai_llama3_dpo_zh_en_emoji,
+    'hjh0119/shareAI-Llama3-DPO-zh-en-emoji', ['default'],
+    process_shareai_dpo,
     get_dataset_from_repo,
-    function_kwargs={'train_dataset_sample': 50000},
-    tags=['chat', 'medical'])
+    tags=['rlhf', 'dpo', 'pairwise'])
 
 
 def _preprocess_sharegpt(dataset: HfDataset) -> HfDataset:
     query = []
     response = []
     history: List[History] = []
     for d in tqdm(dataset):
         if isinstance(d['conversation'], str):
-            conversation = ast.literal_eval(d['conversation'])
+            try:
+                conversation = ast.literal_eval(d['conversation'])
+            except SyntaxError:
+                continue
         query.append(conversation[-1]['human'])
         response.append(conversation[-1]['assistant'])
         h = []
         for c in conversation[:-1]:
             h.append([c['human'], c['assistant']])
         history.append(h)
     return HfDataset.from_dict({'query': query, 'response': response, 'history': history})
 
 
-_sharegpt_zh_subset_list = ['common-zh', 'computer-zh', 'unknow-zh']
-
-_sharegpt_en_subset_list = ['common-en', 'computer-en']
-
 register_dataset(
-    DatasetName.sharegpt_zh,
-    'huangjintao/sharegpt', [(subset, 'train') for subset in _sharegpt_zh_subset_list],
-    None,
-    _preprocess_sharegpt,
-    get_dataset_from_repo,
-    tags=['chat', 'general', 'multi-round'])
-
-register_dataset(
-    DatasetName.sharegpt_en,
-    'huangjintao/sharegpt', [(subset, 'train') for subset in _sharegpt_en_subset_list],
-    None,
+    DatasetName.sharegpt,
+    'huangjintao/sharegpt', ['common-zh', 'computer-zh', 'unknow-zh', 'common-en', 'computer-en'],
     _preprocess_sharegpt,
     get_dataset_from_repo,
     tags=['chat', 'general', 'multi-round'])
 
 
 def _preprocess_capcha_images(dataset: HfDataset) -> HfDataset:
     query = 'recognize the content.'
@@ -1022,138 +848,72 @@
         images.append(d[image_key])
         response.append(d[response_key])
     dataset = HfDataset.from_dict({'query': [query] * len(response), 'response': response, 'images': images})
     dataset._info.features._column_requires_decoding['images'] = True
     return dataset
 
 
-def _repair_planner(conversations: list) -> list:
-    if isinstance(conversations, str):
-        conversations = ast.literal_eval(conversations)
-    if len(conversations) == 2 and conversations[0]['from'] != 'user':
-        conversations[0]['from'] = 'user'
-    return conversations
-
-
 register_dataset(
     DatasetName.capcha_images,
-    'AI-ModelScope/captcha-images', [('default', 'train')], [('default', 'validation')],
+    'AI-ModelScope/captcha-images',
+    None,
     _preprocess_capcha_images,
     get_dataset_from_repo,
+    split=['train', 'validation'],
     tags=['chat', 'multi-modal', 'vision'])
 
-register_dataset(
-    DatasetName.cls_fudan_news_zh,
-    'damo/zh_cls_fudan-news', ['train'],
-    None,
-    RenameColumnsPreprocessor({
-        'prompt': 'query',
-        'answer': 'response'
-    }),
-    get_dataset_from_repo,
-    tags=['chat', 'classification'])
 
-register_dataset(
-    DatasetName.ner_java_zh,
-    'damo/zh_ner-JAVE', ['train'],
-    None,
-    RenameColumnsPreprocessor({
-        'prompt': 'query',
-        'answer': 'response'
-    }),
-    get_dataset_from_repo,
-    tags=['chat', 'ner'])
-
-register_dataset(
-    DatasetName.codefuse_python_en,
-    'codefuse-ai/CodeExercise-Python-27k', ['train'],
-    None,
-    ConversationsPreprocessor('human', 'bot', conversations_key='chat_rounds', from_key='role', value_key='content'),
-    get_dataset_from_repo,
-    tags=['chat', 'coding', '🔥'])
+def _repair_toolbench(conversations: Dict[str, str]) -> Dict[str, str]:
+    assert len(conversations) == 2
+    if (conversations[1]['from'] in {'caller', 'conclusion'}):
+        conversations[1]['from'] = 'assistant'
+    return conversations
 
-register_dataset(
-    DatasetName.toolbench_for_alpha_umi_backbone,
-    'shenweizhou/alpha-umi-toolbench-processed-v2', [('backbone', 'train')],
-    None,
-    ConversationsPreprocessor('system', system_role=None),
-    get_dataset_from_repo,
-    tags=['chat', 'agent'])
 
 register_dataset(
-    DatasetName.toolbench_for_alpha_umi_caller,
-    'shenweizhou/alpha-umi-toolbench-processed-v2', [('caller', 'train')],
-    None,
-    ConversationsPreprocessor('system', 'caller', None),
+    DatasetName.toolbench_for_alpha_umi,
+    'shenweizhou/alpha-umi-toolbench-processed-v2', ['backbone', 'caller', 'planner', 'summarizer'],
+    ConversationsPreprocessor('system', system_role='-', repair_conversations=_repair_toolbench),
     get_dataset_from_repo,
-    tags=['chat', 'agent'])
-
-register_dataset(
-    DatasetName.toolbench_for_alpha_umi_planner,
-    'shenweizhou/alpha-umi-toolbench-processed-v2', [('planner', 'train')],
-    None,
-    ConversationsPreprocessor(repair_conversations=_repair_planner, error_strategy='delete'),
-    get_dataset_from_repo,
-    tags=['chat', 'agent'])
-
-register_dataset(
-    DatasetName.toolbench_for_alpha_umi_summarizer,
-    'shenweizhou/alpha-umi-toolbench-processed-v2', [('summarizer', 'train')],
-    None,
-    ConversationsPreprocessor('system', 'conclusion', None),
-    get_dataset_from_repo,
-    tags=['chat', 'agent'])
+    tags=['chat', 'agent', '🔥'])
 
 
 def _preprocess_blossom_math(dataset: HfDataset) -> HfDataset:
     response = []
     for d in tqdm(dataset):
         output, answer = d['output'], d['answer']
         response.append(f'{output}\n\nAnswer: {answer}')
     return HfDataset.from_dict({'query': dataset['input'], 'response': response})
 
 
 register_dataset(
     DatasetName.blossom_math_zh,
-    'AI-ModelScope/blossom-math-v2', ['train'],
+    'AI-ModelScope/blossom-math-v2',
     None,
     _preprocess_blossom_math,
     get_dataset_from_repo,
     tags=['chat', 'math', '🔥'],
     hf_dataset_id='Azure99/blossom-math-v2')
 
 register_dataset(
     DatasetName.sql_create_context_en,
-    'AI-ModelScope/sql-create-context', ['train'],
+    'AI-ModelScope/sql-create-context',
     None,
     ComposePreprocessor([
         RenameColumnsPreprocessor({
             'question': 'instruction',
             'context': 'input',
             'answer': 'output'
         }),
         AlpacaPreprocessor(),
     ]),
     get_dataset_from_repo,
     tags=['chat', 'sql', '🔥'],
     hf_dataset_id='b-mc2/sql-create-context')
 
-register_dataset(
-    DatasetName.lawyer_llama_zh,
-    'AI-ModelScope/lawyer_llama_data', ['train'],
-    None,
-    RenameColumnsPreprocessor({
-        'instruction': 'query',
-        'output': 'response',
-        'history': '_'
-    }),
-    get_dataset_from_repo,
-    tags=['chat', 'law'],
-    hf_dataset_id='Skepsun/lawyer_llama_data')
-
 
 def _preprocess_tigerbot_law(dataset: HfDataset) -> HfDataset:
     prompt = """{type}
 {title}
 """
     response = []
     for d in tqdm(dataset):
@@ -1167,15 +927,15 @@
     return HfDataset.from_dict({
         'response': response,
     })
 
 
 register_dataset(
     DatasetName.tigerbot_law_zh,
-    'AI-ModelScope/tigerbot-law-plugin', ['train'],
+    'AI-ModelScope/tigerbot-law-plugin',
     None,
     _preprocess_tigerbot_law,
     get_dataset_from_repo,
     tags=['text-generation', 'law', 'pretrained'],
     hf_dataset_id='TigerResearch/tigerbot-law-plugin')
 
 
@@ -1195,81 +955,72 @@
         query.append(problem)
         response.append(f'{code}\n\n{explanation}')
     return HfDataset.from_dict({'query': query, 'response': response})
 
 
 register_dataset(
     DatasetName.leetcode_python_en,
-    'AI-ModelScope/leetcode-solutions-python', ['train'],
+    'AI-ModelScope/leetcode-solutions-python',
     None,
     _preprocess_leetcode_python,
     get_dataset_from_repo,
     tags=['chat', 'coding', '🔥'])
 
-_agent_instruct_subset_list = ['alfworld', 'db', 'kg', 'mind2web', 'os', 'webshop']
-
 
 def _repair_conversations_agent_instruct(s: str) -> List[Dict[str, Any]]:
     s = s.replace('}\n {', '},\n {')
     if isinstance(s, str):
         s = ast.literal_eval(s)
     return s
 
 
 register_dataset(
     DatasetName.agent_instruct_all_en,
-    'huangjintao/AgentInstruct_copy', [(subset, 'train') for subset in _agent_instruct_subset_list],
-    None,
+    'huangjintao/AgentInstruct_copy', ['alfworld', 'db', 'kg', 'mind2web', 'os', 'webshop'],
     ConversationsPreprocessor('human', 'gpt', repair_conversations=_repair_conversations_agent_instruct),
     get_dataset_from_repo,
     tags=['chat', 'agent', 'multi-round'])
 
 
 def _preprocess_msagent_multirole_dataset(dataset: HfDataset) -> HfDataset:
     res_prompt = """\n\n【注意事项】\n1. 这是聊天室，不要发送私信给任何人\n2. 仅代表你个人说话,不要扮演其他人，
     只根据对话历史进行回复\n3. 长话短说，不要说太多话，不要超过50字 """
     history_prompt = '\n\n【chat history】'
     conv_prompt = '\n {name}:{content}'
-    query = []
-    response = []
+    system, query, response = [], [], []
+
+    def process_conversation(conv):
+        query, response = '', conv[-1]['value']
+        system = conv[0]['value'] if conv[0]['from'] != 'user' else ''
+        if conv[0]['from'] == 'user':
+            query = conv[0]['value']
+        elif 'next_speakers:' not in system:
+            if '【注意事项】' not in system and system:
+                system += res_prompt
+            system += history_prompt
+            system += ''.join([conv_prompt.format(name=c['from'], content=c['value']) for c in conv[1:-1]])
+
+        return system, query, response
 
     for d in dataset:
-        conv = d['conversations']
-        system = conv[0]['value']
-        if '【注意事项】' not in system:
-            system += res_prompt
-        system += history_prompt
-        response.append(conv[-1]['value'])
-        for i in range(1, len(conv) - 1):
-            system += conv_prompt.format(name=conv[i]['from'], content=conv[i]['value'])
-        query.append(system)
-    return HfDataset.from_dict({'query': query, 'response': response})
+        sys, qry, resp = process_conversation(d['conversations'])
+        system.append(sys)
+        query.append(qry)
+        response.append(resp)
+    return HfDataset.from_dict({'system': system, 'query': query, 'response': response})
 
 
 register_dataset(
     DatasetName.ms_agent_multirole,
-    'iic/MSAgent-MultiRole', [('default', 'train')],
+    'iic/MSAgent-MultiRole',
     None,
     _preprocess_msagent_multirole_dataset,
     get_dataset_from_repo,
     tags=['chat', 'agent', 'multi-round', 'role-play', 'multi-agent'])
 
-register_dataset(
-    DatasetName.codefuse_evol_instruction_zh,
-    'codefuse-ai/Evol-instruction-66k', ['train'],
-    None,
-    RenameColumnsPreprocessor({
-        'instruction': 'query',
-        'output': 'response'
-    }),
-    get_dataset_from_repo,
-    tags=['chat', 'coding', '🔥'])
-
-hc3_chinese_subset = ['baike', 'open_qa', 'nlpcc_dbqa', 'finance', 'medicine', 'law', 'psychology']
-
 
 def _preprocess_hc3(dataset: HfDataset) -> HfDataset:
     prompt = """Classification Task: Are the following responses from a human or from ChatGPT?
 Question: {question}
 Answer: {answer}
 Category: Human, ChatGPT
 Output:"""
@@ -1284,164 +1035,28 @@
             query.append(prompt.format(question=question, answer=c))
             response.append('ChatGPT')
     return HfDataset.from_dict({'query': query, 'response': response})
 
 
 register_dataset(
     DatasetName.hc3_zh,
-    'simpleai/HC3-Chinese', [[subset, 'train'] for subset in hc3_chinese_subset], [],
+    'simpleai/HC3-Chinese', ['baike', 'open_qa', 'nlpcc_dbqa', 'finance', 'medicine', 'law', 'psychology'],
     _preprocess_hc3,
     get_dataset_from_repo,
     tags=['text-generation', 'classification', '🔥'],
     hf_dataset_id='Hello-SimpleAI/HC3-Chinese')
 
 register_dataset(
     DatasetName.hc3_en,
-    'simpleai/HC3', [[subset, 'train'] for subset in ['finance', 'medicine']], [],
+    'simpleai/HC3', ['finance', 'medicine'],
     _preprocess_hc3,
     get_dataset_from_repo,
     tags=['text-generation', 'classification', '🔥'],
     hf_dataset_id='Hello-SimpleAI/HC3')
 
-register_dataset(
-    DatasetName.tulu_v2_sft_mixture,
-    'AI-ModelScope/tulu-v2-sft-mixture', ['train'], [],
-    None,
-    get_dataset_from_repo,
-    tags=['chat', 'multilingual', 'general', 'multi-round'],
-    hf_dataset_id='allenai/tulu-v2-sft-mixture')
-register_dataset(
-    DatasetName.webnovel_zh,
-    'AI-ModelScope/webnovel_cn', ['train'], [],
-    None,
-    get_dataset_from_repo,
-    tags=['chat', 'novel'],
-    hf_dataset_id='zxbsmk/webnovel_cn')
-register_dataset(
-    DatasetName.generated_chat_zh,
-    'AI-ModelScope/generated_chat_0.4M', ['train'], [],
-    None,
-    get_dataset_from_repo,
-    tags=['chat', 'character-dialogue'],
-    hf_dataset_id='BelleGroup/generated_chat_0.4M')
-register_dataset(
-    DatasetName.wikipedia_zh,
-    'AI-ModelScope/wikipedia-cn-20230720-filtered', ['train'],
-    None,
-    RenameColumnsPreprocessor({'completion': 'response'}),
-    get_dataset_from_repo,
-    tags=['text-generation', 'general', 'pretrained'],
-    hf_dataset_id='pleisto/wikipedia-cn-20230720-filtered')
-register_dataset(
-    DatasetName.open_platypus_en,
-    'AI-ModelScope/Open-Platypus', ['train'],
-    None,
-    None,
-    get_dataset_from_repo,
-    tags=['chat', 'math'],
-    hf_dataset_id='garage-bAInd/Open-Platypus')
-register_dataset(
-    DatasetName.open_orca_gpt4,
-    'AI-ModelScope/OpenOrca', ['train'],
-    None,
-    RenameColumnsPreprocessor({'question': 'query'}),
-    get_dataset_from_repo,
-    tags=['chat', 'multilingual', 'general'])
-register_dataset(
-    DatasetName.open_orca,
-    'AI-ModelScope/OpenOrca', [['3_5M', 'train']],
-    None,
-    RenameColumnsPreprocessor({'question': 'query'}),
-    get_dataset_from_repo,
-    tags=['chat', 'multilingual', 'general'])
-
-register_dataset(
-    DatasetName.sharegpt_gpt4_mini,
-    'AI-ModelScope/sharegpt_gpt4', ['train'],
-    None,
-    ConversationsPreprocessor('human', 'gpt', error_strategy='delete'),
-    get_dataset_from_repo,
-    tags=['chat', 'multilingual', 'general', 'multi-round', 'gpt4', '🔥'])
-register_dataset(
-    DatasetName.sharegpt_gpt4,
-    'AI-ModelScope/sharegpt_gpt4', [[subset, 'train'] for subset in ['default', 'V3_format', 'zh_38K_format']],
-    None,
-    ConversationsPreprocessor('human', 'gpt', error_strategy='delete'),
-    get_dataset_from_repo,
-    tags=['chat', 'multilingual', 'general', 'multi-round'])
-
-register_dataset(
-    DatasetName.disc_med_sft_zh,
-    'AI-ModelScope/DISC-Med-SFT', ['train'],
-    None,
-    ConversationsPreprocessor(
-        conversations_key='conversation', from_key='role', value_key='content', error_strategy='delete'),
-    get_dataset_from_repo,
-    tags=['chat', 'medical', '🔥'],
-    hf_dataset_id='Flmc/DISC-Med-SFT')
-
-register_dataset(
-    DatasetName.disc_law_sft_zh,
-    'AI-ModelScope/DISC-Law-SFT', ['train'],
-    None,
-    RenameColumnsPreprocessor({
-        'input': 'query',
-        'output': 'response'
-    }),
-    get_dataset_from_repo,
-    tags=['chat', 'law', '🔥'],
-    hf_dataset_id='ShengbinYue/DISC-Law-SFT')
-
-register_dataset(
-    DatasetName.pileval,
-    'huangjintao/pile-val-backup', ['validation'],
-    None,
-    RenameColumnsPreprocessor({
-        'text': 'response',
-    }),
-    get_dataset_from_repo,
-    tags=['text-generation', 'awq'],
-    hf_dataset_id='mit-han-lab/pile-val-backup')
-
-
-def add_self_cognition_dataset(train_dataset: HfDataset, dataset_sample: int, model_name: Tuple[str, Optional[str]],
-                               model_author: Tuple[str, Optional[str]]) -> HfDataset:
-    assert model_name[0] is not None
-    assert model_author[0] is not None
-    if model_name[1] is None:
-        model_name = (model_name[0], model_name[0])
-    if model_author[1] is None:
-        model_author = (model_author[0], model_author[0])
-    dataset_path = os.path.join(os.path.dirname(os.path.dirname(__file__)), 'data', 'self_cognition.jsonl')
-    assert os.path.exists(dataset_path)
-    dataset = load_dataset_from_local([dataset_path], SmartPreprocessor())
-    response = []
-    for d in dataset:
-        if d['tag'] == 'zh':
-            model_n, model_a = model_name[0], model_author[0]
-        else:
-            model_n, model_a = model_name[1], model_author[1]
-
-        r = d['response'].replace('{{NAME}}', model_n).replace('{{AUTHOR}}', model_a)
-        response.append(r)
-    dataset = dataset.remove_columns('response').add_column('response', response).remove_columns('tag')
-
-    random_state = RandomState(42)
-    idx = random_state.permutation(len(dataset))[:dataset_sample]
-    dataset_sample -= len(idx)
-    if dataset_sample > 0:
-        idx2 = random_state.choice(len(dataset), dataset_sample)
-        idx = np.concatenate([idx, idx2], axis=0)
-    dataset = dataset.select(idx)
-    if train_dataset is None:
-        return dataset
-    else:
-        return concatenate_datasets([train_dataset, dataset])
-
-
 NoneType = type(None)
 
 
 def _check_dataset(dataset: Optional[None], check_dataset_strategy: Literal['none', 'discard', 'error',
                                                                             'warning']) -> HfDataset:
     if check_dataset_strategy == 'none' or dataset is None:
         return dataset
@@ -1490,57 +1105,199 @@
         idx_list.append(i)
     if is_modified:
         dataset = dataset.select(idx_list)
     assert len(dataset) > 0
     return dataset
 
 
+def _safe_split(s: str, sep: str, use_0: bool) -> Tuple[str, str]:
+    # use_0: When the length of the part is 1, is it considered as part0 or part1.
+    if s is None or len(s) == 0:
+        return None, None
+    part = s.split(sep)
+    if len(part) == 1:
+        if use_0:
+            part = part[0], None
+        else:
+            part = None, part[0]
+    else:
+        assert len(part) == 2
+    return part
+
+
+def parse_dataset_name(dataset_name: str) -> Tuple[bool, str, List[str], int]:
+    # HF::dataset_name:subset1/subset2/subset3#dataset_sample
+    use_hf, other = _safe_split(dataset_name, '::', False)
+    if use_hf is None:
+        use_hf = strtobool(os.environ.get('USE_HF', 'False'))
+    elif isinstance(use_hf, str):
+        use_hf = {'hf': 1, 'ms': 0}[use_hf.lower()]
+    part1, dataset_sample = _safe_split(other, '#', True)
+    dataset_name, subsets = _safe_split(part1, ':', True)
+    if subsets is not None:
+        subset_list = subsets.split('/')
+        subset_list = [subset.strip() for subset in subset_list]
+    else:
+        subset_list = None
+    if dataset_sample is None:
+        dataset_sample = -1
+    else:
+        dataset_sample = int(dataset_sample)
+    return tuple(t.strip() if isinstance(t, str) else t for t in [use_hf, dataset_name, subset_list, dataset_sample])
+
+
+def _dataset_name_exists(dataset_list: str, dataset_name: str) -> List[int]:
+    dataset_name = parse_dataset_name(dataset_name)[1]
+    cache_name_list = [parse_dataset_name(dataset)[1] for dataset in dataset_list]
+    res = []
+    for i, cache_name in enumerate(cache_name_list):
+        if cache_name == dataset_name:
+            res.append(i)
+    return res
+
+
+def _preprocess_self_cognition_dataset(
+    dataset_list: Tuple[HfDataset, Optional[HfDataset]],
+    model_name: Tuple[str, Optional[str]],
+    model_author: Tuple[str, Optional[str]],
+) -> Tuple[HfDataset, HfDataset]:
+    # model_name: Tuple[zh, en]
+    assert model_name[0] is not None
+    assert model_author[0] is not None
+    if len(model_name) == 1 or model_name[1] is None:
+        model_name = (model_name[0], model_name[0])
+    if len(model_author) == 1 or model_author[1] is None:
+        model_author = (model_author[0], model_author[0])
+    res_d_list = []
+    for dataset in dataset_list:
+        if dataset is None:
+            res_d_list.append(dataset)
+            continue
+        response = []
+        for d in dataset:
+            if d['tag'] == 'zh':
+                model_n, model_a = model_name[0], model_author[0]
+            else:
+                model_n, model_a = model_name[1], model_author[1]
+
+            r = d['response'].replace('{{NAME}}', model_n).replace('{{AUTHOR}}', model_a)
+            response.append(r)
+        dataset = dataset.remove_columns('response').add_column('response', response).remove_columns('tag')
+        res_d_list.append(dataset)
+    return tuple(res_d_list)
+
+
+def _dataset_id_to_name(dataset_name_list: List[str]) -> List[int]:
+    # register dataset_id (ms/hf). Convert dataset_id to dataset_name.
+    ms_dataset_mapping = {}
+    hf_dataset_mapping = {}
+    for k_name, container in zip(['dataset_id_or_path', 'hf_dataset_id'], [ms_dataset_mapping, hf_dataset_mapping]):
+        for k, v in DATASET_MAPPING.items():
+            if v.get(k_name) is None or not v.get('is_main', True):
+                continue
+            if v[k_name] not in container:
+                container[v[k_name]] = []
+            container[v[k_name]].append(k)
+
+    dataset_list = []
+    res_dataset = []
+    for d in dataset_name_list:
+        use_hf, d_name = parse_dataset_name(d)[:2]
+        if '/' in d_name:
+            dataset_list.append((d, use_hf, d_name))
+        else:
+            res_dataset.append(d)
+
+    extra_dataset = []
+    for d, use_hf, d_name in dataset_list:
+        dataset_mapping = hf_dataset_mapping if use_hf else ms_dataset_mapping
+        if d_name in dataset_mapping:
+            for d_name2 in dataset_mapping[d_name]:
+                res_dataset.append(d.replace(d_name, d_name2))
+        else:
+            extra_dataset.append((d, use_hf, d_name))
+
+    for i, (d, use_hf, d_name) in enumerate(extra_dataset):
+        d_info = {}
+        d_name2 = f'_{i}'
+        if os.path.isfile(d_name):
+            d_info['dataset_path'] = d_name
+        else:
+            if use_hf:
+                d_info['hf_dataset_id'] = d_name
+            else:
+                d_info['dataset_id'] = d_name
+        register_dataset_info(d_name2, d_info)
+        res_dataset.append(d.replace(d_name, d_name2))
+    return res_dataset
+
+
 def get_dataset(
-    dataset_name_list: Union[List[str], str],
-    dataset_test_ratio: float = 0.,
-    dataset_seed: Union[RandomState, int] = 42,
-    check_dataset_strategy: Literal['none', 'discard', 'error', 'warning'] = 'none',
-) -> Tuple[HfDataset, Optional[HfDataset]]:
+        dataset_name_list: Union[List[str], str],
+        dataset_test_ratio: float = 0.,
+        dataset_seed: Union[int, RandomState] = 42,
+        check_dataset_strategy: Literal['none', 'discard', 'error', 'warning'] = 'none',
+        *,
+        # for self-cognition
+        model_name: Optional[Tuple[str, str]] = None,
+        model_author: Optional[Tuple[str, str]] = None) -> Tuple[HfDataset, Optional[HfDataset]]:
     """Returns train_dataset and val_dataset"""
     if isinstance(dataset_name_list, str):
         dataset_name_list = [dataset_name_list]
     train_dataset_list: List[HfDataset] = []
     val_dataset_list: List[HfDataset] = []
-    random_state = dataset_seed
-    if isinstance(dataset_seed, int):
-        random_state = RandomState(dataset_seed)
+
+    dataset_name_list = _dataset_id_to_name(dataset_name_list)
     for dataset_name in dataset_name_list:
+        use_hf, dataset_name, subsets, dataset_sample = parse_dataset_name(dataset_name)
         dataset_info = DATASET_MAPPING[dataset_name]
-        use_hf = strtobool(os.environ.get('USE_HF', 'False'))
-        dataset_str_f = 'Downloading the dataset from {hub}, dataset_id: {dataset_id}'
-        if use_hf:
-            dataset_id_or_path = dataset_info['hf_dataset_id']
-            dataset_str = dataset_str_f.format(hub='HuggingFace', dataset_id=dataset_id_or_path)
+        if subsets is None:
+            subsets = dataset_info['subsets']
+        if dataset_sample == -1:
+            dataset_sample = dataset_info.get('dataset_sample', -1)
+        if isinstance(dataset_seed, int):
+            random_state = RandomState(dataset_seed)
         else:
-            dataset_id_or_path = dataset_info['dataset_id_or_path']
-            dataset_str = dataset_str_f.format(hub='ModelScope', dataset_id=dataset_id_or_path)
-        logger.info(dataset_str)
-        assert dataset_id_or_path is not None, (f'dataset_name: {dataset_name}, use_hf: {use_hf}, '
-                                                f'dataset_id_or_path: {dataset_id_or_path}.')
+            random_state = dataset_seed
+
         get_function: GetDatasetFunction = dataset_info['get_function']
+        is_local = dataset_info.get('is_local', False)
+        dataset_id_or_path = dataset_info['dataset_id_or_path']
+        remove_useless_columns = dataset_info.get('remove_useless_columns', True)
+
+        if not is_local:
+            dataset_str_f = 'Downloading the dataset from {hub}, dataset_id: {dataset_id}'
+            if use_hf:
+                dataset_id_or_path = dataset_info['hf_dataset_id']
+                dataset_str = dataset_str_f.format(hub='HuggingFace', dataset_id=dataset_id_or_path)
+            else:
+                dataset_str = dataset_str_f.format(hub='ModelScope', dataset_id=dataset_id_or_path)
+            logger.info(dataset_str)
+            assert dataset_id_or_path is not None, (f'dataset_name: {dataset_name}, use_hf: {use_hf}, '
+                                                    f'dataset_id_or_path: {dataset_id_or_path}.')
         dataset = get_function(
             dataset_id_or_path,
-            train_subset_split_list=dataset_info['train_subset_split_list'],
-            val_subset_split_list=dataset_info['val_subset_split_list'],
-            preprocess_func=dataset_info['preprocess_func'],
+            subsets,
+            dataset_info['preprocess_func'],
+            dataset_info['split'],
+            dataset_sample,
+            random_state=random_state,
+            dataset_test_ratio=dataset_test_ratio,
+            remove_useless_columns=remove_useless_columns,
             use_hf=use_hf)
+
+        if dataset_name == 'self-cognition':
+            assert model_name is not None and model_author is not None
+            dataset = _preprocess_self_cognition_dataset(dataset, model_name, model_author)
         train_d: HfDataset
         if isinstance(dataset, (list, tuple)):
             train_d, val_d = dataset
         else:
             train_d, val_d = dataset, None
         assert train_d is not None or val_d is not None
-        if val_d is None and dataset_test_ratio > 0:
-            dataset_dict = train_d.train_test_split(dataset_test_ratio, seed=get_seed(random_state))
-            train_d, val_d = dataset_dict['train'], dataset_dict['test']
         if train_d is not None:
             train_dataset_list.append(train_d)
         if val_d is not None:
             val_dataset_list.append(val_d)
 
     train_dataset = None
     if len(train_dataset_list) > 0:
@@ -1581,13 +1338,44 @@
                              '`https://github.com/modelscope/swift/blob/main/docs/source/LLM/自定义与拓展.md#注册数据集的方式` '
                              'for more information.')
         dataset = HfDataset.from_dict(df.to_dict(orient='list'))
         dataset_list.append(preprocess_func(dataset))
     return concatenate_datasets(dataset_list)
 
 
-def get_custom_dataset(_: str, train_subset_split_list: Union[str, List[str]],
-                       val_subset_split_list: Optional[Union[str, List[str]]], preprocess_func: PreprocessFunc,
-                       **kwargs) -> Tuple[HfDataset, Optional[HfDataset]]:
-    train_dataset = load_dataset_from_local(train_subset_split_list, preprocess_func)
-    val_dataset = load_dataset_from_local(val_subset_split_list, preprocess_func)
-    return train_dataset, val_dataset
+def get_local_dataset(_1: str,
+                      _2: Optional[List[str]],
+                      preprocess_func: PreprocessFunc,
+                      split: List[str],
+                      dataset_sample: int = -1,
+                      random_state: Optional[RandomState] = None,
+                      dataset_test_ratio: float = 0.,
+                      remove_useless_columns: bool = True,
+                      **kwargs) -> Tuple[HfDataset, Optional[HfDataset]]:
+    dataset = load_dataset_from_local(split, preprocess_func)
+    return _post_preprocess(dataset, dataset_sample, random_state, None, dataset_test_ratio, remove_useless_columns)
+
+
+def register_dataset_info_file(dataset_info_path: Optional[str] = None) -> None:
+    # dataset_info_path: path, json or None
+    if dataset_info_path is None:
+        dataset_info_path = os.path.abspath(os.path.join(__file__, '..', '..', 'data', 'dataset_info.json'))
+    if isinstance(dataset_info_path, str):
+        if os.path.isfile(dataset_info_path):
+            with open(dataset_info_path, 'r') as f:
+                dataset_info = json.load(f)
+            base_dir = os.path.dirname(dataset_info_path)
+        else:
+            dataset_info = json.loads(dataset_info_path)
+            dataset_info_path = list(dataset_info.keys())
+            base_dir = None
+    else:
+        assert isinstance(dataset_info_path, dict)
+        dataset_info = deepcopy(dataset_info_path)
+        dataset_info_path = list(dataset_info.keys())
+        base_dir = None
+    for dataset_name, d_info in dataset_info.items():
+        register_dataset_info(dataset_name, d_info, base_dir=base_dir)
+    logger.info(f'Successfully registered `{dataset_info_path}`')
+
+
+register_dataset_info_file()
```

### Comparing `ms-swift-2.0.4/swift/llm/utils/model.py` & `ms-swift-2.0.5/swift/llm/utils/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,19 @@
 from torch import Tensor
 from torch import dtype as Dtype
 from transformers import PretrainedConfig, PreTrainedModel, PreTrainedTokenizerBase
 from transformers.dynamic_module_utils import get_class_from_dynamic_module
 from transformers.models.auto.tokenization_auto import get_tokenizer_config
 from transformers.utils import strtobool
 from transformers.utils.versions import require_version
-from trl.import_utils import is_unsloth_available
 
 from swift import get_logger
-from swift.utils import get_dist_setting, is_dist, is_local_master, safe_ddp_context, subprocess_run, use_torchacc
+from swift.utils import get_dist_setting, safe_ddp_context, subprocess_run, use_torchacc
 from .template import TemplateType
-from .utils import get_max_model_len
+from .utils import get_max_model_len, is_unsloth_available
 
 logger = get_logger()
 
 # Model Home: 'https://modelscope.cn/models/{model_id_or_path}/summary'
 MODEL_MAPPING: Dict[str, Dict[str, Any]] = {}
 
 
@@ -157,30 +156,47 @@
     llama_3_chinese_8b_instruct = 'llama-3-chinese-8b-instruct'
     # atom
     atom_7b = 'atom-7b'
     atom_7b_chat = 'atom-7b-chat'
     # llava
     llava1d6_mistral_7b_instruct = 'llava1d6-mistral-7b-instruct'
     llava1d6_yi_34b_instruct = 'llava1d6-yi-34b-instruct'
+    llama3_llava_next_8b = 'llama3-llava-next-8b'
+    llava_next_72b = 'llava-next-72b'
+    llava_next_110b = 'llava-next-110b'
     # yi
     yi_6b = 'yi-6b'
     yi_6b_200k = 'yi-6b-200k'
     yi_6b_chat = 'yi-6b-chat'
     yi_6b_chat_awq = 'yi-6b-chat-awq'
     yi_6b_chat_int8 = 'yi-6b-chat-int8'
     yi_9b = 'yi-9b'
     yi_9b_200k = 'yi-9b-200k'
     yi_34b = 'yi-34b'
     yi_34b_200k = 'yi-34b-200k'
     yi_34b_chat = 'yi-34b-chat'
     yi_34b_chat_awq = 'yi-34b-chat-awq'
     yi_34b_chat_int8 = 'yi-34b-chat-int8'
+    yi_1_5_6b = 'yi-1_5-6b'
+    yi_1_5_6b_chat = 'yi-1_5-6b-chat'
+    yi_1_5_6b_chat_awq_int4 = 'yi-1_5-6b-chat-awq-int4'
+    yi_1_5_6b_chat_gptq_int4 = 'yi-1_5-6b-chat-gptq-int4'
+    yi_1_5_9b_chat_awq_int4 = 'yi-1_5-9b-chat-awq-int4'
+    yi_1_5_9b_chat_gptq_int4 = 'yi-1_5-9b-chat-gptq-int4'
+    yi_1_5_34b_chat_awq_int4 = 'yi-1_5-34b-chat-awq-int4'
+    yi_1_5_34b_chat_gptq_int4 = 'yi-1_5-34b-chat-gptq-int4'
+    yi_1_5_9b = 'yi-1_5-9b'
+    yi_1_5_9b_chat = 'yi-1_5-9b-chat'
+    yi_1_5_34b = 'yi-1_5-34b'
+    yi_1_5_34b_chat = 'yi-1_5-34b-chat'
     # yi-vl
     yi_vl_6b_chat = 'yi-vl-6b-chat'
     yi_vl_34b_chat = 'yi-vl-34b-chat'
+    # llava-llama
+    llava_llama3_8b_v1_1 = 'llava-llama-3-8b-v1_1'
     # internlm
     internlm_7b = 'internlm-7b'
     internlm_7b_chat = 'internlm-7b-chat'
     internlm_7b_chat_8k = 'internlm-7b-chat-8k'
     internlm_20b = 'internlm-20b'
     internlm_20b_chat = 'internlm-20b-chat'
     # internlm2
@@ -200,14 +216,15 @@
     internlm2_math_7b_chat = 'internlm2-math-7b-chat'
     internlm2_math_20b = 'internlm2-math-20b'
     internlm2_math_20b_chat = 'internlm2-math-20b-chat'
     # internlm-xcomposer2
     internlm_xcomposer2_7b_chat = 'internlm-xcomposer2-7b-chat'
     # internvl
     internvl_chat_v1_5 = 'internvl-chat-v1_5'
+    internvl_chat_v1_5_int8 = 'internvl-chat-v1_5-int8'
     # deepseek
     deepseek_7b = 'deepseek-7b'
     deepseek_7b_chat = 'deepseek-7b-chat'
     deepseek_moe_16b = 'deepseek-moe-16b'
     deepseek_moe_16b_chat = 'deepseek-moe-16b-chat'
     deepseek_67b = 'deepseek-67b'
     deepseek_67b_chat = 'deepseek-67b-chat'
@@ -221,28 +238,33 @@
     # deepseek-math
     deepseek_math_7b = 'deepseek-math-7b'
     deepseek_math_7b_instruct = 'deepseek-math-7b-instruct'
     deepseek_math_7b_chat = 'deepseek-math-7b-chat'
     # deepseek-vl
     deepseek_vl_1_3b_chat = 'deepseek-vl-1_3b-chat'
     deepseek_vl_7b_chat = 'deepseek-vl-7b-chat'
+    # deepseek-v2
+    deepseek_v2_chat = 'deepseek-v2-chat'
+    deepseek_v2_lite = 'deepseek-v2-lite'
+    deepseek_v2_lite_chat = 'deepseek-v2-lite-chat'
     # gemma
     gemma_2b = 'gemma-2b'
     gemma_7b = 'gemma-7b'
     gemma_2b_instruct = 'gemma-2b-instruct'
     gemma_7b_instruct = 'gemma-7b-instruct'
     # minicpm
     minicpm_1b_sft_chat = 'minicpm-1b-sft-chat'
     minicpm_2b_sft_chat = 'minicpm-2b-sft-chat'
     minicpm_2b_chat = 'minicpm-2b-chat'
     minicpm_2b_128k = 'minicpm-2b-128k'
     minicpm_moe_8x2b = 'minicpm-moe-8x2b'
     # minicpm-v
     minicpm_v_3b_chat = 'minicpm-v-3b-chat'
-    minicpm_v_v2 = 'minicpm-v-v2'
+    minicpm_v_v2_chat = 'minicpm-v-v2-chat'
+    minicpm_v_v2_5_chat = 'minicpm-v-v2_5-chat'
     # openbuddy
     openbuddy_llama2_13b_chat = 'openbuddy-llama2-13b-chat'
     openbuddy_llama3_8b_chat = 'openbuddy-llama3-8b-chat'
     openbuddy_llama2_65b_chat = 'openbuddy-llama-65b-chat'
     openbuddy_llama2_70b_chat = 'openbuddy-llama2-70b-chat'
     openbuddy_mistral_7b_chat = 'openbuddy-mistral-7b-chat'
     openbuddy_zephyr_7b_chat = 'openbuddy-zephyr-7b-chat'
@@ -319,27 +341,31 @@
     codefuse_codegeex2_6b_chat = 'codefuse-codegeex2-6b-chat'
     codefuse_qwen_14b_chat = 'codefuse-qwen-14b-chat'
     # phi
     phi2_3b = 'phi2-3b'
     phi3_4b_4k_instruct = 'phi3-4b-4k-instruct'
     phi3_4b_128k_instruct = 'phi3-4b-128k-instruct'
     # cogagent
-    cogvlm_17b_instruct = 'cogvlm-17b-instruct'
+    cogvlm_17b_chat = 'cogvlm-17b-chat'
+    cogvlm2_19b_chat = 'cogvlm2-19b-chat'  # chinese
+    cogvlm2_en_19b_chat = 'cogvlm2-en-19b-chat'
     cogagent_18b_chat = 'cogagent-18b-chat'
     cogagent_18b_instruct = 'cogagent-18b-instruct'
     # mamba
     mamba_130m = 'mamba-130m'
     mamba_370m = 'mamba-370m'
     mamba_390m = 'mamba-390m'
     mamba_790m = 'mamba-790m'
     mamba_1_4b = 'mamba-1.4b'
     mamba_2_8b = 'mamba-2.8b'
     # teleAI
     telechat_7b = 'telechat-7b'
     telechat_12b = 'telechat-12b'
+    telechat_12b_v2 = 'telechat-12b-v2'
+    telechat_12b_v2_gptq_int4 = 'telechat-12b-v2-gptq-int4'
     # grok-1
     grok_1 = 'grok-1'
     # dbrx
     dbrx_instruct = 'dbrx-instruct'
     dbrx_base = 'dbrx-base'
     # mengzi
     mengzi3_13b_base = 'mengzi3-13b-base'
@@ -388,14 +414,21 @@
         'v_proj.multiway.0',
         'v_proj.multiway.1',
     ]
     mplug_owl2d1 = [
         'c_attn.multiway.0',
         'c_attn.multiway.1',
     ]
+    deepseek2 = [
+        'q_a_proj',
+        'q_b_proj',
+        'kv_a_proj_with_mqa',
+        'kv_b_proj',
+        'o_proj',
+    ]
 
 
 GetModelTokenizerFunction = Callable[..., Tuple[Optional[PreTrainedModel], PreTrainedTokenizerBase]]
 
 
 def register_model(
         model_type: str,
@@ -406,18 +439,18 @@
         *,
         requires: Optional[List[str]] = None,
         torch_dtype: Optional[Dtype] = None,
         hf_model_id: Optional[str] = None,
         revision: Optional[str] = None,  # only modelscope
         ignore_file_pattern: Optional[List[str]] = None,
         function_kwargs: Optional[Dict[str, Any]] = None,
-        exists_ok: bool = False,
+        exist_ok: bool = False,
         eos_token: Optional[str] = None,
         **kwargs) -> Optional[Callable[[GetModelTokenizerFunction], GetModelTokenizerFunction]]:
-    if not exists_ok and model_type in MODEL_MAPPING:
+    if not exist_ok and model_type in MODEL_MAPPING:
         raise ValueError(f'The `{model_type}` has already been registered in the MODEL_MAPPING.')
     if requires is None:
         requires = []
     if function_kwargs is None:
         function_kwargs = {}
     if revision is None:
         revision = 'master'
@@ -484,14 +517,30 @@
 
     if not hasattr(QuantLinear, '__old_forward'):  # avoid double patching
         QuantLinear.__old_forward = __old_forward
         QuantLinear.forward = _new_forward
 
 
 @register_model(
+    ModelType.cogvlm2_en_19b_chat,
+    'ZhipuAI/cogvlm2-llama3-chat-19B',
+    LoRATM.cogvlm,
+    TemplateType.cogvlm,
+    support_gradient_checkpointing=False,
+    pad_token='<|reserved_special_token_0|>',
+    hf_model_id='THUDM/cogvlm2-llama3-chat-19B')
+@register_model(
+    ModelType.cogvlm2_19b_chat,
+    'ZhipuAI/cogvlm2-llama3-chinese-chat-19B',
+    LoRATM.cogvlm,
+    TemplateType.cogvlm,
+    support_gradient_checkpointing=False,
+    pad_token='<|reserved_special_token_0|>',
+    hf_model_id='THUDM/cogvlm2-llama3-chinese-chat-19B')
+@register_model(
     ModelType.atom_7b,
     'FlagAlpha/Atom-7B',
     LoRATM.llama2,
     TemplateType.default_generation,
     support_flash_attn=True,
     support_vllm=True,
     hf_model_id='FlagAlpha/Atom-7B')
@@ -778,18 +827,24 @@
     if torch_dtype is not None:
         model_config.torch_dtype = torch_dtype
     if tokenizer is None:
         tokenizer = AutoTokenizer.from_pretrained(model_dir, trust_remote_code=True)
     eos_token = kwargs.get('eos_token')
     if eos_token is not None:
         tokenizer.eos_token = eos_token
+    pad_token = kwargs.get('pad_token')
+    if pad_token is not None:
+        tokenizer.pad_token = pad_token
     model = None
     if load_model:
         if kwargs.get('use_unsloth', False):
             assert is_unsloth_available(), 'please install unsloth if using `use_unsloth=True`'
+            if 'qwen' in model_dir:
+                logger.warn('If using qwen2 models, please install unsloth with '
+                            '`pip install git+https://github.com/yangjianxin1/unsloth`')
             from unsloth import FastLanguageModel
             model, tokenizer = FastLanguageModel.from_pretrained(
                 model_name=model_dir,
                 max_seq_length=kwargs.get('max_length', None),
                 dtype=torch_dtype,
                 load_in_4bit=kwargs.get('load_in_4bit', True),
                 trust_remote_code=True,
@@ -802,14 +857,44 @@
             model.is_awq = is_awq
         if load_model and gptq_bits > 0:
             model.gptq_bits = gptq_bits
     return model, tokenizer
 
 
 @register_model(
+    ModelType.llava_llama3_8b_v1_1,
+    'AI-ModelScope/llava-llama-3-8b-v1_1-transformers',
+    LoRATM.llama2,
+    TemplateType.llava_llama_instruct,
+    support_flash_attn=True,
+    requires=['transformers>=4.36'],
+    tags=['multi-modal', 'vision'],
+    hf_model_id='xtuner/llava-llama-3-8b-v1_1-transformers')
+def get_model_tokenizer_llava_llama(model_dir: str,
+                                    torch_dtype: Dtype,
+                                    model_kwargs: Dict[str, Any],
+                                    load_model: bool = True,
+                                    **kwargs):
+    from transformers import LlavaForConditionalGeneration, LlavaConfig, AutoProcessor
+
+    model_config = LlavaConfig.from_pretrained(model_dir)
+    processor = AutoProcessor.from_pretrained(model_dir)
+    model, tokenizer = get_model_tokenizer_with_flash_attn(
+        model_dir,
+        torch_dtype,
+        model_kwargs,
+        load_model,
+        model_config=model_config,
+        automodel_class=LlavaForConditionalGeneration,
+        **kwargs)
+    model.processor = processor
+    return model, tokenizer
+
+
+@register_model(
     ModelType.grok_1,
     'colossalai/grok-1-pytorch',
     LoRATM.grok_1,
     TemplateType.default_generation,
     support_vllm=False,
     support_flash_attn=False,
     hf_model_id='hpcai-tech/grok-1')
@@ -893,18 +978,18 @@
                               **kwargs):
     logger.info('[IMPORTANT] Remember installing causal-conv1d>=1.2.0 and mamba-ssm, or you training and inference will'
                 'be really slow!')
     return get_model_tokenizer_from_repo(model_dir, torch_dtype, model_kwargs, load_model, **kwargs)
 
 
 @register_model(
-    ModelType.cogvlm_17b_instruct,
+    ModelType.cogvlm_17b_chat,
     'ZhipuAI/cogvlm-chat',
     LoRATM.cogvlm,
-    TemplateType.cogvlm_instruct,
+    TemplateType.cogvlm,
     support_gradient_checkpointing=False,
     tags=['multi-modal', 'vision'],
     hf_model_id='THUDM/cogvlm-chat-hf')
 @register_model(
     ModelType.cogagent_18b_chat,
     'ZhipuAI/cogagent-chat',
     LoRATM.cogagent,
@@ -1673,14 +1758,128 @@
     '01ai/Yi-6B',
     LoRATM.llama2,
     TemplateType.default_generation,
     support_flash_attn=True,
     support_vllm=True,
     hf_model_id='01-ai/Yi-6B')
 @register_model(
+    ModelType.yi_1_5_6b,
+    '01ai/Yi-1.5-6B',
+    LoRATM.llama2,
+    TemplateType.default_generation,
+    support_flash_attn=True,
+    support_vllm=True,
+    hf_model_id='01-ai/Yi-1.5-6B')
+@register_model(
+    ModelType.yi_1_5_6b_chat,
+    '01ai/Yi-1.5-6B-Chat',
+    LoRATM.llama2,
+    TemplateType.yi1_5,
+    support_flash_attn=True,
+    support_vllm=True,
+    hf_model_id='01-ai/Yi-1.5-6B-Chat')
+@register_model(
+    ModelType.yi_1_5_6b_chat_awq_int4,
+    'AI-ModelScope/Yi-1.5-6B-Chat-AWQ',
+    LoRATM.llama2,
+    TemplateType.yi1_5,
+    requires=['autoawq'],
+    torch_dtype=torch.float16,
+    function_kwargs={'is_awq': True},
+    support_flash_attn=True,
+    hf_model_id='modelscope/Yi-1.5-6B-Chat-AWQ',
+    support_vllm=True)
+@register_model(
+    ModelType.yi_1_5_6b_chat_gptq_int4,
+    'AI-ModelScope/Yi-1.5-6B-Chat-GPTQ',
+    LoRATM.llama2,
+    TemplateType.yi1_5,
+    requires=['auto_gptq>=0.5'],
+    function_kwargs={'gptq_bits': 4},
+    torch_dtype=torch.float16,
+    support_flash_attn=True,
+    hf_model_id='modelscope/Yi-1.5-6B-Chat-GPTQ',
+    support_vllm=True)
+@register_model(
+    ModelType.yi_1_5_9b_chat_awq_int4,
+    'AI-ModelScope/Yi-1.5-9B-Chat-AWQ',
+    LoRATM.llama2,
+    TemplateType.yi1_5,
+    requires=['autoawq'],
+    torch_dtype=torch.float16,
+    function_kwargs={'is_awq': True},
+    support_flash_attn=True,
+    hf_model_id='modelscope/Yi-1.5-9B-Chat-AWQ',
+    support_vllm=True)
+@register_model(
+    ModelType.yi_1_5_9b_chat_gptq_int4,
+    'AI-ModelScope/Yi-1.5-9B-Chat-GPTQ',
+    LoRATM.llama2,
+    TemplateType.yi1_5,
+    requires=['auto_gptq>=0.5'],
+    function_kwargs={'gptq_bits': 4},
+    torch_dtype=torch.float16,
+    support_flash_attn=True,
+    hf_model_id='modelscope/Yi-1.5-9B-Chat-GPTQ',
+    support_vllm=True)
+@register_model(
+    ModelType.yi_1_5_34b_chat_awq_int4,
+    'AI-ModelScope/Yi-1.5-34B-Chat-AWQ',
+    LoRATM.llama2,
+    TemplateType.yi1_5,
+    requires=['autoawq'],
+    torch_dtype=torch.float16,
+    function_kwargs={'is_awq': True},
+    support_flash_attn=True,
+    hf_model_id='modelscope/Yi-1.5-34B-Chat-AWQ',
+    support_vllm=True)
+@register_model(
+    ModelType.yi_1_5_34b_chat_gptq_int4,
+    'AI-ModelScope/Yi-1.5-34B-Chat-GPTQ',
+    LoRATM.llama2,
+    TemplateType.yi1_5,
+    requires=['auto_gptq>=0.5'],
+    function_kwargs={'gptq_bits': 4},
+    torch_dtype=torch.float16,
+    support_flash_attn=True,
+    hf_model_id='modelscope/Yi-1.5-34B-Chat-GPTQ',
+    support_vllm=True)
+@register_model(
+    ModelType.yi_1_5_9b,
+    '01ai/Yi-1.5-9B',
+    LoRATM.llama2,
+    TemplateType.default_generation,
+    support_flash_attn=True,
+    support_vllm=True,
+    hf_model_id='01-ai/Yi-1.5-9B')
+@register_model(
+    ModelType.yi_1_5_9b_chat,
+    '01ai/Yi-1.5-9B-Chat',
+    LoRATM.llama2,
+    TemplateType.yi1_5,
+    support_flash_attn=True,
+    support_vllm=True,
+    hf_model_id='01-ai/Yi-1.5-9B-Chat')
+@register_model(
+    ModelType.yi_1_5_34b,
+    '01ai/Yi-1.5-34B',
+    LoRATM.llama2,
+    TemplateType.default_generation,
+    support_flash_attn=True,
+    support_vllm=True,
+    hf_model_id='01-ai/Yi-1.5-34B')
+@register_model(
+    ModelType.yi_1_5_34b_chat,
+    '01ai/Yi-1.5-34B-Chat',
+    LoRATM.llama2,
+    TemplateType.yi1_5,
+    support_flash_attn=True,
+    support_vllm=True,
+    hf_model_id='01-ai/Yi-1.5-34B-Chat')
+@register_model(
     ModelType.ziya2_13b_chat,
     'Fengshenbang/Ziya2-13B-Chat',
     LoRATM.llama2,
     TemplateType.ziya,
     support_flash_attn=True,
     support_vllm=True,
     hf_model_id='IDEA-CCNL/Ziya2-13B-Chat')
@@ -2062,14 +2261,15 @@
     'qwen/Qwen1.5-0.5B-Chat-GPTQ-Int8',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
     function_kwargs={'gptq_bits': 8},
     support_flash_attn=True,
+    support_vllm=True,
     hf_model_id='Qwen/Qwen1.5-0.5B-Chat-GPTQ-Int8')
 @register_model(
     ModelType.qwen1half_1_8b_chat_int4,
     'qwen/Qwen1.5-1.8B-Chat-GPTQ-Int4',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
@@ -2083,14 +2283,15 @@
     'qwen/Qwen1.5-1.8B-Chat-GPTQ-Int8',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
     function_kwargs={'gptq_bits': 8},
     support_flash_attn=True,
+    support_vllm=True,
     hf_model_id='Qwen/Qwen1.5-1.8B-Chat-GPTQ-Int8')
 @register_model(
     ModelType.qwen1half_4b_chat_int4,
     'qwen/Qwen1.5-4B-Chat-GPTQ-Int4',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
@@ -2104,14 +2305,15 @@
     'qwen/Qwen1.5-4B-Chat-GPTQ-Int8',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
     function_kwargs={'gptq_bits': 8},
     support_flash_attn=True,
+    support_vllm=True,
     hf_model_id='Qwen/Qwen1.5-4B-Chat-GPTQ-Int8')
 @register_model(
     ModelType.qwen1half_7b_chat_int4,
     'qwen/Qwen1.5-7B-Chat-GPTQ-Int4',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
@@ -2125,14 +2327,15 @@
     'qwen/Qwen1.5-7B-Chat-GPTQ-Int8',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
     function_kwargs={'gptq_bits': 8},
     support_flash_attn=True,
+    support_vllm=True,
     hf_model_id='Qwen/Qwen1.5-7B-Chat-GPTQ-Int8')
 @register_model(
     ModelType.qwen1half_14b_chat_int4,
     'qwen/Qwen1.5-14B-Chat-GPTQ-Int4',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
@@ -2146,14 +2349,15 @@
     'qwen/Qwen1.5-14B-Chat-GPTQ-Int8',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
     function_kwargs={'gptq_bits': 8},
     support_flash_attn=True,
+    support_vllm=True,
     hf_model_id='Qwen/Qwen1.5-14B-Chat-GPTQ-Int8')
 @register_model(
     ModelType.qwen1half_32b_chat_int4,
     'qwen/Qwen1.5-32B-Chat-GPTQ-Int4',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
@@ -2189,14 +2393,15 @@
     'qwen/Qwen1.5-72B-Chat-GPTQ-Int8',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.37'],
     torch_dtype=torch.float16,
     function_kwargs={'gptq_bits': 8},
     support_flash_attn=True,
+    support_vllm=True,
     hf_model_id='Qwen/Qwen1.5-72B-Chat-GPTQ-Int8')
 @register_model(
     ModelType.qwen1half_moe_a2_7b_chat_int4,
     'qwen/Qwen1.5-MoE-A2.7B-Chat-GPTQ-Int4',
     LoRATM.qwen1half,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5', 'transformers>=4.40'],
@@ -2377,56 +2582,142 @@
         if getattr(tokenizer.__class__.eos_token_id, 'fset', None) is None:
             del tokenizer.__class__.eos_token_id
         tokenizer.eos_token = eos_token
 
     return model, tokenizer
 
 
+@register_model(
+    ModelType.deepseek_v2_lite,
+    'deepseek-ai/DeepSeek-V2-Lite',
+    LoRATM.deepseek2,
+    TemplateType.default_generation,
+    support_gradient_checkpointing=False,
+    support_flash_attn=True,
+    support_vllm=True,
+    requires=['transformers>=4.39.3'],
+    hf_model_id='deepseek-ai/DeepSeek-V2-Lite')
+@register_model(
+    ModelType.deepseek_v2_lite_chat,
+    'deepseek-ai/DeepSeek-V2-Lite-Chat',
+    LoRATM.deepseek2,
+    TemplateType.deepseek2,
+    support_gradient_checkpointing=False,
+    support_flash_attn=True,
+    support_vllm=True,
+    requires=['transformers>=4.39.3'],
+    hf_model_id='deepseek-ai/DeepSeek-V2-Lite-Chat')
+@register_model(
+    ModelType.deepseek_v2_chat,
+    'deepseek-ai/DeepSeek-V2-Chat',
+    LoRATM.deepseek2,
+    TemplateType.deepseek2,
+    support_gradient_checkpointing=False,
+    support_flash_attn=True,
+    support_vllm=True,
+    requires=['transformers>=4.39.3'],
+    hf_model_id='deepseek-ai/DeepSeek-V2-Chat')
+def get_model_tokenizer_deepseek2(model_dir: str,
+                                  torch_dtype: Dtype,
+                                  model_kwargs: Dict[str, Any],
+                                  load_model: bool = True,
+                                  **kwargs):
+    model_config = AutoConfig.from_pretrained(model_dir, trust_remote_code=True)
+    use_flash_attn = kwargs.pop('use_flash_attn', False)
+    model_config._attn_implementation = 'flash_attention_2' if use_flash_attn else 'eager'
+    model, tokenizer = get_model_tokenizer_from_repo(
+        model_dir, torch_dtype, model_kwargs, load_model, model_config=model_config, **kwargs)
+    if model is not None:
+        model.generation_config.pad_token_id = model.generation_config.eos_token_id
+        # fix dtype bug
+        model.generation_config.pad_token_id = model.generation_config.eos_token_id
+        mlp_cls = model.model.layers[1].mlp.__class__
+        for module in model.modules():
+            if isinstance(module, mlp_cls):
+                if not hasattr(module, '__old_forward'):  # Avoid double patching
+                    __old_forward = module._old_forward if hasattr(module, '_old_forward') else module.forward
+
+                    def _new_forward(hidden_states, *, __old_forward) -> Tensor:
+                        dtype = hidden_states.dtype
+                        return __old_forward(hidden_states).to(dtype)
+
+                    _new_forward = partial(_new_forward, __old_forward=__old_forward)
+                    if hasattr(module, '_old_forward'):  # device_map
+                        module._old_forward = _new_forward
+                    else:
+                        module.forward = _new_forward
+                    module.__old_forward = __old_forward
+    return model, tokenizer
+
+
 def fix_internvl_inplace_bug(model) -> None:
 
     embedding = model.language_model.get_input_embeddings()
     if not hasattr(embedding, '__old_forward'):  # Avoid double patching
-        if hasattr(embedding, '_old_forward'):  # device_map
-            __old_forward = embedding._old_forward
-            embedding._old_forward = lambda *args, **kwargs: __old_forward(*args, **kwargs).requires_grad_(True).clone()
-        else:
-            __old_forward = embedding.forward
-            embedding.forward = lambda *args, **kwargs: __old_forward(*args, **kwargs).requires_grad_(True).clone()
-        embedding.__old_forward = __old_forward
+        old_forward = embedding.forward
+
+        @wraps(old_forward)
+        def _new_forward(*args, **kwargs):
+            device = args[0].device
+            return old_forward(*args, **kwargs).requires_grad_(True).clone().to(device)
+
+        embedding.__old_forward = old_forward
+        embedding.forward = _new_forward
 
 
 @register_model(
     ModelType.internvl_chat_v1_5,
     'AI-ModelScope/InternVL-Chat-V1-5',
     LoRATM.internlm2,
     TemplateType.internvl,
-    requires=['transformers>=4.35'],
+    requires=['transformers>=4.35', 'timm'],
     support_flash_attn=True,
     support_gradient_checkpointing=False,
     hf_model_id='OpenGVLab/InternVL-Chat-V1-5')
+@register_model(
+    ModelType.internvl_chat_v1_5_int8,
+    'AI-ModelScope/InternVL-Chat-V1-5-int8',
+    LoRATM.internlm2,
+    TemplateType.internvl,
+    requires=['transformers>=4.35', 'timm'],
+    support_flash_attn=True,
+    support_gradient_checkpointing=False,
+    hf_model_id='OpenGVLab/InternVL-Chat-V1-5-int8')
 def get_model_tokenizer_internvl(model_dir: str,
                                  torch_dtype: Dtype,
                                  model_kwargs: Dict[str, Any],
                                  load_model: bool = True,
                                  **kwargs):
-
     model_config = AutoConfig.from_pretrained(model_dir, trust_remote_code=True)
     use_flash_attn = kwargs.pop('use_flash_attn', False)
-    if use_flash_attn:
-        model_config.attn_implementation = 'flash_attention_2'
+    model_config.vision_config.use_flash_attn = use_flash_attn
+    model_config.llm_config.attn_implementation = 'flash_attention_2' if use_flash_attn else 'eager'
+    model_quant_config = getattr(model_config, 'quantization_config', None)
+
+    use_bnb = False
+    if model_quant_config is not None:
+        use_bnb = model_quant_config.get('quant_method', None) == 'bitsandbytes'
+    quantization_config = model_kwargs.get('quantization_config', None)
+    if isinstance(quantization_config, BitsAndBytesConfig):
+        use_bnb = True
 
     model, tokenizer = get_model_tokenizer_from_repo(
         model_dir,
         torch_dtype,
         model_kwargs,
         load_model,
         model_config=model_config,
         automodel_class=AutoModel,
         **kwargs)
 
+    if use_bnb and kwargs.get('is_training'):
+        # patch: bnb backward shape mismatch bug
+        if model is not None and model.language_model is not None:
+            model.language_model.output.state.force_no_igemmlt = True
+
     if model is not None:
         _use_submodel_func(model, 'language_model', ['get_input_embeddings'])
         fix_internvl_inplace_bug(model)
         if not hasattr(model, '__old_forward'):  # Avoid double patching
             forward = model.forward
             model.__old_forward = forward
 
@@ -2450,15 +2741,15 @@
 
         if not hasattr(model, '_old_extract_feature'):
             extract_feature = model.extract_feature
             model._old_extract_feature = extract_feature
 
             @wraps(extract_feature)
             def _new_extract_feature(pixel_values):
-                return extract_feature(pixel_values).to(pixel_values.device)
+                return extract_feature(pixel_values).to(pixel_values.device).to(pixel_values.dtype)
 
             model.extract_feature = _new_extract_feature
 
         if not hasattr(model.language_model, '__old_forward'):  # Avoid double patching
             old_forward = model.language_model.forward
             model.language_model.__old_forward = old_forward
 
@@ -2642,15 +2933,18 @@
                                     **kwargs):
     # compat with python==3.10
     if sys.version_info.minor >= 10:
         import collections
         import collections.abc
         for type_name in collections.abc.__all__:
             setattr(collections, type_name, getattr(collections.abc, type_name))
-    local_repo_path = _git_clone_github('https://github.com/deepseek-ai/DeepSeek-VL')
+    if 'local_repo_path' in kwargs:
+        local_repo_path = kwargs['local_repo_path']
+    else:
+        local_repo_path = _git_clone_github('https://github.com/deepseek-ai/DeepSeek-VL')
     sys.path.append(os.path.join(local_repo_path))
     from deepseek_vl.models import VLChatProcessor, MultiModalityCausalLM
     vl_chat_processor = VLChatProcessor.from_pretrained(model_dir)
     tokenizer = vl_chat_processor.tokenizer
     # flash_attn
     model_config = AutoConfig.from_pretrained(model_dir, trust_remote_code=True)
     use_flash_attn = kwargs.pop('use_flash_attn', False)
@@ -3197,14 +3491,15 @@
     'qwen/Qwen-1_8B-Chat-Int8',
     LoRATM.qwen,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5'],
     torch_dtype=torch.float16,
     function_kwargs={'gptq_bits': 8},
     support_flash_attn=True,
+    support_vllm=True,
     hf_model_id='Qwen/Qwen-1_8B-Chat-Int8')
 @register_model(
     ModelType.qwen_1_8b_chat_int4,
     'qwen/Qwen-1_8B-Chat-Int4',
     LoRATM.qwen,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5'],
@@ -3218,14 +3513,15 @@
     'qwen/Qwen-72B-Chat-Int8',
     LoRATM.qwen,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5'],
     torch_dtype=torch.float16,
     function_kwargs={'gptq_bits': 8},
     support_flash_attn=True,
+    support_vllm=True,
     hf_model_id='Qwen/Qwen-72B-Chat-Int8')
 @register_model(
     ModelType.qwen_72b_chat_int4,
     'qwen/Qwen-72B-Chat-Int4',
     LoRATM.qwen,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5'],
@@ -3265,24 +3561,26 @@
     'qwen/Qwen-14B-Chat-Int8',
     LoRATM.qwen,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5'],
     torch_dtype=torch.float16,
     function_kwargs={'gptq_bits': 8},
     support_flash_attn=True,
+    support_vllm=True,
     hf_model_id='Qwen/Qwen-14B-Chat-Int8')
 @register_model(
     ModelType.qwen_7b_chat_int8,
     'qwen/Qwen-7B-Chat-Int8',
     LoRATM.qwen,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5'],
     torch_dtype=torch.float16,
     function_kwargs={'gptq_bits': 8},
     support_flash_attn=True,
+    support_vllm=True,
     hf_model_id='Qwen/Qwen-7B-Chat-Int8')
 @register_model(
     ModelType.qwen_14b_chat_int4,
     'qwen/Qwen-14B-Chat-Int4',
     LoRATM.qwen,
     TemplateType.qwen,
     requires=['auto_gptq>=0.5'],
@@ -3366,14 +3664,31 @@
 @register_model(
     ModelType.telechat_12b,
     'TeleAI/TeleChat-12B',
     LoRATM.telechat,
     TemplateType.telechat,
     support_flash_attn=True,
     hf_model_id='Tele-AI/TeleChat-12B')
+@register_model(
+    ModelType.telechat_12b_v2,
+    'TeleAI/TeleChat-12B-v2',
+    LoRATM.telechat,
+    TemplateType.telechat_v2,
+    eos_token=2,
+    support_flash_attn=True,
+    hf_model_id='Tele-AI/TeleChat-12B-v2')
+@register_model(
+    ModelType.telechat_12b_v2_gptq_int4,
+    'swift/TeleChat-12B-V2-GPTQ-Int4',
+    LoRATM.telechat,
+    TemplateType.telechat_v2,
+    eos_token=2,
+    requires=['auto_gptq>=0.5'],
+    support_flash_attn=True,
+    function_kwargs={'gptq_bits': 4})
 def get_model_tokenizer_phi(model_dir: str,
                             torch_dtype: Dtype,
                             model_kwargs: Dict[str, Any],
                             load_model: bool = True,
                             **kwargs):
     model_config = AutoConfig.from_pretrained(model_dir, trust_remote_code=True)
     use_flash_attn = kwargs.pop('use_flash_attn', False)
@@ -3559,15 +3874,18 @@
     tags=['multi-modal', 'vision'],
     hf_model_id='01-ai/Yi-VL-6B')
 def get_model_tokenizer_yi_vl(model_dir: str,
                               torch_dtype: Dtype,
                               model_kwargs: Dict[str, Any],
                               load_model: bool = True,
                               **kwargs):
-    local_repo_path = _git_clone_github('https://github.com/01-ai/Yi')
+    if 'local_repo_path' in kwargs:
+        local_repo_path = kwargs['local_repo_path']
+    else:
+        local_repo_path = _git_clone_github('https://github.com/01-ai/Yi')
     sys.path.append(os.path.join(local_repo_path, 'VL'))
     from llava.model import LlavaLlamaForCausalLM, LlavaConfig
     from llava.model.constants import key_info
 
     model_config = LlavaConfig.from_pretrained(model_dir)
     mm_vision_tower = model_config.mm_vision_tower
     model_config.mm_vision_tower = os.path.join(model_dir, *mm_vision_tower.rsplit('/', maxsplit=2)[-2:])
@@ -3589,38 +3907,108 @@
         vision_tower.load_model()
         vision_tower.to(device=model.device, dtype=torch_dtype)
         if not hasattr(model.config, 'max_sequence_length'):
             model.config.max_sequence_length = 2048
     return model, tokenizer
 
 
+def _patch_minicpm_v_device_map(model) -> None:
+    if not hasattr(model, 'hf_device_map') or len(model.hf_device_map.values()) == 1:
+        return
+    if hasattr(model.llm, '__old_forward'):
+        # avoid double patching
+        return
+    device = list(model.hf_device_map.values())[0]
+    if hasattr(model, 'get_vision_embedding'):  # minicpm-v-v2-chat
+        _old_get_vision_embedding = model.get_vision_embedding
+
+        def _get_vision_embedding(pixel_values):
+            if len(pixel_values) == 0:
+                return _old_get_vision_embedding(pixel_values)
+            output = _old_get_vision_embedding(pixel_values)
+            return output.to(device=device)
+
+        model._old_get_vision_embedding = _old_get_vision_embedding
+        model.get_vision_embedding = _get_vision_embedding
+
+    if hasattr(model, 'resampler'):  # minicpm-v-v2_5-chat
+        __old_resampler_forward = model.resampler.forward
+
+        def _new_resampler_forward(*args, **kwargs) -> Tensor:
+            output = __old_resampler_forward(*args, **kwargs)
+            return output.to(device=device)
+
+        model.resampler.forward = _new_resampler_forward
+
+    __old_forward = model.llm.forward
+
+    def _new_forward(*args, **kwargs) -> Tensor:
+        inputs = kwargs.get('inputs_embeds')
+        if inputs is None:
+            inputs = kwargs.get('input_ids')
+        device = inputs.device
+        output = __old_forward(*args, **kwargs)
+        if output.logits is not None:
+            output.logits = output.logits.to(device)
+        if output.loss is not None:
+            output.loss = output.loss.to(device)
+        return output
+
+    model.llm.forward = _new_forward
+    model.llm.__old_forward = __old_forward
+
+
 @register_model(
     ModelType.minicpm_v_3b_chat,
     'OpenBMB/MiniCPM-V',
     LoRATM.llama2,
     TemplateType.minicpm_v,
     support_flash_attn=True,
     hf_model_id='openbmb/MiniCPM-V')
 @register_model(
-    ModelType.minicpm_v_v2,
+    ModelType.minicpm_v_v2_chat,
     'OpenBMB/MiniCPM-V-2',
     LoRATM.llama2,
     TemplateType.minicpm_v,
     support_flash_attn=True,
+    requires=['timm'],
     hf_model_id='openbmb/MiniCPM-V-2')
+@register_model(
+    ModelType.minicpm_v_v2_5_chat,
+    'OpenBMB/MiniCPM-Llama3-V-2_5',
+    LoRATM.llama2,
+    TemplateType.minicpm_v_v2_5,
+    support_flash_attn=True,
+    requires=['timm'],
+    pad_token='<unk>',
+    function_kwargs={'patching_embedding': True},
+    hf_model_id='openbmb/MiniCPM-Llama3-V-2_5')
 def get_model_tokenizer_minicpm_v(model_dir: str,
                                   torch_dtype: Dtype,
                                   model_kwargs: Dict[str, Any],
                                   load_model: bool = True,
                                   **kwargs):
-    model, tokenizer = get_model_tokenizer_minicpm(model_dir, torch_dtype, model_kwargs, load_model, **kwargs)
+    patching_embedding = kwargs.pop('patching_embedding', False)
+    model, tokenizer = get_model_tokenizer_with_flash_attn(model_dir, torch_dtype, model_kwargs, load_model, **kwargs)
     if load_model:
         model.resampler.to(torch_dtype)  # fix float32
+        _patch_minicpm_v_device_map(model)
         func_list = ['generate', 'get_input_embeddings', 'forward']
         _use_submodel_func(model, 'llm', func_list)
+        if patching_embedding:
+            embedding = model.get_input_embeddings()
+            if not hasattr(embedding, '__old_forward'):  # Avoid double patching
+                old_forward = embedding.forward
+
+                @wraps(old_forward)
+                def _new_forward(*args, **kwargs):
+                    return old_forward(*args, **kwargs).requires_grad_(True).clone()
+
+                embedding.__old_forward = old_forward
+                embedding.forward = _new_forward
     return model, tokenizer
 
 
 def _patch_llava(model):
     if hasattr(model, '__old_generate'):
         return
     generate = model.generate
@@ -3652,41 +4040,79 @@
     LoRATM.llama2,
     TemplateType.llava_mistral_instruct,
     requires=['transformers>=4.34'],
     support_flash_attn=True,
     function_kwargs={'llm_model_type': 'mistral'},
     tags=['multi-modal', 'vision'],
     hf_model_id='liuhaotian/llava-v1.6-mistral-7b')
+@register_model(
+    ModelType.llama3_llava_next_8b,
+    'AI-Modelscope/llama3-llava-next-8b',
+    LoRATM.llama2,
+    TemplateType.llama_llava_next,
+    support_flash_attn=True,
+    tags=['multi-modal', 'vision'],
+    function_kwargs={'llm_model_type': 'next_llama'},
+    hf_model_id='lmms-lab/llama3-llava-next-8b')
+@register_model(
+    ModelType.llava_next_72b,
+    'AI-Modelscope/llava-next-72b',
+    LoRATM.llama2,
+    TemplateType.llava_qwen_instruct,
+    support_flash_attn=True,
+    tags=['multi-modal', 'vision'],
+    function_kwargs={'llm_model_type': 'next_qwen'},
+    hf_model_id='lmms-lab/llava-next-72b')
+@register_model(
+    ModelType.llava_next_110b,
+    'AI-Modelscope/llava-next-110b',
+    LoRATM.llama2,
+    TemplateType.llava_qwen_instruct,
+    support_flash_attn=True,
+    tags=['multi-modal', 'vision'],
+    function_kwargs={'llm_model_type': 'next_qwen'},
+    hf_model_id='lmms-lab/llava-next-110b')
 def get_model_tokenizer_llava(model_dir: str,
                               torch_dtype: Dtype,
                               model_kwargs: Dict[str, Any],
                               load_model: bool = True,
                               **kwargs):
-    local_repo_path = _git_clone_github('https://github.com/haotian-liu/LLaVA.git')
+    llm_model_type = kwargs.pop('llm_model_type')
+    if 'local_repo_path' in kwargs:
+        repo_path = kwargs['local_repo_path']
+    elif 'next' in llm_model_type:
+        repo_path = 'https://github.com/LLaVA-VL/LLaVA-NeXT.git'
+    else:
+        repo_path = 'https://github.com/haotian-liu/LLaVA.git'
+    local_repo_path = _git_clone_github(repo_path)
     sys.path.append(os.path.join(local_repo_path))
 
-    llm_model_type = kwargs.pop('llm_model_type')
     if llm_model_type == 'mistral':
         from llava.model import LlavaMistralForCausalLM, LlavaMistralConfig
         model_config = LlavaMistralConfig.from_pretrained(model_dir)
         automodel_class = LlavaMistralForCausalLM
-    else:  # llama
+    elif 'llama' in llm_model_type:  # llama
         from llava.model import LlavaLlamaForCausalLM, LlavaConfig
         if not hasattr(LlavaLlamaForCausalLM, '__old_forward'):  # Avoid double patching
             forward = LlavaLlamaForCausalLM.forward
             LlavaLlamaForCausalLM.__old_forward = forward
 
             @wraps(forward)
             def _new_forward(*args, **kwargs):
                 kwargs.pop('cache_position', None)
                 return forward(*args, **kwargs)
 
             LlavaLlamaForCausalLM.forward = _new_forward
         model_config = LlavaConfig.from_pretrained(model_dir)
         automodel_class = LlavaLlamaForCausalLM
+    else:  # qwen
+        from llava.model import LlavaQwenForCausalLM
+        automodel_class = LlavaQwenForCausalLM
+        model_config = AutoConfig.from_pretrained(model_dir)
+
     model_config.mm_vision_tower = snapshot_download('AI-ModelScope/clip-vit-large-patch14-336')
     model, tokenizer = get_model_tokenizer_with_flash_attn(
         model_dir,
         torch_dtype,
         model_kwargs,
         load_model,
         model_config=model_config,
@@ -3729,15 +4155,18 @@
     support_flash_attn=True,
     hf_model_id='Mizukiluke/mplug_owl_2_1')
 def get_model_tokenizer_mplug_owl2(model_dir: str,
                                    torch_dtype: Dtype,
                                    model_kwargs: Dict[str, Any],
                                    load_model: bool = True,
                                    **kwargs):
-    local_repo_path = _git_clone_github('https://github.com/X-PLUG/mPLUG-Owl')
+    if 'local_repo_path' in kwargs:
+        local_repo_path = kwargs['local_repo_path']
+    else:
+        local_repo_path = _git_clone_github('https://github.com/X-PLUG/mPLUG-Owl')
     local_repo_path = os.path.join(local_repo_path, 'mPLUG-Owl2')
     sys.path.append(os.path.join(local_repo_path))
 
     # register
     # https://github.com/X-PLUG/mPLUG-Owl/blob/main/mPLUG-Owl2/mplug_owl2/model/modeling_mplug_owl2.py#L447
     from mplug_owl2 import MPLUGOwl2LlamaForCausalLM
     from transformers.models.clip.image_processing_clip import CLIPImageProcessor
@@ -3839,15 +4268,15 @@
 
 
 def get_torch_dtype(model_dir: str) -> Dtype:
     model_config = PretrainedConfig.get_config_dict(model_dir)[0]
     torch_dtype = model_config.get('torch_dtype', None)
     if isinstance(torch_dtype, str):
         torch_dtype = eval(f'torch.{torch_dtype}')
-    if torch_dtype == torch.float32:
+    if torch_dtype in {torch.float32, None}:
         torch_dtype = torch.float16
     return torch_dtype
 
 
 def get_model_tokenizer(model_type: str,
                         torch_dtype: Optional[Dtype] = None,
                         model_kwargs: Optional[Dict[str, Any]] = None,
@@ -3888,14 +4317,17 @@
             logger.info(f'Setting torch_dtype: {torch_dtype}')
             quantization_config = model_kwargs.get('quantization_config')
             if (isinstance(quantization_config, BitsAndBytesConfig)
                     and quantization_config.bnb_4bit_compute_dtype is None):
                 quantization_config.bnb_4bit_compute_dtype = torch_dtype
                 logger.info(f'Setting quantization_config.bnb_4bit_compute_dtype: {torch_dtype}')
     kwargs['eos_token'] = model_info['eos_token']
+    pad_token = model_info.get('pad_token')
+    if pad_token is not None:
+        kwargs['pad_token'] = pad_token
     if 'is_training' not in kwargs:
         kwargs['is_training'] = False
     model, tokenizer = get_function(model_dir, torch_dtype, model_kwargs, load_model, **kwargs)
     if model is not None:
         model.max_model_len = get_max_model_len(model.config)
         logger.info(f'model.max_model_len: {model.max_model_len}')
         model.model_type = model_type
```

### Comparing `ms-swift-2.0.4/swift/llm/utils/preprocess.py` & `ms-swift-2.0.5/swift/llm/utils/preprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,16 @@
     def __init__(self,
                  user_role: str = 'user',
                  assistant_role: str = 'assistant',
                  system_role: str = 'system',
                  conversations_key: str = 'conversations',
                  from_key: str = 'from',
                  value_key: str = 'value',
-                 repair_conversations: Callable[[str], Optional[Dict[str, str]]] = _default_repair_conversations,
+                 repair_conversations: Callable[[Union[str, Dict[str, str]]],
+                                                Optional[Dict[str, str]]] = _default_repair_conversations,
                  error_strategy: Literal['delete', 'raise'] = 'raise'):
         self.user_role = user_role
         self.assistant_role = assistant_role
         self.system_role = system_role
         self.conversations_key = conversations_key
         self.from_key = from_key
         self.value_key = value_key
@@ -218,15 +219,15 @@
         for d in tqdm(dataset):
             query.append(self.prompt.format(query=d[self.query_key]))
         return HfDataset.from_dict({'query': query, 'response': dataset[self.response_key]})
 
 
 class ClsPreprocessor:
 
-    def __init__(self, labels: List[str], task_name: str, is_pair_seq: bool) -> None:
+    def __init__(self, labels: List[str], task_name: str, is_pair_seq: bool = False) -> None:
         self.labels = labels
         category = ', '.join(labels)
         if is_pair_seq:
             inputs = 'Sentence1: {sentence1}\nSentence2: {sentence2}'
         else:
             inputs = 'Sentence: {sentence}'
         self.prompt = f"""Task: {task_name}
```

### Comparing `ms-swift-2.0.4/swift/llm/utils/protocol.py` & `ms-swift-2.0.5/swift/llm/utils/protocol.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/llm/utils/template.py` & `ms-swift-2.0.5/swift/llm/utils/template.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,47 +33,54 @@
     baichuan = 'baichuan'
     chatglm2 = 'chatglm2'
     chatglm3 = 'chatglm3'
     llama = 'llama'  # llama2
     llama3 = 'llama3'
     llava_mistral_instruct = 'llava-mistral-instruct'
     llava_yi_instruct = 'llava-yi-instruct'
+    llava_llama_instruct = 'llava-llama-instruct'
+    llava_qwen_instruct = 'llava-qwen-instruct'
+    llama_llava_next = 'llama-llava-next'
     openbuddy = 'openbuddy'
     openbuddy2 = 'openbuddy2'
     internlm = 'internlm'
     internlm2 = 'internlm2'
     internlm_xcomposer2 = 'internlm-xcomposer2'
     internvl = 'internvl'
     yi = 'yi'
+    yi1_5 = 'yi1_5'
     yi_vl = 'yi-vl'
     yuan = 'yuan'
     xverse = 'xverse'
     ziya = 'ziya'
     skywork = 'skywork'
     bluelm = 'bluelm'
     zephyr = 'zephyr'
     sus = 'sus'
     deepseek = 'deepseek'
     deepseek_coder = 'deepseek-coder'
     deepseek_vl = 'deepseek-vl'
+    deepseek2 = 'deepseek2'
     codefuse_codellama = 'codefuse-codellama'
     codefuse = 'codefuse'
-    cogvlm_instruct = 'cogvlm-instruct'
+    cogvlm = 'cogvlm'
     cogagent_chat = 'cogagent-chat'
     cogagent_instruct = 'cogagent-instruct'
     orion = 'orion'
     minicpm = 'minicpm'
     minicpm_v = 'minicpm-v'
+    minicpm_v_v2_5 = 'minicpm-v-v2_5'
     gemma = 'gemma'
     mplug_owl2 = 'mplug-owl2'
     wizardlm2_awq = 'wizardlm2-awq'
     wizardlm2 = 'wizardlm2'
     atom = 'atom'
     phi3 = 'phi3'
     telechat = 'telechat'
+    telechat_v2 = 'telechat-v2'
     dbrx = 'dbrx'
     mengzi = 'mengzi'
     c4ai = 'c4ai'
     chatml = 'chatml'
     # compatibility. (Deprecated)
     default_generation_bos = 'default-generation-bos'
 
@@ -198,14 +205,16 @@
         elif default_system is not None:
             assert self.prefix_has_system is not None, 'The template does not support `system`.'
             self.default_system = default_system
         self.max_length = max_length
         self.truncation_strategy = truncation_strategy
         self.model = kwargs.get('model', None)
         self.use_loss_scale = kwargs.get('use_loss_scale', False)
+        self.sequence_parallel_size = kwargs.get('sequence_parallel_size', 1)
+
         for key in ['prefix', 'prompt', 'chat_sep', 'suffix', 'prefix_has_system']:
             value = getattr(self, key)
             value = self._preprocess_prompt(tokenizer, value)
             setattr(self, key, value)
 
     def encode(self, example: Dict[str, Any]) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         """return: inputs, tokenizer_kwargs"""
@@ -416,14 +425,25 @@
 
         if use_torchacc():
             rank, _, world_size, _ = get_dist_setting()
             input_ids, attention_mask, labels, loss_scale = pad_and_split_batch(padding_to, input_ids, attention_mask,
                                                                                 labels, loss_scale, self.max_length,
                                                                                 self.tokenizer, rank, world_size)
 
+        bs, seq_len = input_ids.shape
+        position_ids = torch.arange(seq_len).unsqueeze(0).long().repeat(bs, 1)
+
+        if self.sequence_parallel_size > 1:
+            from swift.trainers.xtuner import get_xtuner_sequence_parallel_world_size
+            if get_xtuner_sequence_parallel_world_size() > 1:
+                from swift.trainers.xtuner import pad_and_split_for_sequence_parallel
+                input_ids, labels, position_ids, attention_mask, loss_scale = \
+                    pad_and_split_for_sequence_parallel(
+                        tokenizer, input_ids, labels, position_ids, attention_mask, loss_scale)
+
         res = {
             'input_ids': input_ids,
             'attention_mask': attention_mask,
             'labels': labels,
         }
         if loss_scale is not None:
             res['loss_scale'] = loss_scale
@@ -502,16 +522,16 @@
             assert is_finished and not return_delta
         return response
 
 
 TEMPLATE_MAPPING: Dict[str, Dict[str, Any]] = {}
 
 
-def register_template(template_type: str, template: Template, *, exists_ok: bool = False, **kwargs) -> None:
-    if not exists_ok and template_type in TEMPLATE_MAPPING:
+def register_template(template_type: str, template: Template, *, exist_ok: bool = False, **kwargs) -> None:
+    if not exist_ok and template_type in TEMPLATE_MAPPING:
         raise ValueError(f'The `{template_type}` has already been registered in the TEMPLATE_MAPPING.')
     template_info = {'template': template, **kwargs}
     TEMPLATE_MAPPING[template_type] = template_info
 
 
 register_template(
     TemplateType.default,
@@ -592,14 +612,19 @@
 register_template(TemplateType.qwen_audio_generation, QwenAudioGenerationTemplate(), lazy_tokenize=True)
 
 register_template(
     TemplateType.yi,
     Template([], ['<|im_start|>user\n{{QUERY}}<|im_end|>\n<|im_start|>assistant\n'], ['<|im_end|>\n'], ['<|im_end|>'],
              None, ['<|im_start|>system\n{{SYSTEM}}<|im_end|>\n']))
 
+register_template(
+    TemplateType.yi1_5,
+    Template([], ['<|im_start|>user\n{{QUERY}}<|im_end|> \n<|im_start|>assistant\n'], ['<|im_end|>\n'], ['<|im_end|>'],
+             None, ['{{SYSTEM}}']))
+
 yi_vl_default_system = (
     'This is a chat between an inquisitive human and an AI assistant. Assume the role of the AI assistant. '
     "Read all the images carefully, and respond to the human's questions with informative, "
     'helpful, detailed and polite answers. '
     '这是一个好奇的人类和一个人工智能助手之间的对话。假设你扮演这个AI助手的角色。'
     '仔细阅读所有的图像，并对人类的问题做出信息丰富、有帮助、详细的和礼貌的回答。')
 
@@ -669,14 +694,17 @@
     Template([[64790, 64792]], [[64795], '\n {{QUERY}}', [64796], '\n'], [], [[64795]], None,
              [[64790, 64792, 64794], '\n {{SYSTEM}}']))
 
 register_template(
     TemplateType.deepseek,
     Template([['bos_token_id']], ['User: {{QUERY}}\n\nAssistant:'], [['eos_token_id']], [['eos_token_id']], None,
              [['bos_token_id'], '{{SYSTEM}}\n\n']))
+register_template(
+    TemplateType.deepseek2,
+    Template([[100000]], ['User: {{QUERY}}\n\nAssistant:'], [[100001]], [[100001]], None, [[100000], '{{SYSTEM}}\n\n']))
 
 # ref: https://github.com/facebookresearch/llama/blob/main/llama/generation.py
 LLAMA_DEFAULT_SYSTEM = (
     'You are a helpful, respectful and honest assistant. '
     'Always answer as helpfully as possible, while being safe. '
     'Your answers should not include any harmful, unethical, racist, sexist, toxic, dangerous, or illegal content. '
     'Please ensure that your responses are socially unbiased and positive in nature.\n\n'
@@ -1002,14 +1030,78 @@
         Template.__init__(self, [], [[-200], self.llavayi_query_template], None, ['<|im_end|>'])
 
 
 register_template(
     TemplateType.llava_yi_instruct, LLavaYiTemplate(), use_model=True, infer_media_type='round', lazy_tokenize=True)
 
 
+class LLavaLlamaTemplate(Template):
+
+    llavallama_query_template = '<|start_header_id|>user<|end_header_id|>\n\n<image>\n' \
+                                '{{QUERY}}<|eot_id|><|start_header_id|>assistant<|end_header_id|>\n\n'
+
+    def __init__(self):
+        Template.__init__(self, [], [self.llavallama_query_template], ['<|eot_id|>'], ['<|eot_id|>'])
+
+    def encode(self, example: Dict[str, Any]) -> Tuple[Dict[str, Any], Dict[str, Any]]:
+        inputs, _ = super().encode(example)
+        image_path = example['images']
+        raw_image = _read_from_path(image_path[0])
+        pixel_values = self.model.processor.image_processor(raw_image, return_tensors='pt')['pixel_values']
+        inputs['pixel_values'] = pixel_values.to(self.model.dtype)
+        return inputs, {}
+
+    def data_collator(self, batch: List[Dict[str, Any]], padding_to: Optional[int] = None) -> Dict[str, Any]:
+        res = super().data_collator(batch, padding_to)
+        res['pixel_values'] = torch.concat([b['pixel_values'] for b in batch])
+        return res
+
+
+register_template(
+    TemplateType.llava_llama_instruct,
+    LLavaLlamaTemplate(),
+    use_model=True,
+    infer_media_type='round',
+    lazy_tokenize=True)
+
+
+class LlamaLlavaNextTemplate(LLavaTemplate):
+    default_system = 'You are a helpful language and vision assistant. ' \
+            'You are able to understand the visual content that the user provides, ' \
+            'and assist the user with a variety of tasks using natural language.'
+
+    def __init__(self):
+        Template.__init__(self, [], [
+            '<|start_header_id|>user<|end_header_id|>\n\n', [-200],
+            '\n{{QUERY}}<|eot_id|><|start_header_id|>assistant<|end_header_id|>\n\n'
+        ], ['<|eot_id|>'], ['<|eot_id|>'], self.default_system,
+                          ['<|begin_of_text|><|start_header_id|>system<|end_header_id|>\n\n{{SYSTEM}}'])
+
+
+register_template(
+    TemplateType.llama_llava_next,
+    LlamaLlavaNextTemplate(),
+    use_model=True,
+    infer_media_type='round',
+    lazy_tokenize=True)
+
+
+class LLavaQwenTemplate(LLavaTemplate):
+    llavayi_query_template = 'You are a helpful assistant'
+
+    def __init__(self):
+        Template.__init__(self, [], ['<|im_start|>user\n', [-200], '{{QUERY}}<|im_end|>\n<|im_start|>assistant\n'],
+                          ['<|im_end|>\n'], ['<|im_end|>'], self.llavayi_query_template,
+                          ['<|im_start|>system\n{{SYSTEM}}<|im_end|>\n'])
+
+
+register_template(
+    TemplateType.llava_qwen_instruct, LLavaQwenTemplate(), use_model=True, infer_media_type='round', lazy_tokenize=True)
+
+
 def _findall(token_list: List[int], token: int) -> List[int]:
     """Find the index of a token in the token_list."""
     res = []
     idx = -1
     try:
         while True:
             idx = token_list.index(token, idx + 1)
@@ -1136,15 +1228,15 @@
         model = self.model
         inputs2 = model.build_conversation_input_ids(
             self.tokenizer, query=example['query'], history=example.get('history'), images=[image])
         image_token_len = inputs2['token_type_ids'].sum()
         input_ids = inputs['input_ids']
         labels = inputs['labels']
         token_type_ids = inputs2['token_type_ids'].tolist()
-        inputs['input_ids'] = input_ids[:1] + [0] * image_token_len + input_ids[1:]
+        inputs['input_ids'] = input_ids[:1] + [self.tokenizer.pad_token_id] * image_token_len + input_ids[1:]
         if labels is not None:
             inputs['labels'] = labels[:1] + [-100] * image_token_len + labels[1:]
         dtype = model.dtype
         inputs['images'] = [[img.to(dtype=dtype)] for img in inputs2['images']]
         if 'cross_images' in inputs2:
             # is cogagent
             inputs['cross_images'] = [[cross_img.to(dtype=dtype)] for cross_img in inputs2['cross_images']]
@@ -1174,27 +1266,28 @@
     TemplateType.cogagent_instruct,
     CogTemplate(['<s>'], ['<EOI>Question: {{QUERY}} Answer:'], None, ['</s>']),
     use_model=True,
     infer_media_type='dialogue',
     lazy_tokenize=True)
 
 register_template(
-    TemplateType.cogvlm_instruct,
-    CogTemplate(['<s>'], ['Question: {{QUERY}} Answer:'], None, ['</s>']),
+    TemplateType.cogvlm,
+    CogTemplate([['bos_token_id']], ['Question: {{QUERY}} Answer:'], ['\n'], [['eos_token_id']]),
     use_model=True,
     infer_media_type='dialogue',
     lazy_tokenize=True)
 
 register_template(TemplateType.minicpm, Template(['<s>{{SYSTEM}}'], ['<用户>{{QUERY}}<AI>'], [], ['</s>']))
 
 
 class MiniCPMVTemlate(Template):
 
-    def __init__(self):
-        return super().__init__(['<s>{{SYSTEM}}'], ['<用户><image><unk></image>\n{{QUERY}}<AI>'], [], ['</s>'])
+    def __init__(self, *args, **kwargs):
+        self.is_v2_5 = kwargs.pop('is_v2_5', False)
+        return super().__init__(*args, **kwargs)
 
     def encode(self, example: Dict[str, Any]) -> Tuple[Dict[str, Any], Dict[str, Any]]:
         images_path = example['images']
         assert len(images_path) == 1
         image = _read_from_path(images_path[0])
         inputs, _ = super().encode(example)
         if len(inputs) == 0:
@@ -1216,78 +1309,97 @@
             input_ids = new_input_ids
             if labels is not None:
                 new_labels = new_labels + labels[start:]
                 labels = new_labels
 
         idx = img_start_idxs[0] + 1  # first <unk>
         config = self.model.config
-        if hasattr(config, 'slice_mode') and config.slice_mode:
-            slice_mode = True
-            assert hasattr(config, 'patch_size')
-            assert hasattr(config, 'max_slice_nums')
-            assert hasattr(config, 'scale_resolution')
-        else:
-            slice_mode = False
-
-        if slice_mode:
+        tgt_sizes = None
+        if config.slice_mode:
             images, placeholder = self.model.get_slice_image_placeholder(image, self.tokenizer)
             placeholder_id = self.tokenizer.encode(placeholder, add_special_tokens=False)
             input_ids = (input_ids[:idx - 1] + placeholder_id + input_ids[idx + 2:])
             if labels is not None:
                 labels = (labels[:idx - 1] + [-100] * len(placeholder_id) + labels[idx + 2:])
             input_tensor_ids = torch.tensor(input_ids)
             image_start_idx = torch.where(input_tensor_ids == self.tokenizer.im_start_id)[0]
             image_start_idx += 1
             image_end_idx = torch.where(input_tensor_ids == self.tokenizer.im_end_id)[0]
             valid_image_nums = max(len(image_start_idx), len(image_end_idx))
             image_bound = [
                 torch.hstack(
                     [image_start_idx[:valid_image_nums].unsqueeze(-1), image_end_idx[:valid_image_nums].unsqueeze(-1)])
             ]
-            pixel_values = [self.model.transform(img).to(device=self.model.device) for img in images]
-
+            if self.is_v2_5:
+                pixel_values = []
+                tgt_sizes = []
+                config = self.model.config
+                for image in images:
+                    image = self.model.transform(image).to(device=self.model.device)
+                    H, W = image.shape[1:]
+                    pixel_values.append(self.model.reshape_by_patch(image))
+                    tgt_sizes.append(torch.Tensor([H // config.patch_size, W // config.patch_size]).type(torch.int32))
+                tgt_sizes = torch.vstack(tgt_sizes)
+            else:
+                pixel_values = [self.model.transform(img).to(device=self.model.device) for img in images]
         else:
             input_ids = (input_ids[:idx] + [self.tokenizer.unk_token_id] * config.query_num + input_ids[idx + 1:])
             if labels is not None:
                 labels = (labels[:idx] + [-100] * config.query_num + labels[idx + 1:])
             image_bound = [torch.tensor([[idx, idx + config.query_num]])]
             pixel_values = [self.model.transform(image).to(device=self.model.device)]
-        inputs_embeds, _ = self.model.get_vllm_embedding({
-            'input_ids':
-            torch.tensor(input_ids)[None].to(device=self.model.device),
-            'image_bound':
-            image_bound,
+        data = {
+            'input_ids': torch.tensor(input_ids)[None].to(device=self.model.device),
+            'image_bound': image_bound,
             'pixel_values': [pixel_values]
-        })
+        }
+        if tgt_sizes is not None:
+            data['tgt_sizes'] = [tgt_sizes]
+        inputs_embeds, _ = self.model.get_vllm_embedding(data)
         inputs['input_ids'] = input_ids
         inputs['labels'] = labels
         inputs['inputs_embeds'] = inputs_embeds[0]
         return inputs, {}
 
     @staticmethod
     def get_generate_ids(generate_ids: Tensor, input_token_len: int) -> List[int]:
         return generate_ids[0].tolist()
 
 
 register_template(
     TemplateType.minicpm_v,
-    MiniCPMVTemlate(),
+    MiniCPMVTemlate(['<s>{{SYSTEM}}'], ['<用户><image><unk></image>\n{{QUERY}}<AI>'], [], ['</s>']),
+    use_model=True,
+    lazy_tokenize=True,
+    infer_media_type='dialogue',
+    dataloader_num_workers=0,
+    dataloader_pin_memory=False)
+
+register_template(
+    TemplateType.minicpm_v_v2_5,
+    MiniCPMVTemlate(['<|begin_of_text|>{{SYSTEM}}'], [
+        '<|start_header_id|>user<|end_header_id|>\n\n<image><unk></image>\n{{QUERY}}<|eot_id|>'
+        '<|start_header_id|>assistant<|end_header_id|>\n\n'
+    ], ['<|eot_id|>'], ['<|eot_id|>'],
+                    is_v2_5=True),
     use_model=True,
     lazy_tokenize=True,
     infer_media_type='dialogue',
     dataloader_num_workers=0,
     dataloader_pin_memory=False)
 
 gemma_template = Template(['<bos>'], ['<start_of_turn>user\n{{QUERY}}<end_of_turn>\n<start_of_turn>model\n'],
                           ['<end_of_turn>\n'], ['<end_of_turn>'], None,
                           ['<bos><start_of_turn>system\n{{SYSTEM}}<end_of_turn>\n'])
 register_template(TemplateType.gemma, gemma_template)
 
 register_template(TemplateType.telechat, Template([], ['<_user>{{QUERY}}<_bot>'], ['<_end>'], ['<_end>']))
 
+register_template(TemplateType.telechat_v2, Template([], ['<_user> {{QUERY}}<_bot>'], [], ['<_end>']))
+
 DBRX_SYSTEM = (
     'You are DBRX, created by Databricks. You were last updated in December 2023. '
     'You answer questions based on information available up to that point.\n'
     'YOU PROVIDE SHORT RESPONSES TO SHORT QUESTIONS OR STATEMENTS, '
     'but provide thorough responses to more complex and open-ended questions.\n'
     'You assist with various tasks, from writing to coding (using markdown for code blocks '
     '— remember to use ``` with code, JSON, and tables).\n'
```

### Comparing `ms-swift-2.0.4/swift/llm/utils/utils.py` & `ms-swift-2.0.5/swift/llm/utils/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 import multiprocess
 import numpy as np
 import requests
 import torch
 import torch.distributed as dist
 import transformers
 from datasets import Dataset as HfDataset
+from datasets.arrow_writer import SchemaInferenceError
+from datasets.exceptions import DatasetGenerationError
 from modelscope.utils.config_ds import MS_CACHE_HOME
 from modelscope.utils.logger import get_logger as get_ms_logger
 from torch import device as Device
 from torch.nn import Linear, Module
 from torch.nn.parallel import DistributedDataParallel as DDP
-from torch.utils.data import Dataset
+from torch.utils.data import Dataset, IterableDataset
 from tqdm.auto import tqdm
 from transformers import (GenerationConfig, PretrainedConfig, PreTrainedModel, PreTrainedTokenizerBase,
                           StoppingCriteriaList, TextStreamer, trainer)
 from transformers.generation.streamers import BaseStreamer
 from transformers.utils import is_torch_npu_available, strtobool
 
 from swift.hub import ModelScopeConfig
@@ -59,14 +61,15 @@
     resp = requests.get(url, cookies=cookies, stream=True)
     with open(local_path, 'wb') as f:
         for data in tqdm(resp.iter_lines()):
             f.write(data)
 
 
 def download_dataset(model_id: str, files: List[str], force_download: bool = False) -> str:
+    assert isinstance(files, list)
     url = f'http://www.modelscope.cn/api/v1/datasets/{model_id}/repo?Revision=master&FilePath={{fpath}}'
     cache_dir = os.path.join(MS_CACHE_HOME, 'datasets', model_id, 'master')
     local_dir = os.path.join(cache_dir, 'raw')
     tmp_dir = os.path.join(cache_dir, 'tmp')
     os.makedirs(local_dir, exist_ok=True)
     os.makedirs(tmp_dir, exist_ok=True)
     cookies = ModelScopeConfig.get_cookies()
@@ -153,14 +156,97 @@
         data = [self.data[i] for i in idx_list]
         return self.__class__(data)
 
     def __len__(self) -> int:
         return len(self.data)
 
 
+# Code borrowed from trl
+class ConstantLengthDataset(IterableDataset):
+
+    def __init__(
+        self,
+        template: 'Template',
+        dataset,
+        seq_length=1024,
+        num_of_sequences=1024,
+        chars_per_token=3.6,
+        append_concat_token=True,
+        add_special_tokens=True,
+    ):
+        self.template = template
+
+        self.concat_token_id = self.template.tokenizer.eos_token_id
+        self.dataset = dataset
+        self.seq_length = seq_length
+        self.max_buffer_size = seq_length * chars_per_token * num_of_sequences
+        self.append_concat_token = append_concat_token
+        self.add_special_tokens = add_special_tokens
+
+    @staticmethod
+    def get_packed_dataset(template: 'Template',
+                           dataset,
+                           seq_length=1024,
+                           num_of_sequences=1024,
+                           chars_per_token=3.6,
+                           append_concat_token=True,
+                           add_special_tokens=True,
+                           lazy_tokenize=False):
+        constant_length_iterator = ConstantLengthDataset(template, dataset, seq_length, num_of_sequences,
+                                                         chars_per_token, append_concat_token, add_special_tokens)
+
+        if lazy_tokenize:
+            return constant_length_iterator
+
+        def data_generator(constant_length_iterator):
+            yield from constant_length_iterator
+
+        try:
+            packed_dataset = HfDataset.from_generator(
+                data_generator, gen_kwargs={'constant_length_iterator': constant_length_iterator})
+        except (DatasetGenerationError, SchemaInferenceError) as exc:
+            raise ValueError(
+                'Error occurred while packing the dataset. '
+                'Make sure that your dataset has enough samples to at least yield one packed sequence.') from exc
+        return packed_dataset
+
+    def __len__(self):
+        return len(self.dataset)
+
+    def __iter__(self):
+        iterator = iter(self.dataset)
+        more_examples = True
+        while more_examples:
+            buffer, buffer_len = [], 0
+            while True:
+                if buffer_len >= self.max_buffer_size:
+                    break
+                try:
+                    example = next(iterator)
+                    lens = sum([len(value) if value else 0 for value in example.values()])
+                    buffer.append(next(iterator))
+                    buffer_len += lens
+                except StopIteration:
+                    more_examples = False
+                    break
+
+            packed_sequences = {}
+            for example in buffer:
+                input, _ = self.template.encode(example)
+                for key in input.keys():
+                    if key not in packed_sequences:
+                        packed_sequences[key] = []
+                    packed_sequences[key].extend(input[key])
+
+            lens = len(packed_sequences[list(packed_sequences.keys())[0]])
+            for i in range(0, lens, self.seq_length):
+                example = {key: value[i:i + self.seq_length] for key, value in packed_sequences.items()}
+                yield example
+
+
 class LazyLLMDataset(Dataset):
 
     def __init__(self, dataset: HfDataset, template: Template, *, try_fetch_time: int = 20) -> None:
         self.dataset = dataset
         self.template = template
         self.try_fetch_time = min(try_fetch_time, len(self.dataset))
         assert self.try_fetch_time >= 1
@@ -253,32 +339,42 @@
             _token_len.append(len(d['input_ids']))
     _, stat_str = stat_array(_token_len)
     logger.info(f'Dataset Token Length: {stat_str}')
     return stat_str
 
 
 def safe_tokenizer_decode(tokenizer: PreTrainedTokenizerBase, input_ids: List[int], **tokenizer_kwargs) -> str:
+
+    def _is_special(token: int) -> bool:
+        if token < 0:
+            return True
+        if tokenizer.eos_token_id != tokenizer.pad_token_id:
+            return token == tokenizer.pad_token_id
+        return False
+
+    if isinstance(input_ids, torch.Tensor):
+        input_ids = input_ids.tolist()
     if len(input_ids) == 0:
         return ''
     result_str = ''
     for i in range(len(input_ids)):
         if i == 0:
-            if input_ids[i] < 0:
+            if _is_special(input_ids[i]):
                 s = 0
             else:
                 e = 0
             continue
-        if input_ids[i] < 0 and input_ids[i - 1] >= 0:
+        if _is_special(input_ids[i]) and not _is_special(input_ids[i - 1]):
             s = i
             result_str += tokenizer.decode(input_ids[e:s], **tokenizer_kwargs)
-        if input_ids[i] >= 0 and input_ids[i - 1] < 0:
+        if not _is_special(input_ids[i]) and _is_special(input_ids[i - 1]):
             e = i
-            result_str += f'[-100 * {e - s}]'
-    if input_ids[-1] < 0:
-        result_str += f'[-100 * {len(input_ids) - s}]'
+            result_str += f'[{input_ids[i - 1]} * {e - s}]'
+    if _is_special(input_ids[-1]):
+        result_str += f'[{input_ids[i - 1]} * {len(input_ids) - s}]'
     else:
         result_str += tokenizer.decode(input_ids[e:], **tokenizer_kwargs)
     return result_str
 
 
 def print_example(example: Dict[str, Any],
                   tokenizer: PreTrainedTokenizerBase,
@@ -303,14 +399,15 @@
         if isinstance(module, module_cls):
             module_name = '.'.join(name.split('.')[-2:])
             module_names.add(module_name)
     return list(module_names)
 
 
 def find_ln(model: Module) -> List[str]:
+    # find_layer_norm
     module_names = set()
     for name, module in model.named_modules():
         module_cls_name = module.__class__.__name__.lower()
         if isinstance(module, torch.nn.LayerNorm) or 'rmsnorm' in module_cls_name:
             module_name = '.'.join(name.split('.')[-1:])
             module_names.add(module_name)
     return list(module_names)
@@ -419,23 +516,25 @@
         value = self.token_queue.get(timeout=self.timeout)
         if value == self.stop_signal:
             raise StopIteration()
         else:
             return value
 
 
+@torch.inference_mode()
 def inference_stream(model: PreTrainedModel,
                      template: Template,
                      query: str,
                      history: Optional[History] = None,
                      system: Optional[str] = None,
                      *,
                      generation_config: Optional[GenerationConfig] = None,
                      stop_words: Optional[StopWords] = None,
                      generation_info: Optional[Dict[str, int]] = None,
+                     adapter_names: Optional[List[str]] = None,
                      **kwargs) -> Iterator[Tuple[str, History]]:
     """
     generation_config: Priority: generation_config > model.generation_config.
     """
     if stop_words is None:
         stop_words = []
     if history is None:
@@ -468,15 +567,15 @@
         inputs['input_ids'] = input_ids
         token_len = input_ids.shape[1]
     if 'inputs_embeds' in inputs:
         inputs_embeds = inputs['inputs_embeds'][None]
         inputs['inputs_embeds'] = inputs_embeds
         token_len = inputs_embeds.shape[1]
 
-    inputs['attention_mask'] = torch.ones(token_len)[None]
+    inputs['attention_mask'] = torch.ones(token_len, dtype=torch.int64)[None]
     if 'token_type_ids' in inputs:
         inputs['token_type_ids'] = torch.tensor(inputs['token_type_ids'])[None]
     model.eval()
     if generation_config is None:
         generation_config = getattr(model, 'generation_config', None)
     generation_config = deepcopy(generation_config)
     if generation_config.num_beams != 1:
@@ -501,14 +600,16 @@
     stopping_criteria = StoppingCriteriaList([StopWordsCriteria(tokenizer, stop_words, **tokenizer_kwargs)])
     inputs = to_device(inputs, device)
     if generation_info is not None:
         generation_info['num_prompt_tokens'] = token_len
     if 'inputs_embeds' in inputs:
         inputs.pop('input_ids', None)
     streamer = TokenListIteratorStreamer()
+    if adapter_names is not None:
+        inputs['adapter_names'] = adapter_names
     generation_kwargs = {
         'streamer': streamer,
         'generation_config': generation_config,
         'stopping_criteria': stopping_criteria,
         **inputs
     }
     _model_generate = model.generate
@@ -547,27 +648,29 @@
         if not is_observation:
             history[-1] = [query, response]
         else:
             history[-1][-1] = history[-1][-1][:act_length] + response
         yield response, history
 
 
+@torch.inference_mode()
 def inference(model: PreTrainedModel,
               template: Template,
               query: str,
               history: Optional[History] = None,
               system: Optional[str] = None,
               *,
               generation_config: Optional[GenerationConfig] = None,
               stop_words: Optional[StopWords] = None,
               stream: bool = False,
               verbose: bool = False,
               prompt_prefix: str = '[PROMPT]',
               output_prefix: str = '[OUTPUT]',
               generation_info: Optional[Dict[str, int]] = None,
+              adapter_names: Optional[List[str]] = None,
               **kwargs) -> Tuple[str, History]:
     """
     generation_config: Priority: generation_config > model.generation_config.
     """
     if stop_words is None:
         stop_words = []
     if history is None:
@@ -584,16 +687,19 @@
         'query': query,
         'history': history,
         'system': system,
         'images': kwargs.pop('images', None)  # for vl. str.
     }
     template.model = model
     inputs, tokenizer_kwargs = template.encode(example)
-    if len(inputs) == 0:
-        raise ValueError('input_ids exceeds `max_length`. Please increase the value of `max_length`.')
+
+    truncation_strategy = kwargs.pop('truncation_strategy', None)
+    if len(inputs) == 0 and truncation_strategy == 'delete':
+        return '', history
+
     inputs.pop('labels', None)
     tokenizer = template.tokenizer
     device = next(model.parameters()).device
     if 'input_ids' in inputs:
         input_ids = torch.tensor(inputs['input_ids'])[None]
         inputs['input_ids'] = input_ids
         token_len = input_ids.shape[1]
@@ -641,14 +747,16 @@
         stop_words.append(template.suffix[-1])
     stopping_criteria = StoppingCriteriaList([StopWordsCriteria(tokenizer, stop_words, **tokenizer_kwargs)])
     inputs = to_device(inputs, device)
     if generation_info is not None:
         generation_info['num_prompt_tokens'] = token_len
     if 'inputs_embeds' in inputs:
         inputs.pop('input_ids', None)
+    if adapter_names is not None:
+        inputs['adapter_names'] = adapter_names
     generate_ids = model.generate(
         streamer=streamer, generation_config=generation_config, stopping_criteria=stopping_criteria, **inputs)
     generate_ids = template.get_generate_ids(generate_ids, token_len)
     if generation_info is not None:
         generation_info['num_generated_tokens'] = len(generate_ids)
     response = None
     if verbose and stream is False:
@@ -729,14 +837,22 @@
     model.generation_config = generation_config
 
 
 def is_vllm_available():
     return importlib.util.find_spec('vllm') is not None
 
 
+def is_xtuner_available():
+    return importlib.util.find_spec('xtuner') is not None
+
+
+def is_unsloth_available() -> bool:
+    return importlib.util.find_spec('unsloth') is not None
+
+
 def get_time_info(log_history: List[Dict[str, Any]], n_train_samples: Optional[int]) -> Optional[Dict[str, Any]]:
     time_info = None
     try:
         last_log_history = log_history[-1]
         train_runtime = last_log_history['train_runtime']
         train_samples_per_second = n_train_samples / train_runtime
         time_info = {
```

### Comparing `ms-swift-2.0.4/swift/llm/utils/vision_utils.py` & `ms-swift-2.0.5/swift/llm/utils/vision_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/torchacc_utils.py` & `ms-swift-2.0.5/swift/torchacc_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/trainers/__init__.py` & `ms-swift-2.0.5/swift/trainers/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/trainers/arguments.py` & `ms-swift-2.0.5/swift/trainers/arguments.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/trainers/callback.py` & `ms-swift-2.0.5/swift/trainers/callback.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/trainers/dpo_trainers.py` & `ms-swift-2.0.5/swift/trainers/dpo_trainers.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/trainers/mixin.py` & `ms-swift-2.0.5/swift/trainers/mixin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 # Part of the implementation is borrowed from huggingface/transformers.
 import importlib
 import os
 import re
 import shutil
+import time
 from pathlib import Path
 from types import MethodType
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 import json
 import numpy as np
+import peft
 import safetensors
 import torch
 import transformers
 from datasets import Dataset as HfDataset
 from packaging import version
 from peft import PeftModel
 from torch.nn import Module
@@ -245,20 +247,24 @@
             tokenizer=tokenizer,
             model_init=model_init,
             compute_metrics=compute_metrics,
             callbacks=callbacks,
             optimizers=optimizers,
             preprocess_logits_for_metrics=preprocess_logits_for_metrics,
             **kwargs)
+        if not self.label_names:
+            self.label_names = ['labels']
         if is_quantized and use_swift:
             model._hf_peft_config_loaded = _hf_peft_config_loaded
 
         if get_function(model.__class__.forward) is not get_function(model.forward):
             self.label_names = find_labels(model)
             self.can_return_loss = can_return_loss(model)
+        self.max_memory = 0.0
+        self.start_time = time.time()
 
     @staticmethod
     def _create_configuration_file(model: Module, output_dir: str) -> None:
         cfg = getattr(model, 'cfg', {})
         configuration_path = os.path.join(output_dir, 'configuration.json')
         new_cfg = {}
         if os.path.exists(configuration_path):
@@ -369,21 +375,21 @@
                 else:
                     torch.save(state_dict, os.path.join(output_dir, 'pytorch_model.bin'))
         elif is_instance_of_ms_model(self.model):
             PreTrainedModel.save_pretrained(
                 self.model, output_dir, state_dict=state_dict, safe_serialization=save_safetensors)
         else:
             self.model.save_pretrained(output_dir, state_dict=state_dict, safe_serialization=save_safetensors)
+        sft_args = getattr(self, 'sft_args', None)
         # tokenizer
-        if self.tokenizer is not None:
+        if self.tokenizer is not None and sft_args is not None and sft_args.sft_type == 'full':
             self.tokenizer.save_pretrained(output_dir)
         # training_args.bin
         torch.save(self.args, os.path.join(output_dir, 'training_args.bin'))
         # additional files
-        sft_args = getattr(self, 'sft_args', None)
         if sft_args is not None and sft_args.sft_type == 'full':
             additional_files = getattr(self.args, 'additional_saved_files', []) + ['preprocessor_config.json']
             if model_dir is not None:
                 for file in additional_files:
                     src_path = os.path.join(model_dir, file)
                     dst_path = os.path.join(output_dir, file)
                     if os.path.isfile(src_path):
@@ -498,14 +504,26 @@
                 if state_dict is not None:
                     self.model.load_state_dict(state_dict, strict=False, adapter_name='default')
             else:
                 super()._load_best_model()
         except ValueError as e:
             logger.warning(e)
 
+    def get_max_cuda_memory(self, device: Optional[Union[torch.device, int]] = None) -> float:
+        if device is None:
+            mems = [torch.cuda.max_memory_reserved(device=device) for device in range(torch.cuda.device_count())]
+        else:
+            mems = [torch.cuda.max_memory_reserved(device=device)]
+        mem = sum([float(mem) / 1024 / 1024 / 1024 for mem in mems])
+        if self.max_memory < mem:
+            self.max_memory = mem
+        if torch.cuda.is_available():
+            torch.cuda.reset_peak_memory_stats()
+        return mem
+
     def _maybe_log_save_evaluate(self, tr_loss, *args, **kwargs):
         if self.control.should_log:
             self.control.should_log = False
             logs: Dict[str, float] = {}
             metrics_log = {'loss': tr_loss}  # loss first
             if hasattr(self, '_custom_metrics'):
                 metrics_log.update(self._custom_metrics)
@@ -519,15 +537,19 @@
             if version.parse(transformers.__version__) >= version.parse('4.38'):
                 grad_norm = args[0]
                 if isinstance(grad_norm, torch.Tensor):
                     grad_norm = grad_norm.item()
                 if grad_norm is not None:
                     logs['grad_norm'] = grad_norm
             logs['learning_rate'] = self._get_learning_rate()
-
+            logs['memory(GiB)'] = round(self.get_max_cuda_memory(), 2)
+            import time
+            time_now = time.time()
+            elapse_time = time_now - self.start_time
+            logs['train_speed(iter/s)'] = round(self.state.global_step / elapse_time, 6)
             tr_loss -= tr_loss
             self._globalstep_last_logged = self.state.global_step
             self.store_flos()
             self.log(logs)
         super()._maybe_log_save_evaluate(tr_loss, *args, **kwargs)
 
     def create_optimizer_and_scheduler(self, num_training_steps: int):
```

### Comparing `ms-swift-2.0.4/swift/trainers/optimizers/galore/__init__.py` & `ms-swift-2.0.5/swift/trainers/optimizers/galore/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/trainers/optimizers/galore/adafactor.py` & `ms-swift-2.0.5/swift/trainers/optimizers/galore/adafactor.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/trainers/optimizers/galore/adamw.py` & `ms-swift-2.0.5/swift/trainers/optimizers/galore/adamw.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/trainers/optimizers/galore/adamw8bit.py` & `ms-swift-2.0.5/swift/trainers/optimizers/galore/adamw8bit.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/trainers/optimizers/galore/galore_projector.py` & `ms-swift-2.0.5/swift/trainers/optimizers/galore/galore_projector.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/trainers/optimizers/galore/utils.py` & `ms-swift-2.0.5/swift/trainers/optimizers/galore/utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/trainers/trainers.py` & `ms-swift-2.0.5/swift/trainers/trainers.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import time
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import torch
 from peft import PeftModel
 from torch import Tensor, nn
 from torch.nn import CrossEntropyLoss
-from torch.utils.data import DataLoader
 from transformers import Seq2SeqTrainer as HfSeq2SeqTrainer
 from transformers import Trainer as HfTrainer
 from transformers import trainer
 from transformers.modeling_utils import unwrap_model
 from transformers.models.auto.modeling_auto import MODEL_FOR_CAUSAL_LM_MAPPING_NAMES
 from transformers.utils import is_peft_available
 
@@ -29,28 +28,31 @@
 class Trainer(PushToMsHubMixin, SwiftMixin, HfTrainer):
     pass
 
 
 class Seq2SeqTrainer(PushToMsHubMixin, SwiftMixin, HfSeq2SeqTrainer):
 
     def __init__(self, *args, **kwargs):
+        self.sequence_parallel_size = kwargs.pop('sequence_parallel_size', 1)
         super().__init__(*args, **kwargs)
         # performance
         self.perf: Dict[str, Any] = {
             'gen_time': 0.,
             'gen_len': 0,
             'memory': {},
             'model': self.model.get_trainable_parameters() if hasattr(self.model, 'get_trainable_parameters') else None,
         }
         self._acc = torch.tensor(0.).to(self.args.device)
+        if self.sequence_parallel_size > 1:
+            from swift.trainers.xtuner import init_sequence_parallel_xtuner
+            init_sequence_parallel_xtuner(self.sequence_parallel_size)
 
     def train(self, *args, **kwargs) -> torch.Tensor:
         res = super().train(*args, **kwargs)
-        for i in range(torch.cuda.device_count()):
-            self.perf['memory'][f'cuda:{i}'] = f'{torch.cuda.max_memory_reserved(i)/1024/1024/1024:.2f}GiB'
+        self.perf['memory']['cuda'] = f'{self.max_memory:.2f}GiB'
         return res
 
     def prediction_step(
         self,
         model: nn.Module,
         inputs: Dict[str, Union[torch.Tensor, Any]],
         prediction_loss_only: bool,
@@ -204,14 +206,21 @@
                 loss = self.label_smoother(outputs, labels)
         else:
             loss = outputs['loss'] if isinstance(outputs, dict) else outputs[0]
 
         preds = outputs.logits.argmax(dim=2)[..., :-1]
         if labels is None:
             labels = inputs['labels']
+
+        if self.sequence_parallel_size > 1:
+            from swift.trainers.xtuner import reduce_xtuner_sequence_parallel_loss
+            loss = reduce_xtuner_sequence_parallel_loss(loss, labels)
+
+        preds = outputs.logits.argmax(dim=2)[..., :-1]
+
         labels = labels[..., 1:]
         masks = labels != -100
         acc_strategy = getattr(self.args, 'acc_strategy', 'token')
         acc: Optional[Tensor] = None
         if preds.shape != labels.shape:
             pass
         elif acc_strategy == 'sentence':
@@ -224,19 +233,18 @@
         if model.training and acc is not None:
             if 'acc' not in self._custom_metrics:
                 self._custom_metrics['acc'] = self._acc
             self._custom_metrics['acc'] = self._custom_metrics['acc'] + acc / self.args.gradient_accumulation_steps
         return (loss, outputs) if return_outputs else loss
 
     def get_train_dataloader(self):
-
-        if not use_torchacc():
-            return super().get_train_dataloader()
-
-        else:
+        if self.sequence_parallel_size > 1:
+            from swift.trainers.xtuner import get_xtuner_train_dataloader
+            return get_xtuner_train_dataloader(self)
+        elif use_torchacc():
             if trainer.is_datasets_available():
                 import datasets
 
             if self.train_dataset is None:
                 raise ValueError('Trainer: training requires a train_dataset.')
 
             train_dataset = self.train_dataset
@@ -245,20 +253,21 @@
             if trainer.is_datasets_available() and isinstance(train_dataset, datasets.Dataset):
                 train_dataset = self._remove_unused_columns(train_dataset, description='training')
             else:
                 data_collator = self._get_collator_with_removed_columns(data_collator, description='training')
 
             return ta_train_dataloader(train_dataset, data_collator, self._get_train_sampler(), self.args,
                                        self._train_batch_size)
+        else:
+            return super().get_train_dataloader()
 
     def get_eval_dataloader(self, eval_dataset):
         if not use_torchacc():
             return super().get_eval_dataloader(eval_dataset)
         else:
-            import torchacc as ta
             if trainer.is_datasets_available():
                 import datasets
 
             if eval_dataset is None and self.eval_dataset is None:
                 raise ValueError('Trainer: evaluation requires an eval_dataset.')
             eval_dataset = eval_dataset if eval_dataset is not None else self.eval_dataset
             data_collator = self.data_collator
@@ -270,15 +279,14 @@
 
             return ta_eval_dataloader(eval_dataset, data_collator, self._get_eval_sampler(eval_dataset), self.args)
 
     def get_test_dataloader(self, test_dataset):
         if not use_torchacc():
             return super().get_test_dataloader(test_dataset)
         else:
-            import torchacc as ta
             if trainer.is_datasets_available():
                 import datasets
 
             data_collator = self.data_collator
 
             if trainer.is_datasets_available() and isinstance(test_dataset, datasets.Dataset):
                 test_dataset = self._remove_unused_columns(test_dataset, description='test')
```

### Comparing `ms-swift-2.0.4/swift/trainers/utils.py` & `ms-swift-2.0.5/swift/trainers/utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/__init__.py` & `ms-swift-2.0.5/swift/tuners/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,34 +8,35 @@
     from .base import SwiftModel, Swift
     from .lora import LoRA, LoRAConfig
     from .mapping import SWIFT_MAPPING, SwiftTuners
     from .side import Side, SideConfig, SideModule
     from .neftune import NEFTune, NEFTuneConfig
     from .longlora.longlora import LongLoRAModelType, LongLoRAConfig, LongLoRA
     from .restuning import ResTuning, ResTuningConfig, ResTuningBypassModule
-    from .peft import (AdaLoraConfig, IA3Config, LoftQConfig, LoHaConfig, LoKrConfig, LoraConfig, OFTConfig, PeftConfig,
-                       PeftModel, PeftModelForCausalLM, PeftModelForSeq2SeqLM, PeftModelForSequenceClassification,
-                       PeftModelForTokenClassification, PrefixTuningConfig, PromptEncoderConfig, PromptLearningConfig,
-                       PromptTuningConfig, get_peft_config, get_peft_model, get_peft_model_state_dict)
+    from .peft import (AdaLoraConfig, IA3Config, LoftQConfig, LoHaConfig, LoKrConfig, LoraConfig, VeraConfig,
+                       BOFTConfig, OFTConfig, PeftConfig, PeftModel, PeftModelForCausalLM, PeftModelForSeq2SeqLM,
+                       PeftModelForSequenceClassification, PeftModelForTokenClassification, PrefixTuningConfig,
+                       PromptEncoderConfig, PromptLearningConfig, PromptTuningConfig, get_peft_config, get_peft_model,
+                       get_peft_model_state_dict)
     from .prompt import Prompt, PromptConfig, PromptModule
     from .scetuning.scetuning import SCETuning, SCETuningConfig
     from .utils import SwiftConfig, SwiftOutput
 else:
     _import_structure = {
         'adapter': ['Adapter', 'AdapterConfig', 'AdapterModule'],
         'base': ['SwiftModel', 'Swift'],
         'lora': ['LoRA', 'LoRAConfig'],
         'longlora.longlora': ['LongLoRAModelType', 'LongLoRAConfig', 'LongLoRA'],
         'mapping': ['SWIFT_MAPPING', 'SwiftTuners'],
         'side': ['Side', 'SideConfig', 'SideModule'],
         'neftune': ['NEFTune', 'NEFTuneConfig'],
         'restuning': ['ResTuning', 'ResTuningConfig', 'ResTuningBypassModule'],
         'peft': [
-            'AdaLoraConfig', 'IA3Config', 'LoftQConfig', 'LoHaConfig', 'LoKrConfig', 'LoraConfig', 'OFTConfig',
-            'PeftConfig', 'PeftModel', 'PeftModelForCausalLM', 'PeftModelForSeq2SeqLM',
+            'AdaLoraConfig', 'IA3Config', 'LoftQConfig', 'LoHaConfig', 'LoKrConfig', 'LoraConfig', 'VeraConfig',
+            'BOFTConfig', 'OFTConfig', 'PeftConfig', 'PeftModel', 'PeftModelForCausalLM', 'PeftModelForSeq2SeqLM',
             'PeftModelForSequenceClassification', 'PeftModelForTokenClassification', 'PrefixTuningConfig',
             'PromptEncoderConfig', 'PromptLearningConfig', 'PromptTuningConfig', 'get_peft_config', 'get_peft_model',
             'get_peft_model_state_dict'
         ],
         'prompt': ['Prompt', 'PromptConfig', 'PromptModule'],
         'scetuning': ['SCETuning', 'SCETuningConfig'],
         'utils': ['SwiftConfig', 'SwiftOutput'],
```

### Comparing `ms-swift-2.0.4/swift/tuners/adapter.py` & `ms-swift-2.0.5/swift/tuners/adapter.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/base.py` & `ms-swift-2.0.5/swift/tuners/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -799,15 +799,15 @@
             shutil.move(os.path.join(output_dir, 'default', CONFIG_NAME), os.path.join(output_dir, CONFIG_NAME))
             state_dict = SwiftModel.load_state_file(os.path.join(output_dir, 'default'))
             safe_serialization = os.path.isfile(os.path.join(output_dir, 'default', SAFETENSORS_WEIGHTS_NAME))
             SwiftModel._save_state_dict(state_dict, output_dir, safe_serialization)
             shutil.rmtree(os.path.join(output_dir, 'default'))
 
     @staticmethod
-    def from_pretrained(model: Union[nn.Module, SwiftModel],
+    def from_pretrained(model: Union[nn.Module, SwiftModel, PeftModel],
                         model_id: str = None,
                         adapter_name: Union[str, List[str], Dict[str, str]] = None,
                         revision: str = None,
                         **kwargs):
         """Prepare a model by a model_id in the ModelScope hub or a local dir.
 
         Args:
@@ -833,11 +833,45 @@
             if isinstance(adapter_name, list) else list(adapter_name.keys())[0]
         _name = _name or ''
         if os.path.exists(os.path.join(model_id, _name, CONFIG_NAME)):
             with open(os.path.join(model_id, _name, CONFIG_NAME), 'r') as f:
                 _json = json.load(f)
             is_peft_model = SWIFT_TYPE_KEY not in _json and 'extra_state_keys' not in _json
         if is_peft_model:
-            return PeftModel.from_pretrained(
-                model, model_id, revision=revision, adapter_name=adapter_name or 'default', **kwargs)
+
+            def load_peft_model(_model, _adapter_name, _new_name=None):
+                if not _new_name:
+                    _new_name = _adapter_name
+                import peft
+                if not isinstance(_model, peft.PeftModel):
+                    return PeftModel.from_pretrained(
+                        _model,
+                        os.path.join(model_id, _adapter_name) if _adapter_name != 'default'
+                        and os.path.exists(os.path.join(model_id, _adapter_name)) else model_id,
+                        revision=revision,
+                        adapter_name=_new_name,
+                        **kwargs)
+                else:
+                    _model.load_adapter(
+                        os.path.join(model_id, _adapter_name) if _adapter_name != 'default'
+                        and os.path.exists(os.path.join(model_id, _adapter_name)) else model_id, _new_name)
+                    return _model
+
+            if not adapter_name:
+                peft_model = load_peft_model(model, 'default')
+                for _dir in os.listdir(model_id):
+                    if os.path.isdir(os.path.join(model_id, _dir)) and \
+                            os.path.exists(os.path.join(model_id, _dir, CONFIG_NAME)):
+                        peft_model = load_peft_model(peft_model, _dir)
+            elif isinstance(adapter_name, str):
+                return load_peft_model(model, adapter_name)
+            elif isinstance(adapter_name, list):
+                peft_model = model
+                for name in adapter_name:
+                    peft_model = load_peft_model(peft_model, name)
+            else:
+                peft_model = model
+                for key, value in adapter_name.items():
+                    peft_model = load_peft_model(peft_model, key, value)
+            return peft_model
         else:
             return SwiftModel.from_pretrained(model, model_id, revision=revision, adapter_name=adapter_name, **kwargs)
```

### Comparing `ms-swift-2.0.4/swift/tuners/llamapro.py` & `ms-swift-2.0.5/swift/tuners/llamapro.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/longlora/llama.py` & `ms-swift-2.0.5/swift/tuners/longlora/llama.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/longlora/longlora.py` & `ms-swift-2.0.5/swift/tuners/longlora/longlora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/lora.py` & `ms-swift-2.0.5/swift/tuners/lora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/lora_layers.py` & `ms-swift-2.0.5/swift/tuners/lora_layers.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,20 +31,27 @@
 from .utils import ActivationMixin, ModulesToSaveWrapper, SwiftAdapter
 
 logger = get_logger()
 dispatchers = []
 
 
 def is_auto_awq_available():
-    return importlib.util.find_spec('awq') is not None and importlib.util.find_spec('peft.tuners.lora.awq') is not None
+    return importlib.util.find_spec('awq') is not None
 
 
 def is_aqlm_available():
-    return importlib.util.find_spec('aqlm') is not None and importlib.util.find_spec(
-        'peft.tuners.lora.aqlm') is not None
+    return importlib.util.find_spec('aqlm') is not None
+
+
+def is_eetq_available():
+    return importlib.util.find_spec('eetq') is not None
+
+
+def is_hqq_available():
+    return importlib.util.find_spec('hqq') is not None
 
 
 def is_auto_gptq_available():
     try:
         return peft.import_utils._is_auto_gptq_available()
     except ImportError as e:
         logger.warn(e)
@@ -354,14 +361,84 @@
             new_module = QuantLinear(target, adapter_name, module_key=module_key, **kwargs)
             target.qweight = target_base_layer.qweight
 
         return new_module
 
     dispatchers.append(dispatch_gptq)
 
+if is_eetq_available():
+    from peft.tuners.lora.eetq import EetqLoraLinear as _EetqLoraLinear
+    from eetq import EetqLinear
+
+    class EetqLoraLinear(LoRAActivationMixin, _EetqLoraLinear):
+
+        def __init__(
+            self,
+            *args,
+            module_key: str,
+            **kwargs,
+        ):
+            super(EetqLoraLinear, self).__init__(module_key)
+            self.set_activation(args[1], True)
+            super(ActivationMixin, self).__init__(*args, **kwargs)
+
+    def dispatch_eetq(
+        target: torch.nn.Module,
+        adapter_name: str,
+        **kwargs: Any,
+    ) -> Optional[torch.nn.Module]:
+        new_module = None
+
+        if isinstance(target, BaseTunerLayer):
+            target_base_layer = target.get_base_layer()
+        else:
+            target_base_layer = target
+
+        if is_eetq_available() and isinstance(target_base_layer, EetqLinear):
+            new_module = EetqLoraLinear(target, adapter_name, **kwargs)
+            target.weight = target_base_layer.weight
+
+            if hasattr(target, 'bias'):
+                target.bias = target_base_layer.bias
+
+        return new_module
+
+    dispatchers.append(dispatch_eetq)
+
+if is_hqq_available():
+    from peft.tuners.lora.hqq import HqqLoraLinear as _HqqLoraLinear
+    from hqq.core.quantize import HQQLinear
+
+    class HqqLoraLinear(LoRAActivationMixin, _HqqLoraLinear):
+
+        def __init__(
+            self,
+            *args,
+            module_key: str,
+            **kwargs,
+        ):
+            super(HqqLoraLinear, self).__init__(module_key)
+            self.set_activation(args[1], True)
+            super(ActivationMixin, self).__init__(*args, **kwargs)
+
+    def dispatch_hqq(target: torch.nn.Module, adapter_name: str, **kwargs):
+        new_module = None
+
+        if isinstance(target, BaseTunerLayer):
+            target_base_layer = target.get_base_layer()
+        else:
+            target_base_layer = target
+
+        if is_hqq_available() and isinstance(target_base_layer, HQQLinear):
+            new_module = HqqLoraLinear(target_base_layer, adapter_name, **kwargs)
+
+        return new_module
+
+    dispatchers.append(dispatch_hqq)
+
 
 def dispatch_megatron(
     target: torch.nn.Module,
     adapter_name: str,
     lora_config,
     module_key,
     **kwargs: Any,
@@ -371,36 +448,36 @@
     if isinstance(target, BaseTunerLayer):
         target_base_layer = target.get_base_layer()
     else:
         target_base_layer = target
 
     if lora_config.megatron_config:
         megatron_core = importlib.import_module(lora_config.megatron_core)
-        linears = (megatron_core.tensor_parallel.ColumnParallelLinear, megatron_core.tensor_parallel.RowParallelLinear)
     else:
         megatron_core = None
-        linears = None
 
-    if megatron_core and isinstance(target_base_layer, linears):
+    if megatron_core and isinstance(
+            target_base_layer,
+        (megatron_core.tensor_parallel.ColumnParallelLinear, megatron_core.tensor_parallel.RowParallelLinear)):  # noqa
         megatron_kwargs = kwargs.copy()
         megatron_config = lora_config.megatron_config
         if isinstance(megatron_config, dict):
             transformer_config_class = megatron_core.transformer.transformer_config.TransformerConfig
             megatron_config = transformer_config_class(**lora_config.megatron_config)
         megatron_kwargs['megatron_config'] = megatron_config
         if megatron_kwargs['fan_in_fan_out']:
             warnings.warn('fan_in_fan_out is set to True but the target module is `ColumnParallelLinear` '
                           'or `RowParallelLinear`. '
                           'Setting fan_in_fan_out to False.')
             megatron_kwargs['fan_in_fan_out'] = lora_config.fan_in_fan_out = False
         new_module = LoraParallelLinear(
             base_layer=target,
             adapter_name=adapter_name,
-            backend=megatron_core.tensor_parallel,
             module_key=module_key,
+            backend=megatron_core.tensor_parallel,
             **megatron_kwargs)
 
     return new_module
 
 
 def dispatch_default(
     target: torch.nn.Module,
@@ -501,15 +578,17 @@
         self.lora_A[adapter_name] = nn.Linear(self.in_features, r, bias=False)
         self.lora_B[adapter_name] = nn.Linear(r, self.out_features, bias=False)
         if use_rslora:
             self.scaling[adapter_name] = lora_alpha / math.sqrt(r)
         else:
             self.scaling[adapter_name] = lora_alpha / r
 
-        if init_lora_weights == 'loftq':
+        if isinstance(init_lora_weights, str) and init_lora_weights.startswith('pissa'):
+            self.pissa_init(adapter_name, init_lora_weights)
+        elif init_lora_weights == 'loftq':
             self.loftq_init(adapter_name)
         elif init_lora_weights:
             self.reset_lora_parameters(adapter_name, init_lora_weights)
 
         # check weight and qweight (for GPTQ)
         for weight_name in ('weight', 'qweight'):
             weight = getattr(self.get_base_layer(), weight_name, None)
@@ -597,20 +676,18 @@
 
         model_config = getattr(model, 'config', {'model_type': 'custom'})
         if hasattr(model_config, 'to_dict'):
             model_config = model_config.to_dict()
 
         peft_config = self._prepare_adapter_config(peft_config, model_config)
 
-        if version.parse(peft.__version__) > version.parse('0.8.2'):
-            from peft.tuners.tuners_utils import _maybe_include_all_linear_layers
-            # update peft_config.target_modules if required
-            peft_config = _maybe_include_all_linear_layers(peft_config, model)
-        if version.parse(peft.__version__) >= version.parse('0.10.0'):
-            self._prepare_model(peft_config, model)
+        from peft.tuners.tuners_utils import _maybe_include_all_linear_layers
+        # update peft_config.target_modules if required
+        peft_config = _maybe_include_all_linear_layers(peft_config, model)
+        self._prepare_model(peft_config, model)
 
         for key in key_list:
             # Check for modules_to_save in case
             if _check_for_modules_to_save and any(
                     key.endswith(f'{module_to_save}') for module_to_save in peft_config.modules_to_save):
                 # Optionally set the modules to save
                 parent, target, target_name = _get_submodules(model, key)
@@ -759,17 +836,18 @@
             else:
                 new_module.state = child.state
             new_module.to(child.weight.device)
 
         # dispatch to correct device
         for name, module in new_module.named_modules():
             if (self.prefix in name) or ('ranknum' in name):
-                weight = child.qweight if hasattr(child, 'qweight') else child.weight
-                if weight.device != torch.device('meta'):
-                    module.to(weight.device)
+                weight = (
+                    child.qweight
+                    if hasattr(child, 'qweight') else child.W_q if hasattr(child, 'W_q') else child.weight)
+                module.to(weight.device)
 
     @staticmethod
     def _create_new_module(lora_config, adapter_name, target, **kwargs):
         """
         Override code:
         1. Support current_key argument
         2. Support MergedLinear
```

### Comparing `ms-swift-2.0.4/swift/tuners/mapping.py` & `ms-swift-2.0.5/swift/tuners/mapping.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/module_mapping.py` & `ms-swift-2.0.5/swift/tuners/module_mapping.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/neftune.py` & `ms-swift-2.0.5/swift/tuners/neftune.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/peft.py` & `ms-swift-2.0.5/swift/tuners/peft.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 from functools import partial, reduce
 from typing import Dict, Optional
 
 import json
 import peft
 import torch
 import torch.nn
-from peft import (AdaLoraConfig, IA3Config, LoftQConfig, LoHaConfig, LoKrConfig, LoraModel, OFTConfig, PeftConfig,
-                  PeftModel, PeftModelForCausalLM, PeftModelForSeq2SeqLM, PeftModelForSequenceClassification,
-                  PeftModelForTokenClassification, PrefixTuningConfig, PromptEncoderConfig, PromptLearningConfig,
-                  PromptTuningConfig, get_peft_config, get_peft_model, get_peft_model_state_dict)
+from packaging import version
+from peft import (AdaLoraConfig, BOFTConfig, IA3Config, LoftQConfig, LoHaConfig, LoKrConfig, LoraModel, OFTConfig,
+                  PeftConfig, PeftModel, PeftModelForCausalLM, PeftModelForSeq2SeqLM,
+                  PeftModelForSequenceClassification, PeftModelForTokenClassification, PrefixTuningConfig,
+                  PromptEncoderConfig, PromptLearningConfig, PromptTuningConfig, VeraConfig, get_peft_config,
+                  get_peft_model, get_peft_model_state_dict)
 from peft.config import PeftConfigMixin
 from peft.tuners.lora import Embedding
 from transformers import Trainer
 
 from swift import get_logger
 from swift.hub.snapshot_download import snapshot_download
 
@@ -264,14 +266,16 @@
     # Fix Lora does not support NonDynamicallyQuantizableLinear
     LoraModel._create_and_replace_origin = LoraModel._create_and_replace
     LoraModel._create_and_replace = _create_and_replace_hook
 
     # Support type conversion
     def init(self, model: torch.nn.Module, config: Dict[str, LoraConfig], adapter_name):
         self.__init_origin__(model, config, adapter_name)
+        if isinstance(self.active_adapter, list):
+            self.active_adapter = self.active_adapter[0]
         active_config = config[self.active_adapter] if isinstance(config, dict) else config
         if hasattr(active_config, 'lora_dtype'):
             for name, module in model.named_modules():
                 if isinstance(module, LoraLayer):
                     _convert_dtype(module, self.active_adapter, active_config.lora_dtype)
 
     LoraModel.__init_origin__ = LoraModel.__init__
@@ -340,10 +344,13 @@
 LoraConfig = wrap_module(LoraConfig)
 AdaLoraConfig = wrap_module(AdaLoraConfig)
 IA3Config = wrap_module(IA3Config)
 LoHaConfig = wrap_module(LoHaConfig)
 LoKrConfig = wrap_module(LoKrConfig)
 LoftQConfig = wrap_module(LoftQConfig)
 OFTConfig = wrap_module(OFTConfig)
+BOFTConfig = wrap_module(BOFTConfig)
+VeraConfig = wrap_module(VeraConfig)
+OFTConfig = wrap_module(OFTConfig)
 get_peft_config = get_peft_config
 get_peft_model_state_dict = get_peft_model_state_dict
 get_peft_model = get_peft_model
```

### Comparing `ms-swift-2.0.4/swift/tuners/prompt.py` & `ms-swift-2.0.5/swift/tuners/prompt.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/restuning.py` & `ms-swift-2.0.5/swift/tuners/restuning.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/restuning_components.py` & `ms-swift-2.0.5/swift/tuners/restuning_components.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/rome/compute_u.py` & `ms-swift-2.0.5/swift/tuners/rome/compute_u.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/rome/compute_v.py` & `ms-swift-2.0.5/swift/tuners/rome/compute_v.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/rome/context_template.py` & `ms-swift-2.0.5/swift/tuners/rome/context_template.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/rome/nethook.py` & `ms-swift-2.0.5/swift/tuners/rome/nethook.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/rome/repr_tools.py` & `ms-swift-2.0.5/swift/tuners/rome/repr_tools.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/rome/rome.py` & `ms-swift-2.0.5/swift/tuners/rome/rome.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/rome/rome_hparams.py` & `ms-swift-2.0.5/swift/tuners/rome/rome_hparams.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/scetuning/scetuning.py` & `ms-swift-2.0.5/swift/tuners/scetuning/scetuning.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/scetuning/scetuning_components.py` & `ms-swift-2.0.5/swift/tuners/scetuning/scetuning_components.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/side.py` & `ms-swift-2.0.5/swift/tuners/side.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/tuners/utils.py` & `ms-swift-2.0.5/swift/tuners/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Copyright (c) Alibaba, Inc. and its affiliates.
 # Copyright 2023-present the HuggingFace Inc. team.
 
 import hashlib
 import os
 import shutil
 import threading
+import uuid
 from dataclasses import asdict, dataclass, field
 from types import FunctionType
-from typing import Dict, List, Optional, OrderedDict, Union
+from typing import Dict, Optional, Union
 
 import json
 import numpy as np
 import torch
 from packaging import version
 from peft.utils import CONFIG_NAME
 from peft.utils import ModulesToSaveWrapper as _ModulesToSaveWrapper
@@ -172,19 +173,23 @@
 
     def get_activated_adapters(self):
         return [key for key, value in self._thread_inf.get(self.indent, {}).items() if value]
 
 
 class OffloadHelper:
 
-    sub_dir = 'offload_cache'
-    cache_dir = os.path.join(get_cache_dir(), sub_dir)
-    shutil.rmtree(cache_dir, ignore_errors=True)
-    os.makedirs(cache_dir, exist_ok=True)
-    index = {}
+    def __init__(self):
+        sub_dir = os.path.join('offload_cache', str(uuid.uuid4().hex))
+        self.cache_dir = os.path.join(get_cache_dir(), sub_dir)
+        shutil.rmtree(self.cache_dir, ignore_errors=True)
+        os.makedirs(self.cache_dir, exist_ok=True)
+        self.index = {}
+
+    def __del__(self):
+        shutil.rmtree(self.cache_dir, ignore_errors=True)
 
     @staticmethod
     def offload_weight(weight, weight_name, offload_folder, index=None):
         dtype = None
         if str(weight.dtype) == 'torch.bfloat16':
             weight = weight.view(torch.int16)
             dtype = 'bfloat16'
@@ -217,34 +222,32 @@
             weight = weight[0]
         weight = torch.tensor(weight)
         if weight_info['dtype'] == 'bfloat16':
             weight = weight.view(torch.bfloat16)
 
         return weight
 
-    @staticmethod
-    def offload_disk(module: torch.nn.Module, adapter_name, module_key):
+    def offload_disk(self, module: torch.nn.Module, adapter_name, module_key):
         key = adapter_name + ':' + module_key
         md5 = hashlib.md5(key.encode('utf-8')).hexdigest()
-        sub_folder = os.path.join(OffloadHelper.cache_dir, md5)
+        sub_folder = os.path.join(self.cache_dir, md5)
         os.makedirs(sub_folder, exist_ok=True)
         state_dict = module.state_dict()
-        OffloadHelper.index[md5] = {}
+        self.index[md5] = {}
         for key, tensor in state_dict.items():
-            OffloadHelper.offload_weight(tensor, key, sub_folder, OffloadHelper.index[md5])
+            OffloadHelper.offload_weight(tensor, key, sub_folder, self.index[md5])
 
-    @staticmethod
-    def load_disk(module: torch.nn.Module, adapter_name, module_key):
+    def load_disk(self, module: torch.nn.Module, adapter_name, module_key):
         key = adapter_name + ':' + module_key
         md5 = hashlib.md5(key.encode('utf-8')).hexdigest()
-        sub_folder = os.path.join(OffloadHelper.cache_dir, md5)
+        sub_folder = os.path.join(self.cache_dir, md5)
         state_dict = {}
-        for key, value in OffloadHelper.index[md5].items():
+        for key, value in self.index[md5].items():
             file = os.path.join(sub_folder, f'{key}.dat')
-            state_dict[key] = OffloadHelper.load_offloaded_weight(file, OffloadHelper.index[md5][key])
+            state_dict[key] = OffloadHelper.load_offloaded_weight(file, self.index[md5][key])
         if version.parse(torch.__version__) >= version.parse('2.1.0'):
             module.load_state_dict(state_dict, assign=True)
         else:
             for name, _module in module.named_modules():
                 if len(list(_module.modules())) > 1:
                     continue
 
@@ -260,14 +263,16 @@
                     params[sub_name] = param_cls(state_dict[prefix + sub_name], requires_grad=param.requires_grad)
                 _module._parameters.update(params)
         shutil.rmtree(sub_folder, ignore_errors=True)
 
 
 class SwiftAdapter:
 
+    offload_helper = OffloadHelper()
+
     @staticmethod
     def prepare_model(model: torch.nn.Module, config: SwiftConfig, adapter_name: str) -> SwiftOutput:
         raise NotImplementedError
 
     @staticmethod
     def activate_adapter(module: torch.nn.Module, adapter_name: str, activate: bool, offload: str = None):
         raise NotImplementedError
@@ -290,30 +295,30 @@
             return
         module.origin_device = str(device)
         if offload == 'cpu':
             if str(device) != 'cpu':
                 module.to('cpu')
         elif offload == 'meta':
             if str(device) != 'meta':
-                OffloadHelper.offload_disk(module, adapter_name=adapter_name, module_key=module_key)
+                SwiftAdapter.offload_helper.offload_disk(module, adapter_name=adapter_name, module_key=module_key)
                 module.to('meta')
         else:
             raise NotImplementedError
         torch.cuda.empty_cache()
 
     @staticmethod
     def load(module: torch.nn.Module, adapter_name, module_key):
         device = next(iter(module.parameters())).device
         if not hasattr(module, 'origin_device') or module.origin_device == str(device):
             return
         if str(device) == 'cpu':
             module.to(module.origin_device)
             delattr(module, 'origin_device')
         elif str(device) == 'meta':
-            OffloadHelper.load_disk(module, adapter_name=adapter_name, module_key=module_key)
+            SwiftAdapter.offload_helper.load_disk(module, adapter_name=adapter_name, module_key=module_key)
             module.to(module.origin_device)
             delattr(module, 'origin_device')
 
     @staticmethod
     def has_additional_modules():
         return True
```

### Comparing `ms-swift-2.0.4/swift/ui/base.py` & `ms-swift-2.0.5/swift/ui/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,18 @@
         if not isinstance(self, (Tab, TabItem, Accordion)) and 'interactive' not in kwargs:  # noqa
             kwargs['interactive'] = True
 
         if 'is_list' in kwargs:
             self.is_list = kwargs.pop('is_list')
 
         if base_builder and base_builder.default(elem_id) is not None:
-            kwargs['value'] = base_builder.default(elem_id)
+            if os.environ.get('MODELSCOPE_ENVIRONMENT') == 'studio' and kwargs.get('value') is not None:
+                pass
+            else:
+                kwargs['value'] = base_builder.default(elem_id)
 
         if builder is not None:
             if elem_id in builder.locales(lang):
                 values = builder.locale(elem_id, lang)
                 if 'info' in values:
                     kwargs['info'] = values['info']
                 if 'value' in values:
```

### Comparing `ms-swift-2.0.4/swift/ui/llm_infer/generate.py` & `ms-swift-2.0.5/swift/ui/llm_infer/generate.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/ui/llm_infer/llm_infer.py` & `ms-swift-2.0.5/swift/ui/llm_infer/llm_infer.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,15 @@
                         cls.generate_chat,
                         inputs=[
                             model_and_template,
                             cls.element('template_type'), prompt, chatbot,
                             cls.element('system'),
                             cls.element('max_new_tokens'),
                             cls.element('temperature'),
+                            cls.element('do_sample'),
                             cls.element('top_k'),
                             cls.element('top_p'),
                             cls.element('repetition_penalty')
                         ],
                         outputs=[prompt, chatbot],
                         queue=True)
 
@@ -220,15 +221,17 @@
             model_dir = kwargs.pop('model_id_or_path')
             if not os.path.exists(model_dir):
                 model_dir = snapshot_download(model_dir)
             kwargs['ckpt_dir'] = model_dir
 
         if 'ckpt_dir' in kwargs:
             with open(os.path.join(kwargs['ckpt_dir'], 'sft_args.json'), 'r') as f:
-                kwargs['model_type'] = json.load(f)['model_type']
+                _json = json.load(f)
+                kwargs['model_type'] = _json['model_type']
+                kwargs['sft_type'] = _json['sft_type']
         deploy_args = DeployArguments(
             **{
                 key: value.split(' ') if key in kwargs_is_list and kwargs_is_list[key] else value
                 for key, value in kwargs.items()
             })
         if deploy_args.port in Runtime.get_all_ports():
             raise gr.Error(cls.locale('port_alert', cls.lang)['value'])
@@ -267,15 +270,15 @@
     @classmethod
     def deploy_model(cls, *args):
         run_command, deploy_args, log_file = cls.deploy(*args)
         os.system(run_command)
         gr.Info(cls.locale('load_alert', cls.lang)['value'])
         time.sleep(2)
         return gr.update(open=True), Runtime.refresh_tasks(log_file), [
-            deploy_args.model_type, deploy_args.template_type
+            deploy_args.model_type, deploy_args.template_type, deploy_args.sft_type
         ]
 
     @classmethod
     def update_runtime(cls):
         return gr.update(open=True), gr.update(visible=True)
 
     @classmethod
@@ -346,41 +349,52 @@
     @classmethod
     def send_message(cls, running_task, model_and_template, template_type, prompt: str, history, system, max_new_tokens,
                      temperature, top_k, top_p, repetition_penalty):
         if not model_and_template:
             gr.Warning(cls.locale('generate_alert', cls.lang)['value'])
             return '', None
         _, args = Runtime.parse_info_from_cmdline(running_task)
-        model_type, template = model_and_template
+        model_type, template, sft_type = model_and_template
         old_history, history = history or [], []
         request_config = XRequestConfig(
             temperature=temperature, top_k=top_k, top_p=top_p, repetition_penalty=repetition_penalty)
         request_config.stream = True
         request_config.stop = ['Observation:']
         stream_resp_with_history = ''
         if not template_type.endswith('generation'):
             stream_resp = inference_client(
-                model_type, prompt, old_history, system=system, port=args['port'], request_config=request_config)
+                model_type,
+                prompt,
+                old_history,
+                system=system,
+                port=args['port'],
+                adapter_name='default-lora' if sft_type in ('lora', 'longlora') else None,
+                request_config=request_config)
             for chunk in stream_resp:
                 stream_resp_with_history += chunk.choices[0].delta.content
                 qr_pair = [prompt, stream_resp_with_history]
                 total_history = old_history + [qr_pair]
                 yield '', total_history
         else:
             request_config.max_tokens = max_new_tokens
-            stream_resp = inference_client(model_type, prompt, port=args['port'], request_config=request_config)
+            stream_resp = inference_client(
+                model_type,
+                prompt,
+                port=args['port'],
+                adapter_name='default-lora' if sft_type in ('lora', 'longlora') else None,
+                request_config=request_config)
             for chunk in stream_resp:
                 stream_resp_with_history += chunk.choices[0].text
                 qr_pair = [prompt, stream_resp_with_history]
                 total_history = old_history + [qr_pair]
                 yield '', total_history
 
     @classmethod
     def generate_chat(cls, model_and_template, template_type, prompt: str, history, system, max_new_tokens, temperature,
-                      top_k, top_p, repetition_penalty):
+                      do_sample, top_k, top_p, repetition_penalty):
         if not model_and_template:
             gr.Warning(cls.locale('generate_alert', cls.lang)['value'])
             return '', None
         model, template = model_and_template
         if os.environ.get('MODELSCOPE_ENVIRONMENT') == 'studio':
             model.cuda()
         if not template_type.endswith('generation'):
@@ -389,14 +403,15 @@
             old_history = []
             history = []
 
         generation_config = GenerationConfig(
             temperature=temperature,
             top_k=top_k,
             top_p=top_p,
+            do_sample=do_sample,
             max_new_tokens=int(max_new_tokens),
             repetition_penalty=repetition_penalty)
         gen = inference_stream(
             model,
             template,
             prompt,
             history,
```

### Comparing `ms-swift-2.0.4/swift/ui/llm_infer/model.py` & `ms-swift-2.0.5/swift/ui/llm_infer/model.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/ui/llm_infer/runtime.py` & `ms-swift-2.0.5/swift/ui/llm_infer/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os.path
 import sys
 import time
 from datetime import datetime
 from typing import Dict, List, Tuple, Type
 
 import gradio as gr
+import json
 import psutil
 from gradio import Accordion, Tab
 from packaging import version
 
 from swift.ui.base import BaseUI
 from swift.utils import get_logger
 
@@ -281,8 +282,13 @@
                         else:
                             arg = all_args['model_id_or_path']
                     else:
                         arg = all_args[e.elem_id]
                 ret.append(gr.update(value=arg))
             else:
                 ret.append(gr.update())
-        return ret + [gr.update(value=None), [all_args.get('model_type'), all_args.get('template_type')]]
+        sft_type = None
+        if is_custom_path:
+            with open(os.path.join(all_args['ckpt_dir'], 'sft_args.json'), 'r') as f:
+                _json = json.load(f)
+                sft_type = _json['sft_type']
+        return ret + [gr.update(value=None), [all_args.get('model_type'), all_args.get('template_type'), sft_type]]
```

### Comparing `ms-swift-2.0.4/swift/ui/llm_train/advanced.py` & `ms-swift-2.0.5/swift/ui/llm_train/advanced.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/ui/llm_train/dataset.py` & `ms-swift-2.0.5/swift/ui/llm_train/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 from typing import Type
 
 import gradio as gr
 
 from swift.llm import DATASET_MAPPING
 from swift.ui.base import BaseUI
 
@@ -33,16 +34,16 @@
         },
         'custom_train_dataset_path': {
             'label': {
                 'zh': '自定义训练数据集路径',
                 'en': 'Custom train dataset path'
             },
             'info': {
-                'zh': '输入自定义的训练数据集路径，逗号分隔',
-                'en': 'Extra train files, split by comma'
+                'zh': '输入自定义的训练数据集路径，空格分隔',
+                'en': 'Extra train files, split by blank'
             }
         },
         'custom_val_dataset_path': {
             'label': {
                 'zh': '自定义校验数据集路径',
                 'en': 'Custom val dataset path'
             },
@@ -64,43 +65,54 @@
         'train_dataset_sample': {
             'label': {
                 'zh': '训练集采样数量',
                 'en': 'The sample size from the train dataset'
             },
             'info': {
                 'zh': '从训练集中采样一定行数进行训练',
-                'en': 'Train with the sample size from the dataset'
+                'en': 'Train with the sample size from the dataset',
             }
         },
         'val_dataset_sample': {
             'label': {
                 'zh': '验证集采样数量',
                 'en': 'The sample size from the val dataset'
             },
             'info': {
                 'zh': '从验证集中采样一定行数进行训练',
-                'en': 'Validate with the sample size from the dataset'
+                'en': 'Validate with the sample size from the dataset',
             }
         },
         'truncation_strategy': {
             'label': {
                 'zh': '数据集超长策略',
                 'en': 'Dataset truncation strategy'
             },
             'info': {
                 'zh': '如果token超长该如何处理',
                 'en': 'How to deal with the rows exceed the max length'
             }
-        }
+        },
+        'custom_dataset_info': {
+            'label': {
+                'zh': '外部数据集配置',
+                'en': 'Custom dataset config'
+            },
+            'info': {
+                'zh': '注册外部数据集的配置文件',
+                'en': 'An extra dataset config to register your own datasets'
+            }
+        },
     }
 
     @classmethod
     def do_build_ui(cls, base_tab: Type['BaseUI']):
         with gr.Row():
             gr.Dropdown(elem_id='dataset', multiselect=True, choices=list(DATASET_MAPPING.keys()), scale=20)
+            gr.Textbox(elem_id='custom_dataset_info', is_list=False, scale=20)
             gr.Textbox(elem_id='custom_train_dataset_path', is_list=True, scale=20)
             gr.Textbox(elem_id='custom_val_dataset_path', is_list=True, scale=20)
         with gr.Row():
             gr.Slider(elem_id='dataset_test_ratio', minimum=0.0, maximum=1.0, step=0.05, scale=20)
             gr.Slider(elem_id='max_length', minimum=32, maximum=8192, step=32, scale=20)
             gr.Textbox(elem_id='train_dataset_sample', scale=20)
             gr.Textbox(elem_id='val_dataset_sample', scale=20)
```

### Comparing `ms-swift-2.0.4/swift/ui/llm_train/hyper.py` & `ms-swift-2.0.5/swift/ui/llm_train/hyper.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/ui/llm_train/llm_train.py` & `ms-swift-2.0.5/swift/ui/llm_train/llm_train.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,30 +12,41 @@
 import torch
 from gradio import Accordion, Tab
 
 from swift.llm import SftArguments
 from swift.ui.base import BaseUI
 from swift.ui.llm_train.advanced import Advanced
 from swift.ui.llm_train.dataset import Dataset
+from swift.ui.llm_train.galore import Galore
 from swift.ui.llm_train.hyper import Hyper
+from swift.ui.llm_train.lisa import Lisa
+from swift.ui.llm_train.llamapro import LlamaPro
 from swift.ui.llm_train.lora import LoRA
 from swift.ui.llm_train.model import Model
 from swift.ui.llm_train.quantization import Quantization
 from swift.ui.llm_train.runtime import Runtime
 from swift.ui.llm_train.save import Save
 from swift.ui.llm_train.self_cog import SelfCog
 from swift.utils import get_logger
 
 logger = get_logger()
 
+is_spaces = True if 'SPACE_ID' in os.environ else False
+if is_spaces:
+    is_shared_ui = True if 'modelscope/swift' in os.environ['SPACE_ID'] else False
+else:
+    is_shared_ui = False
+
 
 class LLMTrain(BaseUI):
 
     group = 'llm_train'
 
+    is_studio = os.environ.get('MODELSCOPE_ENVIRONMENT') == 'studio'
+
     sub_ui = [
         Model,
         Dataset,
         Runtime,
         Save,
         LoRA,
         Hyper,
@@ -158,42 +169,34 @@
                 'en': 'neftune_noise_alpha'
             },
             'info': {
                 'zh': '使用neftune提升训练效果, 一般设置为5或者10',
                 'en': 'Use neftune to improve performance, normally the value should be 5 or 10'
             }
         },
-        'use_galore': {
+        'tuner_backend': {
             'label': {
-                'zh': '使用GaLore',
-                'en': 'Use GaLore'
+                'zh': 'Tuner backend',
+                'en': 'Tuner backend'
             },
             'info': {
-                'zh': '使用Galore来减少全参数训练的显存消耗',
-                'en': 'Use Galore to reduce GPU memory usage in full parameter training'
+                'zh': 'tuner实现框架，建议peft或者unsloth',
+                'en': 'The tuner backend, suggest to use peft or unsloth'
             }
         },
-        'galore_rank': {
-            'label': {
-                'zh': 'Galore的秩',
-                'en': 'The rank of Galore'
-            },
-        },
-        'galore_update_proj_gap': {
+        'sequence_parallel_size': {
             'label': {
-                'zh': 'Galore project matrix更新频率',
-                'en': 'The updating gap of the project matrix'
+                'zh': '序列并行分段',
+                'en': 'Sequence parallel size'
             },
+            'info': {
+                'zh': 'DDP条件下的序列并行（减小显存），需要安装ms-swift[seq_parallel]',
+                'en': 'Sequence parallel when ddp, need to install ms-swift[seq_parallel]'
+            }
         },
-        'galore_optim_per_parameter': {
-            'label': {
-                'zh': '为每个Galore Parameter创建单独的optimizer',
-                'en': 'Create unique optimizer for per Galore parameter'
-            },
-        }
     }
 
     choice_dict = BaseUI.get_choices_from_dataclass(SftArguments)
     default_dict = BaseUI.get_default_value_from_dataclass(SftArguments)
     arguments = BaseUI.get_argument_names(SftArguments)
 
     @classmethod
@@ -206,70 +209,74 @@
                 default_device = '0'
             with gr.Blocks():
                 Model.build_ui(base_tab)
                 Dataset.build_ui(base_tab)
                 Runtime.build_ui(base_tab)
                 with gr.Row():
                     gr.Dropdown(elem_id='sft_type', scale=4)
+                    gr.Dropdown(elem_id='tuner_backend', scale=4)
+                    gr.Textbox(elem_id='sequence_parallel_size', scale=4)
                     gr.Textbox(elem_id='seed', scale=4)
                     gr.Dropdown(elem_id='dtype', scale=4)
                     gr.Checkbox(elem_id='use_ddp', value=False, scale=4)
                     gr.Textbox(elem_id='ddp_num', value='2', scale=4)
                     gr.Slider(elem_id='neftune_noise_alpha', minimum=0.0, maximum=20.0, step=0.5, scale=4)
                 with gr.Row():
-                    gr.Checkbox(elem_id='use_galore', scale=4)
-                    gr.Slider(elem_id='galore_rank', minimum=8, maximum=256, step=8, scale=4)
-                    gr.Slider(elem_id='galore_update_proj_gap', minimum=10, maximum=1000, step=50, scale=4)
-                    gr.Checkbox(elem_id='galore_optim_per_parameter', scale=4)
-                with gr.Row():
                     gr.Dropdown(
                         elem_id='gpu_id',
                         multiselect=True,
                         choices=[str(i) for i in range(gpu_count)] + ['cpu'],
                         value=default_device,
                         scale=8)
                     gr.Textbox(elem_id='gpu_memory_fraction', scale=4)
-                    gr.Checkbox(elem_id='dry_run', value=False, scale=4)
+                    if is_shared_ui:
+                        gr.Checkbox(elem_id='dry_run', value=True, interactive=False, scale=4)
+                    else:
+                        gr.Checkbox(elem_id='dry_run', value=False, scale=4)
                     submit = gr.Button(elem_id='submit', scale=4, variant='primary')
 
                 Save.build_ui(base_tab)
                 LoRA.build_ui(base_tab)
                 Hyper.build_ui(base_tab)
+                Galore.build_ui(base_tab)
+                Lisa.build_ui(base_tab)
+                LlamaPro.build_ui(base_tab)
                 Quantization.build_ui(base_tab)
                 SelfCog.build_ui(base_tab)
                 Advanced.build_ui(base_tab)
-                if os.environ.get('MODELSCOPE_ENVIRONMENT') == 'studio':
+                if cls.is_studio:
                     submit.click(
                         cls.update_runtime, [],
                         [cls.element('runtime_tab'), cls.element('log')]).then(
                             cls.train_studio,
                             [value for value in cls.elements().values() if not isinstance(value, (Tab, Accordion))],
-                            [cls.element('log')],
+                            [cls.element('log')] + Runtime.all_plots + [cls.element('running_cmd')],
                             queue=True)
                 else:
                     submit.click(
                         cls.train_local,
                         [value for value in cls.elements().values() if not isinstance(value, (Tab, Accordion))], [
                             cls.element('running_cmd'),
                             cls.element('logging_dir'),
                             cls.element('runtime_tab'),
                             cls.element('running_tasks'),
                         ],
                         queue=True)
-                base_tab.element('running_tasks').change(
-                    partial(Runtime.task_changed, base_tab=base_tab), [base_tab.element('running_tasks')],
-                    [value for value in base_tab.elements().values() if not isinstance(value, (Tab, Accordion))]
-                    + [cls.element('log')] + Runtime.all_plots,
-                    cancels=Runtime.log_event)
-                Runtime.element('kill_task').click(
-                    Runtime.kill_task,
-                    [Runtime.element('running_tasks')],
-                    [Runtime.element('running_tasks')] + [Runtime.element('log')] + Runtime.all_plots,
-                    cancels=[Runtime.log_event],
-                ).then(Runtime.reset, [], [Runtime.element('logging_dir')] + [Save.element('output_dir')])
+                if not cls.is_studio:
+                    base_tab.element('running_tasks').change(
+                        partial(Runtime.task_changed, base_tab=base_tab), [base_tab.element('running_tasks')],
+                        [value for value in base_tab.elements().values() if not isinstance(value, (Tab, Accordion))]
+                        + [cls.element('log')] + Runtime.all_plots,
+                        cancels=Runtime.log_event)
+                    Runtime.element('kill_task').click(
+                        Runtime.kill_task,
+                        [Runtime.element('running_tasks')],
+                        [Runtime.element('running_tasks')] + [Runtime.element('log')] + Runtime.all_plots,
+                        cancels=[Runtime.log_event],
+                    ).then(Runtime.reset, [], [Runtime.element('logging_dir')] + [Save.element('output_dir')])
 
     @classmethod
     def update_runtime(cls):
         return gr.update(open=True), gr.update(visible=True)
 
     @classmethod
     def train(cls, *args):
@@ -338,32 +345,37 @@
         log_file = os.path.join(sft_args.logging_dir, 'run.log')
         if sys.platform == 'win32':
             if cuda_param:
                 cuda_param = f'set {cuda_param} && '
             if ddp_param:
                 ddp_param = f'set {ddp_param} && '
             run_command = f'{cuda_param}{ddp_param}start /b swift sft {params} > {log_file} 2>&1'
-        elif os.environ.get('MODELSCOPE_ENVIRONMENT') == 'studio':
+        elif cls.is_studio:
             run_command = f'{cuda_param} {ddp_param} swift sft {params}'
         else:
             run_command = f'{cuda_param} {ddp_param} nohup swift sft {params} > {log_file} 2>&1 &'
         logger.info(f'Run training: {run_command}')
         return run_command, sft_args, other_kwargs
 
     @classmethod
     def train_studio(cls, *args):
         run_command, sft_args, other_kwargs = cls.train(*args)
-        if os.environ.get('MODELSCOPE_ENVIRONMENT') == 'studio':
+        if not other_kwargs['dry_run']:
             lines = collections.deque(maxlen=int(os.environ.get('MAX_LOG_LINES', 50)))
             process = Popen(run_command, shell=True, stdout=PIPE, stderr=STDOUT)
             with process.stdout:
                 for line in iter(process.stdout.readline, b''):
                     line = line.decode('utf-8')
                     lines.append(line)
-                    yield '\n'.join(lines)
+                    yield ['\n'.join(lines)] + Runtime.plot(run_command) + [run_command]
+        else:
+            yield [
+                'Current is dryrun mode so you can only view the training cmd, please duplicate this space to '
+                'do training or use with inference.'
+            ] + [None] * len(Runtime.sft_plot) + [run_command]
 
     @classmethod
     def train_local(cls, *args):
         run_command, sft_args, other_kwargs = cls.train(*args)
         if not other_kwargs['dry_run']:
             os.makedirs(sft_args.logging_dir, exist_ok=True)
             os.system(run_command)
```

### Comparing `ms-swift-2.0.4/swift/ui/llm_train/lora.py` & `ms-swift-2.0.5/swift/ui/llm_train/lora.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/ui/llm_train/model.py` & `ms-swift-2.0.5/swift/ui/llm_train/model.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/ui/llm_train/quantization.py` & `ms-swift-2.0.5/swift/ui/llm_train/quantization.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,27 @@
 
     group = 'llm_train'
 
     locale_dict = {
         'quantization_tab': {
             'label': {
                 'zh': '量化参数',
-                'en': 'Quantization'
+                'en': 'Quantization settings'
             },
         },
+        'quant_method': {
+            'label': {
+                'zh': '量化方式',
+                'en': 'Quantization method'
+            },
+            'info': {
+                'zh': '如果制定了量化位数，本参数默认为bnb',
+                'en': 'Default is bnb if quantization_bit is specified'
+            }
+        },
         'quantization_bit': {
             'label': {
                 'zh': '量化bit数',
                 'en': 'Quantization bit'
             },
             'info': {
                 'zh': '设置量化bit数, 0代表不进行量化',
@@ -47,10 +57,11 @@
     }
 
     @classmethod
     def do_build_ui(cls, base_tab: Type['BaseUI']):
         with gr.Accordion(elem_id='quantization_tab', open=False):
             with gr.Row():
                 gr.Dropdown(elem_id='quantization_bit')
+                gr.Dropdown(elem_id='quant_method')
                 gr.Dropdown(elem_id='bnb_4bit_comp_dtype')
                 gr.Dropdown(elem_id='bnb_4bit_quant_type')
                 gr.Checkbox(elem_id='bnb_4bit_use_double_quant')
```

### Comparing `ms-swift-2.0.4/swift/ui/llm_train/runtime.py` & `ms-swift-2.0.5/swift/ui/llm_train/runtime.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,14 +26,16 @@
 
     group = 'llm_train'
 
     all_plots = None
 
     log_event = None
 
+    is_studio = os.environ.get('MODELSCOPE_ENVIRONMENT') == 'studio'
+
     sft_plot = [
         {
             'name': 'train/loss',
             'smooth': 0.9,
         },
         {
             'name': 'train/acc',
@@ -183,57 +185,60 @@
 
     @classmethod
     def do_build_ui(cls, base_tab: Type['BaseUI']):
         with gr.Accordion(elem_id='runtime_tab', open=False, visible=True):
             with gr.Blocks():
                 with gr.Row():
                     gr.Textbox(elem_id='running_cmd', lines=1, scale=20, interactive=False, max_lines=1)
-                    gr.Textbox(elem_id='logging_dir', lines=1, scale=20, max_lines=1)
-                    gr.Button(elem_id='show_log', scale=2, variant='primary')
-                    gr.Button(elem_id='stop_show_log', scale=2)
-                    gr.Textbox(elem_id='tb_url', lines=1, scale=10, interactive=False, max_lines=1)
-                    gr.Button(elem_id='start_tb', scale=2, variant='primary')
-                    gr.Button(elem_id='close_tb', scale=2)
+                    if not cls.is_studio:
+                        gr.Textbox(elem_id='logging_dir', lines=1, scale=20, max_lines=1)
+                        gr.Button(elem_id='show_log', scale=2, variant='primary')
+                        gr.Button(elem_id='stop_show_log', scale=2)
+                        gr.Textbox(elem_id='tb_url', lines=1, scale=10, interactive=False, max_lines=1)
+                        gr.Button(elem_id='start_tb', scale=2, variant='primary')
+                        gr.Button(elem_id='close_tb', scale=2)
                 with gr.Row():
                     gr.Textbox(elem_id='log', lines=6, visible=False)
-                with gr.Row():
-                    gr.Dropdown(elem_id='running_tasks', scale=10)
-                    gr.Button(elem_id='refresh_tasks', scale=1)
-                    gr.Button(elem_id='kill_task', scale=1)
+                if not cls.is_studio:
+                    with gr.Row():
+                        gr.Dropdown(elem_id='running_tasks', scale=10)
+                        gr.Button(elem_id='refresh_tasks', scale=1)
+                        gr.Button(elem_id='kill_task', scale=1)
 
                 with gr.Row():
                     cls.all_plots = []
                     for k in Runtime.sft_plot:
                         name = k['name']
                         cls.all_plots.append(gr.Plot(elem_id=name, label=name))
 
-                cls.log_event = base_tab.element('show_log').click(
-                    Runtime.update_log, [], [cls.element('log')] + cls.all_plots).then(
-                        Runtime.wait, [base_tab.element('logging_dir'),
-                                       base_tab.element('running_tasks')], [cls.element('log')] + cls.all_plots)
-
-                base_tab.element('stop_show_log').click(lambda: None, cancels=cls.log_event)
-
-                base_tab.element('start_tb').click(
-                    Runtime.start_tb,
-                    [base_tab.element('logging_dir')],
-                    [base_tab.element('tb_url')],
-                )
-
-                base_tab.element('close_tb').click(
-                    Runtime.close_tb,
-                    [base_tab.element('logging_dir')],
-                    [],
-                )
-
-                base_tab.element('refresh_tasks').click(
-                    Runtime.refresh_tasks,
-                    [base_tab.element('running_tasks')],
-                    [base_tab.element('running_tasks')],
-                )
+                if not cls.is_studio:
+                    cls.log_event = base_tab.element('show_log').click(
+                        Runtime.update_log, [], [cls.element('log')] + cls.all_plots).then(
+                            Runtime.wait, [base_tab.element('logging_dir'),
+                                           base_tab.element('running_tasks')], [cls.element('log')] + cls.all_plots)
+
+                    base_tab.element('stop_show_log').click(lambda: None, cancels=cls.log_event)
+
+                    base_tab.element('start_tb').click(
+                        Runtime.start_tb,
+                        [base_tab.element('logging_dir')],
+                        [base_tab.element('tb_url')],
+                    )
+
+                    base_tab.element('close_tb').click(
+                        Runtime.close_tb,
+                        [base_tab.element('logging_dir')],
+                        [],
+                    )
+
+                    base_tab.element('refresh_tasks').click(
+                        Runtime.refresh_tasks,
+                        [base_tab.element('running_tasks')],
+                        [base_tab.element('running_tasks')],
+                    )
 
     @classmethod
     def update_log(cls):
         return [gr.update(visible=True)] * (len(Runtime.sft_plot) + 1)
 
     @classmethod
     def wait(cls, logging_dir, task):
@@ -358,19 +363,20 @@
 
         return f'pid:{pid}/create:{create_time_formatted}' \
                f'/running:{format_time(ts-create_time)}/cmd:{" ".join(proc.cmdline())}'
 
     @staticmethod
     def parse_info_from_cmdline(task):
         pid = None
-        for i in range(3):
-            slash = task.find('/')
-            if i == 0:
-                pid = task[:slash].split(':')[1]
-            task = task[slash + 1:]
+        if '/cmd:' in task:
+            for i in range(3):
+                slash = task.find('/')
+                if i == 0:
+                    pid = task[:slash].split(':')[1]
+                task = task[slash + 1:]
         args = task.split('swift sft')[1]
         args = [arg.strip() for arg in args.split('--') if arg.strip()]
         all_args = {}
         for i in range(len(args)):
             space = args[i].find(' ')
             splits = args[i][:space], args[i][space + 1:]
             all_args[splits[0]] = splits[1]
@@ -423,14 +429,16 @@
 
     @staticmethod
     def plot(task):
         if not task:
             return [None] * len(Runtime.sft_plot)
         _, all_args = Runtime.parse_info_from_cmdline(task)
         tb_dir = all_args['logging_dir']
+        if not os.path.exists(tb_dir):
+            return [None] * len(Runtime.sft_plot)
         fname = [
             fname for fname in os.listdir(tb_dir)
             if os.path.isfile(os.path.join(tb_dir, fname)) and fname.startswith('events.out')
         ]
         if fname:
             fname = fname[0]
         else:
```

### Comparing `ms-swift-2.0.4/swift/ui/llm_train/save.py` & `ms-swift-2.0.5/swift/ui/llm_train/save.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/ui/llm_train/self_cog.py` & `ms-swift-2.0.5/swift/ui/llm_train/self_cog.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/ui/llm_train/utils.py` & `ms-swift-2.0.5/swift/ui/llm_train/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 import asyncio
 import sys
 from asyncio.subprocess import PIPE, STDOUT
-from dataclasses import fields
-
-from swift.llm import SftArguments
 
 
 async def run_and_get_log(*args, timeout=None):
     process = await asyncio.create_subprocess_exec(*args, stdout=PIPE, stderr=STDOUT)
     lines = []
     while True:
         try:
```

### Comparing `ms-swift-2.0.4/swift/utils/__init__.py` & `ms-swift-2.0.5/swift/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/utils/constants.py` & `ms-swift-2.0.5/swift/utils/constants.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/utils/hub.py` & `ms-swift-2.0.5/swift/utils/hub.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/utils/import_utils.py` & `ms-swift-2.0.5/swift/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/utils/io_utils.py` & `ms-swift-2.0.5/swift/utils/io_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/utils/logger.py` & `ms-swift-2.0.5/swift/utils/logger.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/utils/metric.py` & `ms-swift-2.0.5/swift/utils/metric.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/utils/np_utils.py` & `ms-swift-2.0.5/swift/utils/np_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/utils/run_utils.py` & `ms-swift-2.0.5/swift/utils/run_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/utils/tb_utils.py` & `ms-swift-2.0.5/swift/utils/tb_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/swift/utils/torch_utils.py` & `ms-swift-2.0.5/swift/utils/torch_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 
 
 def is_mp() -> bool:
     if use_torchacc():
         return False
     n_gpu = torch.cuda.device_count()
     local_world_size = get_dist_setting()[3]
-    assert n_gpu % local_world_size == 0
+    assert n_gpu % local_world_size == 0, f'n_gpu: {n_gpu}, local_world_size: {local_world_size}'
     if n_gpu // local_world_size >= 2:
         return True
     return False
 
 
 def is_ddp_plus_mp() -> bool:
     if not is_dist():
```

### Comparing `ms-swift-2.0.4/swift/utils/utils.py` & `ms-swift-2.0.5/swift/utils/utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/tests/hub/test_check_model.py` & `ms-swift-2.0.5/tests/hub/test_check_model.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/tests/llm/test_dataset.py` & `ms-swift-2.0.5/tests/llm/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/tests/llm/test_run.py` & `ms-swift-2.0.5/tests/llm/test_run.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 if __name__ == '__main__':
     import os
     os.environ['CUDA_VISIBLE_DEVICES'] = '0'
+    os.environ['HF_ENDPOINT'] = 'https://hf-mirror.com'
 
 import os
 import shutil
 import tempfile
 import time
 import unittest
 from functools import partial
@@ -34,20 +35,53 @@
         print(f'Testing {type(self).__name__}.{self._testMethodName}')
         self._tmp_dir = tempfile.TemporaryDirectory()
         self.tmp_dir = self._tmp_dir.name
 
     def tearDown(self):
         shutil.rmtree(self.tmp_dir)
 
+    def test_template(self):
+        if not __name__ == '__main__':
+            # ignore citest error in github
+            return
+        torch.cuda.empty_cache()
+        output = sft_main(
+            SftArguments(
+                model_type=ModelType.qwen1half_1_8b,
+                model_id_or_path='../models/Qwen1.5-1.8B',
+                template_type='qwen',
+                sft_type='full',
+                dataset=f'{DatasetName.jd_sentiment_zh}#200',
+                eval_steps=5))
+        best_model_checkpoint = output['best_model_checkpoint']
+        torch.cuda.empty_cache()
+        result = infer_main(
+            InferArguments(ckpt_dir=best_model_checkpoint, load_dataset_config=True, val_dataset_sample=2))
+        assert len(result['result'][0]['response']) < 20
+
     def test_basic(self):
         output_dir = 'output'
         quantization_bit_list = [0, 4]
+        train_dataset_fnames = [
+            'alpaca.csv', 'chatml.jsonl', 'swift_pre.jsonl', 'swift_single.csv', 'swift_multi.jsonl',
+            'swift_multi.json#2'
+        ]
+        folder = os.path.join(os.path.dirname(__file__), 'data')
+        dataset = [
+            f'MS::{DatasetName.alpaca_zh}#20',
+            f'{DatasetName.jd_sentiment_zh}#20',
+            'AI-ModelScope/alpaca-gpt4-data-zh#20',
+            'HF::llm-wizard/alpaca-gpt4-data-zh#20',
+            'hurner/alpaca-gpt4-data-zh#20',
+            'HF::shibing624/alpaca-zh#20',
+        ] + [os.path.join(folder, fname) for fname in train_dataset_fnames]
         if not __name__ == '__main__':
             output_dir = self.tmp_dir
             quantization_bit_list = [4]
+            dataset = dataset[:2]
         model_type = ModelType.chatglm3_6b
         for quantization_bit in quantization_bit_list:
             if quantization_bit == 4 and version.parse(transformers.__version__) >= version.parse('4.38'):
                 continue
             predict_with_generate = True
             if quantization_bit == 0:
                 predict_with_generate = False
@@ -56,35 +90,35 @@
                 template_type='AUTO',
                 lora_target_modules=['AUTO', 'EMBEDDING'],
                 quantization_bit=quantization_bit,
                 batch_size=2,
                 eval_steps=5,
                 adam_beta2=0.95,
                 check_dataset_strategy='warning',
-                train_dataset_sample=200,
                 predict_with_generate=predict_with_generate,
-                dataset=[DatasetName.jd_sentiment_zh],
-                include_num_input_tokens_seen=True,
+                dataset=dataset,
                 output_dir=output_dir,
+                include_num_input_tokens_seen=True,
                 gradient_checkpointing=True)
             self.assertTrue(sft_args.gradient_accumulation_steps == 8)
             torch.cuda.empty_cache()
             output = sft_main(sft_args)
             print(output)
             best_model_checkpoint = output['best_model_checkpoint']
             print(f'best_model_checkpoint: {best_model_checkpoint}')
             if __name__ == '__main__':
                 infer_args = InferArguments(
                     ckpt_dir=best_model_checkpoint,
-                    merge_lora_and_save={
+                    merge_lora={
                         0: True,
                         4: False
                     }[quantization_bit],
+                    merge_device_map='cpu',
                     load_dataset_config=NO_EVAL_HUMAN,
-                    show_dataset_sample=5)
+                    val_dataset_sample=5)
                 torch.cuda.empty_cache()
                 result = infer_main(infer_args)
                 print(result)
         # if __name__ == '__main__':
         #     app_ui_main(infer_args)
 
     def test_loss_matching(self):
@@ -97,47 +131,48 @@
             if tuner_backend == 'swift':
                 bool_var = True
             else:
                 bool_var = False
             torch.cuda.empty_cache()
             output = sft_main([
                 '--model_type', ModelType.qwen_7b_chat, '--eval_steps', '5', '--tuner_backend', tuner_backend,
-                '--train_dataset_sample', '200', '--dataset', DatasetName.leetcode_python_en, '--output_dir',
-                output_dir, '--gradient_checkpointing', 'true', '--max_new_tokens', '100', '--use_flash_attn', 'true',
+                '--dataset', f'{DatasetName.leetcode_python_en}#200', '--output_dir', output_dir,
+                '--gradient_checkpointing', 'true', '--max_new_tokens', '100', '--use_flash_attn', 'true',
                 '--lora_target_modules', 'ALL', '--seed', '0', '--lora_bias_trainable', 'all', '--lora_modules_to_save',
                 'EMBEDDING', 'LN', 'lm_head'
             ])
             best_model_checkpoint = output['best_model_checkpoint']
             print(f'best_model_checkpoint: {best_model_checkpoint}')
             load_dataset_config = str(bool_var or NO_EVAL_HUMAN)
             if load_dataset_config:
-                show_dataset_sample = 2
+                val_dataset_sample = 2
             else:
-                show_dataset_sample = -1
+                val_dataset_sample = -1
             torch.cuda.empty_cache()
             infer_main([
-                '--ckpt_dir', best_model_checkpoint, '--show_dataset_sample',
-                str(show_dataset_sample), '--max_new_tokens', '100', '--use_flash_attn', 'false', '--verbose',
-                str(not bool_var), '--merge_lora_and_save',
+                '--ckpt_dir', best_model_checkpoint, '--val_dataset_sample',
+                str(val_dataset_sample), '--max_new_tokens', '100', '--use_flash_attn', 'false', '--verbose',
+                str(not bool_var), '--merge_lora',
                 str(bool_var), '--load_dataset_config',
                 str(load_dataset_config)
             ])
             loss = output['log_history'][-1]['train_loss']
             losses.append(loss)
         self.assertTrue(abs(losses[0] - losses[1]) < 5e-4)
         print(f'swift_loss: {losses[0]}')
         print(f'peft_loss: {losses[1]}')
+        self.assertTrue(0.95 <= losses[0] <= 1)
 
     def test_vl_audio(self):
         output_dir = 'output'
         if not __name__ == '__main__':
             # ignore citest error in github
             return
         model_type_list = [ModelType.qwen_vl_chat, ModelType.qwen_audio_chat]
-        dataset_list = [DatasetName.coco_mini_en, DatasetName.aishell1_mini_zh]
+        dataset_list = [DatasetName.coco_en_mini, DatasetName.aishell1_zh_mini]
         for model_type, dataset in zip(model_type_list, dataset_list):
             sft_args = SftArguments(
                 model_type=model_type,
                 template_type='AUTO',
                 eval_steps=5,
                 check_dataset_strategy='warning',
                 lora_target_modules='ALL',
@@ -155,15 +190,15 @@
             infer_args = InferArguments(
                 ckpt_dir=best_model_checkpoint,
                 load_dataset_config=True,
                 stream={
                     ModelType.qwen_vl_chat: True,
                     ModelType.qwen_audio_chat: False
                 }[model_type],
-                show_dataset_sample=5)
+                val_dataset_sample=5)
             # merge_lora_main(infer_args)  # TODO: ERROR FIX
             torch.cuda.empty_cache()
             result = infer_main(infer_args)
             print(result)
 
     def test_custom_dataset(self):
         if not __name__ == '__main__':
@@ -171,40 +206,43 @@
             return
         train_dataset_fnames = [
             'alpaca.csv', 'chatml.jsonl', 'swift_pre.jsonl', 'swift_single.csv', 'swift_multi.jsonl', 'swift_multi.json'
         ]
         val_dataset_fnames = [
             'alpaca.jsonl', 'alpaca2.csv', 'conversations.jsonl', 'swift_pre.csv', 'swift_single.jsonl'
         ]
-        mixture_dataset = val_dataset_fnames
         folder = os.path.join(os.path.dirname(__file__), 'data')
         resume_from_checkpoint = None
-        for num_train_epochs in [5, 10]:
+        for num_train_epochs in [1, 2]:
             sft_args = SftArguments(
                 model_type='qwen-7b-chat',
+                dataset=['self-cognition#20'],
                 custom_train_dataset_path=[os.path.join(folder, fname) for fname in train_dataset_fnames],
-                train_dataset_mix_ds=[os.path.join(folder, fname) for fname in mixture_dataset],
-                train_dataset_mix_ratio=0.1,
+                custom_val_dataset_path=[os.path.join(folder, fname) for fname in val_dataset_fnames],
+                lora_target_modules='ALL',
                 resume_from_checkpoint=resume_from_checkpoint,
                 num_train_epochs=num_train_epochs,
+                model_name='小黄',
+                model_author='魔搭',
                 check_dataset_strategy='warning')
+
             torch.cuda.empty_cache()
             result = sft_main(sft_args)
             best_model_checkpoint = result['best_model_checkpoint']
             resume_from_checkpoint = result['last_model_checkpoint']
 
         for load_args_from_ckpt_dir in [True, False]:
             kwargs = {}
             if load_args_from_ckpt_dir is False:
                 kwargs = {'model_type': 'qwen-7b-chat'}
             infer_args = InferArguments(
                 ckpt_dir=best_model_checkpoint,
                 load_args_from_ckpt_dir=load_args_from_ckpt_dir,
                 load_dataset_config=load_args_from_ckpt_dir and NO_EVAL_HUMAN,
-                merge_lora_and_save=load_args_from_ckpt_dir,
+                merge_lora=load_args_from_ckpt_dir,
                 val_dataset_sample=-1,
                 custom_val_dataset_path=[os.path.join(folder, fname) for fname in val_dataset_fnames],
                 **kwargs)
             torch.cuda.empty_cache()
             infer_main(infer_args)
 
     def test_self_cognition(self):
@@ -232,15 +270,15 @@
             best_model_checkpoint = output['best_model_checkpoint']
             print(f'last_model_checkpoint: {last_model_checkpoint}')
             print(f'best_model_checkpoint: {best_model_checkpoint}')
             ckpt_dir = best_model_checkpoint or last_model_checkpoint
             if len(dataset) == 0:
                 continue
             infer_args = InferArguments(
-                ckpt_dir=ckpt_dir, show_dataset_sample=2, verbose=False, load_dataset_config=True)
+                ckpt_dir=ckpt_dir, val_dataset_sample=2, verbose=False, load_dataset_config=True)
             # merge_lora_main(infer_args)
             torch.cuda.empty_cache()
             result = infer_main(infer_args)
             print(result)
 
     def test_cogagent_instruct(self):
         if not __name__ == '__main__':
@@ -249,15 +287,15 @@
         quantization_bit = 4
         if version.parse(transformers.__version__) >= version.parse('4.38'):
             quantization_bit = 0
         torch.cuda.empty_cache()
         output = sft_main(
             SftArguments(
                 model_type=ModelType.cogagent_18b_instruct,
-                dataset=DatasetName.coco_mini_en_2,
+                dataset=DatasetName.coco_en_2_mini,
                 train_dataset_sample=100,
                 lora_target_modules='ALL',
                 eval_steps=5,
                 quantization_bit=quantization_bit))
         best_model_checkpoint = output['best_model_checkpoint']
         torch.cuda.empty_cache()
         infer_main(InferArguments(ckpt_dir=best_model_checkpoint, load_dataset_config=True, val_dataset_sample=2))
@@ -266,15 +304,15 @@
         if not __name__ == '__main__':
             # ignore citest error in github
             return
         torch.cuda.empty_cache()
         output = sft_main(
             SftArguments(
                 model_type=ModelType.internlm_xcomposer2_7b_chat,
-                dataset=DatasetName.coco_mini_en,
+                dataset=DatasetName.coco_en_mini,
                 lora_target_modules='DEFAULT',
                 train_dataset_sample=100,
                 eval_steps=5))
         best_model_checkpoint = output['best_model_checkpoint']
         torch.cuda.empty_cache()
         infer_main(InferArguments(ckpt_dir=best_model_checkpoint, load_dataset_config=True, val_dataset_sample=2))
 
@@ -302,15 +340,15 @@
             # ignore citest error in github
             return
         torch.cuda.empty_cache()
         output = dpo_main(
             DPOArguments(
                 model_type=ModelType.qwen_1_8b_chat,
                 sft_type='full',
-                dataset=DatasetName.hh_rlhf_cn_harmless_base_cn,
+                dataset='hh-rlhf-cn-harmless-base-cn',
                 train_dataset_sample=100,
                 eval_steps=5))
         best_model_checkpoint = output['best_model_checkpoint']
         torch.cuda.empty_cache()
         infer_main(InferArguments(ckpt_dir=best_model_checkpoint, load_dataset_config=True, val_dataset_sample=2))
 
     def test_pai_compat(self):
@@ -458,14 +496,15 @@
                 hub_model_id=self.hub_model_id,
                 overwrite_output_dir=True,
                 save_steps=10,
                 save_total_limit=2,
                 metric_for_best_model='loss',
                 greater_is_better=False,
                 gradient_accumulation_steps=1,
+                logging_steps=5,
                 eval_steps=10,
                 save_only_model=save_only_model)
         trainer_args._n_gpu = 1
         trainer = BertTrainer(model, trainer_args, data_collator, train_dataset, val_dataset, tokenizer)
         self.hub_model_id = trainer_args.hub_model_id
         trainer.train()
         if trainer_args.push_to_hub:
```

### Comparing `ms-swift-2.0.4/tests/llm/test_template.py` & `ms-swift-2.0.5/tests/llm/test_template.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/tests/llm/test_utils.py` & `ms-swift-2.0.5/tests/llm/test_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/tests/llm/test_vllm_utils.py` & `ms-swift-2.0.5/tests/llm/test_vllm_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/tests/model_tag.py` & `ms-swift-2.0.5/tests/model_tag.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/tests/run.py` & `ms-swift-2.0.5/tests/run.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/tests/test_utils.py` & `ms-swift-2.0.5/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/tests/tuners/test_extra_state_dict.py` & `ms-swift-2.0.5/tests/tuners/test_extra_state_dict.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/tests/tuners/test_merged_linear.py` & `ms-swift-2.0.5/tests/tuners/test_merged_linear.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/tests/tuners/test_neft.py` & `ms-swift-2.0.5/tests/tuners/test_neft.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/tests/tuners/test_peft.py` & `ms-swift-2.0.5/tests/tuners/test_peft.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/tests/tuners/test_rome.py` & `ms-swift-2.0.5/tests/tuners/test_rome.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/tests/tuners/test_scetuning.py` & `ms-swift-2.0.5/tests/tuners/test_scetuning.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/tests/tuners/test_swift_base.py` & `ms-swift-2.0.5/tests/tuners/test_swift_base.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/tests/tuners/test_swift_device_map.py` & `ms-swift-2.0.5/tests/tuners/test_swift_device_map.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/tests/tuners/test_swift_restuning.py` & `ms-swift-2.0.5/tests/tuners/test_swift_restuning.py`

 * *Files identical despite different names*

### Comparing `ms-swift-2.0.4/tests/utils/test_io_utils.py` & `ms-swift-2.0.5/tests/utils/test_io_utils.py`

 * *Files identical despite different names*

