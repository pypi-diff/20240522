# Comparing `tmp/slidingRP-1.1.0.tar.gz` & `tmp/slidingRP-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slidingRP-1.1.0.tar", last modified: Sun May 19 10:41:06 2024, max compression
+gzip compressed data, was "slidingRP-1.1.1.tar", last modified: Wed May 22 09:27:08 2024, max compression
```

## Comparing `slidingRP-1.1.0.tar` & `slidingRP-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2024-05-19 10:41:06.323487 slidingRP-1.1.0/
--rw-r--r--   0 olivier   (1000) olivier   (1000)     1786 2024-05-19 10:41:06.323487 slidingRP-1.1.0/PKG-INFO
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1200 2024-04-12 13:27:04.000000 slidingRP-1.1.0/README.md
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2024-05-19 10:41:06.319486 slidingRP-1.1.0/python/
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2024-05-19 10:41:06.323487 slidingRP-1.1.0/python/slidingRP/
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     8264 2024-04-12 13:27:04.000000 slidingRP-1.1.0/python/slidingRP/Fig2_ACGMetric.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     3298 2024-04-12 13:27:04.000000 slidingRP-1.1.0/python/slidingRP/Fig3_simulations.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    10128 2024-04-12 13:27:04.000000 slidingRP-1.1.0/python/slidingRP/Fig4_HillCompConfidence.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     8676 2024-04-12 13:27:04.000000 slidingRP-1.1.0/python/slidingRP/Fig5_ConfROC.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     3619 2024-04-12 13:27:04.000000 slidingRP-1.1.0/python/slidingRP/Fig6_drift.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)        0 2024-04-12 13:27:04.000000 slidingRP-1.1.0/python/slidingRP/__init__.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    16946 2024-04-12 13:27:04.000000 slidingRP-1.1.0/python/slidingRP/loadSaveData.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    31832 2024-05-19 10:40:40.000000 slidingRP-1.1.0/python/slidingRP/metrics.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1885 2024-04-12 13:27:04.000000 slidingRP-1.1.0/python/slidingRP/scriptSavePaperFigs.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)    67086 2024-04-12 13:27:04.000000 slidingRP-1.1.0/python/slidingRP/simulations.py
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1445 2024-04-12 13:27:04.000000 slidingRP-1.1.0/python/slidingRP/spike_sorting_benchmark.py
-drwxrwxr-x   0 olivier   (1000) olivier   (1000)        0 2024-05-19 10:41:06.323487 slidingRP-1.1.0/python/slidingRP.egg-info/
--rw-r--r--   0 olivier   (1000) olivier   (1000)     1786 2024-05-19 10:41:06.000000 slidingRP-1.1.0/python/slidingRP.egg-info/PKG-INFO
--rw-rw-r--   0 olivier   (1000) olivier   (1000)      603 2024-05-19 10:41:06.000000 slidingRP-1.1.0/python/slidingRP.egg-info/SOURCES.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)        1 2024-05-19 10:41:06.000000 slidingRP-1.1.0/python/slidingRP.egg-info/dependency_links.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       44 2024-05-19 10:41:06.000000 slidingRP-1.1.0/python/slidingRP.egg-info/requires.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       10 2024-05-19 10:41:06.000000 slidingRP-1.1.0/python/slidingRP.egg-info/top_level.txt
--rw-rw-r--   0 olivier   (1000) olivier   (1000)       38 2024-05-19 10:41:06.323487 slidingRP-1.1.0/setup.cfg
--rw-rw-r--   0 olivier   (1000) olivier   (1000)     1013 2024-05-19 10:40:40.000000 slidingRP-1.1.0/setup.py
+drwxr-xr-x   0 olivier    (501) staff       (20)        0 2024-05-22 09:27:08.126290 slidingRP-1.1.1/
+-rw-r--r--   0 olivier    (501) staff       (20)     1667 2024-05-22 09:27:08.126043 slidingRP-1.1.1/PKG-INFO
+-rw-r--r--   0 olivier    (501) staff       (20)     1200 2022-10-22 17:56:12.000000 slidingRP-1.1.1/README.md
+drwxr-xr-x   0 olivier    (501) staff       (20)        0 2024-05-22 09:27:08.120006 slidingRP-1.1.1/python/
+drwxr-xr-x   0 olivier    (501) staff       (20)        0 2024-05-22 09:27:08.124955 slidingRP-1.1.1/python/slidingRP/
+-rw-r--r--   0 olivier    (501) staff       (20)     8264 2024-05-22 09:24:07.000000 slidingRP-1.1.1/python/slidingRP/Fig2_ACGMetric.py
+-rw-r--r--   0 olivier    (501) staff       (20)     3298 2024-05-22 09:24:07.000000 slidingRP-1.1.1/python/slidingRP/Fig3_simulations.py
+-rw-r--r--   0 olivier    (501) staff       (20)    10128 2024-05-22 09:24:07.000000 slidingRP-1.1.1/python/slidingRP/Fig4_HillCompConfidence.py
+-rw-r--r--   0 olivier    (501) staff       (20)     8676 2024-05-22 09:24:07.000000 slidingRP-1.1.1/python/slidingRP/Fig5_ConfROC.py
+-rw-r--r--   0 olivier    (501) staff       (20)     3619 2024-05-22 09:24:07.000000 slidingRP-1.1.1/python/slidingRP/Fig6_drift.py
+-rw-r--r--   0 olivier    (501) staff       (20)        0 2022-10-22 17:56:12.000000 slidingRP-1.1.1/python/slidingRP/__init__.py
+-rw-r--r--   0 olivier    (501) staff       (20)    16946 2024-05-22 09:24:07.000000 slidingRP-1.1.1/python/slidingRP/loadSaveData.py
+-rw-r--r--   0 olivier    (501) staff       (20)    31721 2024-05-22 09:24:07.000000 slidingRP-1.1.1/python/slidingRP/metrics.py
+-rw-r--r--   0 olivier    (501) staff       (20)     1885 2024-05-22 09:24:07.000000 slidingRP-1.1.1/python/slidingRP/scriptSavePaperFigs.py
+-rw-r--r--   0 olivier    (501) staff       (20)    67086 2024-05-22 09:24:07.000000 slidingRP-1.1.1/python/slidingRP/simulations.py
+-rw-r--r--   0 olivier    (501) staff       (20)     1445 2024-05-22 09:24:07.000000 slidingRP-1.1.1/python/slidingRP/spike_sorting_benchmark.py
+drwxr-xr-x   0 olivier    (501) staff       (20)        0 2024-05-22 09:27:08.125787 slidingRP-1.1.1/python/slidingRP.egg-info/
+-rw-r--r--   0 olivier    (501) staff       (20)     1667 2024-05-22 09:27:08.000000 slidingRP-1.1.1/python/slidingRP.egg-info/PKG-INFO
+-rw-r--r--   0 olivier    (501) staff       (20)      603 2024-05-22 09:27:08.000000 slidingRP-1.1.1/python/slidingRP.egg-info/SOURCES.txt
+-rw-r--r--   0 olivier    (501) staff       (20)        1 2024-05-22 09:27:08.000000 slidingRP-1.1.1/python/slidingRP.egg-info/dependency_links.txt
+-rw-r--r--   0 olivier    (501) staff       (20)       44 2024-05-22 09:27:08.000000 slidingRP-1.1.1/python/slidingRP.egg-info/requires.txt
+-rw-r--r--   0 olivier    (501) staff       (20)       10 2024-05-22 09:27:08.000000 slidingRP-1.1.1/python/slidingRP.egg-info/top_level.txt
+-rw-r--r--   0 olivier    (501) staff       (20)       38 2024-05-22 09:27:08.126340 slidingRP-1.1.1/setup.cfg
+-rw-r--r--   0 olivier    (501) staff       (20)     1013 2024-05-22 09:24:07.000000 slidingRP-1.1.1/setup.py
```

### Comparing `slidingRP-1.1.0/PKG-INFO` & `slidingRP-1.1.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 Metadata-Version: 2.1
 Name: slidingRP
