# Comparing `tmp/mavisim-1.1.8.tar.gz` & `tmp/mavisim-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mavisim-1.1.8.tar", last modified: Mon May  2 03:28:32 2022, max compression
+gzip compressed data, was "mavisim-1.1.9.tar", last modified: Tue May 17 02:28:54 2022, max compression
```

## Comparing `mavisim-1.1.8.tar` & `mavisim-1.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 jcranney   (503) staff       (20)        0 2022-05-02 03:28:32.323508 mavisim-1.1.8/
--rw-r--r--   0 jcranney   (503) staff       (20)    35149 2022-02-02 09:06:18.000000 mavisim-1.1.8/LICENSE
--rw-r--r--   0 jcranney   (503) staff       (20)     1950 2022-05-02 03:28:32.323797 mavisim-1.1.8/PKG-INFO
--rw-r--r--   0 jcranney   (503) staff       (20)     1455 2022-02-02 09:06:18.000000 mavisim-1.1.8/README.md
-drwxr-xr-x   0 jcranney   (503) staff       (20)        0 2022-05-02 03:28:32.319990 mavisim-1.1.8/mavisim/
--rw-r--r--   0 jcranney   (503) staff       (20)      172 2022-02-02 09:06:18.000000 mavisim-1.1.8/mavisim/__init__.py
--rw-r--r--   0 jcranney   (503) staff       (20)    16573 2022-02-02 09:06:18.000000 mavisim-1.1.8/mavisim/astromsim.py
--rw-r--r--   0 jcranney   (503) staff       (20)    14652 2022-05-02 03:27:09.000000 mavisim-1.1.8/mavisim/generate_image.py
--rw-r--r--   0 jcranney   (503) staff       (20)    11210 2022-05-02 03:04:44.000000 mavisim-1.1.8/mavisim/source.py
--rw-r--r--   0 jcranney   (503) staff       (20)     8045 2022-02-02 09:06:18.000000 mavisim-1.1.8/mavisim/util.py
-drwxr-xr-x   0 jcranney   (503) staff       (20)        0 2022-05-02 03:28:32.323033 mavisim-1.1.8/mavisim.egg-info/
--rw-r--r--   0 jcranney   (503) staff       (20)     1950 2022-05-02 03:28:31.000000 mavisim-1.1.8/mavisim.egg-info/PKG-INFO
--rw-r--r--   0 jcranney   (503) staff       (20)      297 2022-05-02 03:28:32.000000 mavisim-1.1.8/mavisim.egg-info/SOURCES.txt
--rw-r--r--   0 jcranney   (503) staff       (20)        1 2022-05-02 03:28:31.000000 mavisim-1.1.8/mavisim.egg-info/dependency_links.txt
--rw-r--r--   0 jcranney   (503) staff       (20)       33 2022-05-02 03:28:32.000000 mavisim-1.1.8/mavisim.egg-info/requires.txt
--rw-r--r--   0 jcranney   (503) staff       (20)        8 2022-05-02 03:28:32.000000 mavisim-1.1.8/mavisim.egg-info/top_level.txt
--rw-r--r--   0 jcranney   (503) staff       (20)      104 2022-02-02 09:06:18.000000 mavisim-1.1.8/pyproject.toml
--rw-r--r--   0 jcranney   (503) staff       (20)      605 2022-05-02 03:28:32.325085 mavisim-1.1.8/setup.cfg
+drwxr-xr-x   0 jcranney   (503) staff       (20)        0 2022-05-17 02:28:54.135149 mavisim-1.1.9/
+-rw-r--r--   0 jcranney   (503) staff       (20)    35149 2022-02-02 09:06:18.000000 mavisim-1.1.9/LICENSE
+-rw-r--r--   0 jcranney   (503) staff       (20)     1913 2022-05-17 02:28:54.135389 mavisim-1.1.9/PKG-INFO
+-rw-r--r--   0 jcranney   (503) staff       (20)     1455 2022-02-02 09:06:18.000000 mavisim-1.1.9/README.md
+drwxr-xr-x   0 jcranney   (503) staff       (20)        0 2022-05-17 02:28:54.131285 mavisim-1.1.9/mavisim/
+-rw-r--r--   0 jcranney   (503) staff       (20)      172 2022-02-02 09:06:18.000000 mavisim-1.1.9/mavisim/__init__.py
+-rw-r--r--   0 jcranney   (503) staff       (20)    16573 2022-02-02 09:06:18.000000 mavisim-1.1.9/mavisim/astromsim.py
+-rw-r--r--   0 jcranney   (503) staff       (20)    14653 2022-05-17 02:27:12.000000 mavisim-1.1.9/mavisim/generate_image.py
+-rw-r--r--   0 jcranney   (503) staff       (20)    10692 2022-05-17 02:27:40.000000 mavisim-1.1.9/mavisim/source.py
+-rw-r--r--   0 jcranney   (503) staff       (20)     8045 2022-02-02 09:06:18.000000 mavisim-1.1.9/mavisim/util.py
+drwxr-xr-x   0 jcranney   (503) staff       (20)        0 2022-05-17 02:28:54.134774 mavisim-1.1.9/mavisim.egg-info/
+-rw-r--r--   0 jcranney   (503) staff       (20)     1913 2022-05-17 02:28:53.000000 mavisim-1.1.9/mavisim.egg-info/PKG-INFO
+-rw-r--r--   0 jcranney   (503) staff       (20)      297 2022-05-17 02:28:54.000000 mavisim-1.1.9/mavisim.egg-info/SOURCES.txt
+-rw-r--r--   0 jcranney   (503) staff       (20)        1 2022-05-17 02:28:53.000000 mavisim-1.1.9/mavisim.egg-info/dependency_links.txt
+-rw-r--r--   0 jcranney   (503) staff       (20)       33 2022-05-17 02:28:53.000000 mavisim-1.1.9/mavisim.egg-info/requires.txt
+-rw-r--r--   0 jcranney   (503) staff       (20)        8 2022-05-17 02:28:54.000000 mavisim-1.1.9/mavisim.egg-info/top_level.txt
+-rw-r--r--   0 jcranney   (503) staff       (20)      104 2022-05-03 00:40:35.000000 mavisim-1.1.9/pyproject.toml
+-rw-r--r--   0 jcranney   (503) staff       (20)      605 2022-05-17 02:28:54.136060 mavisim-1.1.9/setup.cfg
```

### Comparing `mavisim-1.1.8/LICENSE` & `mavisim-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mavisim-1.1.8/PKG-INFO` & `mavisim-1.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: mavisim
-Version: 1.1.8
+Version: 1.1.9
 Summary: Tool for simulating MAVIS images
 Home-page: https://github.com/smonty93/mavisim
 Author: Stephanie Monty
 Author-email: stephanie.monty@anu.edu.au
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -41,9 +39,7 @@
 # Future Versions
 
 ## MAVISIM 1.2: Broadband End-to-End PSF
 Broadband images! Starting with the V band
 
 ## MAVISIM 2.0
 Extended object version, not yet in development.
