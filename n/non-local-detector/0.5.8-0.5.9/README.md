# Comparing `tmp/non_local_detector-0.5.8.tar.gz` & `tmp/non_local_detector-0.5.9.tar.gz`

## Comparing `non_local_detector-0.5.8.tar` & `non_local_detector-0.5.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/.gitattributes
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/environment.yml
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/environment_gpu.yml
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/.github/workflows/test_package_build.yml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/.vscode/settings.json
--rw-r--r--   0        0        0   188206 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/notebooks/test.ipynb
--rw-r--r--   0        0        0   180074 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/notebooks/test_clusterless.ipynb
--rw-r--r--   0        0        0  1311936 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/notebooks/test_non_local.ipynb
--rw-r--r--   0        0        0   163929 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/notebooks/test_non_local_2D.ipynb
--rw-r--r--   0        0        0   719261 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/notebooks/test_non_local_spike_times.ipynb
--rw-r--r--   0        0        0    55241 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/notebooks/test_non_stationary_discrete_transition.ipynb
--rw-r--r--   0        0        0   200972 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/notebooks/test_simulated.ipynb
--rw-r--r--   0        0        0  1721172 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/notebooks/test_simulated2.ipynb
--rw-r--r--   0        0        0   476355 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/notebooks/test_sorted_spikes.ipynb
--rw-r--r--   0        0        0   403327 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/notebooks/test_spike_times.ipynb
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/__init__.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/_version.py
--rw-r--r--   0        0        0    14326 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/continuous_state_transitions.py
--rw-r--r--   0        0        0     7690 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/core.py
--rw-r--r--   0        0        0    22767 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/discrete_state_transitions.py
--rw-r--r--   0        0        0    28255 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/environment.py
--rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/initial_conditions.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/observation_models.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/types.py
--rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/analysis/__init__.py
--rw-r--r--   0        0        0    12373 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/analysis/distance1D.py
--rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/analysis/distance2D.py
--rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/analysis/highest_posterior_density.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/analysis/posterior.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/likelihoods/__init__.py
--rw-r--r--   0        0        0    13971 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/likelihoods/clusterless_kde.py
--rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/likelihoods/common.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/likelihoods/no_spike.py
--rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/likelihoods/sorted_spikes_glm.py
--rw-r--r--   0        0        0     6953 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/likelihoods/sorted_spikes_kde.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/model_checking/__init__.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/model_checking/clusterless.py
--rw-r--r--   0        0        0    11295 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/model_checking/sorted_spikes.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/models/__init__.py
--rw-r--r--   0        0        0    53876 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/models/base.py
--rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/models/cont_frag_model.py
--rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/models/decoder.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/models/multienvironment_model.py
--rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/models/non_local_model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/simulate/__init__.py
--rw-r--r--   0        0        0    12846 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/simulate/clusterless_simulation.py
--rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/simulate/simulate.py
--rw-r--r--   0        0        0    12776 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/simulate/sorted_spikes_simulation.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/tests/test_version_import.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/visualization/__init__.py
--rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/visualization/figurl_1D.py
--rw-r--r--   0        0        0    15888 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/visualization/figurl_2D.py
--rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/src/non_local_detector/visualization/static.py
--rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/LICENSE
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/README.md
--rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 non_local_detector-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/.gitattributes
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/environment.yml
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/environment_gpu.yml
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/.github/workflows/test_package_build.yml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/.vscode/settings.json
+-rw-r--r--   0        0        0   188206 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/notebooks/test.ipynb
+-rw-r--r--   0        0        0   180074 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/notebooks/test_clusterless.ipynb
+-rw-r--r--   0        0        0  1311936 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/notebooks/test_non_local.ipynb
+-rw-r--r--   0        0        0   163929 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/notebooks/test_non_local_2D.ipynb
+-rw-r--r--   0        0        0   719261 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/notebooks/test_non_local_spike_times.ipynb
+-rw-r--r--   0        0        0    55241 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/notebooks/test_non_stationary_discrete_transition.ipynb
+-rw-r--r--   0        0        0   200972 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/notebooks/test_simulated.ipynb
+-rw-r--r--   0        0        0  1721172 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/notebooks/test_simulated2.ipynb
+-rw-r--r--   0        0        0   476355 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/notebooks/test_sorted_spikes.ipynb
+-rw-r--r--   0        0        0   403327 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/notebooks/test_spike_times.ipynb
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/_version.py
+-rw-r--r--   0        0        0    14326 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/continuous_state_transitions.py
+-rw-r--r--   0        0        0     8593 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/core.py
+-rw-r--r--   0        0        0    22767 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/discrete_state_transitions.py
+-rw-r--r--   0        0        0    28255 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/environment.py
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/initial_conditions.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/observation_models.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/types.py
+-rw-r--r--   0        0        0      657 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/analysis/__init__.py
+-rw-r--r--   0        0        0    12373 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/analysis/distance1D.py
+-rw-r--r--   0        0        0    12709 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/analysis/distance2D.py
+-rw-r--r--   0        0        0     1974 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/analysis/highest_posterior_density.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/analysis/posterior.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/likelihoods/__init__.py
+-rw-r--r--   0        0        0    13971 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/likelihoods/clusterless_kde.py
+-rw-r--r--   0        0        0     3969 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/likelihoods/common.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/likelihoods/no_spike.py
+-rw-r--r--   0        0        0     8082 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/likelihoods/sorted_spikes_glm.py
+-rw-r--r--   0        0        0     6953 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/likelihoods/sorted_spikes_kde.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/model_checking/__init__.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/model_checking/clusterless.py
+-rw-r--r--   0        0        0    11295 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/model_checking/sorted_spikes.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/models/__init__.py
+-rw-r--r--   0        0        0    53876 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/models/base.py
+-rw-r--r--   0        0        0     5040 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/models/cont_frag_model.py
+-rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/models/decoder.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/models/multienvironment_model.py
+-rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/models/non_local_model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/simulate/__init__.py
+-rw-r--r--   0        0        0    12846 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/simulate/clusterless_simulation.py
+-rw-r--r--   0        0        0     6840 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/simulate/simulate.py
+-rw-r--r--   0        0        0    12776 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/simulate/sorted_spikes_simulation.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/tests/test_version_import.py
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/visualization/__init__.py
+-rw-r--r--   0        0        0     5942 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/visualization/figurl_1D.py
+-rw-r--r--   0        0        0    15888 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/visualization/figurl_2D.py
+-rw-r--r--   0        0        0     5074 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/src/non_local_detector/visualization/static.py
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/LICENSE
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/README.md
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     3000 2020-02-02 00:00:00.000000 non_local_detector-0.5.9/PKG-INFO
```

### Comparing `non_local_detector-0.5.8/.github/workflows/test_package_build.yml` & `non_local_detector-0.5.9/.github/workflows/test_package_build.yml`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/notebooks/test.ipynb` & `non_local_detector-0.5.9/notebooks/test.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/notebooks/test_clusterless.ipynb` & `non_local_detector-0.5.9/notebooks/test_clusterless.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/notebooks/test_non_local.ipynb` & `non_local_detector-0.5.9/notebooks/test_non_local.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/notebooks/test_non_local_2D.ipynb` & `non_local_detector-0.5.9/notebooks/test_non_local_2D.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/notebooks/test_non_local_spike_times.ipynb` & `non_local_detector-0.5.9/notebooks/test_non_local_spike_times.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/notebooks/test_non_stationary_discrete_transition.ipynb` & `non_local_detector-0.5.9/notebooks/test_non_stationary_discrete_transition.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/notebooks/test_simulated.ipynb` & `non_local_detector-0.5.9/notebooks/test_simulated.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/notebooks/test_simulated2.ipynb` & `non_local_detector-0.5.9/notebooks/test_simulated2.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/notebooks/test_sorted_spikes.ipynb` & `non_local_detector-0.5.9/notebooks/test_sorted_spikes.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/notebooks/test_spike_times.ipynb` & `non_local_detector-0.5.9/notebooks/test_spike_times.ipynb`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/continuous_state_transitions.py` & `non_local_detector-0.5.9/src/non_local_detector/continuous_state_transitions.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/core.py` & `non_local_detector-0.5.9/src/non_local_detector/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,21 +3,48 @@
 
 import jax
 import jax.numpy as jnp
 import numpy as np
 
 np.seterr(divide="ignore", invalid="ignore")
 
