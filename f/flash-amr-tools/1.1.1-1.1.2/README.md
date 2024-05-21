# Comparing `tmp/flash_amr_tools-1.1.1.tar.gz` & `tmp/flash_amr_tools-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flash_amr_tools-1.1.1.tar", last modified: Wed May  8 13:17:49 2024, max compression
+gzip compressed data, was "flash_amr_tools-1.1.2.tar", last modified: Tue May 21 22:40:34 2024, max compression
```

## Comparing `flash_amr_tools-1.1.1.tar` & `flash_amr_tools-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-08 13:17:49.188599 flash_amr_tools-1.1.1/
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     1501 2024-04-30 14:06:17.000000 flash_amr_tools-1.1.1/LICENSE
--rw-r--r--   0 watanabe  (1000) watanabe  (1000)     6916 2024-05-08 13:17:49.188599 flash_amr_tools-1.1.1/PKG-INFO
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     4502 2024-05-08 13:13:17.000000 flash_amr_tools-1.1.1/README.md
-drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-08 13:17:49.188599 flash_amr_tools-1.1.1/flash_amr_tools/
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       74 2024-05-08 13:13:17.000000 flash_amr_tools-1.1.1/flash_amr_tools/__init__.py
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)    19965 2024-05-08 13:13:17.000000 flash_amr_tools-1.1.1/flash_amr_tools/amr_tools.py
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     9694 2024-05-08 13:13:17.000000 flash_amr_tools-1.1.1/flash_amr_tools/block_tools.py
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     8991 2024-04-30 14:06:32.000000 flash_amr_tools-1.1.1/flash_amr_tools/zorder.py
-drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-08 13:17:49.188599 flash_amr_tools-1.1.1/flash_amr_tools.egg-info/
--rw-r--r--   0 watanabe  (1000) watanabe  (1000)     6916 2024-05-08 13:17:49.000000 flash_amr_tools-1.1.1/flash_amr_tools.egg-info/PKG-INFO
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)      363 2024-05-08 13:17:49.000000 flash_amr_tools-1.1.1/flash_amr_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)        1 2024-05-08 13:17:49.000000 flash_amr_tools-1.1.1/flash_amr_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       44 2024-05-08 13:17:49.000000 flash_amr_tools-1.1.1/flash_amr_tools.egg-info/requires.txt
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       16 2024-05-08 13:17:49.000000 flash_amr_tools-1.1.1/flash_amr_tools.egg-info/top_level.txt
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)      737 2024-05-08 13:13:17.000000 flash_amr_tools-1.1.1/pyproject.toml
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       38 2024-05-08 13:17:49.188599 flash_amr_tools-1.1.1/setup.cfg
-drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-08 13:17:49.188599 flash_amr_tools-1.1.1/tests/
--rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     3557 2024-05-08 13:13:17.000000 flash_amr_tools-1.1.1/tests/test_amrtools.py
+drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-21 22:40:34.132785 flash_amr_tools-1.1.2/
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     1501 2024-04-30 14:06:17.000000 flash_amr_tools-1.1.2/LICENSE
+-rw-r--r--   0 watanabe  (1000) watanabe  (1000)     6916 2024-05-21 22:40:34.132785 flash_amr_tools-1.1.2/PKG-INFO
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     4502 2024-05-08 13:13:17.000000 flash_amr_tools-1.1.2/README.md
+drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-21 22:40:34.128785 flash_amr_tools-1.1.2/flash_amr_tools/
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       74 2024-05-08 13:13:17.000000 flash_amr_tools-1.1.2/flash_amr_tools/__init__.py
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)    20160 2024-05-21 22:22:18.000000 flash_amr_tools-1.1.2/flash_amr_tools/amr_tools.py
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     9733 2024-05-21 22:22:02.000000 flash_amr_tools-1.1.2/flash_amr_tools/block_tools.py
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     8991 2024-04-30 14:06:32.000000 flash_amr_tools-1.1.2/flash_amr_tools/zorder.py
+drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-21 22:40:34.132785 flash_amr_tools-1.1.2/flash_amr_tools.egg-info/
+-rw-r--r--   0 watanabe  (1000) watanabe  (1000)     6916 2024-05-21 22:40:34.000000 flash_amr_tools-1.1.2/flash_amr_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)      363 2024-05-21 22:40:34.000000 flash_amr_tools-1.1.2/flash_amr_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)        1 2024-05-21 22:40:34.000000 flash_amr_tools-1.1.2/flash_amr_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       44 2024-05-21 22:40:34.000000 flash_amr_tools-1.1.2/flash_amr_tools.egg-info/requires.txt
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       16 2024-05-21 22:40:34.000000 flash_amr_tools-1.1.2/flash_amr_tools.egg-info/top_level.txt
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)      737 2024-05-21 22:38:05.000000 flash_amr_tools-1.1.2/pyproject.toml
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)       38 2024-05-21 22:40:34.132785 flash_amr_tools-1.1.2/setup.cfg
+drwxrwxr-x   0 watanabe  (1000) watanabe  (1000)        0 2024-05-21 22:40:34.132785 flash_amr_tools-1.1.2/tests/
+-rw-rw-r--   0 watanabe  (1000) watanabe  (1000)     3557 2024-05-08 13:13:17.000000 flash_amr_tools-1.1.2/tests/test_amrtools.py
```

### Comparing `flash_amr_tools-1.1.1/LICENSE` & `flash_amr_tools-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flash_amr_tools-1.1.1/PKG-INFO` & `flash_amr_tools-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flash_amr_tools
-Version: 1.1.1
+Version: 1.1.2
 Summary: Small tool to create uniform data cubes of FLASH datasets. Port from bitbucket.org/pierrenbg/flash-amr-tools
 Author-email: Keito Watanabe <k.wat8973@gmail.com>, Pierre Nürnberger <nuernb@ph1.uni-koeln.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Keito Watanabe
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `flash_amr_tools-1.1.1/README.md` & `flash_amr_tools-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `flash_amr_tools-1.1.1/flash_amr_tools/amr_tools.py` & `flash_amr_tools-1.1.2/flash_amr_tools/amr_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,25 +13,26 @@
 def get_true_blocks(
         fname: str,
         xmin=np.array([], dtype=np.float32),
         xmax=np.array([], dtype=np.float32),
         is_cuboid=True,
         max_ref_given=None,
         min_ref_given=None,
+        verbose=True,
     ):
     '''
     Extract the complete list of blocks which are in the box chosen within xmin and xmax. In particular, it sets the minimum & maximum refinement within the block list, and the number of blocks in x, y, z on the lowest refinement level.
 
     - fname (str): the filename of the FLASH output file. needs to be a .h5 file
     - xmin (3-D array): the lower corner of the region of interest. Defaults to empty array, which uses the whole domain
     - xmax (3-D array): the upper corner of the region of interest. Defaults to empty array, which uses the whole domain
     - is_cuboid (bool): set to True if the region is not a cube. Defaults to True.
     - max_ref_given (int): force the maximum refinement level of the blocks. Defaults to None, which uses the maximum refinement level in the simulation.
     - min_ref_given (int): force the minimum refinement level of the blocks. Defaults to None, which uses the minimum refinement level in the simulation.
-
+    - verbose (bool) : show print statements or not.
 
     Returns:
     - blist (list) : the list of blocks that cover the region of interest 
     - brefs (list) : the maximum & minimum refinement level within the region of interest
     - bns (list) : returns the number of blocks in (x, y, z) direction at the lowest refinement level
     '''
 
