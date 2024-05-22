# Comparing `tmp/llm2vec-0.1.7.tar.gz` & `tmp/llm2vec-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm2vec-0.1.7.tar", last modified: Mon May 20 19:52:11 2024, max compression
+gzip compressed data, was "llm2vec-0.1.8.tar", last modified: Wed May 22 19:22:56 2024, max compression
```

## Comparing `llm2vec-0.1.7.tar` & `llm2vec-0.1.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-20 19:52:11.350339 llm2vec-0.1.7/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1067 2024-04-08 21:09:47.000000 llm2vec-0.1.7/LICENSE
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    14785 2024-05-20 19:52:11.350859 llm2vec-0.1.7/PKG-INFO
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    14335 2024-05-20 19:39:21.000000 llm2vec-0.1.7/README.md
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-20 19:52:11.328401 llm2vec-0.1.7/llm2vec/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       29 2024-04-16 16:56:44.000000 llm2vec-0.1.7/llm2vec/__init__.py
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-20 19:52:11.339303 llm2vec-0.1.7/llm2vec/dataset/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     6148 2024-05-08 16:25:06.000000 llm2vec-0.1.7/llm2vec/dataset/E5Data.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1368 2024-05-20 19:39:21.000000 llm2vec-0.1.7/llm2vec/dataset/Wiki1M.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       53 2024-05-20 19:39:21.000000 llm2vec-0.1.7/llm2vec/dataset/__init__.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1137 2024-05-20 19:39:21.000000 llm2vec-0.1.7/llm2vec/dataset/dataset.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      778 2024-05-20 19:39:21.000000 llm2vec-0.1.7/llm2vec/dataset/utils.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     2417 2024-04-30 22:31:54.000000 llm2vec-0.1.7/llm2vec/experiment_utils.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    16796 2024-05-20 19:39:21.000000 llm2vec-0.1.7/llm2vec/llm2vec.py
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-20 19:52:11.343390 llm2vec-0.1.7/llm2vec/loss/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1478 2024-04-30 22:31:54.000000 llm2vec-0.1.7/llm2vec/loss/HardNegativeNLLLoss.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       52 2024-04-30 22:31:54.000000 llm2vec-0.1.7/llm2vec/loss/__init__.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     3080 2024-04-30 22:31:54.000000 llm2vec-0.1.7/llm2vec/loss/loss_utils.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      289 2024-04-30 22:31:54.000000 llm2vec-0.1.7/llm2vec/loss/utils.py
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-20 19:52:11.348430 llm2vec-0.1.7/llm2vec/models/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      130 2024-04-16 16:56:44.000000 llm2vec-0.1.7/llm2vec/models/__init__.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7620 2024-04-16 16:56:44.000000 llm2vec-0.1.7/llm2vec/models/attn_mask_utils.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7774 2024-05-20 19:39:21.000000 llm2vec-0.1.7/llm2vec/models/bidirectional_llama.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    10368 2024-04-17 17:32:47.000000 llm2vec-0.1.7/llm2vec/models/bidirectional_mistral.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       22 2024-05-20 19:51:17.000000 llm2vec-0.1.7/llm2vec/version.py
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-20 19:52:11.333543 llm2vec-0.1.7/llm2vec.egg-info/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    14785 2024-05-20 19:52:11.000000 llm2vec-0.1.7/llm2vec.egg-info/PKG-INFO
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      687 2024-05-20 19:52:11.000000 llm2vec-0.1.7/llm2vec.egg-info/SOURCES.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-05-20 19:52:11.000000 llm2vec-0.1.7/llm2vec.egg-info/dependency_links.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-04-16 16:57:16.000000 llm2vec-0.1.7/llm2vec.egg-info/not-zip-safe
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       74 2024-05-20 19:52:11.000000 llm2vec-0.1.7/llm2vec.egg-info/requires.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        8 2024-05-20 19:52:11.000000 llm2vec-0.1.7/llm2vec.egg-info/top_level.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       79 2024-05-20 19:52:11.352866 llm2vec-0.1.7/setup.cfg
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1089 2024-04-17 17:32:47.000000 llm2vec-0.1.7/setup.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-22 19:22:56.767772 llm2vec-0.1.8/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1067 2024-04-08 21:09:47.000000 llm2vec-0.1.8/LICENSE
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    14785 2024-05-22 19:22:56.768016 llm2vec-0.1.8/PKG-INFO
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    14335 2024-05-20 19:39:21.000000 llm2vec-0.1.8/README.md
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-22 19:22:56.751928 llm2vec-0.1.8/llm2vec/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       29 2024-04-16 16:56:44.000000 llm2vec-0.1.8/llm2vec/__init__.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-22 19:22:56.760272 llm2vec-0.1.8/llm2vec/dataset/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     6148 2024-05-08 16:25:06.000000 llm2vec-0.1.8/llm2vec/dataset/E5Data.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1368 2024-05-20 19:39:21.000000 llm2vec-0.1.8/llm2vec/dataset/Wiki1M.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       53 2024-05-20 19:39:21.000000 llm2vec-0.1.8/llm2vec/dataset/__init__.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1137 2024-05-20 19:39:21.000000 llm2vec-0.1.8/llm2vec/dataset/dataset.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      778 2024-05-20 19:39:21.000000 llm2vec-0.1.8/llm2vec/dataset/utils.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     2417 2024-04-30 22:31:54.000000 llm2vec-0.1.8/llm2vec/experiment_utils.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    16796 2024-05-20 19:39:21.000000 llm2vec-0.1.8/llm2vec/llm2vec.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-22 19:22:56.763459 llm2vec-0.1.8/llm2vec/loss/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1478 2024-04-30 22:31:54.000000 llm2vec-0.1.8/llm2vec/loss/HardNegativeNLLLoss.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       52 2024-04-30 22:31:54.000000 llm2vec-0.1.8/llm2vec/loss/__init__.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     3080 2024-04-30 22:31:54.000000 llm2vec-0.1.8/llm2vec/loss/loss_utils.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      289 2024-04-30 22:31:54.000000 llm2vec-0.1.8/llm2vec/loss/utils.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-22 19:22:56.766688 llm2vec-0.1.8/llm2vec/models/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      130 2024-04-16 16:56:44.000000 llm2vec-0.1.8/llm2vec/models/__init__.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7620 2024-04-16 16:56:44.000000 llm2vec-0.1.8/llm2vec/models/attn_mask_utils.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7837 2024-05-22 19:22:23.000000 llm2vec-0.1.8/llm2vec/models/bidirectional_llama.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    10368 2024-04-17 17:32:47.000000 llm2vec-0.1.8/llm2vec/models/bidirectional_mistral.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       22 2024-05-22 19:22:37.000000 llm2vec-0.1.8/llm2vec/version.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-05-22 19:22:56.756119 llm2vec-0.1.8/llm2vec.egg-info/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    14785 2024-05-22 19:22:56.000000 llm2vec-0.1.8/llm2vec.egg-info/PKG-INFO
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      687 2024-05-22 19:22:56.000000 llm2vec-0.1.8/llm2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-05-22 19:22:56.000000 llm2vec-0.1.8/llm2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-04-16 16:57:16.000000 llm2vec-0.1.8/llm2vec.egg-info/not-zip-safe
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       74 2024-05-22 19:22:56.000000 llm2vec-0.1.8/llm2vec.egg-info/requires.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        8 2024-05-22 19:22:56.000000 llm2vec-0.1.8/llm2vec.egg-info/top_level.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       79 2024-05-22 19:22:56.768905 llm2vec-0.1.8/setup.cfg
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1089 2024-04-17 17:32:47.000000 llm2vec-0.1.8/setup.py
```

### Comparing `llm2vec-0.1.7/LICENSE` & `llm2vec-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.7/PKG-INFO` & `llm2vec-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm2vec
-Version: 0.1.7
+Version: 0.1.8
 Summary: The official llm2vec library
 Home-page: https://github.com/McGill-NLP/llm2vec
 Author: McGill NLP
 Author-email: parishad.behnamghader@mila.quebec
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `llm2vec-0.1.7/README.md` & `llm2vec-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.7/llm2vec/dataset/E5Data.py` & `llm2vec-0.1.8/llm2vec/dataset/E5Data.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.7/llm2vec/dataset/Wiki1M.py` & `llm2vec-0.1.8/llm2vec/dataset/Wiki1M.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.7/llm2vec/dataset/dataset.py` & `llm2vec-0.1.8/llm2vec/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.7/llm2vec/dataset/utils.py` & `llm2vec-0.1.8/llm2vec/dataset/utils.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.7/llm2vec/experiment_utils.py` & `llm2vec-0.1.8/llm2vec/experiment_utils.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.7/llm2vec/llm2vec.py` & `llm2vec-0.1.8/llm2vec/llm2vec.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.7/llm2vec/loss/HardNegativeNLLLoss.py` & `llm2vec-0.1.8/llm2vec/loss/HardNegativeNLLLoss.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.7/llm2vec/loss/loss_utils.py` & `llm2vec-0.1.8/llm2vec/loss/loss_utils.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.7/llm2vec/models/attn_mask_utils.py` & `llm2vec-0.1.8/llm2vec/models/attn_mask_utils.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.7/llm2vec/models/bidirectional_llama.py` & `llm2vec-0.1.8/llm2vec/models/bidirectional_llama.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         )
         self.norm = LlamaRMSNorm(config.hidden_size, eps=config.rms_norm_eps)
         self.gradient_checkpointing = False
 
         # Initialize weights and apply final processing
         self.post_init()
 
-    def _update_causal_mask(self, attention_mask, input_tensor, cache_position, past_seen_tokens=None):
+    def _update_causal_mask(self, attention_mask, input_tensor, cache_position, past_seen_tokens=None, output_attentions=False):
         if self.config._attn_implementation == "flash_attention_2":
             if attention_mask is not None and 0.0 in attention_mask:
                 return attention_mask
             return None
 
         # if is_transformers_attn_greater_or_equal_4_40() and self.config._attn_implementation == "sdpa":
         #     # For SDPA, when possible, we will rely on its `is_causal` argument instead of its `attn_mask` argument,
@@ -175,14 +175,15 @@
                     : mask_shape[3],
                 ] = mask_slice
 
         if (
             self.config._attn_implementation == "sdpa"
             and attention_mask is not None
             and attention_mask.device.type == "cuda"
+            and not output_attentions
         ):
             causal_mask = AttentionMaskConverter._unmask_unattended(
                 causal_mask, min_dtype
             )
 
         return causal_mask
```

### Comparing `llm2vec-0.1.7/llm2vec/models/bidirectional_mistral.py` & `llm2vec-0.1.8/llm2vec/models/bidirectional_mistral.py`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.7/llm2vec.egg-info/PKG-INFO` & `llm2vec-0.1.8/llm2vec.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llm2vec
-Version: 0.1.7
+Version: 0.1.8
 Summary: The official llm2vec library
 Home-page: https://github.com/McGill-NLP/llm2vec
 Author: McGill NLP
 Author-email: parishad.behnamghader@mila.quebec
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `llm2vec-0.1.7/llm2vec.egg-info/SOURCES.txt` & `llm2vec-0.1.8/llm2vec.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.7/setup.py` & `llm2vec-0.1.8/setup.py`

 * *Files identical despite different names*

