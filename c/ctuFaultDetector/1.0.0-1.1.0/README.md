# Comparing `tmp/ctuFaultDetector-1.0.0.tar.gz` & `tmp/ctuFaultDetector-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctuFaultDetector-1.0.0.tar", last modified: Sun May 19 17:15:01 2024, max compression
+gzip compressed data, was "ctuFaultDetector-1.1.0.tar", last modified: Wed May 22 00:02:58 2024, max compression
```

## Comparing `ctuFaultDetector-1.0.0.tar` & `ctuFaultDetector-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 17:15:01.718801 ctuFaultDetector-1.0.0/
--rw-rw-rw-   0        0        0      762 2024-05-19 17:15:01.717800 ctuFaultDetector-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-19 17:15:01.704801 ctuFaultDetector-1.0.0/PROD/
--rw-rw-rw-   0        0        0      165 2024-05-16 20:35:15.000000 ctuFaultDetector-1.0.0/PROD/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 17:15:01.706801 ctuFaultDetector-1.0.0/PROD/metrics/
--rw-rw-rw-   0        0        0        0 2024-05-16 20:35:15.000000 ctuFaultDetector-1.0.0/PROD/metrics/__init__.py
--rw-rw-rw-   0        0        0    10195 2024-04-25 14:37:05.000000 ctuFaultDetector-1.0.0/PROD/metrics/dtw_barycenter.py
-drwxrwxrwx   0        0        0        0 2024-05-19 17:15:01.710801 ctuFaultDetector-1.0.0/PROD/models/
--rw-rw-rw-   0        0        0        0 2024-05-16 20:35:15.000000 ctuFaultDetector-1.0.0/PROD/models/__init__.py
--rw-rw-rw-   0        0        0      825 2024-04-25 14:37:05.000000 ctuFaultDetector-1.0.0/PROD/models/baseModel.py
--rw-rw-rw-   0        0        0    17033 2024-05-16 20:35:15.000000 ctuFaultDetector-1.0.0/PROD/models/deviationClassifier.py
--rw-rw-rw-   0        0        0    15670 2024-05-16 20:35:15.000000 ctuFaultDetector-1.0.0/PROD/models/featureClassifier.py
--rw-rw-rw-   0        0        0     7410 2024-05-15 13:37:39.000000 ctuFaultDetector-1.0.0/PROD/models/lstmClassifier.py
-drwxrwxrwx   0        0        0        0 2024-05-19 17:15:01.711801 ctuFaultDetector-1.0.0/PROD/support/
--rw-rw-rw-   0        0        0        0 2024-05-16 20:35:15.000000 ctuFaultDetector-1.0.0/PROD/support/__init__.py
--rw-rw-rw-   0        0        0     5744 2024-05-15 13:37:39.000000 ctuFaultDetector-1.0.0/PROD/support/my_k_means.py
--rw-rw-rw-   0        0        0     3128 2024-05-15 13:37:39.000000 ctuFaultDetector-1.0.0/PROD/utils.py
--rw-rw-rw-   0        0        0     7552 2024-05-15 13:37:39.000000 ctuFaultDetector-1.0.0/PROD/visual.py
--rw-rw-rw-   0        0        0      437 2024-04-25 14:37:05.000000 ctuFaultDetector-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 17:15:01.717800 ctuFaultDetector-1.0.0/ctuFaultDetector.egg-info/
--rw-rw-rw-   0        0        0      762 2024-05-19 17:15:01.000000 ctuFaultDetector-1.0.0/ctuFaultDetector.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      518 2024-05-19 17:15:01.000000 ctuFaultDetector-1.0.0/ctuFaultDetector.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 17:15:01.000000 ctuFaultDetector-1.0.0/ctuFaultDetector.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      145 2024-05-19 17:15:01.000000 ctuFaultDetector-1.0.0/ctuFaultDetector.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-19 17:15:01.000000 ctuFaultDetector-1.0.0/ctuFaultDetector.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 17:15:01.718801 ctuFaultDetector-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      888 2024-05-19 17:14:46.000000 ctuFaultDetector-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 00:02:58.526991 ctuFaultDetector-1.1.0/
+-rw-rw-rw-   0        0        0      762 2024-05-22 00:02:58.525988 ctuFaultDetector-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      437 2024-04-25 14:37:05.000000 ctuFaultDetector-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 00:02:58.512991 ctuFaultDetector-1.1.0/ctuFaultDetector/
+-rw-rw-rw-   0        0        0      165 2024-05-22 00:01:14.000000 ctuFaultDetector-1.1.0/ctuFaultDetector/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 00:02:58.517989 ctuFaultDetector-1.1.0/ctuFaultDetector/metrics/
+-rw-rw-rw-   0        0        0        0 2024-05-22 00:01:15.000000 ctuFaultDetector-1.1.0/ctuFaultDetector/metrics/__init__.py
+-rw-rw-rw-   0        0        0    10195 2024-05-22 00:00:52.000000 ctuFaultDetector-1.1.0/ctuFaultDetector/metrics/dtw_barycenter.py
+drwxrwxrwx   0        0        0        0 2024-05-22 00:02:58.522991 ctuFaultDetector-1.1.0/ctuFaultDetector/models/
+-rw-rw-rw-   0        0        0        0 2024-05-22 00:01:15.000000 ctuFaultDetector-1.1.0/ctuFaultDetector/models/__init__.py
+-rw-rw-rw-   0        0        0      825 2024-05-22 00:00:52.000000 ctuFaultDetector-1.1.0/ctuFaultDetector/models/baseModel.py
+-rw-rw-rw-   0        0        0    23853 2024-05-22 00:00:52.000000 ctuFaultDetector-1.1.0/ctuFaultDetector/models/deviationClassifier.py
+-rw-rw-rw-   0        0        0    13990 2024-05-22 00:00:52.000000 ctuFaultDetector-1.1.0/ctuFaultDetector/models/featureClassifier.py
+-rw-rw-rw-   0        0        0     7410 2024-05-22 00:00:52.000000 ctuFaultDetector-1.1.0/ctuFaultDetector/models/lstmClassifier.py
+drwxrwxrwx   0        0        0        0 2024-05-22 00:02:58.523991 ctuFaultDetector-1.1.0/ctuFaultDetector/support/
+-rw-rw-rw-   0        0        0        0 2024-05-22 00:01:15.000000 ctuFaultDetector-1.1.0/ctuFaultDetector/support/__init__.py
+-rw-rw-rw-   0        0        0     5744 2024-05-22 00:00:52.000000 ctuFaultDetector-1.1.0/ctuFaultDetector/support/my_k_means.py
+-rw-rw-rw-   0        0        0     6290 2024-05-22 00:00:52.000000 ctuFaultDetector-1.1.0/ctuFaultDetector/utils.py
+-rw-rw-rw-   0        0        0     8869 2024-05-22 00:00:52.000000 ctuFaultDetector-1.1.0/ctuFaultDetector/visual.py
+drwxrwxrwx   0        0        0        0 2024-05-22 00:02:58.524989 ctuFaultDetector-1.1.0/ctuFaultDetector.egg-info/
+-rw-rw-rw-   0        0        0      762 2024-05-22 00:02:58.000000 ctuFaultDetector-1.1.0/ctuFaultDetector.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      662 2024-05-22 00:02:58.000000 ctuFaultDetector-1.1.0/ctuFaultDetector.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 00:02:58.000000 ctuFaultDetector-1.1.0/ctuFaultDetector.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      145 2024-05-22 00:02:58.000000 ctuFaultDetector-1.1.0/ctuFaultDetector.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-22 00:02:58.000000 ctuFaultDetector-1.1.0/ctuFaultDetector.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 00:02:58.526991 ctuFaultDetector-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      888 2024-05-22 00:02:33.000000 ctuFaultDetector-1.1.0/setup.py
```

### Comparing `ctuFaultDetector-1.0.0/PKG-INFO` & `ctuFaultDetector-1.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctuFaultDetector
-Version: 1.0.0
+Version: 1.1.0
 Summary: Anomaly detection in time series model
 Home-page: https://github.com/altrna/Anomaly-detection-in-timeseries
 Author: Ales Trna
 Author-email: altrna@fel.cvut.cz
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `ctuFaultDetector-1.0.0/PROD/metrics/dtw_barycenter.py` & `ctuFaultDetector-1.1.0/ctuFaultDetector/metrics/dtw_barycenter.py`

 * *Files identical despite different names*

