# Comparing `tmp/msigen-0.2.2rc2.tar.gz` & `tmp/msigen-0.2.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msigen-0.2.2rc2.tar", max compression
+gzip compressed data, was "msigen-0.2.2rc3.tar", max compression
```

## Comparing `msigen-0.2.2rc2.tar` & `msigen-0.2.2rc3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1091 2024-05-16 19:53:18.606091 msigen-0.2.2rc2/LICENSE.txt
--rw-r--r--   0        0        0      178 2024-05-16 19:53:07.444990 msigen-0.2.2rc2/MSIGen/__init__.py
--rw-r--r--   0        0        0    52811 2024-05-21 21:28:04.589990 msigen-0.2.2rc2/MSIGen/D.py
--rw-r--r--   0        0        0    51172 2024-05-21 22:20:05.964509 msigen-0.2.2rc2/MSIGen/GUI.py
--rw-r--r--   0        0        0    58255 2024-05-21 20:55:02.009291 msigen-0.2.2rc2/MSIGen/msigen.py
--rw-r--r--   0        0        0    33676 2024-05-21 20:54:59.311672 msigen-0.2.2rc2/MSIGen/mzml.py
--rw-r--r--   0        0        0    19677 2024-05-21 21:13:04.416726 msigen-0.2.2rc2/MSIGen/raw.py
--rw-r--r--   0        0        0 12886552 2024-04-30 20:20:11.276935 msigen-0.2.2rc2/MSIGen/timsdata.dll
--rw-r--r--   0        0        0     9775 2024-05-16 19:53:12.647190 msigen-0.2.2rc2/MSIGen/tsf.py
--rw-r--r--   0        0        0    22015 2024-05-21 22:23:23.701777 msigen-0.2.2rc2/MSIGen/visualization.py
--rw-r--r--   0        0        0     1323 2024-05-21 22:04:55.945896 msigen-0.2.2rc2/pyproject.toml
--rw-r--r--   0        0        0     2323 2024-05-14 23:34:29.375945 msigen-0.2.2rc2/README.md
--rw-r--r--   0        0        0     3716 1970-01-01 00:00:00.000000 msigen-0.2.2rc2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-05-16 19:53:18.606091 msigen-0.2.2rc3/LICENSE.txt
+-rw-r--r--   0        0        0      178 2024-05-16 19:53:07.444990 msigen-0.2.2rc3/MSIGen/__init__.py
+-rw-r--r--   0        0        0    52811 2024-05-22 15:27:11.046113 msigen-0.2.2rc3/MSIGen/D.py
+-rw-r--r--   0        0        0    51172 2024-05-22 15:27:15.963695 msigen-0.2.2rc3/MSIGen/GUI.py
+-rw-r--r--   0        0        0    58255 2024-05-22 15:27:13.112556 msigen-0.2.2rc3/MSIGen/msigen.py
+-rw-r--r--   0        0        0    33676 2024-05-22 15:27:12.458045 msigen-0.2.2rc3/MSIGen/mzml.py
+-rw-r--r--   0        0        0    19677 2024-05-22 15:27:13.089375 msigen-0.2.2rc3/MSIGen/raw.py
+-rw-r--r--   0        0        0 12886552 2024-04-30 20:20:11.276935 msigen-0.2.2rc3/MSIGen/timsdata.dll
+-rw-r--r--   0        0        0     9775 2024-05-16 19:53:12.647190 msigen-0.2.2rc3/MSIGen/tsf.py
+-rw-r--r--   0        0        0    22255 2024-05-22 15:50:49.963103 msigen-0.2.2rc3/MSIGen/visualization.py
+-rw-r--r--   0        0        0     1323 2024-05-22 16:02:11.565525 msigen-0.2.2rc3/pyproject.toml
+-rw-r--r--   0        0        0     2323 2024-05-14 23:34:29.375945 msigen-0.2.2rc3/README.md
+-rw-r--r--   0        0        0     3716 1970-01-01 00:00:00.000000 msigen-0.2.2rc3/PKG-INFO
```

### Comparing `msigen-0.2.2rc2/LICENSE.txt` & `msigen-0.2.2rc3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `msigen-0.2.2rc2/MSIGen/D.py` & `msigen-0.2.2rc3/MSIGen/D.py`

 * *Files identical despite different names*

