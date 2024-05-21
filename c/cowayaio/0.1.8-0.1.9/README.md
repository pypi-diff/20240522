# Comparing `tmp/cowayaio-0.1.8.tar.gz` & `tmp/cowayaio-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cowayaio-0.1.8.tar", last modified: Mon Aug 28 19:55:19 2023, max compression
+gzip compressed data, was "cowayaio-0.1.9.tar", last modified: Sun Apr 28 22:34:12 2024, max compression
```

## Comparing `cowayaio-0.1.8.tar` & `cowayaio-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-08-28 19:55:19.946836 cowayaio-0.1.8/
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1067 2023-08-28 19:51:29.000000 cowayaio-0.1.8/LICENSE
--rw-r--r--   0 robertdrinovac   (501) staff       (20)      774 2023-08-28 19:55:19.946349 cowayaio-0.1.8/PKG-INFO
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)       92 2023-08-28 19:51:29.000000 cowayaio-0.1.8/README.md
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-08-28 19:55:19.943700 cowayaio-0.1.8/cowayaio/
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      523 2023-08-28 19:51:29.000000 cowayaio-0.1.8/cowayaio/__init__.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1050 2023-08-28 19:51:29.000000 cowayaio-0.1.8/cowayaio/constants.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)    21620 2023-08-28 19:51:29.000000 cowayaio-0.1.8/cowayaio/coway_client.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      663 2023-08-28 19:51:29.000000 cowayaio-0.1.8/cowayaio/exceptions.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1085 2023-08-28 19:51:29.000000 cowayaio-0.1.8/cowayaio/purifier_model.py
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      680 2023-08-28 19:51:29.000000 cowayaio-0.1.8/cowayaio/str_enum.py
-drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2023-08-28 19:55:19.945685 cowayaio-0.1.8/cowayaio.egg-info/
--rw-r--r--   0 robertdrinovac   (501) staff       (20)      774 2023-08-28 19:55:19.000000 cowayaio-0.1.8/cowayaio.egg-info/PKG-INFO
--rw-r--r--   0 robertdrinovac   (501) staff       (20)      324 2023-08-28 19:55:19.000000 cowayaio-0.1.8/cowayaio.egg-info/SOURCES.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2023-08-28 19:55:19.000000 cowayaio-0.1.8/cowayaio.egg-info/dependency_links.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       38 2023-08-28 19:55:19.000000 cowayaio-0.1.8/cowayaio.egg-info/requires.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)        9 2023-08-28 19:55:19.000000 cowayaio-0.1.8/cowayaio.egg-info/top_level.txt
--rw-r--r--   0 robertdrinovac   (501) staff       (20)       38 2023-08-28 19:55:19.946988 cowayaio-0.1.8/setup.cfg
--rw-rw-r--   0 robertdrinovac   (501) staff       (20)      985 2023-08-28 19:51:29.000000 cowayaio-0.1.8/setup.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2024-04-28 22:34:12.864282 cowayaio-0.1.9/
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1067 2024-04-28 22:26:56.000000 cowayaio-0.1.9/LICENSE
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)      774 2024-04-28 22:34:12.863878 cowayaio-0.1.9/PKG-INFO
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)       92 2024-04-28 22:26:56.000000 cowayaio-0.1.9/README.md
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2024-04-28 22:34:12.860560 cowayaio-0.1.9/cowayaio/
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      547 2024-04-28 22:26:56.000000 cowayaio-0.1.9/cowayaio/__init__.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1124 2024-04-28 22:26:56.000000 cowayaio-0.1.9/cowayaio/constants.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)    23563 2024-04-28 22:26:56.000000 cowayaio-0.1.9/cowayaio/coway_client.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      663 2024-04-28 22:26:56.000000 cowayaio-0.1.9/cowayaio/exceptions.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)     1126 2024-04-28 22:26:56.000000 cowayaio-0.1.9/cowayaio/purifier_model.py
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      680 2024-04-28 22:26:56.000000 cowayaio-0.1.9/cowayaio/str_enum.py
+drwxr-xr-x   0 robertdrinovac   (501) staff       (20)        0 2024-04-28 22:34:12.863219 cowayaio-0.1.9/cowayaio.egg-info/
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)      774 2024-04-28 22:34:12.000000 cowayaio-0.1.9/cowayaio.egg-info/PKG-INFO
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)      324 2024-04-28 22:34:12.000000 cowayaio-0.1.9/cowayaio.egg-info/SOURCES.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)        1 2024-04-28 22:34:12.000000 cowayaio-0.1.9/cowayaio.egg-info/dependency_links.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       38 2024-04-28 22:34:12.000000 cowayaio-0.1.9/cowayaio.egg-info/requires.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)        9 2024-04-28 22:34:12.000000 cowayaio-0.1.9/cowayaio.egg-info/top_level.txt
+-rw-r--r--   0 robertdrinovac   (501) staff       (20)       38 2024-04-28 22:34:12.864485 cowayaio-0.1.9/setup.cfg
+-rw-rw-r--   0 robertdrinovac   (501) staff       (20)      985 2024-04-28 22:26:56.000000 cowayaio-0.1.9/setup.py
```

### Comparing `cowayaio-0.1.8/LICENSE` & `cowayaio-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cowayaio-0.1.8/PKG-INFO` & `cowayaio-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cowayaio
-Version: 0.1.8
+Version: 0.1.9
 Summary: A asynchronous python library for Coway Air Purifiers 
 Home-page: https://github.com/RobertD502/cowayaio
 Author: Robert Drinovac
 Author-email: unlisted@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/RobertD502/cowayaio/issues
 Project-URL: Source, https://github.com/RobertD502/cowayaio/
