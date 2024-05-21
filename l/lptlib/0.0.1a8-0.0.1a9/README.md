# Comparing `tmp/lptlib-0.0.1a8.tar.gz` & `tmp/lptlib-0.0.1a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lptlib-0.0.1a8.tar", last modified: Tue May 14 01:07:59 2024, max compression
+gzip compressed data, was "lptlib-0.0.1a9.tar", last modified: Sat May 18 01:47:47 2024, max compression
```

## Comparing `lptlib-0.0.1a8.tar` & `lptlib-0.0.1a9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-14 01:07:59.948164 lptlib-0.0.1a8/
--rwx------   0 kal        (501) staff       (20)     1093 2024-05-10 20:01:36.000000 lptlib-0.0.1a8/LICENSE
--rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-14 01:07:59.947672 lptlib-0.0.1a8/PKG-INFO
--rw-r--r--   0 kal        (501) staff       (20)      579 2024-05-13 17:06:24.000000 lptlib-0.0.1a8/README.md
--rw-r--r--   0 kal        (501) staff       (20)     1085 2024-05-14 01:07:40.000000 lptlib-0.0.1a8/pyproject.toml
--rw-r--r--   0 kal        (501) staff       (20)       38 2024-05-14 01:07:59.948297 lptlib-0.0.1a8/setup.cfg
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-14 01:07:59.905975 lptlib-0.0.1a8/src/
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-14 01:07:59.909656 lptlib-0.0.1a8/src/lptlib/
--rw-r--r--   0 kal        (501) staff       (20)      122 2024-05-14 00:59:59.000000 lptlib-0.0.1a8/src/lptlib/__init__.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-14 01:07:59.916633 lptlib-0.0.1a8/src/lptlib/function/
--rw-r--r--   0 kal        (501) staff       (20)      109 2024-01-23 01:40:32.000000 lptlib-0.0.1a8/src/lptlib/function/__init__.py
--rwx------   0 kal        (501) staff       (20)    12533 2024-05-13 21:39:16.000000 lptlib-0.0.1a8/src/lptlib/function/plots.py
--rw-r--r--   0 kal        (501) staff       (20)     2034 2024-01-23 01:40:32.000000 lptlib-0.0.1a8/src/lptlib/function/timer.py
--rw-r--r--   0 kal        (501) staff       (20)    11942 2024-05-13 23:27:55.000000 lptlib-0.0.1a8/src/lptlib/function/variables.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-14 01:07:59.921292 lptlib-0.0.1a8/src/lptlib/io/
--rw-r--r--   0 kal        (501) staff       (20)       91 2024-01-23 01:40:32.000000 lptlib-0.0.1a8/src/lptlib/io/__init__.py
--rw-r--r--   0 kal        (501) staff       (20)    14877 2024-05-13 21:52:46.000000 lptlib-0.0.1a8/src/lptlib/io/dataio.py
--rw-r--r--   0 kal        (501) staff       (20)    24440 2024-04-22 21:46:04.000000 lptlib-0.0.1a8/src/lptlib/io/plot3dio.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-14 01:07:59.935661 lptlib-0.0.1a8/src/lptlib/streamlines/
--rw-r--r--   0 kal        (501) staff       (20)      257 2024-01-23 01:40:32.000000 lptlib-0.0.1a8/src/lptlib/streamlines/__init__.py
--rw-r--r--   0 kal        (501) staff       (20)    34469 2024-05-13 21:54:19.000000 lptlib-0.0.1a8/src/lptlib/streamlines/integration.py
--rw-r--r--   0 kal        (501) staff       (20)    47329 2024-05-13 23:27:55.000000 lptlib-0.0.1a8/src/lptlib/streamlines/interpolation.py
--rwxr-xr-x   0 kal        (501) staff       (20)    15615 2024-05-13 17:24:06.000000 lptlib-0.0.1a8/src/lptlib/streamlines/search.py
--rw-r--r--   0 kal        (501) staff       (20)     7537 2024-05-13 21:50:14.000000 lptlib-0.0.1a8/src/lptlib/streamlines/stochastic_model.py
--rw-r--r--   0 kal        (501) staff       (20)    39727 2024-05-13 21:49:30.000000 lptlib-0.0.1a8/src/lptlib/streamlines/streamlines.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-14 01:07:59.939786 lptlib-0.0.1a8/src/lptlib/test_cases/
--rwx------   0 kal        (501) staff       (20)       89 2024-01-23 01:40:32.000000 lptlib-0.0.1a8/src/lptlib/test_cases/__init__.py
--rwx------   0 kal        (501) staff       (20)     9741 2024-05-14 01:00:49.000000 lptlib-0.0.1a8/src/lptlib/test_cases/oblique_shock_data.py
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-14 01:07:59.946982 lptlib-0.0.1a8/src/lptlib.egg-info/
--rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-14 01:07:59.000000 lptlib-0.0.1a8/src/lptlib.egg-info/PKG-INFO
--rw-r--r--   0 kal        (501) staff       (20)     1010 2024-05-14 01:07:59.000000 lptlib-0.0.1a8/src/lptlib.egg-info/SOURCES.txt
--rw-r--r--   0 kal        (501) staff       (20)        1 2024-05-14 01:07:59.000000 lptlib-0.0.1a8/src/lptlib.egg-info/dependency_links.txt
--rw-r--r--   0 kal        (501) staff       (20)       43 2024-05-14 01:07:59.000000 lptlib-0.0.1a8/src/lptlib.egg-info/requires.txt
--rw-r--r--   0 kal        (501) staff       (20)        7 2024-05-14 01:07:59.000000 lptlib-0.0.1a8/src/lptlib.egg-info/top_level.txt
-drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-14 01:07:59.946331 lptlib-0.0.1a8/test/
--rw-r--r--   0 kal        (501) staff       (20)     1017 2024-05-13 22:59:21.000000 lptlib-0.0.1a8/test/test_dataio.py
--rwx------   0 kal        (501) staff       (20)      471 2024-05-13 23:04:33.000000 lptlib-0.0.1a8/test/test_import.py
--rwx------   0 kal        (501) staff       (20)     2366 2024-05-13 23:04:33.000000 lptlib-0.0.1a8/test/test_integration.py
--rw-r--r--   0 kal        (501) staff       (20)     2039 2024-05-13 23:04:33.000000 lptlib-0.0.1a8/test/test_interpolation.py
--rwx------   0 kal        (501) staff       (20)     1202 2024-05-13 23:04:33.000000 lptlib-0.0.1a8/test/test_oblique_shock_data.py
--rw-r--r--   0 kal        (501) staff       (20)     2059 2023-08-17 08:22:42.000000 lptlib-0.0.1a8/test/test_plot.py
--rw-r--r--   0 kal        (501) staff       (20)     7334 2024-05-13 23:04:33.000000 lptlib-0.0.1a8/test/test_plot3dio.py
--rwx------   0 kal        (501) staff       (20)     2641 2024-05-13 23:04:33.000000 lptlib-0.0.1a8/test/test_plots.py
--rw-r--r--   0 kal        (501) staff       (20)     3276 2024-05-13 23:04:33.000000 lptlib-0.0.1a8/test/test_search.py
--rw-r--r--   0 kal        (501) staff       (20)     1943 2024-05-13 23:04:33.000000 lptlib-0.0.1a8/test/test_stochastic_model.py
--rw-r--r--   0 kal        (501) staff       (20)     1428 2024-05-13 23:04:33.000000 lptlib-0.0.1a8/test/test_terminal_run.py
--rwx------   0 kal        (501) staff       (20)     2744 2024-05-13 23:04:33.000000 lptlib-0.0.1a8/test/test_variables.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-18 01:47:47.333295 lptlib-0.0.1a9/
+-rwx------   0 kal        (501) staff       (20)     1093 2024-05-10 20:01:36.000000 lptlib-0.0.1a9/LICENSE
+-rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-18 01:47:47.332550 lptlib-0.0.1a9/PKG-INFO
+-rw-r--r--   0 kal        (501) staff       (20)      579 2024-05-13 17:06:24.000000 lptlib-0.0.1a9/README.md
+-rw-r--r--   0 kal        (501) staff       (20)     1085 2024-05-18 01:47:38.000000 lptlib-0.0.1a9/pyproject.toml
+-rw-r--r--   0 kal        (501) staff       (20)       38 2024-05-18 01:47:47.333447 lptlib-0.0.1a9/setup.cfg
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-18 01:47:47.299656 lptlib-0.0.1a9/src/
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-18 01:47:47.303532 lptlib-0.0.1a9/src/lptlib/
+-rw-r--r--   0 kal        (501) staff       (20)      122 2024-05-14 00:59:59.000000 lptlib-0.0.1a9/src/lptlib/__init__.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-18 01:47:47.308482 lptlib-0.0.1a9/src/lptlib/function/
+-rw-r--r--   0 kal        (501) staff       (20)      109 2024-01-23 01:40:32.000000 lptlib-0.0.1a9/src/lptlib/function/__init__.py
+-rwx------   0 kal        (501) staff       (20)    12533 2024-05-13 21:39:16.000000 lptlib-0.0.1a9/src/lptlib/function/plots.py
+-rw-r--r--   0 kal        (501) staff       (20)     2034 2024-01-23 01:40:32.000000 lptlib-0.0.1a9/src/lptlib/function/timer.py
+-rw-r--r--   0 kal        (501) staff       (20)    11942 2024-05-13 23:27:55.000000 lptlib-0.0.1a9/src/lptlib/function/variables.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-18 01:47:47.312332 lptlib-0.0.1a9/src/lptlib/io/
+-rw-r--r--   0 kal        (501) staff       (20)       91 2024-01-23 01:40:32.000000 lptlib-0.0.1a9/src/lptlib/io/__init__.py
+-rw-r--r--   0 kal        (501) staff       (20)    14877 2024-05-13 21:52:46.000000 lptlib-0.0.1a9/src/lptlib/io/dataio.py
+-rw-r--r--   0 kal        (501) staff       (20)    24440 2024-04-22 21:46:04.000000 lptlib-0.0.1a9/src/lptlib/io/plot3dio.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-18 01:47:47.318212 lptlib-0.0.1a9/src/lptlib/streamlines/
+-rw-r--r--   0 kal        (501) staff       (20)      257 2024-01-23 01:40:32.000000 lptlib-0.0.1a9/src/lptlib/streamlines/__init__.py
+-rw-r--r--   0 kal        (501) staff       (20)    34469 2024-05-13 21:54:19.000000 lptlib-0.0.1a9/src/lptlib/streamlines/integration.py
+-rw-r--r--   0 kal        (501) staff       (20)    47329 2024-05-13 23:27:55.000000 lptlib-0.0.1a9/src/lptlib/streamlines/interpolation.py
+-rwxr-xr-x   0 kal        (501) staff       (20)    15615 2024-05-13 17:24:06.000000 lptlib-0.0.1a9/src/lptlib/streamlines/search.py
+-rw-r--r--   0 kal        (501) staff       (20)     7583 2024-05-17 20:14:47.000000 lptlib-0.0.1a9/src/lptlib/streamlines/stochastic_model.py
+-rw-r--r--   0 kal        (501) staff       (20)    39828 2024-05-16 05:24:05.000000 lptlib-0.0.1a9/src/lptlib/streamlines/streamlines.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-18 01:47:47.320369 lptlib-0.0.1a9/src/lptlib/test_cases/
+-rwx------   0 kal        (501) staff       (20)       89 2024-01-23 01:40:32.000000 lptlib-0.0.1a9/src/lptlib/test_cases/__init__.py
+-rwx------   0 kal        (501) staff       (20)     9741 2024-05-14 01:00:49.000000 lptlib-0.0.1a9/src/lptlib/test_cases/oblique_shock_data.py
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-18 01:47:47.331672 lptlib-0.0.1a9/src/lptlib.egg-info/
+-rw-r--r--   0 kal        (501) staff       (20)     1545 2024-05-18 01:47:47.000000 lptlib-0.0.1a9/src/lptlib.egg-info/PKG-INFO
+-rw-r--r--   0 kal        (501) staff       (20)     1010 2024-05-18 01:47:47.000000 lptlib-0.0.1a9/src/lptlib.egg-info/SOURCES.txt
+-rw-r--r--   0 kal        (501) staff       (20)        1 2024-05-18 01:47:47.000000 lptlib-0.0.1a9/src/lptlib.egg-info/dependency_links.txt
+-rw-r--r--   0 kal        (501) staff       (20)       43 2024-05-18 01:47:47.000000 lptlib-0.0.1a9/src/lptlib.egg-info/requires.txt
+-rw-r--r--   0 kal        (501) staff       (20)        7 2024-05-18 01:47:47.000000 lptlib-0.0.1a9/src/lptlib.egg-info/top_level.txt
+drwxr-xr-x   0 kal        (501) staff       (20)        0 2024-05-18 01:47:47.330731 lptlib-0.0.1a9/test/
+-rw-r--r--   0 kal        (501) staff       (20)     1017 2024-05-13 22:59:21.000000 lptlib-0.0.1a9/test/test_dataio.py
+-rwx------   0 kal        (501) staff       (20)      471 2024-05-13 23:04:33.000000 lptlib-0.0.1a9/test/test_import.py
+-rwx------   0 kal        (501) staff       (20)     2366 2024-05-13 23:04:33.000000 lptlib-0.0.1a9/test/test_integration.py
+-rw-r--r--   0 kal        (501) staff       (20)     2039 2024-05-13 23:04:33.000000 lptlib-0.0.1a9/test/test_interpolation.py
+-rwx------   0 kal        (501) staff       (20)     1202 2024-05-13 23:04:33.000000 lptlib-0.0.1a9/test/test_oblique_shock_data.py
+-rw-r--r--   0 kal        (501) staff       (20)     2059 2023-08-17 08:22:42.000000 lptlib-0.0.1a9/test/test_plot.py
+-rw-r--r--   0 kal        (501) staff       (20)     7334 2024-05-13 23:04:33.000000 lptlib-0.0.1a9/test/test_plot3dio.py
+-rwx------   0 kal        (501) staff       (20)     2641 2024-05-13 23:04:33.000000 lptlib-0.0.1a9/test/test_plots.py
+-rw-r--r--   0 kal        (501) staff       (20)     3276 2024-05-13 23:04:33.000000 lptlib-0.0.1a9/test/test_search.py
+-rw-r--r--   0 kal        (501) staff       (20)     1943 2024-05-13 23:04:33.000000 lptlib-0.0.1a9/test/test_stochastic_model.py
+-rw-r--r--   0 kal        (501) staff       (20)     1428 2024-05-13 23:04:33.000000 lptlib-0.0.1a9/test/test_terminal_run.py
+-rwx------   0 kal        (501) staff       (20)     2744 2024-05-13 23:04:33.000000 lptlib-0.0.1a9/test/test_variables.py
```

### Comparing `lptlib-0.0.1a8/LICENSE` & `lptlib-0.0.1a9/LICENSE`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/PKG-INFO` & `lptlib-0.0.1a9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lptlib
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: One-way coupled Lagrangian Particle Tracking algorithms.
 Author: Dilip Kalagotla
 Author-email: dilipkalagotla@gmail.com
 Project-URL: homepage, https://github.com/kalagotla/project-arrakis
 Project-URL: issues, https://github.com/kalagotla/project-arrakis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lptlib-0.0.1a8/README.md` & `lptlib-0.0.1a9/README.md`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/pyproject.toml` & `lptlib-0.0.1a9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lptlib"
