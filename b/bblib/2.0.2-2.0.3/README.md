# Comparing `tmp/bblib-2.0.2.tar.gz` & `tmp/bblib-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bblib-2.0.2.tar", max compression
+gzip compressed data, was "bblib-2.0.3.tar", max compression
```

## Comparing `bblib-2.0.2.tar` & `bblib-2.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35146 2024-05-21 16:17:07.517690 bblib-2.0.2/LICENSE
--rw-r--r--   0        0        0     3925 2024-05-21 16:17:07.517690 bblib-2.0.2/README.md
--rw-r--r--   0        0        0        0 2024-05-21 16:17:07.517690 bblib-2.0.2/bblib/__init__.py
--rwxr-xr-x   0        0        0    37411 2024-05-21 16:17:07.517690 bblib-2.0.2/bblib/methods.py
--rwxr-xr-x   0        0        0     9961 2024-05-21 16:17:07.517690 bblib-2.0.2/bblib/models.py
--rwxr-xr-x   0        0        0    18198 2024-05-21 16:17:07.517690 bblib-2.0.2/bblib/utils.py
--rw-r--r--   0        0        0     2104 2024-05-21 16:17:16.305720 bblib-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     7456 1970-01-01 00:00:00.000000 bblib-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35146 2024-05-22 11:06:26.981155 bblib-2.0.3/LICENSE
+-rw-r--r--   0        0        0     3917 2024-05-22 11:06:26.981155 bblib-2.0.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-22 11:06:26.981155 bblib-2.0.3/bblib/__init__.py
+-rwxr-xr-x   0        0        0    37195 2024-05-22 11:06:26.981155 bblib-2.0.3/bblib/methods.py
+-rwxr-xr-x   0        0        0     9961 2024-05-22 11:06:26.981155 bblib-2.0.3/bblib/models.py
+-rwxr-xr-x   0        0        0    18198 2024-05-22 11:06:26.981155 bblib-2.0.3/bblib/utils.py
+-rw-r--r--   0        0        0     2104 2024-05-22 11:06:39.665029 bblib-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     7448 1970-01-01 00:00:00.000000 bblib-2.0.3/PKG-INFO
```

### Comparing `bblib-2.0.2/LICENSE` & `bblib-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bblib-2.0.2/README.md` & `bblib-2.0.3/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,68 +1,60 @@
 # beambusters library
 
-beambusters library. It refines the detector center of diffraction patterns.
+beambusters library. Python library to refine the detector center of diffraction patterns.
+
+For more information, see: https://github.com/anananacr/beambusters
 
 ## Python version
 
 Python 3.10.5 
 
 ## Installation
 pip install bblib
 
 ## Usage
 
-To utilize the methods `CenterOfMass`,  `FriedelPairs`, `MinimizePeakFWHM`  and `CircleDetection` it is required to have two configuration dictionaries, one for PeakFinder8 and another one for this library itself. The follow snippet shows the expected structure for both:
+To utilize the methods `CenterOfMass`,  `FriedelPairs`, `MinimizePeakFWHM`  and `CircleDetection` it is required to have two configuration dictionaries, one for PeakFinder8 and another one for this library itself. The following snippet shows the general structure for both (parameters not used in your case can be omitted):
 
 ```python
 config = {
     "plots_flag": ...,
-	"force_center": {
-		"mode": ...,
-		"x": ...,
-		"y": ...
-		},
 	"search_radius": ...,
 	"pf8": {
 		"max_num_peaks": ...,
 		"adc_threshold": ...,
 		"minimum_snr": ...,
 		"min_pixel_count": ...,
 		"max_pixel_count": ...,
 		"local_bg_radius": ...,
 		"min_res": ...,
 		"max_res": ...
 		},
-	"starting_frame": ...,
 	"offset": {
 		"x": ...,
 		"y": ...
 		},
 	"peak_region":{
 		"min": ...,
 		"max": ...
 		},
-	"outlier_distance": ...,
 	"canny":{
 		"sigma": ...,
 		"low_threshold": ...,
 		"high_threshold": ...
 		},	
-	"method": ...,
 	"bragg_peaks_positions_for_center_of_mass_calculation": ...,
 	"pixels_for_mask_of_bragg_peaks": ...,
-	"skip_methods": ...,
 	"polarization": {
 		"skip": ...,
 		"axis": ...,
 		"value": ...
 		}
 }
 
-
 PF8Info = {
 	"max_num_peaks": 
 	"adc_threshold": 
 	"minimum_snr": ...,
 	"min_pixel_count": ...,
 	"max_pixel_count": ...,
 	"local_bg_radius": ...,
@@ -149,13 +141,13 @@
                     )
 center_coordinates_from_friedel_pairs = friedel_pairs_method(
                         data = ..., initial_guess= ...
                     )
 ```         
 ## Author:
 
-Ana Carolina Rodrigues (2021 - )
+Ana Carolina Rodrigues (2021 - 2024)
 
