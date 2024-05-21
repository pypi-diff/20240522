# Comparing `tmp/msigen-0.2.1.tar.gz` & `tmp/msigen-0.2.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msigen-0.2.1.tar", max compression
+gzip compressed data, was "msigen-0.2.2rc1.tar", max compression
```

## Comparing `msigen-0.2.1.tar` & `msigen-0.2.2rc1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1091 2024-05-16 19:53:18.606091 msigen-0.2.1/LICENSE.txt
--rw-r--r--   0        0        0      178 2024-05-16 19:53:07.444990 msigen-0.2.1/MSIGen/__init__.py
--rw-r--r--   0        0        0    52726 2024-05-16 19:53:03.628205 msigen-0.2.1/MSIGen/D.py
--rw-r--r--   0        0        0    51238 2024-05-16 19:52:31.864409 msigen-0.2.1/MSIGen/GUI.py
--rw-r--r--   0        0        0    58278 2024-05-16 19:53:10.557672 msigen-0.2.1/MSIGen/msigen.py
--rw-r--r--   0        0        0    33676 2024-05-16 19:53:09.653091 msigen-0.2.1/MSIGen/mzml.py
--rw-r--r--   0        0        0    19004 2024-05-16 19:53:08.655754 msigen-0.2.1/MSIGen/raw.py
--rw-r--r--   0        0        0 12886552 2024-04-30 20:20:11.276935 msigen-0.2.1/MSIGen/timsdata.dll
--rw-r--r--   0        0        0     9775 2024-05-16 19:53:12.647190 msigen-0.2.1/MSIGen/tsf.py
--rw-r--r--   0        0        0    21985 2024-05-20 15:10:20.012509 msigen-0.2.1/MSIGen/visualization.py
--rw-r--r--   0        0        0     1320 2024-05-20 15:23:06.551962 msigen-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2323 2024-05-14 23:34:29.375945 msigen-0.2.1/README.md
--rw-r--r--   0        0        0     1077 2024-05-16 20:43:03.261270 msigen-0.2.1/tests/example_config_file.json
--rw-r--r--   0        0        0     3713 1970-01-01 00:00:00.000000 msigen-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-05-16 19:53:18.606091 msigen-0.2.2rc1/LICENSE.txt
+-rw-r--r--   0        0        0      178 2024-05-16 19:53:07.444990 msigen-0.2.2rc1/MSIGen/__init__.py
+-rw-r--r--   0        0        0    52811 2024-05-21 21:28:04.589990 msigen-0.2.2rc1/MSIGen/D.py
+-rw-r--r--   0        0        0    51238 2024-05-16 19:52:31.864409 msigen-0.2.2rc1/MSIGen/GUI.py
+-rw-r--r--   0        0        0    58255 2024-05-21 20:55:02.009291 msigen-0.2.2rc1/MSIGen/msigen.py
+-rw-r--r--   0        0        0    33676 2024-05-21 20:54:59.311672 msigen-0.2.2rc1/MSIGen/mzml.py
+-rw-r--r--   0        0        0    19677 2024-05-21 21:13:04.416726 msigen-0.2.2rc1/MSIGen/raw.py
+-rw-r--r--   0        0        0 12886552 2024-04-30 20:20:11.276935 msigen-0.2.2rc1/MSIGen/timsdata.dll
+-rw-r--r--   0        0        0     9775 2024-05-16 19:53:12.647190 msigen-0.2.2rc1/MSIGen/tsf.py
+-rw-r--r--   0        0        0    22015 2024-05-21 21:27:26.804996 msigen-0.2.2rc1/MSIGen/visualization.py
+-rw-r--r--   0        0        0     1323 2024-05-21 21:31:03.924391 msigen-0.2.2rc1/pyproject.toml
+-rw-r--r--   0        0        0     2323 2024-05-14 23:34:29.375945 msigen-0.2.2rc1/README.md
+-rw-r--r--   0        0        0     3716 1970-01-01 00:00:00.000000 msigen-0.2.2rc1/PKG-INFO
```

### Comparing `msigen-0.2.1/LICENSE.txt` & `msigen-0.2.2rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `msigen-0.2.1/MSIGen/D.py` & `msigen-0.2.2rc1/MSIGen/D.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,43 @@
 from MSIGen import msigen
+
+import os, sys
+import numpy as np
+from tqdm import tqdm
+
 try:
     from MSIGen import tsf
     assert "dll" in dir(tsf)
 except:
     print("Cannot extract Bruker .tsf data. Check that you input the timsdata.dll in the correct location")
 
 # bruker tdf
 try:
     from opentimspy.opentims import OpenTIMS
 except:
     print('Could not import opentimspy. Cannot process .tdf format data from Bruker TIMS-TOF')
 
 # Agilent
 try:
+    # import multiplierz and necessary dlls
+    import multiplierz
     from multiplierz.mzAPI import mzFile
+    import clr
+    # gets dlls from within multiplierz package to access DesiredMSStorageType variable
+    multiplierz_path = multiplierz.__file__
+    dllpath = os.path.split(multiplierz_path)[0]+"\\mzAPI\\agilentdlls"
+    sys.path += [dllpath]
+    dlls = ['MassSpecDataReader', 'BaseCommon', 'BaseDataAccess']
+    for dll in dlls: clr.AddReference(dll)
+    import Agilent
+    from Agilent.MassSpectrometry.DataAnalysis import DesiredMSStorageType
+
 except: 
     print("Could not import mzFile. Cannot process Agilent's .d format data")
 
-import os, sys
-import numpy as np
-from tqdm import tqdm
-from scipy.interpolate import interpn
 
 # =====================================================================================
 # General functions
 # =====================================================================================
 
 def determine_file_format(line_list):
     MS_level = 'Not specified'
@@ -372,14 +385,19 @@
     TICs: np array of TICs
     '''
     headers = np.array(data.xic())
     Acq_times = np.round(headers[:,0], 4)
     TICs = headers[:,1]
     return Acq_times, TICs
 
+def get_agilent_scan(data, index):
+    # faster implementation of multiplierz scan() method for agilent files
+    mode = DesiredMSStorageType.ProfileElsePeak
+    scanObj = data.source.GetSpectrum(data.source, index, data.noFilter, data.noFilter, mode)
+    return np.array(scanObj.XArray), np.array(scanObj.YArray)
 
 # =====================================================================================
 # Agilent MS1 Workflow
 # =====================================================================================
 
 def agilent_d_ms1_no_mob(line_list, mass_lists, lower_lims, upper_lims, experiment_type, metadata, in_jupyter = True, testing = False, gui=False, tkinter_widgets = [None, None, None]):
 
@@ -412,36 +430,40 @@
         with HiddenPrints():
             data = mzFile(file_dir)
 
         if i == 0:
             metadata = get_basic_instrument_metadata_agilent(line_list, data, metadata)
 
         # grab headers for all scans
+        # the TIC here is from centroided data. 
+        # This means that it should not be used since default data extraction is in profile mode in MSIGen 
         line_rts, TICs = get_agilent_d_headers(data)
-        num_spe = len(TICs)
+        num_spe = len(line_rts)
         line_rts = np.array(line_rts[:num_spe])
         
         line_pixels = np.zeros((num_spe, MS1_list.shape[0]+1))
-        line_pixels[:,0] = TICs
 
         for j in tqdm(range(num_spe), desc = 'Progress through line {}'.format(i+1), disable = (testing or gui)):
             # Update gui variables            
             if gui:
                 tkinter_widgets[0]['value']=(100*i/len(line_list))+((100/len(line_list))*(j/num_spe))
                 tkinter_widgets[0].update()
                 tkinter_widgets[2]['text']=f'line {i+1}/{len(line_list)}, spectrum {j+1}/{num_spe}'
                 tkinter_widgets[2].update()
             
             # get all intensity values for pixel 
-            intensity_points = np.array(data.source.GetSpectrum(data.source, j).YArray)
+            mz, intensity_points = get_agilent_scan(data, j)
             # remove all values of zero to improve speed
             intensity_points_mask = np.where(intensity_points)
             intensity_points = np.append(intensity_points[intensity_points_mask[0]],0)
             # get all m/z values with nonzero intensity
-            mz = np.array(data.source.GetSpectrum(data.source, j).XArray)[intensity_points_mask[0]]
+            mz = mz[intensity_points_mask[0]]
+
+            # Get TIC
+            line_pixels[j,0]=np.sum(intensity_points)
             
             if msigen.numba_present:
                 idxs_to_sum = msigen.vectorized_sorted_slice_njit(mz, lb_sort, ub_sort)
                 pixel = msigen.assign_values_to_pixel_njit(intensity_points, idxs_to_sum)
                 line_pixels[j,1:] = pixel
             else:
                 idxs_to_sum = msigen.vectorized_sorted_slice(mz, lb_sort, ub_sort) # Slower
@@ -521,17 +543,15 @@
             # if i == 0:
             #     metadata = get_basic_instrument_metadata_raw_no_mob(data, metadata)
 
             # a list of 2d matrix, matrix: scans x (mzs +1)  , 1 -> tic
             pixels_meta = [ np.zeros((scans_per_filter_grp[i][_] , peak_counts_per_filter_grp[_] + 1)) for _ in range(num_filter_groups) ]
             
             # old version kept in case of bugs 
-            # TIC = np.array(data.xic())[:,1]
-
-            TIC = get_TIC_agilent(data, acq_times[i])
+            # TIC = get_TIC_agilent(data, acq_times[i])
 
             for j, TimeStamp in tqdm(enumerate(acq_times[i]), disable = True):
                 # Update gui variables            
                 if gui:
                     tkinter_widgets[0]['value']=(100*i/len(line_list))+((100/len(line_list))*(j/len(acq_times[i])))
                     tkinter_widgets[0].update()
                     tkinter_widgets[2]['text']=f'line {i+1}/{len(line_list)}, spectrum {j+1}/{len(acq_times[i])}'
@@ -539,26 +559,27 @@
 
                 # determine which group is going to be used
                 grp = grp_from_scan_idx[scan_idx]
                 counter[grp]+=1
 
                 # handle info
                 TimeStamps[grp][counter[grp]] = TimeStamp 
-                pixels_meta[grp][counter[grp], 0] = TIC[j]
+                # get all intensity values for pixel 
+                mz, intensity_points = get_agilent_scan(data, j)
+                # Get TIC
+                pixels_meta[grp][counter[grp], 0] = np.sum(intensity_points)
 
                 # skip filters with no masses in the mass list
                 if peak_counts_per_filter_grp[grp]:
 
-                    # get spectrum
-                    intensity_points = np.array(data.source.GetSpectrum(data.source, j).YArray)
                     # remove all values of zero to improve speed
                     intensity_points_mask = np.where(intensity_points)
-                    intensity_points = intensity_points[intensity_points_mask[0]]
+                    intensity_points = np.append(intensity_points[intensity_points_mask[0]],0)
                     # get all m/z values with nonzero intensity
-                    mz = np.array(data.source.GetSpectrum(data.source, j).XArray)[intensity_points_mask[0]]
+                    mz = mz[intensity_points_mask[0]]
                     
                     lbs,ubs = np.array(mzs_per_filter_grp_lb[grp]), np.array(mzs_per_filter_grp_ub[grp])
                 
                     if msigen.numba_present:
                         idxs_to_sum = msigen.vectorized_sorted_slice_njit(mz, lbs, ubs)
                         pixel = msigen.assign_values_to_pixel_njit(intensity_points, idxs_to_sum)
                         pixels_meta[grp][counter[grp],1:] = pixel
@@ -597,37 +618,14 @@
     # Order the pixels in the way the mass list csv/excel file was ordered
     pixels = reorder_pixels_d(pixels, consolidated_filter_list, mz_idxs_per_filter_grp, mass_list_idxs)    
     if normalize_img_sizes:
         pixels = msigen.pixels_list_to_array(pixels, line_list, all_TimeStamps_aligned)
 
     return metadata, pixels 
 
-def get_TIC_agilent(data, line_acq_times):
-    # get TIC object intensities
-    TIC_obj = data.source.GetTIC(data.source)
-    # get TIC intensities
-    TIC = TIC_obj.YArray
-
-    # MRM scans do not return a TIC, so make those scans zero
-    if len(TIC) != len(line_acq_times):
-        # get the time of each intensity value
-        TIC_times = TIC_obj.XArray
-        TIC_idxs = []
-
-        # find which scan each TIC corresponds to
-        for t in TIC_times:
-            TIC_idxs.append(np.where(np.isclose(t, line_acq_times))[0])
-
-        # Make a new TIC array with 0s where a TIC value was missing
-        TICs = np.zeros(len(line_acq_times), dtype = float)
-        for idx1, idx2 in enumerate(TIC_idxs):
-            TICs[idx2] = TIC[idx1]
-        TIC = TICs
-    return TIC
-
 # ================================================================================
 # Bruker General functions
 # ================================================================================
 
 def parse_bruker_scan_level(scanmode):
     if scanmode == 0:
         level = 'MS1'
```

