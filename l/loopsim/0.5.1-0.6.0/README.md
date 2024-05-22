# Comparing `tmp/loopsim-0.5.1.tar.gz` & `tmp/loopsim-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopsim-0.5.1.tar", max compression
+gzip compressed data, was "loopsim-0.6.0.tar", max compression
```

## Comparing `loopsim-0.5.1.tar` & `loopsim-0.6.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1119 2023-07-01 09:29:45.124005 loopsim-0.5.1/LICENSE
--rw-r--r--   0        0        0       22 2024-04-09 19:26:26.933225 loopsim-0.5.1/loopsim/__init__.py
--rw-r--r--   0        0        0       59 2023-04-12 00:42:22.535797 loopsim-0.5.1/loopsim/__main__.py
--rwxr-xr-x   0        0        0     2715 2023-06-26 14:56:26.502571 loopsim-0.5.1/loopsim/analyze.py
--rw-r--r--   0        0        0     3243 2023-07-04 10:54:37.475195 loopsim-0.5.1/loopsim/batch_analyze.py
--rw-r--r--   0        0        0      753 2023-07-04 11:17:20.278702 loopsim-0.5.1/loopsim/cli.py
--rw-r--r--   0        0        0      322 2023-04-12 00:42:22.536114 loopsim-0.5.1/loopsim/common.py
--rwxr-xr-x   0        0        0     6538 2024-02-20 23:10:00.383152 loopsim-0.5.1/loopsim/simulate.py
--rw-r--r--   0        0        0     5725 2023-07-04 11:40:26.672482 loopsim-0.5.1/loopsim/validate.py
--rwxr-xr-x   0        0        0     2356 2023-04-12 00:42:22.536362 loopsim-0.5.1/loopsim/visualize.py
--rw-r--r--   0        0        0     1103 2024-04-09 19:26:40.299878 loopsim-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     1215 1970-01-01 00:00:00.000000 loopsim-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1119 2023-07-01 09:29:45.124005 loopsim-0.6.0/LICENSE
+-rw-r--r--   0        0        0       22 2024-05-22 19:27:28.871788 loopsim-0.6.0/loopsim/__init__.py
+-rw-r--r--   0        0        0       59 2023-04-12 00:42:22.535797 loopsim-0.6.0/loopsim/__main__.py
+-rwxr-xr-x   0        0        0     2715 2023-06-26 14:56:26.502571 loopsim-0.6.0/loopsim/analyze.py
+-rw-r--r--   0        0        0     3243 2023-07-04 10:54:37.475195 loopsim-0.6.0/loopsim/batch_analyze.py
+-rw-r--r--   0        0        0      753 2023-07-04 11:17:20.278702 loopsim-0.6.0/loopsim/cli.py
+-rw-r--r--   0        0        0      322 2023-04-12 00:42:22.536114 loopsim-0.6.0/loopsim/common.py
+-rwxr-xr-x   0        0        0     6538 2024-02-20 23:10:00.383152 loopsim-0.6.0/loopsim/simulate.py
+-rw-r--r--   0        0        0     5725 2023-07-04 11:40:26.672482 loopsim-0.6.0/loopsim/validate.py
+-rwxr-xr-x   0        0        0     2573 2024-05-22 19:26:31.879985 loopsim-0.6.0/loopsim/visualize.py
+-rw-r--r--   0        0        0     1103 2024-05-22 19:38:21.655655 loopsim-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1215 1970-01-01 00:00:00.000000 loopsim-0.6.0/PKG-INFO
```

### Comparing `loopsim-0.5.1/LICENSE` & `loopsim-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `loopsim-0.5.1/loopsim/analyze.py` & `loopsim-0.6.0/loopsim/analyze.py`

 * *Files identical despite different names*

### Comparing `loopsim-0.5.1/loopsim/batch_analyze.py` & `loopsim-0.6.0/loopsim/batch_analyze.py`

 * *Files identical despite different names*

### Comparing `loopsim-0.5.1/loopsim/cli.py` & `loopsim-0.6.0/loopsim/cli.py`

 * *Files identical despite different names*

