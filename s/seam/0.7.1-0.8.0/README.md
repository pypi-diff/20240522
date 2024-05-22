# Comparing `tmp/seam-0.7.1.tar.gz` & `tmp/seam-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seam-0.7.1.tar", max compression
+gzip compressed data, was "seam-0.8.0.tar", max compression
```

## Comparing `seam-0.7.1.tar` & `seam-0.8.0.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     1087 2024-05-20 16:46:52.747360 seam-0.7.1/LICENSE.txt
--rw-r--r--   0        0        0    10091 2024-05-20 16:46:52.747360 seam-0.7.1/README.rst
--rw-r--r--   0        0        0      726 2024-05-20 16:46:52.747360 seam-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      397 2024-05-20 16:46:52.747360 seam-0.7.1/seam/__init__.py
--rw-r--r--   0        0        0     4076 2024-05-20 16:46:52.747360 seam-0.7.1/seam/auth.py
--rw-r--r--   0        0        0       72 2024-05-20 16:46:52.747360 seam-0.7.1/seam/constants.py
--rw-r--r--   0        0        0     2018 2024-05-20 16:46:52.751360 seam-0.7.1/seam/options.py
--rw-r--r--   0        0        0      623 2024-05-20 16:46:52.751360 seam-0.7.1/seam/parse_options.py
--rw-r--r--   0        0        0     1337 2024-05-20 16:46:52.751360 seam-0.7.1/seam/request.py
--rw-r--r--   0        0        0    11981 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/access_codes.py
--rw-r--r--   0        0        0      915 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/access_codes_simulate.py
--rw-r--r--   0        0        0     3991 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/access_codes_unmanaged.py
--rw-r--r--   0        0        0     1824 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/acs.py
--rw-r--r--   0        0        0     2513 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/acs_access_groups.py
--rw-r--r--   0        0        0      730 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/acs_credential_pools.py
--rw-r--r--   0        0        0     1807 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/acs_credential_provisioning_automations.py
--rw-r--r--   0        0        0     4964 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/acs_credentials.py
--rw-r--r--   0        0        0     2180 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/acs_entrances.py
--rw-r--r--   0        0        0     1476 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/acs_systems.py
--rw-r--r--   0        0        0     6505 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/acs_users.py
--rw-r--r--   0        0        0     3982 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/action_attempts.py
--rw-r--r--   0        0        0     5780 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/client_sessions.py
--rw-r--r--   0        0        0     3321 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/connect_webviews.py
--rw-r--r--   0        0        0     2549 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/connected_accounts.py
--rw-r--r--   0        0        0     4804 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/devices.py
--rw-r--r--   0        0        0      546 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/devices_simulate.py
--rw-r--r--   0        0        0     3352 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/devices_unmanaged.py
--rw-r--r--   0        0        0     2414 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/events.py
--rw-r--r--   0        0        0     4210 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/locks.py
--rw-r--r--   0        0        0      794 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/networks.py
--rw-r--r--   0        0        0      757 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/noise_sensors.py
--rw-r--r--   0        0        0     4362 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/noise_sensors_noise_thresholds.py
--rw-r--r--   0        0        0      623 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/noise_sensors_simulate.py
--rw-r--r--   0        0        0     1099 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/phones.py
--rw-r--r--   0        0        0     1214 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/phones_simulate.py
--rw-r--r--   0        0        0     1436 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/routes.py
--rw-r--r--   0        0        0     8962 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/thermostats.py
--rw-r--r--   0        0        0     6955 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/thermostats_climate_setting_schedules.py
--rw-r--r--   0        0        0    64963 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/types.py
--rw-r--r--   0        0        0     6732 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/user_identities.py
--rw-r--r--   0        0        0     2928 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/user_identities_enrollment_automations.py
--rw-r--r--   0        0        0      864 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/utils/deep_attr_dict.py
--rw-r--r--   0        0        0     1844 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/webhooks.py
--rw-r--r--   0        0        0     2182 2024-05-20 16:46:52.751360 seam-0.7.1/seam/routes/workspaces.py
--rw-r--r--   0        0        0     2555 2024-05-20 16:46:52.751360 seam-0.7.1/seam/seam.py
--rw-r--r--   0        0        0     2418 2024-05-20 16:46:52.751360 seam-0.7.1/seam/seam_multi_workspace.py
--rw-r--r--   0        0        0     1027 2024-05-20 16:46:52.751360 seam-0.7.1/seam/token.py
--rw-r--r--   0        0        0     3242 2024-05-20 16:46:52.751360 seam-0.7.1/seam/types.py
--rw-r--r--   0        0        0    10841 1970-01-01 00:00:00.000000 seam-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1087 2024-05-22 14:09:41.498841 seam-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0    10091 2024-05-22 14:09:41.498841 seam-0.8.0/README.rst
+-rw-r--r--   0        0        0      725 2024-05-22 14:09:41.502841 seam-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      397 2024-05-22 14:09:41.502841 seam-0.8.0/seam/__init__.py
+-rw-r--r--   0        0        0     4076 2024-05-22 14:09:41.502841 seam-0.8.0/seam/auth.py
+-rw-r--r--   0        0        0     1184 2024-05-22 14:09:41.502841 seam-0.8.0/seam/client.py
+-rw-r--r--   0        0        0       72 2024-05-22 14:09:41.502841 seam-0.8.0/seam/constants.py
+-rw-r--r--   0        0        0     2018 2024-05-22 14:09:41.502841 seam-0.8.0/seam/options.py
+-rw-r--r--   0        0        0      623 2024-05-22 14:09:41.502841 seam-0.8.0/seam/parse_options.py
+-rw-r--r--   0        0        0    11865 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/access_codes.py
+-rw-r--r--   0        0        0      881 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/access_codes_simulate.py
+-rw-r--r--   0        0        0     3858 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/access_codes_unmanaged.py
+-rw-r--r--   0        0        0     1824 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/acs.py
+-rw-r--r--   0        0        0     2380 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/acs_access_groups.py
+-rw-r--r--   0        0        0      699 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/acs_credential_pools.py
+-rw-r--r--   0        0        0     1798 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/acs_credential_provisioning_automations.py
+-rw-r--r--   0        0        0     4879 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/acs_credentials.py
+-rw-r--r--   0        0        0     2144 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/acs_entrances.py
+-rw-r--r--   0        0        0     1437 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/acs_systems.py
+-rw-r--r--   0        0        0     6362 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/acs_users.py
+-rw-r--r--   0        0        0     3964 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/action_attempts.py
+-rw-r--r--   0        0        0     5651 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/client_sessions.py
+-rw-r--r--   0        0        0     3241 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/connect_webviews.py
+-rw-r--r--   0        0        0     2447 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/connected_accounts.py
+-rw-r--r--   0        0        0     4737 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/devices.py
+-rw-r--r--   0        0        0      537 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/devices_simulate.py
+-rw-r--r--   0        0        0     3281 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/devices_unmanaged.py
+-rw-r--r--   0        0        0     2396 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/events.py
+-rw-r--r--   0        0        0     4174 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/locks.py
+-rw-r--r--   0        0        0      776 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/networks.py
+-rw-r--r--   0        0        0      757 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/noise_sensors.py
+-rw-r--r--   0        0        0     4317 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/noise_sensors_noise_thresholds.py
+-rw-r--r--   0        0        0      614 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/noise_sensors_simulate.py
+-rw-r--r--   0        0        0     1081 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/phones.py
+-rw-r--r--   0        0        0     1205 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/phones_simulate.py
+-rw-r--r--   0        0        0     1436 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/routes.py
+-rw-r--r--   0        0        0     8846 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/thermostats.py
+-rw-r--r--   0        0        0     6910 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/thermostats_climate_setting_schedules.py
+-rw-r--r--   0        0        0    64963 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/types.py
+-rw-r--r--   0        0        0     6558 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/user_identities.py
+-rw-r--r--   0        0        0     2892 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/user_identities_enrollment_automations.py
+-rw-r--r--   0        0        0      864 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/utils/deep_attr_dict.py
+-rw-r--r--   0        0        0     1799 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/webhooks.py
+-rw-r--r--   0        0        0     2124 2024-05-22 14:09:41.502841 seam-0.8.0/seam/routes/workspaces.py
+-rw-r--r--   0        0        0     2583 2024-05-22 14:09:41.502841 seam-0.8.0/seam/seam.py
+-rw-r--r--   0        0        0     2545 2024-05-22 14:09:41.502841 seam-0.8.0/seam/seam_multi_workspace.py
+-rw-r--r--   0        0        0     1027 2024-05-22 14:09:41.502841 seam-0.8.0/seam/token.py
+-rw-r--r--   0        0        0     3487 2024-05-22 14:09:41.502841 seam-0.8.0/seam/types.py
+-rw-r--r--   0        0        0    10840 1970-01-01 00:00:00.000000 seam-0.8.0/PKG-INFO
```

### Comparing `seam-0.7.1/LICENSE.txt` & `seam-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `seam-0.7.1/README.rst` & `seam-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `seam-0.7.1/pyproject.toml` & `seam-0.8.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "seam"
-version = "0.7.1"
+version = "0.8.0"
 description = "SDK for the Seam API written in Python."
 authors = ["Seam Labs, Inc. <engineering@getseam.com>"]
 license = "MIT"
 readme = "README.rst"
 homepage = "https://github.com/seamapi/python-next"
 repository = "https://github.com/seamapi/python-next"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 dataclasses-json = "^0.6.4"
-requests = "^2.26.0"
+niquests = "^3.6.4"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 pylint = "^3.1.0"
 pytest = "^8.1.1"
 pytest-cov = "^5.0.0"
 pytest-runner = "^6.0.0"
```

### Comparing `seam-0.7.1/seam/auth.py` & `seam-0.8.0/seam/auth.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.1/seam/options.py` & `seam-0.8.0/seam/options.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.1/seam/parse_options.py` & `seam-0.8.0/seam/parse_options.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.1/seam/routes/access_codes.py` & `seam-0.8.0/seam/routes/access_codes.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         if sync is not None:
             json_payload["sync"] = sync
         if use_backup_access_code_pool is not None:
             json_payload["use_backup_access_code_pool"] = use_backup_access_code_pool
         if use_offline_access_code is not None:
             json_payload["use_offline_access_code"] = use_offline_access_code
 