### Comparing `msigen-0.2.1/MSIGen/GUI.py` & `msigen-0.2.2rc1/MSIGen/GUI.py`

 * *Files identical despite different names*

### Comparing `msigen-0.2.1/MSIGen/msigen.py` & `msigen-0.2.2rc1/MSIGen/msigen.py`

 * *Files 0% similar despite different names*

```diff
@@ -712,15 +712,15 @@
     rts_normed = [(line_rts - line_rts.min())/(line_rts.max() - line_rts.min()) for line_rts in rts]
     rts_aligned = np.linspace(0, 1, int(np.mean([len(rts) for rts in rts_normed])))
 
     # Initialize pixels
     pixels_aligned = np.empty([len(line_list), len(rts_aligned), (mass_list.shape[0]+1)])
 
     # Interpolate each line with nearest neighbor to align number of pixels per line
-    X = np.linspace(0, pixels_aligned.shape[-1], len(mass_list)+1)
+    X = np.arange(pixels_aligned.shape[-1])
     for idx, line in enumerate(pixels):
         coords = (rts_normed[idx], X)
         line_pixels_aligned = interpn(coords, line, np.array(np.meshgrid(rts_aligned,X)).reshape(2, -1).transpose(1,0), method='nearest').reshape(X.size, rts_aligned.size)
         pixels_aligned[idx] = line_pixels_aligned.T
         
     # makes axes (m/z, h, w)
     pixels_aligned = np.moveaxis(pixels_aligned, -1, 0)
```