### Comparing `msigen-0.2.2rc2/MSIGen/GUI.py` & `msigen-0.2.2rc3/MSIGen/GUI.py`

 * *Files identical despite different names*

### Comparing `msigen-0.2.2rc2/MSIGen/msigen.py` & `msigen-0.2.2rc3/MSIGen/msigen.py`

 * *Files identical despite different names*

### Comparing `msigen-0.2.2rc2/MSIGen/mzml.py` & `msigen-0.2.2rc3/MSIGen/mzml.py`

 * *Files identical despite different names*

### Comparing `msigen-0.2.2rc2/MSIGen/raw.py` & `msigen-0.2.2rc3/MSIGen/raw.py`

 * *Files identical despite different names*

### Comparing `msigen-0.2.2rc2/MSIGen/timsdata.dll` & `msigen-0.2.2rc3/MSIGen/timsdata.dll`

 * *Files identical despite different names*

### Comparing `msigen-0.2.2rc2/MSIGen/tsf.py` & `msigen-0.2.2rc3/MSIGen/tsf.py`

 * *Files identical despite different names*

### Comparing `msigen-0.2.2rc2/MSIGen/visualization.py` & `msigen-0.2.2rc3/MSIGen/visualization.py`

 * *Files 10% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
 def base_peak_normalize_pixels(pixels):
     for i, img in enumerate(pixels):
         if img.max():
             pixels[i]=img/img.max()
     return pixels
 
-def get_and_dispay_images(pixels, metadata, normalize = None, std_idx = None, std_precursor = None, std_mass = None, \
+def get_and_display_images(pixels, metadata, normalize = None, std_idx = None, std_precursor = None, std_mass = None, \
                         std_fragment = None, std_mobility = None, std_charge = None, aspect = None, scale = .999, \
                         how_many_images_to_display = 'all', save_imgs = False, MSI_data_output = None, cmap = 'viridis', \
                         titles = None, threshold = None, title_fontsize = 10, image_savetype = "figure", axis_tick_marks = False):
     pixels_normed = get_pixels_to_display(pixels, metadata, normalize, std_idx, std_precursor, std_mass, std_fragment, std_mobility, std_charge)
     display_images(pixels_normed, metadata, aspect, scale, how_many_images_to_display, save_imgs, MSI_data_output, cmap, titles, threshold, \
                    title_fontsize, image_savetype=image_savetype, axis_tick_marks=axis_tick_marks)
 
@@ -159,18 +159,18 @@
 
     # Get the titles for all figures:
     mass_list = metadata["final_mass_list"]
     
     default_titles = determine_titles(mass_list, idxs = how_many_images_to_display)
 
     # make sure save directory exists
+    if MSI_data_output == None:
+        MSI_data_output = os.getcwd()
+    img_output_folder = os.path.join(MSI_data_output,'images')
     if save_imgs:
-        if MSI_data_output == None:
-            MSI_data_output = os.getcwd()
-        img_output_folder = os.path.join(MSI_data_output,'images')
         if not os.path.exists(img_output_folder):
             os.makedirs(img_output_folder)
 
     # plot each image
     img_height, img_width = metadata['image_dimensions']
     # use manually given aspect ratio
     a = aspect
@@ -234,19 +234,21 @@
 
 # ===========================================================================================
 # fractional abuncance images
 # ===========================================================================================
 
 def fractional_abundance_images(pixels, metadata, idxs = [1,2], normalize = None,titles = None, \
                         aspect = None, save_imgs = False, MSI_data_output = None, cmap = 'viridis', \
-                        title_fontsize = 10, image_savetype = 'figure', scale = 1.0, threshold=None):
+                        title_fontsize = 10, image_savetype = 'figure', scale = 1.0, threshold=None, \
+                        axis_tick_marks=False):
     
     fract_imgs = get_fractional_abundance_imgs(pixels, metadata, idxs, normalize)
     display_fractional_images(fract_imgs, metadata, titles, aspect, save_imgs, MSI_data_output, cmap, \
-                              title_fontsize, idxs, image_savetype=image_savetype, scale=scale, threshold=threshold)
+                              title_fontsize, idxs, image_savetype=image_savetype, scale=scale, \
+                              threshold=threshold, axis_tick_marks=axis_tick_marks)
 
 def get_fractional_abundance_imgs(pixels, metadata, idxs = [1,2], normalize = None):
     normalize = get_normalize_value(normalize, ['None', 'base_peak'])
 
     imgs = [pixels[i] for i in idxs]
 
     # Ensure images are all the same size
