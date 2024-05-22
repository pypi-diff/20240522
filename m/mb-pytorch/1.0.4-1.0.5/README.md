# Comparing `tmp/mb_pytorch-1.0.4.tar.gz` & `tmp/mb_pytorch-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mb_pytorch-1.0.4.tar", last modified: Tue Apr 30 14:49:40 2024, max compression
+gzip compressed data, was "mb_pytorch-1.0.5.tar", last modified: Tue Apr 30 16:58:37 2024, max compression
```

## Comparing `mb_pytorch-1.0.4.tar` & `mb_pytorch-1.0.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 14:49:40.679221 mb_pytorch-1.0.4/
--rw-r--r--   0 winnow    (1000) winnow    (1000)      205 2024-04-30 14:49:40.679221 mb_pytorch-1.0.4/PKG-INFO
--rw-rw-r--   0 winnow    (1000) winnow    (1000)      742 2024-04-30 13:36:42.000000 mb_pytorch-1.0.4/README.md
-drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 14:49:40.675221 mb_pytorch-1.0.4/mb_pytorch/
--rw-rw-r--   0 winnow    (1000) winnow    (1000)       97 2024-04-30 14:49:22.000000 mb_pytorch-1.0.4/mb_pytorch/__init__.py
-drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 14:49:40.675221 mb_pytorch-1.0.4/mb_pytorch/dataloader/
--rw-rw-r--   0 winnow    (1000) winnow    (1000)       44 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/dataloader/__init__.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)    12981 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/dataloader/loader.py
-drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 14:49:40.675221 mb_pytorch-1.0.4/mb_pytorch/metalearning/
--rw-rw-r--   0 winnow    (1000) winnow    (1000)        0 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/metalearning/__init__.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)     1385 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/metalearning/meta_utils.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)     1030 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/metalearning/proto_dataloader.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)     2861 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/metalearning/prototypical.py
-drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 14:49:40.679221 mb_pytorch-1.0.4/mb_pytorch/models/
--rw-rw-r--   0 winnow    (1000) winnow    (1000)        0 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/models/__init__.py
-drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 14:49:40.679221 mb_pytorch-1.0.4/mb_pytorch/models/blocks/
--rw-rw-r--   0 winnow    (1000) winnow    (1000)        0 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/models/blocks/__init__.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)     2801 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/models/blocks/attention_block.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)     3629 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/models/blocks/cnn.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)     4783 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/models/blocks/conv_block.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)      920 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/models/blocks/conv_with_relu.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)     2256 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/models/blocks/model_out.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)     1184 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/models/blocks/rnn.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)    21087 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/models/extra_models.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)      920 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/models/lenet.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)     3661 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/models/modelloader.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)    10784 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/models/unet_models.py
-drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 14:49:40.679221 mb_pytorch-1.0.4/mb_pytorch/utils/
--rw-rw-r--   0 winnow    (1000) winnow    (1000)        0 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/utils/__init__.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)     1055 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/utils/compiler.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)      257 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/utils/dist.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)     3391 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/utils/extra_utils.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)     7178 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/utils/generate_emb.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)     2582 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/utils/losses.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)     1199 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/utils/metrics.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)    10502 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/utils/viewer.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)      994 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/mb_pytorch/utils/yaml_reader.py
-drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 14:49:40.679221 mb_pytorch-1.0.4/mb_pytorch.egg-info/
--rw-r--r--   0 winnow    (1000) winnow    (1000)      205 2024-04-30 14:49:40.000000 mb_pytorch-1.0.4/mb_pytorch.egg-info/PKG-INFO
--rw-rw-r--   0 winnow    (1000) winnow    (1000)     1225 2024-04-30 14:49:40.000000 mb_pytorch-1.0.4/mb_pytorch.egg-info/SOURCES.txt
--rw-rw-r--   0 winnow    (1000) winnow    (1000)        1 2024-04-30 14:49:40.000000 mb_pytorch-1.0.4/mb_pytorch.egg-info/dependency_links.txt
--rw-rw-r--   0 winnow    (1000) winnow    (1000)       27 2024-04-30 14:49:40.000000 mb_pytorch-1.0.4/mb_pytorch.egg-info/requires.txt
--rw-rw-r--   0 winnow    (1000) winnow    (1000)       19 2024-04-30 14:49:40.000000 mb_pytorch-1.0.4/mb_pytorch.egg-info/top_level.txt
--rw-rw-r--   0 winnow    (1000) winnow    (1000)       81 2024-04-30 13:39:22.000000 mb_pytorch-1.0.4/pyproject.toml
-drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 14:49:40.679221 mb_pytorch-1.0.4/scripts/
--rw-rw-r--   0 winnow    (1000) winnow    (1000)        0 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/scripts/__init__.py
-drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 14:49:40.679221 mb_pytorch-1.0.4/scripts/extra_utils/
--rw-rw-r--   0 winnow    (1000) winnow    (1000)        0 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/scripts/extra_utils/__init__.py
--rwxrwxr-x   0 winnow    (1000) winnow    (1000)     1314 2023-06-01 10:35:06.000000 mb_pytorch-1.0.4/scripts/extra_utils/dataload_results.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)       38 2024-04-30 14:49:40.679221 mb_pytorch-1.0.4/setup.cfg
--rw-rw-r--   0 winnow    (1000) winnow    (1000)      818 2024-04-30 13:40:06.000000 mb_pytorch-1.0.4/setup.py
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 16:58:37.438201 mb_pytorch-1.0.5/
+-rw-r--r--   0 winnow    (1000) winnow    (1000)      205 2024-04-30 16:58:37.438201 mb_pytorch-1.0.5/PKG-INFO
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)      742 2024-04-30 13:36:42.000000 mb_pytorch-1.0.5/README.md
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 16:58:37.434200 mb_pytorch-1.0.5/mb_pytorch/
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)       97 2024-04-30 14:49:22.000000 mb_pytorch-1.0.5/mb_pytorch/__init__.py
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 16:58:37.434200 mb_pytorch-1.0.5/mb_pytorch/dataloader/
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)       44 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/dataloader/__init__.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)    12981 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/dataloader/loader.py
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 16:58:37.434200 mb_pytorch-1.0.5/mb_pytorch/metalearning/
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)        0 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/metalearning/__init__.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     1385 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/metalearning/meta_utils.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     1030 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/metalearning/proto_dataloader.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     2861 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/metalearning/prototypical.py
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 16:58:37.434200 mb_pytorch-1.0.5/mb_pytorch/models/
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)        0 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/__init__.py
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 16:58:37.434200 mb_pytorch-1.0.5/mb_pytorch/models/blocks/
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)        0 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/blocks/__init__.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     2801 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/blocks/attention_block.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     3629 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/blocks/cnn.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     4783 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/blocks/conv_block.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)      920 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/blocks/conv_with_relu.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     2256 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/blocks/model_out.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     1184 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/blocks/rnn.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)    21087 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/extra_models.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)      920 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/lenet.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     3661 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/modelloader.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)    10784 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/models/unet_models.py
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 16:58:37.434200 mb_pytorch-1.0.5/mb_pytorch/utils/
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)        0 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/utils/__init__.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     1055 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/utils/compiler.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)      257 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/utils/dist.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     3391 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/utils/extra_utils.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     7178 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/utils/generate_emb.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     2582 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/utils/losses.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     1199 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/utils/metrics.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)    10502 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/utils/viewer.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)      994 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/mb_pytorch/utils/yaml_reader.py
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 16:58:37.438201 mb_pytorch-1.0.5/mb_pytorch.egg-info/
+-rw-r--r--   0 winnow    (1000) winnow    (1000)      205 2024-04-30 16:58:37.000000 mb_pytorch-1.0.5/mb_pytorch.egg-info/PKG-INFO
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)     1225 2024-04-30 16:58:37.000000 mb_pytorch-1.0.5/mb_pytorch.egg-info/SOURCES.txt
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)        1 2024-04-30 16:58:37.000000 mb_pytorch-1.0.5/mb_pytorch.egg-info/dependency_links.txt
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)       27 2024-04-30 16:58:37.000000 mb_pytorch-1.0.5/mb_pytorch.egg-info/requires.txt
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)       19 2024-04-30 16:58:37.000000 mb_pytorch-1.0.5/mb_pytorch.egg-info/top_level.txt
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)       81 2024-04-30 13:39:22.000000 mb_pytorch-1.0.5/pyproject.toml
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 16:58:37.434200 mb_pytorch-1.0.5/scripts/
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)        0 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/scripts/__init__.py
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-04-30 16:58:37.434200 mb_pytorch-1.0.5/scripts/extra_utils/
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)        0 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/scripts/extra_utils/__init__.py
+-rwxrwxr-x   0 winnow    (1000) winnow    (1000)     1314 2023-06-01 10:35:06.000000 mb_pytorch-1.0.5/scripts/extra_utils/dataload_results.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)       38 2024-04-30 16:58:37.438201 mb_pytorch-1.0.5/setup.cfg
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)      818 2024-04-30 13:40:06.000000 mb_pytorch-1.0.5/setup.py
```

### Comparing `mb_pytorch-1.0.4/README.md` & `mb_pytorch-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch/dataloader/loader.py` & `mb_pytorch-1.0.5/mb_pytorch/dataloader/loader.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch/metalearning/meta_utils.py` & `mb_pytorch-1.0.5/mb_pytorch/metalearning/meta_utils.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch/metalearning/proto_dataloader.py` & `mb_pytorch-1.0.5/mb_pytorch/metalearning/proto_dataloader.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch/metalearning/prototypical.py` & `mb_pytorch-1.0.5/mb_pytorch/metalearning/prototypical.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch/models/blocks/attention_block.py` & `mb_pytorch-1.0.5/mb_pytorch/models/blocks/attention_block.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch/models/blocks/cnn.py` & `mb_pytorch-1.0.5/mb_pytorch/models/blocks/cnn.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch/models/blocks/conv_block.py` & `mb_pytorch-1.0.5/mb_pytorch/models/blocks/conv_block.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch/models/blocks/conv_with_relu.py` & `mb_pytorch-1.0.5/mb_pytorch/models/blocks/conv_with_relu.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch/models/blocks/model_out.py` & `mb_pytorch-1.0.5/mb_pytorch/models/blocks/model_out.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch/models/blocks/rnn.py` & `mb_pytorch-1.0.5/mb_pytorch/models/blocks/rnn.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch/models/extra_models.py` & `mb_pytorch-1.0.5/mb_pytorch/models/extra_models.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch/models/lenet.py` & `mb_pytorch-1.0.5/mb_pytorch/models/lenet.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch/models/modelloader.py` & `mb_pytorch-1.0.5/mb_pytorch/models/modelloader.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch/models/unet_models.py` & `mb_pytorch-1.0.5/mb_pytorch/models/unet_models.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch/utils/compiler.py` & `mb_pytorch-1.0.5/mb_pytorch/utils/compiler.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch/utils/extra_utils.py` & `mb_pytorch-1.0.5/mb_pytorch/utils/extra_utils.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch/utils/generate_emb.py` & `mb_pytorch-1.0.5/mb_pytorch/utils/generate_emb.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch/utils/losses.py` & `mb_pytorch-1.0.5/mb_pytorch/utils/losses.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch/utils/metrics.py` & `mb_pytorch-1.0.5/mb_pytorch/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch/utils/viewer.py` & `mb_pytorch-1.0.5/mb_pytorch/utils/viewer.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch/utils/yaml_reader.py` & `mb_pytorch-1.0.5/mb_pytorch/utils/yaml_reader.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/mb_pytorch.egg-info/SOURCES.txt` & `mb_pytorch-1.0.5/mb_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/scripts/extra_utils/dataload_results.py` & `mb_pytorch-1.0.5/scripts/extra_utils/dataload_results.py`

 * *Files identical despite different names*

### Comparing `mb_pytorch-1.0.4/setup.py` & `mb_pytorch-1.0.5/setup.py`

 * *Files identical despite different names*

