# Comparing `tmp/mke_sculib-2.5.8.tar.gz` & `tmp/mke_sculib-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mke_sculib-2.5.8.tar", last modified: Wed May 15 19:54:01 2024, max compression
+gzip compressed data, was "mke_sculib-2.5.9.tar", last modified: Tue May 21 20:08:22 2024, max compression
```

## Comparing `mke_sculib-2.5.8.tar` & `mke_sculib-2.5.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 19:54:01.397412 mke_sculib-2.5.8/
--rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.5.8/LICENSE
--rw-rw-rw-   0        0        0     4120 2024-05-15 19:54:01.397412 mke_sculib-2.5.8/PKG-INFO
--rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.5.8/README.rst
--rw-rw-rw-   0        0        0     1017 2024-05-15 19:54:01.398412 mke_sculib-2.5.8/setup.cfg
--rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.5.8/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 19:54:01.381408 mke_sculib-2.5.8/src/
-drwxrwxrwx   0        0        0        0 2024-05-15 19:54:01.392411 mke_sculib-2.5.8/src/mke_sculib/
--rw-rw-rw-   0        0        0     1216 2024-05-15 19:50:49.000000 mke_sculib-2.5.8/src/mke_sculib/__init__.py
--rw-rw-rw-   0        0        0   102025 2024-05-11 06:53:52.000000 mke_sculib-2.5.8/src/mke_sculib/acu.py
--rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.5.8/src/mke_sculib/cam_sensors.py
--rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.5.8/src/mke_sculib/chan_list_acu.py
--rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.5.8/src/mke_sculib/helpers.py
--rw-rw-rw-   0        0        0    10152 2024-05-11 15:06:30.000000 mke_sculib-2.5.8/src/mke_sculib/js_helpers.py
--rw-rw-rw-   0        0        0    26166 2023-12-05 16:11:38.000000 mke_sculib-2.5.8/src/mke_sculib/mock_telescope.py
--rw-rw-rw-   0        0        0   108468 2024-05-15 19:53:14.000000 mke_sculib-2.5.8/src/mke_sculib/scu.py
--rw-rw-rw-   0        0        0    21285 2024-05-15 19:50:24.000000 mke_sculib-2.5.8/src/mke_sculib/sim.py
--rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.5.8/src/mke_sculib/stellarium_api.py
-drwxrwxrwx   0        0        0        0 2024-05-15 19:54:01.395412 mke_sculib-2.5.8/src/mke_sculib.egg-info/
--rw-rw-rw-   0        0        0     4120 2024-05-15 19:54:01.000000 mke_sculib-2.5.8/src/mke_sculib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      542 2024-05-15 19:54:01.000000 mke_sculib-2.5.8/src/mke_sculib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 19:54:01.000000 mke_sculib-2.5.8/src/mke_sculib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2024-05-15 19:54:01.000000 mke_sculib-2.5.8/src/mke_sculib.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-15 19:54:01.000000 mke_sculib-2.5.8/src/mke_sculib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-15 19:54:01.396412 mke_sculib-2.5.8/tests/
--rw-rw-rw-   0        0        0     9759 2024-05-09 13:27:46.000000 mke_sculib-2.5.8/tests/test_acu_sim.py
--rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.5.8/tests/test_scu.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:08:22.583356 mke_sculib-2.5.9/
+-rw-rw-rw-   0        0        0    35149 2022-07-03 09:33:46.000000 mke_sculib-2.5.9/LICENSE
+-rw-rw-rw-   0        0        0     4120 2024-05-21 20:08:22.583356 mke_sculib-2.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3367 2023-09-13 15:37:28.000000 mke_sculib-2.5.9/README.rst
+-rw-rw-rw-   0        0        0     1017 2024-05-21 20:08:22.584357 mke_sculib-2.5.9/setup.cfg
+-rw-rw-rw-   0        0        0      359 2022-07-29 10:19:10.000000 mke_sculib-2.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:08:22.552356 mke_sculib-2.5.9/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 20:08:22.578356 mke_sculib-2.5.9/src/mke_sculib/
+-rw-rw-rw-   0        0        0     1216 2024-05-21 18:09:07.000000 mke_sculib-2.5.9/src/mke_sculib/__init__.py
+-rw-rw-rw-   0        0        0   102025 2024-05-11 06:53:52.000000 mke_sculib-2.5.9/src/mke_sculib/acu.py
+-rw-rw-rw-   0        0        0     1492 2022-07-08 13:07:16.000000 mke_sculib-2.5.9/src/mke_sculib/cam_sensors.py
+-rw-rw-rw-   0        0        0    24398 2023-06-30 07:33:40.000000 mke_sculib-2.5.9/src/mke_sculib/chan_list_acu.py
+-rw-rw-rw-   0        0        0     1261 2023-09-22 14:56:52.000000 mke_sculib-2.5.9/src/mke_sculib/helpers.py
+-rw-rw-rw-   0        0        0    10152 2024-05-11 15:06:30.000000 mke_sculib-2.5.9/src/mke_sculib/js_helpers.py
+-rw-rw-rw-   0        0        0    27277 2024-05-21 18:30:01.000000 mke_sculib-2.5.9/src/mke_sculib/mock_telescope.py
+-rw-rw-rw-   0        0        0   108891 2024-05-21 20:04:12.000000 mke_sculib-2.5.9/src/mke_sculib/scu.py
+-rw-rw-rw-   0        0        0    21771 2024-05-21 18:30:09.000000 mke_sculib-2.5.9/src/mke_sculib/sim.py
+-rw-rw-rw-   0        0        0     9006 2024-03-13 10:18:35.000000 mke_sculib-2.5.9/src/mke_sculib/stellarium_api.py
+drwxrwxrwx   0        0        0        0 2024-05-21 20:08:22.581355 mke_sculib-2.5.9/src/mke_sculib.egg-info/
+-rw-rw-rw-   0        0        0     4120 2024-05-21 20:08:22.000000 mke_sculib-2.5.9/src/mke_sculib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      542 2024-05-21 20:08:22.000000 mke_sculib-2.5.9/src/mke_sculib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 20:08:22.000000 mke_sculib-2.5.9/src/mke_sculib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2024-05-21 20:08:22.000000 mke_sculib-2.5.9/src/mke_sculib.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-21 20:08:22.000000 mke_sculib-2.5.9/src/mke_sculib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 20:08:22.582356 mke_sculib-2.5.9/tests/
+-rw-rw-rw-   0        0        0     9759 2024-05-09 13:27:46.000000 mke_sculib-2.5.9/tests/test_acu_sim.py
+-rw-rw-rw-   0        0        0     2273 2023-12-05 16:11:38.000000 mke_sculib-2.5.9/tests/test_scu.py
```

### Comparing `mke_sculib-2.5.8/LICENSE` & `mke_sculib-2.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.8/PKG-INFO` & `mke_sculib-2.5.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke_sculib
-Version: 2.5.8
+Version: 2.5.9
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.5.8/README.rst` & `mke_sculib-2.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.8/setup.cfg` & `mke_sculib-2.5.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.8/src/mke_sculib/__init__.py` & `mke_sculib-2.5.9/src/mke_sculib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '2.5.8'
+__version__ = '2.5.9'
 
 from mke_sculib.scu import scu as scu_api, plot_tt, print_color, colors
 from mke_sculib.sim import scu_sim
 from mke_sculib.stellarium_api import stellarium_api as stellar_api
 from mke_sculib.sim import plot_motion_pyplot as plot_motion
 from mke_sculib.helpers import get_utcnow, make_zulustr, parse_zulutime
