# Comparing `tmp/batchstats-0.3.2.tar.gz` & `tmp/batchstats-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "batchstats-0.3.2.tar", last modified: Mon May 20 14:56:14 2024, max compression
+gzip compressed data, was "batchstats-0.3.3.tar", last modified: Tue May 21 22:04:00 2024, max compression
```

## Comparing `batchstats-0.3.2.tar` & `batchstats-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:56:14.502996 batchstats-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-20 14:56:02.000000 batchstats-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-20 14:56:14.502996 batchstats-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-20 14:56:02.000000 batchstats-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:56:14.498996 batchstats-0.3.2/batchstats/
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-20 14:56:02.000000 batchstats-0.3.2/batchstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-20 14:56:02.000000 batchstats-0.3.2/batchstats/_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-20 14:56:02.000000 batchstats-0.3.2/batchstats/nanstats.py
--rw-r--r--   0 runner    (1001) docker     (127)    14481 2024-05-20 14:56:02.000000 batchstats-0.3.2/batchstats/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:56:14.502996 batchstats-0.3.2/batchstats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-20 14:56:14.000000 batchstats-0.3.2/batchstats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-20 14:56:14.000000 batchstats-0.3.2/batchstats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:56:14.000000 batchstats-0.3.2/batchstats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 14:56:14.000000 batchstats-0.3.2/batchstats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 14:56:14.000000 batchstats-0.3.2/batchstats.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:56:14.502996 batchstats-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-20 14:56:02.000000 batchstats-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:56:14.502996 batchstats-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-20 14:56:02.000000 batchstats-0.3.2/tests/test_nanstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2024-05-20 14:56:02.000000 batchstats-0.3.2/tests/test_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:03:59.999523 batchstats-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 22:03:49.000000 batchstats-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-21 22:03:59.999523 batchstats-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-05-21 22:03:49.000000 batchstats-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:03:59.999523 batchstats-0.3.3/batchstats/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-21 22:03:49.000000 batchstats-0.3.3/batchstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-21 22:03:49.000000 batchstats-0.3.3/batchstats/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3021 2024-05-21 22:03:49.000000 batchstats-0.3.3/batchstats/nanstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15754 2024-05-21 22:03:49.000000 batchstats-0.3.3/batchstats/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:03:59.999523 batchstats-0.3.3/batchstats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5688 2024-05-21 22:03:59.000000 batchstats-0.3.3/batchstats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-21 22:03:59.000000 batchstats-0.3.3/batchstats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 22:03:59.000000 batchstats-0.3.3/batchstats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 22:03:59.000000 batchstats-0.3.3/batchstats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 22:03:59.000000 batchstats-0.3.3/batchstats.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 22:03:59.999523 batchstats-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-21 22:03:49.000000 batchstats-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:03:59.999523 batchstats-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-21 22:03:49.000000 batchstats-0.3.3/tests/test_nanstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 2024-05-21 22:03:49.000000 batchstats-0.3.3/tests/test_stats.py
```

### Comparing `batchstats-0.3.2/LICENSE` & `batchstats-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `batchstats-0.3.2/PKG-INFO` & `batchstats-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchstats
-Version: 0.3.2
+Version: 0.3.3
 Summary: Efficient batch statistics computation library for Python.
 Home-page: https://github.com/CyrilJl/BatchStats
 Author: Cyril Joly
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `batchstats-0.3.2/README.md` & `batchstats-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `batchstats-0.3.2/batchstats/_misc.py` & `batchstats-0.3.3/batchstats/_misc.py`

 * *Files identical despite different names*

### Comparing `batchstats-0.3.2/batchstats/nanstats.py` & `batchstats-0.3.3/batchstats/nanstats.py`

 * *Files identical despite different names*

### Comparing `batchstats-0.3.2/batchstats/stats.py` & `batchstats-0.3.3/batchstats/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import string
 
 import numpy as np
 
-from ._misc import (NoValidSamplesError, UnequalSamplesNumber, any_nan,
-                    check_params)
+from ._misc import NoValidSamplesError, UnequalSamplesNumber, any_nan, check_params
 
 
 class BatchStat:
     """
     Base class for calculating statistics over batches of data.
 
     Attributes:
@@ -376,14 +375,51 @@
 
         """
         if self.var is None:
             raise NoValidSamplesError("No valid samples for calculating variance.")
         return (self.n_samples / (self.n_samples - self.ddof)) * self.var
 
 