```

### Comparing `cowayaio-0.1.8/cowayaio/constants.py` & `cowayaio-0.1.9/cowayaio/constants.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     REDIRECT_URL = "https://iocareapp.coway.com/bizmob.iocare/redirect/redirect_bridge.html"
 
 
 class Parameter(StrEnum):
 
     CLIENT_ID = "cwid-prd-iocare-20220930"
     SERVICE_CODE = "com.coway.IOCareKor"
-    APP_VERSION = "2.3.22"
+    APP_VERSION = "2.3.33"
 
 class Header(StrEnum):
 
     USER_AGENT = "Mozilla/5.0 (iPhone; CPU iPhone OS 10_3_1 like Mac OS X) AppleWebKit/603.1.30 (KHTML, like Gecko) Version/10.0 Mobile/14E304 Safari/602.1 app"
     ACCEPT = "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8"
     ACCEPT_LANG = "en-US,en;q=0.9"
 
@@ -29,8 +29,15 @@
     STATUS = 'CWIG0602'
     CONTROL = 'CWIG0603'
     FILTERS = 'CWIA0120'
     MCU_VERSION = "CWIG0615"
     PROD_SETTINGS = "CWIG0301"
     CHANGE_PRE_FILTER = "CWIA0600"
 
+
+class LightMode(StrEnum):
+
+    ON = '0'
+    AQI_OFF = '1'
+    OFF = '2'
+
 TIMEOUT = 5 * 60
```

### Comparing `cowayaio-0.1.8/cowayaio/coway_client.py` & `cowayaio-0.1.9/cowayaio/coway_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import json
 import logging
 
 from bs4 import BeautifulSoup
 from aiohttp import ClientResponse, ClientSession
 from http.cookies import SimpleCookie
 
-from cowayaio.constants import (Endpoint, Endpoint_JSON, Header, Parameter, TIMEOUT,)
+from cowayaio.constants import (Endpoint, Endpoint_JSON, Header, LightMode, Parameter, TIMEOUT,)
 from cowayaio.exceptions import AuthError, CowayError, PasswordExpired
 from cowayaio.purifier_model import PurifierData, CowayPurifier
 
 
 LOGGER = logging.getLogger(__name__)
 
 
@@ -143,45 +143,49 @@
                 'device_id': dev.get('barcode'),
                 'model': dev.get('dvcModel'),
                 'name': dev.get('dvcNick'),
                 'product_name': dev.get('prodName'),
                 'product_name_full': dev.get('prodNameFull'),
                 'device_type': dev.get('dvcTypeCd'),
                 'device_brand': dev.get('dvcBrandCd'),