```

### Comparing `mke_sculib-2.5.8/src/mke_sculib/acu.py` & `mke_sculib-2.5.9/src/mke_sculib/acu.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.8/src/mke_sculib/cam_sensors.py` & `mke_sculib-2.5.9/src/mke_sculib/cam_sensors.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.8/src/mke_sculib/chan_list_acu.py` & `mke_sculib-2.5.9/src/mke_sculib/chan_list_acu.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.8/src/mke_sculib/helpers.py` & `mke_sculib-2.5.9/src/mke_sculib/helpers.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.8/src/mke_sculib/js_helpers.py` & `mke_sculib-2.5.9/src/mke_sculib/js_helpers.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.8/src/mke_sculib/mock_telescope.py` & `mke_sculib-2.5.9/src/mke_sculib/mock_telescope.py`

 * *Files 2% similar despite different names*

```diff
@@ -544,26 +544,55 @@
         except Exception as E:
             _log.error("Exception thrown during command execution")
             _log.exception(E)
             return dict(status=500, headers={'Content-Type': 'application/json'}, body="{}")
 
         return dict(status=200, headers={'Content-Type': 'application/json'}, body="{}")
 
+    def devices_getAllDeviceStatusValues(self, args):
+        _log.debug("status value")
+        if "device" not in args:
+            return dict(status=202, headers={'Content-Type': 'application/json'}, body="{}")
+        
+        if args["device"] != "acu":
+            return dict(status=404, headers={'Content-Type': 'application/json'}, body="{}")
+
+        with self.dataLock:
+            def helper(k):
+                return {
+                    "path": k,
+                    "values": [
+                        {
+                            "timestamp": self.t_internal.iso,
+                            "lastValue": str(copy.copy(self.data[k]))
+                        }
+                    ]
+                }
+            r = [helper(k) for k in self.data]
+
+        return dict(status=200, headers={'Content-Type': 'application/json'}, body=json.dumps(r))
+    
+    def devices_statusPaths(self, args):
+        with self.dataLock:
+            return dict(status=200, headers={'Content-Type': 'application/json'}, body=json.dumps([k for k in self.data.keys()]))
+        
+
     def devices_statusValue(self, args):
         _log.debug("status value")
         if "path" not in args:
             return dict(status=202, headers={'Content-Type': 'application/json'}, body="{}")
         path = args.get("path")
         try:
             value = self.get(path)
         except KeyError:
             value = 'UNKNOWN'
 
         return dict(status=200, headers={'Content-Type': 'application/json'}, body=json.dumps({"value": value, 'finalValue': value}))
 