-email: ana.rodrigues@desy.de
+Email: sc.anarodrigues@gmail.com
```

### Comparing `bblib-2.0.2/bblib/methods.py` & `bblib-2.0.3/bblib/methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -523,18 +523,14 @@
                 self.initial_guess[1] + 21,
                 self.pixel_step,
                 dtype=int,
             ),
         )
         coordinates = np.column_stack((np.ravel(xx), np.ravel(yy)))
 
-        ## TEST avoid effects from secondary peaks
-        # ring_mask_array=ring_mask(masked_data,initial_guess config["peak_region"]["min"], config["peak_region"]["max"])
-        # masked_data[~ring_mask_array]=0
-
         pool = multiprocessing.Pool()
         with pool:
             self.fwhm_summary = pool.map(self._calculate_fwhm, coordinates)
 
     def _run_centering(self, **kwargs) -> tuple:
         if self.config["plots_flag"]:
             path = pathlib.Path(
```

### Comparing `bblib-2.0.2/bblib/models.py` & `bblib-2.0.3/bblib/models.py`

 * *Files identical despite different names*

### Comparing `bblib-2.0.2/bblib/utils.py` & `bblib-2.0.3/bblib/utils.py`

 * *Files identical despite different names*

### Comparing `bblib-2.0.2/pyproject.toml` & `bblib-2.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bblib"
-version = "2.0.2"
+version = "2.0.3"
 description = "beambusters library to refine the detector center for crystallography data processing."
 authors = ["Ana Rodrigues <ana.rodrigues@desy.de>"]
 license = "GNU"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `bblib-2.0.2/PKG-INFO` & `bblib-2.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bblib
-Version: 2.0.2
+Version: 2.0.3
 Summary: beambusters library to refine the detector center for crystallography data processing.
 License: GNU
 Author: Ana Rodrigues
 Author-email: ana.rodrigues@desy.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -95,73 +95,65 @@
 Requires-Dist: urllib3 (==2.2.1)
 Requires-Dist: virtualenv (==20.25.1)
 Requires-Dist: zipp (==3.17.0)
 Description-Content-Type: text/markdown
 
 # beambusters library
 
-beambusters library. It refines the detector center of diffraction patterns.
+beambusters library. Python library to refine the detector center of diffraction patterns.
+
+For more information, see: https://github.com/anananacr/beambusters
 
 ## Python version
 
 Python 3.10.5 
 
 ## Installation
 pip install bblib
 
 ## Usage
 
-To utilize the methods `CenterOfMass`,  `FriedelPairs`, `MinimizePeakFWHM`  and `CircleDetection` it is required to have two configuration dictionaries, one for PeakFinder8 and another one for this library itself. The follow snippet shows the expected structure for both:
+To utilize the methods `CenterOfMass`,  `FriedelPairs`, `MinimizePeakFWHM`  and `CircleDetection` it is required to have two configuration dictionaries, one for PeakFinder8 and another one for this library itself. The following snippet shows the general structure for both (parameters not used in your case can be omitted):
 
 ```python
 config = {
     "plots_flag": ...,
-	"force_center": {
-		"mode": ...,
-		"x": ...,
-		"y": ...
-		},
 	"search_radius": ...,
 	"pf8": {
 		"max_num_peaks": ...,
 		"adc_threshold": ...,
 		"minimum_snr": ...,
 		"min_pixel_count": ...,
 		"max_pixel_count": ...,
 		"local_bg_radius": ...,
 		"min_res": ...,
 		"max_res": ...
 		},
-	"starting_frame": ...,
 	"offset": {
 		"x": ...,
 		"y": ...
 		},
 	"peak_region":{
 		"min": ...,
 		"max": ...
 		},
-	"outlier_distance": ...,
 	"canny":{
 		"sigma": ...,
 		"low_threshold": ...,
 		"high_threshold": ...
 		},	
-	"method": ...,
 	"bragg_peaks_positions_for_center_of_mass_calculation": ...,
 	"pixels_for_mask_of_bragg_peaks": ...,
-	"skip_methods": ...,
 	"polarization": {
 		"skip": ...,
 		"axis": ...,
 		"value": ...
 		}
 }
 
-
 PF8Info = {
 	"max_num_peaks": 
 	"adc_threshold": 
 	"minimum_snr": ...,
 	"min_pixel_count": ...,
 	"max_pixel_count": ...,
 	"local_bg_radius": ...,
@@ -248,14 +240,14 @@
                     )
 center_coordinates_from_friedel_pairs = friedel_pairs_method(
                         data = ..., initial_guess= ...
                     )
 ```         
 ## Author:
 
-Ana Carolina Rodrigues (2021 - )
+Ana Carolina Rodrigues (2021 - 2024)
 
-email: ana.rodrigues@desy.de
+Email: sc.anarodrigues@gmail.com
```

