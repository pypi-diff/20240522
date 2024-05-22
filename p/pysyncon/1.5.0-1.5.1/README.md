# Comparing `tmp/pysyncon-1.5.0.tar.gz` & `tmp/pysyncon-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysyncon-1.5.0.tar", last modified: Sat May 11 20:36:01 2024, max compression
+gzip compressed data, was "pysyncon-1.5.1.tar", last modified: Wed May 22 20:31:48 2024, max compression
```

## Comparing `pysyncon-1.5.0.tar` & `pysyncon-1.5.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 20:36:01.797161 pysyncon-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-11 20:35:51.000000 pysyncon-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-11 20:36:01.793161 pysyncon-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-11 20:35:51.000000 pysyncon-1.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 20:36:01.793161 pysyncon-1.5.0/pysyncon/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pysyncon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pysyncon/augsynth.py
--rw-r--r--   0 runner    (1001) docker     (127)    19121 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pysyncon/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    13423 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pysyncon/dataprep.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pysyncon/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9427 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pysyncon/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pysyncon/penalized.py
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pysyncon/robust.py
--rw-r--r--   0 runner    (1001) docker     (127)    20219 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pysyncon/synth.py
--rw-r--r--   0 runner    (1001) docker     (127)    12473 2024-05-11 20:35:51.000000 pysyncon-1.5.0/pysyncon/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 20:36:01.793161 pysyncon-1.5.0/pysyncon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-11 20:36:01.000000 pysyncon-1.5.0/pysyncon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-11 20:36:01.000000 pysyncon-1.5.0/pysyncon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 20:36:01.000000 pysyncon-1.5.0/pysyncon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-11 20:36:01.000000 pysyncon-1.5.0/pysyncon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-11 20:36:01.000000 pysyncon-1.5.0/pysyncon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-11 20:36:01.797161 pysyncon-1.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 20:36:01.793161 pysyncon-1.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_augsynth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_augsynth_basque.py
--rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_conformal_interence.py
--rw-r--r--   0 runner    (1001) docker     (127)    19419 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_dataprep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_linear_factor_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_penalized.py
--rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_penalized_basque.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_robust.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_robust_basque.py
--rw-r--r--   0 runner    (1001) docker     (127)    13205 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_synth.py
--rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_synth_basque.py
--rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_synth_germany.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_synth_texas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-05-11 20:35:51.000000 pysyncon-1.5.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:31:48.446686 pysyncon-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 20:31:44.000000 pysyncon-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-22 20:31:48.446686 pysyncon-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-05-22 20:31:44.000000 pysyncon-1.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-22 20:31:44.000000 pysyncon-1.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:31:48.442686 pysyncon-1.5.1/pysyncon/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-22 20:31:44.000000 pysyncon-1.5.1/pysyncon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4909 2024-05-22 20:31:44.000000 pysyncon-1.5.1/pysyncon/augsynth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19121 2024-05-22 20:31:44.000000 pysyncon-1.5.1/pysyncon/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14243 2024-05-22 20:31:44.000000 pysyncon-1.5.1/pysyncon/dataprep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-05-22 20:31:44.000000 pysyncon-1.5.1/pysyncon/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9427 2024-05-22 20:31:44.000000 pysyncon-1.5.1/pysyncon/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-05-22 20:31:44.000000 pysyncon-1.5.1/pysyncon/penalized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-22 20:31:44.000000 pysyncon-1.5.1/pysyncon/robust.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20219 2024-05-22 20:31:44.000000 pysyncon-1.5.1/pysyncon/synth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12389 2024-05-22 20:31:44.000000 pysyncon-1.5.1/pysyncon/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:31:48.446686 pysyncon-1.5.1/pysyncon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-22 20:31:48.000000 pysyncon-1.5.1/pysyncon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-22 20:31:48.000000 pysyncon-1.5.1/pysyncon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:31:48.000000 pysyncon-1.5.1/pysyncon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-22 20:31:48.000000 pysyncon-1.5.1/pysyncon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 20:31:48.000000 pysyncon-1.5.1/pysyncon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-22 20:31:48.446686 pysyncon-1.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:31:48.446686 pysyncon-1.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-22 20:31:44.000000 pysyncon-1.5.1/tests/test_augsynth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-05-22 20:31:44.000000 pysyncon-1.5.1/tests/test_augsynth_basque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-05-22 20:31:44.000000 pysyncon-1.5.1/tests/test_conformal_interence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22345 2024-05-22 20:31:44.000000 pysyncon-1.5.1/tests/test_dataprep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-22 20:31:44.000000 pysyncon-1.5.1/tests/test_linear_factor_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-05-22 20:31:44.000000 pysyncon-1.5.1/tests/test_penalized.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2024-05-22 20:31:44.000000 pysyncon-1.5.1/tests/test_penalized_basque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-05-22 20:31:44.000000 pysyncon-1.5.1/tests/test_robust.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-22 20:31:44.000000 pysyncon-1.5.1/tests/test_robust_basque.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13205 2024-05-22 20:31:44.000000 pysyncon-1.5.1/tests/test_synth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8897 2024-05-22 20:31:44.000000 pysyncon-1.5.1/tests/test_synth_basque.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6667 2024-05-22 20:31:44.000000 pysyncon-1.5.1/tests/test_synth_germany.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5370 2024-05-22 20:31:44.000000 pysyncon-1.5.1/tests/test_synth_texas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7127 2024-05-22 20:31:44.000000 pysyncon-1.5.1/tests/test_utils.py
```

### Comparing `pysyncon-1.5.0/LICENSE` & `pysyncon-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/PKG-INFO` & `pysyncon-1.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysyncon
-Version: 1.5.0
+Version: 1.5.1
 Home-page: https://github.com/sdfordham/pysyncon/
 Author: Stiofán Fordham
 License: MIT License
 Keywords: Synth,augsynth,synthetic-control-method,causal-inference
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pysyncon-1.5.0/README.md` & `pysyncon-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/pysyncon/augsynth.py` & `pysyncon-1.5.1/pysyncon/augsynth.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/pysyncon/base.py` & `pysyncon-1.5.1/pysyncon/base.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/pysyncon/dataprep.py` & `pysyncon-1.5.1/pysyncon/dataprep.py`

 * *Files 6% similar despite different names*

```diff
@@ -127,14 +127,19 @@
             raise ValueError(f"unit_variable {unit_variable} not in foo columns.")
         self.unit_variable = unit_variable
 
         if time_variable not in foo.columns:
             raise ValueError(f"time_variable {time_variable} not in foo columns.")
         self.time_variable = time_variable
 
