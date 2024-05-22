# Comparing `tmp/wallbox-0.6.0.tar.gz` & `tmp/wallbox-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wallbox-0.6.0.tar", last modified: Wed Feb 14 15:48:26 2024, max compression
+gzip compressed data, was "wallbox-0.7.0.tar", last modified: Wed May 22 17:17:39 2024, max compression
```

## Comparing `wallbox-0.6.0.tar` & `wallbox-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:48:26.554873 wallbox-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-02-14 15:48:18.000000 wallbox-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-02-14 15:48:26.554873 wallbox-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-02-14 15:48:18.000000 wallbox-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-14 15:48:26.554873 wallbox-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-02-14 15:48:18.000000 wallbox-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:48:26.554873 wallbox-0.6.0/wallbox/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-02-14 15:48:18.000000 wallbox-0.6.0/wallbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-02-14 15:48:18.000000 wallbox-0.6.0/wallbox/bearerauth.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-02-14 15:48:18.000000 wallbox-0.6.0/wallbox/statuses.py
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-02-14 15:48:18.000000 wallbox-0.6.0/wallbox/wallbox.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-14 15:48:26.554873 wallbox-0.6.0/wallbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3411 2024-02-14 15:48:26.000000 wallbox-0.6.0/wallbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-02-14 15:48:26.000000 wallbox-0.6.0/wallbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-14 15:48:26.000000 wallbox-0.6.0/wallbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-14 15:48:26.000000 wallbox-0.6.0/wallbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-14 15:48:26.000000 wallbox-0.6.0/wallbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:17:39.395798 wallbox-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 17:17:33.000000 wallbox-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-05-22 17:17:39.395798 wallbox-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4526 2024-05-22 17:17:33.000000 wallbox-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 17:17:39.395798 wallbox-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-22 17:17:33.000000 wallbox-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:17:39.391798 wallbox-0.7.0/wallbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-22 17:17:33.000000 wallbox-0.7.0/wallbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-22 17:17:33.000000 wallbox-0.7.0/wallbox/bearerauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-22 17:17:33.000000 wallbox-0.7.0/wallbox/statuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9318 2024-05-22 17:17:33.000000 wallbox-0.7.0/wallbox/wallbox.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:17:39.395798 wallbox-0.7.0/wallbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-05-22 17:17:39.000000 wallbox-0.7.0/wallbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-22 17:17:39.000000 wallbox-0.7.0/wallbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 17:17:39.000000 wallbox-0.7.0/wallbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-22 17:17:39.000000 wallbox-0.7.0/wallbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 17:17:39.000000 wallbox-0.7.0/wallbox.egg-info/top_level.txt
```

### Comparing `wallbox-0.6.0/LICENSE` & `wallbox-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wallbox-0.6.0/PKG-INFO` & `wallbox-0.7.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: wallbox
-Version: 0.6.0
-Summary: Module for interacting with Wallbox EV charger api
-Home-page: https://github.com/cliviu74/wallbox
-Author: Liviu Chiribuca
-Author-email: cliviu74@yahoo.com
-License: Apache 2
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests>=2.22.0
-Requires-Dist: simplejson>=3.16.0
-Requires-Dist: aenum>=3.1.8
-
 # wallbox
 
 Python Module interface for Wallbox EV chargers api
 
 ## Requirements
 
 Python 3.7 or older Python modules "requests>=2.22.0", "simplejson>=3.16.0"
@@ -60,14 +44,18 @@
 
 - pauses a charging session
 
 ### resumeChargingSession(chargerId)
 
 - resumes a charging session
 
+### resumeSchedule(chargerId)
+
+- revert charger back to default schedule after manually starting a charging session, it reverts the charger back into "Eco Smart and Scheduled" charing mode, if used.
+
 ### getSessionList(chargerId, startDate, endDate)
 
 - provides the list of charging sessions between startDate and endDate
 - startDate and endDate are provided in Python datetime format (i.e. 2021-05-04 08:41:12.765644)
 
 ### setEnergyCost(chargerId, energyCost)
 
@@ -75,14 +63,67 @@
 
 ### restartCharger(chargerId)
 
 - restarts (reboots) charger
 - a full charger reboot can take a few minutes. Charger status will be slow to update (ie: READY (10s) -> DISCONNECTED (90s) -> READY)
 CAUTION: use this method with care!! Check if the charger is not in the middle of a firmware upgrade as this can brick your charger. 
 
