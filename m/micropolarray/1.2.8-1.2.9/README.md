# Comparing `tmp/micropolarray-1.2.8.tar.gz` & `tmp/micropolarray-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "micropolarray-1.2.8.tar", last modified: Thu Feb  1 09:54:51 2024, max compression
+gzip compressed data, was "micropolarray-1.2.9.tar", last modified: Thu Feb  8 09:50:11 2024, max compression
```

## Comparing `micropolarray-1.2.8.tar` & `micropolarray-1.2.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2024-02-01 09:54:51.678266 micropolarray-1.2.8/
--rw-rw-r--   0 herve     (1000) herve     (1000)     1494 2023-02-09 16:24:14.000000 micropolarray-1.2.8/LICENSE
--rw-r--r--   0 herve     (1000) herve     (1000)     5006 2024-02-01 09:54:51.678266 micropolarray-1.2.8/PKG-INFO
--rw-rw-r--   0 herve     (1000) herve     (1000)     2027 2023-09-19 13:29:11.000000 micropolarray-1.2.8/README.md
-drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2024-02-01 09:54:51.674266 micropolarray-1.2.8/micropolarray/
--rw-rw-r--   0 herve     (1000) herve     (1000)     1858 2024-02-01 09:13:25.000000 micropolarray-1.2.8/micropolarray/__init__.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     4279 2024-01-30 16:49:45.000000 micropolarray-1.2.8/micropolarray/cameras.py
--rw-rw-r--   0 herve     (1000) herve     (1000)    10139 2024-01-05 11:03:49.000000 micropolarray-1.2.8/micropolarray/image.py
--rw-rw-r--   0 herve     (1000) herve     (1000)    37044 2024-01-26 16:17:38.000000 micropolarray-1.2.8/micropolarray/micropol_image.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     2645 2023-10-18 09:48:08.000000 micropolarray-1.2.8/micropolarray/polarization_functions.py
-drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2024-02-01 09:54:51.678266 micropolarray-1.2.8/micropolarray/processing/
--rw-rw-r--   0 herve     (1000) herve     (1000)       13 2023-02-09 16:24:14.000000 micropolarray-1.2.8/micropolarray/processing/__init__.py
--rw-rw-r--   0 herve     (1000) herve     (1000)    11217 2023-09-22 14:07:13.000000 micropolarray-1.2.8/micropolarray/processing/chen_wan_liang_calibration.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     2080 2023-09-22 10:11:31.000000 micropolarray-1.2.8/micropolarray/processing/congrid.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     7118 2023-12-18 13:33:05.000000 micropolarray-1.2.8/micropolarray/processing/convert.py
--rw-rw-r--   0 herve     (1000) herve     (1000)    39607 2024-01-26 10:28:57.000000 micropolarray-1.2.8/micropolarray/processing/demodulation.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     2732 2024-01-16 17:55:04.000000 micropolarray-1.2.8/micropolarray/processing/demodulation_errors.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     5355 2024-01-26 16:48:35.000000 micropolarray-1.2.8/micropolarray/processing/demosaic.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     3342 2024-02-01 09:52:21.000000 micropolarray-1.2.8/micropolarray/processing/image_cleaning.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     6162 2024-02-01 08:29:23.000000 micropolarray-1.2.8/micropolarray/processing/linear_roi.py
--rw-rw-r--   0 herve     (1000) herve     (1000)    13011 2024-02-01 09:12:03.000000 micropolarray-1.2.8/micropolarray/processing/nrgf.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     5485 2024-01-24 15:00:55.000000 micropolarray-1.2.8/micropolarray/processing/rebin.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     1134 2023-10-16 08:25:34.000000 micropolarray-1.2.8/micropolarray/processing/shift.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     8693 2024-01-26 15:35:46.000000 micropolarray-1.2.8/micropolarray/utils.py
-drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2024-02-01 09:54:51.678266 micropolarray-1.2.8/micropolarray.egg-info/
--rw-r--r--   0 herve     (1000) herve     (1000)     5006 2024-02-01 09:54:51.000000 micropolarray-1.2.8/micropolarray.egg-info/PKG-INFO
--rw-rw-r--   0 herve     (1000) herve     (1000)     1494 2024-02-01 09:54:51.000000 micropolarray-1.2.8/micropolarray.egg-info/SOURCES.txt
--rw-rw-r--   0 herve     (1000) herve     (1000)        1 2024-02-01 09:54:51.000000 micropolarray-1.2.8/micropolarray.egg-info/dependency_links.txt
--rw-rw-r--   0 herve     (1000) herve     (1000)      171 2024-02-01 09:54:51.000000 micropolarray-1.2.8/micropolarray.egg-info/requires.txt
--rw-rw-r--   0 herve     (1000) herve     (1000)       14 2024-02-01 09:54:51.000000 micropolarray-1.2.8/micropolarray.egg-info/top_level.txt
--rw-rw-r--   0 herve     (1000) herve     (1000)     1111 2024-02-01 09:53:19.000000 micropolarray-1.2.8/pyproject.toml
--rw-rw-r--   0 herve     (1000) herve     (1000)       38 2024-02-01 09:54:51.678266 micropolarray-1.2.8/setup.cfg
--rw-rw-r--   0 herve     (1000) herve     (1000)      643 2023-09-26 10:29:37.000000 micropolarray-1.2.8/setup.py
-drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2024-02-01 09:54:51.678266 micropolarray-1.2.8/tests/
--rw-rw-r--   0 herve     (1000) herve     (1000)     8679 2024-01-30 11:40:12.000000 micropolarray-1.2.8/tests/test_demodulation.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     7806 2024-01-26 16:47:03.000000 micropolarray-1.2.8/tests/test_image_and_micropolimage.py
--rw-rw-r--   0 herve     (1000) herve     (1000)     2282 2023-09-29 10:43:34.000000 micropolarray-1.2.8/tests/test_utils.py
+drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2024-02-08 09:50:11.413042 micropolarray-1.2.9/
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1494 2023-02-09 16:24:14.000000 micropolarray-1.2.9/LICENSE
+-rw-r--r--   0 herve     (1000) herve     (1000)     5080 2024-02-08 09:50:11.413042 micropolarray-1.2.9/PKG-INFO
+-rw-rw-r--   0 herve     (1000) herve     (1000)     2101 2024-02-08 09:31:20.000000 micropolarray-1.2.9/README.md
+drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2024-02-08 09:50:11.409042 micropolarray-1.2.9/micropolarray/
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1858 2024-02-08 09:29:16.000000 micropolarray-1.2.9/micropolarray/__init__.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     4279 2024-01-30 16:49:45.000000 micropolarray-1.2.9/micropolarray/cameras.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     9861 2024-02-05 14:39:29.000000 micropolarray-1.2.9/micropolarray/image.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)    38119 2024-02-07 10:08:04.000000 micropolarray-1.2.9/micropolarray/micropol_image.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     2645 2023-10-18 09:48:08.000000 micropolarray-1.2.9/micropolarray/polarization_functions.py
+drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2024-02-08 09:50:11.413042 micropolarray-1.2.9/micropolarray/processing/
+-rw-rw-r--   0 herve     (1000) herve     (1000)       43 2024-02-08 09:08:33.000000 micropolarray-1.2.9/micropolarray/processing/__init__.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)    11217 2023-09-22 14:07:13.000000 micropolarray-1.2.9/micropolarray/processing/chen_wan_liang_calibration.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     2080 2023-09-22 10:11:31.000000 micropolarray-1.2.9/micropolarray/processing/congrid.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     7118 2023-12-18 13:33:05.000000 micropolarray-1.2.9/micropolarray/processing/convert.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)    40016 2024-02-02 16:07:01.000000 micropolarray-1.2.9/micropolarray/processing/demodulation.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     2732 2024-01-16 17:55:04.000000 micropolarray-1.2.9/micropolarray/processing/demodulation_errors.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     5355 2024-01-26 16:48:35.000000 micropolarray-1.2.9/micropolarray/processing/demosaic.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     3342 2024-02-01 09:52:21.000000 micropolarray-1.2.9/micropolarray/processing/image_cleaning.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     6162 2024-02-01 08:29:23.000000 micropolarray-1.2.9/micropolarray/processing/linear_roi.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)    13011 2024-02-01 09:12:03.000000 micropolarray-1.2.9/micropolarray/processing/nrgf.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     5485 2024-01-24 15:00:55.000000 micropolarray-1.2.9/micropolarray/processing/rebin.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1134 2023-10-16 08:25:34.000000 micropolarray-1.2.9/micropolarray/processing/shift.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     8693 2024-01-26 15:35:46.000000 micropolarray-1.2.9/micropolarray/utils.py
+drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2024-02-08 09:50:11.413042 micropolarray-1.2.9/micropolarray.egg-info/
+-rw-r--r--   0 herve     (1000) herve     (1000)     5080 2024-02-08 09:50:11.000000 micropolarray-1.2.9/micropolarray.egg-info/PKG-INFO
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1494 2024-02-08 09:50:11.000000 micropolarray-1.2.9/micropolarray.egg-info/SOURCES.txt
+-rw-rw-r--   0 herve     (1000) herve     (1000)        1 2024-02-08 09:50:11.000000 micropolarray-1.2.9/micropolarray.egg-info/dependency_links.txt
+-rw-rw-r--   0 herve     (1000) herve     (1000)      171 2024-02-08 09:50:11.000000 micropolarray-1.2.9/micropolarray.egg-info/requires.txt
+-rw-rw-r--   0 herve     (1000) herve     (1000)       14 2024-02-08 09:50:11.000000 micropolarray-1.2.9/micropolarray.egg-info/top_level.txt
+-rw-rw-r--   0 herve     (1000) herve     (1000)     1111 2024-02-08 09:49:37.000000 micropolarray-1.2.9/pyproject.toml
+-rw-rw-r--   0 herve     (1000) herve     (1000)       38 2024-02-08 09:50:11.413042 micropolarray-1.2.9/setup.cfg
+-rw-rw-r--   0 herve     (1000) herve     (1000)      643 2023-09-26 10:29:37.000000 micropolarray-1.2.9/setup.py
+drwxrwxr-x   0 herve     (1000) herve     (1000)        0 2024-02-08 09:50:11.413042 micropolarray-1.2.9/tests/
+-rw-rw-r--   0 herve     (1000) herve     (1000)     8679 2024-01-30 11:40:12.000000 micropolarray-1.2.9/tests/test_demodulation.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     7806 2024-01-26 16:47:03.000000 micropolarray-1.2.9/tests/test_image_and_micropolimage.py
+-rw-rw-r--   0 herve     (1000) herve     (1000)     2282 2023-09-29 10:43:34.000000 micropolarray-1.2.9/tests/test_utils.py
```

### Comparing `micropolarray-1.2.8/LICENSE` & `micropolarray-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `micropolarray-1.2.8/PKG-INFO` & `micropolarray-1.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropolarray
-Version: 1.2.8
+Version: 1.2.9
 Summary: micropolarizer array data utilities
 Home-page: https://github.com/Hevil33/micropolarray_master
 Author: Hervé Haudemand
 Author-email: Herve Haudemand <herve.haudemand@inaf.it>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Hevil33
@@ -90,22 +90,23 @@
 - Automatic polarization calculation
 - Fast and optimized operations on the micropolarizer array
 - Basic image cleaning (dark/flat subtraction)
 
 
 ## Documentation
 
-Get the simple [jupyter tutorial](https://github.com/Hevil33/micropolarray_master/blob/main/TUTORIAL.ipynb) for a brief introduction.
-
 Documentation is hosted at ReadTheDocs and can be found [HERE](https://micropolarray.readthedocs.io/en/latest/) (html format).
 
 
-
 ## Usage
 
+Get the simple [jupyter tutorial](https://github.com/Hevil33/micropolarray_master/blob/main/TUTORIAL.ipynb) for a brief introduction.
+
+After installation, you can import the library in your python application
+
 ```
 import micropolarray as ml
 ```
 
 The main class is `MicropolImage()`, which can be initialized from
 
 1. A `numpy` 2D array
```