-                'device_seq': dev.get('dvcSeq')
+                'device_seq': dev.get('dvcSeq'),
+                'order_number': dev.get('ordNo'),
             }
             state = await self.async_fetch_all_endpoints(device_attr)
             network_status = state[1][1]
             try:
                 mcu_version = state[0].get('curMcuVer')
                 is_on = state[1][0].get('0001') == '1'
                 auto_mode = state[1][0].get('0002') == '1'
                 auto_eco_mode = state[1][0].get('0002') == '6'
                 eco_mode = state[1][0].get('0002') == '6'
                 night_mode = state[1][0].get('0002') == '2'
+                rapid_mode = state[1][0].get('0002') == '5'
                 fan_speed = state[1][0].get('0003')
                 light_on = state[1][0].get('0007') == '2'
+                # 250s purifier has more than just on and off
+                light_mode = state[1][0].get('0007')
                 timer = state[1][0].get('offTimerData')
                 timer_remaining = state[1][0].get('0008')
                 pre_filter_name = state[2][0][0].get('filterName')
                 pre_filter_pct = state[2][0][0].get('filterPer')
                 pre_filter_last_changed = state[2][0][0].get('lastChangeDate')
                 pre_filter_change_months = state[2][0][0].get('changeCycle')
                 max2_name = state[2][0][1].get('filterName')
                 max2_pct = state[2][0][1].get('filterPer')
                 max2_last_changed = state[2][0][1].get('lastChangeDate')
                 max2_change_months = state[2][0][1].get('changeCycle')
-                dust_pollution = state[2][1][0].get('dustPollution')
-                air_volume = state[2][1][0].get('airVolume')
-                pollen_mode = state[2][1][0].get('pollenMode')
-                particulate_matter_2_5 = state[2][2][0].get('dustpm25')
-                particulate_matter_10 = state[2][2][0].get('dustpm10')
-                carbon_dioxide = state[2][2][0].get('co2')
-                volatile_organic_compounds = state[2][2][0].get('vocs')
-                air_quality_index = state[2][2][0].get('inairquality')
+                dust_pollution = state[2][1].get('dustPollution')
+                air_volume = state[2][1].get('airVolume')
+                pollen_mode = state[2][1].get('pollenMode')
+                particulate_matter_2_5 = state[2][2].get('dustpm25')
+                particulate_matter_10 = state[2][2].get('dustpm10')
+                carbon_dioxide = state[2][2].get('co2')
+                volatile_organic_compounds = state[2][2].get('vocs')
+                air_quality_index = state[2][2].get('inairquality')
                 pre_filter_change_frequency = state[3][1]
                 smart_mode_sensitivity = state[3][2]
             except IndexError:
                 if not network_status:
                     LOGGER.warning(f'Purifier {device_attr["name"]} is not connected to WiFi.')
                     continue
                 else:
@@ -192,16 +196,18 @@
                 mcu_version=mcu_version,
                 network_status=network_status,
                 is_on=is_on,
                 auto_mode=auto_mode,
                 auto_eco_mode=auto_eco_mode,
                 eco_mode=eco_mode,
                 night_mode=night_mode,
+                rapid_mode=rapid_mode,
                 fan_speed=fan_speed,
                 light_on=light_on,
+                light_mode=light_mode,
                 timer=timer,
                 timer_remaining=timer_remaining,
                 pre_filter_name=pre_filter_name,
                 pre_filter_pct=pre_filter_pct,
                 pre_filter_last_changed=pre_filter_last_changed,
                 pre_filter_change_months=pre_filter_change_months,
                 max2_name=max2_name,
@@ -270,25 +276,25 @@
     async def async_get_quality_status(self, device_attr: dict[str, Any]) -> tuple[list, list, list]:
         """Returns data for prefilter, max2 filter, and air quality sensors."""
 
         params = {
             'barcode': device_attr['device_id'],
             'dvcBrandCd': device_attr['device_brand'],
             'prodName': device_attr['product_name'],
-            'stationCd': '',
-            'resetDttm': '',
-            'dvcTypeCd': device_attr['device_type'],
-            'refreshFlag': 'true'
+            'deviceType': device_attr['device_type'],
+            'mqttDevice': 'true',
+            'orderNo': device_attr['order_number'],
+            'membershipYn': 'N',
         }
 
