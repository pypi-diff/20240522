# Comparing `tmp/nqrduck_spectrometer_limenqr-0.0.6.tar.gz` & `tmp/nqrduck_spectrometer_limenqr-0.0.7.tar.gz`

## Comparing `nqrduck_spectrometer_limenqr-0.0.6.tar` & `nqrduck_spectrometer_limenqr-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/CHANGELOG.md
--rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/src/nqrduck_spectrometer_limenqr/__init__.py
--rw-r--r--   0        0        0    30951 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/src/nqrduck_spectrometer_limenqr/controller.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/src/nqrduck_spectrometer_limenqr/limenqr.py
--rw-r--r--   0        0        0    12094 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/src/nqrduck_spectrometer_limenqr/model.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/src/nqrduck_spectrometer_limenqr/view.py
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/src/nqrduck_spectrometer_limenqr/resources/limenqr.ini
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/src/nqrduck_spectrometer_limenqr/resources/limenqr_widget.ui
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/LICENSE
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/README.md
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.7/CHANGELOG.md
+-rw-r--r--   0        0        0      908 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.7/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.7/src/nqrduck_spectrometer_limenqr/__init__.py
+-rw-r--r--   0        0        0    31095 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.7/src/nqrduck_spectrometer_limenqr/controller.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.7/src/nqrduck_spectrometer_limenqr/limenqr.py
+-rw-r--r--   0        0        0    12094 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.7/src/nqrduck_spectrometer_limenqr/model.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.7/src/nqrduck_spectrometer_limenqr/view.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.7/src/nqrduck_spectrometer_limenqr/resources/limenqr.ini
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.7/src/nqrduck_spectrometer_limenqr/resources/limenqr_widget.ui
+-rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.7/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.7/README.md
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 nqrduck_spectrometer_limenqr-0.0.7/PKG-INFO
```

### Comparing `nqrduck_spectrometer_limenqr-0.0.6/.github/workflows/python-publish.yml` & `nqrduck_spectrometer_limenqr-0.0.7/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer_limenqr-0.0.6/src/nqrduck_spectrometer_limenqr/controller.py` & `nqrduck_spectrometer_limenqr-0.0.7/src/nqrduck_spectrometer_limenqr/controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,14 +54,18 @@
             self.emit_measurement_error(
                 "Error with measurement data. Did you set an RX event?"
             )
             return -1
 
         measurement_data = self.process_measurement_results(lime)
 
+        if not measurement_data:
+            self.emit_measurement_error("Measurement failed. Unable to retrieve data.")
+            return -1
+
         # Resample the RX data to the dwell time settings
         dwell_time = self.module.model.get_setting_by_name(
             self.module.model.RX_DWELL_TIME
         ).value
         dwell_time = UnitConverter.to_float(dwell_time) * 1e6
         logger.debug("Dwell time: %s", dwell_time)
         logger.debug(f"Last tdx value: {measurement_data.tdx[-1]}")
```

### Comparing `nqrduck_spectrometer_limenqr-0.0.6/src/nqrduck_spectrometer_limenqr/model.py` & `nqrduck_spectrometer_limenqr-0.0.7/src/nqrduck_spectrometer_limenqr/model.py`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer_limenqr-0.0.6/src/nqrduck_spectrometer_limenqr/resources/limenqr_widget.ui` & `nqrduck_spectrometer_limenqr-0.0.7/src/nqrduck_spectrometer_limenqr/resources/limenqr_widget.ui`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer_limenqr-0.0.6/LICENSE` & `nqrduck_spectrometer_limenqr-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer_limenqr-0.0.6/README.md` & `nqrduck_spectrometer_limenqr-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `nqrduck_spectrometer_limenqr-0.0.6/pyproject.toml` & `nqrduck_spectrometer_limenqr-0.0.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [project]
 name = "nqrduck-spectrometer-limenqr"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="jupfi", email="support@nqrduck.cool" },
 ]
 
 description = "A submodule for the nqrduck-spectrometer module which implements the functionality for the LimeNQR spectrometer."
 readme = "README.md"
 license = { file="LICENSE" }
```

### Comparing `nqrduck_spectrometer_limenqr-0.0.6/PKG-INFO` & `nqrduck_spectrometer_limenqr-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nqrduck-spectrometer-limenqr
-Version: 0.0.6
+Version: 0.0.7
 Summary: A submodule for the nqrduck-spectrometer module which implements the functionality for the LimeNQR spectrometer.
 Project-URL: Homepage, https://nqrduck.cool
 Project-URL: Bug Tracker, https://github.com/nqrduck/nqrduck-spectrometer-limenqr/issues
 Project-URL: Source Code, https://github.com/nqrduck/nqrduck-spectrometer-limenqr
 Author-email: jupfi <support@nqrduck.cool>
 License: MIT License
```