+EPS = 1e-15
+
 
 def convert_to_state_probability(
     causal_posterior: np.ndarray,
     acausal_posterior: np.ndarray,
     predictive_distribution: np.ndarray,
     state_ind: np.ndarray,
-):
+) -> Tuple[np.ndarray, np.ndarray, np.ndarray]:
+    """
+    Convert the causal, acausal, and predictive distributions to state probabilities.
+
+    Parameters
+    ----------
+    causal_posterior : np.ndarray, shape (n_time, n_state_bins)
+        The causal posterior distribution.
+    acausal_posterior : np.ndarray, shape (n_time, n_states_bins)
+        The acausal posterior distribution.
+    predictive_distribution : np.ndarray, shape (n_time, n_state_bins)
+        The predictive distribution.
+    state_ind : np.ndarray, shape (n_time,)
+        The state indices.
+
+    Returns
+    -------
+    Tuple[np.ndarray, np.ndarray, np.ndarray]
+        A tuple containing the causal, acausal, and predictive state probabilities.
+        causal_state_probabilities : np.ndarray, shape (n_time, n_states)
+            The causal state probabilities.
+        acausal_state_probabilities : np.ndarray, shape (n_time, n_states)
+            The acausal state probabilities.
+        predictive_state_probabilities : np.ndarray, shape (n_time, n_states)
+            The predictive state probabilities.
+    """
     n_states = np.unique(state_ind).size
     n_time = causal_posterior.shape[0]
 
     causal_state_probabilities = np.zeros((n_time, n_states))
     acausal_state_probabilities = np.zeros((n_time, n_states))
     predictive_state_probabilities = np.zeros((n_time, n_states))
 