-
-
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: mavisim Version: 1.1.8 Summary: Tool for simulating
+Metadata-Version: 2.1 Name: mavisim Version: 1.1.9 Summary: Tool for simulating
 MAVIS images Home-page: https://github.com/smonty93/mavisim Author: Stephanie
-Monty Author-email: stephanie.monty@anu.edu.au License: UNKNOWN Platform:
-UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier: License ::
-OSI Approved :: GNU General Public License (GPL) Classifier: Operating System
-:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
-markdown License-File: LICENSE # MAVISIM Image simulating tool for the next
-generation ESO instrument MAVIS. If you use MAVISIM please cite _M_o_n_t_y_ _e_t_ _a_l_.
-_2_0_2_1_. ## Current Version **1.1 - EtE PSF** - more accurate representation of
-the PSF, suitable for photometric and astrometric science cases Documentation
-can be found _h_e_r_e ## Past Versions 1.0 - Fourier PSF - fast, most flexibility
-for astrometric modeling Documentation can be found _h_e_r_e ## General Features 1.
-Can simulate full stellar field (eg. Milky Way Globular Cluster) from an input
-catalogue 2. Models three major sources of astrometric error introduced by the
-AO system: 1. Tip-tilt residuals originating from uncorrected LO aberrations
-(dependent on the NGS constellation brightness and geometry) **field variable**
-2. HO aberrations originating from the LGS constellation and characteristics
-**field variable** 3. Static field distortion originating from the AO module
-optics ## Current Limitations 1. Monochromatic images only 2. Only compatible
-with input **point source catalogues only** # Future Versions ## MAVISIM 1.2:
-Broadband End-to-End PSF Broadband images! Starting with the V band ## MAVISIM
-2.0 Extended object version, not yet in development.
+Monty Author-email: stephanie.monty@anu.edu.au Classifier: Programming Language
+:: Python :: 3 Classifier: License :: OSI Approved :: GNU General Public
+License (GPL) Classifier: Operating System :: OS Independent Requires-Python:
+>=3.7 Description-Content-Type: text/markdown License-File: LICENSE # MAVISIM
+Image simulating tool for the next generation ESO instrument MAVIS. If you use
+MAVISIM please cite _M_o_n_t_y_ _e_t_ _a_l_._ _2_0_2_1_. ## Current Version **1.1 - EtE PSF** -
+more accurate representation of the PSF, suitable for photometric and
+astrometric science cases Documentation can be found _h_e_r_e ## Past Versions 1.0
+- Fourier PSF - fast, most flexibility for astrometric modeling Documentation
+can be found _h_e_r_e ## General Features 1. Can simulate full stellar field (eg.
+Milky Way Globular Cluster) from an input catalogue 2. Models three major
+sources of astrometric error introduced by the AO system: 1. Tip-tilt residuals
+originating from uncorrected LO aberrations (dependent on the NGS constellation
+brightness and geometry) **field variable** 2. HO aberrations originating from
+the LGS constellation and characteristics **field variable** 3. Static field
+distortion originating from the AO module optics ## Current Limitations 1.
+Monochromatic images only 2. Only compatible with input **point source
+catalogues only** # Future Versions ## MAVISIM 1.2: Broadband End-to-End PSF
+Broadband images! Starting with the V band ## MAVISIM 2.0 Extended object
+version, not yet in development.
```

### Comparing `mavisim-1.1.8/README.md` & `mavisim-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `mavisim-1.1.8/mavisim/astromsim.py` & `mavisim-1.1.9/mavisim/astromsim.py`

 * *Files identical despite different names*