-version = "0.0.1a8"
+version = "0.0.1a9"
 authors = [
     {name="Dilip Kalagotla"},
     {email="dilipkalagotla@gmail.com"},
     ]
 description = "One-way coupled Lagrangian Particle Tracking algorithms."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `lptlib-0.0.1a8/src/lptlib/function/plots.py` & `lptlib-0.0.1a9/src/lptlib/function/plots.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/src/lptlib/function/timer.py` & `lptlib-0.0.1a9/src/lptlib/function/timer.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/src/lptlib/function/variables.py` & `lptlib-0.0.1a9/src/lptlib/function/variables.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/src/lptlib/io/dataio.py` & `lptlib-0.0.1a9/src/lptlib/io/dataio.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/src/lptlib/io/plot3dio.py` & `lptlib-0.0.1a9/src/lptlib/io/plot3dio.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/src/lptlib/streamlines/integration.py` & `lptlib-0.0.1a9/src/lptlib/streamlines/integration.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/src/lptlib/streamlines/interpolation.py` & `lptlib-0.0.1a9/src/lptlib/streamlines/interpolation.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/src/lptlib/streamlines/search.py` & `lptlib-0.0.1a9/src/lptlib/streamlines/search.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/src/lptlib/streamlines/stochastic_model.py` & `lptlib-0.0.1a9/src/lptlib/streamlines/stochastic_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         self.particles = particles
         self.spawn_locations = spawn_locations
         # Read-in grid and flow files
         self.grid = grid
         self.flow = flow
         self.method = method
         self.chunksize = 32
+        self.cpu_count = mp.cpu_count()
 
     def setup(self, spawn_location, particle_dia, task):
         """
         Sets up the function to be run in parallel
         Args:
             self:
             spawn_location:
@@ -67,28 +68,28 @@
         """
         To parallelize using multiprocessing approach; the setup function
         Returns:
 
         """
         # track progress using tqdm
         inputs = zip(self.spawn_locations.locations, self.particles.particle_field, np.arange(self.particles.n_concentration))
-        with mp.Pool(mp.cpu_count() - 1) as pool:
+        with mp.Pool(self.cpu_count) as pool:
             lpt_data = pool.starmap(self.setup, tqdm(inputs, total=self.particles.n_concentration), chunksize=self.chunksize)
 
         return lpt_data
 
     def multi_thread(self):
         """
         To parallelize using multithreading approach; the setup function
         Returns:
 
         """
-        with Pool(mp.cpu_count() - 1) as pool:
+        with Pool(self.cpu_count) as pool:
             lpt_data = pool.starmap(self.setup, zip(self.spawn_locations.locations, self.particles.particle_field,
-                                                    np.arange(self.particles.n_concentration)), chunksize=1)
+                                                    np.arange(self.particles.n_concentration)), chunksize=self.chunksize)
 
         return lpt_data
 
     def serial(self):
         """
         To run setup in serial
         Returns:
```

