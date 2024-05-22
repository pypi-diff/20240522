# Comparing `tmp/pycellmech-2.1.8.tar.gz` & `tmp/pycellmech-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pycellmech-2.1.8.tar", last modified: Sat May 18 01:50:45 2024, max compression
+gzip compressed data, was "dist/pycellmech-2.1.9.tar", last modified: Wed May 22 21:22:51 2024, max compression
```

## Comparing `pycellmech-2.1.8.tar` & `pycellmech-2.1.9.tar`

### file list

```diff
@@ -1,21 +1,29 @@
-drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 01:50:45.105371 pycellmech-2.1.8/
--rw-rw-r--   0 janan.arslan (31680)    10513       20 2024-05-18 01:50:12.000000 pycellmech-2.1.8/MANIFEST.in
--rw-r--r--   0 janan.arslan (31680)    10513     7782 2024-05-18 01:50:45.106020 pycellmech-2.1.8/PKG-INFO
--rw-rw-r--   0 janan.arslan (31680)    10513     5873 2024-05-18 00:12:55.000000 pycellmech-2.1.8/README.md
--rw-rw-r--   0 janan.arslan (31680)    10513       79 2024-05-18 01:50:45.107289 pycellmech-2.1.8/setup.cfg
--rw-rw-r--   0 janan.arslan (31680)    10513     1171 2024-05-18 01:50:17.000000 pycellmech-2.1.8/setup.py
-drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 01:50:45.088615 pycellmech-2.1.8/src/
-drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 01:50:45.097914 pycellmech-2.1.8/src/pycellmech/
--rw-rw-r--   0 janan.arslan (31680)    10513      140 2024-05-18 01:25:31.000000 pycellmech-2.1.8/src/pycellmech/__init__.py
--rw-r--r--   0 janan.arslan (31680)    10513      627 2024-05-18 01:32:02.000000 pycellmech-2.1.8/src/pycellmech/cli.py
--rw-rw-r--   0 janan.arslan (31680)    10513    14907 2024-05-18 00:12:55.000000 pycellmech-2.1.8/src/pycellmech/geometric_shape_features.py
--rw-rw-r--   0 janan.arslan (31680)    10513     8999 2024-05-18 01:48:29.000000 pycellmech-2.1.8/src/pycellmech/main.py
--rw-rw-r--   0 janan.arslan (31680)    10513     9396 2024-05-18 00:12:55.000000 pycellmech-2.1.8/src/pycellmech/one_dimensional_features.py
--rw-rw-r--   0 janan.arslan (31680)    10513    16979 2024-05-18 00:12:55.000000 pycellmech-2.1.8/src/pycellmech/polygonal_shape_features.py
-drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-18 01:50:45.104744 pycellmech-2.1.8/src/pycellmech.egg-info/
--rw-r--r--   0 janan.arslan (31680)    10513     7782 2024-05-18 01:50:44.000000 pycellmech-2.1.8/src/pycellmech.egg-info/PKG-INFO
--rw-r--r--   0 janan.arslan (31680)    10513      507 2024-05-18 01:50:45.000000 pycellmech-2.1.8/src/pycellmech.egg-info/SOURCES.txt
--rw-r--r--   0 janan.arslan (31680)    10513        1 2024-05-18 01:50:44.000000 pycellmech-2.1.8/src/pycellmech.egg-info/dependency_links.txt
--rw-r--r--   0 janan.arslan (31680)    10513       52 2024-05-18 01:50:44.000000 pycellmech-2.1.8/src/pycellmech.egg-info/entry_points.txt
--rw-r--r--   0 janan.arslan (31680)    10513       51 2024-05-18 01:50:44.000000 pycellmech-2.1.8/src/pycellmech.egg-info/requires.txt
--rw-r--r--   0 janan.arslan (31680)    10513       11 2024-05-18 01:50:44.000000 pycellmech-2.1.8/src/pycellmech.egg-info/top_level.txt
+drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-22 21:22:51.842064 pycellmech-2.1.9/
+-rw-rw-r--   0 janan.arslan (31680)    10513       20 2024-05-18 01:50:12.000000 pycellmech-2.1.9/MANIFEST.in
+-rw-r--r--   0 janan.arslan (31680)    10513     7782 2024-05-22 21:22:51.842459 pycellmech-2.1.9/PKG-INFO
+-rw-rw-r--   0 janan.arslan (31680)    10513     5873 2024-05-18 00:12:55.000000 pycellmech-2.1.9/README.md
+-rw-rw-r--   0 janan.arslan (31680)    10513       79 2024-05-22 21:22:51.843559 pycellmech-2.1.9/setup.cfg
+-rw-rw-r--   0 janan.arslan (31680)    10513     1387 2024-05-22 21:19:49.000000 pycellmech-2.1.9/setup.py
+drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-22 21:22:51.819372 pycellmech-2.1.9/src/
+drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-22 21:22:51.828047 pycellmech-2.1.9/src/pycellmech/
+-rw-rw-r--   0 janan.arslan (31680)    10513      140 2024-05-18 01:25:31.000000 pycellmech-2.1.9/src/pycellmech/__init__.py
+-rw-r--r--   0 janan.arslan (31680)    10513     2030 2024-05-22 21:09:28.000000 pycellmech-2.1.9/src/pycellmech/cli.py
+-rw-rw-r--   0 janan.arslan (31680)    10513    14907 2024-05-18 00:12:55.000000 pycellmech-2.1.9/src/pycellmech/geometric_shape_features.py
+-rw-r--r--   0 janan.arslan (31680)    10513    12783 2024-05-22 20:52:16.000000 pycellmech-2.1.9/src/pycellmech/main.py
+-rw-rw-r--   0 janan.arslan (31680)    10513     9396 2024-05-18 00:12:55.000000 pycellmech-2.1.9/src/pycellmech/one_dimensional_features.py
+-rw-rw-r--   0 janan.arslan (31680)    10513    16979 2024-05-18 00:12:55.000000 pycellmech-2.1.9/src/pycellmech/polygonal_shape_features.py
+drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-22 21:22:51.833945 pycellmech-2.1.9/src/pycellmech.egg-info/
+-rw-r--r--   0 janan.arslan (31680)    10513     7782 2024-05-22 21:22:51.000000 pycellmech-2.1.9/src/pycellmech.egg-info/PKG-INFO
+-rw-r--r--   0 janan.arslan (31680)    10513      720 2024-05-22 21:22:51.000000 pycellmech-2.1.9/src/pycellmech.egg-info/SOURCES.txt
+-rw-r--r--   0 janan.arslan (31680)    10513        1 2024-05-22 21:22:51.000000 pycellmech-2.1.9/src/pycellmech.egg-info/dependency_links.txt
+-rw-r--r--   0 janan.arslan (31680)    10513      156 2024-05-22 21:22:51.000000 pycellmech-2.1.9/src/pycellmech.egg-info/entry_points.txt
+-rw-r--r--   0 janan.arslan (31680)    10513       93 2024-05-22 21:22:51.000000 pycellmech-2.1.9/src/pycellmech.egg-info/requires.txt
+-rw-r--r--   0 janan.arslan (31680)    10513       52 2024-05-22 21:22:51.000000 pycellmech-2.1.9/src/pycellmech.egg-info/top_level.txt
+drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-22 21:22:51.837612 pycellmech-2.1.9/src/pycellmech_create_label/
+-rw-rw-r--   0 janan.arslan (31680)    10513       22 2024-05-22 21:18:02.000000 pycellmech-2.1.9/src/pycellmech_create_label/__init__.py
+-rw-r--r--   0 janan.arslan (31680)    10513     1000 2024-05-22 21:11:18.000000 pycellmech-2.1.9/src/pycellmech_create_label/cli.py
+-rw-r--r--   0 janan.arslan (31680)    10513     4084 2024-05-22 18:35:33.000000 pycellmech-2.1.9/src/pycellmech_create_label/main.py
+drwxr-xr-x   0 janan.arslan (31680)    10513        0 2024-05-22 21:22:51.840855 pycellmech-2.1.9/src/pycellmech_nifti/
+-rw-rw-r--   0 janan.arslan (31680)    10513       22 2024-05-22 21:17:58.000000 pycellmech-2.1.9/src/pycellmech_nifti/__init__.py
+-rw-r--r--   0 janan.arslan (31680)    10513     1188 2024-05-22 21:12:08.000000 pycellmech-2.1.9/src/pycellmech_nifti/cli.py
+-rw-r--r--   0 janan.arslan (31680)    10513     5806 2024-05-22 18:58:42.000000 pycellmech-2.1.9/src/pycellmech_nifti/main.py
```

### Comparing `pycellmech-2.1.8/PKG-INFO` & `pycellmech-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycellmech
-Version: 2.1.8
+Version: 2.1.9
 Summary: A shape-based feature extractor for use in biological and medical studies.
 Home-page: https://github.com/icm-dac/pycellmech
 Author: Janan Arslan
 Author-email: janan.arslan@icm-institute.org
 License: UNKNOWN
 Description: <div align="left">
           <img width="15%" src="/figures/pyrcellmech_logo_v2.png" alt="pycellmech Logo">