### Comparing `msigen-0.2.1/MSIGen/mzml.py` & `msigen-0.2.2rc1/MSIGen/mzml.py`

 * *Files identical despite different names*

### Comparing `msigen-0.2.1/MSIGen/raw.py` & `msigen-0.2.2rc1/MSIGen/raw.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from tqdm import tqdm
 import numpy as np
 from scipy.interpolate import interpn#, NearestNDInterpolator
 
 # ==================================
 # General functions
 # ==================================
-
 def get_basic_instrument_metadata_raw(data, metadata = {}):
     
     metadata_vars = ['filter_list']
     metadata = msigen.get_attr_values(metadata, data, metadata_vars)
 
     metadata_vars = ['CreationDate']
     source = data.source
@@ -33,14 +32,33 @@
 
     return metadata
 
 
 # ==================================
 # MS1 - No Mobility
 # ==================================
+def get_raw_scan(data, scannum, centroid = False):
+    # Faster implementation of multiplierz scan method for .raw files    
+    scan_stats = data.source.GetScanStatsForScanNumber(scannum)
+    # Does IsCentroidScan indicate that profile data is not available?
+    if centroid or scan_stats.IsCentroidScan:
+        
+        stream = data.source.GetCentroidStream(scannum, False)
+        if stream.Masses is not None and stream.Intensities is not None:
+            return np.array(stream.Masses), np.array(stream.Intensities)
+        else:
+            # Fall back on "profile" mode, which seems to usually turn
+            # out centroid data for some reason.  The format is confused.
+            scan = data.source.GetSegmentedScanFromScanNumber(scannum, scan_stats) 
+            return np.array(scan.Positions), np.array(scan.Intensities)
+    
+    else: # Profile-only scan.
+        scan = data.source.GetSegmentedScanFromScanNumber(scannum, scan_stats)
+        return np.array(scan.Positions), np.array(scan.Intensities)
+
 
 def raw_ms1_no_mob(line_list, mass_lists, lower_lims, upper_lims, experiment_type, metadata, in_jupyter = True, testing = False, gui=False, tkinter_widgets = [None, None, None]):
     '''Takes Thermo .raw files, mass list, and metadata and extracts MS image array.'''
 
     # variables for monitoring progress on gui
     if gui:
         tkinter_widgets[1]['text']="Extracting data"