@@ -265,24 +267,24 @@
         fract_imgs.append(np.divide(i, img_sum, out=np.zeros_like(i), where=img_sum!=0))
 
     return fract_imgs
 
 def display_fractional_images(fract_imgs, metadata, titles = None, aspect = None,\
                             save_imgs = False, MSI_data_output = None, cmap = 'viridis', \
                             title_fontsize = 10, idxs = [1,2], image_savetype='figure', \
-                            scale = 1.0, threshold = None):    
+                            scale = 1.0, threshold = None, axis_tick_marks=False):    
 
     mass_list = metadata["final_mass_list"]
     default_titles = determine_titles(mass_list, idxs = idxs, fract_abund=True)
 
     # make sure save directory exists
+    if MSI_data_output == None:
+        MSI_data_output = os.getcwd()
+    img_output_folder = os.path.join(MSI_data_output,'images')
     if save_imgs:
-        if MSI_data_output == None:
-            MSI_data_output = os.getcwd()
-        img_output_folder = os.path.join(MSI_data_output,'images')
         if not os.path.exists(img_output_folder):
             os.makedirs(img_output_folder)
 
     if threshold:
         thre = threshold
 
     # plot each image
@@ -305,28 +307,28 @@
         default_title = default_titles[i]
         
         # recalculate aspect ratio for each image in case image sizes are different
         if aspect == None:
             a = (img_height/img.shape[0])/(img_width/img.shape[1])
 
         plot_image(img=img, img_output_folder=img_output_folder, title=title, default_title=default_title, title_fontsize=title_fontsize, \
-                   cmap=cmap, aspect=a, save_imgs=save_imgs, thre=thre, log_scale = False, image_savetype=image_savetype)
+                   cmap=cmap, aspect=a, save_imgs=save_imgs, thre=thre, log_scale = False, image_savetype=image_savetype, axis_tick_marks=axis_tick_marks)
 
 
 # ===========================================================================================
 # ratio images
 # ===========================================================================================
 
 def ratio_images(pixels, metadata, idxs = [1,2], normalize = None, handle_infinity = 'maximum', titles = None, \
                 aspect = None, scale = .999,save_imgs = False, MSI_data_output = None, cmap = 'viridis', \
-                log_scale = False, threshold = None, title_fontsize = 10, image_savetype = 'figure'):
+                log_scale = False, threshold = None, title_fontsize = 10, image_savetype = 'figure',axis_tick_marks=False):
     
     ratio_imgs = get_ratio_imgs(pixels, metadata, idxs, normalize, handle_infinity, titles)
     display_ratio_images(ratio_imgs, metadata, titles, aspect, scale, save_imgs, MSI_data_output, cmap, log_scale, \
-                         threshold, title_fontsize, idxs, image_savetype=image_savetype)
+                         threshold, title_fontsize, idxs, image_savetype=image_savetype, axis_tick_marks=axis_tick_marks)
 
 def get_ratio_imgs(pixels, metadata, idxs = [1,2], normalize = None, handle_infinity = 'maximum', titles = None):
     assert handle_infinity.lower() in ['maximum', 'infinity', 'zero'], "handle_infinity must be in ['maximum', 'infinity', 'zero']"
 
     idxs = idxs[:2]
     normalize = get_normalize_value(normalize, ['None', 'base_peak'])
 