@@ -36,33 +63,28 @@
     )
 
 
 ## NOTE: copied from dynamax: https://github.com/probml/dynamax/ with modifications ##
 def get_trans_mat(transition_matrix, transition_fn, t):
     if transition_fn is not None:
         return transition_fn(t)
-    else:
-        if transition_matrix.ndim == 3:  # (T,K,K)
-            return transition_matrix[t]
-        else:
-            return transition_matrix
+    return transition_matrix[t] if transition_matrix.ndim == 3 else transition_matrix
 
 
-def _normalize(u, axis=0, eps=1e-15):
+def _normalize(u, axis=0):
     """Normalizes the values within the axis in a way that they sum up to 1.
 
     Args:
         u: Input array to normalize.
         axis: Axis over which to normalize.
-        eps: Minimum value threshold for numerical stability.
 
     Returns:
         Tuple of the normalized values, and the normalizing denominator.
     """
-    u = jnp.clip(u, a_min=eps, a_max=None)
+    u = jnp.clip(u, a_min=EPS, a_max=None)
     c = u.sum(axis=axis)
     return u / c, c
 
 
 # Helper functions for the two key filtering steps
 def _condition_on(probs, ll):
     """Condition on new emissions, given in the form of log likelihoods
@@ -73,21 +95,17 @@
         ll(k): log likelihood for state k
 
     Returns:
         probs(k): posterior for state k
     """
     ll_max = ll.max()
     ll_max = jnp.where(jnp.isfinite(ll_max), ll_max, 0.0)