### Comparing `mavisim-1.1.8/mavisim/generate_image.py` & `mavisim-1.1.9/mavisim/generate_image.py`

 * *Files 3% similar despite different names*

```diff
@@ -182,30 +182,30 @@
             # Run einsum calcs once to determine optimal sequence:
             self.optimize_star_kernel()
             
             self._init = False
         
         # Pick star from source table
         star_flux = self.source_flux[index]
-        star_pos  = self.source_pos[index]
+        star_pos  = self.source_pos[index] - 0.5*self.pixsize # convention is that (0,0)" is between the middle 4 pixels"
         
         if self.dtype==np.complex64:
             star_flux = np.float32(star_flux)
             star_pos  = star_pos.astype(np.float32)
 
         # Clear internal array:
         self._psf_array *= 0.0
 
         # Compute effective PSF:
         self.get_effective_psf_fft(star_pos)
 
         # Prepare for FFT Gaussian computation:
-        offset = (((((star_pos % self.pixsize)/self.pixsize)+0.5)%1)-1)*self.pixsize # this has to be easier
+        offset = star_pos%self.pixsize
         _star_pos = (self.psf_width_as+self.gauss_width_as)/2 * np.r_[1.0,1.0] + offset
-        bottom_left_corner = star_pos-offset-self.psf_width_as/2 - 0.5*self.pixsize
+        bottom_left_corner = np.int32(star_pos//self.pixsize - self.psf_width_pix//2)
 
         # Compute star Gaussian and convolve with PSF:
         self._psf_array *= self.get_star_kernel_fft(star_flux, _star_pos)
         
         # Inverse FFT and trimming:
         out = (np.fft.fftshift(
             np.fft.irfft2(
@@ -312,16 +312,16 @@
     def main(self):
         """Loop over all stars and add the tile to the full image.
         """
         for ni in tqdm(range(self.nsource),leave=False):
             # Generate the tile:
             tile,origin = self.tile_gen.get_tile(ni)
             # Find the location of the tile in the full image:
-            xstart = np.abs(self.xx-origin[0]).argmin()
-            ystart = np.abs(self.xx-origin[1]).argmin()
+            xstart = origin[0]+self.xx.shape[0]//2
+            ystart = origin[1]+self.xx.shape[0]//2
             # Slice the tile in:
             self.full_image[ystart:ystart+self.tile_gen.psf_width_pix,
                             xstart:xstart+self.tile_gen.psf_width_pix] += tile
         
     def get_rebinned_cropped(self,rebin_factor,cropped_width_as):
         """Rebin self.full_image after cropping to desired rebin factor.
```