+class BatchStd(BatchStat):
+    """Class for calculating the standard deviation of batches of data.
+
+    Args:
+        ddof (int, optional): Means Delta Degrees of Freedom. The divisor used in calculations is N - ddof, where N represents the number of elements. By default ddof is zero.
+    """
+
+    def __init__(self, ddof=0):
+        super().__init__()
+        self.var = BatchVar(ddof=ddof)
+
+    def update_batch(self, batch, assume_valid=False):
+        """Update the standard deviation with a new batch of data.
+
+        Args:
+            batch (numpy.ndarray): Input batch.
+            assume_valid (bool, optional): If True, assumes all elements in the batch are valid. Default is False.
+
+        Returns:
+            BatchStd: Updated BatchStd object.
+        """
+        batch = self._process_batch(batch=batch, assume_valid=assume_valid)
+        self.var.update_batch(batch=batch, assume_valid=True)
+        return self
+
+    def __call__(self) -> np.ndarray:
+        """Calculate the standard deviation.
+
+        Returns:
+            numpy.ndarray: Standard deviation of the batches.
+
+        Raises:
+            NoValidSamplesError: If no valid samples are available.
+        """
+        return np.sqrt(self.var())
+
+
 class BatchCov(BatchStat):
     """
     Class for calculating the covariance of batches of data.
 
     Args:
         ddof (int, optional): Means Delta Degrees of Freedom. The divisor used in calculations is N - ddof, where N represents the number of elements. By default ddof is zero.
     """
@@ -472,7 +508,8 @@
         Raises:
             NoValidSamplesError: If no valid samples are available.
 
         """
         if self.cov is None:
             raise NoValidSamplesError("No valid samples for calculating covariance.")
         return self.n_samples/(self.n_samples - self.ddof)*self.cov
+        return self.n_samples/(self.n_samples - self.ddof)*self.cov
```

### Comparing `batchstats-0.3.2/batchstats.egg-info/PKG-INFO` & `batchstats-0.3.3/batchstats.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: batchstats
-Version: 0.3.2
+Version: 0.3.3
 Summary: Efficient batch statistics computation library for Python.
 Home-page: https://github.com/CyrilJl/BatchStats
 Author: Cyril Joly
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
```

### Comparing `batchstats-0.3.2/setup.py` & `batchstats-0.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `batchstats-0.3.2/tests/test_nanstats.py` & `batchstats-0.3.3/tests/test_nanstats.py`

 * *Files identical despite different names*

### Comparing `batchstats-0.3.2/tests/test_stats.py` & `batchstats-0.3.3/tests/test_stats.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import numpy as np
 import pytest
 
-from batchstats import (BatchCov, BatchMax, BatchMean, BatchMin,
-                        BatchPeakToPeak, BatchSum, BatchVar)
+from batchstats import BatchCov, BatchMax, BatchMean, BatchMin, BatchPeakToPeak, BatchStd, BatchSum, BatchVar
 
 
 @pytest.fixture
 def data():
     m, n = 1_000_000, 50
     return np.random.randn(m, n)
 
@@ -68,14 +67,24 @@
     batchsum = BatchSum()
     for batch_data in np.array_split(data, n_batches):
         batchsum.update_batch(batch=batch_data)
     batch_stat = batchsum()
     assert np.allclose(true_stat, batch_stat)
 
 
+def test_std(data, n_batches):
+    true_stat = np.std(data, axis=0)
+
+    batchstd = BatchStd()
+    for batch_data in np.array_split(data, n_batches):
+        batchstd.update_batch(batch=batch_data)
+    batch_stat = batchstd()
+    assert np.allclose(true_stat, batch_stat)
+
+
 def test_var(data, n_batches):
     true_stat = np.var(data, axis=0)
 
     batchvar = BatchVar()
     for batch_data in np.array_split(data, n_batches):
         batchvar.update_batch(batch=batch_data)
     batch_stat = batchvar()
```