@@ -81,17 +82,17 @@
     # Sanity check coordinates
     if np.any(xmax < xmin):
         sys.exit(
             'Check coordinates. Some value in xmin is larger than xmax.\n' +
             'xmin : %s\t%s\t%s\n' % tuple(xmin) +
             'xmax : %s\t%s\t%s\n' % tuple(xmax)
         )
-
-    print("minimum position of the region of interest: ", xmin)
-    print("maximum position of the region of interest: ", xmax)
+    if verbose:
+        print("minimum position of the region of interest: ", xmin)
+        print("maximum position of the region of interest: ", xmax)
 
     # Find all leaf blocks for inner and outer borders
     # Inner borders only includes blocks which center coordinate is included in selected region.
     # Outer borders also includes blocks which intersect with the selected region. Those variables are denoted with a 2.
     print('Finding all leaf blocks in given region')
     ind = np.argwhere(np.all(gid[:, 7:] == -1, axis=1)).T[0]
     tmpc = coords[ind]
@@ -131,17 +132,18 @@
         if min_ref_given < min_ref2:
             min_ref2 = min_ref_given
 
     max_ref_reg = brlvl.max()
     max_ref_reg2 = brlvl2.max()
 
     max_ref = refine_level[ind].max()
-    print('Biggest block has refinement level: %s' % min_ref)
-    print('Highest refinement level in simulation: %s' % max_ref)
-    print('Highest refinement level in selected box: %s' % max_ref_reg)
+    if verbose:
+        print('Biggest block has refinement level: %s' % min_ref)
+        print('Highest refinement level in simulation: %s' % max_ref)
+        print('Highest refinement level in selected box: %s' % max_ref_reg)
 
     print('Extending region to fit amr structure at level %s.' % min_ref)
     blist_minref, bx, by, bz, bmax = find_blocks(
         block_list=blist_raw, min_ref_lvl=min_ref, max_ref_lvl=max_ref, block_size=block_size, brlvl=brlvl, bsmin=bsmin,
         coords=coords, gid=gid, refine_level=refine_level, center=(xmin+xmax)/2., is_cuboid=is_cuboid
     )
 