### Comparing `micropolarray-1.2.8/README.md` & `micropolarray-1.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,22 +25,23 @@
 - Automatic polarization calculation
 - Fast and optimized operations on the micropolarizer array
 - Basic image cleaning (dark/flat subtraction)
 
 
 ## Documentation
 
-Get the simple [jupyter tutorial](https://github.com/Hevil33/micropolarray_master/blob/main/TUTORIAL.ipynb) for a brief introduction.
-
 Documentation is hosted at ReadTheDocs and can be found [HERE](https://micropolarray.readthedocs.io/en/latest/) (html format).
 
 
-
 ## Usage
 
+Get the simple [jupyter tutorial](https://github.com/Hevil33/micropolarray_master/blob/main/TUTORIAL.ipynb) for a brief introduction.
+
+After installation, you can import the library in your python application
+
 ```
 import micropolarray as ml
 ```
 
 The main class is `MicropolImage()`, which can be initialized from
 
 1. A `numpy` 2D array
```

### Comparing `micropolarray-1.2.8/micropolarray/__init__.py` & `micropolarray-1.2.9/micropolarray/__init__.py`

 * *Files identical despite different names*

### Comparing `micropolarray-1.2.8/micropolarray/cameras.py` & `micropolarray-1.2.9/micropolarray/cameras.py`

 * *Files identical despite different names*

### Comparing `micropolarray-1.2.8/micropolarray/image.py` & `micropolarray-1.2.9/micropolarray/image.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,20 +65,22 @@
                         hul[0].data / (1 + int(averageimages) * (filenames_len - 1))
                     )  # divide by 1 if summing, either n if averaging
 
                 hul.verify("fix")
 
                 try:  # standard format
                     datetimes[idx] = datetime.datetime.strptime(
-                        hul[0].header["DATE-OBS"],
+                        hul[0].header["DATE-OBS"].split(".")[0],
                         "%Y-%m-%dT%H:%M:%S",
                     )
                 except ValueError:  # antarticor format
                     datetimes[idx] = datetime.datetime.strptime(
-                        hul[0].header["DATE-OBS"] + "-" + hul[0].header["TIME-OBS"],
+                        hul[0].header["DATE-OBS"]
+                        + "-"
+                        + hul[0].header["TIME-OBS"].split(".")[0],
                         "%Y-%m-%d-%H:%M:%S",
                     )
                 except KeyError:
                     pass
 
         datetimes = [datetime for datetime in datetimes if datetime != 0]
         if len(datetimes) == 0:
@@ -211,27 +213,22 @@
 
         return image_fig, imageax
 
     def show_histogram(self, split_pols=False, **kwargs) -> tuple:
         """Print the histogram of the flattened image data
 
         Args:
-            split_pols (bool, optional): Whether to overplot histograms of same family pixels separately. Defaults to False.
             **kwargs (int, optional): arguments to pass to numpy.histogram(), like bins and range.
 
         Returns:
             tuple: fig, ax tuple as returned by matplotlib.pyplot.subplots
         """
         fig, ax = plt.subplots(dpi=200, constrained_layout=True)
         histo = np.histogram(self.data, **kwargs)
         ax.stairs(*histo, label="Total histogram")
-        if split_pols:
-            for i, single_pol_subimage in enumerate(self.single_pol_subimages):
-                subhist = np.histogram(single_pol_subimage, **kwargs)
-                ax.stairs(*subhist, label=f"pixel {i}")
         ax.set_title("Image histogram", color="black")
         ax.set_xlabel("Signal [DN]")
         ax.set_ylabel("Number of pixels")
         plt.legend()
 
         return fig, ax
```

### Comparing `micropolarray-1.2.8/micropolarray/micropol_image.py` & `micropolarray-1.2.9/micropolarray/micropol_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -316,15 +316,17 @@
             )
             for i in range(num_of_malus_parameters):
                 for j in range(pixels_in_superpix):
                     demo_component = demodulator.mij[i, j]
                     mij[i, j, :, :] = merge_polarizations(
                         np.repeat(demo_component[np.newaxis, :, :], 4, axis=0)
                     )  # repeat necessary to avoid numba problems
-
+            fit_found_flags = merge_polarizations(
+                np.array(4 * [demodulator.fit_found_flags.astype(float)])
+            )  # idk why but fit_found_flags is >f8 as default
         else:
             mij = demodulator.mij
             splitted_pols = self.single_pol_subimages
 
         """
         print(mij.shape)
         print(splitted_pols.shape)
@@ -603,14 +605,31 @@
             mappable,
             ax=ax,
             label=polparam.measure_unit,
             fraction=data_ratio * 0.05,
         )
         return fig, ax
 
+    def show_histogram(self, split_pols: bool = True, **kwargs):
+        """Print the histogram of the flattened image data
+
+        Args:
+            split_pols (bool, optional): Whether to overplot histograms of same family pixels separately. Defaults to False.
+            **kwargs (int, optional): arguments to pass to numpy.histogram(), like bins and range.
+        Returns:
+            tuple: fig, ax tuple as returned by matplotlib.pyplot.subplots
+        """
+
+        fig, ax = super().show_histogram()
+        if split_pols:
+            for i, single_pol_subimage in enumerate(self.single_pol_subimages):
+                subhist = np.histogram(single_pol_subimage, **kwargs)
+                ax.stairs(*subhist, label=f"pixel {i}")
+        return fig, ax
+
     # ----------------------------------------------------------------
     # -------------------------- SAVING ------------------------------
     # ----------------------------------------------------------------
 
     def save_single_pol_images(
         self, filename: str, fixto: list[float, float] = None
     ) -> None:
@@ -765,15 +784,16 @@
             hdu.writeto(new_filename, overwrite=True)
         info(f'Demosaiced images successfully saved to "{group_filename}_POLX.fits"')
 
     # ----------------------------------------------------------------
     # -------------------- DATA MANIPULATION -------------------------
     # ----------------------------------------------------------------
     def demosaic(self, demosaic_mode="adjacent") -> MicropolImage:
-        """Returns a demosaiced copy of the image with updated polarization parameters. Demoisacing is done IN PLACE.
+        """Returns a demosaiced copy of the image with updated polarization parameters. Demoisacing is done IN PLACE and
+        using the THEORETICAL MATRIX. If demodulation and demosaicing are required, please use demodulate(demosaic=True)
 
         Args:
             demosaic_mode (str, optional): demosaicing mode (see processing.demosaic). Defaults to "adjacent".
 
         Returns:
             MicropolImage: demosaiced image
         """
```

### Comparing `micropolarray-1.2.8/micropolarray/polarization_functions.py` & `micropolarray-1.2.9/micropolarray/polarization_functions.py`

 * *Files identical despite different names*

### Comparing `micropolarray-1.2.8/micropolarray/processing/chen_wan_liang_calibration.py` & `micropolarray-1.2.9/micropolarray/processing/chen_wan_liang_calibration.py`

 * *Files identical despite different names*

### Comparing `micropolarray-1.2.8/micropolarray/processing/congrid.py` & `micropolarray-1.2.9/micropolarray/processing/congrid.py`

 * *Files identical despite different names*

### Comparing `micropolarray-1.2.8/micropolarray/processing/convert.py` & `micropolarray-1.2.9/micropolarray/processing/convert.py`

 * *Files identical despite different names*

### Comparing `micropolarray-1.2.8/micropolarray/processing/demodulation.py` & `micropolarray-1.2.9/micropolarray/processing/demodulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -245,14 +245,15 @@
     binning: int = 1,
     occulter: list = None,
     procs_grid: list = [4, 4],
     dark_filename: str = None,
     flat_filename: str = None,
     normalizing_S=None,
     tk_boundary: list = None,
+    eff_boundary: list = None,
     DEBUG: bool = False,
 ):
     """Calculates the demodulation tensor images and saves them. Requires a set of images with different polarizations to fit a Malus curve model.
 
     Args:
         polarizer_orientations (list[float]): List containing the orientations of the incoming light for each image.
         filenames_list (list[str]): List of input images filenames to read. Must include [0, 45, 90, -45].
@@ -262,14 +263,15 @@
         binning (int, optional): Output matrices binning. Defaults to 1 (no binning). Be warned that binning matrices AFTER calculation is an incorrect operation.
         occulter (list, optional): occulter y, x center and radius to exclude from calculations. Defaults to None.
         procs_grid ([int, int], optional): number of processors per side [Y, X], parallelization will be done in a Y x X grid. Defaults to [4,4] (16 procs in a 4x4 grid).
         dark_filename (str, optional): Dark image filename to correct input images. Defaults to None.
         flat_filename (str, optional): Flat image filename to correct input images. Defaults to None.
         normalizing_S (float or np.ndarray, optional): maximum signal used to normalize single pixel signal. If not set will be estimated as the 4sigma of the signal distribution.
         tk_boundary (list): if provided, sets the transmittancy [initial guess, boundary_inf, boundary_sup] of the Malus curve (max value). Defaults to [0.5, 0.1, 1.-1.e-6].
+        eff_boundary (list): if provided, sets the efficiency [initial guess, boundary_inf, boundary_sup] of the Malus curve (max value). Defaults to [0.5, 0.1, 1.-1.e-6].
 
     Raises:
         ValueError: Raised if any among [0, 45, 90, -45] is not included in the input polarizations.
 
     Notes:
         In the binning process the sum of values is considered, which is ok because data is normalized over the maximum S before being fitted.
     """