+
     
     def datalogging_sessions(self, *args):
         _log.debug("sessions")
         with self.dataLock:
             value = [k for k in self.datalog.keys()]
         return dict(status=200, headers={'Content-Type': 'application/json'}, body=json.dumps({"value": value}))
```

### Comparing `mke_sculib-2.5.8/src/mke_sculib/scu.py` & `mke_sculib-2.5.9/src/mke_sculib/scu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1006,23 +1006,37 @@
                     log('  -> done', color=colors.OKBLUE)
                 return True
 
             if not no_stout and is_first:
                 if isinstance(value, float):
                     log('wait for {}: {:.3f} (currently at: {:.3f})'.format(path, value, v), color=colors.OKBLUE)
                 elif 'state' in path:
-                    log('wait for {}: {} (currently at: {})'.format(path, state_dc.get(value, value), state_dc.get(v, v)), color=colors.OKBLUE)
+                    if not isinstance(value, str) and hasattr(value, '__len__'):
+                        vv = [state_dc.get(vvv, vvv) for vvv in value]
+                    else:
+                        vv = state_dc.get(value, value)
+                    log('wait for {}: {} (currently at: {})'.format(path, vv, state_dc.get(v, v)), color=colors.OKBLUE)
                 else:
                     log('wait for {}: {} (currently at: {})'.format(path, value, v), color=colors.OKBLUE)
 
                 is_first = False
 
