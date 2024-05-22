# Comparing `tmp/nvidia_dali_nightly_cuda120-1.39.0.dev20240520.tar.gz` & `tmp/nvidia_dali_nightly_cuda120-1.39.0.dev20240521.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia_dali_nightly_cuda120-1.39.0.dev20240520.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
+gzip compressed data, was "nvidia_dali_nightly_cuda120-1.39.0.dev20240521.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `nvidia_dali_nightly_cuda120-1.39.0.dev20240520.tar` & `nvidia_dali_nightly_cuda120-1.39.0.dev20240521.tar`

### PKG-INFO

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda120
-Version: 1.39.0.dev20240520
-Summary: NVIDIA DALI nightly  for CUDA 12.0. Git SHA: 306221661a585ed7791857141e15b69e28952905
+Version: 1.39.0.dev20240521
+Summary: NVIDIA DALI nightly  for CUDA 12.0. Git SHA: d0f8231f99c406b4553b5c5fbc9c673460e2ac6d
 Home-page: https://github.com/NVIDIA/dali
 Author: NVIDIA Corporation
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

