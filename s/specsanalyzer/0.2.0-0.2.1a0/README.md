# Comparing `tmp/specsanalyzer-0.2.0.tar.gz` & `tmp/specsanalyzer-0.2.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "specsanalyzer-0.2.0.tar", max compression
+gzip compressed data, was "specsanalyzer-0.2.1a0.tar", max compression
```

## Comparing `specsanalyzer-0.2.0.tar` & `specsanalyzer-0.2.1a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0     1067 2024-04-19 20:34:39.421211 specsanalyzer-0.2.0/LICENSE
--rw-r--r--   0        0        0     4279 2024-04-19 20:34:39.421211 specsanalyzer-0.2.0/README.md
--rw-r--r--   0        0        0     2629 2024-04-19 20:34:51.301210 specsanalyzer-0.2.0/pyproject.toml
--rwxr-xr-x   0        0        0      145 2024-04-19 20:34:39.421211 specsanalyzer-0.2.0/specsanalyzer/__init__.py
--rw-r--r--   0        0        0      695 2024-04-19 20:34:39.421211 specsanalyzer-0.2.0/specsanalyzer/config/default.yaml
--rwxr-xr-x   0        0        0      411 2024-04-19 20:34:39.421211 specsanalyzer-0.2.0/specsanalyzer/config/phoibos150.calib2d
--rwxr-xr-x   0        0        0     8973 2024-04-19 20:34:39.421211 specsanalyzer-0.2.0/specsanalyzer/config.py
--rwxr-xr-x   0        0        0    19345 2024-04-19 20:34:39.421211 specsanalyzer-0.2.0/specsanalyzer/convert.py
--rwxr-xr-x   0        0        0    30409 2024-04-19 20:34:39.421211 specsanalyzer-0.2.0/specsanalyzer/core.py
--rwxr-xr-x   0        0        0     4250 2024-04-19 20:34:39.425211 specsanalyzer-0.2.0/specsanalyzer/img_tools.py
--rwxr-xr-x   0        0        0    18805 2024-04-19 20:34:39.425211 specsanalyzer-0.2.0/specsanalyzer/io.py
--rwxr-xr-x   0        0        0      133 2024-04-19 20:34:39.425211 specsanalyzer-0.2.0/specsscan/__init__.py
--rwxr-xr-x   0        0        0    15200 2024-04-19 20:34:39.425211 specsanalyzer-0.2.0/specsscan/config/NXmpes_arpes_config.json
--rw-r--r--   0        0        0      556 2024-04-19 20:34:39.425211 specsanalyzer-0.2.0/specsscan/config/default.yaml
--rw-r--r--   0        0        0     3347 2024-04-19 20:34:39.425211 specsanalyzer-0.2.0/specsscan/config/example_config_FHI.yaml
--rwxr-xr-x   0        0        0    23671 2024-04-19 20:34:39.425211 specsanalyzer-0.2.0/specsscan/core.py
--rw-r--r--   0        0        0    20015 2024-04-19 20:34:39.425211 specsanalyzer-0.2.0/specsscan/helpers.py
--rw-r--r--   0        0        0     5619 1970-01-01 00:00:00.000000 specsanalyzer-0.2.0/setup.py
--rw-r--r--   0        0        0     5769 1970-01-01 00:00:00.000000 specsanalyzer-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0     1067 2024-05-22 19:25:26.146681 specsanalyzer-0.2.1a0/LICENSE
+-rw-r--r--   0        0        0     4279 2024-05-22 19:25:26.146681 specsanalyzer-0.2.1a0/README.md
+-rw-r--r--   0        0        0     3056 2024-05-22 19:25:45.458925 specsanalyzer-0.2.1a0/pyproject.toml
+-rwxr-xr-x   0        0        0      145 2024-05-22 19:25:26.150681 specsanalyzer-0.2.1a0/specsanalyzer/__init__.py
+-rw-r--r--   0        0        0      695 2024-05-22 19:25:26.150681 specsanalyzer-0.2.1a0/specsanalyzer/config/default.yaml
+-rwxr-xr-x   0        0        0      411 2024-05-22 19:25:26.150681 specsanalyzer-0.2.1a0/specsanalyzer/config/phoibos150.calib2d
+-rwxr-xr-x   0        0        0     8973 2024-05-22 19:25:26.150681 specsanalyzer-0.2.1a0/specsanalyzer/config.py
+-rwxr-xr-x   0        0        0    19345 2024-05-22 19:25:26.150681 specsanalyzer-0.2.1a0/specsanalyzer/convert.py
+-rwxr-xr-x   0        0        0    30409 2024-05-22 19:25:26.150681 specsanalyzer-0.2.1a0/specsanalyzer/core.py
+-rwxr-xr-x   0        0        0     4250 2024-05-22 19:25:26.150681 specsanalyzer-0.2.1a0/specsanalyzer/img_tools.py
+-rwxr-xr-x   0        0        0    18805 2024-05-22 19:25:26.150681 specsanalyzer-0.2.1a0/specsanalyzer/io.py
+-rwxr-xr-x   0        0        0      133 2024-05-22 19:25:26.150681 specsanalyzer-0.2.1a0/specsscan/__init__.py
+-rwxr-xr-x   0        0        0    15244 2024-05-22 19:25:26.150681 specsanalyzer-0.2.1a0/specsscan/config/NXmpes_arpes_config.json
+-rw-r--r--   0        0        0      556 2024-05-22 19:25:26.150681 specsanalyzer-0.2.1a0/specsscan/config/default.yaml
+-rw-r--r--   0        0        0     3334 2024-05-22 19:25:26.150681 specsanalyzer-0.2.1a0/specsscan/config/example_config_FHI.yaml
+-rwxr-xr-x   0        0        0    23681 2024-05-22 19:25:26.154682 specsanalyzer-0.2.1a0/specsscan/core.py
+-rw-r--r--   0        0        0    20040 2024-05-22 19:25:26.154682 specsanalyzer-0.2.1a0/specsscan/helpers.py
+-rw-r--r--   0        0        0     5659 1970-01-01 00:00:00.000000 specsanalyzer-0.2.1a0/setup.py
+-rw-r--r--   0        0        0     5837 1970-01-01 00:00:00.000000 specsanalyzer-0.2.1a0/PKG-INFO
```

### Comparing `specsanalyzer-0.2.0/LICENSE` & `specsanalyzer-0.2.1a0/LICENSE`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.2.0/README.md` & `specsanalyzer-0.2.1a0/README.md`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.2.0/pyproject.toml` & `specsanalyzer-0.2.1a0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "specsanalyzer"
 packages = [
     {include = "specsanalyzer"},
     {include = "specsscan"},
 ]