-Version: 1.1.0
+Version: 1.1.1
 Summary: Quality metric from spike trains
 Home-page: https://github.com/SteinmetzLab/slidingRefractory
 Author: Noam Roth
 Project-URL: Bug Tracker, https://github.com/SteinmetzLab/slidingRefractory/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: matplotlib
-Requires-Dist: colorcet
-Requires-Dist: statsmodels
 
 # slidingRefractory
 Code to perform a new test of whether neurons have contaminated refractory periods, with a sliding window
 
 
 ## Python
```

### Comparing `slidingRP-1.1.0/README.md` & `slidingRP-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `slidingRP-1.1.0/python/slidingRP/Fig2_ACGMetric.py` & `slidingRP-1.1.1/python/slidingRP/Fig2_ACGMetric.py`

 * *Files identical despite different names*

### Comparing `slidingRP-1.1.0/python/slidingRP/Fig3_simulations.py` & `slidingRP-1.1.1/python/slidingRP/Fig3_simulations.py`

 * *Files identical despite different names*

### Comparing `slidingRP-1.1.0/python/slidingRP/Fig4_HillCompConfidence.py` & `slidingRP-1.1.1/python/slidingRP/Fig4_HillCompConfidence.py`

 * *Files identical despite different names*

### Comparing `slidingRP-1.1.0/python/slidingRP/Fig5_ConfROC.py` & `slidingRP-1.1.1/python/slidingRP/Fig5_ConfROC.py`

 * *Files identical despite different names*

### Comparing `slidingRP-1.1.0/python/slidingRP/Fig6_drift.py` & `slidingRP-1.1.1/python/slidingRP/Fig6_drift.py`

 * *Files identical despite different names*