@@ -57,37 +75,35 @@
     for i, file_dir in tqdm(enumerate(line_list), total = len(line_list), desc='Progress through lines', disable = testing or gui):
         
         # Get relevant data if .raw data.      
         data = mzFile(file_dir)
 
         headers = np.array(data.xic())
         Acq_times = np.round(headers[:,0], 4)
-        TICs = headers[:,1]
         num_spe = len(Acq_times)
 
         line_pixels = np.zeros((num_spe, MS1_list.shape[0]+1))
-        line_pixels[:,0] = TICs
 
         # Get masses for each scan
         for j in tqdm(range(num_spe), desc = 'Progress through line {}'.format(i+1), disable = True):
             # Update line dependent gui variables            
             if gui:
                 tkinter_widgets[0]['value']=(100*i/len(line_list))+((100/len(line_list))*(j/num_spe))
                 tkinter_widgets[0].update()
                 tkinter_widgets[2]['text']=f'line {i+1}/{len(line_list)}, spectrum {j+1}/{num_spe}'
                 tkinter_widgets[2].update()
 
-            scan_stats = data.source.GetScanStatsForScanNumber(j+1)
-            spectrum = data.source.GetSegmentedScanFromScanNumber(j+1, scan_stats)
-            intensity_points = np.array(spectrum.Intensities)
-            # remove all values of zero to improve speed
+            # remove zeros from the arrays for faster slicing
+            mz, intensity_points = get_raw_scan(data, j+1, False)
             intensity_points_mask = np.where(intensity_points)
             intensity_points = np.append(intensity_points[intensity_points_mask[0]],0)