@@ -192,31 +194,32 @@
         blvl = min_ref - np.int32(np.round(np.log2(bmax)))
         
     if max_ref_given != None:
         max_ref = max_ref_given
 
     blist_maxref, b_tot_nr = create_blists(
         minref_blist=blist_minref, block_level=blvl, gid=gid, coords=coords, max_ref_lvl=max_ref,
-        bnx=bx, bny=by, bnz=bz, is_cuboid=is_cuboid
+        bnx=bx, bny=by, bnz=bz, is_cuboid=is_cuboid, verbose=verbose,
     )
 
     if not is_cuboid:
         b_tot_nr += np.sum(np.logspace(start=0., stop=np.log2(bmax)-1, base=2, num=int(np.log2(bmax)))**3).astype(int)
 
-    print('Total number of blocks including parent blocks: %s' % b_tot_nr)
+    if verbose:
+        print('Total number of blocks including parent blocks: %s' % b_tot_nr)
 
-    boundariesl = np.min(coords[blist_maxref] - 0.5 * block_size[blist_maxref], axis=0)
-    boundariesr = np.max(coords[blist_maxref] + 0.5 * block_size[blist_maxref], axis=0)
-    print('Region extended to:\tlower\t\tupper')
-    print('\tx\t%+1.8e\t\t%+1.8e' % (boundariesl[0], boundariesr[0]))
-    print('\ty\t%+1.8e\t\t%+1.8e' % (boundariesl[1], boundariesr[1]))
-    print('\tz\t%+1.8e\t\t%+1.8e\n' % (boundariesl[2], boundariesr[2]))
+        boundariesl = np.min(coords[blist_maxref] - 0.5 * block_size[blist_maxref], axis=0)
+        boundariesr = np.max(coords[blist_maxref] + 0.5 * block_size[blist_maxref], axis=0)
+        print('Region extended to:\tlower\t\tupper')
+        print('\tx\t%+1.8e\t\t%+1.8e' % (boundariesl[0], boundariesr[0]))
+        print('\ty\t%+1.8e\t\t%+1.8e' % (boundariesl[1], boundariesr[1]))
+        print('\tz\t%+1.8e\t\t%+1.8e\n' % (boundariesl[2], boundariesr[2]))
 
