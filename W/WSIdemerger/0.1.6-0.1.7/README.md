# Comparing `tmp/wsidemerger-0.1.6.tar.gz` & `tmp/wsidemerger-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsidemerger-0.1.6.tar", last modified: Wed May 22 20:21:39 2024, max compression
+gzip compressed data, was "wsidemerger-0.1.7.tar", last modified: Wed May 22 20:47:43 2024, max compression
```

## Comparing `wsidemerger-0.1.6.tar` & `wsidemerger-0.1.7.tar`

### file list

```diff
@@ -1,18 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 20:21:39.799655 wsidemerger-0.1.6/
--rw-rw-rw-   0        0        0     1086 2024-05-22 20:20:43.000000 wsidemerger-0.1.6/LICENSE
--rw-rw-rw-   0        0        0       19 2024-05-22 20:20:43.000000 wsidemerger-0.1.6/MANIFEST.in
--rw-rw-rw-   0        0        0     3476 2024-05-22 20:21:39.797659 wsidemerger-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     2744 2024-05-22 20:20:43.000000 wsidemerger-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 20:21:39.770730 wsidemerger-0.1.6/WSIdemerger/
--rw-rw-rw-   0        0        0     1107 2024-05-22 20:20:44.000000 wsidemerger-0.1.6/WSIdemerger/Colour_standardisation.py
--rw-rw-rw-   0        0        0     2825 2024-05-22 20:20:44.000000 wsidemerger-0.1.6/WSIdemerger/Patches_generation.py
--rw-rw-rw-   0        0        0       93 2024-05-22 20:20:44.000000 wsidemerger-0.1.6/WSIdemerger/__init__.py
--rw-rw-rw-   0        0        0     1640 2024-05-22 20:20:44.000000 wsidemerger-0.1.6/WSIdemerger/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-22 20:21:39.796661 wsidemerger-0.1.6/WSIdemerger.egg-info/
--rw-rw-rw-   0        0        0     3476 2024-05-22 20:21:39.000000 wsidemerger-0.1.6/WSIdemerger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-22 20:21:39.000000 wsidemerger-0.1.6/WSIdemerger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 20:21:39.000000 wsidemerger-0.1.6/WSIdemerger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-22 20:21:39.000000 wsidemerger-0.1.6/WSIdemerger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-22 20:21:39.000000 wsidemerger-0.1.6/WSIdemerger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 20:21:39.799655 wsidemerger-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1086 2024-05-22 20:20:44.000000 wsidemerger-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:47:43.229804 wsidemerger-0.1.7/
+-rw-rw-rw-   0        0        0     1049 2024-05-22 20:46:23.000000 wsidemerger-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     1723 2024-05-22 20:47:43.228805 wsidemerger-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      952 2024-05-22 20:46:23.000000 wsidemerger-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 20:47:43.205866 wsidemerger-0.1.7/WSIdemerger/
+-rw-rw-rw-   0        0        0     1070 2024-05-22 20:46:23.000000 wsidemerger-0.1.7/WSIdemerger/Colour_standardisation.py
+-rw-rw-rw-   0        0        0     2921 2024-05-22 20:46:23.000000 wsidemerger-0.1.7/WSIdemerger/Patches_generation.py
+-rw-rw-rw-   0        0        0       22 2024-05-22 20:46:23.000000 wsidemerger-0.1.7/WSIdemerger/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:47:43.227810 wsidemerger-0.1.7/WSIdemerger.egg-info/
+-rw-rw-rw-   0        0        0     1723 2024-05-22 20:47:43.000000 wsidemerger-0.1.7/WSIdemerger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2024-05-22 20:47:43.000000 wsidemerger-0.1.7/WSIdemerger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 20:47:43.000000 wsidemerger-0.1.7/WSIdemerger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-22 20:47:43.000000 wsidemerger-0.1.7/WSIdemerger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-22 20:47:43.000000 wsidemerger-0.1.7/WSIdemerger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 20:47:43.229804 wsidemerger-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1031 2024-05-22 20:46:23.000000 wsidemerger-0.1.7/setup.py
```

### Comparing `wsidemerger-0.1.6/LICENSE` & `wsidemerger-0.1.7/LICENSE`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,9 @@
-MIT License
-
-Copyright (c) 2024 Thirteen
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+
+MIT License
+===========
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `wsidemerger-0.1.6/WSIdemerger/Colour_standardisation.py` & `wsidemerger-0.1.7/WSIdemerger/Colour_standardisation.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# WSIdemerger/Colour_standardisation.py
+
 import os
 import cv2
 import staintools
 from pathlib import Path
 from tqdm import tqdm
 
 def normalize_images(input_folder, reference_image_path, output_folder):
@@ -20,9 +20,11 @@
     for image_path in tqdm(image_files, desc="Processing Images"):
         image = staintools.read_image(str(image_path))
         image = staintools.LuminosityStandardizer.standardize(image)
         normalized_image = normalizer.transform(image)
 
         relative_path = image_path.relative_to(input_folder)
         save_path = Path(output_folder) / relative_path