+
+### setIcpMaxCurrent(chargerId, newIcpMaxCurrentValue)
+
+- sets charger Maximum ICP Current available (Amps).
+
+Please note that the wallbox may refuse this action if not setup properly of if not supported by your model
+
+
+### getChargerSchedules(chargerId)
+
+- gets the currently configured schedules for that charger. 
+
+Response is a JSON structure like the following:
+
+```json
+{
+    'schedules': [{
+        'chargerId': 42,
+        'enable': 1,
+        'max_current': 1,
+        'max_energy': 0,
+        'days': {'friday': true, 'monday': true, 'saturday': true, 'sunday': true, 'thursday': true,
+                    'tuesday': true, 'wednesday': true},
+        'start': '2100',
+        'stop': '0500'
+    }]
+}
+```
+
+### setChargerSchedules(chargerId, newSchedules)
+
+- Create or replace an existing schedule. 
+
+`newSchedules` is a dictionary like the following:
+
+```json
+{
+    'schedules': [{
+        'id': 0,
+        'chargerId': 42,
+        'enable': 1,
+        'max_current': 1,
+        'max_energy': 0,
+        'days': {'friday': true, 'monday': true, 'saturday': true, 'sunday': true, 'thursday': true,
+                    'tuesday': true, 'wednesday': true},
+        'start': '2100',
+        'stop': '0500'
+    }]
+}
+```
+
+As schedules returned by `getChargerSchedules` are positional, the `id` field in the payload represents the position of the schedule to add/replace.
+
 ## Simple example
 
 ```python
 from wallbox import Wallbox, Statuses
 import time
 import datetime
```

