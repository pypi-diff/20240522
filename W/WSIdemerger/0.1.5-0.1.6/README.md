# Comparing `tmp/wsidemerger-0.1.5.tar.gz` & `tmp/wsidemerger-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wsidemerger-0.1.5.tar", last modified: Wed May 22 19:52:42 2024, max compression
+gzip compressed data, was "wsidemerger-0.1.6.tar", last modified: Wed May 22 20:21:39 2024, max compression
```

## Comparing `wsidemerger-0.1.5.tar` & `wsidemerger-0.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 19:52:42.349657 wsidemerger-0.1.5/
--rw-rw-rw-   0        0        0     1086 2024-05-22 19:45:50.000000 wsidemerger-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       19 2024-05-22 19:45:50.000000 wsidemerger-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     3476 2024-05-22 19:52:42.348661 wsidemerger-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     2744 2024-05-22 19:45:50.000000 wsidemerger-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 19:52:42.318740 wsidemerger-0.1.5/WSIdemerger/
--rw-rw-rw-   0        0        0     1135 2024-05-22 19:45:50.000000 wsidemerger-0.1.5/WSIdemerger/Colour_standardisation.py
--rw-rw-rw-   0        0        0     2890 2024-05-22 19:45:51.000000 wsidemerger-0.1.5/WSIdemerger/Patches_generation.py
--rw-rw-rw-   0        0        0       93 2024-05-22 19:45:51.000000 wsidemerger-0.1.5/WSIdemerger/__init__.py
--rw-rw-rw-   0        0        0     1688 2024-05-22 19:45:51.000000 wsidemerger-0.1.5/WSIdemerger/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-22 19:52:42.346666 wsidemerger-0.1.5/WSIdemerger.egg-info/
--rw-rw-rw-   0        0        0     3476 2024-05-22 19:52:42.000000 wsidemerger-0.1.5/WSIdemerger.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      329 2024-05-22 19:52:42.000000 wsidemerger-0.1.5/WSIdemerger.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 19:52:42.000000 wsidemerger-0.1.5/WSIdemerger.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-22 19:52:42.000000 wsidemerger-0.1.5/WSIdemerger.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-22 19:52:42.000000 wsidemerger-0.1.5/WSIdemerger.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 19:52:42.349657 wsidemerger-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1123 2024-05-22 19:48:55.000000 wsidemerger-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:21:39.799655 wsidemerger-0.1.6/
+-rw-rw-rw-   0        0        0     1086 2024-05-22 20:20:43.000000 wsidemerger-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       19 2024-05-22 20:20:43.000000 wsidemerger-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     3476 2024-05-22 20:21:39.797659 wsidemerger-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2744 2024-05-22 20:20:43.000000 wsidemerger-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 20:21:39.770730 wsidemerger-0.1.6/WSIdemerger/
+-rw-rw-rw-   0        0        0     1107 2024-05-22 20:20:44.000000 wsidemerger-0.1.6/WSIdemerger/Colour_standardisation.py
+-rw-rw-rw-   0        0        0     2825 2024-05-22 20:20:44.000000 wsidemerger-0.1.6/WSIdemerger/Patches_generation.py
+-rw-rw-rw-   0        0        0       93 2024-05-22 20:20:44.000000 wsidemerger-0.1.6/WSIdemerger/__init__.py
+-rw-rw-rw-   0        0        0     1640 2024-05-22 20:20:44.000000 wsidemerger-0.1.6/WSIdemerger/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 20:21:39.796661 wsidemerger-0.1.6/WSIdemerger.egg-info/
+-rw-rw-rw-   0        0        0     3476 2024-05-22 20:21:39.000000 wsidemerger-0.1.6/WSIdemerger.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2024-05-22 20:21:39.000000 wsidemerger-0.1.6/WSIdemerger.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 20:21:39.000000 wsidemerger-0.1.6/WSIdemerger.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-22 20:21:39.000000 wsidemerger-0.1.6/WSIdemerger.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-22 20:21:39.000000 wsidemerger-0.1.6/WSIdemerger.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 20:21:39.799655 wsidemerger-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1086 2024-05-22 20:20:44.000000 wsidemerger-0.1.6/setup.py
```

### Comparing `wsidemerger-0.1.5/LICENSE` & `wsidemerger-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `wsidemerger-0.1.5/PKG-INFO` & `wsidemerger-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WSIdemerger
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for extracting image patches from SVS files and performing color normalization
 Home-page: https://github.com/yourusername/WSI_Preprocessing
 Author: Thirteen
 Author-email: 506607814@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `wsidemerger-0.1.5/README.md` & `wsidemerger-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `wsidemerger-0.1.5/WSIdemerger/Colour_standardisation.py` & `wsidemerger-0.1.6/WSIdemerger/Colour_standardisation.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# WSIdemerger/Colour_standardisation.py
-import os
-import cv2
-import staintools
-from pathlib import Path
-from tqdm import tqdm
-
-def normalize_images(input_folder, reference_image_path, output_folder):
-    if not os.path.exists(output_folder):
-        os.makedirs(output_folder)
-
-    reference_image = staintools.read_image(reference_image_path)
-    reference_image = staintools.LuminosityStandardizer.standardize(reference_image)
-
-    normalizer = staintools.StainNormalizer(method='vahadane')
-    normalizer.fit(reference_image)
-
-    image_files = [p for p in Path(input_folder).rglob('*.png')]
-
-    for image_path in tqdm(image_files, desc="Processing Images"):
-        image = staintools.read_image(str(image_path))
-        image = staintools.LuminosityStandardizer.standardize(image)
-        normalized_image = normalizer.transform(image)
-
-        relative_path = image_path.relative_to(input_folder)
-        save_path = Path(output_folder) / relative_path
-        save_path.parent.mkdir(parents=True, exist_ok=True)
-        cv2.imwrite(str(save_path), cv2.cvtColor(normalized_image, cv2.COLOR_RGB2BGR))
+# WSIdemerger/Colour_standardisation.py
+import os
+import cv2
+import staintools
+from pathlib import Path
+from tqdm import tqdm
+
+def normalize_images(input_folder, reference_image_path, output_folder):
+    if not os.path.exists(output_folder):
+        os.makedirs(output_folder)
+
+    reference_image = staintools.read_image(reference_image_path)
+    reference_image = staintools.LuminosityStandardizer.standardize(reference_image)
+
+    normalizer = staintools.StainNormalizer(method='vahadane')
+    normalizer.fit(reference_image)
+
+    image_files = [p for p in Path(input_folder).rglob('*.png')]
+
+    for image_path in tqdm(image_files, desc="Processing Images"):
+        image = staintools.read_image(str(image_path))
+        image = staintools.LuminosityStandardizer.standardize(image)
+        normalized_image = normalizer.transform(image)
+
+        relative_path = image_path.relative_to(input_folder)
+        save_path = Path(output_folder) / relative_path
+        save_path.parent.mkdir(parents=True, exist_ok=True)
+        cv2.imwrite(str(save_path), cv2.cvtColor(normalized_image, cv2.COLOR_RGB2BGR))
```