### Comparing `ctuFaultDetector-1.0.0/PROD/models/baseModel.py` & `ctuFaultDetector-1.1.0/ctuFaultDetector/models/baseModel.py`

 * *Files identical despite different names*

### Comparing `ctuFaultDetector-1.0.0/PROD/models/featureClassifier.py` & `ctuFaultDetector-1.1.0/ctuFaultDetector/models/featureClassifier.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,24 @@
 from tslearn.utils import to_time_series_dataset
 from scipy.stats import chi2
 import numpy as np
 import pandas as pd
 import pickle
 import time
 from datetime import datetime
-from PROD.metrics.dtw_barycenter import compute_dtw_dists, get_distance
-from PROD.visual import plot_samples, plot_one_6dim_signal
-from PROD.support.my_k_means import classify_kmeans, get_cluster_params, GaussianClassifier
-from PROD.utils import transform_pd_to_npy, set_signals_to_same_length
+from ctuFaultDetector.metrics.dtw_barycenter import compute_dtw_dists, get_distance
+from ctuFaultDetector.visual import plot_samples, plot_one_6dim_signal
+from ctuFaultDetector.support.my_k_means import classify_kmeans, get_cluster_params, GaussianClassifier
+from ctuFaultDetector.utils import transform_pd_to_npy, set_signals_to_same_length
 
 
 class featureClassifier():