-    new_probs, norm = _normalize(probs * jnp.exp(ll - ll_max))
-    log_norm = jnp.log(norm) + ll_max
-    return new_probs, log_norm
-
-
-def _predict(probs, A):
-    return A.T @ probs
+    probs, log_norm = _normalize(probs * jnp.exp(ll - ll_max))
+    log_norm += ll_max
+    return probs, log_norm
 
 
 @partial(jax.jit, static_argnames=["transition_fn"])
 def hmm_filter(
     initial_distribution,
     transition_matrix,
     log_likelihoods,
@@ -111,20 +129,19 @@
 
     """
     num_timesteps = log_likelihoods.shape[0]
 
     def _step(carry, t):
         log_normalizer, predicted_probs = carry
 
-        A = get_trans_mat(transition_matrix, transition_fn, t)
-        ll = log_likelihoods[t]
-
-        filtered_probs, log_norm = _condition_on(predicted_probs, ll)
+        filtered_probs, log_norm = _condition_on(predicted_probs, log_likelihoods[t])
         log_normalizer += log_norm
-        predicted_probs_next = _predict(filtered_probs, A)
+        predicted_probs_next = (
+            get_trans_mat(transition_matrix, transition_fn, t).T @ filtered_probs
+        )
 
         return (log_normalizer, predicted_probs_next), (filtered_probs, predicted_probs)
 
     carry = (0.0, initial_distribution)
     (log_normalizer, _), (filtered_probs, predicted_probs) = jax.lax.scan(
         _step, carry, jnp.arange(num_timesteps)
     )
@@ -172,39 +189,42 @@
 
     # Run the smoother backward in time
     def _step(carry, args):
         # Unpack the inputs
         smoothed_probs_next = carry
         t, filtered_probs, predicted_probs_next = args
 
-        A = get_trans_mat(transition_matrix, transition_fn, t)
-
         # Fold in the next state (Eq. 8.2 of Saarka, 2013)
         # If hard 0. in predicted_probs_next, set relative_probs_next as 0. to avoid NaN values
         relative_probs_next = jnp.where(
             jnp.isclose(predicted_probs_next, 0.0),
             0.0,
             smoothed_probs_next / predicted_probs_next,
         )
-        smoothed_probs = filtered_probs * (A @ relative_probs_next)
+        smoothed_probs = filtered_probs * (
+            get_trans_mat(transition_matrix, transition_fn, t) @ relative_probs_next
+        )
         smoothed_probs /= smoothed_probs.sum()
 
         return smoothed_probs, smoothed_probs
 
     # Run the HMM smoother
-    carry = filtered_probs[-1]
-    args = (
-        jnp.arange(num_timesteps - 2, -1, -1),
-        filtered_probs[:-1][::-1],
-        predicted_probs[1:][::-1],
+    _, smoothed_probs = jax.lax.scan(
+        f=_step,
+        init=filtered_probs[-1],
+        xs=(
+            jnp.arange(0, num_timesteps - 1),
+            filtered_probs[:-1],
+            predicted_probs[1:],
+        ),
+        reverse=True,
     )
-    _, rev_smoothed_probs = jax.lax.scan(_step, carry, args)
 
     # Reverse the arrays and return
-    smoothed_probs = jnp.row_stack([rev_smoothed_probs[::-1], filtered_probs[-1]])
+    smoothed_probs = jnp.vstack([smoothed_probs, filtered_probs[-1]])
 
     return (
         marginal_loglik,
         filtered_probs,
         predicted_probs,
         smoothed_probs,
     )
```

### Comparing `non_local_detector-0.5.8/src/non_local_detector/discrete_state_transitions.py` & `non_local_detector-0.5.9/src/non_local_detector/discrete_state_transitions.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/environment.py` & `non_local_detector-0.5.9/src/non_local_detector/environment.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/initial_conditions.py` & `non_local_detector-0.5.9/src/non_local_detector/initial_conditions.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/observation_models.py` & `non_local_detector-0.5.9/src/non_local_detector/observation_models.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/types.py` & `non_local_detector-0.5.9/src/non_local_detector/types.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/analysis/__init__.py` & `non_local_detector-0.5.9/src/non_local_detector/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/analysis/distance1D.py` & `non_local_detector-0.5.9/src/non_local_detector/analysis/distance1D.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/analysis/distance2D.py` & `non_local_detector-0.5.9/src/non_local_detector/analysis/distance2D.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/analysis/highest_posterior_density.py` & `non_local_detector-0.5.9/src/non_local_detector/analysis/highest_posterior_density.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/analysis/posterior.py` & `non_local_detector-0.5.9/src/non_local_detector/analysis/posterior.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/likelihoods/__init__.py` & `non_local_detector-0.5.9/src/non_local_detector/likelihoods/__init__.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/likelihoods/clusterless_kde.py` & `non_local_detector-0.5.9/src/non_local_detector/likelihoods/clusterless_kde.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/likelihoods/common.py` & `non_local_detector-0.5.9/src/non_local_detector/likelihoods/common.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/likelihoods/no_spike.py` & `non_local_detector-0.5.9/src/non_local_detector/likelihoods/no_spike.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/likelihoods/sorted_spikes_glm.py` & `non_local_detector-0.5.9/src/non_local_detector/likelihoods/sorted_spikes_glm.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/likelihoods/sorted_spikes_kde.py` & `non_local_detector-0.5.9/src/non_local_detector/likelihoods/sorted_spikes_kde.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/model_checking/clusterless.py` & `non_local_detector-0.5.9/src/non_local_detector/model_checking/clusterless.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/model_checking/sorted_spikes.py` & `non_local_detector-0.5.9/src/non_local_detector/model_checking/sorted_spikes.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/models/__init__.py` & `non_local_detector-0.5.9/src/non_local_detector/models/__init__.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/models/base.py` & `non_local_detector-0.5.9/src/non_local_detector/models/base.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/models/cont_frag_model.py` & `non_local_detector-0.5.9/src/non_local_detector/models/cont_frag_model.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/models/decoder.py` & `non_local_detector-0.5.9/src/non_local_detector/models/decoder.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/models/multienvironment_model.py` & `non_local_detector-0.5.9/src/non_local_detector/models/multienvironment_model.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/models/non_local_model.py` & `non_local_detector-0.5.9/src/non_local_detector/models/non_local_model.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/simulate/clusterless_simulation.py` & `non_local_detector-0.5.9/src/non_local_detector/simulate/clusterless_simulation.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/simulate/simulate.py` & `non_local_detector-0.5.9/src/non_local_detector/simulate/simulate.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/simulate/sorted_spikes_simulation.py` & `non_local_detector-0.5.9/src/non_local_detector/simulate/sorted_spikes_simulation.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/visualization/figurl_1D.py` & `non_local_detector-0.5.9/src/non_local_detector/visualization/figurl_1D.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/visualization/figurl_2D.py` & `non_local_detector-0.5.9/src/non_local_detector/visualization/figurl_2D.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/src/non_local_detector/visualization/static.py` & `non_local_detector-0.5.9/src/non_local_detector/visualization/static.py`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/.gitignore` & `non_local_detector-0.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/LICENSE` & `non_local_detector-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/README.md` & `non_local_detector-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/pyproject.toml` & `non_local_detector-0.5.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `non_local_detector-0.5.8/PKG-INFO` & `non_local_detector-0.5.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: non_local_detector
-Version: 0.5.8
+Version: 0.5.9
 Summary: A python package to decode non-local activity from neural data
 Project-URL: Homepage, https://github.com/LorenFrankLab/non_local_detector
 Project-URL: Bug Tracker, https://github.com/LorenFrankLab/non_local_detector/issues
 Author-email: Eric Denovellis <eric.denovellis@ucsf.edu>
 License: MIT License
         
         Copyright (c) 2023 Eric Denovellis
```