### Comparing `wsidemerger-0.1.5/WSIdemerger/Patches_generation.py` & `wsidemerger-0.1.6/WSIdemerger/Patches_generation.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-# WSIdemerger/Patches_generation.py
-import os
-import pandas as pd
-import openslide
-from PIL import Image
-import numpy as np
-from skimage.color import rgb2hsv
-from skimage import img_as_ubyte
-import shutil
-import logging
-import time
-from .utils import calculate_saturation, clear_output_directory, select_level_by_magnification
-
-def extract_patches_from_svs(input_path, output_path, excel_path, patch_size=512, target_magnification=20, saturation_threshold=50):
-    slide = openslide.OpenSlide(input_path)
-    level = select_level_by_magnification(slide, target_magnification)
-    level_downsample = slide.level_downsamples[level]
-    width, height = slide.level_dimensions[level]
-
-    if not os.path.exists(output_path):
-        os.makedirs(output_path)
-
-    data = []
-    num_patches = 0
-
-    for x in range(0, width - patch_size + 1, patch_size):
-        for y in range(0, height - patch_size + 1, patch_size):
-            patch = slide.read_region((int(x * level_downsample), int(y * level_downsample)), level,
-                                      (patch_size, patch_size)).convert('RGB')
-            saturation = calculate_saturation(patch)
-            patch_name = f'patch_{x}_{y}.png'
-            is_saved = saturation >= saturation_threshold
-
-            if is_saved:
-                patch.save(os.path.join(output_path, patch_name))
-                num_patches += 1
-
-            data.append([patch_name, saturation, is_saved])
-
-    df = pd.DataFrame(data, columns=['Patch Name', 'Saturation', 'Saved'])
-    df.to_excel(excel_path, index=False)
-
-    slide.close()
-
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
-        try:
-            extract_patches_from_svs(svs_file, output_path, excel_path, patch_size, target_magnification, saturation_threshold)
-        except Exception as e:
-            logging.error(f'处理文件 {svs_file} 时出现错误: {str(e)}')
-
-        print(f'已处理 {index + 1}/{total_files} 文件，占总进度的 {(index + 1) / total_files * 100:.2f}%')
-
-    total_elapsed_time = time.time() - start_time
-    print(f'所有文件已处理完成，总耗时 {total_elapsed_time / 60:.2f} 分钟。')
+# WSIdemerger/Patches_generation.py
+import os
+import pandas as pd
+import openslide
+from PIL import Image
+import numpy as np
+from skimage.color import rgb2hsv
+from skimage import img_as_ubyte
+import shutil
+import logging
+import time
+from .utils import calculate_saturation, clear_output_directory, select_level_by_magnification
+
+def extract_patches_from_svs(input_path, output_path, excel_path, patch_size=512, target_magnification=20, saturation_threshold=50):
+    slide = openslide.OpenSlide(input_path)
+    level = select_level_by_magnification(slide, target_magnification)
+    level_downsample = slide.level_downsamples[level]
+    width, height = slide.level_dimensions[level]
+
+    if not os.path.exists(output_path):
+        os.makedirs(output_path)
+
+    data = []
+    num_patches = 0
+
+    for x in range(0, width - patch_size + 1, patch_size):
+        for y in range(0, height - patch_size + 1, patch_size):
+            patch = slide.read_region((int(x * level_downsample), int(y * level_downsample)), level,
+                                      (patch_size, patch_size)).convert('RGB')
+            saturation = calculate_saturation(patch)
+            patch_name = f'patch_{x}_{y}.png'
+            is_saved = saturation >= saturation_threshold
+
+            if is_saved:
+                patch.save(os.path.join(output_path, patch_name))
+                num_patches += 1
+
+            data.append([patch_name, saturation, is_saved])
+
+    df = pd.DataFrame(data, columns=['Patch Name', 'Saturation', 'Saved'])
+    df.to_excel(excel_path, index=False)
+
+    slide.close()
+
+def process_svs_files(base_path, output_base, saturation_threshold, patch_size, target_magnification):
+    logging.basicConfig(filename=os.path.join(output_base, 'error_log.txt'), level=logging.ERROR)
+    svs_files = [os.path.join(dp, f) for dp, dn, filenames in os.walk(base_path) for f in filenames if f.endswith('.svs')]
+    total_files = len(svs_files)
+    start_time = time.time()
+
+    for index, svs_file in enumerate(svs_files):
+        current_file_start_time = time.time()
+        folder_name = os.path.basename(os.path.dirname(svs_file))
+        output_path = os.path.join(output_base, folder_name)
+        excel_path = os.path.join(output_path, f'{folder_name}_patches_info.xlsx')
+        clear_output_directory(output_path)
+        try:
+            extract_patches_from_svs(svs_file, output_path, excel_path, patch_size, target_magnification, saturation_threshold)
+        except Exception as e:
+            logging.error(f'处理文件 {svs_file} 时出现错误: {str(e)}')
+
+        print(f'已处理 {index + 1}/{total_files} 文件，占总进度的 {(index + 1) / total_files * 100:.2f}%')
+
+    total_elapsed_time = time.time() - start_time
+    print(f'所有文件已处理完成，总耗时 {total_elapsed_time / 60:.2f} 分钟。')
```

### Comparing `wsidemerger-0.1.5/WSIdemerger/utils.py` & `wsidemerger-0.1.6/WSIdemerger/utils.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-# WSIdemerger/utils.py
-import numpy as np
-from skimage.color import rgb2hsv
-from skimage import img_as_ubyte
-import os
-import shutil
-import logging
-
-def calculate_saturation(patch):
-    patch_array = np.array(patch)
-    hsv_patch = rgb2hsv(patch_array)
-    saturation_channel = hsv_patch[:, :, 1]
-    saturation_channel_0_255 = img_as_ubyte(saturation_channel)
-    return np.mean(saturation_channel_0_255)
-
-def clear_output_directory(output_path):
-    if not os.path.exists(output_path):
-        os.makedirs(output_path)
-    else:
-        for filename in os.listdir(output_path):
-            file_path = os.path.join(output_path, filename)
-            try:
-                if os.path.isfile(file_path) or os.path.islink(file_path):
-                    os.unlink(file_path)
-                elif os.path.isdir(file_path):
-                    shutil.rmtree(file_path)
-            except Exception as e:
-                logging.error(f'Failed to delete {file_path}. Reason: {str(e)}')
-
-def select_level_by_magnification(slide, target_magnification):
-    best_level = 0
-    min_diff = float('inf')
-    for i, downsample in enumerate(slide.level_downsamples):
-        try:
-            objective_power = float(slide.properties['openslide.objective-power'])
-            current_magnification = objective_power / downsample
-            magnification_diff = abs(current_magnification - target_magnification)
-
-            if magnification_diff < min_diff:
-                min_diff = magnification_diff
-                best_level = i
-        except KeyError:
-            continue
-        except ValueError:
-            continue
-
-    return best_level
-
+# WSIdemerger/utils.py
+import numpy as np
+from skimage.color import rgb2hsv
+from skimage import img_as_ubyte
+import os
+import shutil
+import logging
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
+
+def select_level_by_magnification(slide, target_magnification):
+    best_level = 0
+    min_diff = float('inf')
+    for i, downsample in enumerate(slide.level_downsamples):
+        try:
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
+
+    return best_level
+
```

### Comparing `wsidemerger-0.1.5/WSIdemerger.egg-info/PKG-INFO` & `wsidemerger-0.1.6/WSIdemerger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: WSIdemerger
-Version: 0.1.5
+Version: 0.1.6
 Summary: A package for extracting image patches from SVS files and performing color normalization
 Home-page: https://github.com/yourusername/WSI_Preprocessing
 Author: Thirteen
 Author-email: 506607814@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