### Comparing `mavisim-1.1.8/mavisim/source.py` & `mavisim-1.1.9/mavisim/source.py`

 * *Files 6% similar despite different names*

```diff
@@ -158,47 +158,35 @@
 		Args:
 			star_info = row of the astropy table containing all the info required for that star
 			
 		Returns:
 			x/y_dist = the sub-pixel shift in the x/y-direction for the star
 
 		"""
-
-		# Save the sub-pixel shift that comes from converting e.g. 15.1 degrees to pixels, pass this to the Gaussian later
-		x_mu_pix_true = (star_info["X"])/self._input_par.ccd_sampling
-		y_mu_pix_true = (star_info["Y"])/self._input_par.ccd_sampling
-
-		# Nearest integer pixel
-		x_mu_pix = int(np.around(star_info["X"]/self._input_par.ccd_sampling, 0))
-		y_mu_pix = int(np.around(star_info["Y"]/self._input_par.ccd_sampling, 0))
-
-		# Sub-pixel shift
-		delta_xpix = x_mu_pix_true - x_mu_pix
-		delta_ypix = y_mu_pix_true - y_mu_pix
-
+		# TODO: this can be made significantly cleaner
 		if self._static_dist_flag == True:
 			# Retrieve the interpolated distortion at each point and convert from the default output (mm) to pixels
 			# Input to functions is in degrees
 			x_deg = star_info["X"]/3600.0
 			y_deg = star_info["Y"]/3600.0
 
 			# Static distortion for the star given the location, converting from mm to pixels
 			x_static_dist = (((self._dist_x_func_degmm(x_deg, y_deg) * self._input_par.plate_scale)/self._input_par.ccd_sampling)[0][0]) * self._stat_amp
 			y_static_dist = (((self._dist_y_func_degmm(x_deg, y_deg) * self._input_par.plate_scale)/self._input_par.ccd_sampling)[0][0]) * self._stat_amp
 
 			# Sum the two sub-pixel terms to find the final distortion
-			final_x_dist = x_static_dist + delta_xpix
-			final_y_dist = y_static_dist + delta_ypix
+			final_x_dist = x_static_dist
+			final_y_dist = y_static_dist
 
 			return (final_x_dist, final_y_dist, np.asarray([x_static_dist, y_static_dist]))
 
 		else:
 			# Sub-pixel shift is solely associated with the conversion from arcseconds to pixels
-			final_x_dist = delta_xpix
-			final_y_dist = delta_ypix
+			final_x_dist = 0.0
+			final_y_dist = 0.0
 
 			return (final_x_dist, final_y_dist, np.asarray([0, 0]))
 
 	def decimate(self, nstar):
 		"""Decimate the list of objects in the object (e.g., for faster simualtions).
 
 		Args:
```

### Comparing `mavisim-1.1.8/mavisim/util.py` & `mavisim-1.1.9/mavisim/util.py`

 * *Files identical despite different names*

