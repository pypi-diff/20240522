# Comparing `tmp/peakfit-0.4.0.tar.gz` & `tmp/peakfit-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakfit-0.4.0.tar", max compression
+gzip compressed data, was "peakfit-0.5.0.tar", last modified: Wed May 22 21:42:15 2024, max compression
```

## Comparing `peakfit-0.4.0.tar` & `peakfit-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,17 @@
--rw-r--r--   0        0        0    34916 2023-01-13 10:54:30.485705 peakfit-0.4.0/LICENSE
--rw-r--r--   0        0        0       75 2023-01-13 10:53:29.231653 peakfit-0.4.0/README.md
--rw-r--r--   0        0        0     6148 2023-01-13 10:04:36.733861 peakfit-0.4.0/peakfit/.DS_Store
--rw-r--r--   0        0        0      326 2023-01-17 09:04:07.564916 peakfit-0.4.0/peakfit/__init__.py
--rw-r--r--   0        0        0      125 2023-01-13 10:53:29.231714 peakfit-0.4.0/peakfit/__main__.py
--rw-r--r--   0        0        0     1425 2023-01-17 10:56:05.263617 peakfit-0.4.0/peakfit/cli.py
--rw-r--r--   0        0        0     3360 2023-01-17 10:45:58.518650 peakfit-0.4.0/peakfit/clustering.py
--rw-r--r--   0        0        0     1005 2021-07-02 15:49:02.720758 peakfit-0.4.0/peakfit/computing.py
--rw-r--r--   0        0        0     1297 2023-01-17 11:09:31.801388 peakfit-0.4.0/peakfit/messages.py
--rw-r--r--   0        0        0     8062 2023-01-17 11:06:01.299819 peakfit-0.4.0/peakfit/peakfit.py
--rw-r--r--   0        0        0     1710 2023-01-17 10:50:13.967687 peakfit-0.4.0/peakfit/plot_cest.py
--rw-r--r--   0        0        0     2650 2023-01-17 10:33:47.034165 peakfit-0.4.0/peakfit/plot_cpmg.py
--rw-r--r--   0        0        0     1211 2023-01-17 11:07:39.544158 peakfit-0.4.0/peakfit/plot_intensities.py
--rw-r--r--   0        0        0     1720 2023-01-13 10:53:29.231766 peakfit-0.4.0/peakfit/shapes.py
--rw-r--r--   0        0        0        0 2021-06-01 12:54:07.610095 peakfit-0.4.0/peakfit/writing.py
--rw-r--r--   0        0        0     1306 2023-01-17 11:09:52.395856 peakfit-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1196 1970-01-01 00:00:00.000000 peakfit-0.4.0/setup.py
--rw-r--r--   0        0        0     1231 1970-01-01 00:00:00.000000 peakfit-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    34916 2024-05-22 21:42:11.421680 peakfit-0.5.0/LICENSE
+-rw-r--r--   0        0        0       75 2024-05-22 21:42:11.421680 peakfit-0.5.0/README.md
+-rw-r--r--   0        0        0       73 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/__init__.py
+-rw-r--r--   0        0        0      126 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/__main__.py
+-rw-r--r--   0        0        0     1431 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/cli.py
+-rw-r--r--   0        0        0     3845 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/clustering.py
+-rw-r--r--   0        0        0      999 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/computing.py
+-rw-r--r--   0        0        0     2597 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/messages.py
+-rw-r--r--   0        0        0      467 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/noise.py
+-rw-r--r--   0        0        0     8075 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/peakfit.py
+-rw-r--r--   0        0        0     1678 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/plot_cest.py
+-rw-r--r--   0        0        0     2725 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/plot_cpmg.py
+-rw-r--r--   0        0        0     1225 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/plot_intensities.py
+-rw-r--r--   0        0        0     1719 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/shapes.py
+-rw-r--r--   0        0        0        0 2024-05-22 21:42:11.833682 peakfit-0.5.0/peakfit/writing.py
+-rw-r--r--   0        0        0     1138 2024-05-22 21:42:15.869702 peakfit-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 peakfit-0.5.0/PKG-INFO
```

### Comparing `peakfit-0.4.0/LICENSE` & `peakfit-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peakfit-0.4.0/peakfit/cli.py` & `peakfit-0.5.0/peakfit/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The parsing module contains the code for the parsing of command-line arguments."""
+
 from __future__ import annotations
 
 from argparse import ArgumentParser
 from pathlib import Path
 
 
 def build_parser() -> ArgumentParser:
@@ -17,19 +18,23 @@
         dest="path_spectra",
         required=True,
         type=Path,
         nargs="+",
     )
     parser.add_argument("--list", "-l", dest="path_list", required=True, type=Path)
     parser.add_argument(
-        "--zvalues", "-z", dest="path_z_values", required=True, nargs="+"
+        "--zvalues",
+        "-z",
+        dest="path_z_values",
+        required=True,
+        nargs="+",
     )
-    parser.add_argument("--ct", "-t", dest="contour_level", required=True, type=float)
+    parser.add_argument("--ct", "-t", dest="contour_level", type=float)
     parser.add_argument("--out", "-o", dest="path_output", default="Fits", type=Path)
-    parser.add_argument("--noise", "-n", dest="noise", default=1.0, type=float)
+    parser.add_argument("--noise", "-n", dest="noise", type=float)
     parser.add_argument(
         "--mc",
         nargs=5,
         metavar=("X_MIN", "X_MAX", "Y_MIN", "Y_MAX", "N"),
     )
     parser.add_argument("--fixed", dest="fixed", action="store_true")
     parser.add_argument("--pvoigt", dest="pvoigt", action="store_true")
```

### Comparing `peakfit-0.4.0/peakfit/clustering.py` & `peakfit-0.5.0/peakfit/clustering.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,79 +1,116 @@
-import collections as cl
 import itertools as it
+from typing import NamedTuple
 
 import numpy as np
+from nmrglue.fileio.fileiobase import unit_conversion
 
+from peakfit.messages import print_segmenting
 
-Spectra = cl.namedtuple("Spectra", "data ucx ucy z_values")
-Peak = cl.namedtuple("Peak", "name x0 y0")
-Cluster = cl.namedtuple("Cluster", "peaks x y data")
 
+class Spectra(NamedTuple):
+    data: np.ndarray
+    ucx: unit_conversion
+    ucy: unit_conversion
+    z_values: np.ndarray
 
-def _merge_clusters(cluster1, cluster2):
+
+class Peak(NamedTuple):
+    name: str
+    x0: int
+    y0: int
+
+
+class Cluster(NamedTuple):
+    peaks: list
+    x: np.ndarray
+    y: np.ndarray
+    data: np.ndarray
+
+
+def _merge_clusters(cluster1: Cluster, cluster2: Cluster) -> Cluster:
     peak_cluster = [*cluster1.peaks, *cluster2.peaks]
     x_cluster = np.hstack((cluster1.x, cluster2.x))
     y_cluster = np.hstack((cluster1.y, cluster2.y))
     data_cluster = np.vstack((cluster1.data, cluster2.data))
     return Cluster(peak_cluster, x_cluster, y_cluster, data_cluster)
 
 
-def _distance(cluster1, cluster2, spectra):
+def _distance(cluster1: Cluster, cluster2: Cluster, spectra: Spectra) -> float:
     ucx, ucy = spectra.ucx, spectra.ucy
     distances2 = [
         (ucx.hz(ucx.f(peak1.x0, "ppm")) - ucx.hz(ucx.f(peak2.x0, "ppm"))) ** 2
         + (ucy.hz(ucy.f(peak1.y0, "ppm")) - ucy.hz(ucy.f(peak2.y0, "ppm"))) ** 2
         for peak1, peak2 in it.product(cluster1.peaks, cluster2.peaks)
     ]
 
     return np.sqrt(min(distances2))
 
 
-def _merge_close_clusters(clusters, spectra, cutoff):
+def _merge_close_clusters(
+    clusters: list[Cluster],
+    spectra: Spectra,
+    cutoff: float,
+) -> list[Cluster]:
     grouped = True
     while grouped:
         grouped = False
         for cluster1, cluster2 in it.combinations(clusters, 2):
             if _distance(cluster1, cluster2, spectra) <= cutoff:
                 merged = _merge_clusters(cluster1, cluster2)
                 clusters.remove(cluster1)
                 clusters.remove(cluster2)
                 clusters.append(merged)
                 grouped = True
                 break
     return clusters
 
 
-def _flood(x_start: int, y_start: int, spectra: Spectra, threshold: float) -> list:
-    ny, nx = spectra.data.shape[1:]
+def _flood(
+    x_start: int,
+    y_start: int,
+    spectra: Spectra,
+    threshold: float,
+) -> list[tuple[int, int]]:
+    data = spectra.data
+    ny, nx = data.shape[1:]
     stack = [(x_start, y_start)]
     points = set()
     while stack:
         x, y = stack.pop()
-        above = abs(spectra.data[0, y % ny, x % nx]) >= threshold
+        above = any(abs(data[:, y % ny, x % nx]) >= threshold)
         unvisited = (x, y) not in points
         if above and unvisited:
             points.add((x, y))
             stack.extend([(x - 1, y), (x + 1, y), (x, y - 1), (x, y + 1)])
     if len(points) < 9:
-        points = zip(range(x_start - 1, x_start + 2), range(y_start - 1, y_start + 2))
+        points = zip(
+            range(x_start - 1, x_start + 2),
+            range(y_start - 1, y_start + 2),
+            strict=False,
+        )
     return list(points)
 
 
-def cluster_peaks(spectra: Spectra, peaks: np.ndarray, contour_level: float) -> list:
-
-    print("- Segmenting the spectra and clustering the peaks...")
+def cluster_peaks(
+    spectra: Spectra,
+    peaks: np.ndarray,
+    contour_level: float,
+) -> list[Cluster]:
+    print_segmenting()
 
     nz, ny, nx = spectra.data.shape
 
     peaks_ppm = {name: Peak(name, x, y) for name, y, x in peaks}
 
     x_pts = np.rint(spectra.ucx.f(peaks["x"], "ppm")).astype(int)
     y_pts = np.rint(spectra.ucy.f(peaks["y"], "ppm")).astype(int)
-    peaks_pt = {name: (x, y) for name, x, y in zip(peaks["names"], x_pts, y_pts)}
+    peaks_pt = {
+        name: (x, y) for name, x, y in zip(peaks["names"], x_pts, y_pts, strict=False)
+    }
 
     names = set(peaks_pt)
 
     clusters = []
     for name, (x_pt, y_pt) in peaks_pt.items():
         if name not in names:
             continue
```

### Comparing `peakfit-0.4.0/peakfit/computing.py` & `peakfit-0.5.0/peakfit/computing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import scipy.linalg as sl
 
 import peakfit.shapes as ps
 
 
 def calculate_shape_heights(params, cluster):
     shapes = []
 
@@ -15,19 +14,19 @@
                 cluster.y,
                 params[f"{pre}x0"],
                 params[f"{pre}y0"],
                 params[f"{pre}x_fwhm_ppm"],
                 params[f"{pre}y_fwhm_ppm"],
                 params[f"{pre}x_eta"],
                 params[f"{pre}y_eta"],
-            )
+            ),
         )
 
     shapes = np.asarray(shapes).T
-    amp_values = sl.lstsq(shapes, cluster.data)[0]
+    amp_values = np.linalg.lstsq(shapes, cluster.data, rcond=None)[0]
 
     return shapes, amp_values
 
 
 def residuals(params, cluster, noise):
     shapes, amplitudes = calculate_shape_heights(params, cluster)
     return np.ravel((cluster.data - shapes.dot(amplitudes)) / noise)
```

### Comparing `peakfit-0.4.0/peakfit/peakfit.py` & `peakfit-0.5.0/peakfit/peakfit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,39 @@
-"""Main module"""
+"""Main module."""
+
 import random
-import sys
 from collections.abc import Sequence
 from pathlib import Path
 
 import lmfit as lf
 import nmrglue as ng
 import numpy as np
 import numpy.random as nr
 
 from peakfit.cli import build_parser
-from peakfit.clustering import Cluster
-from peakfit.clustering import cluster_peaks
-from peakfit.clustering import Spectra
-from peakfit.computing import calculate_shape_heights
-from peakfit.computing import residuals
-from peakfit.computing import simulate_data
-from peakfit.messages import print_logo
-from peakfit.messages import print_peaks
+from peakfit.clustering import Cluster, Spectra, cluster_peaks
+from peakfit.computing import calculate_shape_heights, residuals, simulate_data
+from peakfit.messages import (
+    export_html,
+    print_estimated_noise,
+    print_fit_report,
+    print_fitting,
+    print_logo,
+    print_peaks,
+)
+from peakfit.noise import estimate_noise
 from peakfit.shapes import create_params
 
 
 def read_spectra(
     paths_spectra: Sequence[Path],
     paths_z_values: Sequence[Path],
     exclude_list: Sequence[int],
 ) -> Spectra:
-    """Read NMRPipe spectra and return a Spectra object"""
-
+    """Read NMRPipe spectra and return a Spectra object."""
     # Read NMRPipe spectra
     dic_list = []
     data_list = []
     for path in paths_spectra:
         dic, data = ng.fileio.pipe.read(str(path))
         dic_list.append(dic)
         data_list.append(data)
@@ -39,29 +41,37 @@
 
     # Read z values
     z_list = [np.genfromtxt(path, dtype=None) for path in paths_z_values]
     z_values = np.concatenate(z_list)
 
     # Exclude planes
     if exclude_list:
-        exclude_array = np.full_like(z_values, False, np.bool_)
+        exclude_array = np.full_like(z_values, fill_value=False, dtype=np.bool_)
         exclude_array[exclude_list] = True
         data = data[~exclude_array]
         z_values = z_values[~exclude_array]
 
     # Create unit conversion object for indirect and direct dimension
     dic = dic_list[0]
     ucy = ng.pipe.make_uc(dic, data, dim=1)
     ucx = ng.pipe.make_uc(dic, data, dim=2)
 
     # Create and return 'Spectra' object
     return Spectra(data, ucx, ucy, z_values)
 
 
-def write_profiles(path, z_values, cluster, params, heights, params_err, height_err):
+def write_profiles(
+    path,
+    z_values,
+    cluster,
+    params,
+    heights,
+    params_err,
+    height_err,
+) -> None:
     for i, peak in enumerate(cluster.peaks):
         vals = params.valuesdict()
         errs = {k: v if v is not None else 0.0 for k, v in params_err.items()}
 
         x_ppm = vals[f"p{i}_x0"]
         y_ppm = vals[f"p{i}_y0"]
         x_ppm_e = errs[f"p{i}_x0"]
@@ -87,17 +97,17 @@
             f.write(f"# x_ppm: {x_ppm:10.5f} {x_ppm_e:10.5f}\n")
             f.write(f"# xw_hz: {xw_hz:10.5f} {xw_hz_e:10.5f}\n")
             f.write(f"# x_eta: {x_eta:10.5f} {x_eta_e:10.5f}\n")
             f.write("#---------------------------------------------\n")
             f.write(f"# {'Z':>10s}  {'I':>14s}  {'I_err':>14s}\n")
             f.write(
                 "\n".join(
-                    f"  {str(z):>10s}  {ampl:14.6e}  {ampl_e:14.6e}"
-                    for z, ampl in zip(z_values, heights[i])
-                )
+                    f"  {z!s:>10s}  {ampl:14.6e}  {ampl_e:14.6e}"
+                    for z, ampl in zip(z_values, heights[i], strict=False)
+                ),
             )
 
 
 def get_some_noise(spectra, noise, x_pt, y_pt):
     nr.shuffle(noise)
 
     nz_noise, ny_noise, nx_noise = noise.shape
@@ -118,40 +128,37 @@
     y1_pt, y2_pt = sorted((spectra.ucy.i(y1), spectra.ucy.i(y2)))
 
     noise = spectra.data[:, y1_pt:y2_pt, x1_pt:x2_pt]
     return n_iter, noise
 
 
 def calc_err_from_mc(params_list, heights_list):
-
     params_dict = {}
 
     for params_mc in params_list:
         for name, param in params_mc.items():
             params_dict.setdefault(name, []).append(param.value)
 
     params_err = {name: np.std(values) for name, values in params_dict.items()}
     height_err = np.std(heights_list, axis=0, ddof=1)
 
     return params_err, height_err
 
 
 def monte_carlo(mc, spectra, cluster, result, noise):
-
     n_iter, spectra_noise = extract_noise_spectra(mc, spectra)
 
     x_pt = np.rint(spectra.ucx.f(cluster.x, "ppm")).astype(int)
     y_pt = np.rint(spectra.ucy.f(cluster.y, "ppm")).astype(int)
 
     data_sim = simulate_data(result.params, cluster)
 
     mc_list = []
 
     for _ in range(int(n_iter)):
-
         data_noise = get_some_noise(spectra, spectra_noise, x_pt, y_pt)
         data_mc = data_sim + data_noise
         cluster_mc = Cluster(cluster.peaks, cluster.x, cluster.y, data_mc)
 
         params_mc = lf.minimize(
             residuals,
             result.params,
@@ -159,63 +166,61 @@
             method="least_squares",
         ).params
 
         _shapes, heights = calculate_shape_heights(params_mc, cluster_mc)
 
         mc_list.append((params_mc, heights))
 
-    params_list, heights_list = zip(*mc_list)
+    params_list, heights_list = zip(*mc_list, strict=False)
 
     params_err, height_err = calc_err_from_mc(params_list, heights_list)
 
     return params_err, height_err
 
 
-def run_fit(clargs, spectra, clusters, file_logs):
-
-    print("- Lineshape fitting...", end="\n\n\n")
+def run_fit(clargs, spectra, clusters):
+    print_fitting()
 
     shifts = {}
 
     for cluster in clusters:
-
-        print_peaks(cluster.peaks, files=(sys.stdout, file_logs))
+        print_peaks(cluster.peaks)
 
         params = create_params(cluster.peaks, spectra, clargs)
 
         out = lf.minimize(
             residuals,
             params,
             args=(cluster, clargs.noise),
             method="least_squares",
             verbose=2,
         )
 
         _, heights = calculate_shape_heights(out.params, cluster)
 
-        out.init_vals.extend(heights.ravel())
-        out._calculate_statistics()
-
-        print(f"\nReduced Chi2 = {out.redchi}\n\n")
-        print(lf.fit_report(out, min_correl=0.5), end="\n\n\n", file=file_logs)
+        print_fit_report(out)
 
         params_err = {param.name: param.stderr for param in out.params.values()}
         height_err = np.full_like(heights, clargs.noise)
 
         shifts.update(
             {
                 peak.name: (out.params[f"p{i}_x0"].value, out.params[f"p{i}_y0"].value)
                 for i, peak in enumerate(cluster.peaks)
-            }
+            },
         )
 
         # Monte-Carlo
         if clargs.mc and int(clargs.mc[4]) > 1:
             params_err, height_err = monte_carlo(
-                clargs.mc, spectra, cluster, out, clargs.noise
+                clargs.mc,
+                spectra,
+                cluster,
+                out,
+                clargs.noise,
             )
 
         write_profiles(
             clargs.path_output,
             spectra.z_values,
             cluster,
             out.params,
@@ -223,50 +228,57 @@
             params_err,
             height_err,
         )
 
     return shifts
 
 
-def write_shifts(names, shifts, file_shifts):
+def write_shifts(names, shifts, file_shifts) -> None:
     for name in names:
         file_shifts.write(
-            f"{name:>15s} {shifts[name][1]:10.5f} {shifts[name][0]:10.5f}\n"
+            f"{name:>15s} {shifts[name][1]:10.5f} {shifts[name][0]:10.5f}\n",
         )
 
 
 def main() -> None:
-    """Run peakfit"""
-
+    """Run peakfit."""
     print_logo()
 
     parser = build_parser()
     clargs = parser.parse_args()
 
     spectra = read_spectra(clargs.path_spectra, clargs.path_z_values, clargs.exclude)
 
-    # Normalize spectra related to noise
-    if clargs.noise < 0.0:
-        clargs.noise = 1.0
-        print("Warning: `noise` option is < 0.0 (set to 1.0)")
+    if clargs.noise is not None and clargs.noise < 0.0:
+        clargs.noise = None
+
+    if clargs.noise is None:
+        clargs.noise = estimate_noise(spectra.data)
+        print_estimated_noise(clargs.noise)
 
     # Read peak list
     lines = clargs.path_list.read_text().replace("Ass", "#").splitlines()
     peaks = np.genfromtxt(
-        lines, dtype=None, encoding="utf-8", names=("names", "y", "x")
+        lines,
+        dtype=None,
+        encoding="utf-8",
+        names=("names", "y", "x"),
     )
 
     # Create the output directory
     clargs.path_output.mkdir(parents=True, exist_ok=True)
 
     # Cluster peaks
+    if clargs.contour_level is None:
+        clargs.contour_level = 5.0 * clargs.noise
     clusters = cluster_peaks(spectra, peaks, clargs.contour_level)
 
-    with (clargs.path_output / "logs.out").open("w") as file_logs:
-        shifts = run_fit(clargs, spectra, clusters, file_logs)
+    shifts = run_fit(clargs, spectra, clusters)
+
+    export_html(clargs.path_output / "logs.html")
 
-    with (clargs.path_output / "shifts.out").open("w") as file_shifts:
+    with (clargs.path_output / "shifts.list").open("w") as file_shifts:
         write_shifts(peaks["names"], shifts, file_shifts)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `peakfit-0.4.0/peakfit/plot_cest.py` & `peakfit-0.5.0/peakfit/plot_intensities.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,73 +2,49 @@
 import pathlib
 import re
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.backends.backend_pdf import PdfPages
 
+from peakfit.messages import print_filename, print_plotting, print_reading_files
+
 
 def get_args():
-    parser = argparse.ArgumentParser(description="Plot CEST profiles.")
+    parser = argparse.ArgumentParser(description="Plot intensity profiles.")
     parser.add_argument("-f", "--files", nargs="+", type=pathlib.Path)
-    parser.add_argument("--ref", nargs="+", type=int, default=-1)
     return parser.parse_args()
 
 
-def make_fig(name, data_cest, data_ref):
+def make_fig(name, data):
     fig = plt.figure()
     ax = fig.add_subplot(111)
-    ax.errorbar(
-        data_cest["offset"],
-        data_cest["intensity"] / np.mean(data_ref["intensity"]),
-        yerr=data_cest["error"] / abs(np.mean(data_ref["intensity"])),
-        fmt=".",
-    )
+    ax.errorbar(data["xlabel"], data["intensity"], yerr=data["error"], fmt=".")
     ax.set_title(name)
-    ax.set_xlabel(r"$B_1$ offset (Hz)")
-    ax.set_ylabel(r"$I/I_0$")
+    ax.set_ylabel(r"Intensities")
     plt.close()
 
     return fig
 
 
-def plot(args):
-
+def plot(args) -> None:
     figs = {}
 
-    print()
-    print("Reading files...")
+    print_reading_files()
 
     files_ordered = sorted(args.files, key=lambda x: int(re.sub(r"\D", "", str(x))))
 
     for a_file in files_ordered:
+        print_filename(a_file)
+        data = np.genfromtxt(a_file, dtype=None, names=("xlabel", "intensity", "error"))
+        figs[a_file.name] = make_fig(a_file.name, data)
 
-        print(f"  * {a_file.name}")
-
-        data = np.genfromtxt(a_file, dtype=None, names=("offset", "intensity", "error"))
-
-        if args.ref == -1:
-            ref = abs(data["offset"]) >= 1e4
-        else:
-            ref = np.full_like(data["offset"], False, dtype=bool)
-            ref[args.ref] = True
-        data_ref = data[ref]
-        data_cest = data[~ref]
-
-        figs[a_file.name] = make_fig(a_file.name, data_cest, data_ref)
-
-    print()
-    print("Plotting...")
+    print_plotting()
 
     with PdfPages("profiles.pdf") as pdf:
         for fig in figs.values():
             pdf.savefig(fig)
 
-    print("  * profiles.pdf")
-
-
-def main():
 
+def main() -> None:
     args = get_args()
     plot(args)
-
-    return
```

### Comparing `peakfit-0.4.0/peakfit/plot_cpmg.py` & `peakfit-0.5.0/peakfit/plot_cpmg.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 import pathlib
 import re
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.backends.backend_pdf import PdfPages
 
+from peakfit.messages import print_filename, print_plotting, print_reading_files
+
 
 def get_args():
     parser = argparse.ArgumentParser(description="Plot CPMG R2eff profiles.")
     parser.add_argument("-f", "--files", nargs="+", type=pathlib.Path)
     parser.add_argument("-t", "--time_t2", type=float)
     return parser.parse_args()
 
 
 def ncyc_to_nu_cpmg(ncyc, time_t2):
-
     nu_cpmg = []
 
     for a_ncyc in ncyc:
         if a_ncyc > 0.0:
             nu_cpmg.append(a_ncyc / time_t2)
         else:
             nu_cpmg.append(0.5 / time_t2)
@@ -28,17 +29,17 @@
 
 
 def intensity_to_r2eff(intensity, intensity_ref, time_t2):
     return -np.log(intensity / intensity_ref) / time_t2
 
 
 def make_ens(data, size=1000):
-
     return data["intensity"] + data["error"] * np.random.randn(
-        size, len(data["intensity"])
+        size,
+        len(data["intensity"]),
     )
 
 
 def make_fig(name, nu_cpmg, r2_exp, r2_erd, r2_eru):
     fig = plt.figure()
     ax = fig.add_subplot(111)
     ax.errorbar(nu_cpmg, r2_exp, yerr=(r2_erd, r2_eru), fmt="o")
@@ -46,65 +47,52 @@
     ax.set_xlabel(r"$\nu_{CPMG}$ (Hz)")
     ax.set_ylabel(r"$R_{2,eff}$ (s$^{-1}$)")
     plt.close()
 
     return fig
 
 
-def plot(files, time_t2):
-
+def plot(files, time_t2) -> None:
     figs = {}
 
-    print()
-    print("Reading files...")
+    print_reading_files()
 
     files_ordered = sorted(files, key=lambda x: int(re.sub(r"\D", "", str(x))))
 
     for a_file in files_ordered:
-
-        print(f"  * {a_file.name}")
-
+        print_filename(a_file)
         data = np.loadtxt(
             a_file,
             dtype={
                 "names": ("ncyc", "intensity", "error"),
                 "formats": ("i4", "f8", "f8"),
             },
         )
-
         data_ref = data[data["ncyc"] == 0]
         data_cpmg = data[data["ncyc"] != 0]
-
         intensity_ref = np.mean(data_ref["intensity"])
         error_ref = np.mean(data_ref["error"]) / np.sqrt(len(data_ref))
-
         nu_cpmg = ncyc_to_nu_cpmg(data_cpmg["ncyc"], time_t2)
-
         r2_exp = intensity_to_r2eff(data_cpmg["intensity"], intensity_ref, time_t2)
         r2_ens = intensity_to_r2eff(
             make_ens(data_cpmg),
             make_ens(
-                {"intensity": np.array([intensity_ref]), "error": np.array([error_ref])}
+                {
+                    "intensity": np.array([intensity_ref]),
+                    "error": np.array([error_ref]),
+                },
             ),
             time_t2,
         )
-
         r2_erd, r2_eru = abs(np.percentile(r2_ens, [15.9, 84.1], axis=0) - r2_exp)
-
         figs[a_file.name] = make_fig(a_file.name, nu_cpmg, r2_exp, r2_erd, r2_eru)
 
-    print()
-    print("Plotting...")
+    print_plotting()
 
     with PdfPages("profiles.pdf") as pdf:
         for fig in figs.values():
             pdf.savefig(fig)
 
-    print("  * profiles.pdf")
-
-
-def main():
 
+def main() -> None:
     args = get_args()
     plot(args.files, args.time_t2)
-
-    return
```

### Comparing `peakfit-0.4.0/peakfit/plot_intensities.py` & `peakfit-0.5.0/peakfit/plot_cest.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,57 +2,63 @@
 import pathlib
 import re
 
 import matplotlib.pyplot as plt
 import numpy as np
 from matplotlib.backends.backend_pdf import PdfPages
 
+from peakfit.messages import print_filename, print_plotting, print_reading_files
+
 
 def get_args():
-    parser = argparse.ArgumentParser(description="Plot intensity profiles.")
+    parser = argparse.ArgumentParser(description="Plot CEST profiles.")
     parser.add_argument("-f", "--files", nargs="+", type=pathlib.Path)
+    parser.add_argument("--ref", nargs="+", type=int, default=-1)
     return parser.parse_args()
 
 
-def make_fig(name, data):
+def make_fig(name, offset, intensity, error):
     fig = plt.figure()
     ax = fig.add_subplot(111)
-    ax.errorbar(data["xlabel"], data["intensity"], yerr=data["error"], fmt=".")
+    ax.errorbar(offset, intensity, yerr=error, fmt=".")
     ax.set_title(name)
-    ax.set_ylabel(r"Intensities")
+    ax.set_xlabel(r"$B_1$ offset (Hz)")
+    ax.set_ylabel(r"$I/I_0$")
     plt.close()
 
     return fig
 
 
-def plot(args):
-
+def plot(args) -> None:
     figs = {}
 
-    print()
-    print("Reading files...")
+    print_reading_files()
 
     files_ordered = sorted(args.files, key=lambda x: int(re.sub(r"\D", "", str(x))))
 
     for a_file in files_ordered:
+        print_filename(a_file)
+        offset, intensity, error = np.loadtxt(a_file, unpack=True)
+        if args.ref == -1:
+            ref = abs(offset) >= 1e4
+        else:
+            ref = np.full_like(offset, fill_value=False, dtype=bool)
+            ref[args.ref] = True
+
+        intensity_ref = np.mean(intensity[ref])
+
+        offset = offset[~ref]
+        intensity = intensity[~ref] / intensity_ref
+        error = error[~ref] / abs(intensity_ref)
 
-        print(f"  * {a_file.name}")
-
-        data = np.genfromtxt(a_file, dtype=None, names=("xlabel", "intensity", "error"))
-        figs[a_file.name] = make_fig(a_file.name, data)
+        figs[a_file.name] = make_fig(a_file.name, offset, intensity, error)
 
-    print()
-    print("Plotting...")
+    print_plotting()
 
     with PdfPages("profiles.pdf") as pdf:
         for fig in figs.values():
             pdf.savefig(fig)
 
-    print("  * profiles.pdf")
-
-
-def main():
 
+def main() -> None:
     args = get_args()
     plot(args)
-
-    return
```

### Comparing `peakfit-0.4.0/peakfit/shapes.py` & `peakfit-0.5.0/peakfit/shapes.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 def pvoigt2d(x, y, x0, y0, x_fwhm, y_fwhm, x_eta, y_eta):
     shapex = ls.sim_pvoigt_fwhm(x, x0, x_fwhm, x_eta)
     shapey = ls.sim_pvoigt_fwhm(y, y0, y_fwhm, y_eta)
     return shapex * shapey
 
 
 def create_params(peaks, spectra, clargs):
-
     ucx = spectra.ucx
     ucy = spectra.ucy
 
     hz2ppm_x = abs(ucx.ppm(ucx.f(1, "hz")))
     hz2ppm_y = abs(ucy.ppm(ucy.f(1, "hz")))
 
     vary_position = not clargs.fixed
```

