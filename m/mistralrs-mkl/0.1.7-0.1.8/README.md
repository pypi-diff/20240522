# Comparing `tmp/mistralrs_mkl-0.1.7.tar.gz` & `tmp/mistralrs_mkl-0.1.8.tar.gz`

## Comparing `mistralrs_mkl-0.1.7.tar` & `mistralrs_mkl-0.1.8.tar`

### file list

```diff
@@ -1,83 +1,81 @@
--rw-r--r--   0     1001      127      794 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-lora/Cargo.toml
--rw-r--r--   0     1001      127        0 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-lora/README.md
--rw-r--r--   0     1001      127     2429 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-lora/src/layer.rs
--rw-r--r--   0     1001      127     8618 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-lora/src/lib.rs
--rw-r--r--   0     1001      127    11219 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-lora/src/loralinear.rs
--rw-r--r--   0     1001      127    11929 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-lora/src/qloralinear.rs
--rw-r--r--   0     1001      127     2063 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/Cargo.toml
--rw-r--r--   0     1001      127        0 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/README.md
--rw-r--r--   0     1001      127      133 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/aici/README.md
--rw-r--r--   0     1001      127     6551 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/aici/bintokens.rs
--rw-r--r--   0     1001      127      320 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/aici/bytes.rs
--rw-r--r--   0     1001      127    15100 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/aici/cfg.rs
--rw-r--r--   0     1001      127     9819 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/aici/lex.rs
--rw-r--r--   0     1001      127      179 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/aici/mod.rs
--rw-r--r--   0     1001      127     2447 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/aici/recognizer.rs
--rw-r--r--   0     1001      127     1696 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/aici/rx.rs
--rw-r--r--   0     1001      127     3094 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/aici/svob.rs
--rw-r--r--   0     1001      127    17311 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/aici/toktree.rs
--rw-r--r--   0     1001      127     4674 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/device_map.rs
--rw-r--r--   0     1001      127    21173 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/engine/mod.rs
--rw-r--r--   0     1001      127    12620 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/layers.rs
--rw-r--r--   0     1001      127     7871 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/lib.rs
--rw-r--r--   0     1001      127     8538 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/model_loader.rs
--rw-r--r--   0     1001      127    10309 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/model_selected.rs
--rw-r--r--   0     1001      127    15657 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/gemma.rs
--rw-r--r--   0     1001      127    14521 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/llama.rs
--rw-r--r--   0     1001      127    16089 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/mistral.rs
--rw-r--r--   0     1001      127    20876 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/mixtral.rs
--rw-r--r--   0     1001      127     2877 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/mod.rs
--rw-r--r--   0     1001      127    15016 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/phi2.rs
--rw-r--r--   0     1001      127    15712 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/phi3.rs
--rw-r--r--   0     1001      127    18564 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/quantized_llama.rs
--rw-r--r--   0     1001      127     9221 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/quantized_phi2.rs
--rw-r--r--   0     1001      127    11195 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/quantized_phi3.rs
--rw-r--r--   0     1001      127    14488 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/models/qwen2.rs
--rw-r--r--   0     1001      127     5266 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/cache_manager.rs
--rw-r--r--   0     1001      127     5911 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/chat_template.rs
--rw-r--r--   0     1001      127    15865 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/ggml.rs
--rw-r--r--   0     1001      127    22111 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/gguf.rs
--rw-r--r--   0     1001      127    23366 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/loaders.rs
--rw-r--r--   0     1001      127    11539 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/macros.rs
--rw-r--r--   0     1001      127    45316 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/mod.rs
--rw-r--r--   0     1001      127    13640 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/normal.rs
--rw-r--r--   0     1001      127     3781 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/sampling.rs
--rw-r--r--   0     1001      127     9717 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/sampling_pipeline.rs
--rw-r--r--   0     1001      127    17616 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/speculative.rs
--rw-r--r--   0     1001      127     6693 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/prefix_cacher.rs
--rw-r--r--   0     1001      127     2116 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/request.rs
--rw-r--r--   0     1001      127     3848 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/response.rs
--rw-r--r--   0     1001      127    14833 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/sampler.rs
--rw-r--r--   0     1001      127     9630 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/scheduler.rs
--rw-r--r--   0     1001      127    18535 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/sequence.rs
--rw-r--r--   0     1001      127    14577 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/toml_selector.rs
--rw-r--r--   0     1001      127     7848 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/utils/mod.rs
--rw-r--r--   0     1001      127     1716 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/utils/tokens.rs
--rw-r--r--   0     1001      127     6749 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/utils/varbuilder_utils.rs
--rw-r--r--   0     1001      127    11049 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/classifier.rs
--rw-r--r--   0     1001      127     1544 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/config.rs
--rw-r--r--   0     1001      127    26953 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/gemma.rs
--rw-r--r--   0     1001      127    26176 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/llama.rs
--rw-r--r--   0     1001      127    27604 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/mistral.rs
--rw-r--r--   0     1001      127    33531 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/mixtral.rs
--rw-r--r--   0     1001      127     4388 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/mod.rs
--rw-r--r--   0     1001      127    25539 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/phi2.rs
--rw-r--r--   0     1001      127    25038 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/phi3.rs
--rw-r--r--   0     1001      127    36716 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/quantized_llama.rs
--rw-r--r--   0     1001      127    19395 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/quantized_phi3.rs
--rw-r--r--   0        0        0      907 1970-01-01 00:00:00.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/Cargo.toml
--rw-r--r--   0     1001      127      686 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/.gitignore
--rw-r--r--   0     1001      127     3358 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/API.md
--rw-r--r--   0     1001      127      927 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/Cargo_template.toml
--rw-r--r--   0     1001      127     3755 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/README.md
--rw-r--r--   0     1001      127       71 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/build.rs
--rw-r--r--   0     1001      127     8688 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/mistralrs.pyi
--rw-r--r--   0     1001      127      530 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/pyproject_template.toml
--rw-r--r--   0     1001      127    29216 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/src/lib.rs
--rw-r--r--   0     1001      127     1672 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/src/stream.rs
--rw-r--r--   0     1001      127     3020 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/src/which.rs
--rwxr-xr-x   0     1001      127     2203 2024-05-14 12:13:37.000000 mistralrs_mkl-0.1.7/mistralrs-pyo3/upload.py
--rw-r--r--   0     1001      127   100818 2024-05-14 12:14:03.000000 mistralrs_mkl-0.1.7/Cargo.lock
--rw-r--r--   0        0        0     1275 1970-01-01 00:00:00.000000 mistralrs_mkl-0.1.7/Cargo.toml
--rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 mistralrs_mkl-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     4449 1970-01-01 00:00:00.000000 mistralrs_mkl-0.1.7/PKG-INFO
+-rw-r--r--   0     1001      127     2030 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/Cargo.toml
+-rw-r--r--   0     1001      127        0 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/README.md
+-rw-r--r--   0     1001      127      133 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/aici/README.md
+-rw-r--r--   0     1001      127     6551 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/aici/bintokens.rs
+-rw-r--r--   0     1001      127      320 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/aici/bytes.rs
+-rw-r--r--   0     1001      127    15100 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/aici/cfg.rs
+-rw-r--r--   0     1001      127     9819 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/aici/lex.rs
+-rw-r--r--   0     1001      127      179 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/aici/mod.rs
+-rw-r--r--   0     1001      127     2447 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/aici/recognizer.rs
+-rw-r--r--   0     1001      127     1696 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/aici/rx.rs
+-rw-r--r--   0     1001      127     3094 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/aici/svob.rs
+-rw-r--r--   0     1001      127    17311 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/aici/toktree.rs
+-rw-r--r--   0     1001      127     4674 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/device_map.rs
+-rw-r--r--   0     1001      127    20948 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/engine/mod.rs
+-rw-r--r--   0     1001      127    17719 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/layers.rs
+-rw-r--r--   0     1001      127     9967 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/lib.rs
+-rw-r--r--   0     1001      127    10515 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/lora/loralinear.rs
+-rw-r--r--   0     1001      127     8270 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/lora/mod.rs
+-rw-r--r--   0     1001      127    11400 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/lora/qloralinear.rs
+-rw-r--r--   0     1001      127     8538 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/model_loader.rs
+-rw-r--r--   0     1001      127    10303 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/model_selected.rs
+-rw-r--r--   0     1001      127    15418 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/models/gemma.rs
+-rw-r--r--   0     1001      127    13814 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/models/llama.rs
+-rw-r--r--   0     1001      127    14765 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/models/mistral.rs
+-rw-r--r--   0     1001      127    19563 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/models/mixtral.rs
+-rw-r--r--   0     1001      127      250 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/models/mod.rs
+-rw-r--r--   0     1001      127    14639 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/models/phi2.rs
+-rw-r--r--   0     1001      127    14351 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/models/phi3.rs
+-rw-r--r--   0     1001      127    18396 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/models/quantized_llama.rs
+-rw-r--r--   0     1001      127     8978 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/models/quantized_phi2.rs
+-rw-r--r--   0     1001      127    10160 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/models/quantized_phi3.rs
+-rw-r--r--   0     1001      127    14287 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/models/qwen2.rs
+-rw-r--r--   0     1001      127    10617 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/pipeline/cache_manager.rs
+-rw-r--r--   0     1001      127     5911 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/pipeline/chat_template.rs
+-rw-r--r--   0     1001      127    16295 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/pipeline/ggml.rs
+-rw-r--r--   0     1001      127    22643 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/pipeline/gguf.rs
+-rw-r--r--   0     1001      127    23432 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/pipeline/loaders.rs
+-rw-r--r--   0     1001      127    11455 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/pipeline/macros.rs
+-rw-r--r--   0     1001      127    49160 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/pipeline/mod.rs
+-rw-r--r--   0     1001      127    14070 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/pipeline/normal.rs
+-rw-r--r--   0     1001      127     3781 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/pipeline/sampling.rs
+-rw-r--r--   0     1001      127     9717 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/pipeline/sampling_pipeline.rs
+-rw-r--r--   0     1001      127    18669 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/pipeline/speculative.rs
+-rw-r--r--   0     1001      127     6695 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/prefix_cacher.rs
+-rw-r--r--   0     1001      127     2116 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/request.rs
+-rw-r--r--   0     1001      127     4690 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/response.rs
+-rw-r--r--   0     1001      127    14936 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/sampler.rs
+-rw-r--r--   0     1001      127     9630 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/scheduler.rs
+-rw-r--r--   0     1001      127    18537 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/sequence.rs
+-rw-r--r--   0     1001      127    14571 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/toml_selector.rs
+-rw-r--r--   0     1001      127     7874 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/utils/mod.rs
+-rw-r--r--   0     1001      127     1507 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/utils/tokenizer.rs
+-rw-r--r--   0     1001      127     1716 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/utils/tokens.rs
+-rw-r--r--   0     1001      127     6746 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/utils/varbuilder_utils.rs
+-rw-r--r--   0     1001      127    11049 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/classifier.rs
+-rw-r--r--   0     1001      127     1544 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/config.rs
+-rw-r--r--   0     1001      127    26753 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/gemma.rs
+-rw-r--r--   0     1001      127    25357 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/llama.rs
+-rw-r--r--   0     1001      127    26191 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/mistral.rs
+-rw-r--r--   0     1001      127    32158 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/mixtral.rs
+-rw-r--r--   0     1001      127     4532 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/mod.rs
+-rw-r--r--   0     1001      127    25212 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/phi2.rs
+-rw-r--r--   0     1001      127    23653 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/phi3.rs
+-rw-r--r--   0     1001      127    36764 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/quantized_llama.rs
+-rw-r--r--   0     1001      127    18584 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/quantized_phi3.rs
+-rw-r--r--   0        0        0      921 1970-01-01 00:00:00.000000 mistralrs_mkl-0.1.8/mistralrs-pyo3/Cargo.toml
+-rw-r--r--   0     1001      127      686 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-pyo3/.gitignore
+-rw-r--r--   0     1001      127     3358 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-pyo3/API.md
+-rw-r--r--   0     1001      127      941 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-pyo3/Cargo_template.toml
+-rw-r--r--   0     1001      127     3755 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-pyo3/README.md
+-rw-r--r--   0     1001      127       71 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-pyo3/build.rs
+-rw-r--r--   0     1001      127     8688 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-pyo3/mistralrs.pyi
+-rw-r--r--   0     1001      127      530 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-pyo3/pyproject_template.toml
+-rw-r--r--   0     1001      127    29224 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-pyo3/src/lib.rs
+-rw-r--r--   0     1001      127     1672 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-pyo3/src/stream.rs
+-rw-r--r--   0     1001      127     3020 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-pyo3/src/which.rs
+-rwxr-xr-x   0     1001      127     2203 2024-05-16 16:33:04.000000 mistralrs_mkl-0.1.8/mistralrs-pyo3/upload.py
+-rw-r--r--   0     1001      127   100636 2024-05-16 16:33:24.000000 mistralrs_mkl-0.1.8/Cargo.lock
+-rw-r--r--   0        0        0     1278 1970-01-01 00:00:00.000000 mistralrs_mkl-0.1.8/Cargo.toml
+-rw-r--r--   0        0        0      582 1970-01-01 00:00:00.000000 mistralrs_mkl-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     4449 1970-01-01 00:00:00.000000 mistralrs_mkl-0.1.8/PKG-INFO
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-lora/src/layer.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/aici/svob.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,99 +1,127 @@
-use std::sync::Arc;
+use std::{fmt::Debug, ops::Index};
 
-use candle_core::{
-    quantized::{gguf_file, QMatMul, QTensor},
-    DType, Device, Result, Tensor,
-};
-use candle_nn::{Linear, Module};
-
-#[derive(Debug, Clone)]
-pub struct QLinear {
-    inner: QMatMul,
-    bias: Option<Tensor>,
-    dtype: DType,
+use super::bytes::TokenId;
+
+#[derive(Clone)]
+pub struct SimpleVob {
+    data: Vec<u32>,
 }
 
-impl QLinear {
-    pub fn new<R: std::io::Read + std::io::Seek>(
-        ct: &gguf_file::Content,
-        r: &mut R,
-        name: &str,
-        device: &Device,
-    ) -> Result<Self> {
-        let w = ct.tensor(r, &format!("{name}.weight"), device)?;
-        let b = ct.tensor(r, &format!("{name}.bias"), device)?;
-        let inner = QMatMul::from_qtensor(w)?;
-        let bias = b.dequantize(device)?;
-        Ok(Self {
-            inner,
-            bias: Some(bias),
-            dtype: DType::F32,
-        })
-    }
-
-    pub fn from_linear(linear: Linear) -> Self {
-        Self {
-            inner: QMatMul::Tensor(linear.weight().clone()),
-            bias: linear.bias().cloned(),
-            dtype: if linear.weight().device().is_cuda() {
-                DType::BF16
-            } else {
-                DType::F32
-            },
-        }
+impl Debug for SimpleVob {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        f.debug_struct("SimpleVob")
+            .field("len", &self.len())
+            .finish()
     }
+}
 
-    pub fn from_parts(w: Tensor, b: Option<Tensor>) -> Self {
-        let dtype = if w.device().is_cuda() {
-            DType::BF16
-        } else {
-            DType::F32
-        };
-        Self {
-            inner: QMatMul::Tensor(w),
-            bias: b,
-            dtype,
-        }
+impl Default for SimpleVob {
+    fn default() -> Self {
+        Self::new()
+    }
+}
+
+const BITS: usize = 32;
+
+impl SimpleVob {
+    pub fn new() -> Self {
+        Self { data: Vec::new() }
     }
 
-    pub fn from_qparts(w: QTensor, b: Option<Tensor>) -> Self {
-        if let Some(ref b) = b {
-            assert_eq!(b.dtype(), DType::F32);
-        }
-        Self {
-            inner: QMatMul::QTensor(Arc::new(w)),
-            bias: b,
-            dtype: DType::F32,
+    pub fn alloc(size: usize) -> Self {
+        let mut r = Self::new();
+        r.resize(size);
+        r
+    }
+
+    pub fn len(&self) -> usize {
+        self.data.len() * BITS
+    }
+
+    pub fn num_set(&self) -> usize {
+        self.data.iter().map(|x| x.count_ones() as usize).sum()
+    }
+    #[allow(clippy::cast_possible_truncation)]
+    pub fn negated(&self, size: usize) -> Self {
+        let mut r = Self::new();
+        r.data = self.data.iter().map(|x| !x).collect();
+        for i in size..r.len() {
+            // disallow tokens that are out of range
+            r.disallow_token(i as TokenId);
         }
+        r
     }
 
-    pub fn inner(&mut self) -> &mut QMatMul {
-        &mut self.inner
+    pub unsafe fn as_ptr(&self) -> *const u32 {
+        self.data.as_ptr()
     }
 
-    pub fn is_quant(&self) -> bool {
-        matches!(self.inner, QMatMul::QTensor(_))
+    #[inline(always)]
+    pub fn allow_token(&mut self, tok: TokenId) {
+        let idx = tok as usize;
+        let byte_idx = idx / BITS;
+        let bit_idx = idx % BITS;
+        self.data[byte_idx] |= 1 << bit_idx;
     }
 
-    pub fn bias(&self) -> Option<&Tensor> {
-        self.bias.as_ref()
+    #[inline(always)]
+    pub fn disallow_token(&mut self, tok: TokenId) {
+        let idx = tok as usize;
+        let byte_idx = idx / BITS;
+        let bit_idx = idx % BITS;
+        self.data[byte_idx] &= !(1 << bit_idx);
     }
-}
 
-impl Module for QLinear {
-    fn forward(&self, xs: &Tensor) -> Result<Tensor> {
-        let xs = if self.is_quant() {
-            xs.to_dtype(DType::F32)?
+    pub fn set(&mut self, tok: TokenId, val: bool) {
+        if val {
+            self.allow_token(tok);
         } else {
-            xs.clone()
-        };
-        if let Some(bias) = &self.bias {
-            self.inner
-                .forward(&xs)?
-                .broadcast_add(bias)?
-                .to_dtype(self.dtype)
+            self.disallow_token(tok);
+        }
+    }
+
+    pub fn resize(&mut self, size: usize) {
+        let new_size = size / BITS + 1;
+        assert!(new_size >= self.data.len());
+        self.data.resize(new_size, 0);
+    }
+
+    #[inline(always)]
+    pub fn is_allowed(&self, tok: TokenId) -> bool {
+        let idx = tok as usize;
+        let byte_idx = idx / 32;
+        let bit_idx = idx % 32;
+        (self.data[byte_idx] & (1 << bit_idx)) != 0
+    }
+
+    pub fn set_all(&mut self, val: bool) {
+        let val = if val { !0 } else { 0 };
+        self.data.iter_mut().for_each(|x| *x = val);
+    }
+
+    pub fn apply_to(&self, logits: &mut [f32]) {
+        for (idx, v) in self.data.iter().enumerate() {
+            if *v == 0 {
+                continue;
+            }
+            let idx = idx * BITS;
+            for bit_idx in 0..BITS {
+                if v & (1 << bit_idx) != 0 {
+                    logits[idx + bit_idx] = 0.0;
+                }
+            }
+        }
+    }
+}
+
+impl Index<usize> for SimpleVob {
+    type Output = bool;
+    #[allow(clippy::cast_possible_truncation)]
+    fn index(&self, index: usize) -> &Self::Output {
+        if self.is_allowed(index as TokenId) {
+            &true
         } else {
-            self.inner.forward(&xs)?.to_dtype(self.dtype)
+            &false
         }
     }
 }
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-lora/src/lib.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/lora/mod.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+#![allow(clippy::cast_precision_loss)]
+
 use std::{collections::HashSet, fmt::Debug, sync::Arc};
 
 use candle_core::{
     quantized::{QMatMul, QTensor},
     IndexOp, Result, Tensor, D,
 };
 use candle_nn::{init, Linear, Module, VarBuilder};
 use loralinear::LoraLinear;
 pub use qloralinear::QLoraLinear;
 use serde::Deserialize;
 
-pub mod layer;
 mod loralinear;
 mod qloralinear;
 
 use std::collections::HashMap;
 
 #[derive(Clone, Debug, Deserialize)]
 pub struct PreloadAdapter {
@@ -21,15 +22,15 @@
     pub adapter_model_id: String,
 }
 
 #[derive(Clone, Debug, Deserialize)]
 pub struct Ordering {
     #[serde(rename = "order")]
     pub adapters: Option<Vec<String>>,
-    pub layers: HashMap<String, usize>,
+    pub layers: Option<HashMap<String, usize>>,
     pub base_model_id: String,
     pub preload_adapters: Option<Vec<PreloadAdapter>>,
 }
 
 #[derive(Clone, Debug)]
 /// Configuration for LoraLinear
 pub struct LoraLinearConfig {
@@ -59,30 +60,14 @@
 
 fn apply_scalings_to_x(x: Tensor, scalings_layer: &Tensor, adapter: usize) -> Result<Tensor> {
     let scalings = scalings_layer.i((.., .., adapter))?.unsqueeze(D::Minus1)?;
     let res = x.broadcast_mul(&scalings)?;
     Ok(res)
 }
 
-impl LoraConfig {
-    pub const fn new(
-        rank: usize,
-        alpha: f64,
-        dropout: Option<f32>,
-        target_modules: HashSet<String>,
-    ) -> Self {
-        Self {
-            rank,
-            alpha,
-            dropout,
-            target_modules,
-        }
-    }
-}
-
 #[derive(Debug)]
 struct Adapter {
     a: Linear,
     b: Linear,
     scale: f64,
 }
 
@@ -138,23 +123,14 @@
             self._activate_adapters(adapter_names)?;
             Ok(1)
         } else {
             Ok(0)
         }
     }
     fn _activate_adapters(&mut self, adapters: &[String]) -> Result<()>;
-    fn has_adapter(&self, adapter: String) -> bool;
-    /// Pass the prefix for the layer (excluding .lora_?) as `module_prefix`
-    fn load_new_adapter(
-        &mut self,
-        name: String,
-        vb: VarBuilder,
-        cfg: &LoraConfig,
-        module_prefix: String,
-    ) -> Result<()>;
     fn can_load(&self) -> bool;
 }
 
 impl Merge for Linear {
     fn merge_weights(&mut self) -> Result<()> {
         Ok(())
     }
@@ -166,26 +142,14 @@
 impl AdapterSwapper for Linear {
     fn _activate_adapters(&mut self, _adapter: &[String]) -> Result<()> {
         unreachable!()
     }
     fn can_load(&self) -> bool {
         false
     }
-    fn has_adapter(&self, _adapter: String) -> bool {
-        false
-    }
-    fn load_new_adapter(
-        &mut self,
-        _name: String,
-        _vb: VarBuilder,
-        _cfg: &LoraConfig,
-        _module_prefix: String,
-    ) -> Result<()> {
-        unreachable!()
-    }
 }
 
 impl LinearLayerLike for Linear {
     fn inner(&mut self) -> &mut QMatMul {
         unreachable!()
     }
     fn bias(&self) -> Option<&Tensor> {
@@ -208,88 +172,108 @@
     }
 }
 
 #[allow(clippy::too_many_arguments)]
 pub fn linear(
     d1: usize,
     d2: usize,
-    base_vb: crate::VarBuilder,
+    base_vb: VarBuilder,
     vb: VarBuilder,
     lora_config: &[((String, String), LoraConfig)],
     count: &mut usize,
     ord: &Ordering,
     preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
 ) -> Result<Arc<dyn LinearLayerLike + Send + Sync>> {
     let prefix = vb.prefix();
     let module = prefix.split('.').last().unwrap();
 
     let linear_config = LoraLinearConfig::new(d1, d2);
     let inner = candle_nn::linear(d1, d2, base_vb.clone())?;
 
-    let target_modules = &lora_config[0].1.target_modules;
+    let target_modules = &lora_config.first().map(|c| &c.1.target_modules);
     for (_, cfg) in lora_config {
-        if &cfg.target_modules != target_modules {
+        if target_modules
+            .as_ref()
+            .is_some_and(|target_modules| &cfg.target_modules != *target_modules)
+        {
             candle_core::bail!("Expected all target modules to be the same.");
         }
     }
 
-    if !target_modules.contains(module) {
+    if !target_modules
+        .as_ref()
+        .is_some_and(|target_modules| target_modules.contains(module))
+    {
         return Ok(Arc::new(inner));
     }
     let name = prefix.split("lora_A").last().unwrap();
-    let layer = ord.layers.get(name).unwrap();
+    let layer = if let Some(ref layers) = ord.layers {
+        *layers.get(name).unwrap()
+    } else {
+        0
+    };
 
     let lorainner = LoraLinear::new(
         &inner,
         &linear_config,
         lora_config,
         &vb,
-        *layer,
+        layer,
         preload_adapters,
     )?;
     *count += 1;
     Ok(Arc::new(lorainner))
 }
 
 #[allow(clippy::too_many_arguments)]
 pub fn linear_no_bias(
     d1: usize,
     d2: usize,
-    base_vb: crate::VarBuilder,
+    base_vb: VarBuilder,
     vb: VarBuilder,
     lora_config: &[((String, String), LoraConfig)],
     count: &mut usize,
     ord: &Ordering,
     preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
 ) -> Result<Arc<dyn LinearLayerLike + Send + Sync>> {
     let prefix = vb.prefix();
     let module = prefix.split('.').last().unwrap();
 
     let linear_config = LoraLinearConfig::new(d1, d2);
     let inner = candle_nn::linear_no_bias(d1, d2, base_vb.clone())?;
 
-    let target_modules = &lora_config[0].1.target_modules;
+    let target_modules = &lora_config.first().map(|c| &c.1.target_modules);
     for (_, cfg) in lora_config {
-        if &cfg.target_modules != target_modules {
+        if target_modules
+            .as_ref()
+            .is_some_and(|target_modules| &cfg.target_modules != *target_modules)
+        {
             candle_core::bail!("Expected all target modules to be the same.");
         }
     }
 
-    if !target_modules.contains(module) {
+    if !target_modules
+        .as_ref()
+        .is_some_and(|target_modules| target_modules.contains(module))
+    {
         return Ok(Arc::new(inner));
     }
     let name = prefix.split("lora_A").last().unwrap();
-    let layer = ord.layers.get(name).unwrap();
+    let layer = if let Some(ref layers) = ord.layers {
+        *layers.get(name).unwrap()
+    } else {
+        0
+    };
 
     let lorainner = LoraLinear::new(
         &inner,
         &linear_config,
         lora_config,
         &vb,
-        *layer,
+        layer,
         preload_adapters,
     )?;
     *count += 1;
     Ok(Arc::new(lorainner))
 }
 
 fn get_maybe_topk_scalings(scalings: Tensor, layer: usize) -> Result<Tensor> {
@@ -297,16 +281,16 @@
 }
 
 #[allow(clippy::too_many_arguments)]
 pub fn linear_b(
     in_dim: usize,
     out_dim: usize,
     bias: bool,
-    base_vb: crate::VarBuilder,
-    vb: crate::VarBuilder,
+    base_vb: VarBuilder,
+    vb: VarBuilder,
     lora_config: &[((String, String), LoraConfig)],
     count: &mut usize,
     ord: &Ordering,
     preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
 ) -> Result<Arc<dyn LinearLayerLike + Send + Sync>> {
     if bias {
         linear(
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-lora/src/loralinear.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/lora/loralinear.rs`

 * *Files 3% similar despite different names*

```diff
@@ -4,29 +4,30 @@
     bail,
     quantized::{QMatMul, QTensor},
     Module, Result, Tensor,
 };
 use candle_nn::{Linear, VarBuilder};
 use either::Either;
 
-use crate::{
-    apply_scalings_to_x, get_maybe_topk_scalings, layer::QLinear, make_adapter, Adapter,
-    AdapterSwapper, LinearLayerLike, LoraConfig, LoraLinearConfig, Merge,
+use crate::layers::QLinear;
+
+use super::{
+    apply_scalings_to_x, get_maybe_topk_scalings, make_adapter, Adapter, AdapterSwapper,
+    LinearLayerLike, LoraConfig, LoraLinearConfig, Merge,
 };
 
 #[derive(Debug)]
 pub struct LoraLinear {
     old: QLinear,
     a_adapters: Either<Vec<Linear>, (Tensor, Vec<Linear>)>,
     b_adapters: Either<Vec<Linear>, (Tensor, Vec<Linear>)>,
     scale_adapters: Vec<f64>,
     layer_n: usize,
     merged: bool,
     adapters: HashMap<String, Adapter>,
-    linear_config: LoraLinearConfig,
 }
 
 impl LoraLinear {
     pub fn new(
         old: &dyn LinearLayerLike,
         linear_config: &LoraLinearConfig,
         config: &[((String, String), LoraConfig)],
@@ -108,26 +109,24 @@
                 old: QLinear::from_parts(old.weight().clone(), old.bias().cloned()),
                 a_adapters: Either::Right((a_adapters_stack.clone(), a_adapters)),
                 b_adapters: Either::Right((b_adapters_stack, b_adapters)),
                 scale_adapters,
                 layer_n,
                 merged: false,
                 adapters,
-                linear_config: linear_config.clone(),
             })
         } else {
             Ok(LoraLinear {
                 old: QLinear::from_parts(old.weight().clone(), old.bias().cloned()),
                 a_adapters: Either::Left(a_adapters),
                 b_adapters: Either::Left(b_adapters),
                 scale_adapters,
                 layer_n,
                 merged: false,
                 adapters,
-                linear_config: linear_config.clone(),
             })
         }
     }
 }
 
 impl AdapterSwapper for LoraLinear {
     fn _activate_adapters(&mut self, adapter_names: &[String]) -> Result<()> {
@@ -154,30 +153,14 @@
                     s.push(*scale);
                 }
             }
             _ => unreachable!("Adapters should not be stacked if new ones are being activated."),
         }
         Ok(())
     }
-    fn has_adapter(&self, adapter: String) -> bool {
-        self.adapters.contains_key(&adapter)
-    }
-    fn load_new_adapter(
-        &mut self,
-        name: String,
-        vb: VarBuilder,
-        cfg: &LoraConfig,
-        module_prefix: String,
-    ) -> Result<()> {
-        let a_vb = vb.set_prefix(&module_prefix).pp("lora_A".to_string());
-        let b_vb = vb.set_prefix(&module_prefix).pp("lora_B".to_string());
-        let adapter = make_adapter(a_vb, b_vb, cfg, &self.linear_config)?;
-        self.adapters.insert(name.clone(), adapter);
-        Ok(())
-    }
     fn can_load(&self) -> bool {
         true
     }
 }
 
 impl Merge for LoraLinear {
     fn get_delta_weight(&self, adapter: usize) -> Result<Tensor> {
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-lora/src/qloralinear.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/lora/qloralinear.rs`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     bail,
     quantized::{QMatMul, QTensor},
     Module, Result, Tensor,
 };
 use candle_nn::{Linear, VarBuilder};
 use either::Either;
 