### Comparing `loopsim-0.5.1/loopsim/simulate.py` & `loopsim-0.6.0/loopsim/simulate.py`

 * *Files identical despite different names*

### Comparing `loopsim-0.5.1/loopsim/validate.py` & `loopsim-0.6.0/loopsim/validate.py`

 * *Files identical despite different names*

### Comparing `loopsim-0.5.1/loopsim/visualize.py` & `loopsim-0.6.0/loopsim/visualize.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 """Plot ratio distribution"""
 
 import click
 import pandas as pd
 import seaborn as sb
-from scipy.stats import norm
+from scipy.stats import norm, normaltest
 
 from . import common
 
 
 @click.command()
-@click.argument("distribution_file", type=click.Path(exists=True, file_okay=True, dir_okay=False, readable=True))
-@click.argument("plot_file", type=click.Path(exists=False, file_okay=True, dir_okay=False, writable=True))
+@click.argument(
+    "distribution_file",
+    type=click.Path(exists=True, file_okay=True, dir_okay=False, readable=True),
+)
+@click.argument(
+    "plot_file",
+    type=click.Path(exists=False, file_okay=True, dir_okay=False, writable=True),
+)
 @click.option(
     "--other",
     type=float,
     help="if this is passed, a Z-test will be conducted on this value against the mean of the ratio distribution",
 )
 def visualize(distribution_file, plot_file, other):
     """Get visualization and stats from distribution of ratios
@@ -23,20 +29,26 @@
     Optionally, can pass a data point for statistical comparison with --other flag
     """
 
     # Print params
     print(f"Obtaining overlapping ratios from: {distribution_file}.")
 
     # Get data
-    dist = pd.read_table(distribution_file, header=None, delimiter=common.detect_delimiter(distribution_file))
+    dist = pd.read_table(
+        distribution_file,
+        header=None,
+        delimiter=common.detect_delimiter(distribution_file),
+    )
 
     # Create distribution plot
     ax = sb.histplot(data=dist[0], label="Simulated", kde=True)
     ax.set(
-        title=f"Distribution of Overlapping Ratios by Frequency (N = {len(dist)})", xlabel="Overlapping Ratio", ylabel="Frequency"
+        title=f"Distribution of Overlapping Ratios by Frequency (N = {len(dist)})",
+        xlabel="Overlapping Ratio",
+        ylabel="Frequency",
     )
 
     if other:
         ax.axvline(other, color="orange", label="Experimental")
 
     legend_handles, _ = ax.get_legend_handles_labels()
     ax.legend(handles=legend_handles)
@@ -59,7 +71,12 @@
         print("\nCalculating p-value based on empirical distribution:")
         num_larger = len(dist.loc[dist[0] > other])
         print(f"p-value: {num_larger / len(dist):.20f}")
 
         print("\nCalculating p-value based on normal distribution:")
         z_stat = (other - dist[0].mean()) / dist[0].std()
         print(f"p-value: {1 - norm.cdf(z_stat):.20f}")
+
+    # Normality test
+    print("\nD'Agostino-Pearson normality test:")
+    _, p = normaltest(dist[0])
+    print(f"p-value: {p:.20f}")
```

### Comparing `loopsim-0.5.1/pyproject.toml` & `loopsim-0.6.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "loopsim"
-version = "0.5.1"
+version = "0.6.0"
 description = "Loopsim: Enrichment Analysis of Chromosome Conformation Capture with Fast Empirical Distribution Simulation"
 authors = ["Gideon Shaked <gshaked@umich.edu>"]
 maintainers = ["Gideon Shaked <gshaked@umich.edu>"]
 repository = "https://github.com/CutaneousBioinf/loopsim"
 classifiers = ["Environment :: Console",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `loopsim-0.5.1/PKG-INFO` & `loopsim-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopsim
-Version: 0.5.1
+Version: 0.6.0
 Summary: Loopsim: Enrichment Analysis of Chromosome Conformation Capture with Fast Empirical Distribution Simulation
 Home-page: https://github.com/CutaneousBioinf/loopsim
 License: MIT
 Author: Gideon Shaked
 Author-email: gshaked@umich.edu
 Maintainer: Gideon Shaked
 Maintainer-email: gshaked@umich.edu
```