+    """
+    
+    """
     def __init__(self, n_clusters = None, method = [1,5]) -> None:
         self.barycenter_dtw = None
         self.barycenter_euclid = None
         self.classifier = None
         self.n_clusters = n_clusters
         self.method = method
         self.dtw_error = None
@@ -134,44 +137,14 @@
         number_of_signals_to_train_on = int(online_train_ratio*len(correct_signals))
         self.online_fit(correct_signals[:number_of_signals_to_train_on])
     
     def retrain_classifier(self, metric = "ACC", value = 0.95, n_steps = 100):
         print(self.c_samples)
         self.classifier.set_confidence_interval(self.c_samples, self.w_samples, metric = metric, value = value, n_steps=n_steps, report_result = False)
         #self.show_samples()
-
-
-    #def known_cluster_fit(self, training_signals, n_clusters = 4, method = [1, 5], vis = True, keep_barycenters = False):
-    #    if self.method != method:
-    #        keep_barycenters = False
-    #        raise Exception(f"New method {method} does not equal the state of the art method {self.method}.")
-    #    if not keep_barycenters:
-    #        self.barycenter_dtw = []
-    #        self.barycenter_euclid = []
-    #    correct_signals = [[sig.signal for i, sig in enumerate(training_signals) if ((i+1)%n_clusters == j and sig.label == True)] for j in range(n_clusters)]
-    #    for i, cluster in enumerate(correct_signals):
-    #        training_set = to_time_series_dataset(cluster)
-    #        self.barycenter_dtw.append(dtw_barycenter_averaging(training_set))
-    #        self.barycenter_euclid.append(euclidean_barycenter(training_set))
-    #        print(f"INFO: Computed barycenter: {i + 1} out of: {n_clusters}.")
-    #    corsig = [i.signal for i in training_signals if i.label == True]
-    #    wrosig = [i.signal for i in training_signals if i.label == False]
-    #    c, w, b, eb = compute_dtw_dists(corsig,
-    #                                    wrosig,
-    #                                    self.barycenter_dtw,
-    #                                    self.barycenter_euclid,
-    #                                    method = method)
-    #    if vis:
-    #        plot_samples(c, w, b, eb, method)
-    #    data_to_fit = np.array(c).T
-    #    centroids, clusters = classify_kmeans(data_to_fit, n_clusters)
-    #    cluster_params = get_cluster_params(centroids, data_to_fit, clusters)
-    #    print(cluster_params)
-    #    self.classifier = GaussianClassifier(cluster_params)
-        
     
     def __repr__(self) -> str:
         return f"""
         Feature Classifier:
             Number of clusters: {self.n_clusters}
             Confidence treshhold: {None if self.classifier is None else self.classifier.confidence_threshold}
             Number of dtw barycenters: {len(self.barycenter_dtw)}
```

### Comparing `ctuFaultDetector-1.0.0/PROD/models/lstmClassifier.py` & `ctuFaultDetector-1.1.0/ctuFaultDetector/models/lstmClassifier.py`

 * *Files identical despite different names*

### Comparing `ctuFaultDetector-1.0.0/PROD/support/my_k_means.py` & `ctuFaultDetector-1.1.0/ctuFaultDetector/support/my_k_means.py`

 * *Files identical despite different names*

### Comparing `ctuFaultDetector-1.0.0/PROD/visual.py` & `ctuFaultDetector-1.1.0/ctuFaultDetector/visual.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,68 +1,91 @@
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
-from PROD.utils import transform_pd_to_npy
-from PROD.metrics.dtw_barycenter import METHODS_LABEL_DICT
+from utils import transform_pd_to_npy
+from metrics.dtw_barycenter import METHODS_LABEL_DICT
 import pickle
 from scipy.interpolate import interp1d
 
 
-def draw_roc_from_dict(roc_dict, save_fig = None, title = None, scatter = False, fig = None):
+def draw_roc_from_dict(roc_dict, save_fig = None, title = None, scatter = False):
+    """
+    Draws ROC curve from the saved ROC dictionary, used to create ROC figures in the thesis.
+    Args:
+        roc_dict : str - path to the saved dict
+        save_fig : None|str - save generated figure if not none - name of the figure
+        title : str - title for the ROC plt plot
+        scatter : bool - use normal plot if False, else use scatter plot
+    """
     def mean_roc(roc_curves, num_points=100):
         mean_fpr = np.linspace(0, 1, num_points)
         interp_tprs = []
         for roc in roc_curves:
             fpr, tpr = roc[1], roc[0]
             interp_func = interp1d(fpr, tpr, kind='linear', fill_value="extrapolate")
             interp_tprs.append(interp_func(mean_fpr))
         mean_tpr = np.mean(interp_tprs, axis=0) 
         return mean_fpr, mean_tpr
-    #plt.figure(figsize=(4,4))
     colors = ["red", "green", "blue", "orange", "brown"]
     if isinstance(roc_dict, str):
         with open(roc_dict, "rb") as f:
             total_roc = pickle.load(f)
     elif isinstance(roc_dict, dict):
         total_roc = roc_dict
     aucs = []
     curves = [np.flip(i["ROC"], axis=1) for i in total_roc]
     fpr_m, tpr_m = mean_roc(curves)
     for i in range(len(curves)):
         if scatter:
             plt.scatter(curves[i][1,:], curves[i][0,:], color = colors[i%5], marker="x", s=10)
         else:
             plt.plot(curves[i][1,:], curves[i][0,:], color = "tab:green", alpha = 0.75, label="")
-        #auc = np.trapz(np.nan_to_num(np.flip(np.append(np.flip(np.append(curves[i][0, :], 1)), 0))), np.nan_to_num(np.flip(np.append(np.flip(np.append(curves[i][1, :], 1)), 0))))
+
         auc = np.trapz(np.nan_to_num(np.flip(np.append(curves[i][0, :], 0))), np.nan_to_num(np.flip(np.append(curves[i][1, :], 0))))
         aucs.append(auc)
         print(f"AUC is {auc}")
     if scatter:
         pass
-        #plt.plot(tpr_m, fpr_m, color = "blue", label="Mean ROC")
+
     else:
-        #plt.plot(np.nan_to_num(np.flip(np.append(np.flip(np.append(fpr_m, 1)), 0))), np.nan_to_num(np.flip(np.append(np.flip(np.append(tpr_m, 1)), 0))), color = "blue", label="Mean ROC")
+
         plt.plot(fpr_m, tpr_m, color = "blue", label="Mean ROC")
     print(f"Mean AUC is: {np.mean(aucs)}")
     plt.plot([0,1], [0,1], color="black", linestyle= "dotted")
     plt.legend(loc="lower right")
     plt.xlim([0,1])
     plt.ylim([0,1])
     plt.xlabel("False positive rate")
     plt.ylabel("True positive rate")
     plt.grid()
     if title is not None:
         plt.title(title)
     if save_fig is not None:
         name = str(save_fig) if len(save_fig) > 4 and str(save_fig)[-4:] == ".pdf" else str(save_fig) + ".pdf"
         plt.savefig(name , format='pdf', bbox_inches='tight')
-    #plt.show()
-    return total_roc
+    plt.show()
+    return fpr_m, tpr_m
 
 def plot_one_6dim_signal(signal1, avg = None, std = None, sensitivity = None, save_fig = None, anomaly_highlight = False, anomalies = [], anomalies_all = [], real_len = 0):
+    """
+    Plot a 6-dimensional signal  - used for debugging, testing and figures in the thesis
+    Args:
+        signal1 : np.ndarray - signal to be plotted
+        avg : np.ndarray|None - mean signal to be plotted as well if not None
+        std : np.ndarray|None - standard deviation signal for plotting the blue zone if not None
+        sensitivity : int - size of the blue zone std deviation multiplier
+        save_fig : str|None - name of the figure to be saved in pdf format if not None
+        anomaly_highlight : bool - highlight anomalies as in figure 3.2
+        anomalies : list - list of anomalies for each dimension
+        anomalies_all : list - list of anomalies for all dimensions
+        real_len : int = show only part of the signal of length real_len
+    Returns:
+        None, plots the signal
+
+    """
     fig, ax = plt.subplots(6, 1, figsize=(6.5, 5), sharex=False)
     ylabels = [ "Force x",
                 "Force y",
                 "Force z",
                 "Torque x",
                 "Torque y",
                 "Torque z"
@@ -92,50 +115,58 @@
             for k in range(len(anomalies_all[i])):
                 ax[i].axvspan(*anomalies_all[i][k], color='red', alpha = 0.6)
     if save_fig is not None:
         name = str(save_fig) if len(save_fig) > 4 and str(save_fig)[-4:] == ".pdf" else str(save_fig) + ".pdf"
         plt.savefig(name , format='pdf', bbox_inches='tight')
     plt.show()
 
-def plot_6dim_signal_dataset(signal_dataset, save_fig = None, anomaly_highlight = False, anomalies_start = [], anomalies_end = []):
+def plot_6dim_signal_dataset(signal_dataset, save_fig = None):
+    """
+    Function for plotting the whole dataset, used for getting a general information about the dataset
+    Args:
+        signal_dataset : [(np.ndarray, bool), ...] - list of tuples (signal, label)
+        save_fig : None|str - name of the figure to be saved in pdf figure if not None
+    Returns:
+        None, plots the dataset plot
+    """
     fig, ax = plt.subplots(6, 1, figsize=(6.5, 5), sharex=True)
     ylabels = [ "Force x",
                 "Force y",
                 "Force z",
                 "Torque x",
                 "Torque y",
                 "Torque z"
              ]
     for signal in signal_dataset:
         xaxis = np.arange(np.shape(signal[0])[0])
-        color = "blue" if signal[1] else "red"
+        color = "blue" if not signal[1] else "red"
         sig = transform_pd_to_npy(signal[0])
         for i in range(0, 6):
             ax[i].plot(xaxis, sig[ : , i], color = color, linewidth = 1)
             ax[i].set_ylabel(ylabels[i])
             if i < 5:
                 ax[i].set_xticklabels([])
         ax[5].set_xlabel("Time")
         #fig.suptitle("Sample signal of a process", fontweight="bold", fontsize = 12)
         fig.align_ylabels()
-    if anomaly_highlight:
-        assert len(anomalies_start) == len(anomalies_end)
-        for i in range(0,6):
-            for j in range(len(anomalies_start)):
-                ax[i].axvspan(anomalies_start[j], anomalies_end[j], color='red', alpha=0.3)
     if save_fig is not None:
         name = str(save_fig) if len(save_fig) > 4 and str(save_fig)[-4:] == ".pdf" else str(save_fig) + ".pdf"
         plt.savefig(name , format='pdf', bbox_inches='tight')
     plt.show()
 
-def plot_samples(correct_points, wrong_points, barycenters, ebarycenters = [[], []], method = [1, 5], title = "", correct_idx = [], anom_idx = [], save_fig1 = "samples"):
+def plot_samples(correct_points, wrong_points, method = [1, 5], title = "", correct_idx = [], anom_idx = [], save_fig1 = "samples"):
+    """
+    Plots the feature vectors in memory of a feature classifier
+    Args:
+        correct_points : np.ndarray|list - feature vectors from non-anomalous processes
+        wrong_points : np.ndarray|list - feature vectors from anomalous processes
+        method : [int, int] - features of the signal, see ctuFaultDetector.metrics.dtw_barycenter.method.get_distance function
+    """
     scatter_if_not_empty(correct_points, color="blue", marker="+")
     scatter_if_not_empty(wrong_points, color="red", marker="x")
-    #scatter_if_not_empty(barycenters, color="green", marker="o")
-    #scatter_if_not_empty(ebarycenters, color="orange", marker="o")
     plt.grid(True)
     plt.xlabel(METHODS_LABEL_DICT[method[0]])
     plt.ylabel(METHODS_LABEL_DICT[method[1]])
     plt.title(title)
     plt.legend(["Successfull process",
                 "Failed process",
                 "Barycenter distance",
@@ -150,13 +181,21 @@
             plt.annotate(label+1, (wrong_points[i]))
     if save_fig1 is not None:
         name = str(save_fig1) if len(save_fig1) > 4 and str(save_fig1)[-4:] == ".pdf" else str(save_fig1) + ".pdf"
         plt.savefig(name , format='pdf', bbox_inches='tight')
     plt.show()
 
 def scatter_if_not_empty(points, color, marker):
+    """
+    If "points" is not empty, creates a scatter chart of them
+    Args:
+        points : list (can be empty) - points to be scattered
+        color : str from plt colors - color of the points
+        marker : str from plt markers - marker used for points
+    Returns:
+        None, scatters the points.
+    """
     if points:
         if np.shape(points)[0] != 2:
             points = np.array(points).T
         if points is not None:
             plt.scatter(*points, color=color, marker=marker)
-
```

### Comparing `ctuFaultDetector-1.0.0/ctuFaultDetector.egg-info/PKG-INFO` & `ctuFaultDetector-1.1.0/ctuFaultDetector.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctuFaultDetector
-Version: 1.0.0
+Version: 1.1.0
 Summary: Anomaly detection in time series model
 Home-page: https://github.com/altrna/Anomaly-detection-in-timeseries
 Author: Ales Trna
 Author-email: altrna@fel.cvut.cz
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `ctuFaultDetector-1.0.0/setup.py` & `ctuFaultDetector-1.1.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name="ctuFaultDetector",
-    version="1.0.0",
+    version="1.1.0",
     author="Ales Trna",
     author_email="altrna@fel.cvut.cz",
     description="Anomaly detection in time series model",
     long_description="Long Description",
     packages=find_packages(),
     url="https://github.com/altrna/Anomaly-detection-in-timeseries",
     classifiers=[
```