-            self.wait_duration(query_delay, no_stout=True)  
+            self.wait_duration(query_delay, no_stout=True)
+
+        if 'state' in path:
+            v = self.getc(path)
+            v = (state_dc.get(v, v), v)
+            if not isinstance(value, str) and hasattr(value, '__len__'):
+                vv = [(state_dc.get(vvv, vvv), vvv) for vvv in value]
+            else:
+                vv = (state_dc.get(value, value), value)
+            err = "Sensor: {} not equal to {} after {}s. Current value: {}".format(path, vv, timeout, v)
+        else:
+            err = "Sensor: {} not equal to {} after {}s. Current value: {}".format(path, value, timeout, v)
 
-        err = "Sensor: {} not equal to {} after {}s. Current value: {}".format(path, value, timeout, v)
         log(err, color=colors.FAIL)
         raise TimeoutError(err)
 
     def get_device_status_value_async(self, pathes):
         params = [{"path": path} for path in pathes]
         devices = ["/devices/statusValue"] * len(params)
         return self.scu_get_concurrent(devices, params)
@@ -1093,26 +1107,23 @@
 
     def stow(self, pre_move=True, nowait=False):
         """stow the antenna on pos 1 (both axes) and wait for stowing to be completed
         """
         log('Stowing...')
 
 
-        if self.get_state() != 'Stowed':
+        if self.get_state().upper() != 'STOWED':
 
             if pre_move:
                 self.abs_azel(*self.stow_pos)
                 self.wait_duration(0.5)
                 self.wait_settle()
 
             if self.dish_type == 'mke':
-                self.reset_dmc() # because the ACU seems to be ignoring stows sometimes if this is not done 
-                self.scu_put("/devices/command", {"path": "acu.azimuth.drive_to_stow", "params":{"action": "1"}})
-                self.wait_duration(1.0)
-                self.scu_put("/devices/command", {"path": "acu.elevation.drive_to_stow", "params":{"action": "1"}})
+                self.scu_put("/devices/command", {"path": "acu.dish_management_controller.stow", "params": {"az_stow": "1", "el_stow": "1"}})
             else:
                 self.scu_put("/devices/command", {"path": "acu.dish_management_controller.stow", "params": {"action": "1"}})
 
         if not nowait:
             self.wait_state("acu.stow_pin_controller.azimuth_status", "DEPLOYED", operator='==')
             self.wait_state("acu.stow_pin_controller.elevation_status", "DEPLOYED", operator='==')
             self.wait_duration(1, no_stout=True)  
@@ -1974,14 +1985,15 @@
                     if self.debug:
                         log('setting pointing model with payload: ' + json.dumps(payload))
 
                     if is_last and not no_stdout:
                         log('setting pointing model to band "{}". Params: {}'.format(band, params), color=colors.OKBLUE)
 
                     self.scu_put('/devices/command', payload=payload)
+                    self.wait_duration(0.5)
                 
                 if wait_for_set:
                     if band != 'all' and bands_dc_inv[bandi] != str(fi_pos):
                         log('Can not wait for pointing model parameters to be set, because the feed indexer is in the wrong position. Will return without waiting! band_is = {} vs band_set = {}'.format(fi_pos, bandi), color=colors.WARNING)
                     else:
                         
                         for k, v in params.items():
@@ -2189,19 +2201,17 @@
             for k, v in configs_dc.items():
                 if k not in configs_scu:
                     log(f'Creating Default Config: {k} with n={len(v)} channels')
                     self.create_logger(k, v)
         
         self.wait_duration(5)
         self.activate_dmc()
+        self.waitForStatusValue("acu.azimuth.axis_bit_status.abs_active", True, timeout=20)
+        self.waitForStatusValue("acu.elevation.axis_bit_status.abs_active", True, timeout=20)
         self.wait_duration(5)
-        self.activate_axes()
-        self.wait_duration(3)
-        self.reset_dmc()
-        self.wait_duration(2)
 
         if band_start is not None:
             self.move_to_band(band_start)
 
         if az_start is not None:
             self.abs_azimuth(az_start, az_speed)
         if el_start is not None:
@@ -2214,19 +2224,15 @@
 
     def shutdown(self):
         """Stow, deactivate, and release command authority for antenna in order to finish before handing back the antenna
         """
         log('=== INITIATING SHUTDOWN ROUTINE ===', color=colors.BOLD)
         if self.get_state() != 'Stowed':
             self.stow()
-        self.wait_duration(5)
-        self.deactivate_axes()
-        self.wait_duration(5)
-        self.deactivate_dmc()
-        self.wait_duration(5)
+        self.wait_duration(10)
         self.release_command_authority()
         self.wait_duration(5)
 
         log('=== SHUTDOWN ROUTINE COMPLETED ===', color=colors.BOLD)
```

### Comparing `mke_sculib-2.5.8/src/mke_sculib/sim.py` & `mke_sculib-2.5.9/src/mke_sculib/sim.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,14 +78,17 @@
 
 
 
 def get_routes(telescope: Telescope) -> dict:
     dc_routes_get = {
         '/datalogging/currentState': lambda args: telescope.datalogging_currentState(*args),
         '/devices/statusValue': lambda args: telescope.devices_statusValue(args),
+        '/devices/getAllDeviceStatusValues': lambda args: telescope.devices_getAllDeviceStatusValues(args),
+        '/devices/statusPaths': lambda args: telescope.devices_statusPaths(args),
+
         '/datalogging/lastSession': lambda args: telescope.datalogging_lastSession(*args),
         '/datalogging/exportSession': lambda args: telescope.datalogging_exportSession(args),
         '/datalogging/sessions': lambda args: telescope.datalogging_sessions(*args),
     }
     dc_routes_put = {
         '/devices/command': lambda payload, params, data: telescope.devices_command(payload),
         '/datalogging/start': lambda payload, params, data: telescope.datalogging_start(*params),
@@ -214,18 +217,24 @@
                 return {k:allchans[k] for k in key}
             else:
                 return [allchans[k] for k in key]
         else:
             return self._get_device_status_value(key)
 
     def __getitem__(self, key):
-        return self.data[key]
+        if not isinstance(key, str) and hasattr(key, '__len__'):
+            return [self.data[k] for k in key]
+        else:
+            return self.data[key]
     
     def __contains__(self, key):
-        return key in self.data
+        if not isinstance(key, str) and hasattr(key, '__len__'):
+            return True if [k for k in key if k in self.data] else False
+        else:
+            return key in self.data
 
     @property
     def t_internal(self):
         """internal telescope time as astropy Time object based on MJD format
 
         Returns:
             astropy.time.Time: the ACU internal time now
```

### Comparing `mke_sculib-2.5.8/src/mke_sculib/stellarium_api.py` & `mke_sculib-2.5.9/src/mke_sculib/stellarium_api.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.8/src/mke_sculib.egg-info/PKG-INFO` & `mke_sculib-2.5.9/src/mke_sculib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mke-sculib
-Version: 2.5.8
+Version: 2.5.9
 Summary: MeerKAT Extension (SCU) (lib)rary for the MKE antennas and some basic simulators
 Home-page: https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib
 Author: Tobias Glaubach
 Author-email: tglaubach@mpifr-bonn.mpg.de
 Project-URL: Bug Tracker, https://gitlab.mpcdf.mpg.de/tglaubach/mke-sculib/-/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `mke_sculib-2.5.8/src/mke_sculib.egg-info/SOURCES.txt` & `mke_sculib-2.5.9/src/mke_sculib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.8/tests/test_acu_sim.py` & `mke_sculib-2.5.9/tests/test_acu_sim.py`

 * *Files identical despite different names*

### Comparing `mke_sculib-2.5.8/tests/test_scu.py` & `mke_sculib-2.5.9/tests/test_scu.py`

 * *Files identical despite different names*