+        if foo[[unit_variable, time_variable]].duplicated().any():
+            raise ValueError(
+                "Multiple rows found in `foo` for same [unit, time] pairs."
+            )
+
         if isinstance(treatment_identifier, (list, tuple)):
             for treated in treatment_identifier:
                 # This throws FutureWarning (see https://stackoverflow.com/a/46721064/11594901)
                 if treated not in foo[unit_variable].values:
                     raise ValueError(
                         f'treatment_identifier {treated} not found in foo["{unit_variable}"].'
                     )
@@ -165,28 +170,39 @@
                     raise ValueError("treatment_identifier in controls_identifier.")
             if control not in foo[unit_variable].values:
                 raise ValueError(
                     f'controls_identifier {control} not found in foo["{unit_variable}"].'
                 )
         self.controls_identifier = controls_identifier
 
+        if self.foo[self.foo[self.time_variable].isin(time_predictors_prior)].empty:
+            raise ValueError(
+                f"foo has no rows in the time range `time_predictors_prior`."
+            )
         self.time_predictors_prior = time_predictors_prior
+
+        if self.foo[self.foo[self.time_variable].isin(time_optimize_ssr)].empty:
+            raise ValueError(f"foo has no rows in the time range `time_optimize_ssr`.")
         self.time_optimize_ssr = time_optimize_ssr
 
         if special_predictors:
             for el in special_predictors:
                 if not isinstance(el, tuple) or len(el) != 3:
                     raise ValueError(
                         "Elements of special_predictors should be tuples of length 3."
                     )
-                predictor, _, op = el
+                predictor, time_range, op = el
                 if predictor not in foo.columns:
                     raise ValueError(
                         f"{predictor} in special_predictors not in foo columns."
                     )