### Comparing `wallbox-0.6.0/setup.py` & `wallbox-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read(name):
     return open(os.path.join(os.path.dirname(__file__), name)).read()
 
 
 setup(
     name="wallbox",
-    version="0.6.0",
+    version="0.7.0",
     description="Module for interacting with Wallbox EV charger api",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     keywords="",
     author="Liviu Chiribuca",
     author_email="cliviu74@yahoo.com",
     url="https://github.com/cliviu74/wallbox",
```

### Comparing `wallbox-0.6.0/wallbox/wallbox.py` & `wallbox-0.7.0/wallbox/wallbox.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """
 
 Wallbox class
 
 """
 
 from datetime import datetime
-from time import timezone
 from requests.auth import HTTPBasicAuth
 import requests
 import json
 
 from wallbox.bearerauth import BearerAuth
 
 
@@ -68,125 +67,192 @@
         self.jwtRefreshTokenTtl = json.loads(response.text)["data"]["attributes"]["refresh_token_ttl"]
         self.headers["Authorization"] = f"Bearer {self.jwtToken}"
 
     def getChargersList(self):
         chargerIds = []
         try:
             response = requests.get(
-                f"{self.baseUrl}v3/chargers/groups", headers=self.headers,
+                f"{self.baseUrl}v3/chargers/groups",
+                headers=self.headers,
                 timeout=self._requestGetTimeout
             )
             response.raise_for_status()
         except requests.exceptions.HTTPError as err:
             raise (err)
         for group in json.loads(response.text)["result"]["groups"]:
             for charger in group["chargers"]:
                 chargerIds.append(charger["id"])
         return chargerIds
 
     def getChargerStatus(self, chargerId):
         try:
             response = requests.get(
-                f"{self.baseUrl}chargers/status/{chargerId}", headers=self.headers,
+                f"{self.baseUrl}chargers/status/{chargerId}", 
+                headers=self.headers,
                 timeout=self._requestGetTimeout
             )
             response.raise_for_status()
         except requests.exceptions.HTTPError as err:
             raise (err)
         return json.loads(response.text)
 
     def unlockCharger(self, chargerId):
         try:
             response = requests.put(
                 f"{self.baseUrl}v2/charger/{chargerId}",
                 headers=self.headers,
                 data='{"locked":0}',
+                timeout=self._requestGetTimeout
             )
             response.raise_for_status()
         except requests.exceptions.HTTPError as err:
             raise (err)
         return json.loads(response.text)
 
     def lockCharger(self, chargerId):
         try:
             response = requests.put(
                 f"{self.baseUrl}v2/charger/{chargerId}",
                 headers=self.headers,
                 data='{"locked":1}',
+                timeout=self._requestGetTimeout
             )
             response.raise_for_status()
         except requests.exceptions.HTTPError as err:
             raise (err)
         return json.loads(response.text)
 
     def setMaxChargingCurrent(self, chargerId, newMaxChargingCurrentValue):
         try:
             response = requests.put(
                 f"{self.baseUrl}v2/charger/{chargerId}",
                 headers=self.headers,
                 data=f'{{ "maxChargingCurrent":{newMaxChargingCurrentValue}}}',
+                timeout=self._requestGetTimeout
             )
             response.raise_for_status()
         except requests.exceptions.HTTPError as err:
             raise (err)
         return json.loads(response.text)
 
     def pauseChargingSession(self, chargerId):
         try:
             response = requests.post(
                 f"{self.baseUrl}v3/chargers/{chargerId}/remote-action",
                 headers=self.headers,
                 data='{"action":2}',
+                timeout=self._requestGetTimeout
             )
             response.raise_for_status()
         except requests.exceptions.HTTPError as err:
             raise (err)
         return json.loads(response.text)
 
     def resumeChargingSession(self, chargerId):
         try:
             response = requests.post(
                 f"{self.baseUrl}v3/chargers/{chargerId}/remote-action",
                 headers=self.headers,
                 data='{"action":1}',
+                timeout=self._requestGetTimeout
+            )
+            response.raise_for_status()
+        except requests.exceptions.HTTPError as err:
+            raise (err)
+        return json.loads(response.text)
+
+    def resumeSchedule(self, chargerId):
+        try:
+            response = requests.post(
+                f"{self.baseUrl}v3/chargers/{chargerId}/remote-action",
+                headers=self.headers,
+                data='{"action":9}',
+                timeout=self._requestGetTimeout
             )
             response.raise_for_status()
         except requests.exceptions.HTTPError as err:
             raise (err)
         return json.loads(response.text)
 
     def restartCharger(self, chargerId):
         try:
             response = requests.post(
                 f"{self.baseUrl}v3/chargers/{chargerId}/remote-action",
                 headers=self.headers,
                 data='{"action":3}',
+                timeout=self._requestGetTimeout
             )
             response.raise_for_status()
         except requests.exceptions.HTTPError as err:
             raise (err)
         return json.loads(response.text)
 
     def getSessionList(self, chargerId, startDate, endDate):
         try:
             payload = {'charger': chargerId, 'start_date': startDate.timestamp(), 'end_date': endDate.timestamp() }
 
             response = requests.get(
-                f"{self.baseUrl}v4/sessions/stats", params=payload, headers=self.headers,
+                f"{self.baseUrl}v4/sessions/stats",
+                params=payload,
+                headers=self.headers,
                 timeout=self._requestGetTimeout
             )
             response.raise_for_status()
         except requests.exceptions.HTTPError as err:
             raise (err)
         return json.loads(response.text)
 
     def setEnergyCost(self, chargerId, energyCost):
         try:
             response = requests.post(
                 f"{self.baseUrl}chargers/config/{chargerId}",
                 headers=self.headers,
                 json={'energyCost': energyCost},
+                timeout=self._requestGetTimeout
+            )
+            response.raise_for_status()
+        except requests.exceptions.HTTPError as err:
+            raise (err)
+        return json.loads(response.text)
+
+
+    def setIcpMaxCurrent(self, chargerId, newIcpMaxCurrentValue):
+        try:
+            response = requests.post(
+                f"{self.baseUrl}chargers/config/{chargerId}",
+                headers=self.headers,
+                json={'icp_max_current': newIcpMaxCurrentValue},
+                timeout=self._requestGetTimeout
+            )
+            response.raise_for_status()
+        except requests.exceptions.HTTPError as err:
+            raise (err)
+        return json.loads(response.text)
+    
+    def getChargerSchedules(self, chargerId):
+        try:
+            response = requests.get(
+                f"{self.baseUrl}chargers/{chargerId}/schedules",
+                headers=self.headers,
+                timeout=self._requestGetTimeout
+            )
+            response.raise_for_status()
+        except requests.exceptions.HTTPError as err:
+            raise (err)
+        return json.loads(response.text)
+
+    def setChargerSchedules(self, chargerId, newSchedules):
+        try:
+            # Enforce chargerId
+            for schedule in newSchedules.get('schedules', []):
+                schedule['chargerId'] = chargerId
+
+            response = requests.post(
+                f"{self.baseUrl}chargers/{chargerId}/schedules",
+                headers=self.headers,
+                json=newSchedules,
+                timeout=self._requestGetTimeout
             )
             response.raise_for_status()
         except requests.exceptions.HTTPError as err:
             raise (err)
         return json.loads(response.text)
```

