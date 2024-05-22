# Comparing `tmp/antspynet-0.2.3.tar.gz` & `tmp/antspynet-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antspynet-0.2.3.tar", last modified: Thu Jul 13 15:45:32 2023, max compression
+gzip compressed data, was "antspynet-0.2.5.tar", last modified: Wed May 22 14:38:01 2024, max compression
```

## Comparing `antspynet-0.2.3.tar` & `antspynet-0.2.5.tar`

### file list

```diff
@@ -1,93 +1,14 @@
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-07-13 15:45:32.682082 antspynet-0.2.3/
--rw-r--r--   0 stnava     (501) staff       (20)    11357 2023-06-06 13:36:51.000000 antspynet-0.2.3/LICENSE.md
--rw-r--r--   0 stnava     (501) staff       (20)     8365 2023-07-13 15:45:32.681891 antspynet-0.2.3/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)     7944 2023-07-13 13:29:28.000000 antspynet-0.2.3/README.md
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-07-13 15:45:32.663018 antspynet-0.2.3/antspynet/
--rw-r--r--   0 stnava     (501) staff       (20)       76 2023-07-13 13:31:06.000000 antspynet-0.2.3/antspynet/__init__.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-07-13 15:45:32.671349 antspynet-0.2.3/antspynet/architectures/
--rw-r--r--   0 stnava     (501) staff       (20)     3369 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/architectures/__init__.py
--rw-r--r--   0 stnava     (501) staff       (20)    14057 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_alexnet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     2090 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_autoencoder_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     8296 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_convolutional_autoencoder_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     3121 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_custom_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    36597 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_custom_unet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    14211 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_cycle_gan_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    19564 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_deep_back_projection_network_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    10368 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_deep_convolutional_gan_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     8187 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_deep_denoise_super_resolution_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     6197 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_denoising_auto_encoder_super_resolution_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     1704 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_dense_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    13539 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_densenet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    19534 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_denseunet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    15888 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_diffusion_probabilistic_unet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     6163 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_expanded_super_resolution_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     5198 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_image_super_resolution_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    12707 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_improved_wasserstein_gan_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    13493 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_partial_convolution_unet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    17166 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/architectures/create_resnet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     8637 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_resnet_super_resolution_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    27712 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_resunet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     7749 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_simple_classification_with_spatial_transformer_network_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    16664 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_super_resolution_gan_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    16819 2023-07-13 14:21:43.000000 antspynet-0.2.3/antspynet/architectures/create_transformer_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    21396 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/architectures/create_unet_model.py
--rw-r--r--   0 stnava     (501) staff       (20)     6447 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_vanilla_gan_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    11244 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_vgg_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    11233 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_wasserstein_gan_model.py
--rw-r--r--   0 stnava     (501) staff       (20)    15261 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/architectures/create_wide_resnet_model.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-07-13 15:45:32.681253 antspynet-0.2.3/antspynet/utilities/
--rw-r--r--   0 stnava     (501) staff       (20)     4519 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/__init__.py
--rw-r--r--   0 stnava     (501) staff       (20)     8814 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/attention_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)     4994 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/brain_age.py
--rw-r--r--   0 stnava     (501) staff       (20)    10684 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/brain_extraction.py
--rw-r--r--   0 stnava     (501) staff       (20)    17634 2023-07-13 14:23:17.000000 antspynet-0.2.3/antspynet/utilities/cerebellum_morphology.py
--rw-r--r--   0 stnava     (501) staff       (20)     8215 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/claustrum_segmentation.py
--rw-r--r--   0 stnava     (501) staff       (20)     8886 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/cortical_thickness.py
--rw-r--r--   0 stnava     (501) staff       (20)     3104 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/cropping_and_padding_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)     1002 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/custom_activation_layers.py
--rw-r--r--   0 stnava     (501) staff       (20)    10664 2023-06-06 13:37:10.000000 antspynet-0.2.3/antspynet/utilities/custom_convolution_layers.py
--rw-r--r--   0 stnava     (501) staff       (20)     8323 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/custom_metrics.py
--rw-r--r--   0 stnava     (501) staff       (20)     5826 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/custom_normalization_layers.py
--rw-r--r--   0 stnava     (501) staff       (20)    14233 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/data_augmentation.py
--rw-r--r--   0 stnava     (501) staff       (20)     6732 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/deep_atropos.py
--rw-r--r--   0 stnava     (501) staff       (20)     8009 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/deep_embedded_clustering_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)    40258 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/deep_flash.py
--rw-r--r--   0 stnava     (501) staff       (20)     1688 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/denseunet_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)    20657 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/desikan_killiany_tourville_labeling.py
--rw-r--r--   0 stnava     (501) staff       (20)     9997 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/extract_image_patches.py
--rw-r--r--   0 stnava     (501) staff       (20)     6901 2023-06-09 14:56:59.000000 antspynet-0.2.3/antspynet/utilities/gaussian_diffusion_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)     5768 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/get_antsxnet_data.py
--rw-r--r--   0 stnava     (501) staff       (20)    17235 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/get_pretrained_network.py
--rw-r--r--   0 stnava     (501) staff       (20)     8513 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/hippmapp3r_segmentation.py
--rw-r--r--   0 stnava     (501) staff       (20)     4847 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/histogram_warp_image_intensities.py
--rw-r--r--   0 stnava     (501) staff       (20)    28688 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/histology.py
--rw-r--r--   0 stnava     (501) staff       (20)     4881 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/hypothalamus_segmentation.py
--rw-r--r--   0 stnava     (501) staff       (20)    11197 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/inpainting.py
--rw-r--r--   0 stnava     (501) staff       (20)    18688 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/lung_extraction.py
--rw-r--r--   0 stnava     (501) staff       (20)     6470 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/lung_segmentation.py
--rw-r--r--   0 stnava     (501) staff       (20)    12055 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/mixture_density_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)     3375 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/mri_modality_classification.py
--rw-r--r--   0 stnava     (501) staff       (20)     1518 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/mri_super_resolution.py
--rw-r--r--   0 stnava     (501) staff       (20)    18169 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/neural_style_transfer.py
--rw-r--r--   0 stnava     (501) staff       (20)     8633 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/preprocess_image.py
--rw-r--r--   0 stnava     (501) staff       (20)    16947 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/quality_assessment.py
--rw-r--r--   0 stnava     (501) staff       (20)    11102 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/randomly_transform_image_data.py
--rw-r--r--   0 stnava     (501) staff       (20)    11224 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/reconstruct_image_from_patches.py
--rw-r--r--   0 stnava     (501) staff       (20)     2856 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/regression_match_image.py
--rw-r--r--   0 stnava     (501) staff       (20)    11048 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/resample_tensor_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)     2518 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/simulate_bias_field.py
--rw-r--r--   0 stnava     (501) staff       (20)    14538 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/spatial_transformer_network_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)    11177 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/super_resolution_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)     7144 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/transformer_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)     8233 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/ukbb.py
--rw-r--r--   0 stnava     (501) staff       (20)     2871 2023-06-06 13:36:51.000000 antspynet-0.2.3/antspynet/utilities/unet_utilities.py
--rw-r--r--   0 stnava     (501) staff       (20)    46627 2023-07-13 13:29:28.000000 antspynet-0.2.3/antspynet/utilities/white_matter_hyperintensity_segmentation.py
-drwxr-xr-x   0 stnava     (501) staff       (20)        0 2023-07-13 15:45:32.664145 antspynet-0.2.3/antspynet.egg-info/
--rw-r--r--   0 stnava     (501) staff       (20)     8365 2023-07-13 15:45:32.000000 antspynet-0.2.3/antspynet.egg-info/PKG-INFO
--rw-r--r--   0 stnava     (501) staff       (20)     4046 2023-07-13 15:45:32.000000 antspynet-0.2.3/antspynet.egg-info/SOURCES.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2023-07-13 15:45:32.000000 antspynet-0.2.3/antspynet.egg-info/dependency_links.txt
--rw-r--r--   0 stnava     (501) staff       (20)        1 2023-06-06 13:37:14.000000 antspynet-0.2.3/antspynet.egg-info/not-zip-safe
--rw-r--r--   0 stnava     (501) staff       (20)       99 2023-07-13 15:45:32.000000 antspynet-0.2.3/antspynet.egg-info/requires.txt
--rw-r--r--   0 stnava     (501) staff       (20)       54 2023-07-13 15:45:32.000000 antspynet-0.2.3/antspynet.egg-info/top_level.txt
--rw-r--r--   0 stnava     (501) staff       (20)       38 2023-07-13 15:45:32.682126 antspynet-0.2.3/setup.cfg
--rw-r--r--   0 stnava     (501) staff       (20)     1296 2023-07-13 13:29:28.000000 antspynet-0.2.3/setup.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-22 14:38:01.101995 antspynet-0.2.5/
+-rw-r--r--   0 stnava     (501) staff       (20)    11357 2023-06-06 13:36:51.000000 antspynet-0.2.5/LICENSE.md
+-rw-r--r--   0 stnava     (501) staff       (20)    11858 2024-05-22 14:38:01.101791 antspynet-0.2.5/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)    11027 2024-05-22 14:29:17.000000 antspynet-0.2.5/README.md
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-22 14:38:01.100848 antspynet-0.2.5/antspynet/
+-rw-r--r--   0 stnava     (501) staff       (20)      130 2024-05-22 13:48:43.000000 antspynet-0.2.5/antspynet/__init__.py
+drwxr-xr-x   0 stnava     (501) staff       (20)        0 2024-05-22 14:38:01.101616 antspynet-0.2.5/antspynet.egg-info/
+-rw-r--r--   0 stnava     (501) staff       (20)    11858 2024-05-22 14:38:01.000000 antspynet-0.2.5/antspynet.egg-info/PKG-INFO
+-rw-r--r--   0 stnava     (501) staff       (20)      221 2024-05-22 14:38:01.000000 antspynet-0.2.5/antspynet.egg-info/SOURCES.txt
+-rw-r--r--   0 stnava     (501) staff       (20)        1 2024-05-22 14:38:01.000000 antspynet-0.2.5/antspynet.egg-info/dependency_links.txt
+-rw-r--r--   0 stnava     (501) staff       (20)       83 2024-05-22 14:38:01.000000 antspynet-0.2.5/antspynet.egg-info/requires.txt
+-rw-r--r--   0 stnava     (501) staff       (20)       10 2024-05-22 14:38:01.000000 antspynet-0.2.5/antspynet.egg-info/top_level.txt
+-rw-r--r--   0 stnava     (501) staff       (20)      976 2024-05-22 14:27:59.000000 antspynet-0.2.5/pyproject.toml
+-rw-r--r--   0 stnava     (501) staff       (20)       38 2024-05-22 14:38:01.102038 antspynet-0.2.5/setup.cfg
```

### Comparing `antspynet-0.2.3/LICENSE.md` & `antspynet-0.2.5/LICENSE.md`

 * *Files identical despite different names*