-            # get all m/z values with nonzero intensity
-            mz = np.array(np.array(spectrum.Positions))[intensity_points_mask[0]]
+            mz = mz[intensity_points_mask[0]]            
+
+            # get TIC
+            line_pixels[j-1,0] = np.sum(intensity_points)
 
             if msigen.numba_present:
                 idxs_to_sum = msigen.vectorized_sorted_slice_njit(mz, lb, ub)
                 pixel = msigen.assign_values_to_pixel_njit(intensity_points, idxs_to_sum)
                 line_pixels[j-1,1:] = pixel
             else:
                 idxs_to_sum = msigen.vectorized_sorted_slice(mz, lb, ub) # Slower
@@ -171,15 +187,14 @@
             
             # # collect metadata from raw file
             # if i == 0:
             #     metadata = get_basic_instrument_metadata_raw_no_mob(RawFile, metadata)
 
             # The intensity values for all masses/transitions in the mass list. 0 index in each group = TIC.
             pixels_meta = [ np.zeros((scans_per_filter_grp[i][_] , peak_counts_per_filter_grp[_] + 1)) for _ in range(num_filter_groups) ]
-            TIC = np.array(data.xic())[:,1]
 
             # counts how many times numbers have been inputted each array
             counter = np.zeros((scans_per_filter_grp[0].shape[0])).astype(int)-1 # start from -1, +=1 before handeling
 
             for j, TimeStamp in tqdm(enumerate(acq_times[i]), disable = True):
                 # Update gui variables            
                 if gui:
@@ -190,41 +205,41 @@
 
                 # determine which group is going to be used
                 grp = grp_from_scan_idx[scan_idx]
                 counter[grp]+=1
 
                 # handle info
                 TimeStamps[grp][counter[grp]] = TimeStamp 
+
                 # get spectrum
-                scan_stats = data.source.GetScanStatsForScanNumber(j+1)
-                spectrum = data.source.GetSegmentedScanFromScanNumber(j+1, scan_stats)
-                intensity_points = np.array(spectrum.Intensities)
+                mz, intensity_points = get_raw_scan(data, j+1, False)
 
+                # get TIC
                 pixels_meta[grp][counter[grp], 0] = np.sum(intensity_points)
 
                 # skip filters with no masses in the mass list
                 if peak_counts_per_filter_grp[grp]:
 
                     # remove all values of zero to improve speed
                     intensity_points_mask = np.where(intensity_points)
+                    mz = mz[intensity_points_mask[0]]
                     intensity_points = np.append(intensity_points[intensity_points_mask[0]],0)