### Comparing `slidingRP-1.1.0/python/slidingRP/loadSaveData.py` & `slidingRP-1.1.1/python/slidingRP/loadSaveData.py`

 * *Files identical despite different names*

### Comparing `slidingRP-1.1.0/python/slidingRP/metrics.py` & `slidingRP-1.1.1/python/slidingRP/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,22 +199,19 @@
         min_cont = np.nan
         rp_min_val = np.nan
 
     return pass_cont_thresh, min_cont, rp_min_val  # Legacy: value, minContWith90Confidence, timeOfLowestCont
 
 
 def slidingRP(spikeTimes, conf_thresh=90, cont_thresh=10, rp_reject=0.0005,
-              params=None):
-    if params is None:
-        params = {}
+              **params):
+    if not params:
+        params = dict()
         params['sampleRate'] = 30000
         params['binSizeCorr'] = 1 / params['sampleRate']
-        params['returnMatrix'] = True
-        params['verbose'] = True
-        params['cidx'] = [0]
 
     [confMatrix, cont, rp, nACG, firing_rate] = computeMatrix(spikeTimes, params)
     # Legacy: PASS, minContWith90Confidence, timeOfLowestCont
     pass_cont_thresh, min_cont, rp_min_val = \
         pass_slidingRP_confmat(confMatrix, cont, rp, conf_thresh, cont_thresh, rp_reject)
 
     # Legacy 'maxConfidenceAt10Cont'
@@ -236,15 +233,15 @@
     return max_conf, min_cont, rp_min_val, \
         n_spikes_below2, firing_rate,\
         pass_cont_thresh, pass_forced
 
 
 def slidingRP_all(spikeTimes, spikeClusters,
                   conf_thresh=90, cont_thresh=10, rp_reject=0.0005,
-                  params=None):
+                  **params):
     """
     :param spikeTimes:  array of spike times (s)
     :param spikeClusters:  array of spike cluster ids that corresponds to spikeTimes
     :param params:
     :return: dictionary of values
     """
 
@@ -265,15 +262,15 @@
     for cidx in range(len(cids)):
         st = spikeTimes[spikeClusters == cids[cidx]]
 
         [max_confidence, min_contamination, rp_min_val,
          n_spikes_below2, firing_rate,
          pass_cont_thresh, pass_forced] = slidingRP(st,
                                                     conf_thresh=conf_thresh, cont_thresh=cont_thresh,
-                                                    rp_reject=rp_reject, params=params)
+                                                    rp_reject=rp_reject, **params)
 
         rpMetrics['cidx'].append(cids[cidx])
         rpMetrics['max_confidence'].append(max_confidence)
         rpMetrics['min_contamination'].append(min_contamination)
         rpMetrics['rp_min_val'].append(rp_min_val)
         rpMetrics['n_spikes_below2'].append(n_spikes_below2)
         rpMetrics['firing_rate'].append(firing_rate)
```

### Comparing `slidingRP-1.1.0/python/slidingRP/scriptSavePaperFigs.py` & `slidingRP-1.1.1/python/slidingRP/scriptSavePaperFigs.py`

 * *Files identical despite different names*

### Comparing `slidingRP-1.1.0/python/slidingRP/simulations.py` & `slidingRP-1.1.1/python/slidingRP/simulations.py`

 * *Files identical despite different names*

### Comparing `slidingRP-1.1.0/python/slidingRP/spike_sorting_benchmark.py` & `slidingRP-1.1.1/python/slidingRP/spike_sorting_benchmark.py`

 * *Files identical despite different names*

### Comparing `slidingRP-1.1.0/python/slidingRP.egg-info/PKG-INFO` & `slidingRP-1.1.1/python/slidingRP.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 Metadata-Version: 2.1
 Name: slidingRP
-Version: 1.1.0
+Version: 1.1.1
 Summary: Quality metric from spike trains
 Home-page: https://github.com/SteinmetzLab/slidingRefractory
 Author: Noam Roth
 Project-URL: Bug Tracker, https://github.com/SteinmetzLab/slidingRefractory/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: matplotlib
-Requires-Dist: colorcet
-Requires-Dist: statsmodels
 
 # slidingRefractory
 Code to perform a new test of whether neurons have contaminated refractory periods, with a sliding window
 
 
 ## Python
```

### Comparing `slidingRP-1.1.0/python/slidingRP.egg-info/SOURCES.txt` & `slidingRP-1.1.1/python/slidingRP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slidingRP-1.1.0/setup.py` & `slidingRP-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('requirements.txt') as f:
     require = [x.strip() for x in f.readlines() if not x.startswith('git+')]
 
 setuptools.setup(
     name="slidingRP",
-    version="1.1.0",
+    version="1.1.1",
     author="Noam Roth",
     description="Quality metric from spike trains",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SteinmetzLab/slidingRefractory",
     project_urls={
         "Bug Tracker": "https://github.com/SteinmetzLab/slidingRefractory/issues",
```