+                if self.foo[self.foo[self.time_variable].isin(time_range)].empty:
+                    raise ValueError(
+                        f"foo has no rows in the time range {time_range} for `special_predictor` {el}."
+                    )
                 if op not in AGG_OP:
                     agg_op_str = ", ".join([f'"{o}"' for o in AGG_OP])
                     raise ValueError(
                         f"{op} in special_predictors must be one of {agg_op_str}."
                     )
         self.special_predictors = special_predictors
```

### Comparing `pysyncon-1.5.0/pysyncon/generator.py` & `pysyncon-1.5.1/pysyncon/generator.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/pysyncon/inference.py` & `pysyncon-1.5.1/pysyncon/inference.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/pysyncon/penalized.py` & `pysyncon-1.5.1/pysyncon/penalized.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/pysyncon/robust.py` & `pysyncon-1.5.1/pysyncon/robust.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/pysyncon/synth.py` & `pysyncon-1.5.1/pysyncon/synth.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/pysyncon/utils.py` & `pysyncon-1.5.1/pysyncon/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,18 +242,17 @@
             time-series of the gap between the treated unit and the synthetic
             control.
 
         :meta private:
         """
         scm.fit(dataprep=dataprep, **scm_options)
 
-        min_ = int(min(dataprep.foo[dataprep.time_variable]))
-        max_ = int(max(dataprep.foo[dataprep.time_variable]))
-
-        Z0, Z1 = dataprep.make_outcome_mats(time_period=range(min_, max_))
+        Z0, Z1 = dataprep.make_outcome_mats(
+            time_period=dataprep.foo[dataprep.time_variable]
+        )
         synthetic = scm._synthetic(Z0=Z0)
         gaps = scm._gaps(Z0=Z0, Z1=Z1)
         return synthetic.rename(dataprep.treatment_identifier), gaps.rename(
             dataprep.treatment_identifier
         )
 
     def gaps_plot(
```

### Comparing `pysyncon-1.5.0/pysyncon.egg-info/PKG-INFO` & `pysyncon-1.5.1/pysyncon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysyncon
-Version: 1.5.0
+Version: 1.5.1
 Home-page: https://github.com/sdfordham/pysyncon/
 Author: Stiofán Fordham
 License: MIT License
 Keywords: Synth,augsynth,synthetic-control-method,causal-inference
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pysyncon-1.5.0/pysyncon.egg-info/SOURCES.txt` & `pysyncon-1.5.1/pysyncon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/setup.cfg` & `pysyncon-1.5.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pysyncon
-version = 1.5.0
+version = 1.5.1
 author = Stiofán Fordham
 url = https://github.com/sdfordham/pysyncon/
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = Synth,augsynth,synthetic-control-method,causal-inference,
 license = MIT License
```

### Comparing `pysyncon-1.5.0/tests/test_augsynth.py` & `pysyncon-1.5.1/tests/test_augsynth.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/tests/test_augsynth_basque.py` & `pysyncon-1.5.1/tests/test_augsynth_basque.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/tests/test_conformal_interence.py` & `pysyncon-1.5.1/tests/test_conformal_interence.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/tests/test_dataprep.py` & `pysyncon-1.5.1/tests/test_dataprep.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,35 @@
             "time_predictors_prior": self.time_predictors_prior,
             "time_optimize_ssr": self.time_optimize_ssr,
             "special_predictors": self.special_predictors,
         }
 
         self.assertRaises(ValueError, Dataprep, time_variable="badval", **kwargs)
 
+    def test_init_multiple_rows(self):
+        kwargs = {
+            "predictors": self.predictors,
+            "predictors_op": self.predictors_op,
+            "dependent": self.dependent,
+            "unit_variable": self.unit_variable,
+            "time_variable": self.time_variable,
+            "treatment_identifier": self.treatment_identifier,
+            "controls_identifier": self.controls_identifier,
+            "time_predictors_prior": self.time_predictors_prior,
+            "time_optimize_ssr": self.time_optimize_ssr,
+            "special_predictors": self.special_predictors,
+        }
+
+        self.assertRaises(
+            ValueError,
+            Dataprep,
+            foo=pd.concat([self.foo, self.foo.iloc[0:1]], axis=0),
+            **kwargs,
+        )
+
     def test_init_arg_treatment_identifier(self):
         kwargs = {
             "foo": self.foo,
             "predictors": self.predictors,
             "predictors_op": self.predictors_op,
             "dependent": self.dependent,
             "unit_variable": self.unit_variable,
@@ -172,14 +193,69 @@
         }
 
         self.assertRaises(ValueError, Dataprep, treatment_identifier="badval", **kwargs)
         self.assertRaises(
             ValueError, Dataprep, treatment_identifier=["badval"], **kwargs
         )
 
+    def test_bad_time_periods_time_predictors_prior(self):
+        kwargs = {
+            "foo": self.foo,
+            "predictors": self.predictors,
+            "predictors_op": self.predictors_op,
+            "dependent": self.dependent,
+            "unit_variable": self.unit_variable,
+            "time_variable": self.time_variable,
+            "controls_identifier": self.controls_identifier,
+            "time_optimize_ssr": self.time_optimize_ssr,
+            "treatment_identifier": self.treatment_identifier,
+            "special_predictors": self.special_predictors,
+        }
+
+        self.assertRaises(
+            ValueError, Dataprep, time_predictors_prior=["2", "3"], **kwargs
+        )
+
+    def test_bad_time_periods_time_optimize_ssr(self):
+        kwargs = {
+            "foo": self.foo,
+            "predictors": self.predictors,
+            "predictors_op": self.predictors_op,
+            "dependent": self.dependent,
+            "unit_variable": self.unit_variable,
+            "time_variable": self.time_variable,
+            "controls_identifier": self.controls_identifier,
+            "time_predictors_prior": self.time_predictors_prior,
+            "treatment_identifier": self.treatment_identifier,
+            "special_predictors": self.special_predictors,
+        }
+
+        self.assertRaises(ValueError, Dataprep, time_optimize_ssr=["2", "3"], **kwargs)
+
+    def test_bad_time_periods_special_predictors(self):
+        kwargs = {
+            "foo": self.foo,
+            "predictors": self.predictors,
+            "predictors_op": self.predictors_op,
+            "dependent": self.dependent,
+            "unit_variable": self.unit_variable,
+            "time_variable": self.time_variable,
+            "controls_identifier": self.controls_identifier,
+            "time_optimize_ssr": self.time_optimize_ssr,
+            "time_predictors_prior": self.time_predictors_prior,
+            "treatment_identifier": self.treatment_identifier,
+        }
+
+        self.assertRaises(
+            ValueError,
+            Dataprep,
+            special_predictors=[("predictor1", ["2"], "mean")],
+            **kwargs,
+        )
+
     def test_init_arg_controls_identifier(self):
         kwargs = {
             "foo": self.foo,
             "predictors": self.predictors,
             "predictors_op": self.predictors_op,
             "dependent": self.dependent,
             "unit_variable": self.unit_variable,
```

### Comparing `pysyncon-1.5.0/tests/test_linear_factor_model.py` & `pysyncon-1.5.1/tests/test_linear_factor_model.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/tests/test_penalized.py` & `pysyncon-1.5.1/tests/test_penalized.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/tests/test_penalized_basque.py` & `pysyncon-1.5.1/tests/test_penalized_basque.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/tests/test_robust.py` & `pysyncon-1.5.1/tests/test_robust.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/tests/test_robust_basque.py` & `pysyncon-1.5.1/tests/test_robust_basque.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/tests/test_synth.py` & `pysyncon-1.5.1/tests/test_synth.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/tests/test_synth_basque.py` & `pysyncon-1.5.1/tests/test_synth_basque.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/tests/test_synth_germany.py` & `pysyncon-1.5.1/tests/test_synth_germany.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/tests/test_synth_texas.py` & `pysyncon-1.5.1/tests/test_synth_texas.py`

 * *Files identical despite different names*

### Comparing `pysyncon-1.5.0/tests/test_utils.py` & `pysyncon-1.5.1/tests/test_utils.py`

 * *Files identical despite different names*