+
         save_path.parent.mkdir(parents=True, exist_ok=True)
+
         cv2.imwrite(str(save_path), cv2.cvtColor(normalized_image, cv2.COLOR_RGB2BGR))
```

### Comparing `wsidemerger-0.1.6/WSIdemerger/Patches_generation.py` & `wsidemerger-0.1.7/WSIdemerger/Patches_generation.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,38 @@
-# WSIdemerger/Patches_generation.py
+
 import os
 import pandas as pd
 import openslide
 from PIL import Image
 import numpy as np
 from skimage.color import rgb2hsv
 from skimage import img_as_ubyte
 import shutil
 import logging
-import time
-from .utils import calculate_saturation, clear_output_directory, select_level_by_magnification
+
+def calculate_saturation(patch):
+    patch_array = np.array(patch)
+    hsv_patch = rgb2hsv(patch_array)
+    saturation_channel = hsv_patch[:, :, 1]
+    saturation_channel_0_255 = img_as_ubyte(saturation_channel)
+    return np.mean(saturation_channel_0_255)
+
+def clear_output_directory(output_path):
+    if not os.path.exists(output_path):
+        os.makedirs(output_path)
+    else:
+        for filename in os.listdir(output_path):
+            file_path = os.path.join(output_path, filename)
+            try:
+                if os.path.isfile(file_path) or os.path.islink(file_path):
+                    os.unlink(file_path)
+                elif os.path.isdir(file_path):
+                    shutil.rmtree(file_path)
+            except Exception as e:
+                logging.error(f'Failed to delete {file_path}. Reason: {str(e)}')
 
 def extract_patches_from_svs(input_path, output_path, excel_path, patch_size=512, target_magnification=20, saturation_threshold=50):
     slide = openslide.OpenSlide(input_path)
     level = select_level_by_magnification(slide, target_magnification)
     level_downsample = slide.level_downsamples[level]
     width, height = slide.level_dimensions[level]
 
@@ -38,28 +57,25 @@
             data.append([patch_name, saturation, is_saved])
 
     df = pd.DataFrame(data, columns=['Patch Name', 'Saturation', 'Saved'])
     df.to_excel(excel_path, index=False)
 
     slide.close()
 
-def process_svs_files(base_path, output_base, saturation_threshold, patch_size, target_magnification):
-    logging.basicConfig(filename=os.path.join(output_base, 'error_log.txt'), level=logging.ERROR)
-    svs_files = [os.path.join(dp, f) for dp, dn, filenames in os.walk(base_path) for f in filenames if f.endswith('.svs')]
-    total_files = len(svs_files)
-    start_time = time.time()
-
-    for index, svs_file in enumerate(svs_files):
-        current_file_start_time = time.time()
-        folder_name = os.path.basename(os.path.dirname(svs_file))
-        output_path = os.path.join(output_base, folder_name)
-        excel_path = os.path.join(output_path, f'{folder_name}_patches_info.xlsx')
-        clear_output_directory(output_path)
+def select_level_by_magnification(slide, target_magnification):
+    best_level = 0
+    min_diff = float('inf')
+    for i, downsample in enumerate(slide.level_downsamples):
         try:
-            extract_patches_from_svs(svs_file, output_path, excel_path, patch_size, target_magnification, saturation_threshold)
-        except Exception as e:
-            logging.error(f'处理文件 {svs_file} 时出现错误: {str(e)}')
-
-        print(f'已处理 {index + 1}/{total_files} 文件，占总进度的 {(index + 1) / total_files * 100:.2f}%')
+            objective_power = float(slide.properties['openslide.objective-power'])
+            current_magnification = objective_power / downsample
+            magnification_diff = abs(current_magnification - target_magnification)
+
+            if magnification_diff < min_diff:
+                min_diff = magnification_diff
+                best_level = i
+        except KeyError:
+            continue
+        except ValueError:
+            continue
 
-    total_elapsed_time = time.time() - start_time
-    print(f'所有文件已处理完成，总耗时 {total_elapsed_time / 60:.2f} 分钟。')
+    return best_level
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `wsidemerger-0.1.6/setup.py` & `wsidemerger-0.1.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,20 @@
+
 from setuptools import setup, find_packages
 import os
 
 def read(file_name):
     try:
         return open(os.path.join(os.path.dirname(__file__), file_name)).read()
     except FileNotFoundError:
         return ""
 
 setup(
     name='WSIdemerger',
-    version='0.1.6',  # 更新版本号
+    version='0.1.7',
     packages=find_packages(),
     install_requires=[
         'pandas',
         'openslide-python',
         'Pillow',
         'numpy',
         'scikit-image',
@@ -22,15 +23,15 @@
         'staintools'
     ],
     author='Thirteen',
     author_email='506607814@qq.com',
     description='A package for extracting image patches from SVS files and performing color normalization',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
-    url='https://github.com/yourusername/WSI_Preprocessing',  # 替换为你的GitHub仓库地址
+    url='https://github.com/yourusername/WSI_Preprocessing',
     license='MIT',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.6',
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