### Comparing `mavisim-1.1.8/mavisim.egg-info/PKG-INFO` & `mavisim-1.1.9/mavisim.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: mavisim
-Version: 1.1.8
+Version: 1.1.9
 Summary: Tool for simulating MAVIS images
 Home-page: https://github.com/smonty93/mavisim
 Author: Stephanie Monty
 Author-email: stephanie.monty@anu.edu.au
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -41,9 +39,7 @@
 # Future Versions
 
 ## MAVISIM 1.2: Broadband End-to-End PSF
 Broadband images! Starting with the V band
 
 ## MAVISIM 2.0
 Extended object version, not yet in development.
-
-
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: mavisim Version: 1.1.8 Summary: Tool for simulating
+Metadata-Version: 2.1 Name: mavisim Version: 1.1.9 Summary: Tool for simulating
 MAVIS images Home-page: https://github.com/smonty93/mavisim Author: Stephanie
-Monty Author-email: stephanie.monty@anu.edu.au License: UNKNOWN Platform:
-UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier: License ::
-OSI Approved :: GNU General Public License (GPL) Classifier: Operating System
-:: OS Independent Requires-Python: >=3.7 Description-Content-Type: text/
-markdown License-File: LICENSE # MAVISIM Image simulating tool for the next
-generation ESO instrument MAVIS. If you use MAVISIM please cite _M_o_n_t_y_ _e_t_ _a_l_.
-_2_0_2_1_. ## Current Version **1.1 - EtE PSF** - more accurate representation of
-the PSF, suitable for photometric and astrometric science cases Documentation
-can be found _h_e_r_e ## Past Versions 1.0 - Fourier PSF - fast, most flexibility
-for astrometric modeling Documentation can be found _h_e_r_e ## General Features 1.
-Can simulate full stellar field (eg. Milky Way Globular Cluster) from an input
-catalogue 2. Models three major sources of astrometric error introduced by the
-AO system: 1. Tip-tilt residuals originating from uncorrected LO aberrations
-(dependent on the NGS constellation brightness and geometry) **field variable**
-2. HO aberrations originating from the LGS constellation and characteristics
-**field variable** 3. Static field distortion originating from the AO module
-optics ## Current Limitations 1. Monochromatic images only 2. Only compatible
-with input **point source catalogues only** # Future Versions ## MAVISIM 1.2:
-Broadband End-to-End PSF Broadband images! Starting with the V band ## MAVISIM
-2.0 Extended object version, not yet in development.
+Monty Author-email: stephanie.monty@anu.edu.au Classifier: Programming Language
+:: Python :: 3 Classifier: License :: OSI Approved :: GNU General Public
+License (GPL) Classifier: Operating System :: OS Independent Requires-Python:
+>=3.7 Description-Content-Type: text/markdown License-File: LICENSE # MAVISIM
+Image simulating tool for the next generation ESO instrument MAVIS. If you use
+MAVISIM please cite _M_o_n_t_y_ _e_t_ _a_l_._ _2_0_2_1_. ## Current Version **1.1 - EtE PSF** -
+more accurate representation of the PSF, suitable for photometric and
+astrometric science cases Documentation can be found _h_e_r_e ## Past Versions 1.0
+- Fourier PSF - fast, most flexibility for astrometric modeling Documentation
+can be found _h_e_r_e ## General Features 1. Can simulate full stellar field (eg.
+Milky Way Globular Cluster) from an input catalogue 2. Models three major
+sources of astrometric error introduced by the AO system: 1. Tip-tilt residuals
+originating from uncorrected LO aberrations (dependent on the NGS constellation
+brightness and geometry) **field variable** 2. HO aberrations originating from
+the LGS constellation and characteristics **field variable** 3. Static field
+distortion originating from the AO module optics ## Current Limitations 1.
+Monochromatic images only 2. Only compatible with input **point source
+catalogues only** # Future Versions ## MAVISIM 1.2: Broadband End-to-End PSF
+Broadband images! Starting with the V band ## MAVISIM 2.0 Extended object
+version, not yet in development.
```

### Comparing `mavisim-1.1.8/setup.cfg` & `mavisim-1.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = mavisim
-version = 1.1.8
+version = 1.1.9
 author = Stephanie Monty
 author_email = stephanie.monty@anu.edu.au
 description = Tool for simulating MAVIS images
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/smonty93/mavisim
 classifiers =
```