-        response = await self._post_endpoint(Endpoint_JSON.FILTERS, params)
+        response = await self._get_endpoint(Endpoint_JSON.FILTERS, params, use_new_api=True)
         try:
-            filter_list = response['body']['filterList']
-            prod_status = response['body']['prodStatus']
-            iaq = response['body']['IAQ']
+            filter_list = response['data']['filterList']
+            prod_status = response['data']['prodStatus']
+            iaq = response['data']['IAQ']
         except KeyError:
             raise CowayError(f'Coway API error: Coway server failed to return purifier quality status.')
         return filter_list, prod_status, iaq
 
     async def async_get_prod_settings(self, device_attr: dict[str, Any]) -> tuple[list, list, list]:
         """Returns purifier settings such as pre-filter frequency and smart mode sensitivity."""
 
@@ -334,24 +340,41 @@
     async def async_set_eco_mode(self, device_attr: dict[str, str]) -> None:
         """Set Purifier to Eco Mode.
         Only applies to AIRMEGA AP-1512HHS models.
         """
 
         await self.async_control_purifier(device_attr, '0002', '6')
 
+    async def async_set_rapid_mode(self, device_attr: dict[str, str]) -> None:
+        """Set Purifier to Rapid Mode.
+        Only applies to AIRMEGA 250s.
+        """
+
+        await self.async_control_purifier(device_attr, '0002', '5')
+
     async def async_set_fan_speed(self, device_attr: dict[str, str], speed: str) -> None:
         """Speed can be 1, 2, or 3 represented as a string."""
 
         await self.async_control_purifier(device_attr, '0003', speed)
 
     async def async_set_light(self, device_attr: dict[str, str], light_on: bool) -> None:
-        """Provide light_on as True for On and False for Off."""
+        """Provide light_on as True for On and False for Off.
+        NOT used for 250s purifiers.
+        """
 
         await self.async_control_purifier(device_attr, '0007', '2' if light_on else '0')
 
+    async def async_set_light_mode(self, device_attr: dict[str, str], light_mode: LightMode) -> None:
+        """Sets light mode for purifiers, like the 250s,
+        that support more than just On and Off. See LightMode
+        constant for available options.
+        """
+
+        await self.async_control_purifier(device_attr, '0007', light_mode)
+
     async def async_set_timer(self, device_attr: dict[str, str], time: str) -> None:
         """Time, in minutes, can be 0, 60, 120, 240, or 480 represented as a string. A time of 0 sets the timer to off."""
 
         await self.async_control_purifier(device_attr, '0008', time)
 
     async def async_set_smart_mode_sensitivity(self, device_attr: dict[str, str], sensitivity: str) -> None:
         """Sensitivity can be 1, 2, or 3. 1 = Sensitive, 2 = Normal, 3 = Insensitive. """
@@ -405,15 +428,14 @@
             else:
                 password_skip_init = False
                 return resp, password_skip_init
 
     async def _post_endpoint(self, endpoint: str, params: dict[str, Any]) -> dict[str, Any]:
         """Make POST API call to various endpoints."""
 
-
         url = Endpoint.BASE_URI + '/' + endpoint + '.json'
         headers = {
             'Content-Type': 'application/x-www-form-urlencoded;charset=UTF-8',
             'Accept': 'application/json, text/plain, */*',
             'User-Agent': 'Mozilla/5.0 (iPhone; CPU iPhone OS 10_3_1 like Mac OS X) AppleWebKit/603.1.30 (KHTML, like Gecko) Version/10.0 Mobile/14E304 Safari/602.1'
         }
 
@@ -434,14 +456,31 @@
         data = {
             'message': json.dumps(message)
         }
 
         async with self._session.post(url, headers=headers, data=data, timeout=self.timeout) as resp:
             return await self._response(resp)
 