-                    # get all m/z values with nonzero intensity
-                    mz = np.array(np.array(spectrum.Positions))[intensity_points_mask[0]]
                     
                     lbs,ubs = mzs_per_filter_grp_lb[grp], mzs_per_filter_grp_ub[grp] 
-                
+
+                    # TODO: Get this to work with the numba workflow
+                    ### did not work properly with numba
                     # if msigen.numba_present:
                     #     idxs_to_sum = msigen.vectorized_sorted_slice_njit(mz, lbs, ubs)
                     #     pixel = msigen.assign_values_to_pixel_njit(intensity_points, idxs_to_sum)
                     #     pixels_meta[grp][counter[grp],1:] = pixel
                     # else:
                     idxs_to_sum = msigen.vectorized_sorted_slice(mz, lbs, ubs) # Slower
                     pixels_meta[grp][counter[grp],1:] = np.sum(np.take(intensity_points, idxs_to_sum), axis = 1)
 
-
                 # keep count of the 1d scan index
                 scan_idx += 1
 
             data.close()
 
         all_TimeStamps.append(TimeStamps)
         pixels_metas.append(pixels_meta)
```

### Comparing `msigen-0.2.1/MSIGen/timsdata.dll` & `msigen-0.2.2rc1/MSIGen/timsdata.dll`

 * *Files identical despite different names*

### Comparing `msigen-0.2.1/MSIGen/tsf.py` & `msigen-0.2.2rc1/MSIGen/tsf.py`

 * *Files identical despite different names*

### Comparing `msigen-0.2.1/MSIGen/visualization.py` & `msigen-0.2.2rc1/MSIGen/visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,18 +370,18 @@
                          MSI_data_output = None, cmap = 'viridis', log_scale = False, threshold = None, \
                          title_fontsize = 10, idxs = [1,2], image_savetype = 'figure'):    
 
     mass_list = metadata["final_mass_list"]
     default_titles = determine_titles(mass_list, idxs = idxs, ratio_img = True)
 
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
@@ -484,12 +484,13 @@
         if log_scale:
             # Prevent -inf values from taking log of zero
             min_thre = np.min(img[np.nonzero(img)])/10
             min_thre_img = np.where(img==0, min_thre, img)
             img = np.log10(min_thre_img)
             thre = np.log10(thre)
         img = np.where(img>thre, thre, img)
-        try:
-            np.savetxt(os.path.join(img_output_folder,title.replace(':','_').replace('\n',' ').replace('>','').replace('/','')+"_threshold-"+str(thre)+'.csv'), img, delimiter=",")
-        except:
-            np.savetxt(os.path.join(img_output_folder,default_title.replace(':','_').replace('\n',' ').replace('>','').replace('/','')+"_threshold-"+str(thre)+'.csv'), img, delimiter=",")
-            
+        if save_imgs: 
+            try:
+                np.savetxt(os.path.join(img_output_folder,title.replace(':','_').replace('\n',' ').replace('>','').replace('/','')+"_threshold-"+str(thre)+'.csv'), img, delimiter=",")
+            except:
+                np.savetxt(os.path.join(img_output_folder,default_title.replace(':','_').replace('\n',' ').replace('>','').replace('/','')+"_threshold-"+str(thre)+'.csv'), img, delimiter=",")
+
```

### Comparing `msigen-0.2.1/pyproject.toml` & `msigen-0.2.2rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msigen"
-version = "0.2.1"
+version = "0.2.2rc1"
 description = "A package for converting spectrometry imaging line scan data files to a visualizable format"
 authors = ["Emerson Hernly <elhernly@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/LabLaskin/MSIGen"
 homepage = "https://github.com/LabLaskin/MSIGen"
```

### Comparing `msigen-0.2.1/README.md` & `msigen-0.2.2rc1/README.md`

 * *Files identical despite different names*

### Comparing `msigen-0.2.1/PKG-INFO` & `msigen-0.2.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msigen
-Version: 0.2.1
+Version: 0.2.2rc1
 Summary: A package for converting spectrometry imaging line scan data files to a visualizable format
 Home-page: https://github.com/LabLaskin/MSIGen
 License: MIT
 Author: Emerson Hernly
 Author-email: elhernly@gmail.com
 Requires-Python: >=3.9.0,<3.12
 Classifier: Development Status :: 4 - Beta
```