@@ -479,14 +481,15 @@
     splitted_occulter = np.zeros(
         shape=(chunks_n_y * chunks_n_x, chunk_size_y, chunk_size_x)
     )
 
     # calculate normalized data and its error
     # sigma_data = sqrt(e) = sqrt(data / gain) (poisson)
     # sigma_norm = sqrt(data / gain) = sqrt(norm / gain / S) (propagation)
+
     np.divide(all_data_arr, normalizing_S, out=all_data_arr)
     pixel_errors = np.zeros_like(all_data_arr)
     np.divide(all_data_arr, normalizing_S * gain, out=pixel_errors)
     np.sqrt(pixel_errors, out=pixel_errors)
 
     for i in range(chunks_n_y):
         for j in range(chunks_n_x):
@@ -557,14 +560,15 @@
         [
             splitted_data[i],
             splitted_pixel_errors[i],
             splitted_occulter[i],
             polarizer_orientations,
             rad_micropol_phases_previsions,
             tk_boundary,
+            eff_boundary,
             DEBUG,
         ]
         for i in range(chunks_n_y * chunks_n_x)
     )
 
     starting_time = time.perf_counter()
     loc_time = time.strftime("%H:%M:%S  (%Y/%m/%d)", time.localtime())
@@ -725,24 +729,29 @@
 def compute_demodulation_by_chunk(
     splitted_normalized_dara_arr,
     splitted_pixel_erorrs,
     splitted_occulter_flag,
     polarizer_orientations,
     rad_micropol_phases_previsions,
     tk_boundary,
+    eff_boundary,
     DEBUG,
 ):
     """Utility function to parallelize calculations."""
     N_MALUS_PARAMS = 3
     N_PIXELS_IN_SUPERPIX = 4