```

### Comparing `pycellmech-2.1.8/README.md` & `pycellmech-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pycellmech-2.1.8/setup.py` & `pycellmech-2.1.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 readme_path = os.path.join(current_directory, './README.md')
 with open(readme_path, encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="pycellmech",
-    version="2.1.8",
+    version="2.1.9",
     author="Janan Arslan",
     author_email="janan.arslan@icm-institute.org",
     description="A shape-based feature extractor for use in biological and medical studies.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/icm-dac/pycellmech",
     packages=find_packages(where='./src'),
@@ -25,16 +25,22 @@
     ],
     python_requires='>=3.6',
     install_requires=[
         "matplotlib",
         "numpy",
         "opencv-python",
         "pandas",
-        "scikit-learn"
+        "scikit-learn",
+        "SimpleITK",
+        "pandas",
+        "collections",
+        "scikit-image"
     ],
     include_package_data=True,
     entry_points={
         'console_scripts': [
             'pycellmech=pycellmech.cli:main',
+            'pycellmech_create_label=pycellmech_create_label.cli:main',
+            'pycellmech_nifti=pycellmech_nifti.cli:main',
         ],
     },
 )
```

### Comparing `pycellmech-2.1.8/src/pycellmech/geometric_shape_features.py` & `pycellmech-2.1.9/src/pycellmech/geometric_shape_features.py`

 * *Files identical despite different names*

### Comparing `pycellmech-2.1.8/src/pycellmech/main.py` & `pycellmech-2.1.9/src/pycellmech/main.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 '''
 ======================================================================
  Title:                   PYCELLMECH
  Creating Author:         Janan Arslan
  Creation Date:           22 FEB 2024
- Latest Modification:     17 MAY 2024
+ Latest Modification:     15 MAY 2024
  Modification Author:     Janan Arslan
  E-mail:                  janan.arslan@icm-institute.org
- Version:                 2.1.8
+ Version:                 2.1.9
 ======================================================================
 
 
 pycellmech is designed to extract appropriate shape features which can
 be used to extrapolated how the shape of objects in medical studies can
 be used to elucidate the mechanics of the disease and/or its progression.
 
@@ -24,31 +24,81 @@
 
 import os
 import cv2
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 import argparse
+import nibabel as nib
+import tempfile
+from skimage.measure import label, regionprops
+
+
+from .one_dimensional_features import (
+    get_one_dimensional_features, plot_original_contour, plot_centroid, 
+    plot_complex_coordinates, plot_cdf, plot_area_function, plot_clf, plot_tar
+)
+from .geometric_shape_features import (
+    get_geometric_shape_features, plot_AMI, plot_ABE, plot_eccentricity, 
+    plot_mbr, plot_circularity_ratio, plot_ellipse_features, plot_solidity
+)
+from .polygonal_shape_features import (
+    get_polyognal_shape_features, plot_DTM, plot_PEVD, plot_SM, plot_MPP, plot_KMeans
+)
 
-from .one_dimensional_features import get_one_dimensional_features, plot_original_contour, plot_centroid, plot_complex_coordinates, plot_cdf, plot_area_function, plot_clf, plot_tar
-from .geometric_shape_features import get_geometric_shape_features, plot_AMI, plot_ABE, plot_eccentricity, plot_mbr, plot_circularity_ratio, plot_ellipse_features, plot_solidity
-from .polygonal_shape_features import get_polyognal_shape_features, plot_DTM, plot_PEVD, plot_SM, plot_MPP, plot_KMeans
 
 # Preprocess image and find contours
 def preprocess_image(binary_image_path):
-    binary_image = cv2.imread(binary_image_path, 0)
+    binary_image = cv2.imread(binary_image_path, cv2.IMREAD_GRAYSCALE)
     blur = cv2.GaussianBlur(binary_image, (5, 5), 0)
     _, thresh = cv2.threshold(blur, 127, 255, cv2.THRESH_BINARY)
     kernel = np.ones((5,5), np.uint8)
     closing = cv2.morphologyEx(thresh, cv2.MORPH_CLOSE, kernel)
     contours, _ = cv2.findContours(closing, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
-    return contours
+    return contours, binary_image
+
+# Preprocess image and find contours
+def preprocess_slice(slice_data, label_value):
+    binary_image = np.uint8(slice_data == label_value) * 255
+    blur = cv2.GaussianBlur(binary_image, (5, 5), 0)
+    _, thresh = cv2.threshold(blur, 127, 255, cv2.THRESH_BINARY)
+    kernel = np.ones((5,5), np.uint8)
+    closing = cv2.morphologyEx(thresh, cv2.MORPH_CLOSE, kernel)
+    contours, _ = cv2.findContours(closing, cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE)
+    return contours, binary_image
+
+# Process NiFfty files
+def preprocess_nii_image(nii_image_path):
+    try:
+        nii_img = nib.load(nii_image_path)
+        nii_data = nii_img.get_fdata()
+        print(f'Loaded NIfTI file {nii_image_path} with shape {nii_data.shape}')
+    except Exception as e:
+        print(f'Error loading NIfTI file {nii_image_path}: {e}')
+        return [], {}
+
+    contours = []
+    binary_images = {}
+
+    if len(nii_data.shape) == 2:  # 2D case
+        for label_value in np.unique(nii_data):
+            if label_value == 0:  # Skip background
+                continue
+            label_contours, binary_image = preprocess_slice(nii_data, label_value)
+            for contour in label_contours:
+                contours.append((contour, label_value))
+            binary_images[label_value] = binary_image
+    else:
+        print(f'NIfTI file {nii_image_path} does not have the expected 2D shape.')
+        return [], {}
+
+    return contours, binary_images
 
 # Feature illustration through largest contour
-def plot_features(binary_image, contour, one_d_features, geom_features, poly_features, filename, output_folder):
+def plot_features(binary_image, contour, one_d_features, geom_features, poly_features, filename, output_folder, label=None):
     fig, axs = plt.subplots(4, 7, figsize=(45, 8), constrained_layout=False)
     fig.set_constrained_layout_pads(w_pad=4, h_pad=4, hspace=0.2, wspace=0.2)
 
     fig.suptitle('Shape Feature Visualization', fontsize=16)
 
     # Calculate moments for contour
     M = cv2.moments(contour)
@@ -67,17 +117,17 @@
 
     # Plot CDF
     cdf = one_d_features['cdf']
     plot_cdf(axs[0, 3], binary_image, cdf, cx, cy, contour)
 
     # Plot AF
     plot_area_function(axs[0, 4], binary_image, cx, cy, contour)
+    tangent_vectors = one_d_features['tangent_vectors']
 
     # Plot CLF
-    tangent_vectors = one_d_features['tangent_vectors']
     plot_clf(axs[0, 5], binary_image, contour, tangent_vectors)
 
     # Plot TAR
     tar_values = one_d_features['tar_values']
     plot_tar(axs[0, 6], binary_image, contour, tar_values)
 
     for row in axs:
@@ -112,29 +162,28 @@
 
     # Plot CR
     circularity_ratio = geom_features['circularity_ratio']
     axs[1, 4].axis('on')
     axs[1, 4].invert_yaxis()
     plot_circularity_ratio(axs[1, 4], contour_array, circularity_ratio)
 
-
     # Plot EV and EM
-    ev_value, em_value = geom_features['EV'],geom_features['EM']
+    ev_value, em_value = geom_features['EV'], geom_features['EM']
     axs[1, 5].axis('on')
     axs[1, 5].invert_yaxis()
     plot_ellipse_features(axs[1, 5], contour_array, ev_value, em_value)
 
-
     # Plot solidity
     solidity, hull = geom_features['solidity'], geom_features['hull']
     for ax in axs.flat:
         ax.set_aspect('equal')
     plot_solidity(axs[1, 6], contour_array, solidity)
 
-    # Plot DTM
+
+    # Plot DTM    
     # Flatten contour array
     contour_reshape = contour.reshape(-1, 2)
     dtm = poly_features['dtm']
     plot_DTM(axs[2, 0], contour_reshape, dtm)
 
     # Plot PEVD
     pevd = poly_features['pevd']
@@ -144,85 +193,131 @@
     sm = poly_features['sm']
     plot_SM(axs[2, 2], contour_reshape, sm)
 
     # Plot MPP
     mpp = poly_features['mpp']
     plot_MPP(axs[2, 3], contour_reshape, mpp)
 
-
     # Plot KMeans
     km_cluster_centers, km_line_segments, km_labels = poly_features['km_cc'], poly_features['km_ls'], poly_features['km_labels']
     plot_KMeans(axs[2, 4], contour_reshape, km_cluster_centers, km_line_segments, km_labels)
 
-
     # Adjust the spacing of the subplots
     plt.subplots_adjust(left=0.2, top=0.9)
 
     # Define the row titles
     row_titles = ['One-Dimensional \nShape Features', 'Geometric Shape \nFeatures', 'Polygonal\n Approximations']
 
     # Set the position for the row titles
-    row_title_positions = [(-1, 0.25), (-1, 0.25), (-1, 0.25)]  # (x, y) for each title
+    row_title_positions = [(-1, 0.25), (-1, 0.25), (-1, 0.25)]
 
     # Set the row titles
     for ax, title, pos in zip(axs[:,0], row_titles, row_title_positions):
         fig.text(pos[0], pos[1], title, transform=ax.transAxes, ha='center', fontsize=10, color='blue', weight='bold', style='italic')
 
     # Save features for the largest contour of every image
     plot_filename = os.path.splitext(filename)[0] + "_feature_map.jpg"
     plt.savefig(os.path.join(output_folder, plot_filename))
     plt.close(fig)
 
 
-def process_images(folder_path, csv_file_path, output_folder):
+# Overall process to extract features
+def process_file(file_path, label, args):
     all_features = []
 
-    for filename in os.listdir(folder_path):
-        if filename.lower().endswith((".jpg", ".png", ".jpeg", ".tiff", ".tif")):
-            file_path = os.path.join(folder_path, filename)
-            binary_image = cv2.imread(file_path, 0)
-            contours = preprocess_image(file_path)
-            largest_contour = max(contours, key=cv2.contourArea)
-            contour_number = 1
-
-            for i, contour in enumerate(contours):
-                M = cv2.moments(contour)
-                if M["m00"] != 0:
-                    cx = int(M["m10"] / M["m00"])
-                    cy = int(M["m01"] / M["m00"])
-                else:
-                    continue
-
-                one_d_features = get_one_dimensional_features(contour, cx, cy)
-                geom_features = get_geometric_shape_features(contour, cx, cy, file_path)
-                poly_features = get_polyognal_shape_features(contour, cx, cy, file_path)
-
-                combined_features = {'image_name': filename, 'contour_number': contour_number}
-                combined_features.update({**one_d_features, **geom_features, **poly_features})
-                all_features.append(combined_features)
-                contour_number += 1
-
-                if contour is largest_contour:
-                    largest_one_d_features = one_d_features
-                    largest_geom_features = geom_features
-                    largest_poly_features = poly_features
-
-            plot_features(binary_image, largest_contour, largest_one_d_features, largest_geom_features, largest_poly_features, filename, output_folder)
-            print(f'[PROCESSED] {filename}')
-
-    features_df = pd.DataFrame(all_features)
-    features_df.to_csv(csv_file_path, index=False)
-    print(f'[PROCESSED] Features saved to {csv_file_path}')
-
+    if label == 's':
+        contours, binary_image = preprocess_image(file_path)
+        binary_images = {1: binary_image}  # Single class, use label 1
+    else:
+        contours, binary_images = preprocess_nii_image(file_path)
+
+    print(f'Found {len(contours)} contours in {file_path}')
+
+    if len(contours) == 0:
+        print(f'No contours found in {file_path}')
+        return
+
+    largest_contour = max(contours, key=lambda x: cv2.contourArea(x[0] if label == 'm' else x))
+    contour_number = 1 
+
+    for i, item in enumerate(contours):
+        contour, lbl = item if label == 'm' else (item, None)
+        M = cv2.moments(contour)
+        if M["m00"] != 0:
+            cx = int(M["m10"] / M["m00"])
+            cy = int(M["m01"] / M["m00"])
+        else:
+            continue
+
+        binary_image = binary_images[lbl] if label == 'm' else binary_image
+
+        # Save binary_image to a temporary file
+        with tempfile.NamedTemporaryFile(suffix='.png', delete=False) as temp_file:
+            temp_filename = temp_file.name
+            cv2.imwrite(temp_filename, binary_image)
+
+        one_d_features = get_one_dimensional_features(contour, cx, cy)
+        geom_features = get_geometric_shape_features(contour, cx, cy, temp_filename)  # Pass temp file path
+        poly_features = get_polyognal_shape_features(contour, cx, cy, temp_filename)  # Pass temp file path
+
+        combined_features = {'image_name': os.path.basename(file_path), 'contour_number': contour_number, 'label': lbl if lbl is not None else 1}
+        combined_features.update({**one_d_features, **geom_features, **poly_features})
+        all_features.append(combined_features)
+        contour_number += 1 
+
+        if np.array_equal(contour, largest_contour[0] if label == 'm' else largest_contour):
+            largest_one_d_features = one_d_features
+            largest_geom_features = geom_features
+            largest_poly_features = poly_features
+
+    plot_features(binary_image, largest_contour[0] if label == 'm' else largest_contour, largest_one_d_features, largest_geom_features, largest_poly_features, os.path.basename(file_path), args.output, label=largest_contour[1] if label == 'm' else None)
+    print(f'[PROCESSED] {file_path}')
+
+    if all_features:
+        features_df = pd.DataFrame(all_features)
+        csv_filename = os.path.splitext(os.path.basename(file_path))[0] + "_features.csv"
+        features_df.to_csv(os.path.join(args.csv_save, csv_filename), index=False)
+        print(f'[PROCESSED] Features saved to {os.path.join(args.csv_save, csv_filename)}')
 
 
 def main():
-    parser = argparse.ArgumentParser(description='Process some images.')
-    parser.add_argument('--folder_path', type=str, required=True, help='Path to the folder containing binarized images')
-    parser.add_argument('--csv_file_path', type=str, required=True, help='Path to save the shape features CSV file')
-    parser.add_argument('--output_folder', type=str, required=True, help='Path to save the feature maps')
+    parser = argparse.ArgumentParser(description='Process binary mask images and extract shape features.')
+    parser.add_argument('--input', type=str, required=True, help='Path to the folder containing binary mask images.')
+    parser.add_argument('--csv_save', type=str, required=True, help='Folder to save the output CSV files.')
+    parser.add_argument('--output', type=str, required=True, help='Folder to save the output plots.')
+    parser.add_argument('--label', type=str, choices=['s', 'm'], required=True, help='Specify "s" for single class or "m" for multi-class masks.')
+    parser.add_argument('--nifti_folder', type=str, help='Folder containing NIfTI files for multi-class masks (required if --label is "m").')
 
     args = parser.parse_args()
-    process_images(args.folder_path, args.csv_file_path, args.output_folder)
+
+    if args.label == 'm' and not args.nifti_folder:
+        parser.error('--nifti_folder is required when --label is "m"')
+
+    if not os.path.exists(args.csv_save):
+        os.makedirs(args.csv_save)
+
+    if not os.path.exists(args.output):
+        os.makedirs(args.output)
+
+    if args.label == 's':
+        # Single-class case
+        input_folder = args.input
+        for filename in os.listdir(input_folder):
+            if filename.lower().endswith((".jpg", ".png", ".jpeg", ".tiff", ".tif")):
+                file_path = os.path.join(input_folder, filename)
+                process_file(file_path, args.label, args)
+            else:
+                print(f'Skipping file: {filename}')
+    else:
+        # Multi-class case
+        if os.path.isdir(args.nifti_folder):
+            for filename in os.listdir(args.nifti_folder):
+                if filename.lower().endswith(".nii"):
+                    file_path = os.path.join(args.nifti_folder, filename)
+                    process_file(file_path, args.label, args)
+                else:
+                    print(f'Skipping file: {filename}')
+        else:
+            print(f'Invalid folder: {args.nifti_folder}')
 
 if __name__ == "__main__":
     main()
```

### Comparing `pycellmech-2.1.8/src/pycellmech/one_dimensional_features.py` & `pycellmech-2.1.9/src/pycellmech/one_dimensional_features.py`

 * *Files identical despite different names*

### Comparing `pycellmech-2.1.8/src/pycellmech/polygonal_shape_features.py` & `pycellmech-2.1.9/src/pycellmech/polygonal_shape_features.py`

 * *Files identical despite different names*

### Comparing `pycellmech-2.1.8/src/pycellmech.egg-info/PKG-INFO` & `pycellmech-2.1.9/src/pycellmech.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycellmech
-Version: 2.1.8
+Version: 2.1.9
 Summary: A shape-based feature extractor for use in biological and medical studies.
 Home-page: https://github.com/icm-dac/pycellmech
 Author: Janan Arslan
 Author-email: janan.arslan@icm-institute.org
 License: UNKNOWN
 Description: <div align="left">
           <img width="15%" src="/figures/pyrcellmech_logo_v2.png" alt="pycellmech Logo">
```