-version = "0.2.0"
+version = "0.2.1a0"
 description = "Python package for loading and converting SPECS Phoibos analyzer data."
 authors = [
     "Laurenz Rettig <rettig@fhi-berlin.mpg.de>",
     "Michele Puppin <michele.puppin@epfl.ch>",
     "Abeer Arora <arora@fhi-berlin.mpg.de>",
 ]
 readme = "README.md"
@@ -23,47 +23,59 @@
 imutils = ">=0.5.4"
 ipympl = ">=0.9.1"
 ipywidgets = ">=7.7.1"
 matplotlib = ">=3.5.1"
 numpy = ">=1.21.6"
 opencv-python = ">=4.8.1.78"
 pynxtools-mpes = ">=0.0.1"
+pynxtools = ">=0.3.1"
 python-dateutil = ">=2.8.2"
 pyyaml = ">=6.0"
 xarray = ">=0.20.2"
 tifffile = ">=2022.5.4"
+tqdm = ">=4.62.3"
 scipy = ">=1.8.0"
 jupyter = {version = ">=1.0.0", extras = ["notebook"], optional = true}
 ipykernel = {version = ">=6.9.1", extras = ["notebook"], optional = true}
 jupyterlab-h5web = {version = ">=7.0.0", extras = ["notebook"], optional = true}
 
 [tool.poetry.extras]
 notebook = ["jupyter", "ipykernel", "jupyterlab-h5web"]
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.0.1"
 pytest-cov = ">=3.0.0"
 pytest-xdist = ">=2.5.0"
 pytest-clarity = ">=1.0.1"
 ruff = ">=0.1.7, <0.3.0"
-mypy = ">=1.6.0"
+mypy = ">=1.6.0, <1.10.0"
 types-pyyaml = ">=6.0.12.12"
 types-requests = ">=2.31.0.9"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = ">=7.1.2"
 sphinx-rtd-theme = ">=1.0.0"
 tomlkit = ">=0.12.0"
 sphinx-autodoc-typehints = ">=1.17.0"
 nbsphinx = ">=0.9.3"
 myst-parser = ">=2.0.0"
 