-    print('Region center at:\t%+1.8e\t%+1.8e\t%+1.8e' % tuple((boundariesl+boundariesr)/2))
-    print('Given center:\t\t%+1.8e\t%+1.8e\t%+1.8e' % tuple((xmin+xmax)/2))
+        print('Region center at:\t%+1.8e\t%+1.8e\t%+1.8e' % tuple((boundariesl+boundariesr)/2))
+        print('Given center:\t\t%+1.8e\t%+1.8e\t%+1.8e' % tuple((xmin+xmax)/2))
 
     # return min & maximum refinement levels in the block, block list, and number of blocks in each direction
     bns = [bx, by, bz]
     brefs = [max_ref, min_ref]
 
     return blist_maxref, brefs, bns
```

### Comparing `flash_amr_tools-1.1.1/flash_amr_tools/block_tools.py` & `flash_amr_tools-1.1.2/flash_amr_tools/block_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -159,21 +159,22 @@
     # Add new blocks to the current list of blocks at lowest refinement level.
     minref_blist = np.unique(np.concatenate((minref_blist, new_b_p, new_b_m))).astype(int)
 
     return minref_blist, bn[0], bn[1], bn[2]
 
 
 # Sort all blocks at minimum refinement level and replace block with their higher refinement level counterparts.
-def create_blists(minref_blist, max_ref_lvl, block_level, gid, coords, bnx=0, bny=0, bnz=0, is_cuboid=False):
+def create_blists(minref_blist, max_ref_lvl, block_level, gid, coords, bnx=0, bny=0, bnz=0, is_cuboid=False, verbose=False):
 
     # Put the block of the minimum refinement level on a grid correspoding to their coordinates.
     # Change axes to be in order of x, y and z.
     blist_minsort_tmp = blocks_on_grid(b_ids=minref_blist, coords=coords, bnx=bnx, bny=bny, bnz=bnz).swapaxes(0, 2)
-    print('bnx, bny, bnz: ', bnx, bny, bnz)
-    print('Block shape: ', blist_minsort_tmp.shape)
+    if verbose:
+        print('bnx, bny, bnz: ', bnx, bny, bnz)
+        print('Block shape: ', blist_minsort_tmp.shape)
     blist_minsort = []
     # Add blocks in amr order to list.
     if is_cuboid:
         blist_minsort = blist_minsort_tmp.swapaxes(0, 2).flatten()
     else:
         for pos in zenumerate(blist_minsort_tmp.shape):
             blist_minsort.append(blist_minsort_tmp[pos])
```

### Comparing `flash_amr_tools-1.1.1/flash_amr_tools/zorder.py` & `flash_amr_tools-1.1.2/flash_amr_tools/zorder.py`

 * *Files identical despite different names*

### Comparing `flash_amr_tools-1.1.1/flash_amr_tools.egg-info/PKG-INFO` & `flash_amr_tools-1.1.2/flash_amr_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flash_amr_tools
-Version: 1.1.1
+Version: 1.1.2
 Summary: Small tool to create uniform data cubes of FLASH datasets. Port from bitbucket.org/pierrenbg/flash-amr-tools
 Author-email: Keito Watanabe <k.wat8973@gmail.com>, Pierre Nürnberger <nuernb@ph1.uni-koeln.de>
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Keito Watanabe
         
         Redistribution and use in source and binary forms, with or without
```

### Comparing `flash_amr_tools-1.1.1/tests/test_amrtools.py` & `flash_amr_tools-1.1.2/tests/test_amrtools.py`

 * *Files identical despite different names*