-use crate::{
+use super::{
     apply_scalings_to_x, get_maybe_topk_scalings, make_adapter, Adapter, AdapterSwapper,
     LinearLayerLike, LoraConfig, LoraLinearConfig, Merge, Ordering,
 };
 
 #[derive(Debug)]
 pub struct QLoraLinear {
     old: QMatMul,
@@ -34,23 +34,26 @@
         config: &[((String, String), LoraConfig)],
         vb: &VarBuilder,
         ordering: &Ordering,
         prefix: String,
         count: &mut usize,
         preload_adapters: &Option<HashMap<String, (VarBuilder, LoraConfig)>>,
     ) -> Result<Self> {
-        let target_modules = &config[0].1.target_modules;
+        let target_modules = &config.first().map(|c| &c.1.target_modules);
         for (_, cfg) in config {
-            if &cfg.target_modules != target_modules {
+            if target_modules
+                .as_ref()
+                .is_some_and(|target_modules| &cfg.target_modules != *target_modules)
+            {
                 candle_core::bail!("Expected all target modules to be the same.");
             }
         }
 
         let module = prefix.split('.').last().unwrap();
-        if !target_modules.contains(module) {
+        if target_modules.is_some_and(|target_modules| !target_modules.contains(module)) {
             return Ok(Self {
                 old,
                 a_adapters: Either::Left(vec![]),
                 b_adapters: Either::Left(vec![]),
                 scale_adapters: vec![],
                 layer_n: usize::MAX,
                 merged: false,
@@ -106,15 +109,19 @@
                 let a_vb = vb.set_prefix(a_vb.prefix());
                 let b_vb = vb.set_prefix(b_vb.prefix());
                 let adapter = make_adapter(a_vb, b_vb, cfg, linear_config)?;
                 adapters.insert(name.clone(), adapter);
             }
         }
 
-        let layer = *ordering.layers.get(&prefix).unwrap();
+        let layer = if let Some(ref layers) = ordering.layers {
+            *layers.get(&prefix).unwrap()
+        } else {
+            0
+        };
 
         if all_same {
             let a_adapters_stack = Tensor::cat(
                 &a_adapters
                     .iter()
                     .map(|x| x.weight().unsqueeze(0))
                     .collect::<Result<Vec<_>>>()?,
@@ -184,34 +191,14 @@
                     s.push(*scale);
                 }
             }
             _ => unreachable!("Adapters should not be stacked if new ones are being activated."),
         }
         Ok(())
     }
-    fn has_adapter(&self, adapter: String) -> bool {
-        self.adapters.contains_key(&adapter)
-    }
-    fn load_new_adapter(
-        &mut self,
-        name: String,
-        vb: VarBuilder,
-        cfg: &LoraConfig,
-        module_prefix: String,
-    ) -> Result<()> {
-        if let Some(ref linear_config) = self.linear_config {
-            let a_vb = vb.set_prefix(&module_prefix).pp("lora_A".to_string());
-            let b_vb = vb.set_prefix(&module_prefix).pp("lora_B".to_string());
-            let adapter = make_adapter(a_vb, b_vb, cfg, linear_config)?;
-            self.adapters.insert(name.clone(), adapter);
-            Ok(())
-        } else {
-            bail!("Linear config not found. This means that the layer cannot have new adapters loaded.")
-        }
-    }
     fn can_load(&self) -> bool {
         self.linear_config.is_some()
     }
 }
 
 impl Merge for QLoraLinear {
     fn get_delta_weight(&self, adapter: usize) -> Result<Tensor> {
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/Cargo.toml` & `mistralrs_mkl-0.1.8/mistralrs-core/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 dirs = "5.0.1"
 hf-hub = "0.3.2"
 thiserror = "1.0.57"
 tokenizers = "0.15.2"
 tqdm = "0.7.0"
 range-checked = { git = "https://github.com/EricLBuehler/range-checked.git", version = "0.1.0" }
 chrono = "0.4.34"
-mistralrs-lora = { version = "0.1.7", path = "../mistralrs-lora" }
 minijinja = "1.0.12"
 either.workspace = true
 indexmap.workspace = true
 half = "2.4.0"
 accelerate-src = { workspace = true, optional = true }
 intel-mkl-src = { workspace = true, optional = true }
 tracing.workspace = true
@@ -40,27 +39,28 @@
 vob = "3.0.3"
 cfgrammar = "0.13.3"
 lrtable = "0.13.3"
 galil-seiferas = "0.1.5"
 clap.workspace = true
 radix_trie = "0.2.1"
 bytemuck = "1.15.0"
-pyo3.workspace = true
 rayon = "1.10.0"
 tokio.workspace = true
 tokio-rayon = "2.1.0"
 rand_isaac = "0.3.0"
 futures.workspace = true
+pyo3 = {workspace = true, optional = true }
 indicatif = { version = "0.17.8", features = ["rayon"] }
 async-trait = "0.1.80"
-once_cell = "1.19.0"
+once_cell.workspace=true
 toml = "0.8.12"
-ctrlc = "3.4.4"
+
 
 [features]
+pyo3_macros = ["pyo3"]
 cuda = ["candle-core/cuda", "candle-nn/cuda", "candle-transformers/cuda"]
 cudnn = ["candle-core/cudnn"]
 metal = ["candle-core/metal", "candle-nn/metal", "candle-transformers/metal"]
 flash-attn = ["cuda", "candle-transformers/flash-attn", "dep:candle-flash-attn"]
 accelerate = ["candle-core/accelerate", "candle-nn/accelerate", "candle-transformers/accelerate"]
 mkl = ["candle-core/mkl", "candle-nn/mkl", "candle-transformers/mkl"]
 profile = []
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/aici/bintokens.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/aici/bintokens.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/aici/cfg.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/aici/cfg.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/aici/lex.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/aici/lex.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/aici/recognizer.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/aici/recognizer.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/aici/rx.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/aici/rx.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/aici/toktree.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/aici/toktree.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/device_map.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/device_map.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/engine/mod.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/engine/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 use std::{
     collections::{HashMap, VecDeque},
-    sync::{
-        atomic::{AtomicBool, Ordering},
-        Arc,
-    },
+    sync::{atomic::AtomicBool, Arc},
     time::{Instant, SystemTime, UNIX_EPOCH},
 };
 use tokio::sync::{mpsc::Receiver, Mutex};
 
 use crate::{
     aici::{cfg::CfgParser, recognizer::StackRecognizer, rx::RecRx},
     pipeline::{AdapterInstruction, CacheInstruction},
@@ -29,15 +26,16 @@
     sampler::Sampler,
     scheduler::{Scheduler, SchedulerMethod},
     sequence::{Sequence, SequenceGroup, SequenceRecognizer, SequenceState},
     Constraint, StopTokens,
 };
 
 const SEED: u64 = 0;
-pub(crate) static TERMINATE_ALL_NEXT_STEP: AtomicBool = AtomicBool::new(false);
+/// Terminate all sequences on the next scheduling step. Be sure to reset this.
+pub static TERMINATE_ALL_NEXT_STEP: AtomicBool = AtomicBool::new(false);
 
 pub struct Engine {
     rx: Receiver<Request>,
     pipeline: Arc<Mutex<dyn Pipeline>>,
     scheduler: Scheduler<VecDeque<Sequence>>,
     id: usize,
     truncate_sequence: bool,
@@ -54,24 +52,17 @@
         pipeline: Arc<Mutex<dyn Pipeline>>,
         method: SchedulerMethod,
         truncate_sequence: bool,
         no_kv_cache: bool,
         no_prefix_cache: bool,
         prefix_cache_n: usize,
         disable_eos_stop: bool,
-        interactive: bool,
     ) -> Self {
         let device = get_mut_arcmutex!(pipeline).device().clone();
         let is_xlora = get_mut_arcmutex!(pipeline).get_metadata().is_xlora;
-        if interactive {
-            ctrlc::set_handler(move || {
-                TERMINATE_ALL_NEXT_STEP.store(true, Ordering::SeqCst);
-            })
-            .expect("Failed to set CTRL-C handler for interactive mode");
-        }
         Self {
             rx,
             pipeline,
             scheduler: Scheduler::new(method),
             id: 0,
             truncate_sequence,
             no_kv_cache,
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/layers.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/models/phi3.rs`

 * *Files 25% similar despite different names*

```diff
@@ -1,367 +1,430 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
-use std::{collections::HashMap, ops::Mul, str::FromStr, sync::Mutex};
-
-use candle_core::{quantized::QTensor, DType, Device, IndexOp, Result, Tensor, WithDType};
-use candle_nn::{
-    layer_norm::{RmsNormNonQuantized, RmsNormQuantized},
-    Module, VarBuilder,
+// This implementation is based on:
+// https://huggingface.co/microsoft/Phi-3-mini-4k-instruct/blob/main/modeling_phi3.py
+use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor, D};
+use candle_nn::{linear_no_bias, VarBuilder};
+use either::Either;
+use std::{collections::HashMap, sync::Arc};
+
+use crate::{
+    device_map::DeviceMapper,
+    layers::{flash_attn, repeat_kv, CausalMasker, MatMul, PhiRotaryEmbedding, RmsNorm},
+    pipeline::{extract_logits, Cache, NormalModel},
+    DeviceMapMetadata,
 };
-use once_cell::sync::Lazy;
-
-static MASKS: Lazy<Mutex<HashMap<(usize, usize), Tensor>>> =
-    Lazy::new(|| Mutex::new(HashMap::new()));
 
-use crate::models::phi3;
-
-#[derive(Debug, Clone)]
-pub struct RmsNorm {
-    inner: candle_nn::RmsNorm<RmsNormNonQuantized>,
-    eps: f64,
-    weight: Tensor,
+// https://huggingface.co/microsoft/Phi-3-mini-4k-instruct/blob/main/config.json
+#[derive(Debug, Clone, serde::Deserialize)]
+pub struct Config {
+    pub vocab_size: usize,
+    pub hidden_act: candle_nn::Activation,
+    pub hidden_size: usize,
+    pub intermediate_size: usize,
+    pub num_hidden_layers: usize,
+    pub num_attention_heads: usize,
+    pub num_key_value_heads: usize,
+    pub rms_norm_eps: f64,
+    pub rope_theta: f64,
+    pub bos_token_id: Option<u32>,
+    pub eos_token_id: Option<u32>,
+    pub rope_scaling: Option<HashMap<String, Either<Vec<f32>, String>>>,
+    pub max_position_embeddings: usize,
+    pub use_flash_attn: bool,
+    pub sliding_window: Option<usize>,
+    pub original_max_position_embeddings: usize,
+}
+
+impl Config {
+    pub fn head_dim(&self) -> usize {
+        self.hidden_size / self.num_attention_heads
+    }
 }
 
-impl RmsNorm {
-    pub fn new(size: usize, eps: f64, vb: VarBuilder) -> Result<Self> {
-        let inner = candle_nn::rms_norm_non_quant(size, eps, vb)?;
-        let w = inner.inner().weight().clone();
+#[derive(Debug, Clone)]
+struct Attention {
+    qkv_proj: QMatMul,
+    o_proj: QMatMul,
+    num_heads: usize,
+    num_kv_heads: usize,
+    num_kv_groups: usize,
+    head_dim: usize,
+    rotary_emb: Arc<PhiRotaryEmbedding>,
+    use_flash_attn: bool,
+    sliding_window: Option<usize>,
+    neg_inf: Tensor,
+}
+
+impl Attention {
+    fn new(rotary_emb: Arc<PhiRotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
+        let num_heads = cfg.num_attention_heads;
+        let num_kv_heads = cfg.num_key_value_heads;
+        let head_dim = cfg.head_dim();
+        let op_size = num_heads * head_dim + 2 * num_kv_heads * head_dim;
+        let qkv_proj = linear_no_bias(cfg.hidden_size, op_size, vb.pp("qkv_proj"))?;
+        let o_proj = linear_no_bias(num_heads * head_dim, cfg.hidden_size, vb.pp("o_proj"))?;
         Ok(Self {
-            inner,
-            eps,
-            weight: w,
+            qkv_proj: QMatMul::Tensor(qkv_proj.weight().clone()),
+            o_proj: QMatMul::Tensor(o_proj.weight().clone()),
+            rotary_emb,
+            num_heads,
+            num_kv_heads,
+            num_kv_groups: num_heads / num_kv_heads,
+            head_dim,
+            use_flash_attn: cfg.use_flash_attn,
+            sliding_window: cfg.sliding_window,
+            neg_inf: Tensor::new(f32::NEG_INFINITY, vb.device())?.to_dtype(vb.dtype())?,
         })
     }
 
-    pub fn from_w(w: Tensor, eps: f64) -> Result<Self> {
-        let inner = candle_nn::RmsNorm::<RmsNormNonQuantized>::new(w.clone(), eps);
-        Ok(Self {
-            inner,
-            eps,
-            weight: w,
-        })
-    }
-}
+    fn forward(
+        &mut self,
+        xs: &Tensor,
+        attention_mask: Option<&Tensor>,
+        seqlen_offsets: &[usize],
+        position_ids: &[usize],
+        kv_cache: &mut Option<(Tensor, Tensor)>,
+    ) -> Result<Tensor> {
+        let (b_sz, q_len, _) = xs.dims3()?;
 
-impl Module for RmsNorm {
-    fn forward(&self, x: &Tensor) -> Result<Tensor> {
-        if x.device().is_cpu() {
-            // Handle device mapping case
-            return candle_nn::ops::rms_norm(&x.contiguous()?, &self.weight, self.eps as f32);
+        let original_dtype = xs.dtype();
+        let mut xs = xs.clone();
+        if matches!(self.qkv_proj, QMatMul::QTensor(_)) {
+            xs = xs.to_dtype(DType::F32)?;
+        }
+        let mut qkv = MatMul.qmatmul(&xs, &self.qkv_proj)?;
+        if matches!(self.qkv_proj, QMatMul::QTensor(_)) {
+            qkv = qkv.to_dtype(original_dtype)?;
+        }
+        let query_pos = self.num_heads * self.head_dim;
+        let q = qkv.narrow(D::Minus1, 0, query_pos)?;
+        let k = qkv.narrow(D::Minus1, query_pos, self.num_kv_heads * self.head_dim)?;
+        let v = qkv.narrow(
+            D::Minus1,
+            query_pos + self.num_kv_heads * self.head_dim,
+            self.num_kv_heads * self.head_dim,
+        )?;
+
+        let q = q
+            .reshape((b_sz, q_len, self.num_heads, self.head_dim))?
+            .transpose(1, 2)?;
+        let k = k
+            .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
+            .transpose(1, 2)?;
+        let v = v
+            .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
+            .transpose(1, 2)?;
+
+        let (q, k) = self
+            .rotary_emb
+            .forward(&q, &k, seqlen_offsets, position_ids)?;
+
+        let (k, v, attn_mask) = Cache::update_kv_cache_sliding_window(
+            kv_cache,
+            k,
+            v,
+            attention_mask,
+            self.sliding_window,
+            true,
+        )?;
+
+        let k = repeat_kv(k, self.num_kv_groups)?.contiguous()?;
+        let v = repeat_kv(v, self.num_kv_groups)?.contiguous()?;
+
+        let mut attn_output = if self.use_flash_attn {
+            // flash-attn expects (b_sz, seq_len, nheads, head_dim)
+            let q = q.transpose(1, 2)?;
+            let k = k.transpose(1, 2)?;
+            let v = v.transpose(1, 2)?;
+            let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
+            flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
+        } else {
+            let attn_weights = MatMul.matmul_affine_div(
+                &q,
+                &k.transpose(2, 3)?,
+                f64::sqrt(self.head_dim as f64),
+            )?;
+
+            let attn_weights = CausalMasker.apply_mask(&attn_mask, attn_weights, &self.neg_inf)?;
+            let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
+            MatMul.matmul(&attn_weights, &v)?
+        };
+        if matches!(self.qkv_proj, QMatMul::QTensor(_)) {
+            attn_output = attn_output.to_dtype(DType::F32)?;
+        }
+        let mut res = MatMul.qmatmul(
+            &attn_output.transpose(1, 2)?.reshape((b_sz, q_len, ()))?,
+            &self.o_proj,
+        )?;
+        if matches!(self.qkv_proj, QMatMul::QTensor(_)) {
+            res = res.to_dtype(original_dtype)?;
         }
-        self.inner.forward(x)
+        Ok(res)
     }
 }
 
 #[derive(Debug, Clone)]
-pub struct QRmsNorm {
-    inner: candle_nn::RmsNorm<RmsNormQuantized>,
+struct Mlp {
+    gate_up_proj: QMatMul,
+    down_proj: QMatMul,
+    act_fn: candle_nn::Activation,
+    i_size: usize,
 }
 
-impl QRmsNorm {
-    pub fn new(scale: QTensor, eps: f32) -> Result<Self> {
-        let scale = scale.dequantize(&scale.device())?;
-        let inner = candle_nn::RmsNorm::<RmsNormQuantized>::new(scale, eps as f64);
-        Ok(Self { inner })
-    }
-
-    pub fn forward(&self, x: &Tensor) -> Result<Tensor> {
-        self.inner.forward(x)
+impl Mlp {
+    fn new(cfg: &Config, vb: VarBuilder) -> Result<Self> {
+        let hidden_size = cfg.hidden_size;
+        let i_size = cfg.intermediate_size;
+        let gate_up_proj = linear_no_bias(hidden_size, 2 * i_size, vb.pp("gate_up_proj"))?;
+        let down_proj = linear_no_bias(i_size, hidden_size, vb.pp("down_proj"))?;
+        Ok(Self {
+            gate_up_proj: QMatMul::Tensor(gate_up_proj.weight().clone()),
+            down_proj: QMatMul::Tensor(down_proj.weight().clone()),
+            act_fn: cfg.hidden_act,
+            i_size,
+        })
     }
 }
 
-/// RoPE supporting LongRope
-#[derive(Debug, Clone)]
-pub struct PhiRotaryEmbedding {
-    short_sin: Tensor,
-    short_cos: Tensor,
-    long_cos: Option<Tensor>,
-    long_sin: Option<Tensor>,
-    original_max_position_embeddings: usize,
-}
-
-#[derive(Debug, Clone)]
-enum ScaledRopeType {
-    Su,
-    Yarn,
-}
-
-impl FromStr for ScaledRopeType {
-    type Err = candle_core::Error;
-    fn from_str(s: &str) -> std::result::Result<Self, Self::Err> {
-        match s {
-            "su" => Ok(Self::Su),
-            "yarn" => Ok(Self::Yarn),
-            _ => Err(candle_core::Error::Msg(
-                "Expected either `su` or `yarn` scaled RoPE type.".to_string(),
-            )),
+impl Module for Mlp {
+    fn forward(&self, xs: &Tensor) -> Result<Tensor> {
+        let original_dtype = xs.dtype();
+        let mut xs = xs.clone();
+        if matches!(self.gate_up_proj, QMatMul::QTensor(_)) {
+            xs = xs.to_dtype(DType::F32)?;
+        }
+        let up_states = MatMul.qmatmul(&xs, &self.gate_up_proj)?;
+        let gate = up_states.narrow(D::Minus1, 0, self.i_size)?;
+        let up_states = up_states.narrow(D::Minus1, self.i_size, self.i_size)?;
+        let up_states = (up_states * gate.apply(&self.act_fn))?;
+        let mut res = MatMul.qmatmul(&up_states, &self.down_proj)?;
+        if matches!(self.gate_up_proj, QMatMul::QTensor(_)) {
+            res = res.to_dtype(original_dtype)?;
         }
+        Ok(res)
     }
 }
 
 #[derive(Debug, Clone)]
-struct ScaledRopeParams {
-    short_factor: Vec<f32>,
-    long_factor: Vec<f32>,
-    scaling_type: ScaledRopeType,
-}
-
-impl PhiRotaryEmbedding {
-    pub fn new(dtype: DType, cfg: &phi3::Config, dev: &Device) -> Result<Self> {
-        let scaled_params = cfg.rope_scaling.as_ref().map(|r| ScaledRopeParams {
-            short_factor: r["short_factor"].clone().left().unwrap(),
-            long_factor: r["long_factor"].clone().left().unwrap(),
-            scaling_type: r["type"].clone().right().unwrap().parse().unwrap(),
-        });
-        let max_seq_len = cfg.max_position_embeddings;
-        let dim = cfg.head_dim();
-
-        if let Some(scaled_params) = scaled_params {
-            // Calculate scale
-            let scale =
-                cfg.max_position_embeddings as f64 / cfg.original_max_position_embeddings as f64;
-            let scaling_factor = if scale <= 1.0 {
-                1.0
-            } else {
-                match scaled_params.scaling_type {
-                    ScaledRopeType::Su => (1.0
-                        + scale.ln() / (cfg.original_max_position_embeddings as f64).ln())
-                    .sqrt(),
-                    ScaledRopeType::Yarn => 0.1 * scale.ln() + 1.0,
-                }
-            };
-
-            // Calculate inv freqs for short, long
-            let inv_freq_long: Vec<_> = (0..dim)
-                .step_by(2)
-                .enumerate()
-                .map(|(k, i)| {
-                    1f32 / (scaled_params.long_factor[k]
-                        * cfg.rope_theta.powf(i as f64 / dim as f64) as f32)
-                })
-                .collect();
-            let inv_freq_short: Vec<_> = (0..dim)
-                .step_by(2)
-                .enumerate()
-                .map(|(k, i)| {
-                    1f32 / (scaled_params.short_factor[k]
-                        * cfg.rope_theta.powf(i as f64 / dim as f64) as f32)
-                })
-                .collect();
-            let inv_freq_len = inv_freq_long.len();
-
-            let t = Tensor::arange(0u32, max_seq_len as u32, dev)?
-                .to_dtype(DType::F32)?
-                .reshape((max_seq_len, 1))?;
-
-            // Calculate sin,cos for long
-            let inv_freq_long = Tensor::from_vec(inv_freq_long, (1, inv_freq_len), dev)?;
-            let freqs_long = t.matmul(&inv_freq_long)?;
-            let long_sin = freqs_long.sin()?.mul(scaling_factor)?.to_dtype(dtype)?;
-            let long_cos = freqs_long.cos()?.mul(scaling_factor)?.to_dtype(dtype)?;
-
-            // Calculate sin,cos for short
-            let inv_freq_short = Tensor::from_vec(inv_freq_short, (1, inv_freq_len), dev)?;
-            let freqs_short = t.matmul(&inv_freq_short)?;
-            let short_sin = freqs_short.sin()?.mul(scaling_factor)?.to_dtype(dtype)?;
-            let short_cos = freqs_short.cos()?.mul(scaling_factor)?.to_dtype(dtype)?;
-
-            Ok(Self {
-                short_cos,
-                short_sin,
-                long_cos: Some(long_cos),
-                long_sin: Some(long_sin),
-                original_max_position_embeddings: cfg.original_max_position_embeddings,
-            })
-        } else {
-            let inv_freq: Vec<_> = (0..dim)
-                .step_by(2)
-                .map(|i| 1f32 / cfg.rope_theta.powf(i as f64 / dim as f64) as f32)
-                .collect();
-            let inv_freq_len = inv_freq.len();
-            let inv_freq = Tensor::from_vec(inv_freq, (1, inv_freq_len), dev)?;
-            let t = Tensor::arange(0u32, max_seq_len as u32, dev)?
-                .to_dtype(DType::F32)?
-                .reshape((max_seq_len, 1))?;
-            let freqs = t.matmul(&inv_freq)?;
-            let sin = freqs.sin()?.to_dtype(dtype)?;
-            let cos = freqs.cos()?.to_dtype(dtype)?;
-            Ok(Self {
-                short_cos: cos,
-                short_sin: sin,
-                long_cos: None,
-                long_sin: None,
-                original_max_position_embeddings: cfg.original_max_position_embeddings,
-            })
-        }
+struct DecoderLayer {
+    self_attn: Attention,
+    mlp: Mlp,
+    input_layernorm: RmsNorm,
+    post_attention_layernorm: RmsNorm,
+}
+
+impl DecoderLayer {
+    fn new(
+        rotary_emb: Arc<PhiRotaryEmbedding>,
+        cfg: &Config,
+        vb: VarBuilder,
+        mapper: &dyn DeviceMapper,
+        layer_idx: usize,
+        loading_isq: bool,
+    ) -> Result<Self> {
+        let self_attn = Attention::new(
+            rotary_emb,
+            cfg,
+            mapper.set_device(layer_idx, vb.pp("self_attn"), loading_isq),
+        )?;
+        let mlp = Mlp::new(cfg, mapper.set_device(layer_idx, vb.pp("mlp"), loading_isq))?;
+        let input_layernorm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_device(layer_idx, vb.pp("input_layernorm"), false),
+        )?;
+        let post_attention_layernorm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_device(layer_idx, vb.pp("post_attention_layernorm"), false),
+        )?;
+        Ok(Self {
+            self_attn,
+            mlp,
+            input_layernorm,
+            post_attention_layernorm,
+        })
     }
 
-    /// Returns (sin, cos) taking into account LongRope
-    fn get_long_or_short_sin_cos(&self, position_ids: &[usize]) -> (&Tensor, &Tensor) {
-        if self.long_cos.is_none() {
-            return (&self.short_sin, &self.short_cos);
-        }
-        let seq_len = position_ids.iter().max().unwrap() + 1;
-        if seq_len > self.original_max_position_embeddings {
-            (
-                self.long_sin.as_ref().unwrap(),
-                self.long_cos.as_ref().unwrap(),
-            )
-        } else {
-            (&self.short_sin, &self.short_cos)
-        }
+    fn forward(
+        &mut self,
+        xs: &Tensor,
+        attention_mask: Option<&Tensor>,
+        seqlen_offsets: &[usize],
+        position_ids: &[usize],
+        kv_cache: &mut Option<(Tensor, Tensor)>,
+    ) -> Result<Tensor> {
+        let residual = xs;
+        let xs = self.input_layernorm.forward(xs)?;
+        let xs =
+            self.self_attn
+                .forward(&xs, attention_mask, seqlen_offsets, position_ids, kv_cache)?;
+        let xs = (xs + residual)?;
+        let residual = &xs;
+        let xs = xs.apply(&self.post_attention_layernorm)?.apply(&self.mlp)?;
+        residual + xs
+    }
+}
+
+#[derive(Debug)]
+pub struct Model {
+    embed_tokens: candle_nn::Embedding,
+    layers: Vec<DecoderLayer>,
+    norm: RmsNorm,
+    lm_head: QMatMul,
+    pub device: Device,
+    pub cache: Cache,
+    pub max_seq_len: usize,
+    mapper: Box<dyn DeviceMapper + Send + Sync>,
+    sliding_window: Option<usize>,
+}
+
+impl Model {
+    pub fn new(
+        cfg: &Config,
+        vb: VarBuilder,
+        _is_gptx: bool,
+        mapper: DeviceMapMetadata,
+        loading_isq: bool,
+        real_device: Device,
+    ) -> Result<Self> {
+        let vb_m = vb.pp("model");
+        let mapper = mapper.into_mapper(cfg.num_hidden_layers, &real_device)?;
+        let embed_tokens = candle_nn::embedding(
+            cfg.vocab_size,
+            cfg.hidden_size,
+            mapper.set_nm_device(vb_m.pp("embed_tokens"), false),
+        )?;
+        let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
+        let vb_l = vb_m.pp("layers");
+        for layer_idx in 0..cfg.num_hidden_layers {
+            let rotary_emb = Arc::new(PhiRotaryEmbedding::new(
+                vb.dtype(),
+                cfg,
+                mapper.device_for(layer_idx, false).unwrap_or(&real_device),
+            )?);
+            let layer = DecoderLayer::new(
+                rotary_emb.clone(),
+                cfg,
+                vb_l.pp(layer_idx),
+                &*mapper,
+                layer_idx,
+                loading_isq,
+            )?;
+            layers.push(layer)
+        }
+        let norm = RmsNorm::new(
+            cfg.hidden_size,
+            cfg.rms_norm_eps,
+            mapper.set_nm_device(vb_m.pp("norm"), false),
+        )?;
+        let lm_head = linear_no_bias(
+            cfg.hidden_size,
+            cfg.vocab_size,
+            mapper.set_nm_device(vb.pp("lm_head"), loading_isq),
+        )?;
+        Ok(Self {
+            embed_tokens,
+            layers,
+            norm,
+            lm_head: QMatMul::Tensor(lm_head.weight().clone()),
+            device: real_device,
+            cache: Cache::new(cfg.num_hidden_layers, false),
+            max_seq_len: cfg.max_position_embeddings,
+            mapper,
+            sliding_window: cfg.sliding_window,
+        })
     }
 
     pub fn forward(
-        &self,
-        q: &Tensor,
-        k: &Tensor,
+        &mut self,
+        input_ids: &Tensor,
         seqlen_offsets: &[usize],
         position_ids: &[usize],
-    ) -> Result<(Tensor, Tensor)> {
-        let (_b_sz, _h, seq_len, _n_embd) = q.dims4()?;
-        let mut q_embeds = Vec::new();
-        let mut k_embeds = Vec::new();
-        let (sin, cos) = self.get_long_or_short_sin_cos(position_ids);
-        for (i, offset) in seqlen_offsets.iter().enumerate() {
-            let cos = cos.narrow(0, *offset, seq_len)?;
-            let sin = sin.narrow(0, *offset, seq_len)?;
-            let q_embed =
-                candle_nn::rotary_emb::rope(&q.i(i)?.unsqueeze(0)?.contiguous()?, &cos, &sin)?;
-            let k_embed =
-                candle_nn::rotary_emb::rope(&k.i(i)?.unsqueeze(0)?.contiguous()?, &cos, &sin)?;
-            q_embeds.push(q_embed);
-            k_embeds.push(k_embed);
-        }
-        Ok((Tensor::cat(&q_embeds, 0)?, Tensor::cat(&k_embeds, 0)?))
+        context_lens: Vec<(usize, usize)>,
+    ) -> Result<Tensor> {
+        let mut xs = self.embed_tokens.forward(input_ids)?;
+        let mut cache = self.cache.lock();
+        let attention_mask = CausalMasker.make_causal_mask_with_sliding_window(
+            input_ids,
+            &cache,
+            self.sliding_window,
+        )?;
+        let past_key_values_length = CausalMasker.calculate_past_kv_len(&cache)?;
+        let position_ids = position_ids
+            .iter()
+            .map(|p| *p + past_key_values_length)
+            .collect::<Vec<_>>();
+
+        for (i, layer) in self.layers.iter_mut().enumerate() {
+            xs = self.mapper.map(xs, i)?;
+            xs = layer.forward(
+                &xs,
+                attention_mask
+                    .as_ref()
+                    .map(|m| m.to_device(xs.device()).unwrap())
+                    .as_ref(),
+                seqlen_offsets,
+                &position_ids,
+                &mut cache[i],
+            )?
+        }
+        let xs = xs.to_device(&self.device)?;
+        let mut xs = xs.apply(&self.norm)?;
+        if matches!(self.lm_head, QMatMul::QTensor(_)) {
+            xs = xs.to_dtype(DType::F32)?;
+        }
+        extract_logits(&MatMul.qmatmul(&xs, &self.lm_head)?, context_lens)
     }
 }
 
-// https://github.com/huggingface/transformers/blob/main/src/transformers/modeling_attn_mask_utils.py
-pub struct CausalMasker;
-
-// https://github.com/mokeyish/candle-ext/blob/main/src/triangular.rs
-fn apply_tril(xs: &Tensor, diagonal: isize) -> Result<Tensor> {
-    let device = xs.device();
-    let (l, s) = xs.dims2()?;
-    let mut xs_tri = vec![];
-    for i in 0..l as isize {
-        for j in 0..s as isize {
-            let cond = i + diagonal < j;
-            xs_tri.push(if cond { 0u8 } else { 1u8 });
-        }
+impl NormalModel for Model {
+    fn forward(
+        &mut self,
+        input_ids: &Tensor,
+        seqlen_offsets: &[usize],
+        _start_offsets_kernel: Tensor,
+        context_lens: Vec<(usize, usize)>,
+        position_ids: Vec<usize>,
+    ) -> Result<Tensor> {
+        self.forward(input_ids, seqlen_offsets, &position_ids, context_lens)
     }
-    xs * Tensor::from_vec(xs_tri, (l, s), device)?.to_dtype(xs.dtype())?
-}
-
-// https://github.com/mokeyish/candle-ext/blob/main/src/masked_fill.rs
-fn masked_fill<D: WithDType>(xs: &Tensor, mask: &Tensor, value: D) -> Result<Tensor> {
-    let on_true = Tensor::full(value, xs.shape(), xs.device())?;
-    let on_false = xs;
-    mask.broadcast_as(xs.shape())?
-        .where_cond(&on_true, on_false)
-}
-
-impl CausalMasker {
-    fn make_mask(&self, tgt_len: usize, past_kv_len: usize, device: &Device) -> Result<Tensor> {
-        let offset = tgt_len + past_kv_len;
-        let mask: Vec<_> = (0..tgt_len)
-            .flat_map(|i| (0..offset).map(move |j| u8::from(j + tgt_len > i + offset)))
-            .collect();
-        Tensor::from_slice(&mask, (tgt_len, offset), device)
-    }
-
-    pub fn calculate_past_kv_len(
-        &self,
-        cache: &[Option<(Tensor, Tensor)>],
-    ) -> candle_core::Result<usize> {
-        let kv_cache_1 = &cache[0];
-        if kv_cache_1.is_none() {
-            return Ok(0);
-        }
-        let k_cache_1 = &kv_cache_1.as_ref().unwrap().0;
-        return Ok(k_cache_1.dims()[2]);
+    fn xlora_forward(
+        &mut self,
+        _input_ids: &Tensor,
+        _input_ids_full: &Tensor,
+        _seqlen_offsets: &[usize],
+        _seqlen_offsets_full: &[usize],
+        _start_offsets_kernel: Tensor,
+        _start_offsets_kernel_full: Tensor,
+        _no_kv_cache: bool,
+        _non_granular_state: &Option<crate::xlora_models::NonGranularState>,
+        _context_lens: Vec<(usize, usize)>,
+        _position_ids: Vec<usize>,
+    ) -> Result<Tensor> {
+        unimplemented!()
     }
-
-    pub fn make_causal_mask(
-        &self,
-        input_ids: &Tensor,
-        cache: &[Option<(Tensor, Tensor)>],
-    ) -> Result<Option<Tensor>> {
-        let past_kv_len = self.calculate_past_kv_len(cache)?;
-        let (b_sz, tgt_len) = input_ids.dims2()?;
-        if tgt_len == 1 {
-            return Ok(None);
-        }
-        let res = MASKS.lock().unwrap().get(&(tgt_len, past_kv_len)).cloned();
-        if let Some(mask) = res {
-            Ok(Some(mask))
-        } else {
-            let mask = self.make_mask(tgt_len, past_kv_len, input_ids.device())?;
-            let mask = mask
-                .expand((b_sz, 1, tgt_len, tgt_len + past_kv_len))?
-                .to_dtype(DType::U8)?;
-
-            MASKS
-                .lock()
-                .unwrap()
-                .insert((tgt_len, past_kv_len), mask.clone());
-            Ok(Some(mask))
-        }
+    fn cache(&self) -> &Cache {
+        &self.cache
     }
-
-    pub fn make_causal_mask_with_sliding_window(
-        &self,
-        input_ids: &Tensor,
-        cache: &[Option<(Tensor, Tensor)>],
-        sliding_window: Option<usize>,
-    ) -> Result<Option<Tensor>> {
-        if sliding_window.is_none() {
-            return self.make_causal_mask(input_ids, cache);
-        }
-        let sliding_window = sliding_window.unwrap();
-        let past_kv_len = self.calculate_past_kv_len(cache)?;
-        let (b_sz, tgt_len) = input_ids.dims2()?;
-        if tgt_len == 1 {
-            return Ok(None);
-        }
-        let res = MASKS.lock().unwrap().get(&(tgt_len, past_kv_len)).cloned();
-        if let Some(mask) = res {
-            Ok(Some(mask))
-        } else {
-            let mask = self.make_mask(tgt_len, past_kv_len, input_ids.device())?;
-            let diagonal = past_kv_len as isize - sliding_window as isize - 1;
-            let context_mask = apply_tril(&mask.ones_like()?, diagonal)?;
-            let mask = masked_fill(&mask.to_dtype(DType::F32)?, &context_mask, f32::MIN)?;
-            let mask = mask
-                .expand((b_sz, 1, tgt_len, tgt_len + past_kv_len))?
-                .to_dtype(DType::U8)?;
-
-            MASKS
-                .lock()
-                .unwrap()
-                .insert((tgt_len, past_kv_len), mask.clone());
-            Ok(Some(mask))
-        }
+    fn device(&self) -> &Device {
+        &self.device
     }
-
-    pub fn apply_mask(
-        &self,
-        mask: &Option<Tensor>,
-        att: Tensor,
-        neg_inf: &Tensor,
-    ) -> Result<Tensor> {
-        match mask {
-            None => Ok(att),
-            Some(mask) => {
-                let mask = mask.broadcast_as(att.shape())?;
-                mask.where_cond(
-                    &neg_inf
-                        .to_device(att.device())?
-                        .to_dtype(att.dtype())?
-                        .broadcast_as(att.dims())?,
-                    &att,
-                )
-            }
+    fn is_xlora(&self) -> bool {
+        false
+    }
+    fn max_seq_len(&self) -> usize {
+        self.max_seq_len
+    }
+    fn get_tensors(&mut self) -> (Vec<(&mut QMatMul, Option<usize>)>, &dyn DeviceMapper) {
+        let mut tensors = Vec::new();
+        tensors.push((&mut self.lm_head, None));
+        for (i, layer) in self.layers.iter_mut().enumerate() {
+            tensors.push((&mut layer.self_attn.qkv_proj, Some(i)));
+            tensors.push((&mut layer.self_attn.o_proj, Some(i)));
+            tensors.push((&mut layer.mlp.gate_up_proj, Some(i)));
+            tensors.push((&mut layer.mlp.down_proj, Some(i)));
         }
+        (tensors, &*self.mapper)
     }
 }
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/lib.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/lib.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 #![deny(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
 use std::{
     cell::RefCell,
     error::Error,
     fs::OpenOptions,
     io::Write,
-    sync::{Arc, Mutex},
+    sync::{atomic::AtomicBool, Arc, Mutex},
     thread,
     time::{SystemTime, UNIX_EPOCH},
 };
 use tokio::sync::mpsc::{channel, Sender};
 
 use engine::Engine;
-pub use mistralrs_lora::Ordering;
+pub use engine::TERMINATE_ALL_NEXT_STEP;
+pub use lora::Ordering;
 pub use pipeline::Pipeline;
 
 mod aici;
 mod device_map;
 mod engine;
+mod lora;
 mod model_loader;
 pub use model_loader::{get_tgt_non_granular_index, LoaderBuilder};
 mod model_selected;
 pub use model_selected::ModelSelected;
 
 pub mod layers;
 mod models;
@@ -35,18 +37,18 @@
 mod toml_selector;
 mod utils;
 mod xlora_models;
 
 pub use device_map::{DeviceMapMetadata, LayerDeviceMapper};
 pub use pipeline::{
     GGMLLoader, GGMLLoaderBuilder, GGMLSpecificConfig, GGUFLoader, GGUFLoaderBuilder,
-    GGUFSpecificConfig, GemmaLoader, LlamaLoader, Loader, MistralLoader, MixtralLoader, ModelKind,
-    NormalLoader, NormalLoaderBuilder, NormalLoaderType, NormalSpecificConfig, Phi2Loader,
-    Phi3Loader, Qwen2Loader, SpeculativeConfig, SpeculativeLoader, SpeculativePipeline,
-    TokenSource,
+    GGUFSpecificConfig, GemmaLoader, LlamaLoader, Loader, LocalModelPaths, MistralLoader,
+    MixtralLoader, ModelKind, ModelPaths, NormalLoader, NormalLoaderBuilder, NormalLoaderType,
+    NormalSpecificConfig, Phi2Loader, Phi3Loader, Qwen2Loader, SpeculativeConfig,
+    SpeculativeLoader, SpeculativePipeline, TokenSource,
 };
 pub use request::{Constraint, NormalRequest, Request, RequestMessage};
 pub use response::Response;
 pub use response::*;
 pub use sampler::{SamplingParams, StopTokens, TopLogprob};
 pub use scheduler::SchedulerMethod;
 use serde::Serialize;
@@ -73,32 +75,31 @@
     method: SchedulerMethod,
     log: Option<String>,
     truncate_sequence: Option<bool>,
     no_kv_cache: Option<bool>,
     no_prefix_cache: Option<bool>,
     prefix_cache_n: Option<usize>,
     disable_eos_stop: Option<bool>,
-    interactive: Option<bool>,
+    gemm_full_precision_f16: Option<bool>,
 }
 
 impl MistralRsBuilder {
     pub fn new(pipeline: Arc<tokio::sync::Mutex<dyn Pipeline>>, method: SchedulerMethod) -> Self {
         Self {
             pipeline,
             method,
             log: None,
             truncate_sequence: None,
             no_kv_cache: None,
             no_prefix_cache: None,
             prefix_cache_n: None,
             disable_eos_stop: None,
-            interactive: None,
+            gemm_full_precision_f16: None,
         }
     }
-
     pub fn with_log(mut self, log: String) -> Self {
         self.log = Some(log);
         self
     }
     pub fn with_opt_log(mut self, log: Option<String>) -> Self {
         self.log = log;
         self
@@ -119,44 +120,92 @@
         self.prefix_cache_n = Some(prefix_cache_n);
         self
     }
     pub fn with_disable_eos_stop(mut self, disable_eos_stop: bool) -> Self {
         self.disable_eos_stop = Some(disable_eos_stop);
         self
     }
-    pub fn with_interactive(mut self) -> Self {
-        self.interactive = Some(true);
+    pub fn with_gemm_full_precision_f16(mut self, gemm_full_precision: bool) -> Self {
+        self.gemm_full_precision_f16 = Some(gemm_full_precision);
         self
     }
 
     pub fn build(self) -> Arc<MistralRs> {
         MistralRs::new(self)
     }
 }
 
+pub(crate) static INHIBIT_GEMM_F16: AtomicBool = AtomicBool::new(false);
+
+#[cfg(feature = "cuda")]
+fn set_gemm_reduced_precision_f16() {
+    use candle_core::{DType, Device, Tensor};
+
+    // NOTE(EricLBuehler): When we support multi-GPU inference, we should check for each gpu here
+    let a = Tensor::zeros((2, 2), DType::BF16, &Device::new_cuda(0).unwrap()).unwrap();
+    candle_core::cuda::set_gemm_reduced_precision_bf16(true);
+    match a.matmul(&a) {
+        Ok(_) => (),
+        Err(e) => match e {
+            candle_core::Error::Cuda(e) => {
+                let x = e.downcast::<candle_core::cuda::cudarc::cublas::result::CublasError>();
+                if format!("{x:?}").contains("CUBLAS_STATUS_NOT_SUPPORTED") {
+                    tracing::info!("GEMM reduced precision in BF16 not supported.");
+                    candle_core::cuda::set_gemm_reduced_precision_bf16(false);
+                    INHIBIT_GEMM_F16.store(true, std::sync::atomic::Ordering::Relaxed);
+                }
+            }
+            _ => (),
+        },
+    }
+
+    let a = Tensor::zeros((2, 2), DType::F16, &Device::new_cuda(0).unwrap()).unwrap();
+    candle_core::cuda::set_gemm_reduced_precision_f16(true);
+    match a.matmul(&a) {
+        Ok(_) => (),
+        Err(e) => match e {
+            candle_core::Error::Cuda(e) => {
+                let x = e.downcast::<candle_core::cuda::cudarc::cublas::result::CublasError>();
+                if format!("{x:?}").contains("CUBLAS_STATUS_NOT_SUPPORTED") {
+                    tracing::info!("GEMM reduced precision in F16 not supported.");
+                    candle_core::cuda::set_gemm_reduced_precision_f16(false);
+                    INHIBIT_GEMM_F16.store(true, std::sync::atomic::Ordering::Relaxed);
+                }
+            }
+            _ => (),
+        },
+    }
+}
+
+#[cfg(not(feature = "cuda"))]
+fn set_gemm_reduced_precision_f16() {}
+
 impl MistralRs {
     fn new(config: MistralRsBuilder) -> Arc<Self> {
         let MistralRsBuilder {
             pipeline,
             method,
             log,
             truncate_sequence,
             no_kv_cache,
             no_prefix_cache,
             prefix_cache_n,
             disable_eos_stop,
-            interactive,
+            gemm_full_precision_f16,
         } = config;
 
+        if !gemm_full_precision_f16.unwrap_or(false) {
+            set_gemm_reduced_precision_f16();
+        }
+
         let truncate_sequence = truncate_sequence.unwrap_or(false);
         let no_kv_cache = no_kv_cache.unwrap_or(false);
         let no_prefix_cache = no_prefix_cache.unwrap_or(false);
         let prefix_cache_n = prefix_cache_n.unwrap_or(16);
         let disable_eos_stop = disable_eos_stop.unwrap_or(false);
-        let interactive = interactive.unwrap_or(false);
 
         let (tx, rx) = channel(10_000);
 
         let this = Arc::new(Self {
             sender: tx,
             log,
             id: pipeline.try_lock().unwrap().name(),
@@ -174,15 +223,14 @@
                     pipeline,
                     method,
                     truncate_sequence,
                     no_kv_cache,
                     no_prefix_cache,
                     prefix_cache_n,
                     disable_eos_stop,
-                    interactive,
                 );
                 engine.run().await;
             });
         });
 
         this
     }
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/model_loader.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/model_loader.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/model_selected.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/model_selected.rs`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         #[arg(short, long)]
         model_id: Option<String>,
 
         /// Path to local tokenizer.json file. If this is specified it is used over any remote file.
         #[arg(short, long)]
         tokenizer_json: Option<String>,
 
-        /// Model ID to load X-LoRA from. This may be a HF hub repo or a local path.
+        /// Model ID to load LoRA from. This may be a HF hub repo or a local path.
         #[arg(short, long)]
         adapters_model_id: String,
 
         /// Control the application of repeat penalty for the last n tokens
         #[arg(long, default_value_t = 64)]
         repeat_last_n: usize,
 
@@ -173,15 +173,15 @@
         #[arg(short = 'f', long)]
         quantized_filename: String,
 
         /// Control the application of repeat penalty for the last n tokens
         #[arg(long, default_value_t = 64)]
         repeat_last_n: usize,
 
-        /// Model ID to load X-LoRA from. This may be a HF hub repo or a local path.
+        /// Model ID to load LoRA from. This may be a HF hub repo or a local path.
         #[arg(short, long)]
         adapters_model_id: String,
 
         /// Ordering JSON file
         #[arg(short, long)]
         order: String,
     },
@@ -274,15 +274,15 @@
         #[arg(short = 'f', long)]
         quantized_filename: String,
 
         /// Control the application of repeat penalty for the last n tokens
         #[arg(long, default_value_t = 64)]
         repeat_last_n: usize,
 
-        /// Model ID to load X-LoRA from. This may be a HF hub repo or a local path.
+        /// Model ID to load LoRA from. This may be a HF hub repo or a local path.
         #[arg(short, long)]
         adapters_model_id: String,
 
         /// Ordering JSON file
         #[arg(short, long)]
         order: String,
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/models/gemma.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/models/gemma.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
 use std::sync::Arc;
 
 use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor, D};
 use candle_nn::{linear_b as linear, Activation, RotaryEmbedding, VarBuilder};
-use mistralrs_lora::layer::QLinear;
 
 use crate::{
     device_map::DeviceMapper,
-    layers::CausalMasker,
-    pipeline::{extract_logits, NormalModel},
+    layers::{flash_attn, repeat_kv, CausalMasker, MatMul, QLinear},
+    pipeline::{extract_logits, Cache, NormalModel},
     DeviceMapMetadata,
 };
 
-use super::{flash_attn, repeat_kv, Cache};
-
 fn default_max_position_embeddings() -> usize {
     4096
 }
 
 #[derive(serde::Deserialize, Debug, Clone)]
 pub struct Config {
     pub attention_bias: bool,
@@ -206,42 +203,37 @@
                 .contiguous()?;
             k = k
                 .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
                 .transpose(1, 2)?
                 .contiguous()?;
         }
 
-        let (k, v) = match &*kv_cache {
-            None => (k, v),
-            Some((prev_k, prev_v)) => {
-                let k = candle_nn::ops::kvconcat(prev_k, &k, 2)?;
-                let v = candle_nn::ops::kvconcat(prev_v, &v, 2)?;
-                (k, v)
-            }
-        };
-        *kv_cache = Some((k.clone(), v.clone()));
+        let (k, v) = Cache::update_kv_cache(kv_cache, k, v, false)?;
 
         let k = repeat_kv(k, self.num_kv_groups)?.contiguous()?;
         let v = repeat_kv(v, self.num_kv_groups)?.contiguous()?;
 
         let mut attn_output = if self.use_flash_attn {
             // flash-attn expects (b_sz, seq_len, nheads, head_dim)
             let q = q.transpose(1, 2)?;
             let k = k.transpose(1, 2)?;
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
-            let scale = 1f64 / f64::sqrt(self.head_dim as f64);
-            let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
+            let attn_weights = MatMul.matmul_affine_div(
+                &q,
+                &k.transpose(2, 3)?,
+                f64::sqrt(self.head_dim as f64),
+            )?;
 
             let attn_weights =
                 CausalMasker.apply_mask(&attention_mask.cloned(), attn_weights, &self.neg_inf)?;
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
-            attn_weights.matmul(&v)?
+            MatMul.matmul(&attn_weights, &v)?
         };
         if self.q_proj.is_quant() {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
         let mut res = attn_output
             .transpose(1, 2)?
             .reshape((b_sz, q_len, ()))?
@@ -412,15 +404,15 @@
             )?;
         }
         let xs = xs.to_device(&self.device)?;
         let mut xs = xs.apply(&self.norm)?;
         if matches!(self.lm_head, QMatMul::QTensor(_)) {
             xs = xs.to_dtype(DType::F32)?;
         }
-        extract_logits(&xs.apply(&self.lm_head)?, context_lens)
+        extract_logits(&MatMul.qmatmul(&xs, &self.lm_head)?, context_lens)
     }
 }
 
 impl NormalModel for Model {
     fn forward(
         &mut self,
         input_ids: &Tensor,
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/models/llama.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/models/llama.rs`

 * *Files 6% similar despite different names*

```diff
@@ -5,21 +5,19 @@
     embedding, linear_no_bias as linear, Embedding, Module, RotaryEmbedding, VarBuilder,
 };
 use serde::Deserialize;
 use std::sync::Arc;
 
 use crate::{
     device_map::DeviceMapper,
-    layers::{CausalMasker, RmsNorm},
+    layers::{flash_attn, repeat_kv, CausalMasker, MatMul, RmsNorm},
     pipeline::{extract_logits, NormalModel},
     DeviceMapMetadata,
 };
 
-use super::{flash_attn, repeat_kv};
-
 #[derive(Debug, Clone, Deserialize)]
 pub struct Config {
     pub hidden_size: usize,
     pub intermediate_size: usize,
     pub vocab_size: usize,
     pub num_hidden_layers: usize,
     pub num_attention_heads: usize,
@@ -49,35 +47,35 @@
     fn forward(
         &self,
         x: &Tensor,
         attention_mask: &Option<Tensor>,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         block_idx: usize,
-        kv_cache: &mut super::LayerCaches,
+        kv_cache: &mut crate::pipeline::LayerCaches,
     ) -> Result<Tensor> {
         let (b_sz, seq_len, hidden_size) = x.dims3()?;
 
         let original_dtype = x.dtype();
         let mut x = x.clone();
         if matches!(self.q_proj, QMatMul::QTensor(_)) {
             x = x.to_dtype(DType::F32)?;
         }
-        let mut q = self.q_proj.forward(&x)?;
-        let mut k = self.k_proj.forward(&x)?;
-        let mut v = self.v_proj.forward(&x)?;
+        let mut q = MatMul.qmatmul(&x, &self.q_proj)?;
+        let mut k = MatMul.qmatmul(&x, &self.k_proj)?;
+        let mut v = MatMul.qmatmul(&x, &self.v_proj)?;
         if matches!(self.q_proj, QMatMul::QTensor(_)) {
             q = q.to_dtype(original_dtype)?;
             k = k.to_dtype(original_dtype)?;
             v = v.to_dtype(original_dtype)?;
         }
 
         let mut q = q.reshape((b_sz * seq_len, self.num_attention_heads, self.head_dim))?;
         let mut k = k.reshape((b_sz * seq_len, self.num_key_value_heads, self.head_dim))?;
-        let mut v = v
+        let v = v
             .reshape((b_sz, seq_len, self.num_key_value_heads, self.head_dim))?
             .transpose(1, 2)?;
 
         self.rotary_emb
             .forward(seqlen_offsets, &start_offsets_kernel, &mut q, &mut k, b_sz)?;
 
         if q.rank() == 3 {
@@ -87,58 +85,39 @@
                 .contiguous()?;
             k = k
                 .reshape((b_sz, seq_len, self.num_key_value_heads, self.head_dim))?
                 .transpose(1, 2)?
                 .contiguous()?;
         }
 
-        if let Some((cache_k, cache_v)) = &kv_cache[block_idx] {
-            k = candle_nn::ops::kvconcat(cache_k, &k, 2)?.contiguous()?;
-            v = candle_nn::ops::kvconcat(cache_v, &v, 2)?.contiguous()?;
-            let k_seq_len = k.dims()[1];
-            if k_seq_len > self.max_seq_len {
-                k = k
-                    .narrow(D::Minus1, k_seq_len - self.max_seq_len, self.max_seq_len)?
-                    .contiguous()?
-            }
-            let v_seq_len = v.dims()[1];
-            if v_seq_len > 2 * self.max_seq_len {
-                v = v
-                    .narrow(D::Minus1, v_seq_len - self.max_seq_len, self.max_seq_len)?
-                    .contiguous()?
-            }
-        }
-        kv_cache[block_idx] = Some((k.clone(), v.clone()));
+        let (k, v) =
+            crate::pipeline::Cache::update_kv_cache(&mut kv_cache[block_idx], k, v, false)?;
 
         let k = repeat_kv(k, self.num_attention_heads / self.num_key_value_heads)?.contiguous()?;
         let v = repeat_kv(v, self.num_attention_heads / self.num_key_value_heads)?.contiguous()?;
 
         let mut y = if self.use_flash_attn {
             // flash-attn expects (b_sz, seq_len, nheads, head_dim)
             let q = q.transpose(1, 2)?;
             let k = k.transpose(1, 2)?;
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, seq_len > 1)?.transpose(1, 2)?
         } else {
-            let in_dtype = q.dtype();
-            let q = q.to_dtype(DType::F32)?;
-            let k = k.to_dtype(DType::F32)?;
-            let v = v.to_dtype(DType::F32)?;
-            let att = (q.matmul(&k.t()?)? / (self.head_dim as f64).sqrt())?;
+            let att = MatMul.matmul_affine_div(&q, &k.t()?, (self.head_dim as f64).sqrt())?;
             let att = CausalMasker.apply_mask(attention_mask, att, &self.neg_inf)?;
             let att = candle_nn::ops::softmax(&att, D::Minus1)?;
             // Convert to contiguous as matmul doesn't support strided vs for now.
-            att.matmul(&v.contiguous()?)?.to_dtype(in_dtype)?
+            MatMul.matmul(&att, &v.contiguous()?)?
         };
         if matches!(self.q_proj, QMatMul::QTensor(_)) {
             y = y.to_dtype(DType::F32)?;
         }
         let y = y.transpose(1, 2)?.reshape(&[b_sz, seq_len, hidden_size])?;
-        let mut y = self.o_proj.forward(&y)?;
+        let mut y = MatMul.qmatmul(&y, &self.o_proj)?;
         if matches!(self.q_proj, QMatMul::QTensor(_)) {
             y = y.to_dtype(original_dtype)?;
         }
         Ok(y)
     }
 
     fn load(vb: VarBuilder, cfg: &Config, rope: Arc<RotaryEmbedding>) -> Result<Self> {
@@ -175,16 +154,17 @@
 impl Mlp {
     fn forward(&self, x: &Tensor) -> Result<Tensor> {
         let original_dtype = x.dtype();
         let mut x = x.clone();
         if matches!(self.c_fc1, QMatMul::QTensor(_)) {
             x = x.to_dtype(DType::F32)?;
         }
-        let x = (candle_nn::ops::silu(&self.c_fc1.forward(&x)?)? * self.c_fc2.forward(&x)?)?;
-        let mut res = self.c_proj.forward(&x)?;
+        let x = (candle_nn::ops::silu(&MatMul.qmatmul(&x, &self.c_fc1)?)?
+            * MatMul.qmatmul(&x, &self.c_fc2)?)?;
+        let mut res = MatMul.qmatmul(&x, &self.c_proj)?;
         if matches!(self.c_fc1, QMatMul::QTensor(_)) {
             res = res.to_dtype(original_dtype)?;
         }
         Ok(res)
     }
 
     fn load(vb: VarBuilder, cfg: &Config) -> Result<Self> {
@@ -213,15 +193,15 @@
     fn forward(
         &self,
         x: &Tensor,
         attention_mask: &Option<Tensor>,
         seqlen_offsets: &[usize],
         start_offsets_kernel: Tensor,
         block_idx: usize,
-        kv_cache: &mut super::LayerCaches,
+        kv_cache: &mut crate::pipeline::LayerCaches,
     ) -> Result<Tensor> {
         let residual = x;
         let x = self.rms_1.forward(x)?;
         let x = (self.attn.forward(
             &x,
             attention_mask,
             seqlen_offsets,
@@ -269,15 +249,15 @@
 
 #[derive(Debug)]
 pub struct Llama {
     wte: Embedding,
     blocks: Vec<Block>,
     ln_f: RmsNorm,
     lm_head: QMatMul,
-    pub kv_cache: super::Cache,
+    pub kv_cache: crate::pipeline::Cache,
     pub device: Device,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
 }
 
 impl Llama {
     pub fn forward(
         &mut self,
@@ -301,15 +281,15 @@
             )?;
         }
         let x = x.to_device(&self.device)?;
         let mut x = self.ln_f.forward(&x)?;
         if matches!(self.lm_head, QMatMul::QTensor(_)) {
             x = x.to_dtype(DType::F32)?;
         }
-        let logits = self.lm_head.forward(&x)?;
+        let logits = MatMul.qmatmul(&x, &self.lm_head)?;
         extract_logits(&logits, context_lens)
     }
 
     pub fn new(
         cfg: &Config,
         vb: VarBuilder,
         is_gptx: bool,
@@ -360,15 +340,15 @@
             .collect();
 
         Ok(Self {
             wte,
             blocks,
             ln_f,
             lm_head: QMatMul::Tensor(lm_head.weight().clone()),
-            kv_cache: super::Cache::new(cfg.num_hidden_layers, false),
+            kv_cache: crate::pipeline::Cache::new(cfg.num_hidden_layers, false),
             device: real_device,
             mapper,
         })
     }
 }
 
 impl NormalModel for Llama {
@@ -398,15 +378,15 @@
         _no_kv_cache: bool,
         _non_granular_state: &Option<crate::xlora_models::NonGranularState>,
         _context_lens: Vec<(usize, usize)>,
         _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
         unimplemented!()
     }
-    fn cache(&self) -> &super::Cache {
+    fn cache(&self) -> &crate::pipeline::Cache {
         &self.kv_cache
     }
     fn device(&self) -> &Device {
         &self.device
     }
     fn is_xlora(&self) -> bool {
         false
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/models/mistral.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/models/mistral.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
 /// Mistral LLM, https://github.com/mistralai/mistral-src
-use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor, D};
+use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor};
 use candle_nn::{linear_no_bias, Activation, RotaryEmbedding, VarBuilder};
 use std::sync::Arc;
 
 use crate::{
     device_map::DeviceMapper,
-    layers::{CausalMasker, RmsNorm},
-    pipeline::{extract_logits, NormalModel},
+    layers::{flash_attn, repeat_kv, CausalMasker, MatMul, RmsNorm},
+    pipeline::{extract_logits, Cache, NormalModel},
     DeviceMapMetadata,
 };
 
-use super::{flash_attn, repeat_kv, Cache};
-
 #[derive(Debug, Clone, PartialEq)]
 pub struct Config {
     pub(crate) vocab_size: usize,
     pub(crate) hidden_size: usize,
     pub(crate) intermediate_size: usize,
     pub(crate) num_hidden_layers: usize,
     pub(crate) num_attention_heads: usize,
@@ -58,17 +56,17 @@
 impl Module for MLP {
     fn forward(&self, xs: &Tensor) -> Result<Tensor> {
         let original_dtype = xs.dtype();
         let mut xs = xs.clone();
         if matches!(self.gate_proj, QMatMul::QTensor(_)) {
             xs = xs.to_dtype(DType::F32)?;
         }
-        let lhs = xs.apply(&self.gate_proj)?.apply(&self.act_fn)?;
-        let rhs = xs.apply(&self.up_proj)?;
-        let mut res = (lhs * rhs)?.apply(&self.down_proj)?;
+        let lhs = MatMul.qmatmul(&xs, &self.gate_proj)?.apply(&self.act_fn)?;
+        let rhs = MatMul.qmatmul(&xs, &self.up_proj)?;
+        let mut res = MatMul.qmatmul(&(lhs * rhs)?, &self.down_proj)?;
         if matches!(self.gate_proj, QMatMul::QTensor(_)) {
             res = res.to_dtype(original_dtype)?;
         }
         Ok(res)
     }
 }
 
@@ -128,17 +126,17 @@
         let (b_sz, q_len, _) = xs.dims3()?;
 
         let original_dtype = xs.dtype();
         let mut xs = xs.clone();
         if matches!(self.q_proj, QMatMul::QTensor(_)) {
             xs = xs.to_dtype(DType::F32)?;
         }
-        let mut q = self.q_proj.forward(&xs)?;
-        let mut k = self.k_proj.forward(&xs)?;
-        let mut v = self.v_proj.forward(&xs)?;
+        let mut q = MatMul.qmatmul(&xs, &self.q_proj)?;
+        let mut k = MatMul.qmatmul(&xs, &self.k_proj)?;
+        let mut v = MatMul.qmatmul(&xs, &self.v_proj)?;
         if matches!(self.q_proj, QMatMul::QTensor(_)) {
             q = q.to_dtype(original_dtype)?;
             k = k.to_dtype(original_dtype)?;
             v = v.to_dtype(original_dtype)?;
         }
 
         let mut q = q.reshape((b_sz * q_len, self.num_heads, self.head_dim))?;
@@ -157,77 +155,53 @@
                 .contiguous()?;
             k = k
                 .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
                 .transpose(1, 2)?
                 .contiguous()?;
         }
 
-        let (k, v, attn_mask) = match kv_cache.clone() {
-            None => (k, v, attention_mask.cloned()),
-            Some((mut prev_k, mut prev_v)) => {
-                let mut mask = attention_mask.cloned();
-                if let Some(sliding_window) = self.sliding_window {
-                    let kv_seq_len = prev_k.dim(2)?;
-                    if kv_seq_len > sliding_window {
-                        prev_k = prev_k.narrow(
-                            2,
-                            kv_seq_len - (sliding_window - 1),
-                            sliding_window - 1,
-                        )?;
-                        prev_v = prev_v.narrow(
-                            2,
-                            kv_seq_len - (sliding_window - 1),
-                            sliding_window - 1,
-                        )?;
-                        if let Some(ref mut mask) = mask {
-                            let mask_len = mask.dim(1)?;
-                            *mask = mask.narrow(
-                                1,
-                                mask_len - (sliding_window - 1),
-                                sliding_window - 1,
-                            )?;
-                            *mask = Tensor::cat(
-                                &[&*mask, &mask.narrow(1, mask_len - 1, 1)?.ones_like()?],
-                                D::Minus1,
-                            )?;
-                        }
-                    }
-                }
-                let k = candle_nn::ops::kvconcat(&prev_k, &k, 2)?;
-                let v = candle_nn::ops::kvconcat(&prev_v, &v, 2)?;
-                (k, v, mask)
-            }
-        };
-        *kv_cache = Some((k.clone(), v.clone()));
+        let (k, v, attn_mask) = Cache::update_kv_cache_sliding_window(
+            kv_cache,
+            k,
+            v,
+            attention_mask,
+            self.sliding_window,
+            false,
+        )?;
 
         let k = repeat_kv(k, self.num_kv_groups)?.contiguous()?;
         let v = repeat_kv(v, self.num_kv_groups)?.contiguous()?;
 
         let mut attn_output = if self.use_flash_attn {
             // flash-attn expects (b_sz, seq_len, nheads, head_dim)
             let q = q.transpose(1, 2)?;
             let k = k.transpose(1, 2)?;
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
-            let scale = 1f64 / f64::sqrt(self.head_dim as f64);
-            let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
+            let attn_weights = MatMul.matmul_affine_div(
+                &q,
+                &k.transpose(2, 3)?,
+                f64::sqrt(self.head_dim as f64),
+            )?;
 
             let attn_weights = CausalMasker.apply_mask(&attn_mask, attn_weights, &self.neg_inf)?;
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
-            attn_weights.matmul(&v)?
+            MatMul.matmul(&attn_weights, &v)?
         };
         if matches!(self.q_proj, QMatMul::QTensor(_)) {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
-        let mut res = attn_output
-            .transpose(1, 2)?
-            .reshape((b_sz, q_len, self.hidden_size))?
-            .apply(&self.o_proj)?;
+        let mut res = MatMul.qmatmul(
+            &attn_output
+                .transpose(1, 2)?
+                .reshape((b_sz, q_len, self.hidden_size))?,
+            &self.o_proj,
+        )?;
         if matches!(self.q_proj, QMatMul::QTensor(_)) {
             res = res.to_dtype(original_dtype)?;
         }
         Ok(res)
     }
 }
 
@@ -398,15 +372,15 @@
             )?;
         }
         let xs = xs.to_device(&self.device)?;
         let mut xs = xs.apply(&self.norm)?;
         if matches!(self.lm_head, QMatMul::QTensor(_)) {
             xs = xs.to_dtype(DType::F32)?;
         }
-        extract_logits(&xs.apply(&self.lm_head)?, context_lens)
+        extract_logits(&MatMul.qmatmul(&xs, &self.lm_head)?, context_lens)
     }
 }
 
 impl NormalModel for Model {
     fn forward(
         &mut self,
         input_ids: &Tensor,
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/models/mixtral.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/models/mixtral.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
 /// Mixtral Model
 /// https://github.com/huggingface/transformers/blob/main/src/transformers/models/mixtral/modeling_mixtral.py
 /// https://mistral.ai/news/mixtral-of-experts/
-use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor, D};
+use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor};
 use candle_nn::{linear_no_bias, Activation, RotaryEmbedding, VarBuilder};
 use serde::Deserialize;
 use std::sync::Arc;
 
 use crate::{
     device_map::DeviceMapper,
-    layers::{CausalMasker, RmsNorm},
-    pipeline::{extract_logits, NormalModel},
+    layers::{flash_attn, repeat_kv, CausalMasker, MatMul, RmsNorm},
+    pipeline::{extract_logits, Cache, NormalModel},
     DeviceMapMetadata,
 };
 
-use super::{flash_attn, repeat_kv, Cache};
-
 /// https://github.com/huggingface/transformers/blob/1a585c1222a56bcaecc070966d558d4a9d862e83/src/transformers/models/mixtral/configuration_mixtral.py#L113
 #[derive(Debug, Clone, PartialEq, Deserialize)]
 pub struct Config {
     pub(crate) vocab_size: usize,
     pub(crate) hidden_size: usize,
     pub(crate) intermediate_size: usize,
     pub(crate) num_hidden_layers: usize,
@@ -92,17 +90,17 @@
         let (b_sz, q_len, _) = xs.dims3()?;
 
         let original_dtype = xs.dtype();
         let mut xs = xs.clone();
         if matches!(self.q_proj, QMatMul::QTensor(_)) {
             xs = xs.to_dtype(DType::F32)?;
         }
-        let mut q = self.q_proj.forward(&xs)?;
-        let mut k = self.k_proj.forward(&xs)?;
-        let mut v = self.v_proj.forward(&xs)?;
+        let mut q = MatMul.qmatmul(&xs, &self.q_proj)?;
+        let mut k = MatMul.qmatmul(&xs, &self.k_proj)?;
+        let mut v = MatMul.qmatmul(&xs, &self.v_proj)?;
         if matches!(self.q_proj, QMatMul::QTensor(_)) {
             q = q.to_dtype(original_dtype)?;
             k = k.to_dtype(original_dtype)?;
             v = v.to_dtype(original_dtype)?;
         }
 
         let mut q = q.reshape((b_sz * q_len, self.num_heads, self.head_dim))?;
@@ -121,77 +119,53 @@
                 .contiguous()?;
             k = k
                 .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
                 .transpose(1, 2)?
                 .contiguous()?;
         }
 
-        let (k, v, attn_mask) = match kv_cache.clone() {
-            None => (k, v, attention_mask.cloned()),
-            Some((mut prev_k, mut prev_v)) => {
-                let mut mask = attention_mask.cloned();
-                if let Some(sliding_window) = self.sliding_window {
-                    let kv_seq_len = prev_k.dim(2)?;
-                    if kv_seq_len > sliding_window {
-                        prev_k = prev_k.narrow(
-                            2,
-                            kv_seq_len - (sliding_window - 1),
-                            sliding_window - 1,
-                        )?;
-                        prev_v = prev_v.narrow(
-                            2,
-                            kv_seq_len - (sliding_window - 1),
-                            sliding_window - 1,
-                        )?;
-                        if let Some(ref mut mask) = mask {
-                            let mask_len = mask.dim(1)?;
-                            *mask = mask.narrow(
-                                1,
-                                mask_len - (sliding_window - 1),
-                                sliding_window - 1,
-                            )?;
-                            *mask = Tensor::cat(
-                                &[&*mask, &mask.narrow(1, mask_len - 1, 1)?.ones_like()?],
-                                D::Minus1,
-                            )?;
-                        }
-                    }
-                }
-                let k = candle_nn::ops::kvconcat(&prev_k, &k, 2)?;
-                let v = candle_nn::ops::kvconcat(&prev_v, &v, 2)?;
-                (k, v, mask)
-            }
-        };
-        *kv_cache = Some((k.clone(), v.clone()));
+        let (k, v, attn_mask) = Cache::update_kv_cache_sliding_window(
+            kv_cache,
+            k,
+            v,
+            attention_mask,
+            self.sliding_window,
+            false,
+        )?;
 
         let k = repeat_kv(k, self.num_kv_groups)?.contiguous()?;
         let v = repeat_kv(v, self.num_kv_groups)?.contiguous()?;
 
         let mut attn_output = if self.use_flash_attn {
             // flash-attn expects (b_sz, seq_len, nheads, head_dim)
             let q = q.transpose(1, 2)?;
             let k = k.transpose(1, 2)?;
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
-            let scale = 1f64 / f64::sqrt(self.head_dim as f64);
-            let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
+            let attn_weights = MatMul.matmul_affine_div(
+                &q,
+                &k.transpose(2, 3)?,
+                f64::sqrt(self.head_dim as f64),
+            )?;
 
             let attn_weights = CausalMasker.apply_mask(&attn_mask, attn_weights, &self.neg_inf)?;
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
-            attn_weights.matmul(&v)?
+            MatMul.matmul(&attn_weights, &v)?
         };
         if matches!(self.q_proj, QMatMul::QTensor(_)) {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
-        let mut res = attn_output
-            .transpose(1, 2)?
-            .reshape((b_sz, q_len, self.hidden_size))?
-            .apply(&self.o_proj)?;
+        let mut res = MatMul.qmatmul(
+            &attn_output
+                .transpose(1, 2)?
+                .reshape((b_sz, q_len, self.hidden_size))?,
+            &self.o_proj,
+        )?;
         if matches!(self.q_proj, QMatMul::QTensor(_)) {
             res = res.to_dtype(original_dtype)?;
         }
         Ok(res)
     }
 }
 
@@ -222,17 +196,17 @@
 impl Module for BlockSparseTop2MLP {
     fn forward(&self, xs: &Tensor) -> Result<Tensor> {
         let original_dtype = xs.dtype();
         let mut xs = xs.clone();
         if matches!(self.w1, QMatMul::QTensor(_)) {
             xs = xs.to_dtype(DType::F32)?;
         }
-        let lhs = xs.apply(&self.w1)?.apply(&self.act_fn)?;
-        let rhs = xs.apply(&self.w3)?;
-        let mut res = (lhs * rhs)?.apply(&self.w2)?;
+        let lhs = MatMul.qmatmul(&xs, &self.w1)?.apply(&self.act_fn)?;
+        let rhs = MatMul.qmatmul(&xs, &self.w3)?;
+        let mut res = MatMul.qmatmul(&(lhs * rhs)?, &self.w2)?;
         if matches!(self.w1, QMatMul::QTensor(_)) {
             res = res.to_dtype(original_dtype)?;
         }
         Ok(res)
     }
 }
 
@@ -266,15 +240,15 @@
         let xs = xs.reshape(((), hidden_dim))?;
 
         let original_dtype = xs.dtype();
         let mut xs = xs.clone();
         if matches!(self.gate, QMatMul::QTensor(_)) {
             xs = xs.to_dtype(DType::F32)?;
         }
-        let mut router_logits = xs.apply(&self.gate)?;
+        let mut router_logits = MatMul.qmatmul(&xs, &self.gate)?;
         if matches!(self.gate, QMatMul::QTensor(_)) {
             router_logits = router_logits.to_dtype(original_dtype)?;
         }
 
         let routing_weights = candle_nn::ops::softmax_last_dim(&router_logits)?;
 
         // In order to extract topk, we extract the data from the tensor and manipulate it
@@ -501,15 +475,15 @@
             )?;
         }
         let xs = xs.to_device(&self.device)?;
         let mut xs = xs.apply(&self.norm)?;
         if matches!(self.lm_head, QMatMul::QTensor(_)) {
             xs = xs.to_dtype(DType::F32)?;
         }
-        extract_logits(&xs.apply(&self.lm_head)?, context_lens)
+        extract_logits(&MatMul.qmatmul(&xs, &self.lm_head)?, context_lens)
     }
 }
 
 impl NormalModel for Model {
     fn forward(
         &mut self,
         input_ids: &Tensor,
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/models/phi2.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/models/phi2.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,23 @@
 /// There is an alternative implementation of the phi model in mixformers.rs.
 /// This corresponds to the model update made with the following commit:
 /// https://huggingface.co/microsoft/phi-2/commit/cb2f4533604d8b67de604e7df03bfe6f3ca22869
 use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor};
 use candle_nn::{
     embedding, layer_norm, linear, Activation, Embedding, LayerNorm, RotaryEmbedding, VarBuilder,
 };
-use mistralrs_lora::layer::QLinear;
 use serde::Deserialize;
 
 use crate::{
     device_map::DeviceMapper,
-    layers::CausalMasker,
-    pipeline::{extract_logits, NormalModel},
+    layers::{flash_attn, repeat_kv, CausalMasker, MatMul, QLinear},
+    pipeline::{extract_logits, Cache, NormalModel},
     DeviceMapMetadata,
 };
 
-use super::{flash_attn, repeat_kv, Cache};
-
 // https://huggingface.co/microsoft/phi-2/blob/main/configuration_phi.py
 #[derive(Debug, Clone, PartialEq, Deserialize)]
 pub struct Config {
     pub(crate) vocab_size: usize,
     pub(crate) hidden_size: usize,
     pub(crate) intermediate_size: usize,
     pub(crate) num_hidden_layers: usize,
@@ -116,15 +113,15 @@
         let (q_layernorm, k_layernorm) = if cfg.qk_layernorm {
             let q_layernorm = layer_norm(head_dim, cfg.layer_norm_eps, vb.pp("q_layernorm"))?;
             let k_layernorm = layer_norm(head_dim, cfg.layer_norm_eps, vb.pp("k_layernorm"))?;
             (Some(q_layernorm), Some(k_layernorm))
         } else {
             (None, None)
         };
-        let softmax_scale = 1f64 / (head_dim as f64).sqrt();
+        let softmax_scale = (head_dim as f64).sqrt();
         Ok(Self {
             q_proj: QLinear::from_linear(q_proj),
             k_proj: QLinear::from_linear(k_proj),
             v_proj: QLinear::from_linear(v_proj),
             dense: QLinear::from_linear(dense),
             q_layernorm,
             k_layernorm,
@@ -192,44 +189,33 @@
                 .contiguous()?;
             k = k
                 .reshape((b_size, seq_len, self.num_kv_heads, self.head_dim))?
                 .transpose(1, 2)?
                 .contiguous()?;
         }
 
-        let (k, v) = match &*kv_cache {
-            None => (k, v),
-            Some((prev_k, prev_v)) => {
-                let k = candle_nn::ops::kvconcat(prev_k, &k, 2)?;
-                let v = candle_nn::ops::kvconcat(prev_v, &v, 2)?;
-                (k, v)
-            }
-        };
-        *kv_cache = Some((k.clone(), v.clone()));
+        let (k, v) = Cache::update_kv_cache(kv_cache, k, v, false)?;
 
         let k = repeat_kv(k, self.num_heads / self.num_kv_heads)?.contiguous()?;
         let v = repeat_kv(v, self.num_heads / self.num_kv_heads)?.contiguous()?;
 
         let mut attn_output = if self.use_flash_attn {
             // flash-attn expects (b_sz, seq_len, nheads, head_dim)
             let q = q.transpose(1, 2)?;
             let k = k.transpose(1, 2)?;
             let v = v.transpose(1, 2)?;
             flash_attn(&q, &k, &v, self.softmax_scale as f32, seq_len > 1)?.transpose(1, 2)?
         } else {
-            let attn_weights = (q
-                .to_dtype(DType::F32)?
-                .contiguous()?
-                .matmul(&k.to_dtype(DType::F32)?.t()?)?
-                * self.softmax_scale)?;
+            let attn_weights =
+                MatMul.matmul_affine_div(&q.contiguous()?, &k.t()?, self.softmax_scale)?;
             let attn_weights =
                 CausalMasker.apply_mask(&mask.cloned(), attn_weights, &self.neg_inf)?;
             let attn_weights =
                 candle_nn::ops::softmax_last_dim(&attn_weights)?.to_dtype(v.dtype())?;
-            attn_weights.matmul(&v)?
+            MatMul.matmul(&attn_weights, &v)?
         };
         if self.q_proj.is_quant() {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
         let mut res = attn_output
             .transpose(1, 2)?
             .reshape((b_size, seq_len, ()))?
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/models/phi3.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/models/qwen2.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,265 +1,227 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
-// This implementation is based on:
-// https://huggingface.co/microsoft/Phi-3-mini-4k-instruct/blob/main/modeling_phi3.py
-use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor, D};
-use candle_nn::{linear_no_bias, VarBuilder};
-use either::Either;
-use std::{collections::HashMap, sync::Arc};
+use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor};
+use candle_nn::{linear, linear_no_bias, Activation, RotaryEmbedding, VarBuilder};
+use std::sync::Arc;
 
 use crate::{
     device_map::DeviceMapper,
-    layers::{CausalMasker, PhiRotaryEmbedding, RmsNorm},
-    pipeline::{extract_logits, NormalModel},
+    layers::{flash_attn, repeat_kv, CausalMasker, MatMul, QLinear, RmsNorm},
+    pipeline::{extract_logits, Cache, NormalModel},
     DeviceMapMetadata,
 };
 
-use super::{flash_attn, repeat_kv, Cache};
-
-// https://huggingface.co/microsoft/Phi-3-mini-4k-instruct/blob/main/config.json
-#[derive(Debug, Clone, serde::Deserialize)]
+#[derive(Debug, Clone, PartialEq, serde::Deserialize)]
 pub struct Config {
     pub vocab_size: usize,
-    pub hidden_act: candle_nn::Activation,
     pub hidden_size: usize,
     pub intermediate_size: usize,
     pub num_hidden_layers: usize,
     pub num_attention_heads: usize,
     pub num_key_value_heads: usize,
-    pub rms_norm_eps: f64,
-    pub rope_theta: f64,
-    pub bos_token_id: Option<u32>,
-    pub eos_token_id: Option<u32>,
-    pub rope_scaling: Option<HashMap<String, Either<Vec<f32>, String>>>,
     pub max_position_embeddings: usize,
+    pub sliding_window: usize,
+    pub max_window_layers: usize,
+    pub tie_word_embeddings: bool,
+    pub rope_theta: f64,
+    pub rms_norm_eps: f64,
+    pub use_sliding_window: bool,
+    pub hidden_act: Activation,
     pub use_flash_attn: bool,
-    pub sliding_window: Option<usize>,
-    pub original_max_position_embeddings: usize,
 }
 
-impl Config {
-    pub fn head_dim(&self) -> usize {
-        self.hidden_size / self.num_attention_heads
+#[derive(Debug, Clone)]
+#[allow(clippy::upper_case_acronyms)]
+struct MLP {
+    gate_proj: QMatMul,
+    up_proj: QMatMul,
+    down_proj: QMatMul,
+    act_fn: Activation,
+}
+
+impl MLP {
+    fn new(cfg: &Config, vb: VarBuilder) -> Result<Self> {
+        let hidden_sz = cfg.hidden_size;
+        let intermediate_sz = cfg.intermediate_size;
+        let gate_proj = linear_no_bias(hidden_sz, intermediate_sz, vb.pp("gate_proj"))?;
+        let up_proj = linear_no_bias(hidden_sz, intermediate_sz, vb.pp("up_proj"))?;
+        let down_proj = linear_no_bias(intermediate_sz, hidden_sz, vb.pp("down_proj"))?;
+        Ok(Self {
+            gate_proj: QMatMul::Tensor(gate_proj.weight().clone()),
+            up_proj: QMatMul::Tensor(up_proj.weight().clone()),
+            down_proj: QMatMul::Tensor(down_proj.weight().clone()),
+            act_fn: cfg.hidden_act,
+        })
+    }
+}
+
+impl Module for MLP {
+    fn forward(&self, xs: &Tensor) -> Result<Tensor> {
+        let original_dtype = xs.dtype();
+        let mut xs = xs.clone();
+        if matches!(self.gate_proj, QMatMul::QTensor(_)) {
+            xs = xs.to_dtype(DType::F32)?;
+        }
+        let lhs = MatMul.qmatmul(&xs, &self.gate_proj)?.apply(&self.act_fn)?;
+        let rhs = MatMul.qmatmul(&xs, &self.up_proj)?;
+        let mut res = MatMul.qmatmul(&(lhs * rhs)?, &self.down_proj)?;
+        if matches!(self.gate_proj, QMatMul::QTensor(_)) {
+            res = res.to_dtype(original_dtype)?;
+        }
+        Ok(res)
     }
 }
 
 #[derive(Debug, Clone)]
 struct Attention {
-    qkv_proj: QMatMul,
+    q_proj: QLinear,
+    k_proj: QLinear,
+    v_proj: QLinear,
     o_proj: QMatMul,
     num_heads: usize,
     num_kv_heads: usize,
     num_kv_groups: usize,
     head_dim: usize,
-    rotary_emb: Arc<PhiRotaryEmbedding>,
+    rotary_emb: Arc<RotaryEmbedding>,
     use_flash_attn: bool,
-    sliding_window: Option<usize>,
     neg_inf: Tensor,
 }
 
 impl Attention {
-    fn new(rotary_emb: Arc<PhiRotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
+    fn new(rotary_emb: Arc<RotaryEmbedding>, cfg: &Config, vb: VarBuilder) -> Result<Self> {
+        let hidden_sz = cfg.hidden_size;
         let num_heads = cfg.num_attention_heads;
         let num_kv_heads = cfg.num_key_value_heads;
-        let head_dim = cfg.head_dim();
-        let op_size = num_heads * head_dim + 2 * num_kv_heads * head_dim;
-        let qkv_proj = linear_no_bias(cfg.hidden_size, op_size, vb.pp("qkv_proj"))?;
-        let o_proj = linear_no_bias(num_heads * head_dim, cfg.hidden_size, vb.pp("o_proj"))?;
+        let num_kv_groups = num_heads / num_kv_heads;
+        let head_dim = hidden_sz / num_heads;
+        let q_proj = linear(hidden_sz, num_heads * head_dim, vb.pp("q_proj"))?;
+        let k_proj = linear(hidden_sz, num_kv_heads * head_dim, vb.pp("k_proj"))?;
+        let v_proj = linear(hidden_sz, num_kv_heads * head_dim, vb.pp("v_proj"))?;
+        let o_proj = linear_no_bias(num_heads * head_dim, hidden_sz, vb.pp("o_proj"))?;
         Ok(Self {
-            qkv_proj: QMatMul::Tensor(qkv_proj.weight().clone()),
+            q_proj: QLinear::from_linear(q_proj),
+            k_proj: QLinear::from_linear(k_proj),
+            v_proj: QLinear::from_linear(v_proj),
             o_proj: QMatMul::Tensor(o_proj.weight().clone()),
-            rotary_emb,
             num_heads,
             num_kv_heads,
-            num_kv_groups: num_heads / num_kv_heads,
+            num_kv_groups,
             head_dim,
+            rotary_emb,
             use_flash_attn: cfg.use_flash_attn,
-            sliding_window: cfg.sliding_window,
             neg_inf: Tensor::new(f32::NEG_INFINITY, vb.device())?.to_dtype(vb.dtype())?,
         })
     }
 
     fn forward(
         &mut self,
         xs: &Tensor,
         attention_mask: Option<&Tensor>,
         seqlen_offsets: &[usize],
-        position_ids: &[usize],
+        start_offsets_kernel: Tensor,
         kv_cache: &mut Option<(Tensor, Tensor)>,
     ) -> Result<Tensor> {
         let (b_sz, q_len, _) = xs.dims3()?;
 
         let original_dtype = xs.dtype();
         let mut xs = xs.clone();
-        if matches!(self.qkv_proj, QMatMul::QTensor(_)) {
+        if self.q_proj.is_quant() {
             xs = xs.to_dtype(DType::F32)?;
         }
-        let mut qkv = self.qkv_proj.forward(&xs)?;
-        if matches!(self.qkv_proj, QMatMul::QTensor(_)) {
-            qkv = qkv.to_dtype(original_dtype)?;
-        }
-        let query_pos = self.num_heads * self.head_dim;
-        let q = qkv.narrow(D::Minus1, 0, query_pos)?;
-        let k = qkv.narrow(D::Minus1, query_pos, self.num_kv_heads * self.head_dim)?;
-        let v = qkv.narrow(
-            D::Minus1,
-            query_pos + self.num_kv_heads * self.head_dim,
-            self.num_kv_heads * self.head_dim,
-        )?;
+        let mut q = self.q_proj.forward(&xs)?;
+        let mut k = self.k_proj.forward(&xs)?;
+        let mut v = self.v_proj.forward(&xs)?;
+        if self.q_proj.is_quant() {
+            q = q.to_dtype(original_dtype)?;
+            k = k.to_dtype(original_dtype)?;
+            v = v.to_dtype(original_dtype)?;
+        }
 
-        let q = q
-            .reshape((b_sz, q_len, self.num_heads, self.head_dim))?
-            .transpose(1, 2)?;
-        let k = k
-            .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
-            .transpose(1, 2)?;
+        let mut q = q.reshape((b_sz * q_len, self.num_heads, self.head_dim))?;
+        let mut k = k.reshape((b_sz * q_len, self.num_kv_heads, self.head_dim))?;
         let v = v
             .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
             .transpose(1, 2)?;
 
-        let (q, k) = self
-            .rotary_emb
-            .forward(&q, &k, seqlen_offsets, position_ids)?;
-
-        let (k, v, attn_mask) = match kv_cache.clone() {
-            None => (k, v, attention_mask.cloned()),
-            Some((mut prev_k, mut prev_v)) => {
-                let mut mask = attention_mask.cloned();
-                if let Some(sliding_window) = self.sliding_window {
-                    let kv_seq_len = prev_k.dim(2)?;
-                    if kv_seq_len > sliding_window {
-                        prev_k = prev_k.narrow(
-                            2,
-                            kv_seq_len - (sliding_window - 1),
-                            sliding_window - 1,
-                        )?;
-                        prev_v = prev_v.narrow(
-                            2,
-                            kv_seq_len - (sliding_window - 1),
-                            sliding_window - 1,
-                        )?;
-                        if let Some(ref mut mask) = mask {
-                            let mask_len = mask.dim(1)?;
-                            *mask = mask.narrow(
-                                1,
-                                mask_len - (sliding_window - 1),
-                                sliding_window - 1,
-                            )?;
-                            *mask = Tensor::cat(
-                                &[&*mask, &mask.narrow(1, mask_len - 1, 1)?.ones_like()?],
-                                D::Minus1,
-                            )?;
-                        }
-                    }
-                }
-                let k = Tensor::cat(&[prev_k, k], 2)?;
-                let v = Tensor::cat(&[prev_v, v], 2)?;
-                (k, v, mask)
-            }
-        };
-        *kv_cache = Some((k.clone(), v.clone()));
+        self.rotary_emb
+            .forward(seqlen_offsets, &start_offsets_kernel, &mut q, &mut k, b_sz)?;
+
+        if q.rank() == 3 {
+            q = q
+                .reshape((b_sz, q_len, self.num_heads, self.head_dim))?
+                .transpose(1, 2)?
+                .contiguous()?;
+            k = k
+                .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
+                .transpose(1, 2)?
+                .contiguous()?;
+        }
+
+        let (k, v) = Cache::update_kv_cache(kv_cache, k, v, false)?;
 
         let k = repeat_kv(k, self.num_kv_groups)?.contiguous()?;
         let v = repeat_kv(v, self.num_kv_groups)?.contiguous()?;
 
         let mut attn_output = if self.use_flash_attn {
             // flash-attn expects (b_sz, seq_len, nheads, head_dim)
             let q = q.transpose(1, 2)?;
             let k = k.transpose(1, 2)?;
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
-            let scale = 1f64 / f64::sqrt(self.head_dim as f64);
-            let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
+            let attn_weights = MatMul.matmul_affine_div(
+                &q,
+                &k.transpose(2, 3)?,
+                f64::sqrt(self.head_dim as f64),
+            )?;
 
-            let attn_weights = CausalMasker.apply_mask(&attn_mask, attn_weights, &self.neg_inf)?;
+            let attn_weights =
+                CausalMasker.apply_mask(&attention_mask.cloned(), attn_weights, &self.neg_inf)?;
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
-            attn_weights.matmul(&v)?
+            MatMul.matmul(&attn_weights, &v)?
         };
-        if matches!(self.qkv_proj, QMatMul::QTensor(_)) {
+        if self.q_proj.is_quant() {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
-        let mut res = attn_output
-            .transpose(1, 2)?
-            .reshape((b_sz, q_len, ()))?
-            .apply(&self.o_proj)?;
-        if matches!(self.qkv_proj, QMatMul::QTensor(_)) {
-            res = res.to_dtype(original_dtype)?;
-        }
-        Ok(res)
-    }
-}
-
-#[derive(Debug, Clone)]
-struct Mlp {
-    gate_up_proj: QMatMul,
-    down_proj: QMatMul,
-    act_fn: candle_nn::Activation,
-    i_size: usize,
-}
-
-impl Mlp {
-    fn new(cfg: &Config, vb: VarBuilder) -> Result<Self> {
-        let hidden_size = cfg.hidden_size;
-        let i_size = cfg.intermediate_size;
-        let gate_up_proj = linear_no_bias(hidden_size, 2 * i_size, vb.pp("gate_up_proj"))?;
-        let down_proj = linear_no_bias(i_size, hidden_size, vb.pp("down_proj"))?;
-        Ok(Self {
-            gate_up_proj: QMatMul::Tensor(gate_up_proj.weight().clone()),
-            down_proj: QMatMul::Tensor(down_proj.weight().clone()),
-            act_fn: cfg.hidden_act,
-            i_size,
-        })
-    }
-}
-
-impl Module for Mlp {
-    fn forward(&self, xs: &Tensor) -> Result<Tensor> {
-        let original_dtype = xs.dtype();
-        let mut xs = xs.clone();
-        if matches!(self.gate_up_proj, QMatMul::QTensor(_)) {
-            xs = xs.to_dtype(DType::F32)?;
-        }
-        let up_states = xs.apply(&self.gate_up_proj)?;
-        let gate = up_states.narrow(D::Minus1, 0, self.i_size)?;
-        let up_states = up_states.narrow(D::Minus1, self.i_size, self.i_size)?;
-        let up_states = (up_states * gate.apply(&self.act_fn))?;
-        let mut res = up_states.apply(&self.down_proj)?;
-        if matches!(self.gate_up_proj, QMatMul::QTensor(_)) {
+        let mut res = MatMul.qmatmul(
+            &attn_output.transpose(1, 2)?.reshape((b_sz, q_len, ()))?,
+            &self.o_proj,
+        )?;
+        if self.q_proj.is_quant() {
             res = res.to_dtype(original_dtype)?;
         }
         Ok(res)
     }
 }
 
 #[derive(Debug, Clone)]
 struct DecoderLayer {
     self_attn: Attention,
-    mlp: Mlp,
+    mlp: MLP,
     input_layernorm: RmsNorm,
     post_attention_layernorm: RmsNorm,
 }
 
 impl DecoderLayer {
     fn new(
-        rotary_emb: Arc<PhiRotaryEmbedding>,
+        rotary_emb: Arc<RotaryEmbedding>,
         cfg: &Config,
         vb: VarBuilder,
         mapper: &dyn DeviceMapper,
         layer_idx: usize,
         loading_isq: bool,
     ) -> Result<Self> {
         let self_attn = Attention::new(
             rotary_emb,
             cfg,
             mapper.set_device(layer_idx, vb.pp("self_attn"), loading_isq),
         )?;
-        let mlp = Mlp::new(cfg, mapper.set_device(layer_idx, vb.pp("mlp"), loading_isq))?;
+        let mlp = MLP::new(cfg, mapper.set_device(layer_idx, vb.pp("mlp"), loading_isq))?;
         let input_layernorm = RmsNorm::new(
             cfg.hidden_size,
             cfg.rms_norm_eps,
             mapper.set_device(layer_idx, vb.pp("input_layernorm"), false),
         )?;
         let post_attention_layernorm = RmsNorm::new(
             cfg.hidden_size,
@@ -275,65 +237,73 @@
     }
 
     fn forward(
         &mut self,
         xs: &Tensor,
         attention_mask: Option<&Tensor>,
         seqlen_offsets: &[usize],
-        position_ids: &[usize],
+        start_offsets_kernel: Tensor,
         kv_cache: &mut Option<(Tensor, Tensor)>,
     ) -> Result<Tensor> {
         let residual = xs;
         let xs = self.input_layernorm.forward(xs)?;
-        let xs =
-            self.self_attn
-                .forward(&xs, attention_mask, seqlen_offsets, position_ids, kv_cache)?;
+        let xs = self.self_attn.forward(
+            &xs,
+            attention_mask,
+            seqlen_offsets,
+            start_offsets_kernel,
+            kv_cache,
+        )?;
         let xs = (xs + residual)?;
         let residual = &xs;
         let xs = xs.apply(&self.post_attention_layernorm)?.apply(&self.mlp)?;
         residual + xs
     }
 }
 
 #[derive(Debug)]
 pub struct Model {
     embed_tokens: candle_nn::Embedding,
     layers: Vec<DecoderLayer>,
     norm: RmsNorm,
     lm_head: QMatMul,
+    sliding_window: usize,
     pub device: Device,
     pub cache: Cache,
     pub max_seq_len: usize,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
-    sliding_window: Option<usize>,
 }
 
 impl Model {
     pub fn new(
         cfg: &Config,
         vb: VarBuilder,
-        _is_gptx: bool,
+        is_gptx: bool,
         mapper: DeviceMapMetadata,
         loading_isq: bool,
         real_device: Device,
     ) -> Result<Self> {
         let vb_m = vb.pp("model");
         let mapper = mapper.into_mapper(cfg.num_hidden_layers, &real_device)?;
         let embed_tokens = candle_nn::embedding(
             cfg.vocab_size,
             cfg.hidden_size,
             mapper.set_nm_device(vb_m.pp("embed_tokens"), false),
         )?;
         let mut layers = Vec::with_capacity(cfg.num_hidden_layers);
+        let head_dim = cfg.hidden_size / cfg.num_attention_heads;
         let vb_l = vb_m.pp("layers");
         for layer_idx in 0..cfg.num_hidden_layers {
-            let rotary_emb = Arc::new(PhiRotaryEmbedding::new(
-                vb.dtype(),
-                cfg,
+            let rotary_emb = Arc::new(RotaryEmbedding::new(
+                cfg.rope_theta as f32,
+                head_dim,
+                cfg.max_position_embeddings,
                 mapper.device_for(layer_idx, false).unwrap_or(&real_device),
+                is_gptx,
+                vb.dtype(),
             )?);
             let layer = DecoderLayer::new(
                 rotary_emb.clone(),
                 cfg,
                 vb_l.pp(layer_idx),
                 &*mapper,
                 layer_idx,
@@ -352,74 +322,73 @@
             mapper.set_nm_device(vb.pp("lm_head"), loading_isq),
         )?;
         Ok(Self {
             embed_tokens,
             layers,
             norm,
             lm_head: QMatMul::Tensor(lm_head.weight().clone()),
+            sliding_window: cfg.sliding_window,
             device: real_device,
             cache: Cache::new(cfg.num_hidden_layers, false),
             max_seq_len: cfg.max_position_embeddings,
             mapper,
-            sliding_window: cfg.sliding_window,
         })
     }
 
     pub fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
-        position_ids: &[usize],
+        start_offsets_kernel: Tensor,
         context_lens: Vec<(usize, usize)>,
     ) -> Result<Tensor> {
         let mut xs = self.embed_tokens.forward(input_ids)?;
         let mut cache = self.cache.lock();
         let attention_mask = CausalMasker.make_causal_mask_with_sliding_window(
             input_ids,
             &cache,
-            self.sliding_window,
+            Some(self.sliding_window),
         )?;
-        let past_key_values_length = CausalMasker.calculate_past_kv_len(&cache)?;
-        let position_ids = position_ids
-            .iter()
-            .map(|p| *p + past_key_values_length)
-            .collect::<Vec<_>>();
-
         for (i, layer) in self.layers.iter_mut().enumerate() {
             xs = self.mapper.map(xs, i)?;
             xs = layer.forward(
                 &xs,
                 attention_mask
                     .as_ref()
                     .map(|m| m.to_device(xs.device()).unwrap())
                     .as_ref(),
                 seqlen_offsets,
-                &position_ids,
+                start_offsets_kernel.clone(),
                 &mut cache[i],
             )?
         }
         let xs = xs.to_device(&self.device)?;
         let mut xs = xs.apply(&self.norm)?;
         if matches!(self.lm_head, QMatMul::QTensor(_)) {
             xs = xs.to_dtype(DType::F32)?;
         }
-        extract_logits(&xs.apply(&self.lm_head)?, context_lens)
+        extract_logits(&MatMul.qmatmul(&xs, &self.lm_head)?, context_lens)
     }
 }
 
 impl NormalModel for Model {
     fn forward(
         &mut self,
         input_ids: &Tensor,
         seqlen_offsets: &[usize],
-        _start_offsets_kernel: Tensor,
+        start_offsets_kernel: Tensor,
         context_lens: Vec<(usize, usize)>,
-        position_ids: Vec<usize>,
+        _position_ids: Vec<usize>,
     ) -> Result<Tensor> {
-        self.forward(input_ids, seqlen_offsets, &position_ids, context_lens)
+        self.forward(
+            input_ids,
+            seqlen_offsets,
+            start_offsets_kernel,
+            context_lens,
+        )
     }
     fn xlora_forward(
         &mut self,
         _input_ids: &Tensor,
         _input_ids_full: &Tensor,
         _seqlen_offsets: &[usize],
         _seqlen_offsets_full: &[usize],
@@ -444,15 +413,18 @@
     fn max_seq_len(&self) -> usize {
         self.max_seq_len
     }
     fn get_tensors(&mut self) -> (Vec<(&mut QMatMul, Option<usize>)>, &dyn DeviceMapper) {
         let mut tensors = Vec::new();
         tensors.push((&mut self.lm_head, None));
         for (i, layer) in self.layers.iter_mut().enumerate() {
-            tensors.push((&mut layer.self_attn.qkv_proj, Some(i)));
+            tensors.push((layer.self_attn.q_proj.inner(), Some(i)));
+            tensors.push((layer.self_attn.k_proj.inner(), Some(i)));
+            tensors.push((layer.self_attn.v_proj.inner(), Some(i)));
             tensors.push((&mut layer.self_attn.o_proj, Some(i)));
-            tensors.push((&mut layer.mlp.gate_up_proj, Some(i)));
             tensors.push((&mut layer.mlp.down_proj, Some(i)));
+            tensors.push((&mut layer.mlp.gate_proj, Some(i)));
+            tensors.push((&mut layer.mlp.up_proj, Some(i)));
         }
         (tensors, &*self.mapper)
     }
 }
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/models/quantized_llama.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/models/quantized_llama.rs`

 * *Files 6% similar despite different names*

```diff
@@ -2,49 +2,47 @@
 
 use candle_core::quantized::QMatMul;
 use candle_core::quantized::{ggml_file, gguf_file};
 use candle_core::{DType, Device, Result, Tensor};
 use candle_nn::{Embedding, Module, RotaryEmbedding};
 
 use crate::device_map::DeviceMapper;
-use crate::layers::{CausalMasker, QRmsNorm};
-use crate::pipeline::extract_logits;
+use crate::layers::{repeat_kv, verify_sanity_gguf, CausalMasker, MatMul, QRmsNorm};
+use crate::pipeline::{extract_logits, Cache};
 use crate::DeviceMapMetadata;
 
-use super::{repeat_kv, verify_sanity_gguf, Cache};
-
 const MAX_SEQ_LEN: u32 = 4096;
 
 #[derive(Debug, Clone)]
 struct Mlp {
     feed_forward_w1: QMatMul,
     feed_forward_w2: QMatMul,
     feed_forward_w3: QMatMul,
 }
 
-impl Module for Mlp {
+impl Mlp {
     fn forward(&self, xs: &Tensor) -> Result<Tensor> {
-        let w1 = self.feed_forward_w1.forward(xs)?;
-        let w3 = self.feed_forward_w3.forward(xs)?;
-        self.feed_forward_w2
-            .forward(&(candle_nn::ops::silu(&w1)? * w3)?)
+        let w1 = MatMul.qmatmul(xs, &self.feed_forward_w1)?;
+        let w3 = MatMul.qmatmul(xs, &self.feed_forward_w3)?;
+        let y = &(candle_nn::ops::silu(&w1)? * w3)?;
+        MatMul.qmatmul(y, &self.feed_forward_w2)
     }
 }
 
 #[derive(Debug, Clone)]
 enum MlpOrMoe {
     Mlp(Mlp),
     MoE {
         n_expert_used: usize,
         feed_forward_gate_inp: QMatMul,
         experts: Vec<Mlp>,
     },
 }
 
-impl Module for MlpOrMoe {
+impl MlpOrMoe {
     fn forward(&self, xs: &Tensor) -> Result<Tensor> {
         match self {
             Self::MoE {
                 feed_forward_gate_inp,
                 experts,
                 n_expert_used,
             } => {
@@ -132,17 +130,18 @@
         x: &Tensor,
         mask: &Option<Tensor>,
         start_offsets: &[usize],
         start_offsets_kernel: Tensor,
         kv_cache: &mut Option<(Tensor, Tensor)>,
     ) -> Result<Tensor> {
         let (b_sz, seq_len, n_embd) = x.dims3()?;
-        let q = self.attention_wq.forward(x)?;
-        let k = self.attention_wk.forward(x)?;
-        let v = self.attention_wv.forward(x)?;
+
+        let q = MatMul.qmatmul(x, &self.attention_wq)?;
+        let k = MatMul.qmatmul(x, &self.attention_wk)?;
+        let v = MatMul.qmatmul(x, &self.attention_wv)?;
 
         let mut q = q.reshape((b_sz * seq_len, self.n_head, self.head_dim))?;
         let mut k = k.reshape((b_sz * seq_len, self.n_kv_head, self.head_dim))?;
         let v = v
             .reshape((b_sz, seq_len, self.n_kv_head, self.head_dim))?
             .transpose(1, 2)?;
 
@@ -155,34 +154,31 @@
                 .transpose(1, 2)?
                 .contiguous()?;
             k = k
                 .reshape((b_sz, seq_len, self.n_kv_head, self.head_dim))?
                 .transpose(1, 2)?;
         }
 
-        let (k, v) = match &*kv_cache {
-            None => (k, v),
-            Some((k_cache, v_cache)) => {
-                let k = candle_nn::ops::kvconcat(k_cache, &k, 2)?.contiguous()?;
-                let v = candle_nn::ops::kvconcat(v_cache, &v, 2)?.contiguous()?;
-                (k, v)
-            }
-        };
-        *kv_cache = Some((k.clone(), v.clone()));
+        let (k, v) = Cache::update_kv_cache(kv_cache, k, v, false)?;
 
-        let k = repeat_kv(k, self.n_head / self.n_kv_head)?.contiguous()?;
-        let v = repeat_kv(v, self.n_head / self.n_kv_head)?.contiguous()?;
+        let k = repeat_kv(k, self.n_head / self.n_kv_head)?;
+        let v = repeat_kv(v, self.n_head / self.n_kv_head)?;
+        let att = MatMul.matmul_affine_div(
+            &q.contiguous()?,
+            &k.t()?.contiguous()?,
+            (self.head_dim as f64).sqrt(),
+        )?;
 
-        let att = (q.contiguous()?.matmul(&k.t()?.contiguous()?)? / (self.head_dim as f64).sqrt())?;
         let att = CausalMasker.apply_mask(mask, att, &self.neg_inf)?;
         let att = candle_nn::ops::softmax_last_dim(&att)?;
         // Convert to contiguous as matmul doesn't support strided vs for now.
-        let y = att.matmul(&v.contiguous()?)?;
+        let y = MatMul.matmul(&att, &v.contiguous()?)?;
+
         let y = y.transpose(1, 2)?.reshape(&[b_sz, seq_len, n_embd])?;
-        let y = self.attention_wo.forward(&y)?;
+        let y = MatMul.qmatmul(&y, &self.attention_wo)?;
         Ok(y)
     }
 }
 
 #[derive(Debug)]
 pub struct ModelWeights {
     tok_embeddings: Embedding,
@@ -420,10 +416,13 @@
             let x = layer.ffn_norm.forward(&x)?;
             let x = layer.mlp_or_moe.forward(&x)?;
             let x = (x + residual)?;
             layer_in = x;
         }
         let layer_in = layer_in.to_device(&self.device)?;
         let x = self.norm.forward(&layer_in)?;
-        extract_logits(&self.output.forward(&x.contiguous()?)?, context_lens)
+        extract_logits(
+            &MatMul.qmatmul(&x.contiguous()?, &self.output)?,
+            context_lens,
+        )
     }
 }
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/models/quantized_phi2.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/models/quantized_phi2.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
 use candle_core::quantized::gguf_file;
 use candle_core::quantized::QTensor;
 use candle_core::{DType, Device, IndexOp, Module, Result, Tensor, D};
 use candle_nn::{Embedding, LayerNorm};
-use mistralrs_lora::layer::QLinear;
 
 use crate::device_map::DeviceMapper;
-use crate::layers::CausalMasker;
-use crate::pipeline::extract_logits;
+use crate::layers::MatMul;
+use crate::layers::{repeat_kv, CausalMasker, QLinear};
+use crate::pipeline::{extract_logits, Cache};
 use crate::DeviceMapMetadata;
 
-use super::repeat_kv;
-use super::Cache;
-
 pub const MAX_SEQ_LEN: usize = 4096;
 
 #[derive(Debug, Clone)]
 struct Mlp {
     ffn_up: QLinear,
     ffn_down: QLinear,
 }
@@ -79,32 +76,24 @@
         // actually a no-op except when processing the initial prompt so has no significant
         // impact on performance.
         let v = v.contiguous()?;
 
         let q = self.forward(&q, seqlen_offsets)?.contiguous()?;
         let k = self.forward(&k, seqlen_offsets)?;
 
-        let (k, v) = match &*kv_cache {
-            None => (k, v),
-            Some((prev_k, prev_v)) => {
-                let k = Tensor::cat(&[prev_k, &k], 2)?;
-                let v = Tensor::cat(&[prev_v, &v], 2)?;
-                (k, v)
-            }
-        };
-        *kv_cache = Some((k.clone(), v.clone()));
+        let (k, v) = Cache::update_kv_cache(kv_cache, k, v, false)?;
 
         let k = repeat_kv(k, self.n_head / self.n_kv_head)?;
         let v = repeat_kv(v, self.n_head / self.n_kv_head)?;
 
-        let att = (q.matmul(&k.t()?)? / (self.head_dim as f64).sqrt())?;
+        let att = MatMul.matmul_affine_div(&q, &k.t()?, (self.head_dim as f64).sqrt())?;
         let att = CausalMasker.apply_mask(&mask.cloned(), att, &self.neg_inf)?;
         let att = candle_nn::ops::softmax_last_dim(&att)?;
         // Convert to contiguous as matmul doesn't support strided vs for now.
-        let y = att.matmul(&v.contiguous()?)?;
+        let y = MatMul.matmul(&att, &v.contiguous()?)?;
         let y = y.transpose(1, 2)?.reshape(&[b_sz, seq_len, n_embd])?;
         let y = self.attn_output.forward(&y)?;
         Ok(y)
     }
 }
 
 #[derive(Debug)]
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/models/quantized_phi3.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/models/quantized_phi3.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
 use crate::device_map::DeviceMapper;
-use crate::layers::CausalMasker;
-use crate::layers::RmsNorm;
+use crate::layers::{repeat_kv, verify_sanity_gguf, CausalMasker, MatMul, RmsNorm};
+use crate::pipeline::Cache;
 use crate::DeviceMapMetadata;
 use candle_core::quantized::gguf_file;
 use candle_core::quantized::QMatMul;
 use candle_core::quantized::QTensor;
 use candle_core::{DType, Device, IndexOp, Module, Result, Tensor, D};
 use candle_nn::Embedding;
 
-use super::repeat_kv;
-use super::verify_sanity_gguf;
-use super::Cache;
-
 #[derive(Debug, Clone)]
 struct Mlp {
     ffn_up: QMatMul,
     ffn_down: QMatMul,
     i_size: usize,
 }
 
 impl Module for Mlp {
     fn forward(&self, xs: &Tensor) -> Result<Tensor> {
-        let up_states = xs.apply(&self.ffn_up)?;
+        let up_states = MatMul.qmatmul(xs, &self.ffn_up)?;
         let gate = up_states.narrow(D::Minus1, 0, self.i_size)?;
         let up_states = up_states.narrow(D::Minus1, self.i_size, self.i_size)?;
         let up_states = (up_states * gate.silu()?)?;
-        up_states.apply(&self.ffn_down)
+        MatMul.qmatmul(&up_states, &self.ffn_down)
     }
 }
 
 fn rms_norm(w: QTensor, eps: f64) -> Result<RmsNorm> {
     let w = w.dequantize(&w.device())?;
     let rms = RmsNorm::from_w(w, eps)?;
     Ok(rms)
@@ -73,16 +69,15 @@
         &mut self,
         x: &Tensor,
         mask: Option<&Tensor>,
         seqlen_offsets: &[usize],
         kv_cache: &mut Option<(Tensor, Tensor)>,
     ) -> Result<Tensor> {
         let (b_sz, seq_len, n_embd) = x.dims3()?;
-        let qkv = self.attn_qkv.forward(x)?;
-
+        let qkv = MatMul.qmatmul(x, &self.attn_qkv)?;
         let query_pos = self.n_head * self.head_dim;
         let q = qkv.narrow(D::Minus1, 0, query_pos)?;
         let k = qkv.narrow(D::Minus1, query_pos, self.n_kv_head * self.head_dim)?;
         let v = qkv.narrow(
             D::Minus1,
             query_pos + self.n_kv_head * self.head_dim,
             self.n_kv_head * self.head_dim,
@@ -97,52 +92,33 @@
         let v = v
             .reshape((b_sz, seq_len, self.n_kv_head, self.head_dim))?
             .transpose(1, 2)?;
 
         let q = self.apply_rotary_emb(&q, seqlen_offsets)?.contiguous()?;
         let k = self.apply_rotary_emb(&k, seqlen_offsets)?;
 
-        let (k, v, attn_mask) = match kv_cache.clone() {
-            None => (k, v, mask.cloned()),
-            Some((mut prev_k, mut prev_v)) => {
-                let mut mask = mask.cloned();
-                let kv_seq_len = prev_k.dim(2)?;
-                let sliding_window = self.sliding_window;
-                if kv_seq_len > sliding_window {
-                    prev_k =
-                        prev_k.narrow(2, kv_seq_len - (sliding_window - 1), sliding_window - 1)?;
-                    prev_v =
-                        prev_v.narrow(2, kv_seq_len - (sliding_window - 1), sliding_window - 1)?;
-                    if let Some(ref mut mask) = mask {
-                        let mask_len = mask.dim(1)?;
-                        *mask =
-                            mask.narrow(1, mask_len - (sliding_window - 1), sliding_window - 1)?;
-                        *mask = Tensor::cat(
-                            &[&*mask, &mask.narrow(1, mask_len - 1, 1)?.ones_like()?],
-                            D::Minus1,
-                        )?;
-                    }
-                }
-                let k = Tensor::cat(&[prev_k, k], 2)?;
-                let v = Tensor::cat(&[prev_v, v], 2)?;
-                (k, v, mask)
-            }
-        };
-        *kv_cache = Some((k.clone(), v.clone()));
+        let (k, v, attn_mask) = Cache::update_kv_cache_sliding_window(
+            kv_cache,
+            k,
+            v,
+            mask,
+            Some(self.sliding_window),
+            true,
+        )?;
 
         let k = repeat_kv(k, self.n_head / self.n_kv_head)?;
         let v = repeat_kv(v, self.n_head / self.n_kv_head)?;
 
-        let att = (q.matmul(&k.t()?)? / (self.head_dim as f64).sqrt())?;
+        let att = MatMul.matmul_affine_div(&q, &k.t()?, (self.head_dim as f64).sqrt())?;
         let att = CausalMasker.apply_mask(&attn_mask, att, &self.neg_inf)?;
         let att = candle_nn::ops::softmax_last_dim(&att)?;
         // Convert to contiguous as matmul doesn't support strided vs for now.
-        let y = att.matmul(&v.contiguous()?)?;
+        let y = MatMul.matmul(&att, &v.contiguous()?)?;
         let y = y.transpose(1, 2)?.reshape(&[b_sz, seq_len, n_embd])?;
-        let y = self.attn_output.forward(&y)?;
+        let y = MatMul.qmatmul(&y, &self.attn_output)?;
         Ok(y)
     }
 }
 
 #[derive(Debug)]
 pub struct ModelWeights {
     tok_embeddings: Embedding,
@@ -294,10 +270,10 @@
             let residual = &ys;
             let ys = ys.apply(&layer.ffn_norm)?;
             let ys = layer.mlp.forward(&ys)?;
             xs = (ys + residual)?
         }
         let xs = xs.to_device(&self.device)?;
         let xs = xs.apply(&self.output_norm)?.i((.., seq_len - 1, ..))?;
-        self.output.forward(&xs)
+        MatMul.qmatmul(&xs, &self.output)
     }
 }
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/chat_template.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/pipeline/chat_template.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/ggml.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/pipeline/ggml.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 use super::cache_manager::DefaultCacheManager;
 use super::{
     get_model_paths, get_xlora_paths, CacheManager, GeneralMetadata, Loader, ModelInputs,
     ModelKind, ModelPaths, Pipeline, TokenSource, XLoraPaths,
 };
 use crate::aici::bintokens::build_tok_trie;
 use crate::aici::toktree::TokTrie;
-use crate::models::Cache;
+use crate::lora::Ordering;
 use crate::pipeline::chat_template::calculate_eos_tokens;
-use crate::pipeline::{ChatTemplate, SimpleModelPaths};
+use crate::pipeline::Cache;
+use crate::pipeline::{ChatTemplate, LocalModelPaths};
 use crate::prefix_cacher::PrefixCacheManager;
 use crate::sequence::Sequence;
+use crate::utils::tokenizer::get_tokenizer;
 use crate::utils::varbuilder_utils::{from_mmaped_safetensors, load_preload_adapters};
 use crate::xlora_models::NonGranularState;
 use crate::{deserialize_chat_template, do_sample, get_mut_arcmutex, get_paths, DeviceMapMetadata};
 use crate::{
     models::quantized_llama::ModelWeights as QLlama, utils::tokens::get_token,
     xlora_models::XLoraQLlama,
 };
 use anyhow::Result;
 use candle_core::quantized::{ggml_file, GgmlDType};
 use candle_core::{DType, Device, Tensor};
 use hf_hub::{api::sync::ApiBuilder, Repo, RepoType};
-use mistralrs_lora::Ordering;
 use rand_isaac::Isaac64Rng;
 use serde_json::Value;
 use std::collections::HashMap;
 use std::fs;
 use std::path::PathBuf;
 use std::str::FromStr;
 use std::sync::Arc;
@@ -206,35 +207,23 @@
             tgt_non_granular_index,
         }
     }
 }
 
 impl Loader for GGMLLoader {
     #[allow(clippy::type_complexity, clippy::too_many_arguments)]
-    fn load_model(
+    fn load_model_from_path(
         &self,
-        revision: Option<String>,
-        token_source: TokenSource,
+        paths: &Box<dyn ModelPaths>,
         _dtype: Option<DType>,
         device: &Device,
         silent: bool,
         mapper: DeviceMapMetadata,
         in_situ_quant: Option<GgmlDType>,
     ) -> Result<Arc<Mutex<dyn Pipeline + Send + Sync>>> {
-        let paths: anyhow::Result<Box<dyn ModelPaths>> = get_paths!(
-            SimpleModelPaths,
-            &token_source,
-            revision,
-            self,
-            self.quantized_model_id,
-            self.quantized_filename,
-            silent
-        );
-        let paths = paths?;
-
         if in_situ_quant.is_some() {
             anyhow::bail!(
                 "You are trying to in-situ quantize a GGUF model. This will not do anything."
             );
         }
         if !mapper.is_dummy() {
             warn!("GGML models do not support device mapping. Device mapping will not work. Please consider using a GGUF model.");
@@ -309,16 +298,15 @@
                         silent,
                     )?,
                 )?)
             }
             _ => unreachable!(),
         };
 
-        let tokenizer =
-            Tokenizer::from_file(paths.get_tokenizer_filename()).map_err(anyhow::Error::msg)?;
+        let tokenizer = get_tokenizer(paths.get_tokenizer_filename())?;
 
         let (chat_template, gen_conf) = deserialize_chat_template!(paths, self);
 
         let max_seq_len = match model {
             Model::Llama(ref l) => l.max_seq_len,
             Model::XLoraLlama(ref xl) => xl.max_seq_len,
         };
@@ -354,14 +342,37 @@
                 num_hidden_layers,
                 eos_tok: eos,
                 is_lora,
             },
         })))
     }
 
+    #[allow(clippy::type_complexity, clippy::too_many_arguments)]
+    fn load_model_from_hf(
+        &self,
+        revision: Option<String>,
+        token_source: TokenSource,
+        _dtype: Option<DType>,
+        device: &Device,
+        silent: bool,
+        mapper: DeviceMapMetadata,
+        in_situ_quant: Option<GgmlDType>,
+    ) -> Result<Arc<Mutex<dyn Pipeline + Send + Sync>>> {
+        let paths: anyhow::Result<Box<dyn ModelPaths>> = get_paths!(
+            LocalModelPaths,
+            &token_source,
+            revision,
+            self,
+            self.quantized_model_id,
+            self.quantized_filename,
+            silent
+        );
+        self.load_model_from_path(&paths?, _dtype, device, silent, mapper, in_situ_quant)
+    }
+
     fn get_id(&self) -> String {
         self.xlora_model_id
             .as_deref()
             .unwrap_or(&self.model_id)
             .to_string()
     }
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/gguf.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/pipeline/gguf.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 use super::cache_manager::DefaultCacheManager;
 use super::{
     get_model_paths, get_xlora_paths, CacheManager, GeneralMetadata, Loader, ModelInputs,
     ModelKind, ModelPaths, Pipeline, TokenSource, XLoraPaths,
 };
 use crate::aici::bintokens::build_tok_trie;
 use crate::aici::toktree::TokTrie;
-use crate::models::Cache;
+use crate::lora::Ordering;
 use crate::pipeline::chat_template::calculate_eos_tokens;
-use crate::pipeline::{ChatTemplate, SimpleModelPaths};
+use crate::pipeline::Cache;
+use crate::pipeline::{ChatTemplate, LocalModelPaths};
 use crate::prefix_cacher::PrefixCacheManager;
 use crate::sequence::Sequence;
+use crate::utils::tokenizer::get_tokenizer;
 use crate::utils::varbuilder_utils::{from_mmaped_safetensors, load_preload_adapters};
 use crate::xlora_models::NonGranularState;
 use crate::{deserialize_chat_template, do_sample, get_mut_arcmutex, get_paths, DeviceMapMetadata};
 use crate::{
     models::quantized_llama::ModelWeights as QLlama,
     models::quantized_phi2::ModelWeights as QPhi,
     models::quantized_phi3::ModelWeights as QPhi3,
@@ -23,15 +25,14 @@
 use anyhow::{bail, Result};
 use candle_core::quantized::{
     gguf_file::{self, Value as GgufValue},
     GgmlDType,
 };
 use candle_core::{DType, Device, Tensor};
 use hf_hub::{api::sync::ApiBuilder, Repo, RepoType};
-use mistralrs_lora::Ordering;
 use rand_isaac::Isaac64Rng;
 use serde_json::Value;
 use std::collections::HashMap;
 use std::fs;
 use std::path::PathBuf;
 use std::str::FromStr;
 use std::sync::Arc;
@@ -272,35 +273,46 @@
         GgufValue::U32(x) => x.to_string(),
         GgufValue::U64(x) => x.to_string(),
     }
 }
 
 impl Loader for GGUFLoader {
     #[allow(clippy::type_complexity, clippy::too_many_arguments)]
-    fn load_model(
+    fn load_model_from_hf(
         &self,
         revision: Option<String>,
         token_source: TokenSource,
         _dtype: Option<DType>,
         device: &Device,
         silent: bool,
         mapper: DeviceMapMetadata,
         in_situ_quant: Option<GgmlDType>,
     ) -> Result<Arc<Mutex<dyn Pipeline + Send + Sync>>> {
         let paths: anyhow::Result<Box<dyn ModelPaths>> = get_paths!(
-            SimpleModelPaths,
+            LocalModelPaths,
             &token_source,
             revision,
             self,
             self.quantized_model_id,
             self.quantized_filename,
             silent
         );
-        let paths = paths?;
+        self.load_model_from_path(&paths?, _dtype, device, silent, mapper, in_situ_quant)
+    }
 
+    #[allow(clippy::type_complexity, clippy::too_many_arguments)]
+    fn load_model_from_path(
+        &self,
+        paths: &Box<dyn ModelPaths>,
+        _dtype: Option<DType>,
+        device: &Device,
+        silent: bool,
+        mapper: DeviceMapMetadata,
+        in_situ_quant: Option<GgmlDType>,
+    ) -> Result<Arc<Mutex<dyn Pipeline + Send + Sync>>> {
         if in_situ_quant.is_some() {
             anyhow::bail!(
                 "You are trying to in-situ quantize a GGUF model. This will not do anything."
             );
         }
         let mut file = std::fs::File::open(paths.get_weight_filenames().first().unwrap())?;
         let model = gguf_file::Content::read(&mut file)
@@ -308,17 +320,19 @@
         let arch: GGUFArchitecture = model.metadata["general.architecture"]
             .to_string()
             .unwrap()
             .parse()
             .map_err(anyhow::Error::msg)?;
 
         info!("Model config:");
-        for (name, value) in &model.metadata {
+        let mut sorted_keys = model.metadata.keys().collect::<Vec<_>>();
+        sorted_keys.sort();
+        for name in sorted_keys {
             if !name.contains("tokenizer") {
-                let value = parse_gguf_value(value);
+                let value = parse_gguf_value(&model.metadata[name]);
                 println!("{name}: {}", value);
             }
         }
 
         let mut is_lora = false;
         let model = match self.kind {
             ModelKind::QuantizedGGUF => match arch {
@@ -429,22 +443,21 @@
                         &load_preload_adapters(
                             paths.get_lora_preload_adapter_info(),
                             DType::F32,
                             device,
                             silent,
                         )?,
                     )?),
-                    a => bail!("Unsupported architecture for GGUF X-LoRA `{a:?}`"),
+                    a => bail!("Unsupported architecture for GGUF LoRA `{a:?}`"),
                 }
             }
             _ => unreachable!(),
         };
 
-        let tokenizer =
-            Tokenizer::from_file(paths.get_tokenizer_filename()).map_err(anyhow::Error::msg)?;
+        let tokenizer = get_tokenizer(paths.get_tokenizer_filename())?;
 
         let (chat_template, gen_conf) = deserialize_chat_template!(paths, self);
 
         let max_seq_len = match model {
             Model::Llama(ref l) => l.max_seq_len,
             Model::Phi2(ref p) => p.max_seq_len,
             Model::XLoraLlama(ref xl) => xl.max_seq_len,
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/loaders.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/pipeline/loaders.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 use std::{collections::HashMap, fmt::Debug, str::FromStr};
 
+use crate::lora::{LoraConfig, Ordering};
 use anyhow::Result;
 use candle_core::Device;
 use candle_nn::{Activation, VarBuilder};
 use either::Either;
-use mistralrs_lora::{LoraConfig, Ordering};
+
+#[cfg(feature = "pyo3_macros")]
 use pyo3::pyclass;
+
 use serde::Deserialize;
 
 use super::{NormalModel, NormalModelLoader};
 use crate::{
     models,
     xlora_models::{self, XLoraConfig},
     DeviceMapMetadata,
 };
 
-#[pyclass]
+#[cfg_attr(feature = "pyo3_macros", pyclass)]
 #[derive(Clone, Debug, Deserialize)]
 /// The architecture to load the normal model as.
 pub enum NormalLoaderType {
     #[serde(rename = "mistral")]
     Mistral,
     #[serde(rename = "gemma")]
     Gemma,
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/macros.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/pipeline/macros.rs`

 * *Files 2% similar despite different names*

```diff
@@ -271,16 +271,15 @@
         )?
     }};
 }
 
 #[macro_export]
 macro_rules! lora_model_loader {
     ($paths:expr, $dtype:expr, $default_dtype:expr, $device:expr, $config:expr, $loader:expr, $use_flash_attn:expr, $silent:expr, $mapper:expr, $loading_isq:expr, $real_device:expr) => {{
-        let mut safetensors_paths = $paths.get_weight_filenames().iter().collect::<Vec<_>>();
-        safetensors_paths.push($paths.get_classifier_path().as_ref().unwrap());
+        let safetensors_paths = $paths.get_weight_filenames().iter().collect::<Vec<_>>();
         let vb = from_mmaped_safetensors(
             safetensors_paths
                 .iter()
                 .map(|x| (*x).to_owned())
                 .collect::<Vec<_>>(),
             $paths
                 .get_adapter_filenames()
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/mod.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/pipeline/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,18 @@
 mod loaders;
 mod macros;
 mod normal;
 mod sampling;
 mod speculative;
 use crate::aici::toktree::TokTrie;
 use crate::device_map::DeviceMapper;
+use crate::layers::set_use_matmul_via_f16;
 use crate::prefix_cacher::PrefixCacheManager;
 mod sampling_pipeline;
+use crate::lora::{LoraConfig, Ordering};
 use crate::{api_dir_list, api_get_file, DeviceMapMetadata};
 use candle_core::quantized::{GgmlDType, QMatMul, QTensor};
 use candle_nn::VarBuilder;
 use chat_template::{apply_chat_template_to, ChatTemplate};
 use core::fmt;
 use either::Either;
 pub use ggml::{GGMLLoader, GGMLLoaderBuilder, GGMLSpecificConfig};
@@ -25,15 +27,14 @@
 };
 use indexmap::IndexMap;
 use indicatif::{ParallelProgressIterator, ProgressBar, ProgressStyle};
 pub use loaders::{
     GemmaLoader, LlamaLoader, MistralLoader, MixtralLoader, NormalLoaderType, Phi2Loader,
     Phi3Loader, Qwen2Loader,
 };
-use mistralrs_lora::{LoraConfig, Ordering};
 pub use normal::{NormalLoader, NormalLoaderBuilder, NormalSpecificConfig};
 use rand_isaac::Isaac64Rng;
 use rayon::iter::{IndexedParallelIterator, IntoParallelIterator, ParallelIterator};
 pub use speculative::{SpeculativeConfig, SpeculativeLoader, SpeculativePipeline};
 use std::fmt::{Debug, Display};
 use std::path::Path;
 use std::sync::atomic::AtomicUsize;
@@ -43,49 +44,107 @@
 use tokio::sync::Mutex;
 use tracing::{info, warn};
 
 use anyhow::Result;
 use candle_core::{DType, Device, Tensor};
 
 use crate::{
-    models::Cache,
     sequence::Sequence,
     utils::tokens::get_token,
     xlora_models::{NonGranularState, XLoraConfig},
 };
 
+pub use self::cache_manager::{Cache, CacheManager, LayerCaches};
+
+/// `ModelPaths` abstracts the mechanism to get all necessary files for running a model. For
+/// example `SimpleModelPaths` implements `ModelPaths` when all files are in the local file system.
 pub trait ModelPaths {
+    /// Model weights files (multiple files supported).
     fn get_weight_filenames(&self) -> &[PathBuf];
+
+    /// Retrieve the PretrainedConfig file.
+    /// See: https://huggingface.co/docs/transformers/v4.40.2/en/main_classes/configuration#transformers.PretrainedConfig
     fn get_config_filename(&self) -> &PathBuf;
+
+    /// A serialised `tokenizers.Tokenizer` HuggingFace object.
+    /// See: https://huggingface.co/docs/transformers/v4.40.2/en/main_classes/tokenizer
     fn get_tokenizer_filename(&self) -> &PathBuf;
+
+    /// Jinja format chat templating for chat completion.
+    /// See: https://huggingface.co/docs/transformers/chat_templating
     fn get_template_filename(&self) -> &PathBuf;
+
+    /// Optional adapter files. `(String, PathBuf)` is of the form `(id name, path)`.
     fn get_adapter_filenames(&self) -> &Option<Vec<(String, PathBuf)>>;
-    fn get_adapter_configs(&self) -> &Option<Vec<((String, String), LoraConfig)>>; // (id name, name)
+
+    /// Configuration of optional adapters. `(String, String)` is of the form `(id name, name)`.
+    fn get_adapter_configs(&self) -> &Option<Vec<((String, String), LoraConfig)>>;
+
+    /// Filepath for the XLORA classifier
     fn get_classifier_path(&self) -> &Option<PathBuf>;
+
+    /// `XLoraConfig` for the XLORA classifier
     fn get_classifier_config(&self) -> &Option<XLoraConfig>;
+
+    /// Return the defined ordering of adapters and layers within the model.
     fn get_ordering(&self) -> &Option<Ordering>;
+
+    /// Filepath for general model configuration.
     fn get_gen_conf_filename(&self) -> Option<&PathBuf>;
+
     fn get_lora_preload_adapter_info(&self) -> &Option<HashMap<String, (PathBuf, LoraConfig)>>;
 }
 
-pub struct SimpleModelPaths<P> {
+#[derive(Clone)]
+pub struct LocalModelPaths<P> {
     tokenizer_filename: P,
     config_filename: P,
     template_filename: P,
     filenames: Vec<P>,
     xlora_adapter_filenames: Option<Vec<(String, P)>>,
     xlora_adapter_configs: Option<Vec<((String, String), LoraConfig)>>,
     classifier_path: Option<P>,
     classifier_config: Option<XLoraConfig>,
     xlora_ordering: Option<Ordering>,
     gen_conf: Option<P>,
     lora_preload_adapter_info: Option<HashMap<String, (P, LoraConfig)>>,
 }
 
-impl ModelPaths for SimpleModelPaths<PathBuf> {
+impl<P> LocalModelPaths<P> {
+    #[allow(clippy::too_many_arguments)]
+    pub fn new(
+        tokenizer_filename: P,
+        config_filename: P,
+        template_filename: P,
+        filenames: Vec<P>,
+        xlora_adapter_filenames: Option<Vec<(String, P)>>,
+        xlora_adapter_configs: Option<Vec<((String, String), LoraConfig)>>,
+        classifier_path: Option<P>,
+        classifier_config: Option<XLoraConfig>,
+        xlora_ordering: Option<Ordering>,
+        gen_conf: Option<P>,
+        lora_preload_adapter_info: Option<HashMap<String, (P, LoraConfig)>>,
+    ) -> Self {
+        Self {
+            tokenizer_filename,
+            config_filename,
+            template_filename,
+            filenames,
+            xlora_adapter_filenames,
+            xlora_adapter_configs,
+            classifier_path,
+            classifier_config,
+            xlora_ordering,
+            gen_conf,
+            lora_preload_adapter_info,
+        }
+    }
+}
+
+impl ModelPaths for LocalModelPaths<PathBuf> {
     fn get_config_filename(&self) -> &PathBuf {
         &self.config_filename
     }
     fn get_tokenizer_filename(&self) -> &PathBuf {
         &self.tokenizer_filename
     }
     fn get_weight_filenames(&self) -> &[PathBuf] {
@@ -209,39 +268,55 @@
 ///
 /// # Example
 /// ```no_run
 /// use mistralrs_core::{Loader, TokenSource, DeviceMapMetadata};
 /// use candle_core::Device;
 ///
 /// let loader: Box<dyn Loader> = todo!();
-/// let pipeline = loader.load_model(
+/// let pipeline = loader.load_model_from_hf(
 ///     None,
 ///     TokenSource::CacheToken,
 ///     None,
 ///     &Device::cuda_if_available(0).unwrap(),
 ///     false,
 ///     DeviceMapMetadata::dummy(),
 ///     None,
 /// ).unwrap();
 /// ```
 pub trait Loader {
     /// If `revision` is None, then it defaults to `main`.
     /// If `dtype` is None, then it defaults to the model default (usually BF16).
+    /// If model is not found on HF, will attempt to resolve locally.
     #[allow(clippy::type_complexity, clippy::too_many_arguments)]
-    fn load_model(
+    fn load_model_from_hf(
         &self,
         revision: Option<String>,
         token_source: TokenSource,
         dtype: Option<DType>,
         device: &Device,
         silent: bool,
         mapper: DeviceMapMetadata,
         in_situ_quant: Option<GgmlDType>,
     ) -> Result<Arc<Mutex<dyn Pipeline + Send + Sync>>>;
 
+    #[allow(
+        clippy::type_complexity,
+        clippy::too_many_arguments,
+        clippy::borrowed_box
+    )]
+    fn load_model_from_path(
+        &self,
+        paths: &Box<dyn ModelPaths>,
+        _dtype: Option<DType>,
+        device: &Device,
+        silent: bool,
+        mapper: DeviceMapMetadata,
+        in_situ_quant: Option<GgmlDType>,
+    ) -> Result<Arc<Mutex<dyn Pipeline + Send + Sync>>>;
+
     fn get_id(&self) -> String;
     fn get_kind(&self) -> ModelKind;
 }
 
 #[derive(Clone)]
 pub struct GeneralMetadata {
     pub max_seq_len: usize,
@@ -423,31 +498,14 @@
     /// It is not a guarantee that this will be called for each prompt step.
     /// This may also reset the non granular state if applicable.
     fn set_none_cache(&mut self, reset_non_granular: bool, modify_draft_cache: bool);
     fn cache(&self) -> &Cache;
     /// Returns the number of activated adapters.
     fn activate_adapters(&mut self, adapters: Vec<String>) -> Result<usize>;
 }
-
-pub trait CacheManager {
-    fn clone_in_cache(
-        &self,
-        pipeline: &mut dyn Pipeline,
-        seqs: &mut [&mut Sequence],
-        modify_draft_cache: bool,
-    );
-    fn clone_out_cache(
-        &self,
-        pipeline: &mut dyn Pipeline,
-        seqs: &mut [&mut Sequence],
-        modify_draft_cache: bool,
-    );
-    fn set_none_cache(&self, pipeline: &mut dyn Pipeline, modify_draft_cache: bool);
-}
-
 pub trait NormalModelLoader {
     fn load(
         &self,
         config: &str,
         use_flash_attn: bool,
         vb: VarBuilder,
         mapper: DeviceMapMetadata,
@@ -659,16 +717,23 @@
             .map(|_| (0..max_len).map(|x| x as i64).collect::<Vec<_>>())
             .collect::<Vec<_>>()
         {
             tmp.push(Tensor::from_slice(&pos, pos.len(), device)?.unsqueeze(0)?);
         }
     }
     let positions_kernel = Tensor::cat(&tmp, 0)?;
+    let input = Tensor::cat(&seqs_tensors, 0).unwrap();
+    // Only use matmul via f16 if prompt and seqlen > 32
+    if input.dim(1)? > 32 {
+        set_use_matmul_via_f16(true);
+    } else {
+        set_use_matmul_via_f16(false);
+    }
     Ok(InputMetadata {
-        input: Tensor::cat(&seqs_tensors, 0).unwrap(),
+        input,
         positions: seqlen_offsets,
         positions_kernel,
         context_lens,
         position_ids,
     })
 }
 
@@ -699,14 +764,15 @@
     for pos in (0..seqs_tensors.len())
         .map(|i| vec![*seqlen_offsets.get(i).unwrap() as i64])
         .collect::<Vec<_>>()
     {
         tmp.push(Tensor::from_slice(&pos, pos.len(), device)?.unsqueeze(0)?);
     }
     let positions_kernel = Tensor::cat(&tmp, 0)?;
+    set_use_matmul_via_f16(false);
     Ok(InputMetadata {
         input: Tensor::cat(&seqs_tensors, 0).unwrap(),
         positions: seqlen_offsets,
         positions_kernel,
         context_lens,
         position_ids,
     })
@@ -720,14 +786,16 @@
     seqlen_offsets_full: Option<Vec<usize>>,
     seqlen_offsets_kernel: Tensor,
     seqlen_offsets_kernel_full: Option<Tensor>,
     context_lens: Vec<(usize, usize)>,
     position_ids: Vec<usize>,
 }
 
+/// This will also enable matmul via f16 if prompt and the sequence length is greater than 32.
+/// Otherwise, matmul via f16 is disabled
 fn calculate_inputs(
     input_seqs: &[&mut Sequence],
     is_prompt: bool,
     is_xlora: bool,
     device: &Device,
     no_kv_cache: bool,
     last_n_context_len: Option<(usize, usize)>,
@@ -849,38 +917,43 @@
         let api = api.repo(Repo::with_revision(
             xlora_id.clone(),
             RepoType::Model,
             revision,
         ));
         let model_id = Path::new(&xlora_id);
 
+        // Get the path for the xlora classifier
         let xlora_classifier = &api_dir_list!(api, model_id)
             .filter(|x| x.contains("xlora_classifier.safetensors"))
             .collect::<Vec<_>>();
-        if xlora_classifier.len() != 1 {
+        if xlora_classifier.len() > 1 {
             warn!("Detected multiple X-LoRA classifiers: {xlora_classifier:?}");
             warn!("Selected classifier: `{}`", &xlora_classifier[0]);
         }
-        let xlora_classifier = &xlora_classifier[0];
+        let xlora_classifier = xlora_classifier.first();
+
+        let classifier_path =
+            xlora_classifier.map(|xlora_classifier| api_get_file!(api, xlora_classifier, model_id));
+
+        // Get the path for the xlora config by checking all for valid versions.
+        // NOTE(EricLBuehler): Remove this functionality because all configs should be deserializable
         let xlora_configs = &api_dir_list!(api, model_id)
             .filter(|x| x.contains("xlora_config.json"))
             .collect::<Vec<_>>();
-        if xlora_configs.len() != 1 {
+        if xlora_configs.len() > 1 {
             warn!("Detected multiple X-LoRA configs: {xlora_configs:?}");
         }
 
-        let classifier_path = api_get_file!(api, xlora_classifier, Path::new(""));
-
         let mut xlora_config: Option<XLoraConfig> = None;
         let mut last_err: Option<serde_json::Error> = None;
         for (i, config_path) in xlora_configs.iter().enumerate() {
             if xlora_configs.len() != 1 {
                 warn!("Selecting config: `{}`", config_path);
             }
-            let config_path = api_get_file!(api, config_path, Path::new(""));
+            let config_path = api_get_file!(api, config_path, model_id);
             let conf = fs::read_to_string(config_path)?;
             let deser: Result<XLoraConfig, serde_json::Error> = serde_json::from_str(&conf);
             match deser {
                 Ok(conf) => {
                     xlora_config = Some(conf);
                     break;
                 }
@@ -888,109 +961,125 @@
                     if i != xlora_configs.len() - 1 {
                         warn!("Config is broken with error `{e}`");
                     }
                     last_err = Some(e);
                 }
             }
         }
-        let xlora_config = xlora_config.unwrap_or_else(|| {
-            panic!(
-                "Unable to derserialize any configs. Last error: {}",
-                last_err.unwrap()
-            )
+        let xlora_config = xlora_config.map(Some).unwrap_or_else(|| {
+            if let Some(last_err) = last_err {
+                panic!(
+                    "Unable to derserialize any configs. Last error: {}",
+                    last_err
+                )
+            } else {
+                None
+            }
         });
 
+        // If there are adapters in the ordering file, get their names and remote paths
         let adapter_files = api_dir_list!(api, model_id)
             .filter_map(|name| {
-                for adapter_name in xlora_order.as_ref().unwrap().adapters.as_ref().unwrap() {
-                    if name.contains(adapter_name) {
-                        return Some((name, adapter_name.clone()));
+                if let Some(ref adapters) = xlora_order.as_ref().unwrap().adapters {
+                    for adapter_name in adapters {
+                        if name.contains(adapter_name) {
+                            return Some((name, adapter_name.clone()));
+                        }
                     }
                 }
                 None
             })
             .collect::<Vec<_>>();
-        if adapter_files.is_empty() {
+        if adapter_files.is_empty() && xlora_order.as_ref().unwrap().adapters.is_some() {
             anyhow::bail!("Adapter files are empty. Perhaps the ordering file adapters does not match the actual adapters?")
         }
+
+        // Get the local paths for each adapter
         let mut adapters_paths: HashMap<String, Vec<PathBuf>> = HashMap::new();
         for (file, name) in adapter_files {
             if let Some(paths) = adapters_paths.get_mut(&name) {
-                paths.push(api_get_file!(api, &file, Path::new("")));
+                paths.push(api_get_file!(api, &file, model_id));
             } else {
-                adapters_paths.insert(name, vec![api_get_file!(api, &file, Path::new(""))]);
+                adapters_paths.insert(name, vec![api_get_file!(api, &file, model_id)]);
             }
         }
+
+        // Sort local paths for the adapter configs and safetensors files
         let mut adapters_configs = Vec::new();
         let mut adapters_safetensors = Vec::new();
-        for (i, name) in xlora_order
-            .as_ref()
-            .unwrap()
-            .adapters
-            .as_ref()
-            .unwrap()
-            .iter()
-            .enumerate()
-        {
-            let paths = adapters_paths
-                .get(name)
-                .unwrap_or_else(|| panic!("Adapter {name} not found."));
-            for path in paths {
-                if path.extension().unwrap() == "safetensors" {
-                    adapters_safetensors.push((name.clone(), path.to_owned()));
-                } else {
-                    let conf = fs::read_to_string(path)?;
-                    let lora_config: LoraConfig = serde_json::from_str(&conf)?;
-                    adapters_configs.push((((i + 1).to_string(), name.clone()), lora_config));
+        if let Some(ref adapters) = xlora_order.as_ref().unwrap().adapters {
+            for (i, name) in adapters.iter().enumerate() {
+                let paths = adapters_paths
+                    .get(name)
+                    .unwrap_or_else(|| panic!("Adapter {name} not found."));
+                for path in paths {
+                    if path.extension().unwrap() == "safetensors" {
+                        adapters_safetensors.push((name.clone(), path.to_owned()));
+                    } else {
+                        let conf = fs::read_to_string(path)?;
+                        let lora_config: LoraConfig = serde_json::from_str(&conf)?;
+                        adapters_configs.push((((i + 1).to_string(), name.clone()), lora_config));
+                    }
                 }
             }
         }
 
-        if xlora_order
+        // Make sure they all match
+        if xlora_order.as_ref().is_some_and(|order| {
+            &order.base_model_id
+                != xlora_config
+                    .as_ref()
+                    .map(|cfg| &cfg.base_model_id)
+                    .unwrap_or(&base_model_id)
+        }) || xlora_config
             .as_ref()
-            .is_some_and(|order| order.base_model_id != xlora_config.base_model_id)
-            || xlora_config.base_model_id != base_model_id
+            .map(|cfg| &cfg.base_model_id)
+            .unwrap_or(&base_model_id)
+            != &base_model_id
         {
             anyhow::bail!(
                 "Adapter ordering file, adapter model config, and base model ID do not match: {}, {}, and {} respectively.",
                 xlora_order.as_ref().unwrap().base_model_id,
-                xlora_config.base_model_id,
+                xlora_config.map(|cfg| cfg.base_model_id).unwrap_or(base_model_id.clone()),
                 base_model_id
             );
         }
 
         let lora_preload_adapter_info = if let Some(xlora_order) = xlora_order {
+            // If preload adapters are specified, get their metadata like above
             if let Some(preload_adapters) = &xlora_order.preload_adapters {
                 let mut output = HashMap::new();
                 for adapter in preload_adapters {
+                    // Get the names and remote paths of the files associated with this adapter
                     let adapter_files = api_dir_list!(api, &adapter.adapter_model_id)
                         .filter_map(|f| {
                             if f.contains(&adapter.name) {
                                 Some((f, adapter.name.clone()))
                             } else {
                                 None
                             }
                         })
                         .collect::<Vec<_>>();
                     if adapter_files.is_empty() {
                         anyhow::bail!("Adapter files are empty. Perhaps the ordering file adapters does not match the actual adapters?")
                     }
+                    // Get local paths for this adapter
                     let mut adapters_paths: HashMap<String, Vec<PathBuf>> = HashMap::new();
                     for (file, name) in adapter_files {
                         if let Some(paths) = adapters_paths.get_mut(&name) {
-                            paths.push(api_get_file!(api, &file, Path::new("")));
+                            paths.push(api_get_file!(api, &file, model_id));
                         } else {
-                            adapters_paths
-                                .insert(name, vec![api_get_file!(api, &file, Path::new(""))]);
+                            adapters_paths.insert(name, vec![api_get_file!(api, &file, model_id)]);
                         }
                     }
 
                     let mut config = None;
                     let mut safetensor = None;
 
+                    // Sort local paths for the adapter configs and safetensors files
                     let paths = adapters_paths
                         .get(&adapter.name)
                         .unwrap_or_else(|| panic!("Adapter {} not found.", adapter.name));
                     for path in paths {
                         if path.extension().unwrap() == "safetensors" {
                             safetensor = Some(path.to_owned());
                         } else {
@@ -1010,17 +1099,17 @@
         } else {
             None
         };
 
         XLoraPaths {
             adapter_configs: Some(adapters_configs),
             adapter_safetensors: Some(adapters_safetensors),
-            classifier_path: Some(classifier_path),
+            classifier_path,
             xlora_order: xlora_order.clone(),
-            xlora_config: Some(xlora_config),
+            xlora_config,
             lora_preload_adapter_info,
         }
     } else {
         XLoraPaths {
             adapter_configs: None,
             adapter_safetensors: None,
             classifier_path: None,
@@ -1055,15 +1144,15 @@
                 let model_id = Path::new(&id);
                 Ok(vec![api_get_file!(qapi, name, model_id)])
             }
         },
         None => {
             let mut filenames = vec![];
             for rfilename in api_dir_list!(api, model_id).filter(|x| x.ends_with(".safetensors")) {
-                filenames.push(api_get_file!(api, &rfilename, Path::new("")));
+                filenames.push(api_get_file!(api, &rfilename, model_id));
             }
             Ok(filenames)
         }
     }
 }
 
 mod tests {
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/normal.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/pipeline/normal.rs`

 * *Files 3% similar despite different names*

```diff
@@ -5,30 +5,31 @@
 };
 use super::{
     get_model_paths, get_xlora_paths, CacheManager, GeneralMetadata, Loader, ModelInputs,
     ModelKind, ModelPaths, NormalModel, NormalModelLoader, Pipeline, TokenSource, XLoraPaths,
 };
 use crate::aici::bintokens::build_tok_trie;
 use crate::aici::toktree::TokTrie;
-use crate::models::Cache;
+use crate::lora::Ordering;
 use crate::pipeline::chat_template::calculate_eos_tokens;
-use crate::pipeline::{ChatTemplate, SimpleModelPaths};
+use crate::pipeline::Cache;
+use crate::pipeline::{ChatTemplate, LocalModelPaths};
 use crate::prefix_cacher::PrefixCacheManager;
 use crate::sequence::Sequence;
+use crate::utils::tokenizer::get_tokenizer;
 use crate::utils::{tokens::get_token, varbuilder_utils::from_mmaped_safetensors};
 use crate::xlora_models::NonGranularState;
 use crate::{
     deserialize_chat_template, do_sample, get_mut_arcmutex, get_paths, lora_model_loader,
     normal_model_loader, xlora_model_loader, DeviceMapMetadata,
 };
 use anyhow::Result;
 use candle_core::quantized::GgmlDType;
 use candle_core::{DType, Device, Tensor};
 use hf_hub::{api::sync::ApiBuilder, Repo, RepoType};
-use mistralrs_lora::Ordering;
 use rand_isaac::Isaac64Rng;
 use serde_json::Value;
 use std::collections::HashMap;
 use std::fs;
 use std::path::PathBuf;
 use std::str::FromStr;
 use std::sync::Arc;
@@ -166,35 +167,46 @@
             tgt_non_granular_index: self.tgt_non_granular_index,
         })
     }
 }
 
 impl Loader for NormalLoader {
     #[allow(clippy::type_complexity, clippy::too_many_arguments)]
-    fn load_model(
+    fn load_model_from_hf(
         &self,
         revision: Option<String>,
         token_source: TokenSource,
-        dtype: Option<DType>,
+        _dtype: Option<DType>,
         device: &Device,
         silent: bool,
         mapper: DeviceMapMetadata,
         in_situ_quant: Option<GgmlDType>,
     ) -> Result<Arc<Mutex<dyn Pipeline + Send + Sync>>> {
         let paths: anyhow::Result<Box<dyn ModelPaths>> = get_paths!(
-            SimpleModelPaths,
+            LocalModelPaths,
             &token_source,
             revision,
             self,
             None,
             None,
             silent
         );
-        let paths = paths?;
+        self.load_model_from_path(&paths?, _dtype, device, silent, mapper, in_situ_quant)
+    }
 
+    #[allow(clippy::type_complexity, clippy::too_many_arguments)]
+    fn load_model_from_path(
+        &self,
+        paths: &Box<dyn ModelPaths>,
+        dtype: Option<DType>,
+        device: &Device,
+        silent: bool,
+        mapper: DeviceMapMetadata,
+        in_situ_quant: Option<GgmlDType>,
+    ) -> Result<Arc<Mutex<dyn Pipeline + Send + Sync>>> {
         let config = std::fs::read_to_string(paths.get_config_filename())?;
         let default_dtype = if device.is_cuda() && mapper.is_dummy() {
             DType::BF16
         } else if !mapper.is_dummy() {
             DType::F16
         } else {
             DType::F32
@@ -264,16 +276,15 @@
             ModelKind::LoraGGML => unreachable!(),
             ModelKind::Speculative {
                 target: _,
                 draft: _,
             } => unreachable!(),
         };
 
-        let tokenizer =
-            Tokenizer::from_file(paths.get_tokenizer_filename()).map_err(anyhow::Error::msg)?;
+        let tokenizer = get_tokenizer(paths.get_tokenizer_filename())?;
 
         let (chat_template, gen_conf) = deserialize_chat_template!(paths, self);
 
         if let Some(in_situ_quant) = in_situ_quant {
             model.quantize(in_situ_quant, device.clone())?;
         }
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/sampling.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/pipeline/sampling.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/sampling_pipeline.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/pipeline/sampling_pipeline.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/pipeline/speculative.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/pipeline/speculative.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,73 +1,108 @@
 use std::{
     iter::zip,
     sync::{Arc, Mutex},
 };
 
-use candle_core::{quantized::GgmlDType, Device, IndexOp, Result, Tensor};
+use anyhow::Result as anyhowResult;
+use candle_core::{quantized::GgmlDType, DType, Device, IndexOp, Result, Tensor};
 use rand_isaac::Isaac64Rng;
 use tokenizers::Tokenizer;
 
 use crate::{
     finish_and_add_tokens_to_seq, get_mut_arcmutex,
-    models::Cache,
     pipeline::{
         sampling::{sample_sequence, sample_target_sequence_speculative},
-        AdapterInstruction,
+        AdapterInstruction, Cache,
     },
     prefix_cacher::PrefixCacheManager,
     sequence::{Sequence, SequenceRecognizer},
     DeviceMapMetadata, Loader, ModelKind, Pipeline, TokenSource,
 };
 
 use super::{
     cache_manager::DefaultCacheManager, calculate_inputs, chat_template::ChatTemplate,
     sampling::SpeculativeSample, CacheInstruction, CacheManager, GeneralMetadata, ModelInputs,
+    ModelPaths,
 };
 
 pub struct SpeculativeLoader {
     pub target: Box<dyn Loader>,
     pub draft: Box<dyn Loader>,
     pub config: SpeculativeConfig,
 }
 
 impl Loader for SpeculativeLoader {
-    fn load_model(
+    #[allow(clippy::type_complexity, clippy::too_many_arguments)]
+    fn load_model_from_hf(
         &self,
         revision: Option<String>,
         token_source: TokenSource,
-        dtype: Option<candle_core::DType>,
+        dtype: Option<DType>,
         device: &Device,
         silent: bool,
         mapper: DeviceMapMetadata,
         in_situ_quant: Option<GgmlDType>,
-    ) -> anyhow::Result<Arc<tokio::sync::Mutex<dyn Pipeline + Send + Sync>>> {
-        let target = self.target.load_model(
+    ) -> anyhowResult<Arc<tokio::sync::Mutex<dyn Pipeline + Send + Sync>>> {
+        let target = self.target.load_model_from_hf(
             revision.clone(),
             token_source.clone(),
             dtype,
             device,
             silent,
             mapper.clone(),
             in_situ_quant,
         )?;
-        let draft = self.draft.load_model(
+        let draft = self.draft.load_model_from_hf(
             revision,
             token_source,
             dtype,
             device,
             silent,
             mapper,
             in_situ_quant,
         )?;
         Ok(Arc::new(tokio::sync::Mutex::new(SpeculativePipeline::new(
             target,
             draft,
             self.config,
         )?)))
+    }
+
+    #[allow(clippy::type_complexity, clippy::too_many_arguments)]
+    fn load_model_from_path(
+        &self,
+        paths: &Box<dyn ModelPaths>,
+        dtype: Option<DType>,
+        device: &Device,
+        silent: bool,
+        mapper: DeviceMapMetadata,
+        in_situ_quant: Option<GgmlDType>,
+    ) -> anyhowResult<Arc<tokio::sync::Mutex<dyn Pipeline + Send + Sync>>> {
+        let target = self.target.load_model_from_path(
+            paths,
+            dtype,
+            device,
+            silent,
+            mapper.clone(),
+            in_situ_quant,
+        )?;
+        let draft = self.draft.load_model_from_path(
+            paths,
+            dtype,
+            device,
+            silent,
+            mapper.clone(),
+            in_situ_quant,
+        )?;
+        Ok(Arc::new(tokio::sync::Mutex::new(SpeculativePipeline::new(
+            target,
+            draft,
+            self.config,
+        )?)))
     }
     fn get_id(&self) -> String {
         format!(
             "Speculative: tgt = `{}`, draft = `{}`, gamma = `{}`",
             self.target.get_id(),
             self.draft.get_id(),
             self.config.gamma,
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/prefix_cacher.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/prefix_cacher.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use std::sync::{Arc, Mutex};
 
 use candle_core::{Device, Result, Tensor};
 use radix_trie::{Trie, TrieCommon, TrieKey};
 
-use crate::{get_mut_arcmutex, models::LayerCaches, sequence::Sequence};
+use crate::{get_mut_arcmutex, pipeline::LayerCaches, sequence::Sequence};
 
 #[derive(PartialEq, Eq)]
 struct Tokens(Vec<u32>);
 
 impl TrieKey for Tokens {
     fn encode_bytes(&self) -> Vec<u8> {
         self.0
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/request.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/request.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/sampler.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/sampler.rs`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 use std::{
     collections::HashMap,
     iter::zip,
     sync::{Arc, Mutex},
 };
 
 use candle_core::{bail, Device, Error, Result, Tensor, D};
+#[cfg(feature = "pyo3_macros")]
 use pyo3::pyclass;
+
 use rand::distributions::{Distribution, WeightedIndex};
 use rand_isaac::Isaac64Rng;
 use serde::{Deserialize, Serialize};
 use tokenizers::Tokenizer;
 
 #[derive(Clone, Debug)]
 /// Stop sequences or ids.
@@ -61,16 +63,16 @@
     frequency_penalty: Option<f32>,
     presence_penalty: Option<f32>,
     logits_bias: Option<Tensor>,
     topk: i64,
     topp: f64,
 }
 
-#[pyclass]
-#[pyo3(get_all)]
+#[cfg_attr(feature = "pyo3_macros", pyclass)]
+#[cfg_attr(feature = "pyo3_macros", pyo3(get_all))]
 #[derive(Debug, Clone, Serialize, Deserialize, PartialEq)]
 // Top-n logprobs element
 pub struct TopLogprob {
     pub token: u32,
     pub logprob: f32,
     pub bytes: String,
 }
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/scheduler.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/scheduler.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/sequence.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/sequence.rs`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 use crate::{
     aici::{cfg::CfgParser, recognizer::StackRecognizer, rx::RecRx},
     response::CompletionChoice,
     CompletionResponse,
 };
 use crate::{
     get_mut_group,
-    models::LayerCaches,
+    pipeline::LayerCaches,
     response::{ChatCompletionChunkResponse, Choice, ChunkChoice, Response, SYSTEM_FINGERPRINT},
     sampler::{Logprobs, Sampler},
     ChatCompletionResponse, Usage,
 };
 use candle_core::Tensor;
 use regex_automata::util::primitives::StateID;
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/toml_selector.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/toml_selector.rs`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     },
 
     /// Select a LoRA architecture
     Lora {
         /// Force a base model ID to load from instead of using the ordering file. This may be a HF hub repo or a local path.
         model_id: Option<String>,
 
-        /// Model ID to load X-LoRA from. This may be a HF hub repo or a local path.
+        /// Model ID to load LoRA from. This may be a HF hub repo or a local path.
         adapters_model_id: String,
 
         /// Ordering JSON file
         order: String,
 
         /// The architecture of the model.
         arch: NormalLoaderType,
@@ -107,15 +107,15 @@
         /// Quantized model ID to find the `quantized_filename`, only applicable if `quantized` is set.
         /// This may be a HF hub repo or a local path.
         quantized_model_id: String,
 
         /// Quantized filename, only applicable if `quantized` is set.
         quantized_filename: String,
 
-        /// Model ID to load X-LoRA from. This may be a HF hub repo or a local path.
+        /// Model ID to load LoRA from. This may be a HF hub repo or a local path.
         adapters_model_id: String,
 
         /// Ordering JSON file
         order: String,
     },
 
     /// Select a GGML model.
@@ -171,15 +171,15 @@
         /// Quantized model ID to find the `quantized_filename`, only applicable if `quantized` is set.
         /// This may be a HF hub repo or a local path.
         quantized_model_id: String,
 
         /// Quantized filename, only applicable if `quantized` is set.
         quantized_filename: String,
 
-        /// Model ID to load X-LoRA from. This may be a HF hub repo or a local path.
+        /// Model ID to load LoRA from. This may be a HF hub repo or a local path.
         adapters_model_id: String,
 
         /// Ordering JSON file
         order: String,
 
         /// GQA value
         #[serde(default = "default_one")]
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/utils/mod.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/utils/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+pub(crate) mod tokenizer;
 pub(crate) mod tokens;
 pub(crate) mod varbuilder_utils;
 
 #[macro_export]
 macro_rules! get_mut_arcmutex {
     ($thing:expr) => {
         loop {
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/utils/tokens.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/utils/tokens.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/utils/varbuilder_utils.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/utils/varbuilder_utils.rs`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 use candle_core::{DType, Device, Result, Tensor};
 use candle_nn::{
     var_builder::{SimpleBackend, VarBuilderArgs},
     VarBuilder,
 };
 
-use mistralrs_lora::LoraConfig;
+use crate::lora::LoraConfig;
 use tqdm::Iter;
 
 /// Load tensors into a VarBuilder backed by a VarMap using MmapedSafetensors.
 /// Set `silent` to not show a progress bar.
 pub(crate) fn from_mmaped_safetensors<'a>(
     paths: Vec<PathBuf>,
     xlora_paths: Vec<PathBuf>,
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/classifier.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/classifier.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/config.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/config.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/gemma.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/gemma.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
 use std::{collections::HashMap, sync::Arc};
 
+use crate::{
+    layers::MatMul,
+    lora::{linear_b as linear, LinearLayerLike, LoraConfig, Ordering},
+};
 use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor, D};
 use candle_nn::{RotaryEmbedding, VarBuilder};
-use mistralrs_lora::{layer::QLinear, linear_b as linear, LinearLayerLike, LoraConfig, Ordering};
 use tqdm::Iter;
 use tracing::info;
 
 use crate::{
     device_map::DeviceMapper,
-    layers::CausalMasker,
-    models::{flash_attn, gemma::Config, repeat_kv, Cache},
-    pipeline::{extract_logits, NormalModel},
+    layers::{flash_attn, repeat_kv, CausalMasker, QLinear},
+    models::gemma::Config,
+    pipeline::{extract_logits, Cache, NormalModel},
     DeviceMapMetadata,
 };
 
 use super::{classifier::XLoraClassifier, NonGranularState, ScalingsMaker, XLoraConfig};
 
 fn default_max_position_embeddings() -> usize {
     4096
@@ -310,42 +313,37 @@
                 .contiguous()?;
             k = k
                 .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
                 .transpose(1, 2)?
                 .contiguous()?;
         }
 
-        let (k, v) = match &*kv_cache {
-            None => (k, v),
-            Some((prev_k, prev_v)) => {
-                let k = candle_nn::ops::kvconcat(prev_k, &k, 2)?;
-                let v = candle_nn::ops::kvconcat(prev_v, &v, 2)?;
-                (k, v)
-            }
-        };
-        *kv_cache = Some((k.clone(), v.clone()));
+        let (k, v) = Cache::update_kv_cache(kv_cache, k, v, false)?;
 
         let k = repeat_kv(k, self.num_kv_groups)?.contiguous()?;
         let v = repeat_kv(v, self.num_kv_groups)?.contiguous()?;
 
         let mut attn_output = if self.use_flash_attn {
             // flash-attn expects (b_sz, seq_len, nheads, head_dim)
             let q = q.transpose(1, 2)?;
             let k = k.transpose(1, 2)?;
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
-            let scale = 1f64 / f64::sqrt(self.head_dim as f64);
-            let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
+            let attn_weights = MatMul.matmul_affine_div(
+                &q,
+                &k.transpose(2, 3)?,
+                f64::sqrt(self.head_dim as f64),
+            )?;
 
             let attn_weights =
                 CausalMasker.apply_mask(&attention_mask.cloned(), attn_weights, &self.neg_inf)?;
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
-            attn_weights.matmul(&v)?
+            MatMul.matmul(&attn_weights, &v)?
         };
         if self.q_proj.is_quant() {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
         let mut res = self.o_proj.lora_forward(
             &attn_output.transpose(1, 2)?.reshape((b_sz, q_len, ()))?,
             scalings.clone(),
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/llama.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/llama.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
+use crate::{
+    layers::MatMul,
+    lora::{linear_no_bias as linear, LinearLayerLike, LoraConfig, Ordering},
+};
 use candle_core::{quantized::QMatMul, DType, Device, Result, Tensor, D};
 use candle_nn::{embedding, Embedding, Module, RotaryEmbedding, VarBuilder};
-use mistralrs_lora::{
-    layer::QLinear, linear_no_bias as linear, LinearLayerLike, LoraConfig, Ordering,
-};
 use std::{collections::HashMap, sync::Arc};
 use tqdm::Iter;
 use tracing::info;
 
 use crate::{
     device_map::DeviceMapper,
-    layers::{CausalMasker, RmsNorm},
-    models::{self, flash_attn, llama::Config, repeat_kv, LayerCaches},
-    pipeline::{extract_logits, NormalModel},
+    layers::{flash_attn, repeat_kv, CausalMasker, QLinear, RmsNorm},
+    models::llama::Config,
+    pipeline::{self, extract_logits, LayerCaches, NormalModel},
     DeviceMapMetadata,
 };
 
 use super::{classifier::XLoraClassifier, NonGranularState, ScalingsMaker, XLoraConfig};
 
 #[derive(Debug, Clone)]
 struct CausalSelfAttention {
@@ -77,15 +78,15 @@
             q = q.to_dtype(original_dtype)?;
             k = k.to_dtype(original_dtype)?;
             v = v.to_dtype(original_dtype)?;
         }
 
         let mut q = q.reshape((b_sz * seq_len, self.num_attention_heads, self.head_dim))?;
         let mut k = k.reshape((b_sz * seq_len, self.num_key_value_heads, self.head_dim))?;
-        let mut v = v
+        let v = v
             .reshape((b_sz, seq_len, self.num_key_value_heads, self.head_dim))?
             .transpose(1, 2)?;
 
         self.rotary_emb
             .forward(seqlen_offsets, &start_offsets_kernel, &mut q, &mut k, b_sz)?;
 
         if q.rank() == 3 {
@@ -95,52 +96,33 @@
                 .contiguous()?;
             k = k
                 .reshape((b_sz, seq_len, self.num_key_value_heads, self.head_dim))?
                 .transpose(1, 2)?
                 .contiguous()?;
         }
 
-        if let Some((cache_k, cache_v)) = &kv_cache[block_idx] {
-            k = candle_nn::ops::kvconcat(cache_k, &k, 2)?.contiguous()?;
-            v = candle_nn::ops::kvconcat(cache_v, &v, 2)?.contiguous()?;
-            let k_seq_len = k.dims()[1];
-            if k_seq_len > self.max_seq_len {
-                k = k
-                    .narrow(D::Minus1, k_seq_len - self.max_seq_len, self.max_seq_len)?
-                    .contiguous()?
-            }
-            let v_seq_len = v.dims()[1];
-            if v_seq_len > 2 * self.max_seq_len {
-                v = v
-                    .narrow(D::Minus1, v_seq_len - self.max_seq_len, self.max_seq_len)?
-                    .contiguous()?
-            }
-        }
-        kv_cache[block_idx] = Some((k.clone(), v.clone()));
+        let (k, v) =
+            crate::pipeline::Cache::update_kv_cache(&mut kv_cache[block_idx], k, v, false)?;
 
         let k = repeat_kv(k, self.num_attention_heads / self.num_key_value_heads)?.contiguous()?;
         let v = repeat_kv(v, self.num_attention_heads / self.num_key_value_heads)?.contiguous()?;
 
         let y = if self.use_flash_attn {
             // flash-attn expects (b_sz, seq_len, nheads, head_dim)
             let q = q.transpose(1, 2)?;
             let k = k.transpose(1, 2)?;
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, seq_len > 1)?.transpose(1, 2)?
         } else {
-            let in_dtype = q.dtype();
-            let q = q.to_dtype(DType::F32)?;
-            let k = k.to_dtype(DType::F32)?;
-            let v = v.to_dtype(DType::F32)?;
-            let att = (q.matmul(&k.t()?)? / (self.head_dim as f64).sqrt())?;
+            let att = MatMul.matmul_affine_div(&q, &k.t()?, (self.head_dim as f64).sqrt())?;
             let att = CausalMasker.apply_mask(mask, att, &self.neg_inf)?;
             let att = candle_nn::ops::softmax(&att, D::Minus1)?;
             // Convert to contiguous as matmul doesn't support strided vs for now.
-            att.matmul(&v.contiguous()?)?.to_dtype(in_dtype)?
+            MatMul.matmul(&att, &v.contiguous()?)?
         };
         let mut y = y.transpose(1, 2)?.reshape(&[b_sz, seq_len, hidden_size])?;
         if self.q_proj.is_quant() {
             y = y.to_dtype(DType::F32)?;
         }
         let mut res = self.o_proj.lora_forward(
             &y.transpose(1, 2)?.reshape((b_sz, seq_len, ()))?,
@@ -422,15 +404,15 @@
 }
 
 pub struct XLoraLlama {
     wte: Embedding,
     blocks: Vec<Block>,
     ln_f: RmsNorm,
     lm_head: QLinear,
-    pub kv_cache: models::Cache,
+    pub kv_cache: pipeline::Cache,
     pub device: Device,
     xlora_classifier: Option<XLoraClassifier>,
     dtype: DType,
     mapper: Box<dyn DeviceMapper + Send + Sync>,
 }
 
 impl XLoraLlama {
@@ -650,15 +632,15 @@
         }
 
         Ok(Self {
             wte,
             blocks,
             ln_f,
             lm_head: QLinear::from_linear(lm_head),
-            kv_cache: models::Cache::new(cfg.num_hidden_layers, true),
+            kv_cache: pipeline::Cache::new(cfg.num_hidden_layers, true),
             device: real_device,
             xlora_classifier: xlora_config.map(|xlora_config| {
                 XLoraClassifier::new(xlora_config, count, lora_config.len(), vb, false).unwrap()
             }),
             dtype,
             mapper,
         })
@@ -772,15 +754,15 @@
     }
 }
 
 impl ScalingsMaker for XLoraLlama {
     fn dtype(&self) -> DType {
         self.dtype
     }
-    fn get_cache(&self) -> &models::Cache {
+    fn get_cache(&self) -> &pipeline::Cache {
         &self.kv_cache
     }
     fn get_classifier(&self) -> &XLoraClassifier {
         self.xlora_classifier.as_ref().unwrap()
     }
     fn forward(
         &mut self,
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/mistral.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/mistral.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
+use crate::{
+    layers::MatMul,
+    lora::{linear_no_bias, LinearLayerLike, LoraConfig, Ordering},
+};
 /// Mistral LLM, https://github.com/mistralai/mistral-src
-use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor, D};
+use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor};
 use candle_nn::{Activation, RotaryEmbedding, VarBuilder};
-use mistralrs_lora::{layer::QLinear, linear_no_bias, LinearLayerLike, LoraConfig, Ordering};
 use std::{collections::HashMap, sync::Arc};
 use tqdm::Iter;
 use tracing::info;
 
 use crate::{
     device_map::DeviceMapper,
-    layers::{CausalMasker, RmsNorm},
-    models::{flash_attn, mistral::Config, repeat_kv, Cache},
-    pipeline::{extract_logits, NormalModel},
+    layers::{flash_attn, repeat_kv, CausalMasker, QLinear, RmsNorm},
+    models::mistral::Config,
+    pipeline::{extract_logits, Cache, NormalModel},
     DeviceMapMetadata,
 };
 
 use super::{classifier::XLoraClassifier, config::XLoraConfig, NonGranularState, ScalingsMaker};
 
 #[derive(Debug, Clone)]
 #[allow(clippy::upper_case_acronyms)]
@@ -270,69 +273,43 @@
                 .contiguous()?;
             k = k
                 .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
                 .transpose(1, 2)?
                 .contiguous()?;
         }
 
-        let (k, v, attn_mask) = match kv_cache.clone() {
-            None => (k, v, attention_mask.cloned()),
-            Some((mut prev_k, mut prev_v)) => {
-                let mut mask = attention_mask.cloned();
-                if let Some(sliding_window) = self.sliding_window {
-                    let kv_seq_len = prev_k.dim(2)?;
-                    if kv_seq_len > sliding_window {
-                        prev_k = prev_k.narrow(
-                            2,
-                            kv_seq_len - (sliding_window - 1),
-                            sliding_window - 1,
-                        )?;
-                        prev_v = prev_v.narrow(
-                            2,
-                            kv_seq_len - (sliding_window - 1),
-                            sliding_window - 1,
-                        )?;
-                        if let Some(ref mut mask) = mask {
-                            let mask_len = mask.dim(1)?;
-                            *mask = mask.narrow(
-                                1,
-                                mask_len - (sliding_window - 1),
-                                sliding_window - 1,
-                            )?;
-                            *mask = Tensor::cat(
-                                &[&*mask, &mask.narrow(1, mask_len - 1, 1)?.ones_like()?],
-                                D::Minus1,
-                            )?;
-                        }
-                    }
-                }
-                let k = candle_nn::ops::kvconcat(&prev_k, &k, 2)?;
-                let v = candle_nn::ops::kvconcat(&prev_v, &v, 2)?;
-                (k, v, mask)
-            }
-        };
-        *kv_cache = Some((k.clone(), v.clone()));
+        let (k, v, attn_mask) = Cache::update_kv_cache_sliding_window(
+            kv_cache,
+            k,
+            v,
+            attention_mask,
+            self.sliding_window,
+            false,
+        )?;
 
         let k = repeat_kv(k, self.num_kv_groups)?.contiguous()?;
         let v = repeat_kv(v, self.num_kv_groups)?.contiguous()?;
 
         let mut attn_output = if self.use_flash_attn {
             // flash-attn expects (b_sz, seq_len, nheads, head_dim)
             let q = q.transpose(1, 2)?;
             let k = k.transpose(1, 2)?;
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
-            let scale = 1f64 / f64::sqrt(self.head_dim as f64);
-            let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
+            let attn_weights = MatMul.matmul_affine_div(
+                &q,
+                &k.transpose(2, 3)?,
+                f64::sqrt(self.head_dim as f64),
+            )?;
 
             let attn_weights = CausalMasker.apply_mask(&attn_mask, attn_weights, &self.neg_inf)?;
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
-            attn_weights.matmul(&v)?
+            MatMul.matmul(&attn_weights, &v)?
         };
         if self.q_proj.is_quant() {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
         let mut res = self.o_proj.lora_forward(
             &attn_output.transpose(1, 2)?.reshape((b_sz, q_len, ()))?,
             scalings.clone(),
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/mixtral.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/mixtral.rs`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
+use crate::{
+    layers::MatMul,
+    lora::{linear_no_bias, LinearLayerLike, LoraConfig, Ordering},
+};
 /// Mixtral Model
 /// https://github.com/huggingface/transformers/blob/main/src/transformers/models/mixtral/modeling_mixtral.py
 /// https://mistral.ai/news/mixtral-of-experts/
-use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor, D};
+use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor};
 use candle_nn::{Activation, RotaryEmbedding, VarBuilder};
-use mistralrs_lora::{linear_no_bias, LinearLayerLike, LoraConfig, Ordering};
 use std::{collections::HashMap, sync::Arc};
 use tqdm::Iter;
 use tracing::info;
 
 use crate::{
     device_map::DeviceMapper,
-    layers::{CausalMasker, RmsNorm},
-    models::{flash_attn, mixtral::Config, repeat_kv, Cache},
-    pipeline::{extract_logits, NormalModel},
+    layers::{flash_attn, repeat_kv, CausalMasker, RmsNorm},
+    models::mixtral::Config,
+    pipeline::{extract_logits, Cache, NormalModel},
     DeviceMapMetadata,
 };
 
 use super::{classifier::XLoraClassifier, NonGranularState, ScalingsMaker, XLoraConfig};
 
 #[derive(Debug, Clone)]
 struct Attention {
@@ -170,69 +173,43 @@
                 .contiguous()?;
             k = k
                 .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
                 .transpose(1, 2)?
                 .contiguous()?;
         }
 
-        let (k, v, attn_mask) = match kv_cache.clone() {
-            None => (k, v, attention_mask.cloned()),
-            Some((mut prev_k, mut prev_v)) => {
-                let mut mask = attention_mask.cloned();
-                if let Some(sliding_window) = self.sliding_window {
-                    let kv_seq_len = prev_k.dim(2)?;
-                    if kv_seq_len > sliding_window {
-                        prev_k = prev_k.narrow(
-                            2,
-                            kv_seq_len - (sliding_window - 1),
-                            sliding_window - 1,
-                        )?;
-                        prev_v = prev_v.narrow(
-                            2,
-                            kv_seq_len - (sliding_window - 1),
-                            sliding_window - 1,
-                        )?;
-                        if let Some(ref mut mask) = mask {
-                            let mask_len = mask.dim(1)?;
-                            *mask = mask.narrow(
-                                1,
-                                mask_len - (sliding_window - 1),
-                                sliding_window - 1,
-                            )?;
-                            *mask = Tensor::cat(
-                                &[&*mask, &mask.narrow(1, mask_len - 1, 1)?.ones_like()?],
-                                D::Minus1,
-                            )?;
-                        }
-                    }
-                }
-                let k = candle_nn::ops::kvconcat(&prev_k, &k, 2)?;
-                let v = candle_nn::ops::kvconcat(&prev_v, &v, 2)?;
-                (k, v, mask)
-            }
-        };
-        *kv_cache = Some((k.clone(), v.clone()));
+        let (k, v, attn_mask) = Cache::update_kv_cache_sliding_window(
+            kv_cache,
+            k,
+            v,
+            attention_mask,
+            self.sliding_window,
+            false,
+        )?;
 
         let k = repeat_kv(k, self.num_kv_groups)?.contiguous()?;
         let v = repeat_kv(v, self.num_kv_groups)?.contiguous()?;
 
         let mut attn_output = if self.use_flash_attn {
             // flash-attn expects (b_sz, seq_len, nheads, head_dim)
             let q = q.transpose(1, 2)?;
             let k = k.transpose(1, 2)?;
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
-            let scale = 1f64 / f64::sqrt(self.head_dim as f64);
-            let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
+            let attn_weights = MatMul.matmul_affine_div(
+                &q,
+                &k.transpose(2, 3)?,
+                f64::sqrt(self.head_dim as f64),
+            )?;
 
             let attn_weights = CausalMasker.apply_mask(&attn_mask, attn_weights, &self.neg_inf)?;
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
-            attn_weights.matmul(&v)?
+            MatMul.matmul(&attn_weights, &v)?
         };
         if self.q_proj.is_quant() {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
         let mut res = self.o_proj.lora_forward(
             &attn_output.transpose(1, 2)?.reshape((b_sz, q_len, ()))?,
             scalings.clone(),
@@ -789,15 +766,15 @@
                         no_kv_cache,
                         None,
                     )?
                     .contiguous()?;
                 if matches!(self.lm_head, QMatMul::QTensor(_)) {
                     res = res.to_dtype(DType::F32)?;
                 }
-                extract_logits(&res.apply(&self.lm_head)?, context_lens)
+                extract_logits(&MatMul.qmatmul(&res, &self.lm_head)?, context_lens)
             } else {
                 // is_full_pass=true is ok because no_kv_cache=false
                 let mut res = self
                     .inner_forward(
                         input_ids,
                         seqlen_offsets,
                         start_offsets_kernel,
@@ -806,15 +783,15 @@
                         no_kv_cache,
                         None,
                     )?
                     .contiguous()?;
                 if matches!(self.lm_head, QMatMul::QTensor(_)) {
                     res = res.to_dtype(DType::F32)?;
                 }
-                extract_logits(&res.apply(&self.lm_head)?, context_lens)
+                extract_logits(&MatMul.qmatmul(&res, &self.lm_head)?, context_lens)
             }
         } else {
             let mut res = self
                 .inner_forward(
                     input_ids,
                     seqlen_offsets,
                     start_offsets_kernel,
@@ -823,15 +800,15 @@
                     no_kv_cache,
                     None,
                 )?
                 .contiguous()?;
             if matches!(self.lm_head, QMatMul::QTensor(_)) {
                 res = res.to_dtype(DType::F32)?;
             }
-            extract_logits(&res.apply(&self.lm_head)?, context_lens)
+            extract_logits(&MatMul.qmatmul(&res, &self.lm_head)?, context_lens)
         }
     }
 }
 
 impl NormalModel for XLoraModel {
     fn forward(
         &mut self,
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/mod.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/mod.rs`

 * *Files 12% similar despite different names*

```diff
@@ -7,28 +7,28 @@
 mod phi2;
 mod phi3;
 mod quantized_llama;
 mod quantized_phi3;
 
 use std::sync::Arc;
 
+use crate::lora::Ordering;
 use candle_core::{DType, Device, Result, Tensor};
-pub use config::XLoraConfig;
-pub use gemma::XLoraModel as XLoraGemma;
-pub use llama::XLoraLlama;
-pub use mistral::XLoraModel as XLoraMistral;
-use mistralrs_lora::Ordering;
-pub use mixtral::XLoraModel as XLoraMixtral;
-pub use phi2::Model as XLoraPhi2;
-pub use phi3::Model as XLoraPhi3;
-pub use quantized_llama::ModelWeights as XLoraQLlama;
-pub use quantized_phi3::ModelWeights as XLoraQPhi3;
+pub(crate) use config::XLoraConfig;
+pub(crate) use gemma::XLoraModel as XLoraGemma;
+pub(crate) use llama::XLoraLlama;
+pub(crate) use mistral::XLoraModel as XLoraMistral;
+pub(crate) use mixtral::XLoraModel as XLoraMixtral;
+pub(crate) use phi2::Model as XLoraPhi2;
+pub(crate) use phi3::Model as XLoraPhi3;
+pub(crate) use quantized_llama::ModelWeights as XLoraQLlama;
+pub(crate) use quantized_phi3::ModelWeights as XLoraQPhi3;
 use tokio::sync::Mutex;
 
-use crate::{get_mut_arcmutex, models::Cache};
+use crate::{get_mut_arcmutex, pipeline::Cache};
 
 use self::classifier::XLoraClassifier;
 
 pub struct NonGranularState {
     pub non_granular_index: Arc<Mutex<usize>>,
     pub tgt_non_granular_index: usize,
 }
@@ -127,14 +127,17 @@
             }
         }
         Ok(scalings)
     }
 }
 
 fn verify_sanity_adapters(ordering: &Ordering, supported_layers: &[&str]) -> Result<()> {
-    for path in ordering.layers.keys() {
+    if ordering.layers.is_none() {
+        return Ok(());
+    }
+    for path in ordering.layers.as_ref().unwrap().keys() {
         if !supported_layers.iter().any(|layer| path.ends_with(layer)) {
             candle_core::bail!("Got a layer name `{path}` in the ordering, expected it to end with one of {supported_layers:?}");
         }
     }
     Ok(())
 }
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/phi2.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/phi2.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
 use std::{collections::HashMap, sync::Arc};
 
+use crate::{
+    layers::MatMul,
+    lora::{linear, LinearLayerLike, LoraConfig, Ordering},
+};
 /// Phi model.
 /// https://huggingface.co/microsoft/phi-2
 /// There is an alternative implementation of the phi model in mixformers.rs.
 /// This corresponds to the model update made with the following commit:
 /// https://huggingface.co/microsoft/phi-2/commit/cb2f4533604d8b67de604e7df03bfe6f3ca22869
 use candle_core::{quantized::QMatMul, DType, Device, Result, Tensor};
 use candle_nn::{
     embedding, layer_norm, Activation, Embedding, LayerNorm, RotaryEmbedding, VarBuilder,
 };
-use mistralrs_lora::{layer::QLinear, linear, LinearLayerLike, LoraConfig, Ordering};
 use tqdm::Iter;
 use tracing::info;
 
 use crate::{
     device_map::DeviceMapper,
-    layers::CausalMasker,
-    models::{flash_attn, phi2::Config, repeat_kv},
+    layers::{flash_attn, repeat_kv, CausalMasker, QLinear},
+    models::phi2::Config,
     pipeline::{extract_logits, NormalModel},
     DeviceMapMetadata,
 };
 
 use super::{classifier::XLoraClassifier, Cache, NonGranularState, ScalingsMaker, XLoraConfig};
 
 #[derive(Debug, Clone)]
@@ -185,15 +188,15 @@
         let (q_layernorm, k_layernorm) = if cfg.qk_layernorm {
             let q_layernorm = layer_norm(head_dim, cfg.layer_norm_eps, vb.pp("q_layernorm"))?;
             let k_layernorm = layer_norm(head_dim, cfg.layer_norm_eps, vb.pp("k_layernorm"))?;
             (Some(q_layernorm), Some(k_layernorm))
         } else {
             (None, None)
         };
-        let softmax_scale = 1f64 / (head_dim as f64).sqrt();
+        let softmax_scale = (head_dim as f64).sqrt();
         Ok(Self {
             q_proj,
             k_proj,
             v_proj,
             dense,
             q_layernorm,
             k_layernorm,
@@ -279,44 +282,33 @@
                 .contiguous()?;
             k = k
                 .reshape((b_size, seq_len, self.num_kv_heads, self.head_dim))?
                 .transpose(1, 2)?
                 .contiguous()?;
         }
 
-        let (k, v) = match &*kv_cache {
-            None => (k, v),
-            Some((prev_k, prev_v)) => {
-                let k = candle_nn::ops::kvconcat(prev_k, &k, 2)?;
-                let v = candle_nn::ops::kvconcat(prev_v, &v, 2)?;
-                (k, v)
-            }
-        };
-        *kv_cache = Some((k.clone(), v.clone()));
+        let (k, v) = Cache::update_kv_cache(kv_cache, k, v, false)?;
 
         let k = repeat_kv(k, self.num_heads / self.num_kv_heads)?.contiguous()?;
         let v = repeat_kv(v, self.num_heads / self.num_kv_heads)?.contiguous()?;
 
         let attn_output = if self.use_flash_attn {
             // flash-attn expects (b_sz, seq_len, nheads, head_dim)
             let q = q.transpose(1, 2)?;
             let k = k.transpose(1, 2)?;
             let v = v.transpose(1, 2)?;
             flash_attn(&q, &k, &v, self.softmax_scale as f32, seq_len > 1)?.transpose(1, 2)?
         } else {
-            let attn_weights = (q
-                .to_dtype(DType::F32)?
-                .contiguous()?
-                .matmul(&k.to_dtype(DType::F32)?.t()?)?
-                * self.softmax_scale)?;
+            let attn_weights =
+                MatMul.matmul_affine_div(&q.contiguous()?, &k.t()?, self.softmax_scale)?;
             let attn_weights =
                 CausalMasker.apply_mask(&mask.cloned(), attn_weights, &self.neg_inf)?;
             let attn_weights =
                 candle_nn::ops::softmax_last_dim(&attn_weights)?.to_dtype(v.dtype())?;
-            attn_weights.matmul(&v)?
+            MatMul.matmul(&attn_weights, &v)?
         };
 
         let mut attn_output = attn_output
             .transpose(1, 2)?
             .reshape((b_size, seq_len, ()))?;
         if self.q_proj.is_quant() {
             attn_output = attn_output.to_dtype(DType::F32)?;
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/phi3.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/phi3.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
 // This implementation is based on:
 // https://huggingface.co/microsoft/Phi-3-mini-4k-instruct/blob/main/modeling_phi3.py
+use crate::{
+    layers::MatMul,
+    lora::{linear_no_bias, LinearLayerLike, LoraConfig, Ordering},
+};
 use candle_core::{quantized::QMatMul, DType, Device, Module, Result, Tensor, D};
 use candle_nn::VarBuilder;
-use mistralrs_lora::{layer::QLinear, linear_no_bias, LinearLayerLike, LoraConfig, Ordering};
 use std::{collections::HashMap, sync::Arc};
 use tqdm::Iter;
 use tracing::info;
 
 use crate::{
     device_map::DeviceMapper,
-    layers::{CausalMasker, PhiRotaryEmbedding, RmsNorm},
+    layers::{flash_attn, repeat_kv, CausalMasker, PhiRotaryEmbedding, QLinear, RmsNorm},
     models::phi3::Config,
     pipeline::{extract_logits, NormalModel},
     DeviceMapMetadata,
 };
 
-use crate::models::{flash_attn, repeat_kv, Cache};
+use crate::pipeline::Cache;
 
 use super::{classifier::XLoraClassifier, NonGranularState, ScalingsMaker, XLoraConfig};
 
 #[derive(Debug, Clone)]
 struct Attention {
     qkv_proj: Arc<dyn LinearLayerLike + Send + Sync>,
     o_proj: Arc<dyn LinearLayerLike + Send + Sync>,
@@ -134,69 +137,43 @@
             .reshape((b_sz, q_len, self.num_kv_heads, self.head_dim))?
             .transpose(1, 2)?;
 
         let (q, k) = self
             .rotary_emb
             .forward(&q, &k, seqlen_offsets, position_ids)?;
 
-        let (k, v, attn_mask) = match kv_cache.clone() {
-            None => (k, v, attention_mask.cloned()),
-            Some((mut prev_k, mut prev_v)) => {
-                let mut mask = attention_mask.cloned();
-                if let Some(sliding_window) = self.sliding_window {
-                    let kv_seq_len = prev_k.dim(2)?;
-                    if kv_seq_len > sliding_window {
-                        prev_k = prev_k.narrow(
-                            2,
-                            kv_seq_len - (sliding_window - 1),
-                            sliding_window - 1,
-                        )?;
-                        prev_v = prev_v.narrow(
-                            2,
-                            kv_seq_len - (sliding_window - 1),
-                            sliding_window - 1,
-                        )?;
-                        if let Some(ref mut mask) = mask {
-                            let mask_len = mask.dim(1)?;
-                            *mask = mask.narrow(
-                                1,
-                                mask_len - (sliding_window - 1),
-                                sliding_window - 1,
-                            )?;
-                            *mask = Tensor::cat(
-                                &[&*mask, &mask.narrow(1, mask_len - 1, 1)?.ones_like()?],
-                                D::Minus1,
-                            )?;
-                        }
-                    }
-                }
-                let k = Tensor::cat(&[prev_k, k], 2)?;
-                let v = Tensor::cat(&[prev_v, v], 2)?;
-                (k, v, mask)
-            }
-        };
-        *kv_cache = Some((k.clone(), v.clone()));
+        let (k, v, attn_mask) = Cache::update_kv_cache_sliding_window(
+            kv_cache,
+            k,
+            v,
+            attention_mask,
+            self.sliding_window,
+            true,
+        )?;
 
         let k = repeat_kv(k, self.num_kv_groups)?.contiguous()?;
         let v = repeat_kv(v, self.num_kv_groups)?.contiguous()?;
 
         let mut attn_output = if self.use_flash_attn {
             // flash-attn expects (b_sz, seq_len, nheads, head_dim)
             let q = q.transpose(1, 2)?;
             let k = k.transpose(1, 2)?;
             let v = v.transpose(1, 2)?;
             let softmax_scale = 1f32 / (self.head_dim as f32).sqrt();
             flash_attn(&q, &k, &v, softmax_scale, q_len > 1)?.transpose(1, 2)?
         } else {
-            let scale = 1f64 / f64::sqrt(self.head_dim as f64);
-            let attn_weights = (q.matmul(&k.transpose(2, 3)?)? * scale)?;
+            let attn_weights = MatMul.matmul_affine_div(
+                &q,
+                &k.transpose(2, 3)?,
+                f64::sqrt(self.head_dim as f64),
+            )?;
 
             let attn_weights = CausalMasker.apply_mask(&attn_mask, attn_weights, &self.neg_inf)?;
             let attn_weights = candle_nn::ops::softmax_last_dim(&attn_weights)?;
-            attn_weights.matmul(&v)?
+            MatMul.matmul(&attn_weights, &v)?
         };
         if self.qkv_proj.is_quant() {
             attn_output = attn_output.to_dtype(DType::F32)?;
         }
         let mut res = self.o_proj.lora_forward(
             &attn_output.transpose(1, 2)?.reshape((b_sz, q_len, ()))?,
             scalings.clone(),
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/quantized_llama.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/quantized_llama.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
 use std::collections::HashMap;
 
+use crate::lora::{
+    get_lora_cfg, AdapterSwapper, LinearLayerLike, LoraConfig, Merge, Ordering, QLoraLinear,
+};
 use candle_core::quantized::QMatMul;
 use candle_core::quantized::{ggml_file, gguf_file};
 use candle_core::{DType, Device, Result, Tensor};
 use candle_nn::{Embedding, Module, RotaryEmbedding, VarBuilder};
-use mistralrs_lora::{
-    get_lora_cfg, AdapterSwapper, LinearLayerLike, LoraConfig, Merge, Ordering, QLoraLinear,
-};
 use tqdm::Iter;
 use tracing::info;
 
 use crate::device_map::DeviceMapper;
-use crate::layers::{CausalMasker, QRmsNorm};
-use crate::models::{repeat_kv, verify_sanity_gguf, Cache};
-use crate::pipeline::extract_logits;
+use crate::layers::{repeat_kv, verify_sanity_gguf, CausalMasker, MatMul, QRmsNorm};
+use crate::pipeline::{extract_logits, Cache};
 use crate::DeviceMapMetadata;
 
 use super::classifier::XLoraClassifier;
 use super::{verify_sanity_adapters, NonGranularState, ScalingsMaker, XLoraConfig};
 
 const MAX_SEQ_LEN: u32 = 4096;
 const SUPPORTED_LAYERS: [&str; 7] = [
@@ -90,15 +89,15 @@
             Self::MoE {
                 feed_forward_gate_inp,
                 experts,
                 n_expert_used,
             } => {
                 let (b_size, seq_len, hidden_dim) = xs.dims3()?;
                 let xs = xs.reshape(((), hidden_dim))?;
-                let router_logits = feed_forward_gate_inp.forward(&xs)?;
+                let router_logits = MatMul.qmatmul(&xs, feed_forward_gate_inp)?;
                 let routing_weights = candle_nn::ops::softmax_last_dim(&router_logits)?;
 
                 // In order to extract topk, we extract the data from the tensor and manipulate it
                 // directly. Maybe we will want to use some custom ops instead at some point.
                 let routing_weights = routing_weights.to_dtype(DType::F32)?.to_vec2::<f32>()?;
 
                 // routing_weights, selected_experts = torch.topk(routing_weights, self.top_k, dim=-1)
@@ -225,32 +224,28 @@
                 .transpose(1, 2)?
                 .contiguous()?;
             k = k
                 .reshape((b_sz, seq_len, self.n_kv_head, self.head_dim))?
                 .transpose(1, 2)?;
         }
 
-        let (k, v) = match &*kv_cache {
-            None => (k, v),
-            Some((k_cache, v_cache)) => {
-                let k = candle_nn::ops::kvconcat(k_cache, &k, 2)?.contiguous()?;
-                let v = candle_nn::ops::kvconcat(v_cache, &v, 2)?.contiguous()?;
-                (k, v)
-            }
-        };
-        *kv_cache = Some((k.clone(), v.clone()));
+        let (k, v) = Cache::update_kv_cache(kv_cache, k, v, false)?;
 
         let k = repeat_kv(k, self.n_head / self.n_kv_head)?.contiguous()?;
         let v = repeat_kv(v, self.n_head / self.n_kv_head)?.contiguous()?;
 
-        let att = (q.contiguous()?.matmul(&k.t()?.contiguous()?)? / (self.head_dim as f64).sqrt())?;
+        let att = MatMul.matmul_affine_div(
+            &q.contiguous()?,
+            &k.t()?.contiguous()?,
+            (self.head_dim as f64).sqrt(),
+        )?;
         let att = CausalMasker.apply_mask(mask, att, &self.neg_inf)?;
         let att = candle_nn::ops::softmax_last_dim(&att)?;
         // Convert to contiguous as matmul doesn't support strided vs for now.
-        let y = att.matmul(&v.contiguous()?)?;
+        let y = MatMul.matmul(&att, &v.contiguous()?)?;
         let y = y.transpose(1, 2)?.reshape(&[b_sz, seq_len, n_embd])?;
         let y = self.attention_wo.lora_forward(
             &y,
             scalings.clone(),
             global_scaling_weight,
             is_scaling_pass,
         )?;
@@ -836,60 +831,66 @@
                 no_kv_cache,
                 non_granular_state,
                 &vec![usize::MAX; context_lens.len()],
             )?;
 
             if no_kv_cache {
                 extract_logits(
-                    &self
-                        .inner_forward(
-                            input_ids_full,
-                            seqlen_offsets_full,
-                            start_offsets_kernel_full,
-                            Some(scalings),
-                            true,
-                            no_kv_cache,
-                            None,
-                        )?
-                        .contiguous()?
-                        .apply(&self.output)?,
+                    &MatMul.qmatmul(
+                        &self
+                            .inner_forward(
+                                input_ids_full,
+                                seqlen_offsets_full,
+                                start_offsets_kernel_full,
+                                Some(scalings),
+                                true,
+                                no_kv_cache,
+                                None,
+                            )?
+                            .contiguous()?,
+                        &self.output,
+                    )?,
                     context_lens,
                 )
             } else {
                 // is_full_pass=true is ok because no_kv_cache=false
                 extract_logits(
+                    &MatMul.qmatmul(
+                        &self
+                            .inner_forward(
+                                input_ids,
+                                seqlen_offsets,
+                                start_offsets_kernel,
+                                Some(scalings),
+                                true,
+                                no_kv_cache,
+                                None,
+                            )?
+                            .contiguous()?,
+                        &self.output,
+                    )?,
+                    context_lens,
+                )
+            }
+        } else {
+            extract_logits(
+                &MatMul.qmatmul(
                     &self
                         .inner_forward(
                             input_ids,
                             seqlen_offsets,
                             start_offsets_kernel,
-                            Some(scalings),
-                            true,
+                            None,
+                            false,
                             no_kv_cache,
                             None,
                         )?
-                        .contiguous()?
-                        .apply(&self.output)?,
-                    context_lens,
-                )
-            }
-        } else {
-            extract_logits(
-                &self
-                    .inner_forward(
-                        input_ids,
-                        seqlen_offsets,
-                        start_offsets_kernel,
-                        None,
-                        false,
-                        no_kv_cache,
-                        None,
-                    )?
-                    .contiguous()?
-                    .apply(&self.output)?,
+                        .contiguous()?,
+                    &self.output,
+                )?,
                 context_lens,
             )
         }
     }
 }
 
 impl ScalingsMaker for ModelWeights {
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-core/src/xlora_models/quantized_phi3.rs` & `mistralrs_mkl-0.1.8/mistralrs-core/src/xlora_models/quantized_phi3.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 #![allow(clippy::cast_possible_truncation, clippy::cast_precision_loss)]
 
 use std::collections::HashMap;
 
 use crate::device_map::DeviceMapper;
+use crate::layers::repeat_kv;
+use crate::layers::verify_sanity_gguf;
 use crate::layers::CausalMasker;
+use crate::layers::MatMul;
 use crate::layers::RmsNorm;
-use crate::models::repeat_kv;
-use crate::models::verify_sanity_gguf;
+use crate::lora::get_lora_cfg;
+use crate::lora::AdapterSwapper;
+use crate::lora::LinearLayerLike;
+use crate::lora::LoraConfig;
+use crate::lora::Merge;
+use crate::lora::Ordering;
+use crate::lora::QLoraLinear;
 use crate::pipeline::extract_logits;
 use crate::DeviceMapMetadata;
 use candle_core::quantized::gguf_file;
 use candle_core::quantized::QMatMul;
 use candle_core::quantized::QTensor;
 use candle_core::{DType, Device, IndexOp, Module, Result, Tensor, D};
 use candle_nn::Embedding;
 use candle_nn::VarBuilder;
-use mistralrs_lora::get_lora_cfg;
-use mistralrs_lora::AdapterSwapper;
-use mistralrs_lora::LinearLayerLike;
-use mistralrs_lora::LoraConfig;
-use mistralrs_lora::Merge;
-use mistralrs_lora::Ordering;
-use mistralrs_lora::QLoraLinear;
 use tqdm::Iter;
 use tracing::info;
 
 use super::classifier::XLoraClassifier;
 use super::verify_sanity_adapters;
 use super::Cache;
 use super::NonGranularState;
@@ -143,50 +144,31 @@
         let v = v
             .reshape((b_sz, seq_len, self.n_kv_head, self.head_dim))?
             .transpose(1, 2)?;
 
         let q = self.apply_rotary_emb(&q, seqlen_offsets)?.contiguous()?;
         let k = self.apply_rotary_emb(&k, seqlen_offsets)?;
 
-        let (k, v, attn_mask) = match kv_cache.clone() {
-            None => (k, v, mask.cloned()),
-            Some((mut prev_k, mut prev_v)) => {
-                let mut mask = mask.cloned();
-                let kv_seq_len = prev_k.dim(2)?;
-                let sliding_window = self.sliding_window;
-                if kv_seq_len > sliding_window {
-                    prev_k =
-                        prev_k.narrow(2, kv_seq_len - (sliding_window - 1), sliding_window - 1)?;
-                    prev_v =
-                        prev_v.narrow(2, kv_seq_len - (sliding_window - 1), sliding_window - 1)?;
-                    if let Some(ref mut mask) = mask {
-                        let mask_len = mask.dim(1)?;
-                        *mask =
-                            mask.narrow(1, mask_len - (sliding_window - 1), sliding_window - 1)?;
-                        *mask = Tensor::cat(
-                            &[&*mask, &mask.narrow(1, mask_len - 1, 1)?.ones_like()?],
-                            D::Minus1,
-                        )?;
-                    }
-                }
-                let k = Tensor::cat(&[prev_k, k], 2)?;
-                let v = Tensor::cat(&[prev_v, v], 2)?;
-                (k, v, mask)
-            }
-        };
-        *kv_cache = Some((k.clone(), v.clone()));
+        let (k, v, attn_mask) = Cache::update_kv_cache_sliding_window(
+            kv_cache,
+            k,
+            v,
+            mask,
+            Some(self.sliding_window),
+            true,
+        )?;
 
         let k = repeat_kv(k, self.n_head / self.n_kv_head)?;
         let v = repeat_kv(v, self.n_head / self.n_kv_head)?;
 
-        let att = (q.matmul(&k.t()?)? / (self.head_dim as f64).sqrt())?;
+        let att = MatMul.matmul_affine_div(&q, &k.t()?, (self.head_dim as f64).sqrt())?;
         let att = CausalMasker.apply_mask(&attn_mask, att, &self.neg_inf)?;
         let att = candle_nn::ops::softmax_last_dim(&att)?;
         // Convert to contiguous as matmul doesn't support strided vs for now.
-        let y = att.matmul(&v.contiguous()?)?;
+        let y = MatMul.matmul(&att, &v.contiguous()?)?;
         let y = y.transpose(1, 2)?.reshape(&[b_sz, seq_len, n_embd])?;
         let y =
             self.attn_output
                 .lora_forward(&y, scalings, global_scaling_weight, is_scaling_pass)?;
         Ok(y)
     }
 }
@@ -466,50 +448,56 @@
                 no_kv_cache,
                 non_granular_state,
                 &vec![usize::MAX; context_lens.len()],
             )?;
 
             if no_kv_cache {
                 extract_logits(
-                    &self
-                        .inner_forward(
-                            input_ids_full,
-                            seqlen_offsets_full,
-                            Some(scalings),
-                            true,
-                            no_kv_cache,
-                            None,
-                        )?
-                        .contiguous()?
-                        .apply(&self.output)?,
+                    &MatMul.qmatmul(
+                        &self
+                            .inner_forward(
+                                input_ids_full,
+                                seqlen_offsets_full,
+                                Some(scalings),
+                                true,
+                                no_kv_cache,
+                                None,
+                            )?
+                            .contiguous()?,
+                        &self.output,
+                    )?,
                     context_lens,
                 )
             } else {
                 // is_full_pass=true is ok because no_kv_cache=false
                 extract_logits(
-                    &self
-                        .inner_forward(
-                            input_ids,
-                            seqlen_offsets,
-                            Some(scalings),
-                            true,
-                            no_kv_cache,
-                            None,
-                        )?
-                        .contiguous()?
-                        .apply(&self.output)?,
+                    &MatMul.qmatmul(
+                        &self
+                            .inner_forward(
+                                input_ids,
+                                seqlen_offsets,
+                                Some(scalings),
+                                true,
+                                no_kv_cache,
+                                None,
+                            )?
+                            .contiguous()?,
+                        &self.output,
+                    )?,
                     context_lens,
                 )
             }
         } else {
             extract_logits(
-                &self
-                    .inner_forward(input_ids, seqlen_offsets, None, false, no_kv_cache, None)?
-                    .contiguous()?
-                    .apply(&self.output)?,
+                &MatMul.qmatmul(
+                    &self
+                        .inner_forward(input_ids, seqlen_offsets, None, false, no_kv_cache, None)?
+                        .contiguous()?,
+                    &self.output,
+                )?,
                 context_lens,
             )
         }
     }
 }
 
 impl ScalingsMaker for ModelWeights {
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-pyo3/Cargo.toml` & `mistralrs_mkl-0.1.8/mistralrs-pyo3/Cargo.toml`

 * *Files 20% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [lib]
 name = "mistralrs"
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 pyo3.workspace = true
-mistralrs-core = { version = "0.1.7", path = "../mistralrs-core", features=["mkl"] }
+mistralrs-core = { version = "0.1.8", path = "../mistralrs-core", features=["pyo3_macros","mkl"] }
 serde.workspace = true
 serde_json.workspace = true
 candle-core = { git = "https://github.com/EricLBuehler/candle.git", version = "0.5.0", features=["mkl"] }
 indexmap.workspace = true
 accelerate-src = { workspace = true, optional = true }
 intel-mkl-src = { workspace = true, optional = true }
 either.workspace = true
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-pyo3/.gitignore` & `mistralrs_mkl-0.1.8/mistralrs-pyo3/.gitignore`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-pyo3/API.md` & `mistralrs_mkl-0.1.8/mistralrs-pyo3/API.md`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-pyo3/Cargo_template.toml` & `mistralrs_mkl-0.1.8/mistralrs-pyo3/Cargo_template.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 [lib]
 name = "mistralrs"
 crate-type = ["cdylib"]
 doc = false
 
 [dependencies]
 pyo3.workspace = true
-mistralrs-core = { version = "0.1.7", path = "../mistralrs-core", features=["$feature_name"] }
+mistralrs-core = { version = "0.1.8", path = "../mistralrs-core", features=["pyo3_macros","$feature_name"] }
 serde.workspace = true
 serde_json.workspace = true
 candle-core = { git = "https://github.com/EricLBuehler/candle.git", version = "0.5.0", features=["$feature_name"] }
 indexmap.workspace = true
 accelerate-src = { workspace = true, optional = true }
 intel-mkl-src = { workspace = true, optional = true }
 either.workspace = true
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-pyo3/README.md` & `mistralrs_mkl-0.1.8/mistralrs-pyo3/README.md`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-pyo3/mistralrs.pyi` & `mistralrs_mkl-0.1.8/mistralrs-pyo3/mistralrs.pyi`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-pyo3/pyproject_template.toml` & `mistralrs_mkl-0.1.8/mistralrs-pyo3/pyproject_template.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin==1.4"]
 build-backend = "maturin"
 
 [project]
 name = "$name"
-version = "0.1.7"
+version = "0.1.8"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-pyo3/src/lib.rs` & `mistralrs_mkl-0.1.8/mistralrs-pyo3/src/lib.rs`

 * *Files 0% similar despite different names*

```diff
@@ -393,15 +393,15 @@
         let device = get_device().map_err(|e| PyValueError::new_err(e.to_string()))?;
         let isq = if let Some(isq) = in_situ_quant {
             Some(parse_isq(&isq).map_err(|e| PyValueError::new_err(e.to_string()))?)
         } else {
             None
         };
         let pipeline = loader
-            .load_model(
+            .load_model_from_hf(
                 None,
                 TokenSource::from_str(token_source)
                     .map_err(|e| PyValueError::new_err(e.to_string()))?,
                 None,
                 &device,
                 true, // Silent for jupyter
                 num_device_layers
```

### Comparing `mistralrs_mkl-0.1.7/mistralrs-pyo3/src/stream.rs` & `mistralrs_mkl-0.1.8/mistralrs-pyo3/src/stream.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-pyo3/src/which.rs` & `mistralrs_mkl-0.1.8/mistralrs-pyo3/src/which.rs`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/mistralrs-pyo3/upload.py` & `mistralrs_mkl-0.1.8/mistralrs-pyo3/upload.py`

 * *Files identical despite different names*

### Comparing `mistralrs_mkl-0.1.7/Cargo.lock` & `mistralrs_mkl-0.1.8/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -333,15 +333,15 @@
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "candle-core"
 version = "0.5.1"
-source = "git+https://github.com/EricLBuehler/candle.git#afb0dedaff363f6ae8f7a5c952690653e74051fd"
+source = "git+https://github.com/EricLBuehler/candle.git#4e82faba497bfb88ff52099334f2604bd6dcd3af"
 dependencies = [
  "accelerate-src",
  "byteorder",
  "candle-kernels",
  "candle-metal-kernels",
  "cudarc",
  "gemm",
@@ -360,26 +360,26 @@
  "yoke",
  "zip 1.2.3",
 ]
 
 [[package]]
 name = "candle-flash-attn"
 version = "0.5.1"
-source = "git+https://github.com/EricLBuehler/candle.git#afb0dedaff363f6ae8f7a5c952690653e74051fd"
+source = "git+https://github.com/EricLBuehler/candle.git#4e82faba497bfb88ff52099334f2604bd6dcd3af"
 dependencies = [
  "anyhow",
  "bindgen_cuda",
  "candle-core",
  "half",
 ]
 
 [[package]]
 name = "candle-kernels"
 version = "0.5.1"
-source = "git+https://github.com/EricLBuehler/candle.git#afb0dedaff363f6ae8f7a5c952690653e74051fd"
+source = "git+https://github.com/EricLBuehler/candle.git#4e82faba497bfb88ff52099334f2604bd6dcd3af"
 dependencies = [
  "bindgen_cuda",
 ]
 
 [[package]]
 name = "candle-layer-norm"
 version = "0.0.1"
@@ -391,26 +391,26 @@
  "num_cpus",
  "rayon",
 ]
 
 [[package]]
 name = "candle-metal-kernels"
 version = "0.5.1"
-source = "git+https://github.com/EricLBuehler/candle.git#afb0dedaff363f6ae8f7a5c952690653e74051fd"
+source = "git+https://github.com/EricLBuehler/candle.git#4e82faba497bfb88ff52099334f2604bd6dcd3af"
 dependencies = [
  "metal",
  "once_cell",
  "thiserror",
  "tracing",
 ]
 
 [[package]]
 name = "candle-nn"
 version = "0.5.1"
-source = "git+https://github.com/EricLBuehler/candle.git#afb0dedaff363f6ae8f7a5c952690653e74051fd"
+source = "git+https://github.com/EricLBuehler/candle.git#4e82faba497bfb88ff52099334f2604bd6dcd3af"
 dependencies = [
  "accelerate-src",
  "candle-core",
  "candle-layer-norm",
  "candle-metal-kernels",
  "half",
  "intel-mkl-src",
@@ -421,15 +421,15 @@
  "serde",
  "thiserror",
 ]
 
 [[package]]
 name = "candle-transformers"
 version = "0.5.1"
-source = "git+https://github.com/EricLBuehler/candle.git#afb0dedaff363f6ae8f7a5c952690653e74051fd"
+source = "git+https://github.com/EricLBuehler/candle.git#4e82faba497bfb88ff52099334f2604bd6dcd3af"
 dependencies = [
  "accelerate-src",
  "byteorder",
  "candle-core",
  "candle-flash-attn",
  "candle-nn",
  "fancy-regex",
@@ -753,20 +753,20 @@
 dependencies = [
  "darling_core 0.14.4",
  "darling_macro 0.14.4",
 ]
 
 [[package]]
 name = "darling"
-version = "0.20.8"
+version = "0.20.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54e36fcd13ed84ffdfda6f5be89b31287cbb80c439841fe69e04841435464391"
+checksum = "83b2eb4d90d12bdda5ed17de686c2acb4c57914f8f921b8da7e112b5a36f3fe1"
 dependencies = [
- "darling_core 0.20.8",
- "darling_macro 0.20.8",
+ "darling_core 0.20.9",
+ "darling_macro 0.20.9",
 ]
 
 [[package]]
 name = "darling_core"
 version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "109c1ca6e6b7f82cc233a97004ea8ed7ca123a9af07a8230878fcfda9b158bf0"
@@ -777,23 +777,23 @@
  "quote",
  "strsim 0.10.0",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "darling_core"
-version = "0.20.8"
+version = "0.20.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9c2cf1c23a687a1feeb728783b993c4e1ad83d99f351801977dd809b48d0a70f"
+checksum = "622687fe0bac72a04e5599029151f5796111b90f1baaa9b544d807a5e31cd120"
 dependencies = [
  "fnv",
  "ident_case",
  "proc-macro2",
  "quote",
- "strsim 0.10.0",
+ "strsim 0.11.1",
  "syn 2.0.63",
 ]
 
 [[package]]
 name = "darling_macro"
 version = "0.14.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -802,19 +802,19 @@
  "darling_core 0.14.4",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "darling_macro"
-version = "0.20.8"
+version = "0.20.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a668eda54683121533a393014d8692171709ff57a7d61f187b6e782719f8933f"
+checksum = "733cabb43482b1a1b53eee8583c2b9e8684d592215ea83efd305dd31bc2f0178"
 dependencies = [
- "darling_core 0.20.8",
+ "darling_core 0.20.9",
  "quote",
  "syn 2.0.63",
 ]
 
 [[package]]
 name = "defmac"
 version = "0.1.3"
@@ -864,15 +864,15 @@
 
 [[package]]
 name = "derive_builder_core"
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d48cda787f839151732d396ac69e3473923d54312c070ee21e9effcaa8ca0b1d"
 dependencies = [
- "darling 0.20.8",
+ "darling 0.20.9",
  "proc-macro2",
  "quote",
  "syn 2.0.63",
 ]
 
 [[package]]
 name = "derive_builder_macro"
@@ -1876,26 +1876,26 @@
  "log",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "mistralrs"
-version = "0.1.7"
+version = "0.1.8"
 dependencies = [
  "anyhow",
  "candle-core",
  "mistralrs-core",
  "serde_json",
  "tokio",
 ]
 
 [[package]]
 name = "mistralrs-bench"
-version = "0.1.7"
+version = "0.1.8"
 dependencies = [
  "anyhow",
  "candle-core",
  "clap",
  "cli-table",
  "either",
  "mistralrs-core",
@@ -1904,40 +1904,38 @@
  "tokio",
  "tracing",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "mistralrs-core"
-version = "0.1.7"
+version = "0.1.8"
 dependencies = [
  "accelerate-src",
  "anyhow",
  "async-trait",
  "bytemuck",
  "candle-core",
  "candle-flash-attn",
  "candle-nn",
  "candle-transformers",
  "cfgrammar",
  "chrono",
  "clap",
- "ctrlc",
  "dirs",
  "either",
  "futures",
  "galil-seiferas",
  "half",
  "hf-hub",
  "indexmap",
  "indicatif",
  "intel-mkl-src",
  "lrtable",
  "minijinja",
- "mistralrs-lora",
  "once_cell",
  "pyo3",
  "radix_trie",
  "rand",
  "rand_isaac",
  "range-checked",
  "rayon",
@@ -1952,29 +1950,16 @@
  "toml",
  "tqdm",
  "tracing",
  "vob",
 ]
 
 [[package]]
-name = "mistralrs-lora"
-version = "0.1.7"
-dependencies = [
- "accelerate-src",
- "candle-core",
- "candle-nn",
- "either",
- "intel-mkl-src",
- "serde",
- "serde_json",
-]
-
-[[package]]
 name = "mistralrs-pyo3"
-version = "0.1.7"
+version = "0.1.8"
 dependencies = [
  "accelerate-src",
  "candle-core",
  "either",
  "futures",
  "indexmap",
  "intel-mkl-src",
@@ -1985,27 +1970,29 @@
  "serde_json",
  "tokio",
  "tracing-subscriber",
 ]
 
 [[package]]
 name = "mistralrs-server"
-version = "0.1.7"
+version = "0.1.8"
 dependencies = [
  "accelerate-src",
  "anyhow",
  "axum",
  "candle-core",
  "clap",
+ "ctrlc",
  "dyn-fmt",
  "either",
  "futures",
  "indexmap",
  "intel-mkl-src",
  "mistralrs-core",
+ "once_cell",
  "serde",
  "serde_json",
  "tokio",
  "tower-http",
  "tracing",
  "tracing-subscriber",
  "utoipa",
@@ -2472,17 +2459,17 @@
 checksum = "8ad3d49ab951a01fbaafe34f2ec74122942fe18a3f9814c3268f1bb72042131b"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pulp"
-version = "0.18.10"
+version = "0.18.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e14989307e408d9f4245d4fda09a7b144a08114ba124e26cab60ab83dc98db10"
+checksum = "140dfe6dada20716bd5f7284406747c73061a56a0a5d4ad5aee7957c5f71606c"
 dependencies = [
  "bytemuck",
  "libm",
  "num-complex",
  "reborrow",
 ]
 
@@ -2864,28 +2851,28 @@
 name = "rustls-pki-types"
 version = "1.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "976295e77ce332211c0d24d92c0e83e50f5c5f046d11082cea19f3df13a3562d"
 
 [[package]]
 name = "rustls-webpki"
-version = "0.102.3"
+version = "0.102.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f3bce581c0dd41bce533ce695a1437fa16a7ab5ac3ccfa99fe1a620a7885eabf"
+checksum = "ff448f7e92e913c4b7d4c6d8e4540a1724b319b4152b8aef6d4cf8339712b33e"
 dependencies = [
  "ring",
  "rustls-pki-types",
  "untrusted",
 ]
 
 [[package]]
 name = "rustversion"
-version = "1.0.16"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "092474d1a01ea8278f69e6a358998405fae5b8b963ddaeb2b0b04a128bf1dfb0"
+checksum = "955d28af4278de8121b7ebeb796b6a45735dc01436d898801014aced2773a3d6"
 
 [[package]]
 name = "ryu"
 version = "1.0.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f3cb5ba0dc43242ce17de99c180e96db90b235b8a9fdc9543c96d2209116bd9f"
 
@@ -2956,26 +2943,26 @@
 name = "seq-macro"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
 [[package]]
 name = "serde"
-version = "1.0.201"
+version = "1.0.202"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "780f1cebed1629e4753a1a38a3c72d30b97ec044f0aef68cb26650a3c5cf363c"
+checksum = "226b61a0d411b2ba5ff6d7f73a476ac4f8bb900373459cd00fab8512828ba395"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.201"
+version = "1.0.202"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5e405930b9796f1c00bee880d03fc7e0bb4b9a11afc776885ffe84320da2865"
+checksum = "6048858004bcff69094cd972ed40a32500f153bd3be9f716b2eed2e8217c4838"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.63",
 ]
 
 [[package]]
@@ -3006,17 +2993,17 @@
 checksum = "9ce1fc6db65a611022b23a0dec6975d63fb80a302cb3388835ff02c097258d50"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_spanned"
-version = "0.6.5"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb3622f419d1296904700073ea6cc23ad690adbd66f13ea683df73298736f0c1"
+checksum = "79e674e01f999af37c49f70a6ede167a8a60b2503e56c5599532a65baa5969a0"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_urlencoded"
 version = "0.7.1"
@@ -3377,38 +3364,38 @@
 dependencies = [
  "rayon",
  "tokio",
 ]
 
 [[package]]
 name = "toml"
-version = "0.8.12"
+version = "0.8.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e9dd1545e8208b4a5af1aa9bbd0b4cf7e9ea08fabc5d0a5c67fcaafa17433aa3"
+checksum = "a4e43f8cc456c9704c851ae29c67e17ef65d2c30017c17a9765b89c382dc8bba"
 dependencies = [
  "serde",
  "serde_spanned",
  "toml_datetime",
  "toml_edit",
 ]
 
 [[package]]
 name = "toml_datetime"
-version = "0.6.5"
+version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
+checksum = "4badfd56924ae69bcc9039335b2e017639ce3f9b001c393c1b2d1ef846ce2cbf"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml_edit"
-version = "0.22.12"
+version = "0.22.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d3328d4f68a705b2a4498da1d580585d39a6510f98318a2cec3018a7ec61ddef"
+checksum = "c127785850e8c20836d49732ae6abfa47616e60bf9d9f57c43c250361a9db96c"
 dependencies = [
  "indexmap",
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
```

### Comparing `mistralrs_mkl-0.1.7/Cargo.toml` & `mistralrs_mkl-0.1.8/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
-members = ["mistralrs-core", "mistralrs-lora", "mistralrs-pyo3"]
+members = ["mistralrs-core", "mistralrs-pyo3"]
 resolver = "2"
 
 [workspace.package]
-version = "0.1.7"
+version = "0.1.8"
 edition = "2021"
 description = "Fast and easy LLM serving."
 homepage = "https://github.com/EricLBuehler/mistral.rs"
 repository = "https://github.com/EricLBuehler/mistral.rs"
 keywords = ["machine-learning"]
 categories = ["science"]
 license = "MIT"
@@ -24,14 +24,15 @@
 intel-mkl-src = { version = "0.8.1", features = ["mkl-static-lp64-iomp"] }
 tracing = "0.1.40"
 tracing-subscriber = { version = "0.3.18", features = ["env-filter"] }
 futures = "0.3"
 clap = { version = "4.5.1", features = ["derive"] }
 pyo3 = { version = "0.21.0", features = ["full", "extension-module"] }
 tokio = { version = "1.36.0", features = ["full", "rt-multi-thread"] }
+once_cell = "1.19.0"
 
 [profile.profiling]
 inherits = "release"
 debug = true
 
 [profile.dev]
 opt-level = 3
```

### Comparing `mistralrs_mkl-0.1.7/pyproject.toml` & `mistralrs_mkl-0.1.8/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin==1.4"]
 build-backend = "maturin"
 
 [project]
 name = "mistralrs-mkl"
-version = "0.1.7"
+version = "0.1.8"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.8",
```

### Comparing `mistralrs_mkl-0.1.7/PKG-INFO` & `mistralrs_mkl-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mistralrs-mkl
-Version: 0.1.7
+Version: 0.1.8
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Rust
 Summary: Fast and easy LLM serving.
```