+[[tool.poetry.source]]
+# the source is needed to workaround the poetry install error
+# "Package docutils (0.21.post1) not found."
+# details:
+# https://github.com/python-poetry/poetry/issues/9293#issuecomment-2048205226
+# - the root cause is at pypi / docutils, so the workaround might not
+#   be needed when they fix it.
+name = "pypi-public"
+url = "https://pypi.org/simple/"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.report]
 omit = [
     "config.py",
```

### Comparing `specsanalyzer-0.2.0/specsanalyzer/config/default.yaml` & `specsanalyzer-0.2.1a0/specsanalyzer/config/default.yaml`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.2.0/specsanalyzer/config.py` & `specsanalyzer-0.2.1a0/specsanalyzer/config.py`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.2.0/specsanalyzer/convert.py` & `specsanalyzer-0.2.1a0/specsanalyzer/convert.py`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.2.0/specsanalyzer/core.py` & `specsanalyzer-0.2.1a0/specsanalyzer/core.py`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.2.0/specsanalyzer/img_tools.py` & `specsanalyzer-0.2.1a0/specsanalyzer/img_tools.py`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.2.0/specsanalyzer/io.py` & `specsanalyzer-0.2.1a0/specsanalyzer/io.py`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.2.0/specsscan/config/NXmpes_arpes_config.json` & `specsanalyzer-0.2.1a0/specsscan/config/NXmpes_arpes_config.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6650579150579151%*

 * *Differences: {"'/ENTRY[entry]/INSTRUMENT[instrument]/ELECTRONANALYSER[electronanalyser]'": "{'TRANSFORMATIONS[transformations]': "*

 * *                                                                              "OrderedDict([('AXISNAME[trans_z]/@depends_on', "*

 * *                                                                              "'analyzer_elevation'), "*

 * *                                                                              "('AXISNAME[trans_z]', "*

 * *                                                            […]*

```diff
@@ -26,41 +26,15 @@
             "measurement": "pressure",
             "name": "sample_chamber_pressure",
             "value": "@attrs:metadata/scan_info/trARPES:XGS600:PressureAC:P_RD",
             "value/@units": "mbar"
         }
     },
     "/ENTRY[entry]/INSTRUMENT[instrument]/ELECTRONANALYSER[electronanalyser]": {
-        "angular_resolution": {
-            "physical_quantity": "angle",
-            "resolution": "@attrs:metadata/instrument/electronanalyser/angular_resolution",
-            "resolution/@units": "deg",
-            "type": "derived"
-        },
-        "depends_on": "/entry/instrument/electronanalyser/transformations/trans_z",
-        "description": "SPECS Phoibos 150 Hemispherical Energy Analyzer",
-        "device_information": {
-            "model": "Phoibos 150 CCD Hemispherical Analyzer",
-            "vendor": "SPECS GmbH"
-        },
-        "energy_resolution": {
-            "physical_quantity": "energy",
-            "resolution": "@attrs:metadata/instrument/electronanalyser/energy_resolution",
-            "resolution/@units": "meV",
-            "type": "derived"
-        },
-        "fast_axes": "@attrs:metadata/scan_info/fast_axes",
-        "slow_axes": "@attrs:metadata/scan_info/slow_axes",
-        "spatial_resolution": {
-            "physical_quantity": "length",
-            "resolution": "@attrs:metadata/instrument/electronanalyser/spatial_resolution",
-            "resolution/@units": "\u00b5m",
-            "type": "estimated"
-        },
-        "transformations": {
+        "TRANSFORMATIONS[transformations]": {
             "AXISNAME[rot_y]": 140.0,
             "AXISNAME[rot_y]/@depends_on": ".",
             "AXISNAME[rot_y]/@transformation_type": "rotation",
             "AXISNAME[rot_y]/@units": "degrees",
             "AXISNAME[rot_y]/@vector": [
                 0,
                 1,
@@ -99,14 +73,40 @@
             "analyzer_rotation/@units": "degrees",
             "analyzer_rotation/@vector": [
                 0,
                 0,
                 1
             ]
         },
+        "angular_resolution": {
+            "physical_quantity": "angle",
+            "resolution": "@attrs:metadata/instrument/electronanalyser/angular_resolution",
+            "resolution/@units": "deg",
+            "type": "derived"
+        },
+        "depends_on": "/entry/instrument/electronanalyser/transformations/trans_z",
+        "description": "SPECS Phoibos 150 Hemispherical Energy Analyzer",
+        "device_information": {
+            "model": "Phoibos 150 CCD Hemispherical Analyzer",
+            "vendor": "SPECS GmbH"
+        },
+        "energy_resolution": {
+            "physical_quantity": "energy",
+            "resolution": "@attrs:metadata/instrument/electronanalyser/energy_resolution",
+            "resolution/@units": "meV",
+            "type": "derived"
+        },
+        "fast_axes": "@attrs:metadata/scan_info/fast_axes",
+        "slow_axes": "@attrs:metadata/scan_info/slow_axes",
+        "spatial_resolution": {
+            "physical_quantity": "length",
+            "resolution": "@attrs:metadata/instrument/electronanalyser/spatial_resolution",
+            "resolution/@units": "\u00b5m",
+            "type": "estimated"
+        },
         "work_function": 4.55,
         "work_function/@units": "eV"
     },
     "/ENTRY[entry]/INSTRUMENT[instrument]/ELECTRONANALYSER[electronanalyser]/COLLECTIONCOLUMN[collectioncolumn]": {
         "lens_mode": "@attrs:metadata/scan_info/LensMode",
         "projection": "@attrs:metadata/scan_info/projection",
         "scheme": "@attrs:metadata/scan_info/scheme",
@@ -124,27 +124,27 @@
         "detector_voltage/@units": "V",
         "sensor_pixels": [
             256,
             320
         ]
     },
     "/ENTRY[entry]/INSTRUMENT[instrument]/ELECTRONANALYSER[electronanalyser]/ENERGYDISPERSION[energydispersion]": {
+        "center_energy": "@attrs:metadata/scan_info/KineticEnergy",
+        "center_energy/@units": "eV",
         "diameter": 300.0,
         "diameter/@units": "mm",
         "energy_scan_mode": "@attrs:metadata/scan_info/energy_scan_mode",
         "entrance_slit": {
             "shape": "curved",
             "size": 1.0,
             "size/@units": "mm"
         },
         "exit_slit": {
             "shape": "grid"
         },
-        "kinetic_energy": "@attrs:metadata/scan_info/KineticEnergy",
-        "kinetic_energy/@units": "eV",
         "pass_energy": "@attrs:metadata/scan_info/PassEnergy",
         "pass_energy/@units": "eV",
         "scheme": "hemispherical"
     },
     "/ENTRY[entry]/INSTRUMENT[instrument]/MANIPULATOR[manipulator]": {
         "TRANSFORMATIONS[transformations]": {
             "AXISNAME[rot_x]": -90.0,
@@ -191,30 +191,30 @@
         "temperature_sensor": {
             "measurement": "temperature",
             "name": "sample_temperature",
             "value": "@attrs:metadata/scan_info/trARPES:Carving:TEMP_RBV",
             "value/@units": "K"
         }
     },
-    "/ENTRY[entry]/INSTRUMENT[instrument]/beam_TYPE[beam_probe]": {
+    "/ENTRY[entry]/INSTRUMENT[instrument]/beamTYPE[beam_probe]": {
         "associated_source": "/entry/instrument/source_probe",
         "distance": 0.0,
         "distance/@units": "mm",
         "extent": "@attrs:metadata/instrument/beam/probe/extent",
         "extent/@units": "\u00b5m",
         "incident_energy": "@attrs:metadata/instrument/beam/probe/incident_energy",
         "incident_energy/@units": "eV",
         "incident_energy_spread": "@attrs:metadata/instrument/beam/probe/incident_energy_spread",
         "incident_energy_spread/@units": "eV",
         "incident_polarization": "@attrs:metadata/instrument/beam/probe/incident_polarization",
         "incident_polarization/@units": "V^2/mm^2",
         "pulse_duration": "@attrs:metadata/instrument/beam/probe/pulse_duration",
         "pulse_duration/@units": "fs"
     },
-    "/ENTRY[entry]/INSTRUMENT[instrument]/beam_TYPE[beam_pump]": {
+    "/ENTRY[entry]/INSTRUMENT[instrument]/beamTYPE[beam_pump]": {
         "associated_source": "/entry/instrument/source_pump",
         "average_power": "@attrs:metadata/instrument/beam/pump/average_power",
         "average_power/@units": "mW",
         "distance": 0.0,
         "distance/@units": "mm",
         "extent": "@attrs:metadata/instrument/beam/pump/extent",
         "extent/@units": "\u00b5m",
@@ -229,59 +229,41 @@
         "incident_wavelength": "@attrs:metadata/instrument/beam/pump/incident_wavelength",
         "incident_wavelength/@units": "nm",
         "pulse_duration": "@attrs:metadata/instrument/beam/pump/pulse_duration",
         "pulse_duration/@units": "fs",
         "pulse_energy": "@attrs:metadata/instrument/beam/pump/pulse_energy",
         "pulse_energy/@units": "\u00b5J"
     },
-    "/ENTRY[entry]/INSTRUMENT[instrument]/source_TYPE[source_probe]": {
+    "/ENTRY[entry]/INSTRUMENT[instrument]/sourceTYPE[source_probe]": {
         "associated_beam": "/entry/instrument/beam_probe",
         "frequency": "@attrs:metadata/instrument/beam/probe/frequency",
         "frequency/@units": "kHz",
         "mode": "Single Bunch",
         "name": "HHG @ TR-ARPES @ FHI",
         "probe": "photon",
         "type": "HHG laser"
     },
-    "/ENTRY[entry]/INSTRUMENT[instrument]/source_TYPE[source_pump]": {
+    "/ENTRY[entry]/INSTRUMENT[instrument]/sourceTYPE[source_pump]": {
         "associated_beam": "/entry/instrument/beam_pump",
         "frequency": "@attrs:metadata/instrument/beam/pump/frequency",
         "frequency/@units": "kHz",
         "mode": "Single Bunch",
         "name": "OPCPA @ TR-ARPES @ FHI",
         "probe": "visible light",
         "type": "Optical Laser"
     },
-    "/ENTRY[entry]/PROCESS[process]/CALIBRATION[angular1_calibration]": {
-        "calibrated_axis": "@link:/entry/data/angular1"
+    "/ENTRY[entry]/PROCESS[process]/CALIBRATION[angular0_calibration]": {
+        "calibrated_axis": "@link:/entry/data/angular0"
     },
-    "/ENTRY[entry]/PROCESS[process]/energy_calibration": {
+    "/ENTRY[entry]/PROCESS[process]/CALIBRATION[energy_calibration]": {
         "calibrated_axis": "@link:/entry/data/energy"
     },
     "/ENTRY[entry]/SAMPLE[sample]": {
         "SUBSTANCE[substance]/molecular_formula_hill": "@attrs:metadata/sample/chemical_formula",
-        "bias": {
-            "voltmeter": "@link:/entry/instrument/manipulator/sample_bias_voltmeter"
-        },
-        "depends_on": "/entry/sample/transformations/offset_azimuth",
-        "description": "@attrs:metadata/sample/chemical_formula",
-        "drain_current": {
-            "amperemeter": "@link:/entry/instrument/manipulator/drain_current_amperemeter"
-        },
-        "gas_pressure": {
-            "pressure_gauge": "@link:/entry/instrument/pressure_gauge"
-        },
-        "name": "@attrs:metadata/sample/name",
-        "preparation_date": "@attrs:metadata/sample/preparation_date",
-        "sample_history/notes": "@attrs:metadata/sample/sample_history",
-        "situation": "vacuum",
-        "temperature": {
-            "temperature_sensor": "@link:/entry/instrument/manipulator/temperature_sensor"
-        },
-        "transformations": {
+        "TRANSFORMATIONS[transformations]": {
             "AXISNAME[trans_x]": "@attrs:metadata/scan_info/trARPES:Carving:TRX.RBV",
             "AXISNAME[trans_x]/@depends_on": "/entry/instrument/manipulator/transformations/trans_z",
             "AXISNAME[trans_x]/@transformation_type": "translation",
             "AXISNAME[trans_x]/@units": "mm",
             "AXISNAME[trans_x]/@vector": [
                 0,
                 1,
@@ -373,14 +355,32 @@
             "sample_tilt/@transformation_type": "rotation",
             "sample_tilt/@units": "degrees",
             "sample_tilt/@vector": [
                 1,
                 0,
                 0
             ]
+        },
+        "bias": {
+            "voltmeter": "@link:/entry/instrument/manipulator/sample_bias_voltmeter"
+        },
+        "depends_on": "/entry/sample/transformations/offset_azimuth",
+        "description": "@attrs:metadata/sample/chemical_formula",
+        "drain_current": {
+            "amperemeter": "@link:/entry/instrument/manipulator/drain_current_amperemeter"
+        },
+        "gas_pressure": {
+            "pressure_gauge": "@link:/entry/instrument/pressure_gauge"
+        },
+        "history/notes/description": "@attrs:metadata/sample/sample_history",
+        "name": "@attrs:metadata/sample/name",
+        "preparation_date": "@attrs:metadata/sample/preparation_date",
+        "situation": "vacuum",
+        "temperature": {
+            "temperature_sensor": "@link:/entry/instrument/manipulator/temperature_sensor"
         }
     },
     "/ENTRY[entry]/USER[user]": {
         "address": "@attrs:metadata/user0/address",
         "affiliation": "@attrs:metadata/user0/affiliation",
         "email": "@attrs:metadata/user0/email",
         "name": "@attrs:metadata/user0/name",
```

### Comparing `specsanalyzer-0.2.0/specsscan/config/default.yaml` & `specsanalyzer-0.2.1a0/specsscan/config/default.yaml`

 * *Files identical despite different names*

### Comparing `specsanalyzer-0.2.0/specsscan/config/example_config_FHI.yaml` & `specsanalyzer-0.2.1a0/specsscan/config/example_config_FHI.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -2,44 +2,42 @@
 data_path: "path/to/data"
 # option to enable nested progress bars
 enable_nested_progress_bar: false
 
 # dictionary containing renaming rules for axis names (to change the name in the xarrays)
 coordinate_mapping:
   Ekin: "energy"
-  Angle: "angular1"
-  polar: "angular2"
-  tilt: "angular2"
-  azimuth: "angular2"
-  X: "spatial1"
-  Y: "spatial1"
-  Z: "spatial1"
+  Angle: "angular0"
+  polar: "angular1"
+  tilt: "angular1"
+  azimuth: "angular1"
+  X: "spatial0"
+  Y: "spatial0"
+  Z: "spatial0"
 
 # dictionary of corresponding NeXus paths for the different axes
 coordinate_depends:
   Ekin: "/entry/instrument/electronanalyser/energydispersion/kinetic_energy"
   Angle: "/entry/instrument/electronanalyser/transformations/analyzer_dispersion"
   polar: "/entry/sample/transformations/sample_polar"
   tilt: "/entry/sample/transformations/sample_tilt"
   azimuth: "/entry/sample/transformations/sample_azimuth"
   X: "/entry/sample/transformations/trans_x"
   Y: "/entry/sample/transformations/trans_y"
   Z: "/entry/sample/transformations/trans_z"
 
 # dictionary containing units for the respective axes
 units:
+  angular0: "degree"
   angular1: "degree"
-  angular2: "degree"
   energy: "eV"
   delay: "fs"
   mirrorX: "steps"
   mirrorY: "steps"
-  X: "mm"
-  Y: "mm"
-  Z: "mm"
+  spatial0: "mm"
   voltage: "V"
 
 # URL of the epics archiver request engine
 archiver_url: "http://__epicsarchiver_host__:17668/retrieval/data/getData.json?pv="
 # dictionary containing axis names with Epics channels to request from the EPICS archiver
 epics_channels:
   tempa: "trARPES:Carving:TEMP_RBV"
```

### Comparing `specsanalyzer-0.2.0/specsscan/core.py` & `specsanalyzer-0.2.1a0/specsscan/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,15 +154,15 @@
             tqdm_enable_nested=self._config["enable_nested_progress_bar"],
         )
 
         self._scan_info = parse_info_to_dict(scan_path)
 
         loader_dict = {
             "iterations": iterations,
-            "scan_path": scan_path,
+            "scan_path": str(scan_path),
             "raw_data": data,
         }
 
         (scan_type, lens_mode, kin_energy, pass_energy, work_function) = (
             self._scan_info["ScanType"],
             self._scan_info["LensMode"],
             self._scan_info["KineticEnergy"],
@@ -400,15 +400,15 @@
             tqdm_enable_nested=self._config["enable_nested_progress_bar"],
         )
 
         self._scan_info = parse_info_to_dict(scan_path)
 
         loader_dict = {
             "delays": delays,
-            "scan_path": scan_path,
+            "scan_path": str(scan_path),
             "raw_data": data,
             "check_scan": True,
         }
 
         (scan_type, lens_mode, kin_energy, pass_energy, work_function) = (
             self._scan_info["ScanType"],
             self._scan_info["LensMode"],
```

### Comparing `specsanalyzer-0.2.0/specsscan/helpers.py` & `specsanalyzer-0.2.1a0/specsscan/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,26 +375,26 @@
 
     if metadata is None:
         metadata = {}
 
     print("Gathering metadata from different locations")
     # get metadata from LUT dataframe
     lut_meta = {}
-    energy_scan_mode = "fixed"
+    energy_scan_mode = "snapshot"
     if df_lut is not None:
         for col in df_lut.columns:
             col_array = df_lut[f"{col}"].to_numpy()
             if len(set(col_array)) == 1:
                 lut_meta[col] = col_array[0]
             else:
                 lut_meta[col] = col_array
 
         kinetic_energy = df_lut["KineticEnergy"].to_numpy()
         if len(set(kinetic_energy)) > 1 and scan_info["ScanType"] == "voltage":
-            energy_scan_mode = "sweep"
+            energy_scan_mode = "fixed_analyser_transmission"
 
     metadata["scan_info"] = complete_dictionary(
         metadata.get("scan_info", {}),
         complete_dictionary(lut_meta, scan_info),
     )  # merging dictionaries
 
     print("Collecting time stamps...")
```

### Comparing `specsanalyzer-0.2.0/setup.py` & `specsanalyzer-0.2.1a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,30 @@
  'imutils>=0.5.4',
  'ipympl>=0.9.1',
  'ipywidgets>=7.7.1',
  'matplotlib>=3.5.1',
  'numpy>=1.21.6',
  'opencv-python>=4.8.1.78',
  'pynxtools-mpes>=0.0.1',
+ 'pynxtools>=0.3.1',
  'python-dateutil>=2.8.2',
  'pyyaml>=6.0',
  'scipy>=1.8.0',
  'tifffile>=2022.5.4',
+ 'tqdm>=4.62.3',
  'xarray>=0.20.2']
 
 extras_require = \
 {'notebook': ['jupyter[notebook]>=1.0.0',
               'ipykernel[notebook]>=6.9.1',
               'jupyterlab-h5web[notebook]>=7.0.0']}
 
 setup_kwargs = {
     'name': 'specsanalyzer',
-    'version': '0.2.0',
+    'version': '0.2.1a0',
     'description': 'Python package for loading and converting SPECS Phoibos analyzer data.',
     'long_description': '[![Documentation Status](https://github.com/OpenCOMPES/specsanalyzer/actions/workflows/documentation.yml/badge.svg)](https://opencompes.github.io/specsanalyzer/)\n[![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)\n![](https://github.com/OpenCOMPES/specsanalyzer/actions/workflows/linting.yml/badge.svg)\n![](https://github.com/OpenCOMPES/specsanalyzer/actions/workflows/testing_multiversion.yml/badge.svg?branch=main)\n![](https://img.shields.io/pypi/pyversions/specsanalyzer)\n![](https://img.shields.io/pypi/l/specsanalyzer)\n[![](https://img.shields.io/pypi/v/specsanalyzer)](https://pypi.org/project/specsanalyzer)\n[![Coverage Status](https://coveralls.io/repos/github/OpenCOMPES/specsanalyzer/badge.svg?branch=main&kill_cache=1)](https://coveralls.io/github/OpenCOMPES/specsanalyzer?branch=main)\n\n# specsanalyzer\nThis is the package `specsanalyzer` for conversion and handling of SPECS Phoibos analyzer data.\n\nThis package contains two modules:\n`specsanalyzer` is a package to import and convert MCP analyzer images from SPECS Phoibos analyzers into energy and emission angle/physical coordinates.\n`specsscan` is a Python package for loading Specs Phoibos scans accquired with the labview software developed at FHI/EPFL\n\nTutorials for usage and the API documentation can be found in the [Documentation](https://opencompes.github.io/specsanalyzer/)\n\n## Installation\n\n### Pip (for users)\n\n- Create a new virtual environment using either venv, pyenv, conda, etc. See below for an example.\n\n```bash\npython -m venv .specs-venv\n```\n\n- Activate your environment:\n\n```bash\nsource .specs-venv/bin/activate\n```\n\n- Install `specsanalyzer` from PyPI:\n\n```bash\npip install specsanalyzer\n```\n\n- This should install all the requirements to run `specsanalyzer` and `specsscan`in your environment.\n\n- If you intend to work with Jupyter notebooks, it is helpful to install a Jupyter kernel for your environment. This can be done, once your environment is activated, by typing:\n\n```bash\npython -m ipykernel install --user --name=specs_kernel\n```\n\n#### Configuration and calib2d file\nThe conversion procedures require to set up several configuration parameters in a config file. An example config file is provided as part of the package (see documentation). Configuration files can either be passed to the class constructures, or are read from system-wide or user-defined locations (see documentation).\n\nMost importantly, conversion of analyzer data to energy/angular coordinates requires detector calibration data provided by the manufacturer. The corresponding *.calib2d file (e.g. phoibos150.calbid2d) are provided together with the spectrometer software, and need to be set in the config file.\n\n### For Contributors\n\nTo contribute to the development of `specsanalyzer`, you can follow these steps:\n\n1. Clone the repository:\n\n```bash\ngit clone https://github.com/OpenCOMPES/specsanalyzer.git\ncd specsanalyzer\n```\n\n2. Check out test data (optional, requires access rights):\n\n```bash\ngit submodule sync --recursive\ngit submodule update --init --recursive\n```\n\n2. Install the repository in editable mode:\n\n```bash\npip install -e .\n```\n\nNow you have the development version of `specsanalyzer` installed in your local environment. Feel free to make changes and submit pull requests.\n\n### Poetry (for maintainers)\n\n- Prerequisites:\n  + Poetry: https://python-poetry.org/docs/\n\n- Create a virtual environment by typing:\n\n```bash\npoetry shell\n```\n\n- A new shell will be spawned with the new environment activated.\n\n- Install the dependencies from the `pyproject.toml` by typing:\n\n```bash\npoetry install --with dev, docs\n```\n\n- If you wish to use the virtual environment created by Poetry to work in a Jupyter notebook, you first need to install the optional notebook dependencies and then create a Jupyter kernel for that.\n\n  + Install the optional dependencies `ipykernel` and `jupyter`:\n\n  ```bash\n  poetry install -E notebook\n  ```\n\n  + Make sure to run the command below within your virtual environment (`poetry run` ensures this) by typing:\n\n  ```bash\n  poetry run ipython kernel install --user --name=specs_poetry\n  ```\n\n  + The new kernel will now be available in your Jupyter kernels list.\n',
     'author': 'Laurenz Rettig',
     'author_email': 'rettig@fhi-berlin.mpg.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/mpes-kit/specsanalyzer',
```

### Comparing `specsanalyzer-0.2.0/PKG-INFO` & `specsanalyzer-0.2.1a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: specsanalyzer
-Version: 0.2.0
+Version: 0.2.1a0
 Summary: Python package for loading and converting SPECS Phoibos analyzer data.
 Home-page: https://github.com/mpes-kit/specsanalyzer
 License: MIT
 Keywords: specs,phoibos,arpes
 Author: Laurenz Rettig
 Author-email: rettig@fhi-berlin.mpg.de
 Requires-Python: >=3.8,<3.12
@@ -21,19 +21,21 @@
 Requires-Dist: ipympl (>=0.9.1)
 Requires-Dist: ipywidgets (>=7.7.1)
 Requires-Dist: jupyter[notebook] (>=1.0.0); extra == "notebook"
 Requires-Dist: jupyterlab-h5web[notebook] (>=7.0.0); extra == "notebook"
 Requires-Dist: matplotlib (>=3.5.1)
 Requires-Dist: numpy (>=1.21.6)
 Requires-Dist: opencv-python (>=4.8.1.78)
+Requires-Dist: pynxtools (>=0.3.1)
 Requires-Dist: pynxtools-mpes (>=0.0.1)
 Requires-Dist: python-dateutil (>=2.8.2)
 Requires-Dist: pyyaml (>=6.0)
 Requires-Dist: scipy (>=1.8.0)
 Requires-Dist: tifffile (>=2022.5.4)
+Requires-Dist: tqdm (>=4.62.3)
 Requires-Dist: xarray (>=0.20.2)
 Project-URL: Documentation, https://github.com/mpes-kit/specsanalyzer/docs
 Project-URL: Repository, https://github.com/mpes-kit/specsanalyzer
 Description-Content-Type: text/markdown
 
 [![Documentation Status](https://github.com/OpenCOMPES/specsanalyzer/actions/workflows/documentation.yml/badge.svg)](https://opencompes.github.io/specsanalyzer/)
 [![Ruff](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/astral-sh/ruff/main/assets/badge/v2.json)](https://github.com/astral-sh/ruff)
```