+    async def _get_endpoint(self, endpoint: str, params: dict[str, Any], use_new_api=False) -> dict[str, Any]:
+        """Temp usage of new Coway API."""
+
+        if use_new_api:
+            if endpoint == Endpoint_JSON.FILTERS:
+                url = f'https://iocareapi.iot.coway.com/api/v1/air/devices/{params["barcode"]}/home'
+                headers = {
+                    'content-type': 'application/json',
+                    'profile': 'prod',
+                    'accept': '*/*',
+                    'authorization': f'Bearer {self.access_token}',
+                    'accept-language': Header.ACCEPT_LANG,
+                    'user-agent': Header.USER_AGENT,
+                    'trcode': Endpoint_JSON.FILTERS,
+                }
+                async with self._session.get(url, headers=headers, params=params, timeout=self.timeout) as resp:
+                    return await self._response(resp, new_api=True)
 
     async def async_control_purifier(self, device_attr: dict[str, str], command: str, value: Any) -> ClientResponse:
         url = Endpoint.BASE_URI + '/' + Endpoint_JSON.CONTROL + '.json'
         headers = {
             'Content-Type': 'application/x-www-form-urlencoded',
             'Accept': 'application/json',
             'User-Agent': Header.USER_AGENT
@@ -498,20 +537,21 @@
             'message': json.dumps(message)
         }
 
         async with self._session.post(url, headers=headers, data=data, timeout=self.timeout) as resp:
             return resp
 
     @staticmethod
-    async def _response(resp: ClientResponse) -> dict[str, Any]:
+    async def _response(resp: ClientResponse, new_api=False) -> dict[str, Any]:
         """Return response from API call."""
 
         if resp.status != 200:
             error = await resp.text()
             raise CowayError(f'Coway API error: {error}')
         try:
             response: dict[str, Any] = await resp.json()
         except Exception as error:
             raise CowayError(f'Could not return json {error}') from error
-        if (header := response['header']['error_code'])  == 'CWIG0304COWAYLgnE':
-            raise AuthError(f'Error code {header}: Coway IoCare access and refresh tokens are invalid. Attempting to fetch new tokens.')
+        if new_api == False:
+            if (header := response['header']['error_code'])  == 'CWIG0304COWAYLgnE':
+                raise AuthError(f'Error code {header}: Coway IoCare access and refresh tokens are invalid. Attempting to fetch new tokens.')
         return response
```

### Comparing `cowayaio-0.1.8/cowayaio/exceptions.py` & `cowayaio-0.1.9/cowayaio/exceptions.py`

 * *Files identical despite different names*

### Comparing `cowayaio-0.1.8/cowayaio/purifier_model.py` & `cowayaio-0.1.9/cowayaio/purifier_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,16 +18,18 @@
     mcu_version: str | None
     network_status: bool
     is_on: bool
     auto_mode: bool
     auto_eco_mode: bool
     eco_mode: bool
     night_mode: bool
+    rapid_mode: bool
     fan_speed: str | None
     light_on: bool
+    light_mode: str
     timer: str | None
     timer_remaining: str | None
     pre_filter_name: str
     pre_filter_pct: int
     pre_filter_last_changed: str
     pre_filter_change_months: str
     max2_name: str
```

### Comparing `cowayaio-0.1.8/cowayaio/str_enum.py` & `cowayaio-0.1.9/cowayaio/str_enum.py`

 * *Files identical despite different names*

### Comparing `cowayaio-0.1.8/cowayaio.egg-info/PKG-INFO` & `cowayaio-0.1.9/cowayaio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cowayaio
-Version: 0.1.8
+Version: 0.1.9
 Summary: A asynchronous python library for Coway Air Purifiers 
 Home-page: https://github.com/RobertD502/cowayaio
 Author: Robert Drinovac
 Author-email: unlisted@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/RobertD502/cowayaio/issues
 Project-URL: Source, https://github.com/RobertD502/cowayaio/
```

### Comparing `cowayaio-0.1.8/setup.py` & `cowayaio-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="cowayaio",
-    version="0.1.8",
+    version="0.1.9",
     author="Robert Drinovac",
     author_email="unlisted@gmail.com",
     description="A asynchronous python library for Coway Air Purifiers ",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/RobertD502/cowayaio',
     keywords='coway, iocare, iocare api, coway api, airmega',
```