@@ -364,15 +366,15 @@
         ratio_imgs[0][np.isinf(ratio_imgs[0])] = ratio_imgs[0][~np.isinf(ratio_imgs[0])].max()
         ratio_imgs[1][np.isinf(ratio_imgs[0])] = ratio_imgs[1][~np.isinf(ratio_imgs[1])].max()
 
     return ratio_imgs
 
 def display_ratio_images(ratio_imgs, metadata, titles = None, aspect = None, scale = .999,save_imgs = False, \
                          MSI_data_output = None, cmap = 'viridis', log_scale = False, threshold = None, \
-                         title_fontsize = 10, idxs = [1,2], image_savetype = 'figure'):    
+                         title_fontsize = 10, idxs = [1,2], image_savetype = 'figure', axis_tick_marks=False):    
 
     mass_list = metadata["final_mass_list"]
     default_titles = determine_titles(mass_list, idxs = idxs, ratio_img = True)
 
     # make sure save directory exists
     if MSI_data_output == None:
         MSI_data_output = os.getcwd()
@@ -404,15 +406,15 @@
             thre = img.max()
 
         # recalculate aspect ratio for each image in case image sizes are different
         if aspect == None:
             a = (img_height/img.shape[0])/(img_width/img.shape[1])
 
         plot_image(img=img, img_output_folder=img_output_folder, title=title, default_title=default_title, title_fontsize=title_fontsize, \
-                   cmap=cmap, aspect=a, save_imgs=save_imgs, thre=thre, log_scale = log_scale, image_savetype=image_savetype)
+                   cmap=cmap, aspect=a, save_imgs=save_imgs, thre=thre, log_scale = log_scale, image_savetype=image_savetype, axis_tick_marks=axis_tick_marks)
 
 def plot_image(img, img_output_folder, title, default_title, title_fontsize, cmap, aspect, save_imgs, thre, \
     log_scale = False, image_savetype='figure', axis_tick_marks = False):
 
     # Save images as publication-style figure, including a colorbar and title
     if image_savetype == 'figure':
         plt.figure(figsize=(6,6))
@@ -457,21 +459,21 @@
         normed_img = (img-img.min())/(img.max()-img.min())
         colored_img = cm(normed_img)
         colored_img = (colored_img[:,:,:3]*255).astype(np.uint8)
         
         # get dimensions for resizing
         h, w = colored_img.shape[:2]
         
-        if save_imgs:
-            pil_img = Image.fromarray(colored_img)
-            if aspect >=1:
-                pil_img = pil_img.resize((w, round(h*aspect)), resample=0)
-            else:
-                pil_img = pil_img.resize((w//aspect, h), resample=0)
+        pil_img = Image.fromarray(colored_img)
+        if aspect >=1:
+            pil_img = pil_img.resize((w, round(h*aspect)), resample=0)
+        else:
+            pil_img = pil_img.resize((w//aspect, h), resample=0)
 
+        if save_imgs:
             try:
                 pil_img.save(os.path.join(img_output_folder,title.replace(':','_').replace('\n',' ').replace('>','').replace('/','')+"_threshold-"+str(thre)+'.png') )
             except:
                 pil_img.save(os.path.join(img_output_folder,default_title.replace(':','_').replace('\n',' ').replace('>','').replace('/','')+"_threshold-"+str(thre)+'.png') )
         else:
             fig, ax = plt.subplots()
             ax.axis('off')
```

### Comparing `msigen-0.2.2rc2/pyproject.toml` & `msigen-0.2.2rc3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msigen"
-version = "0.2.2rc2"
+version = "0.2.2rc3"
 description = "A package for converting spectrometry imaging line scan data files to a visualizable format"
 authors = ["Emerson Hernly <elhernly@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/LabLaskin/MSIGen"
 homepage = "https://github.com/LabLaskin/MSIGen"
```

### Comparing `msigen-0.2.2rc2/README.md` & `msigen-0.2.2rc3/README.md`

 * *Files identical despite different names*

### Comparing `msigen-0.2.2rc2/PKG-INFO` & `msigen-0.2.2rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msigen
-Version: 0.2.2rc2
+Version: 0.2.2rc3
 Summary: A package for converting spectrometry imaging line scan data files to a visualizable format
 Home-page: https://github.com/LabLaskin/MSIGen
 License: MIT
 Author: Emerson Hernly
 Author-email: elhernly@gmail.com
 Requires-Python: >=3.9.0,<3.12
 Classifier: Development Status :: 4 - Beta
```