-        res = self.seam.make_request("POST", "/access_codes/create", json=json_payload)
+        res = self.seam.client.post("/access_codes/create", json=json_payload)
 
         return AccessCode.from_dict(res["access_code"])
 
     def create_multiple(
         self,
         *,
         device_ids: List[str],
@@ -137,17 +137,15 @@
         if starts_at is not None:
             json_payload["starts_at"] = starts_at
         if use_backup_access_code_pool is not None:
             json_payload["use_backup_access_code_pool"] = use_backup_access_code_pool
         if use_offline_access_code is not None:
             json_payload["use_offline_access_code"] = use_offline_access_code
 
-        res = self.seam.make_request(
-            "POST", "/access_codes/create_multiple", json=json_payload
-        )
+        res = self.seam.client.post("/access_codes/create_multiple", json=json_payload)
 
         return [AccessCode.from_dict(item) for item in res["access_codes"]]
 
     def delete(
         self,
         *,
         access_code_id: str,
@@ -159,27 +157,25 @@
         if access_code_id is not None:
             json_payload["access_code_id"] = access_code_id
         if device_id is not None:
             json_payload["device_id"] = device_id
         if sync is not None:
             json_payload["sync"] = sync
 
-        self.seam.make_request("POST", "/access_codes/delete", json=json_payload)
+        self.seam.client.post("/access_codes/delete", json=json_payload)
 
         return None
 
     def generate_code(self, *, device_id: str) -> AccessCode:
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
 
-        res = self.seam.make_request(
-            "POST", "/access_codes/generate_code", json=json_payload
-        )
+        res = self.seam.client.post("/access_codes/generate_code", json=json_payload)
 
         return AccessCode.from_dict(res["generated_code"])
 
     def get(
         self,
         *,
         access_code_id: Optional[str] = None,
@@ -191,15 +187,15 @@
         if access_code_id is not None:
             json_payload["access_code_id"] = access_code_id
         if code is not None:
             json_payload["code"] = code
         if device_id is not None:
             json_payload["device_id"] = device_id
 
-        res = self.seam.make_request("POST", "/access_codes/get", json=json_payload)
+        res = self.seam.client.post("/access_codes/get", json=json_payload)
 
         return AccessCode.from_dict(res["access_code"])
 
     def list(
         self,
         *,
         access_code_ids: Optional[List[str]] = None,
@@ -211,26 +207,26 @@
         if access_code_ids is not None:
             json_payload["access_code_ids"] = access_code_ids
         if device_id is not None:
             json_payload["device_id"] = device_id
         if user_identifier_key is not None:
             json_payload["user_identifier_key"] = user_identifier_key
 
-        res = self.seam.make_request("POST", "/access_codes/list", json=json_payload)
+        res = self.seam.client.post("/access_codes/list", json=json_payload)
 
         return [AccessCode.from_dict(item) for item in res["access_codes"]]
 
     def pull_backup_access_code(self, *, access_code_id: str) -> AccessCode:
         json_payload = {}
 
         if access_code_id is not None:
             json_payload["access_code_id"] = access_code_id
 
-        res = self.seam.make_request(
-            "POST", "/access_codes/pull_backup_access_code", json=json_payload
+        res = self.seam.client.post(
+            "/access_codes/pull_backup_access_code", json=json_payload
         )
 
         return AccessCode.from_dict(res["backup_access_code"])
 
     def update(
         self,
         *,
@@ -290,10 +286,10 @@
         if type is not None:
             json_payload["type"] = type
         if use_backup_access_code_pool is not None:
             json_payload["use_backup_access_code_pool"] = use_backup_access_code_pool
         if use_offline_access_code is not None:
             json_payload["use_offline_access_code"] = use_offline_access_code
 
-        self.seam.make_request("POST", "/access_codes/update", json=json_payload)
+        self.seam.client.post("/access_codes/update", json=json_payload)
 
         return None
```

### Comparing `seam-0.7.1/seam/routes/access_codes_simulate.py` & `seam-0.8.0/seam/routes/access_codes_simulate.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,14 +17,12 @@
         if code is not None:
             json_payload["code"] = code
         if device_id is not None:
             json_payload["device_id"] = device_id
         if name is not None:
             json_payload["name"] = name
 
-        res = self.seam.make_request(
-            "POST",
-            "/access_codes/simulate/create_unmanaged_access_code",
-            json=json_payload,
+        res = self.seam.client.post(
+            "/access_codes/simulate/create_unmanaged_access_code", json=json_payload
         )
 
         return UnmanagedAccessCode.from_dict(res["access_code"])
```

### Comparing `seam-0.7.1/seam/routes/access_codes_unmanaged.py` & `seam-0.8.0/seam/routes/access_codes_unmanaged.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,31 +29,29 @@
         if is_external_modification_allowed is not None:
             json_payload["is_external_modification_allowed"] = (
                 is_external_modification_allowed
             )
         if sync is not None:
             json_payload["sync"] = sync
 
-        self.seam.make_request(
-            "POST", "/access_codes/unmanaged/convert_to_managed", json=json_payload
+        self.seam.client.post(
+            "/access_codes/unmanaged/convert_to_managed", json=json_payload
         )
 
         return None
 
     def delete(self, *, access_code_id: str, sync: Optional[bool] = None) -> None:
         json_payload = {}
 
         if access_code_id is not None:
             json_payload["access_code_id"] = access_code_id
         if sync is not None:
             json_payload["sync"] = sync
 
-        self.seam.make_request(
-            "POST", "/access_codes/unmanaged/delete", json=json_payload
-        )
+        self.seam.client.post("/access_codes/unmanaged/delete", json=json_payload)
 
         return None
 
     def get(
         self,
         *,
         access_code_id: Optional[str] = None,
@@ -65,33 +63,29 @@
         if access_code_id is not None:
             json_payload["access_code_id"] = access_code_id
         if code is not None:
             json_payload["code"] = code
         if device_id is not None:
             json_payload["device_id"] = device_id
 
-        res = self.seam.make_request(
-            "POST", "/access_codes/unmanaged/get", json=json_payload
-        )
+        res = self.seam.client.post("/access_codes/unmanaged/get", json=json_payload)
 
         return UnmanagedAccessCode.from_dict(res["access_code"])
 
     def list(
         self, *, device_id: str, user_identifier_key: Optional[str] = None
     ) -> List[UnmanagedAccessCode]:
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
         if user_identifier_key is not None:
             json_payload["user_identifier_key"] = user_identifier_key
 
-        res = self.seam.make_request(
-            "POST", "/access_codes/unmanaged/list", json=json_payload
-        )
+        res = self.seam.client.post("/access_codes/unmanaged/list", json=json_payload)
 
         return [UnmanagedAccessCode.from_dict(item) for item in res["access_codes"]]
 
     def update(
         self,
         *,
         access_code_id: str,
@@ -111,12 +105,10 @@
         if force is not None:
             json_payload["force"] = force
         if is_external_modification_allowed is not None:
             json_payload["is_external_modification_allowed"] = (
                 is_external_modification_allowed
             )
 
-        self.seam.make_request(
-            "POST", "/access_codes/unmanaged/update", json=json_payload
-        )
+        self.seam.client.post("/access_codes/unmanaged/update", json=json_payload)
 
         return None
```

### Comparing `seam-0.7.1/seam/routes/acs.py` & `seam-0.8.0/seam/routes/acs.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.1/seam/routes/acs_access_groups.py` & `seam-0.8.0/seam/routes/acs_access_groups.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,64 +13,56 @@
         json_payload = {}
 
         if acs_access_group_id is not None:
             json_payload["acs_access_group_id"] = acs_access_group_id
         if acs_user_id is not None:
             json_payload["acs_user_id"] = acs_user_id
 
-        self.seam.make_request("POST", "/acs/access_groups/add_user", json=json_payload)
+        self.seam.client.post("/acs/access_groups/add_user", json=json_payload)
 
         return None
 
     def get(self, *, acs_access_group_id: str) -> AcsAccessGroup:
         json_payload = {}
 
         if acs_access_group_id is not None:
             json_payload["acs_access_group_id"] = acs_access_group_id
 
-        res = self.seam.make_request(
-            "POST", "/acs/access_groups/get", json=json_payload
-        )
+        res = self.seam.client.post("/acs/access_groups/get", json=json_payload)
 
         return AcsAccessGroup.from_dict(res["acs_access_group"])
 
     def list(
         self, *, acs_system_id: Optional[str] = None, acs_user_id: Optional[str] = None
     ) -> List[AcsAccessGroup]:
         json_payload = {}
 
         if acs_system_id is not None:
             json_payload["acs_system_id"] = acs_system_id
         if acs_user_id is not None:
             json_payload["acs_user_id"] = acs_user_id
 
-        res = self.seam.make_request(
-            "POST", "/acs/access_groups/list", json=json_payload
-        )
+        res = self.seam.client.post("/acs/access_groups/list", json=json_payload)
 
         return [AcsAccessGroup.from_dict(item) for item in res["acs_access_groups"]]
 
     def list_users(self, *, acs_access_group_id: str) -> List[AcsUser]:
         json_payload = {}
 
         if acs_access_group_id is not None:
             json_payload["acs_access_group_id"] = acs_access_group_id
 
-        res = self.seam.make_request(
-            "POST", "/acs/access_groups/list_users", json=json_payload
-        )
+        res = self.seam.client.post("/acs/access_groups/list_users", json=json_payload)
 
         return [AcsUser.from_dict(item) for item in res["acs_users"]]
 
     def remove_user(self, *, acs_access_group_id: str, acs_user_id: str) -> None:
         json_payload = {}
 
         if acs_access_group_id is not None:
             json_payload["acs_access_group_id"] = acs_access_group_id
         if acs_user_id is not None:
             json_payload["acs_user_id"] = acs_user_id
 
-        self.seam.make_request(
-            "POST", "/acs/access_groups/remove_user", json=json_payload
-        )
+        self.seam.client.post("/acs/access_groups/remove_user", json=json_payload)
 
         return None
```

### Comparing `seam-0.7.1/seam/routes/acs_credential_pools.py` & `seam-0.8.0/seam/routes/acs_credential_pools.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,14 +11,12 @@
 
     def list(self, *, acs_system_id: str) -> List[AcsCredentialPool]:
         json_payload = {}
 
         if acs_system_id is not None:
             json_payload["acs_system_id"] = acs_system_id
 
-        res = self.seam.make_request(
-            "POST", "/acs/credential_pools/list", json=json_payload
-        )
+        res = self.seam.client.post("/acs/credential_pools/list", json=json_payload)
 
         return [
             AcsCredentialPool.from_dict(item) for item in res["acs_credential_pools"]
         ]
```

### Comparing `seam-0.7.1/seam/routes/acs_credential_provisioning_automations.py` & `seam-0.8.0/seam/routes/acs_credential_provisioning_automations.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,14 @@
                 create_credential_manager_user
             )
         if credential_manager_acs_user_id is not None:
             json_payload["credential_manager_acs_user_id"] = (
                 credential_manager_acs_user_id
             )
 
-        res = self.seam.make_request(
-            "POST", "/acs/credential_provisioning_automations/launch", json=json_payload
+        res = self.seam.client.post(
+            "/acs/credential_provisioning_automations/launch", json=json_payload
         )
 
         return AcsCredentialProvisioningAutomation.from_dict(
             res["acs_credential_provisioning_automation"]
         )
```

### Comparing `seam-0.7.1/seam/routes/acs_credentials.py` & `seam-0.8.0/seam/routes/acs_credentials.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         json_payload = {}
 
         if acs_credential_id is not None:
             json_payload["acs_credential_id"] = acs_credential_id
         if acs_user_id is not None:
             json_payload["acs_user_id"] = acs_user_id
 
-        self.seam.make_request("POST", "/acs/credentials/assign", json=json_payload)
+        self.seam.client.post("/acs/credentials/assign", json=json_payload)
 
         return None
 
     def create(
         self,
         *,
         access_method: str,
@@ -55,37 +55,35 @@
                 is_multi_phone_sync_credential
             )
         if starts_at is not None:
             json_payload["starts_at"] = starts_at
         if visionline_metadata is not None:
             json_payload["visionline_metadata"] = visionline_metadata
 
-        res = self.seam.make_request(
-            "POST", "/acs/credentials/create", json=json_payload
-        )
+        res = self.seam.client.post("/acs/credentials/create", json=json_payload)
 
         return AcsCredential.from_dict(res["acs_credential"])
 
     def delete(self, *, acs_credential_id: str) -> None:
         json_payload = {}
 
         if acs_credential_id is not None:
             json_payload["acs_credential_id"] = acs_credential_id
 
-        self.seam.make_request("POST", "/acs/credentials/delete", json=json_payload)
+        self.seam.client.post("/acs/credentials/delete", json=json_payload)
 
         return None
 
     def get(self, *, acs_credential_id: str) -> AcsCredential:
         json_payload = {}
 
         if acs_credential_id is not None:
             json_payload["acs_credential_id"] = acs_credential_id
 
-        res = self.seam.make_request("POST", "/acs/credentials/get", json=json_payload)
+        res = self.seam.client.post("/acs/credentials/get", json=json_payload)
 
         return AcsCredential.from_dict(res["acs_credential"])
 
     def list(
         self,
         *,
         acs_user_id: Optional[str] = None,
@@ -102,27 +100,27 @@
         if user_identity_id is not None:
             json_payload["user_identity_id"] = user_identity_id
         if is_multi_phone_sync_credential is not None:
             json_payload["is_multi_phone_sync_credential"] = (
                 is_multi_phone_sync_credential
             )
 
-        res = self.seam.make_request("POST", "/acs/credentials/list", json=json_payload)
+        res = self.seam.client.post("/acs/credentials/list", json=json_payload)
 
         return [AcsCredential.from_dict(item) for item in res["acs_credentials"]]
 
     def unassign(self, *, acs_credential_id: str, acs_user_id: str) -> None:
         json_payload = {}
 
         if acs_credential_id is not None:
             json_payload["acs_credential_id"] = acs_credential_id
         if acs_user_id is not None:
             json_payload["acs_user_id"] = acs_user_id
 
-        self.seam.make_request("POST", "/acs/credentials/unassign", json=json_payload)
+        self.seam.client.post("/acs/credentials/unassign", json=json_payload)
 
         return None
 
     def update(
         self,
         *,
         acs_credential_id: str,
@@ -134,10 +132,10 @@
         if acs_credential_id is not None:
             json_payload["acs_credential_id"] = acs_credential_id
         if code is not None:
             json_payload["code"] = code
         if ends_at is not None:
             json_payload["ends_at"] = ends_at
 
-        self.seam.make_request("POST", "/acs/credentials/update", json=json_payload)
+        self.seam.client.post("/acs/credentials/update", json=json_payload)
 
         return None
```

### Comparing `seam-0.7.1/seam/routes/acs_entrances.py` & `seam-0.8.0/seam/routes/acs_entrances.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 
     def get(self, *, acs_entrance_id: str) -> AcsEntrance:
         json_payload = {}
 
         if acs_entrance_id is not None:
             json_payload["acs_entrance_id"] = acs_entrance_id
 
-        res = self.seam.make_request("POST", "/acs/entrances/get", json=json_payload)
+        res = self.seam.client.post("/acs/entrances/get", json=json_payload)
 
         return AcsEntrance.from_dict(res["acs_entrance"])
 
     def grant_access(self, *, acs_entrance_id: str, acs_user_id: str) -> None:
         json_payload = {}
 
         if acs_entrance_id is not None:
             json_payload["acs_entrance_id"] = acs_entrance_id
         if acs_user_id is not None:
             json_payload["acs_user_id"] = acs_user_id
 
-        self.seam.make_request("POST", "/acs/entrances/grant_access", json=json_payload)
+        self.seam.client.post("/acs/entrances/grant_access", json=json_payload)
 
         return None
 
     def list(
         self,
         *,
         acs_credential_id: Optional[str] = None,
@@ -40,26 +40,26 @@
         json_payload = {}
 
         if acs_credential_id is not None:
             json_payload["acs_credential_id"] = acs_credential_id
         if acs_system_id is not None:
             json_payload["acs_system_id"] = acs_system_id
 
-        res = self.seam.make_request("POST", "/acs/entrances/list", json=json_payload)
+        res = self.seam.client.post("/acs/entrances/list", json=json_payload)
 
         return [AcsEntrance.from_dict(item) for item in res["acs_entrances"]]
 
     def list_credentials_with_access(
         self, *, acs_entrance_id: str, include_if: Optional[List[str]] = None
     ) -> List[AcsCredential]:
         json_payload = {}
 
         if acs_entrance_id is not None:
             json_payload["acs_entrance_id"] = acs_entrance_id
         if include_if is not None:
             json_payload["include_if"] = include_if
 
-        res = self.seam.make_request(
-            "POST", "/acs/entrances/list_credentials_with_access", json=json_payload
+        res = self.seam.client.post(
+            "/acs/entrances/list_credentials_with_access", json=json_payload
         )
 
         return [AcsCredential.from_dict(item) for item in res["acs_credentials"]]
```

### Comparing `seam-0.7.1/seam/routes/acs_systems.py` & `seam-0.8.0/seam/routes/acs_systems.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,36 +11,35 @@
 
     def get(self, *, acs_system_id: str) -> AcsSystem:
         json_payload = {}
 
         if acs_system_id is not None:
             json_payload["acs_system_id"] = acs_system_id
 
-        res = self.seam.make_request("POST", "/acs/systems/get", json=json_payload)
+        res = self.seam.client.post("/acs/systems/get", json=json_payload)
 
         return AcsSystem.from_dict(res["acs_system"])
 
     def list(self, *, connected_account_id: Optional[str] = None) -> List[AcsSystem]:
         json_payload = {}
 
         if connected_account_id is not None:
             json_payload["connected_account_id"] = connected_account_id
 
-        res = self.seam.make_request("POST", "/acs/systems/list", json=json_payload)
+        res = self.seam.client.post("/acs/systems/list", json=json_payload)
 
         return [AcsSystem.from_dict(item) for item in res["acs_systems"]]
 
     def list_compatible_credential_manager_acs_systems(
         self, *, acs_system_id: str
     ) -> List[AcsSystem]:
         json_payload = {}
 
         if acs_system_id is not None:
             json_payload["acs_system_id"] = acs_system_id
 
-        res = self.seam.make_request(
-            "POST",
+        res = self.seam.client.post(
             "/acs/systems/list_compatible_credential_manager_acs_systems",
             json=json_payload,
         )
 
         return [AcsSystem.from_dict(item) for item in res["acs_systems"]]
```

### Comparing `seam-0.7.1/seam/routes/acs_users.py` & `seam-0.8.0/seam/routes/acs_users.py`

 * *Files 11% similar despite different names*

```diff
@@ -15,17 +15,15 @@
         json_payload = {}
 
         if acs_access_group_id is not None:
             json_payload["acs_access_group_id"] = acs_access_group_id
         if acs_user_id is not None:
             json_payload["acs_user_id"] = acs_user_id
 
-        self.seam.make_request(
-            "POST", "/acs/users/add_to_access_group", json=json_payload
-        )
+        self.seam.client.post("/acs/users/add_to_access_group", json=json_payload)
 
         return None
 
     def create(
         self,
         *,
         acs_system_id: str,
@@ -52,35 +50,35 @@
         if full_name is not None:
             json_payload["full_name"] = full_name
         if phone_number is not None:
             json_payload["phone_number"] = phone_number
         if user_identity_id is not None:
             json_payload["user_identity_id"] = user_identity_id
 
-        res = self.seam.make_request("POST", "/acs/users/create", json=json_payload)
+        res = self.seam.client.post("/acs/users/create", json=json_payload)
 
         return AcsUser.from_dict(res["acs_user"])
 
     def delete(self, *, acs_user_id: str) -> None:
         json_payload = {}
 
         if acs_user_id is not None:
             json_payload["acs_user_id"] = acs_user_id
 
-        self.seam.make_request("POST", "/acs/users/delete", json=json_payload)
+        self.seam.client.post("/acs/users/delete", json=json_payload)
 
         return None
 
     def get(self, *, acs_user_id: str) -> AcsUser:
         json_payload = {}
 
         if acs_user_id is not None:
             json_payload["acs_user_id"] = acs_user_id
 
-        res = self.seam.make_request("POST", "/acs/users/get", json=json_payload)
+        res = self.seam.client.post("/acs/users/get", json=json_payload)
 
         return AcsUser.from_dict(res["acs_user"])
 
     def list(
         self,
         *,
         acs_system_id: Optional[str] = None,
@@ -95,75 +93,73 @@
         if user_identity_email_address is not None:
             json_payload["user_identity_email_address"] = user_identity_email_address
         if user_identity_id is not None:
             json_payload["user_identity_id"] = user_identity_id
         if user_identity_phone_number is not None:
             json_payload["user_identity_phone_number"] = user_identity_phone_number
 
-        res = self.seam.make_request("POST", "/acs/users/list", json=json_payload)
+        res = self.seam.client.post("/acs/users/list", json=json_payload)
 
         return [AcsUser.from_dict(item) for item in res["acs_users"]]
 
     def list_accessible_entrances(self, *, acs_user_id: str) -> List[AcsEntrance]:
         json_payload = {}
 
         if acs_user_id is not None:
             json_payload["acs_user_id"] = acs_user_id
 
-        res = self.seam.make_request(
-            "POST", "/acs/users/list_accessible_entrances", json=json_payload
+        res = self.seam.client.post(
+            "/acs/users/list_accessible_entrances", json=json_payload
         )
 
         return [AcsEntrance.from_dict(item) for item in res["acs_entrances"]]
 
     def remove_from_access_group(
         self, *, acs_access_group_id: str, acs_user_id: str
     ) -> None:
         json_payload = {}
 
         if acs_access_group_id is not None:
             json_payload["acs_access_group_id"] = acs_access_group_id
         if acs_user_id is not None:
             json_payload["acs_user_id"] = acs_user_id
 
-        self.seam.make_request(
-            "POST", "/acs/users/remove_from_access_group", json=json_payload
-        )
+        self.seam.client.post("/acs/users/remove_from_access_group", json=json_payload)
 
         return None
 
     def revoke_access_to_all_entrances(self, *, acs_user_id: str) -> None:
         json_payload = {}
 
         if acs_user_id is not None:
             json_payload["acs_user_id"] = acs_user_id
 
-        self.seam.make_request(
-            "POST", "/acs/users/revoke_access_to_all_entrances", json=json_payload
+        self.seam.client.post(
+            "/acs/users/revoke_access_to_all_entrances", json=json_payload
         )
 
         return None
 
     def suspend(self, *, acs_user_id: str) -> None:
         json_payload = {}
 
         if acs_user_id is not None:
             json_payload["acs_user_id"] = acs_user_id
 
-        self.seam.make_request("POST", "/acs/users/suspend", json=json_payload)
+        self.seam.client.post("/acs/users/suspend", json=json_payload)
 
         return None
 
     def unsuspend(self, *, acs_user_id: str) -> None:
         json_payload = {}
 
         if acs_user_id is not None:
             json_payload["acs_user_id"] = acs_user_id
 
-        self.seam.make_request("POST", "/acs/users/unsuspend", json=json_payload)
+        self.seam.client.post("/acs/users/unsuspend", json=json_payload)
 
         return None
 
     def update(
         self,
         *,
         acs_user_id: str,
@@ -187,10 +183,10 @@
         if full_name is not None:
             json_payload["full_name"] = full_name
         if hid_acs_system_id is not None:
             json_payload["hid_acs_system_id"] = hid_acs_system_id
         if phone_number is not None:
             json_payload["phone_number"] = phone_number
 
-        self.seam.make_request("POST", "/acs/users/update", json=json_payload)
+        self.seam.client.post("/acs/users/update", json=json_payload)
 
         return None
```

### Comparing `seam-0.7.1/seam/routes/action_attempts.py` & `seam-0.8.0/seam/routes/action_attempts.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,28 +39,28 @@
         wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None,
     ) -> ActionAttempt:
         json_payload = {}
 
         if action_attempt_id is not None:
             json_payload["action_attempt_id"] = action_attempt_id
 
-        res = self.seam.make_request("POST", "/action_attempts/get", json=json_payload)
+        res = self.seam.client.post("/action_attempts/get", json=json_payload)
 
         return self.seam.action_attempts.decide_and_wait(
             action_attempt=ActionAttempt.from_dict(res["action_attempt"]),
             wait_for_action_attempt=wait_for_action_attempt,
         )
 
     def list(self, *, action_attempt_ids: List[str]) -> List[ActionAttempt]:
         json_payload = {}
 
         if action_attempt_ids is not None:
             json_payload["action_attempt_ids"] = action_attempt_ids
 
-        res = self.seam.make_request("POST", "/action_attempts/list", json=json_payload)
+        res = self.seam.client.post("/action_attempts/list", json=json_payload)
 
         return [ActionAttempt.from_dict(item) for item in res["action_attempts"]]
 
     def poll_until_ready(
         self,
         *,
         action_attempt_id: str,
```

### Comparing `seam-0.7.1/seam/routes/client_sessions.py` & `seam-0.8.0/seam/routes/client_sessions.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,27 +27,25 @@
         if expires_at is not None:
             json_payload["expires_at"] = expires_at
         if user_identifier_key is not None:
             json_payload["user_identifier_key"] = user_identifier_key
         if user_identity_ids is not None:
             json_payload["user_identity_ids"] = user_identity_ids
 
-        res = self.seam.make_request(
-            "POST", "/client_sessions/create", json=json_payload
-        )
+        res = self.seam.client.post("/client_sessions/create", json=json_payload)
 
         return ClientSession.from_dict(res["client_session"])
 
     def delete(self, *, client_session_id: str) -> None:
         json_payload = {}
 
         if client_session_id is not None:
             json_payload["client_session_id"] = client_session_id
 
-        self.seam.make_request("POST", "/client_sessions/delete", json=json_payload)
+        self.seam.client.post("/client_sessions/delete", json=json_payload)
 
         return None
 
     def get(
         self,
         *,
         client_session_id: Optional[str] = None,
@@ -56,15 +54,15 @@
         json_payload = {}
 
         if client_session_id is not None:
             json_payload["client_session_id"] = client_session_id
         if user_identifier_key is not None:
             json_payload["user_identifier_key"] = user_identifier_key
 
-        res = self.seam.make_request("POST", "/client_sessions/get", json=json_payload)
+        res = self.seam.client.post("/client_sessions/get", json=json_payload)
 
         return ClientSession.from_dict(res["client_session"])
 
     def get_or_create(
         self,
         *,
         connect_webview_ids: Optional[List[str]] = None,
@@ -82,17 +80,15 @@
         if expires_at is not None:
             json_payload["expires_at"] = expires_at
         if user_identifier_key is not None:
             json_payload["user_identifier_key"] = user_identifier_key
         if user_identity_ids is not None:
             json_payload["user_identity_ids"] = user_identity_ids
 
-        res = self.seam.make_request(
-            "POST", "/client_sessions/get_or_create", json=json_payload
-        )
+        res = self.seam.client.post("/client_sessions/get_or_create", json=json_payload)
 
         return ClientSession.from_dict(res["client_session"])
 
     def grant_access(
         self,
         *,
         client_session_id: Optional[str] = None,
@@ -110,17 +106,15 @@
         if connected_account_ids is not None:
             json_payload["connected_account_ids"] = connected_account_ids
         if user_identifier_key is not None:
             json_payload["user_identifier_key"] = user_identifier_key
         if user_identity_ids is not None:
             json_payload["user_identity_ids"] = user_identity_ids
 
-        self.seam.make_request(
-            "POST", "/client_sessions/grant_access", json=json_payload
-        )
+        self.seam.client.post("/client_sessions/grant_access", json=json_payload)
 
         return None
 
     def list(
         self,
         *,
         client_session_id: Optional[str] = None,
@@ -138,20 +132,20 @@
         if user_identifier_key is not None:
             json_payload["user_identifier_key"] = user_identifier_key
         if user_identity_id is not None:
             json_payload["user_identity_id"] = user_identity_id
         if without_user_identifier_key is not None:
             json_payload["without_user_identifier_key"] = without_user_identifier_key
 
-        res = self.seam.make_request("POST", "/client_sessions/list", json=json_payload)
+        res = self.seam.client.post("/client_sessions/list", json=json_payload)
 
         return [ClientSession.from_dict(item) for item in res["client_sessions"]]
 
     def revoke(self, *, client_session_id: str) -> None:
         json_payload = {}
 
         if client_session_id is not None:
             json_payload["client_session_id"] = client_session_id
 
-        self.seam.make_request("POST", "/client_sessions/revoke", json=json_payload)
+        self.seam.client.post("/client_sessions/revoke", json=json_payload)
 
         return None
```

### Comparing `seam-0.7.1/seam/routes/connect_webviews.py` & `seam-0.8.0/seam/routes/connect_webviews.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,37 +38,35 @@
         if device_selection_mode is not None:
             json_payload["device_selection_mode"] = device_selection_mode
         if provider_category is not None:
             json_payload["provider_category"] = provider_category
         if wait_for_device_creation is not None:
             json_payload["wait_for_device_creation"] = wait_for_device_creation
 
-        res = self.seam.make_request(
-            "POST", "/connect_webviews/create", json=json_payload
-        )
+        res = self.seam.client.post("/connect_webviews/create", json=json_payload)
 
         return ConnectWebview.from_dict(res["connect_webview"])
 
     def delete(self, *, connect_webview_id: str) -> None:
         json_payload = {}
 
         if connect_webview_id is not None:
             json_payload["connect_webview_id"] = connect_webview_id
 
-        self.seam.make_request("POST", "/connect_webviews/delete", json=json_payload)
+        self.seam.client.post("/connect_webviews/delete", json=json_payload)
 
         return None
 
     def get(self, *, connect_webview_id: str) -> ConnectWebview:
         json_payload = {}
 
         if connect_webview_id is not None:
             json_payload["connect_webview_id"] = connect_webview_id
 
-        res = self.seam.make_request("POST", "/connect_webviews/get", json=json_payload)
+        res = self.seam.client.post("/connect_webviews/get", json=json_payload)
 
         return ConnectWebview.from_dict(res["connect_webview"])
 
     def list(
         self,
         *,
         custom_metadata_has: Optional[Dict[str, Any]] = None,
@@ -77,12 +75,10 @@
         json_payload = {}
 
         if custom_metadata_has is not None:
             json_payload["custom_metadata_has"] = custom_metadata_has
         if user_identifier_key is not None:
             json_payload["user_identifier_key"] = user_identifier_key
 
-        res = self.seam.make_request(
-            "POST", "/connect_webviews/list", json=json_payload
-        )
+        res = self.seam.client.post("/connect_webviews/list", json=json_payload)
 
         return [ConnectWebview.from_dict(item) for item in res["connect_webviews"]]
```

### Comparing `seam-0.7.1/seam/routes/connected_accounts.py` & `seam-0.8.0/seam/routes/connected_accounts.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,45 +13,41 @@
         json_payload = {}
 
         if connected_account_id is not None:
             json_payload["connected_account_id"] = connected_account_id
         if sync is not None:
             json_payload["sync"] = sync
 
-        self.seam.make_request("POST", "/connected_accounts/delete", json=json_payload)
+        self.seam.client.post("/connected_accounts/delete", json=json_payload)
 
         return None
 
     def get(
         self, *, connected_account_id: Optional[str] = None, email: Optional[str] = None
     ) -> ConnectedAccount:
         json_payload = {}
 
         if connected_account_id is not None:
             json_payload["connected_account_id"] = connected_account_id
         if email is not None:
             json_payload["email"] = email
 
-        res = self.seam.make_request(
-            "POST", "/connected_accounts/get", json=json_payload
-        )
+        res = self.seam.client.post("/connected_accounts/get", json=json_payload)
 
         return ConnectedAccount.from_dict(res["connected_account"])
 
     def list(
         self, *, custom_metadata_has: Optional[Dict[str, Any]] = None
     ) -> List[ConnectedAccount]:
         json_payload = {}
 
         if custom_metadata_has is not None:
             json_payload["custom_metadata_has"] = custom_metadata_has
 
-        res = self.seam.make_request(
-            "POST", "/connected_accounts/list", json=json_payload
-        )
+        res = self.seam.client.post("/connected_accounts/list", json=json_payload)
 
         return [ConnectedAccount.from_dict(item) for item in res["connected_accounts"]]
 
     def update(
         self,
         *,
         connected_account_id: str,
@@ -65,12 +61,10 @@
         if automatically_manage_new_devices is not None:
             json_payload["automatically_manage_new_devices"] = (
                 automatically_manage_new_devices
             )
         if custom_metadata is not None:
             json_payload["custom_metadata"] = custom_metadata
 
-        res = self.seam.make_request(
-            "POST", "/connected_accounts/update", json=json_payload
-        )
+        res = self.seam.client.post("/connected_accounts/update", json=json_payload)
 
         return ConnectedAccount.from_dict(res["connected_account"])
```

### Comparing `seam-0.7.1/seam/routes/devices.py` & `seam-0.8.0/seam/routes/devices.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,29 +23,29 @@
 
     def delete(self, *, device_id: str) -> None:
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
 
-        self.seam.make_request("POST", "/devices/delete", json=json_payload)
+        self.seam.client.post("/devices/delete", json=json_payload)
 
         return None
 
     def get(
         self, *, device_id: Optional[str] = None, name: Optional[str] = None
     ) -> Device:
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
         if name is not None:
             json_payload["name"] = name
 
-        res = self.seam.make_request("POST", "/devices/get", json=json_payload)
+        res = self.seam.client.post("/devices/get", json=json_payload)
 
         return Device.from_dict(res["device"])
 
     def list(
         self,
         *,
         connect_webview_id: Optional[str] = None,
@@ -87,29 +87,27 @@
         if limit is not None:
             json_payload["limit"] = limit
         if manufacturer is not None:
             json_payload["manufacturer"] = manufacturer
         if user_identifier_key is not None:
             json_payload["user_identifier_key"] = user_identifier_key
 
-        res = self.seam.make_request("POST", "/devices/list", json=json_payload)
+        res = self.seam.client.post("/devices/list", json=json_payload)
 
         return [Device.from_dict(item) for item in res["devices"]]
 
     def list_device_providers(
         self, *, provider_category: Optional[str] = None
     ) -> List[DeviceProvider]:
         json_payload = {}
 
         if provider_category is not None:
             json_payload["provider_category"] = provider_category
 
-        res = self.seam.make_request(
-            "POST", "/devices/list_device_providers", json=json_payload
-        )
+        res = self.seam.client.post("/devices/list_device_providers", json=json_payload)
 
         return [DeviceProvider.from_dict(item) for item in res["device_providers"]]
 
     def update(
         self,
         *,
         device_id: str,
@@ -127,10 +125,10 @@
         if is_managed is not None:
             json_payload["is_managed"] = is_managed
         if name is not None:
             json_payload["name"] = name
         if properties is not None:
             json_payload["properties"] = properties
 
-        self.seam.make_request("POST", "/devices/update", json=json_payload)
+        self.seam.client.post("/devices/update", json=json_payload)
 
         return None
```

### Comparing `seam-0.7.1/seam/routes/devices_simulate.py` & `seam-0.8.0/seam/routes/noise_sensors_simulate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from seam.types import AbstractSeam as Seam
-from seam.routes.types import AbstractDevicesSimulate
+from seam.routes.types import AbstractNoiseSensorsSimulate
 from typing import Optional, Any, List, Dict, Union
 
 
-class DevicesSimulate(AbstractDevicesSimulate):
+class NoiseSensorsSimulate(AbstractNoiseSensorsSimulate):
     seam: Seam
 
     def __init__(self, seam: Seam):
         self.seam = seam
 
-    def remove(self, *, device_id: str) -> None:
+    def trigger_noise_threshold(self, *, device_id: str) -> None:
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
 
-        self.seam.make_request("POST", "/devices/simulate/remove", json=json_payload)
+        self.seam.client.post(
+            "/noise_sensors/simulate/trigger_noise_threshold", json=json_payload
+        )
 
         return None
```

### Comparing `seam-0.7.1/seam/routes/devices_unmanaged.py` & `seam-0.8.0/seam/routes/devices_unmanaged.py`

 * *Files 15% similar despite different names*

```diff
@@ -15,17 +15,15 @@
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
         if name is not None:
             json_payload["name"] = name
 
-        res = self.seam.make_request(
-            "POST", "/devices/unmanaged/get", json=json_payload
-        )
+        res = self.seam.client.post("/devices/unmanaged/get", json=json_payload)
 
         return UnmanagedDevice.from_dict(res["device"])
 
     def list(
         self,
         *,
         connect_webview_id: Optional[str] = None,
@@ -67,24 +65,22 @@
         if limit is not None:
             json_payload["limit"] = limit
         if manufacturer is not None:
             json_payload["manufacturer"] = manufacturer
         if user_identifier_key is not None:
             json_payload["user_identifier_key"] = user_identifier_key
 
-        res = self.seam.make_request(
-            "POST", "/devices/unmanaged/list", json=json_payload
-        )
+        res = self.seam.client.post("/devices/unmanaged/list", json=json_payload)
 
         return [UnmanagedDevice.from_dict(item) for item in res["devices"]]
 
     def update(self, *, device_id: str, is_managed: bool) -> None:
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
         if is_managed is not None:
             json_payload["is_managed"] = is_managed
 
-        self.seam.make_request("POST", "/devices/unmanaged/update", json=json_payload)
+        self.seam.client.post("/devices/unmanaged/update", json=json_payload)
 
         return None
```

### Comparing `seam-0.7.1/seam/routes/events.py` & `seam-0.8.0/seam/routes/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         if device_id is not None:
             json_payload["device_id"] = device_id
         if event_id is not None:
             json_payload["event_id"] = event_id
         if event_type is not None:
             json_payload["event_type"] = event_type
 
-        res = self.seam.make_request("POST", "/events/get", json=json_payload)
+        res = self.seam.client.post("/events/get", json=json_payload)
 
         return Event.from_dict(res["event"])
 
     def list(
         self,
         *,
         access_code_id: Optional[str] = None,
@@ -62,10 +62,10 @@
         if event_types is not None:
             json_payload["event_types"] = event_types
         if limit is not None:
             json_payload["limit"] = limit
         if since is not None:
             json_payload["since"] = since
 
-        res = self.seam.make_request("POST", "/events/list", json=json_payload)
+        res = self.seam.client.post("/events/list", json=json_payload)
 
         return [Event.from_dict(item) for item in res["events"]]
```

### Comparing `seam-0.7.1/seam/routes/locks.py` & `seam-0.8.0/seam/routes/locks.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
         if name is not None:
             json_payload["name"] = name
 
-        res = self.seam.make_request("POST", "/locks/get", json=json_payload)
+        res = self.seam.client.post("/locks/get", json=json_payload)
 
         return Device.from_dict(res["device"])
 
     def list(
         self,
         *,
         connect_webview_id: Optional[str] = None,
@@ -65,15 +65,15 @@
         if limit is not None:
             json_payload["limit"] = limit
         if manufacturer is not None:
             json_payload["manufacturer"] = manufacturer
         if user_identifier_key is not None:
             json_payload["user_identifier_key"] = user_identifier_key
 
-        res = self.seam.make_request("POST", "/locks/list", json=json_payload)
+        res = self.seam.client.post("/locks/list", json=json_payload)
 
         return [Device.from_dict(item) for item in res["devices"]]
 
     def lock_door(
         self,
         *,
         device_id: str,
@@ -83,15 +83,15 @@
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
         if sync is not None:
             json_payload["sync"] = sync
 
-        res = self.seam.make_request("POST", "/locks/lock_door", json=json_payload)
+        res = self.seam.client.post("/locks/lock_door", json=json_payload)
 
         return self.seam.action_attempts.decide_and_wait(
             action_attempt=ActionAttempt.from_dict(res["action_attempt"]),
             wait_for_action_attempt=wait_for_action_attempt,
         )
 
     def unlock_door(
@@ -104,13 +104,13 @@
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
         if sync is not None:
             json_payload["sync"] = sync
 
-        res = self.seam.make_request("POST", "/locks/unlock_door", json=json_payload)
+        res = self.seam.client.post("/locks/unlock_door", json=json_payload)
 
         return self.seam.action_attempts.decide_and_wait(
             action_attempt=ActionAttempt.from_dict(res["action_attempt"]),
             wait_for_action_attempt=wait_for_action_attempt,
         )
```

### Comparing `seam-0.7.1/seam/routes/networks.py` & `seam-0.8.0/seam/routes/networks.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,19 +11,19 @@
 
     def get(self, *, network_id: str) -> Network:
         json_payload = {}
 
         if network_id is not None:
             json_payload["network_id"] = network_id
 
-        res = self.seam.make_request("POST", "/networks/get", json=json_payload)
+        res = self.seam.client.post("/networks/get", json=json_payload)
 
         return Network.from_dict(res["network"])
 
     def list(
         self,
     ) -> List[Network]:
         json_payload = {}
 
-        res = self.seam.make_request("POST", "/networks/list", json=json_payload)
+        res = self.seam.client.post("/networks/list", json=json_payload)
 
         return [Network.from_dict(item) for item in res["networks"]]
```

### Comparing `seam-0.7.1/seam/routes/noise_sensors.py` & `seam-0.8.0/seam/routes/noise_sensors.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.1/seam/routes/noise_sensors_noise_thresholds.py` & `seam-0.8.0/seam/routes/noise_sensors_noise_thresholds.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         if noise_threshold_decibels is not None:
             json_payload["noise_threshold_decibels"] = noise_threshold_decibels
         if noise_threshold_nrs is not None:
             json_payload["noise_threshold_nrs"] = noise_threshold_nrs
         if sync is not None:
             json_payload["sync"] = sync
 
-        res = self.seam.make_request(
-            "POST", "/noise_sensors/noise_thresholds/create", json=json_payload
+        res = self.seam.client.post(
+            "/noise_sensors/noise_thresholds/create", json=json_payload
         )
 
         return NoiseThreshold.from_dict(res["noise_threshold"])
 
     def delete(
         self, *, device_id: str, noise_threshold_id: str, sync: Optional[bool] = None
     ) -> None:
@@ -51,44 +51,44 @@
         if device_id is not None:
             json_payload["device_id"] = device_id
         if noise_threshold_id is not None:
             json_payload["noise_threshold_id"] = noise_threshold_id
         if sync is not None:
             json_payload["sync"] = sync
 
-        self.seam.make_request(
-            "POST", "/noise_sensors/noise_thresholds/delete", json=json_payload
+        self.seam.client.post(
+            "/noise_sensors/noise_thresholds/delete", json=json_payload
         )
 
         return None
 
     def get(self, *, noise_threshold_id: str) -> NoiseThreshold:
         json_payload = {}
 
         if noise_threshold_id is not None:
             json_payload["noise_threshold_id"] = noise_threshold_id
 
-        res = self.seam.make_request(
-            "POST", "/noise_sensors/noise_thresholds/get", json=json_payload
+        res = self.seam.client.post(
+            "/noise_sensors/noise_thresholds/get", json=json_payload
         )
 
         return NoiseThreshold.from_dict(res["noise_threshold"])
 
     def list(
         self, *, device_id: str, is_programmed: Optional[bool] = None
     ) -> List[NoiseThreshold]:
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
         if is_programmed is not None:
             json_payload["is_programmed"] = is_programmed
 
-        res = self.seam.make_request(
-            "POST", "/noise_sensors/noise_thresholds/list", json=json_payload
+        res = self.seam.client.post(
+            "/noise_sensors/noise_thresholds/list", json=json_payload
         )
 
         return [NoiseThreshold.from_dict(item) for item in res["noise_thresholds"]]
 
     def update(
         self,
         *,
@@ -116,12 +116,12 @@
         if noise_threshold_nrs is not None:
             json_payload["noise_threshold_nrs"] = noise_threshold_nrs
         if starts_daily_at is not None:
             json_payload["starts_daily_at"] = starts_daily_at
         if sync is not None:
             json_payload["sync"] = sync
 
-        self.seam.make_request(
-            "POST", "/noise_sensors/noise_thresholds/update", json=json_payload
+        self.seam.client.post(
+            "/noise_sensors/noise_thresholds/update", json=json_payload
         )
 
         return None
```

### Comparing `seam-0.7.1/seam/routes/noise_sensors_simulate.py` & `seam-0.8.0/seam/routes/devices_simulate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from seam.types import AbstractSeam as Seam
-from seam.routes.types import AbstractNoiseSensorsSimulate
+from seam.routes.types import AbstractDevicesSimulate
 from typing import Optional, Any, List, Dict, Union
 
 
-class NoiseSensorsSimulate(AbstractNoiseSensorsSimulate):
+class DevicesSimulate(AbstractDevicesSimulate):
     seam: Seam
 
     def __init__(self, seam: Seam):
         self.seam = seam
 
-    def trigger_noise_threshold(self, *, device_id: str) -> None:
+    def remove(self, *, device_id: str) -> None:
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
 
-        self.seam.make_request(
-            "POST", "/noise_sensors/simulate/trigger_noise_threshold", json=json_payload
-        )
+        self.seam.client.post("/devices/simulate/remove", json=json_payload)
 
         return None
```

### Comparing `seam-0.7.1/seam/routes/phones.py` & `seam-0.8.0/seam/routes/phones.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 
     def deactivate(self, *, device_id: str) -> None:
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
 
-        self.seam.make_request("POST", "/phones/deactivate", json=json_payload)
+        self.seam.client.post("/phones/deactivate", json=json_payload)
 
         return None
 
     def list(self, *, owner_user_identity_id: Optional[str] = None) -> List[Phone]:
         json_payload = {}
 
         if owner_user_identity_id is not None:
             json_payload["owner_user_identity_id"] = owner_user_identity_id
 
-        res = self.seam.make_request("POST", "/phones/list", json=json_payload)
+        res = self.seam.client.post("/phones/list", json=json_payload)
 
         return [Phone.from_dict(item) for item in res["phones"]]
```

### Comparing `seam-0.7.1/seam/routes/phones_simulate.py` & `seam-0.8.0/seam/routes/phones_simulate.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,12 +24,12 @@
         if assa_abloy_metadata is not None:
             json_payload["assa_abloy_metadata"] = assa_abloy_metadata
         if custom_sdk_installation_id is not None:
             json_payload["custom_sdk_installation_id"] = custom_sdk_installation_id
         if phone_metadata is not None:
             json_payload["phone_metadata"] = phone_metadata
 
-        res = self.seam.make_request(
-            "POST", "/phones/simulate/create_sandbox_phone", json=json_payload
+        res = self.seam.client.post(
+            "/phones/simulate/create_sandbox_phone", json=json_payload
         )
 
         return Phone.from_dict(res["phone"])
```

### Comparing `seam-0.7.1/seam/routes/routes.py` & `seam-0.8.0/seam/routes/routes.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.1/seam/routes/thermostats.py` & `seam-0.8.0/seam/routes/thermostats.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         if cooling_set_point_celsius is not None:
             json_payload["cooling_set_point_celsius"] = cooling_set_point_celsius
         if cooling_set_point_fahrenheit is not None:
             json_payload["cooling_set_point_fahrenheit"] = cooling_set_point_fahrenheit
         if sync is not None:
             json_payload["sync"] = sync
 
-        res = self.seam.make_request("POST", "/thermostats/cool", json=json_payload)
+        res = self.seam.client.post("/thermostats/cool", json=json_payload)
 
         return self.seam.action_attempts.decide_and_wait(
             action_attempt=ActionAttempt.from_dict(res["action_attempt"]),
             wait_for_action_attempt=wait_for_action_attempt,
         )
 
     def get(
@@ -50,15 +50,15 @@
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
         if name is not None:
             json_payload["name"] = name
 
-        res = self.seam.make_request("POST", "/thermostats/get", json=json_payload)
+        res = self.seam.client.post("/thermostats/get", json=json_payload)
 
         return Device.from_dict(res["thermostat"])
 
     def heat(
         self,
         *,
         device_id: str,
@@ -74,15 +74,15 @@
         if heating_set_point_celsius is not None:
             json_payload["heating_set_point_celsius"] = heating_set_point_celsius
         if heating_set_point_fahrenheit is not None:
             json_payload["heating_set_point_fahrenheit"] = heating_set_point_fahrenheit
         if sync is not None:
             json_payload["sync"] = sync
 
-        res = self.seam.make_request("POST", "/thermostats/heat", json=json_payload)
+        res = self.seam.client.post("/thermostats/heat", json=json_payload)
 
         return self.seam.action_attempts.decide_and_wait(
             action_attempt=ActionAttempt.from_dict(res["action_attempt"]),
             wait_for_action_attempt=wait_for_action_attempt,
         )
 
     def heat_cool(
@@ -107,17 +107,15 @@
         if heating_set_point_celsius is not None:
             json_payload["heating_set_point_celsius"] = heating_set_point_celsius
         if heating_set_point_fahrenheit is not None:
             json_payload["heating_set_point_fahrenheit"] = heating_set_point_fahrenheit
         if sync is not None:
             json_payload["sync"] = sync
 
-        res = self.seam.make_request(
-            "POST", "/thermostats/heat_cool", json=json_payload
-        )
+        res = self.seam.client.post("/thermostats/heat_cool", json=json_payload)
 
         return self.seam.action_attempts.decide_and_wait(
             action_attempt=ActionAttempt.from_dict(res["action_attempt"]),
             wait_for_action_attempt=wait_for_action_attempt,
         )
 
     def list(
@@ -162,15 +160,15 @@
         if limit is not None:
             json_payload["limit"] = limit
         if manufacturer is not None:
             json_payload["manufacturer"] = manufacturer
         if user_identifier_key is not None:
             json_payload["user_identifier_key"] = user_identifier_key
 
-        res = self.seam.make_request("POST", "/thermostats/list", json=json_payload)
+        res = self.seam.client.post("/thermostats/list", json=json_payload)
 
         return [Device.from_dict(item) for item in res["thermostats"]]
 
     def off(
         self,
         *,
         device_id: str,
@@ -180,15 +178,15 @@
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
         if sync is not None:
             json_payload["sync"] = sync
 
-        res = self.seam.make_request("POST", "/thermostats/off", json=json_payload)
+        res = self.seam.client.post("/thermostats/off", json=json_payload)
 
         return self.seam.action_attempts.decide_and_wait(
             action_attempt=ActionAttempt.from_dict(res["action_attempt"]),
             wait_for_action_attempt=wait_for_action_attempt,
         )
 
     def set_fan_mode(
@@ -207,17 +205,15 @@
         if fan_mode is not None:
             json_payload["fan_mode"] = fan_mode
         if fan_mode_setting is not None:
             json_payload["fan_mode_setting"] = fan_mode_setting
         if sync is not None:
             json_payload["sync"] = sync
 
-        res = self.seam.make_request(
-            "POST", "/thermostats/set_fan_mode", json=json_payload
-        )
+        res = self.seam.client.post("/thermostats/set_fan_mode", json=json_payload)
 
         return self.seam.action_attempts.decide_and_wait(
             action_attempt=ActionAttempt.from_dict(res["action_attempt"]),
             wait_for_action_attempt=wait_for_action_attempt,
         )
 
     def update(
@@ -226,10 +222,10 @@
         json_payload = {}
 
         if default_climate_setting is not None:
             json_payload["default_climate_setting"] = default_climate_setting
         if device_id is not None:
             json_payload["device_id"] = device_id
 
-        self.seam.make_request("POST", "/thermostats/update", json=json_payload)
+        self.seam.client.post("/thermostats/update", json=json_payload)
 
         return None
```

### Comparing `seam-0.7.1/seam/routes/thermostats_climate_setting_schedules.py` & `seam-0.8.0/seam/routes/thermostats_climate_setting_schedules.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,28 +54,28 @@
         if manual_override_allowed is not None:
             json_payload["manual_override_allowed"] = manual_override_allowed
         if name is not None:
             json_payload["name"] = name
         if schedule_type is not None:
             json_payload["schedule_type"] = schedule_type
 
-        res = self.seam.make_request(
-            "POST", "/thermostats/climate_setting_schedules/create", json=json_payload
+        res = self.seam.client.post(
+            "/thermostats/climate_setting_schedules/create", json=json_payload
         )
 
         return ClimateSettingSchedule.from_dict(res["climate_setting_schedule"])
 
     def delete(self, *, climate_setting_schedule_id: str) -> None:
         json_payload = {}
 
         if climate_setting_schedule_id is not None:
             json_payload["climate_setting_schedule_id"] = climate_setting_schedule_id
 
-        self.seam.make_request(
-            "POST", "/thermostats/climate_setting_schedules/delete", json=json_payload
+        self.seam.client.post(
+            "/thermostats/climate_setting_schedules/delete", json=json_payload
         )
 
         return None
 
     def get(
         self,
         *,
@@ -85,32 +85,32 @@
         json_payload = {}
 
         if climate_setting_schedule_id is not None:
             json_payload["climate_setting_schedule_id"] = climate_setting_schedule_id
         if device_id is not None:
             json_payload["device_id"] = device_id
 
-        res = self.seam.make_request(
-            "POST", "/thermostats/climate_setting_schedules/get", json=json_payload
+        res = self.seam.client.post(
+            "/thermostats/climate_setting_schedules/get", json=json_payload
         )
 
         return ClimateSettingSchedule.from_dict(res["climate_setting_schedule"])
 
     def list(
         self, *, device_id: str, user_identifier_key: Optional[str] = None
     ) -> List[ClimateSettingSchedule]:
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
         if user_identifier_key is not None:
             json_payload["user_identifier_key"] = user_identifier_key
 
-        res = self.seam.make_request(
-            "POST", "/thermostats/climate_setting_schedules/list", json=json_payload
+        res = self.seam.client.post(
+            "/thermostats/climate_setting_schedules/list", json=json_payload
         )
 
         return [
             ClimateSettingSchedule.from_dict(item)
             for item in res["climate_setting_schedules"]
         ]
 
@@ -156,12 +156,12 @@
         if schedule_ends_at is not None:
             json_payload["schedule_ends_at"] = schedule_ends_at
         if schedule_starts_at is not None:
             json_payload["schedule_starts_at"] = schedule_starts_at
         if schedule_type is not None:
             json_payload["schedule_type"] = schedule_type
 
-        self.seam.make_request(
-            "POST", "/thermostats/climate_setting_schedules/update", json=json_payload
+        self.seam.client.post(
+            "/thermostats/climate_setting_schedules/update", json=json_payload
         )
 
         return None
```

### Comparing `seam-0.7.1/seam/routes/types.py` & `seam-0.8.0/seam/routes/types.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.1/seam/routes/user_identities.py` & `seam-0.8.0/seam/routes/user_identities.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,17 +27,15 @@
         json_payload = {}
 
         if acs_user_id is not None:
             json_payload["acs_user_id"] = acs_user_id
         if user_identity_id is not None:
             json_payload["user_identity_id"] = user_identity_id
 
-        self.seam.make_request(
-            "POST", "/user_identities/add_acs_user", json=json_payload
-        )
+        self.seam.client.post("/user_identities/add_acs_user", json=json_payload)
 
         return None
 
     def create(
         self,
         *,
         email_address: Optional[str] = None,
@@ -52,27 +50,25 @@
         if full_name is not None:
             json_payload["full_name"] = full_name
         if phone_number is not None:
             json_payload["phone_number"] = phone_number
         if user_identity_key is not None:
             json_payload["user_identity_key"] = user_identity_key
 
-        res = self.seam.make_request(
-            "POST", "/user_identities/create", json=json_payload
-        )
+        res = self.seam.client.post("/user_identities/create", json=json_payload)
 
         return UserIdentity.from_dict(res["user_identity"])
 
     def delete(self, *, user_identity_id: str) -> None:
         json_payload = {}
 
         if user_identity_id is not None:
             json_payload["user_identity_id"] = user_identity_id
 
-        self.seam.make_request("POST", "/user_identities/delete", json=json_payload)
+        self.seam.client.post("/user_identities/delete", json=json_payload)
 
         return None
 
     def get(
         self,
         *,
         user_identity_id: Optional[str] = None,
@@ -81,106 +77,104 @@
         json_payload = {}
 
         if user_identity_id is not None:
             json_payload["user_identity_id"] = user_identity_id
         if user_identity_key is not None:
             json_payload["user_identity_key"] = user_identity_key
 
-        res = self.seam.make_request("POST", "/user_identities/get", json=json_payload)
+        res = self.seam.client.post("/user_identities/get", json=json_payload)
 
         return UserIdentity.from_dict(res["user_identity"])
 
     def grant_access_to_device(self, *, device_id: str, user_identity_id: str) -> None:
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
         if user_identity_id is not None:
             json_payload["user_identity_id"] = user_identity_id
 
-        self.seam.make_request(
-            "POST", "/user_identities/grant_access_to_device", json=json_payload
+        self.seam.client.post(
+            "/user_identities/grant_access_to_device", json=json_payload
         )
 
         return None
 
     def list(
         self, *, credential_manager_acs_system_id: Optional[str] = None
     ) -> List[UserIdentity]:
         json_payload = {}
 
         if credential_manager_acs_system_id is not None:
             json_payload["credential_manager_acs_system_id"] = (
                 credential_manager_acs_system_id
             )
 
-        res = self.seam.make_request("POST", "/user_identities/list", json=json_payload)
+        res = self.seam.client.post("/user_identities/list", json=json_payload)
 
         return [UserIdentity.from_dict(item) for item in res["user_identities"]]
 
     def list_accessible_devices(self, *, user_identity_id: str) -> List[Device]:
         json_payload = {}
 
         if user_identity_id is not None:
             json_payload["user_identity_id"] = user_identity_id
 
-        res = self.seam.make_request(
-            "POST", "/user_identities/list_accessible_devices", json=json_payload
+        res = self.seam.client.post(
+            "/user_identities/list_accessible_devices", json=json_payload
         )
 
         return [Device.from_dict(item) for item in res["devices"]]
 
     def list_acs_systems(self, *, user_identity_id: str) -> List[AcsSystem]:
         json_payload = {}
 
         if user_identity_id is not None:
             json_payload["user_identity_id"] = user_identity_id
 
-        res = self.seam.make_request(
-            "POST", "/user_identities/list_acs_systems", json=json_payload
+        res = self.seam.client.post(
+            "/user_identities/list_acs_systems", json=json_payload
         )
 
         return [AcsSystem.from_dict(item) for item in res["acs_systems"]]
 
     def list_acs_users(self, *, user_identity_id: str) -> List[AcsUser]:
         json_payload = {}
 
         if user_identity_id is not None:
             json_payload["user_identity_id"] = user_identity_id
 
-        res = self.seam.make_request(
-            "POST", "/user_identities/list_acs_users", json=json_payload
+        res = self.seam.client.post(
+            "/user_identities/list_acs_users", json=json_payload
         )
 
         return [AcsUser.from_dict(item) for item in res["acs_users"]]
 
     def remove_acs_user(self, *, acs_user_id: str, user_identity_id: str) -> None:
         json_payload = {}
 
         if acs_user_id is not None:
             json_payload["acs_user_id"] = acs_user_id
         if user_identity_id is not None:
             json_payload["user_identity_id"] = user_identity_id
 
-        self.seam.make_request(
-            "POST", "/user_identities/remove_acs_user", json=json_payload
-        )
+        self.seam.client.post("/user_identities/remove_acs_user", json=json_payload)
 
         return None
 
     def revoke_access_to_device(self, *, device_id: str, user_identity_id: str) -> None:
         json_payload = {}
 
         if device_id is not None:
             json_payload["device_id"] = device_id
         if user_identity_id is not None:
             json_payload["user_identity_id"] = user_identity_id
 
-        self.seam.make_request(
-            "POST", "/user_identities/revoke_access_to_device", json=json_payload
+        self.seam.client.post(
+            "/user_identities/revoke_access_to_device", json=json_payload
         )
 
         return None
 
     def update(
         self,
         *,
@@ -199,10 +193,10 @@
         if full_name is not None:
             json_payload["full_name"] = full_name
         if phone_number is not None:
             json_payload["phone_number"] = phone_number
         if user_identity_key is not None:
             json_payload["user_identity_key"] = user_identity_key
 
-        self.seam.make_request("POST", "/user_identities/update", json=json_payload)
+        self.seam.client.post("/user_identities/update", json=json_payload)
 
         return None
```

### Comparing `seam-0.7.1/seam/routes/user_identities_enrollment_automations.py` & `seam-0.8.0/seam/routes/user_identities_enrollment_automations.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,28 +14,28 @@
 
     def delete(self, *, enrollment_automation_id: str) -> None:
         json_payload = {}
 
         if enrollment_automation_id is not None:
             json_payload["enrollment_automation_id"] = enrollment_automation_id
 
-        self.seam.make_request(
-            "POST", "/user_identities/enrollment_automations/delete", json=json_payload
+        self.seam.client.post(
+            "/user_identities/enrollment_automations/delete", json=json_payload
         )
 
         return None
 
     def get(self, *, enrollment_automation_id: str) -> EnrollmentAutomation:
         json_payload = {}
 
         if enrollment_automation_id is not None:
             json_payload["enrollment_automation_id"] = enrollment_automation_id
 
-        res = self.seam.make_request(
-            "POST", "/user_identities/enrollment_automations/get", json=json_payload
+        res = self.seam.client.post(
+            "/user_identities/enrollment_automations/get", json=json_payload
         )
 
         return EnrollmentAutomation.from_dict(res["enrollment_automation"])
 
     def launch(
         self,
         *,
@@ -60,27 +60,27 @@
                 create_credential_manager_user
             )
         if credential_manager_acs_user_id is not None:
             json_payload["credential_manager_acs_user_id"] = (
                 credential_manager_acs_user_id
             )
 
-        self.seam.make_request(
-            "POST", "/user_identities/enrollment_automations/launch", json=json_payload
+        self.seam.client.post(
+            "/user_identities/enrollment_automations/launch", json=json_payload
         )
 
         return None
 
     def list(self, *, user_identity_id: str) -> List[EnrollmentAutomation]:
         json_payload = {}
 
         if user_identity_id is not None:
             json_payload["user_identity_id"] = user_identity_id
 
-        res = self.seam.make_request(
-            "POST", "/user_identities/enrollment_automations/list", json=json_payload
+        res = self.seam.client.post(
+            "/user_identities/enrollment_automations/list", json=json_payload
         )
 
         return [
             EnrollmentAutomation.from_dict(item)
             for item in res["enrollment_automations"]
         ]
```

### Comparing `seam-0.7.1/seam/routes/utils/deep_attr_dict.py` & `seam-0.8.0/seam/routes/utils/deep_attr_dict.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.1/seam/routes/webhooks.py` & `seam-0.8.0/seam/routes/webhooks.py`

 * *Files 16% similar despite different names*

```diff
@@ -13,51 +13,51 @@
         json_payload = {}
 
         if url is not None:
             json_payload["url"] = url
         if event_types is not None:
             json_payload["event_types"] = event_types
 
-        res = self.seam.make_request("POST", "/webhooks/create", json=json_payload)
+        res = self.seam.client.post("/webhooks/create", json=json_payload)
 
         return Webhook.from_dict(res["webhook"])
 
     def delete(self, *, webhook_id: str) -> None:
         json_payload = {}
 
         if webhook_id is not None:
             json_payload["webhook_id"] = webhook_id
 
-        self.seam.make_request("POST", "/webhooks/delete", json=json_payload)
+        self.seam.client.post("/webhooks/delete", json=json_payload)
 
         return None
 
     def get(self, *, webhook_id: str) -> Webhook:
         json_payload = {}
 
         if webhook_id is not None:
             json_payload["webhook_id"] = webhook_id
 
-        res = self.seam.make_request("POST", "/webhooks/get", json=json_payload)
+        res = self.seam.client.post("/webhooks/get", json=json_payload)
 
         return Webhook.from_dict(res["webhook"])
 
     def list(
         self,
     ) -> List[Webhook]:
         json_payload = {}
 
-        res = self.seam.make_request("POST", "/webhooks/list", json=json_payload)
+        res = self.seam.client.post("/webhooks/list", json=json_payload)
 
         return [Webhook.from_dict(item) for item in res["webhooks"]]
 
     def update(self, *, event_types: List[str], webhook_id: str) -> None:
         json_payload = {}
 
         if event_types is not None:
             json_payload["event_types"] = event_types
         if webhook_id is not None:
             json_payload["webhook_id"] = webhook_id
 
-        self.seam.make_request("POST", "/webhooks/update", json=json_payload)
+        self.seam.client.post("/webhooks/update", json=json_payload)
 
         return None
```

### Comparing `seam-0.7.1/seam/routes/workspaces.py` & `seam-0.8.0/seam/routes/workspaces.py`

 * *Files 16% similar despite different names*

```diff
@@ -27,42 +27,40 @@
         if is_sandbox is not None:
             json_payload["is_sandbox"] = is_sandbox
         if webview_logo_shape is not None:
             json_payload["webview_logo_shape"] = webview_logo_shape
         if webview_primary_button_color is not None:
             json_payload["webview_primary_button_color"] = webview_primary_button_color
 
-        res = self.seam.make_request("POST", "/workspaces/create", json=json_payload)
+        res = self.seam.client.post("/workspaces/create", json=json_payload)
 
         return Workspace.from_dict(res["workspace"])
 
     def get(
         self,
     ) -> Workspace:
         json_payload = {}
 
-        res = self.seam.make_request("POST", "/workspaces/get", json=json_payload)
+        res = self.seam.client.post("/workspaces/get", json=json_payload)
 
         return Workspace.from_dict(res["workspace"])
 
     def list(
         self,
     ) -> List[Workspace]:
         json_payload = {}
 
-        res = self.seam.make_request("POST", "/workspaces/list", json=json_payload)
+        res = self.seam.client.post("/workspaces/list", json=json_payload)
 
         return [Workspace.from_dict(item) for item in res["workspaces"]]
 
     def reset_sandbox(
         self, wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]] = None
     ) -> ActionAttempt:
         json_payload = {}
 
-        res = self.seam.make_request(
-            "POST", "/workspaces/reset_sandbox", json=json_payload
-        )
+        res = self.seam.client.post("/workspaces/reset_sandbox", json=json_payload)
 
         return self.seam.action_attempts.decide_and_wait(
             action_attempt=ActionAttempt.from_dict(res["action_attempt"]),
             wait_for_action_attempt=wait_for_action_attempt,
         )
```

### Comparing `seam-0.7.1/seam/seam.py` & `seam-0.8.0/seam/seam.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from typing import Optional, Union, Dict
+from typing import Any, Optional, Union, Dict
+import niquests as requests
 from typing_extensions import Self
 
 from .constants import LTS_VERSION
 from .parse_options import parse_options
-from .request import RequestMixin
+from .client import SeamHttpClient
 from .routes.routes import Routes
 from .types import AbstractSeam
 
 
-class Seam(AbstractSeam, RequestMixin):
+class Seam(AbstractSeam):
     """
     Initial Seam class used to interact with Seam API
     """
 
     lts_version: str = LTS_VERSION
 
     def __init__(
@@ -45,16 +46,16 @@
         self.wait_for_action_attempt = wait_for_action_attempt
         auth_headers, endpoint = parse_options(
             api_key=api_key,
             personal_access_token=personal_access_token,
             workspace_id=workspace_id,
             endpoint=endpoint,
         )
-        self._auth_headers = auth_headers
-        self._endpoint = endpoint
+
+        self.client = SeamHttpClient(base_url=endpoint, auth_headers=auth_headers)
 
     @classmethod
     def from_api_key(
         cls,
         api_key: str,
         *,
         endpoint: Optional[str] = None,
```

### Comparing `seam-0.7.1/seam/seam_multi_workspace.py` & `seam-0.8.0/seam/seam_multi_workspace.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from typing import Dict, Optional, Union
+from typing import Any, Dict, Optional, Union
+import niquests as requests
 from typing_extensions import Self
 
 from .auth import get_auth_headers_for_multi_workspace_personal_access_token
 from .constants import LTS_VERSION
 from .options import get_endpoint
-from .request import RequestMixin
+from .client import SeamHttpClient
 from .types import AbstractSeamMultiWorkspace
 from .routes.workspaces import Workspaces
 
 
 class WorkspacesProxy:
     """Proxy to expose only the 'create' and 'list' methods of Workspaces."""
 
@@ -18,15 +19,15 @@
     def list(self, **kwargs):
         return self._workspaces.list(**kwargs)
 
     def create(self, **kwargs):
         return self._workspaces.create(**kwargs)
 
 
-class SeamMultiWorkspace(AbstractSeamMultiWorkspace, RequestMixin):
+class SeamMultiWorkspace(AbstractSeamMultiWorkspace):
     """
     Seam class used to interact with Seam API without being scoped to any specific workspace.
     """
 
     lts_version: str = LTS_VERSION
 
     def __init__(
@@ -45,18 +46,23 @@
           The API endpoint to which the request should be sent.
         wait_for_action_attempt : bool or dict, optional
           Controls whether to wait for an action attempt to complete, either as a boolean or as a dictionary specifying `timeout` and `poll_interval`. Defaults to `False`.
         """
 
         self.lts_version = SeamMultiWorkspace.lts_version
         self.wait_for_action_attempt = wait_for_action_attempt
-        self._auth_headers = get_auth_headers_for_multi_workspace_personal_access_token(
+        auth_headers = get_auth_headers_for_multi_workspace_personal_access_token(
             personal_access_token
         )
-        self._endpoint = get_endpoint(endpoint)
+        endpoint = get_endpoint(endpoint)
+
+        self.client = SeamHttpClient(
+            base_url=endpoint,
+            auth_headers=auth_headers,
+        )
 
         self._workspaces = Workspaces(seam=self)
         self.workspaces = WorkspacesProxy(self._workspaces)
 
     @classmethod
     def from_personal_access_token(
         cls,
```

### Comparing `seam-0.7.1/seam/token.py` & `seam-0.8.0/seam/token.py`

 * *Files identical despite different names*

### Comparing `seam-0.7.1/seam/types.py` & `seam-0.8.0/seam/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Any, Dict, List, Optional, Union
+import niquests as requests
 from typing_extensions import Self
 import abc
 
 from seam.routes.types import AbstractRoutes, Workspace
 
 
 class SeamHttpApiError(Exception):
@@ -19,21 +20,29 @@
             self.metadata = parsed_response.get("error", None)
 
         super().__init__(
             f"SeamHttpApiError: status={self.status_code}, request_id={self.request_id}, metadata={self.metadata}"
         )
 
 
-class AbstractRequestMixin(abc.ABC):
+class AbstractSeamHttpClient(abc.ABC):
     @abc.abstractmethod
-    def make_request(self, method: str, path: str, **kwargs):
+    def __init__(self, base_url: str, auth_headers: Dict[str, str], **kwargs):
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def request(self, method: str, url: str, *args, **kwargs):
+        raise NotImplementedError
+
+    @abc.abstractmethod
+    def _handle_response(self, response: requests.Response):
         raise NotImplementedError
 
 
-class AbstractSeam(AbstractRoutes, AbstractRequestMixin):
+class AbstractSeam(AbstractRoutes):
     lts_version: str
     wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]]
 
     @abc.abstractmethod
     def __init__(
         self,
         api_key: Optional[str] = None,
@@ -85,15 +94,15 @@
     @abc.abstractmethod
     def list(
         self,
     ) -> List[Workspace]:
         raise NotImplementedError()
 
 
-class AbstractSeamMultiWorkspace(AbstractRequestMixin):
+class AbstractSeamMultiWorkspace:
     lts_version: str
     wait_for_action_attempt: Optional[Union[bool, Dict[str, float]]]
 
     @abc.abstractmethod
     def __init__(
         self,
         personal_access_token: str,
```

### Comparing `seam-0.7.1/PKG-INFO` & `seam-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: seam
-Version: 0.7.1
+Version: 0.8.0
 Summary: SDK for the Seam API written in Python.
 Home-page: https://github.com/seamapi/python-next
 License: MIT
 Author: Seam Labs, Inc.
 Author-email: engineering@getseam.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dataclasses-json (>=0.6.4,<0.7.0)
-Requires-Dist: requests (>=2.26.0,<3.0.0)
+Requires-Dist: niquests (>=3.6.4,<4.0.0)
 Project-URL: Repository, https://github.com/seamapi/python-next
 Description-Content-Type: text/x-rst
 
 Seam Python SDK
 ===============
 
 |PyPI| |GitHub Actions|
```