+
+    dof = len(polarizer_orientations) - 2
     if tk_boundary is None:
-        dof = len(polarizer_orientations) - 3
         tk_boundary = [0.5, 0.1, 1.0 - 1.0e-6]
-    else:
-        dof = len(polarizer_orientations) - 2
+        dof -= 1
+    if eff_boundary is None:
+        eff_boundary = [0.5, 0.1, 1.0 - 1.0e-6]
+        dof -= 1
+
     # Preemptly compute the theoretical demo matrix to save time
     theo_modulation_matrix = np.array(
         [
             [0.5, 0.5, 0.5, 0.5],
             [
                 0.5 * np.cos(2.0 * rad_micropol_phases_previsions[i])
                 for i in range(N_PIXELS_IN_SUPERPIX)
@@ -759,15 +768,15 @@
 
     num_of_points, height, width = splitted_normalized_dara_arr.shape
     rad_micropol_phases_previsions = np.array(
         rad_micropol_phases_previsions, dtype=float
     )
     polarizations_rad = np.deg2rad(polarizer_orientations)
     tk_prediction = tk_boundary[0]
-    efficiency_prediction = 0.4
+    efficiency_prediction = eff_boundary[0]
 
     all_zeros = np.zeros(shape=(num_of_points))
     m_ij = np.zeros(
         shape=(
             N_MALUS_PARAMS,
             N_PIXELS_IN_SUPERPIX,
             int(height / 2),
@@ -794,15 +803,15 @@
     predictions = np.zeros(shape=(N_PIXELS_IN_SUPERPIX, N_MALUS_PARAMS))
     predictions[:, 0] = tk_prediction  # Throughput prediction
     predictions[:, 1] = efficiency_prediction  # Efficiency prediction
     predictions[:, 2] = rad_micropol_phases_previsions  # Angle prediction
 
     bounds = np.zeros(shape=(N_PIXELS_IN_SUPERPIX, 2, N_MALUS_PARAMS))
     bounds[:, 0, 0], bounds[:, 1, 0] = tk_boundary[1:]  # Throughput bounds
-    bounds[:, 0, 1], bounds[:, 1, 1] = 0.1, 1.0  # Efficiency bounds
+    bounds[:, 0, 1], bounds[:, 1, 1] = eff_boundary[1:]  # Efficiency bounds
     bounds[:, 0, 2] = rad_micropol_phases_previsions - 15  # Lower angle bounds
     bounds[:, 1, 2] = rad_micropol_phases_previsions + 15  # Upper angle bounds
 
     # Fit for each superpixel. Use theoretical demodulation matrix for
     # occulter if present.
     if DEBUG:
         x_start, x_end = 100, 150
@@ -877,14 +886,15 @@
                         fit_success = False
                         break
 
                 if DEBUG:  # DEBUG
                     colors = ["blue", "orange", "green", "red"]
                     fig, ax = plt.subplots(dpi=200, constrained_layout=True)
                     for i in range(4):
+                        print(f"{np.min(normalized_superpix_arr[:, i]) = :3.2f}")
                         ax.errorbar(
                             np.rad2deg(polarizations_rad),
                             normalized_superpix_arr[:, i],
                             yerr=sigma_pix[:, i],
                             xerr=[1.0] * len(polarizations_rad),
                             label=f"points {i}",
                             fmt="k-",
@@ -907,17 +917,17 @@
                         ax.set_xlabel("Prepolarizer orientations [deg]")
                         ax.set_ylabel("signal / S")
 
                     plt.legend()
                     plt.show()
 
                 if not fit_success:
-                    m_ij[
-                        :, :, int(super_y / 2), int(super_x / 2)
-                    ] = theo_demodulation_matrix
+                    m_ij[:, :, int(super_y / 2), int(super_x / 2)] = (
+                        theo_demodulation_matrix
+                    )
                     continue
 
                 # Compute modulation matrix and its inverse
                 t = superpix_params[:, 0]
                 eff = superpix_params[:, 1]
                 phi = superpix_params[:, 2]
 
@@ -984,20 +994,20 @@
                     eff, dtype=float
                 ).reshape(2, 2)
                 phase_data[super_y : super_y + 2, super_x : super_x + 2] = np.array(
                     phi, dtype=float
                 ).reshape(2, 2)
 
             else:  # pixel is in occulter region
-                m_ij[
-                    :, :, int(super_y / 2), int(super_x / 2)
-                ] = theo_demodulation_matrix
-                phase_data[
-                    super_y : super_y + 2, super_x : super_x + 2
-                ] = rad_micropol_phases_previsions.reshape(2, 2)
+                m_ij[:, :, int(super_y / 2), int(super_x / 2)] = (
+                    theo_demodulation_matrix
+                )
+                phase_data[super_y : super_y + 2, super_x : super_x + 2] = (
+                    rad_micropol_phases_previsions.reshape(2, 2)
+                )
                 tk_data[super_y : super_y + 2, super_x : super_x + 2] = np.array(
                     [
                         [tk_prediction, tk_prediction],
                         [tk_prediction, tk_prediction],
                     ],
                     dtype=float,
                 )
```

### Comparing `micropolarray-1.2.8/micropolarray/processing/demodulation_errors.py` & `micropolarray-1.2.9/micropolarray/processing/demodulation_errors.py`

 * *Files identical despite different names*

### Comparing `micropolarray-1.2.8/micropolarray/processing/demosaic.py` & `micropolarray-1.2.9/micropolarray/processing/demosaic.py`

 * *Files identical despite different names*

### Comparing `micropolarray-1.2.8/micropolarray/processing/image_cleaning.py` & `micropolarray-1.2.9/micropolarray/processing/image_cleaning.py`

 * *Files identical despite different names*

### Comparing `micropolarray-1.2.8/micropolarray/processing/linear_roi.py` & `micropolarray-1.2.9/micropolarray/processing/linear_roi.py`

 * *Files identical despite different names*

### Comparing `micropolarray-1.2.8/micropolarray/processing/nrgf.py` & `micropolarray-1.2.9/micropolarray/processing/nrgf.py`

 * *Files identical despite different names*

### Comparing `micropolarray-1.2.8/micropolarray/processing/rebin.py` & `micropolarray-1.2.9/micropolarray/processing/rebin.py`

 * *Files identical despite different names*

### Comparing `micropolarray-1.2.8/micropolarray/processing/shift.py` & `micropolarray-1.2.9/micropolarray/processing/shift.py`

 * *Files identical despite different names*

### Comparing `micropolarray-1.2.8/micropolarray/utils.py` & `micropolarray-1.2.9/micropolarray/utils.py`

 * *Files identical despite different names*

### Comparing `micropolarray-1.2.8/micropolarray.egg-info/PKG-INFO` & `micropolarray-1.2.9/micropolarray.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: micropolarray
-Version: 1.2.8
+Version: 1.2.9
 Summary: micropolarizer array data utilities
 Home-page: https://github.com/Hevil33/micropolarray_master
 Author: Hervé Haudemand
 Author-email: Herve Haudemand <herve.haudemand@inaf.it>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Hevil33
@@ -90,22 +90,23 @@
 - Automatic polarization calculation
 - Fast and optimized operations on the micropolarizer array
 - Basic image cleaning (dark/flat subtraction)
 
 
 ## Documentation
 
-Get the simple [jupyter tutorial](https://github.com/Hevil33/micropolarray_master/blob/main/TUTORIAL.ipynb) for a brief introduction.
-
 Documentation is hosted at ReadTheDocs and can be found [HERE](https://micropolarray.readthedocs.io/en/latest/) (html format).
 
 
-
 ## Usage
 
+Get the simple [jupyter tutorial](https://github.com/Hevil33/micropolarray_master/blob/main/TUTORIAL.ipynb) for a brief introduction.
+
+After installation, you can import the library in your python application
+
 ```
 import micropolarray as ml
 ```
 
 The main class is `MicropolImage()`, which can be initialized from
 
 1. A `numpy` 2D array
```

### Comparing `micropolarray-1.2.8/micropolarray.egg-info/SOURCES.txt` & `micropolarray-1.2.9/micropolarray.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `micropolarray-1.2.8/pyproject.toml` & `micropolarray-1.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
-version = "1.2.8"
+version = "1.2.9"
 name = "micropolarray"
 description = "micropolarizer array data utilities"
 readme = "README.md"
 authors = [{ name ="Herve Haudemand", email = "herve.haudemand@inaf.it" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: BSD License",
```

### Comparing `micropolarray-1.2.8/setup.py` & `micropolarray-1.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `micropolarray-1.2.8/tests/test_demodulation.py` & `micropolarray-1.2.9/tests/test_demodulation.py`

 * *Files identical despite different names*

### Comparing `micropolarray-1.2.8/tests/test_image_and_micropolimage.py` & `micropolarray-1.2.9/tests/test_image_and_micropolimage.py`

 * *Files identical despite different names*

### Comparing `micropolarray-1.2.8/tests/test_utils.py` & `micropolarray-1.2.9/tests/test_utils.py`

 * *Files identical despite different names*