### Comparing `lptlib-0.0.1a8/src/lptlib/streamlines/streamlines.py` & `lptlib-0.0.1a9/src/lptlib/streamlines/streamlines.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,17 @@
             for _i in range(1, len(f_xdata)):
                 f_xdata[_i] = f_xdata[_i - 1] + udata[_i - 1] * tdata[_i - 1]
             # Data is added towards the end because of the development cycle. Mostly to work with dataio
             _data_save = np.hstack((p_xdata, vdata, udata, tdata, f_xdata,
                                     np.ones(tdata.shape) * self.diameter,
                                     np.ones(tdata.shape) * self.density))
 
-            np.save(self.filepath + 'ppath_' + str(self.task), _data_save)
+            # help closes the file after writing
+            with open(self.filepath + 'ppath_' + str(self.task) + '.npy', 'wb') as f:
+                np.save(f, _data_save)
             self.print_debug(self, '** SUCCESS ** Done writing file for particle number - ' + str(self.task) + ' ** SUCCESS **')
             # set self to None to clear up memory after saving required data
             self.streamline = []
             self.svelocity = []
             self.fvelocity = []
             self.time = []
         return
```

### Comparing `lptlib-0.0.1a8/src/lptlib/test_cases/oblique_shock_data.py` & `lptlib-0.0.1a9/src/lptlib/test_cases/oblique_shock_data.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/src/lptlib.egg-info/PKG-INFO` & `lptlib-0.0.1a9/src/lptlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lptlib
-Version: 0.0.1a8
+Version: 0.0.1a9
 Summary: One-way coupled Lagrangian Particle Tracking algorithms.
 Author: Dilip Kalagotla
 Author-email: dilipkalagotla@gmail.com
 Project-URL: homepage, https://github.com/kalagotla/project-arrakis
 Project-URL: issues, https://github.com/kalagotla/project-arrakis/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `lptlib-0.0.1a8/src/lptlib.egg-info/SOURCES.txt` & `lptlib-0.0.1a9/src/lptlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/test/test_dataio.py` & `lptlib-0.0.1a9/test/test_dataio.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/test/test_integration.py` & `lptlib-0.0.1a9/test/test_integration.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/test/test_interpolation.py` & `lptlib-0.0.1a9/test/test_interpolation.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/test/test_oblique_shock_data.py` & `lptlib-0.0.1a9/test/test_oblique_shock_data.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/test/test_plot.py` & `lptlib-0.0.1a9/test/test_plot.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/test/test_plot3dio.py` & `lptlib-0.0.1a9/test/test_plot3dio.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/test/test_plots.py` & `lptlib-0.0.1a9/test/test_plots.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/test/test_search.py` & `lptlib-0.0.1a9/test/test_search.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/test/test_stochastic_model.py` & `lptlib-0.0.1a9/test/test_stochastic_model.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/test/test_terminal_run.py` & `lptlib-0.0.1a9/test/test_terminal_run.py`

 * *Files identical despite different names*

### Comparing `lptlib-0.0.1a8/test/test_variables.py` & `lptlib-0.0.1a9/test/test_variables.py`

 * *Files identical despite different names*

