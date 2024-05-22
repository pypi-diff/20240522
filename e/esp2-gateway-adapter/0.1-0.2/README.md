# Comparing `tmp/esp2_gateway_adapter-0.1.tar.gz` & `tmp/esp2_gateway_adapter-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "esp2_gateway_adapter-0.1.tar", last modified: Wed Mar 20 10:37:10 2024, max compression
+gzip compressed data, was "esp2_gateway_adapter-0.2.tar", last modified: Wed May 22 20:55:12 2024, max compression
```

## Comparing `esp2_gateway_adapter-0.1.tar` & `esp2_gateway_adapter-0.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:37:10.614794 esp2_gateway_adapter-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-20 10:37:01.000000 esp2_gateway_adapter-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-03-20 10:37:10.614794 esp2_gateway_adapter-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-20 10:37:01.000000 esp2_gateway_adapter-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:37:10.614794 esp2_gateway_adapter-0.1/esp2_gateway_adapter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-03-20 10:37:10.000000 esp2_gateway_adapter-0.1/esp2_gateway_adapter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-20 10:37:10.000000 esp2_gateway_adapter-0.1/esp2_gateway_adapter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 10:37:10.000000 esp2_gateway_adapter-0.1/esp2_gateway_adapter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-20 10:37:10.000000 esp2_gateway_adapter-0.1/esp2_gateway_adapter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-20 10:37:10.000000 esp2_gateway_adapter-0.1/esp2_gateway_adapter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 10:37:10.614794 esp2_gateway_adapter-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-20 10:37:01.000000 esp2_gateway_adapter-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 10:37:10.614794 esp2_gateway_adapter-0.1/src/
--rw-r--r--   0 runner    (1001) docker     (127)    15224 2024-03-20 10:37:01.000000 esp2_gateway_adapter-0.1/src/esp3_serial_com.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:55:12.606546 esp2_gateway_adapter-0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-22 20:55:07.000000 esp2_gateway_adapter-0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-22 20:55:12.606546 esp2_gateway_adapter-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-22 20:55:07.000000 esp2_gateway_adapter-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:55:12.606546 esp2_gateway_adapter-0.2/esp2_gateway_adapter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-22 20:55:12.000000 esp2_gateway_adapter-0.2/esp2_gateway_adapter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-22 20:55:12.000000 esp2_gateway_adapter-0.2/esp2_gateway_adapter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:55:12.000000 esp2_gateway_adapter-0.2/esp2_gateway_adapter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-22 20:55:12.000000 esp2_gateway_adapter-0.2/esp2_gateway_adapter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 20:55:12.000000 esp2_gateway_adapter-0.2/esp2_gateway_adapter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:55:12.606546 esp2_gateway_adapter-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-22 20:55:07.000000 esp2_gateway_adapter-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:55:12.606546 esp2_gateway_adapter-0.2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    15219 2024-05-22 20:55:07.000000 esp2_gateway_adapter-0.2/src/esp3_serial_com.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3959 2024-05-22 20:55:07.000000 esp2_gateway_adapter-0.2/src/esp3_tcp_com.py
```

### Comparing `esp2_gateway_adapter-0.1/LICENSE` & `esp2_gateway_adapter-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `esp2_gateway_adapter-0.1/PKG-INFO` & `esp2_gateway_adapter-0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp2_gateway_adapter
-Version: 0.1
+Version: 0.2
 Summary: Protocol adapter from esp3 to esp2 for Home Assistant Eltako Integration
 Home-page: https://github.com/grimmpp/esp2_gateway_adapter
 Author: Philipp Grimm
 License: MIT License
         
         Copyright (c) 2024 Philipp Grimm
         
@@ -30,13 +30,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: eltako14bus>=0.0.46
 Requires-Dist: enocean>=0.60.1
 Requires-Dist: pyserial
 Requires-Dist: pyserial-asyncio
 Requires-Dist: aiocoap
+Requires-Dist: zeroconf==0.132.2
 
-# EnOcean ESP3 to ESP3 Gateway Adapter
+# EnOcean ESP3 to ESP2 Gateway Adapter
 
 EnOcean gateway adapter from ESP3 to ESP2 for [Eltako Home Assistant Integration](https://github.com/grimmpp/home-assistant-eltako).
 
-This component is mainly required to support USB300, USB400 and USB500 (Wireless EnOcean USB stick/transceiver) which is using ESP3 protocol unlike all other Eltako devices which are using ESP2.
+This component is mainly required to support USB300, USB400 and USB515 (Wireless EnOcean USB stick/transceiver) which is using ESP3 protocol unlike all other Eltako devices which are using ESP2.
+
+Support for [Enocean Multigateway (MGW) LAN and Wifi](https://www.piotek.de/PioTek-MGW-POE).
```

### Comparing `esp2_gateway_adapter-0.1/esp2_gateway_adapter.egg-info/PKG-INFO` & `esp2_gateway_adapter-0.2/esp2_gateway_adapter.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp2_gateway_adapter
-Version: 0.1
+Version: 0.2
 Summary: Protocol adapter from esp3 to esp2 for Home Assistant Eltako Integration
 Home-page: https://github.com/grimmpp/esp2_gateway_adapter
 Author: Philipp Grimm
 License: MIT License
         
         Copyright (c) 2024 Philipp Grimm
         
@@ -30,13 +30,16 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: eltako14bus>=0.0.46
 Requires-Dist: enocean>=0.60.1
 Requires-Dist: pyserial
 Requires-Dist: pyserial-asyncio
 Requires-Dist: aiocoap
+Requires-Dist: zeroconf==0.132.2
 
-# EnOcean ESP3 to ESP3 Gateway Adapter
+# EnOcean ESP3 to ESP2 Gateway Adapter
 
 EnOcean gateway adapter from ESP3 to ESP2 for [Eltako Home Assistant Integration](https://github.com/grimmpp/home-assistant-eltako).
 
-This component is mainly required to support USB300, USB400 and USB500 (Wireless EnOcean USB stick/transceiver) which is using ESP3 protocol unlike all other Eltako devices which are using ESP2.
+This component is mainly required to support USB300, USB400 and USB515 (Wireless EnOcean USB stick/transceiver) which is using ESP3 protocol unlike all other Eltako devices which are using ESP2.
+
+Support for [Enocean Multigateway (MGW) LAN and Wifi](https://www.piotek.de/PioTek-MGW-POE).
```

### Comparing `esp2_gateway_adapter-0.1/setup.py` & `esp2_gateway_adapter-0.2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,21 +10,21 @@
 with open('README.md', encoding="utf-8") as f:
     long_description = f.read()
 
 # with open(os.path.join(base_dir, 'LICENSE'), encoding="utf-8") as f:
 with open('LICENSE', encoding="utf-8") as f:
     license = f.read()
 
-required = ['eltako14bus>=0.0.46', 'enocean>=0.60.1', 'pyserial', 'pyserial-asyncio', 'aiocoap']
+required = ['eltako14bus>=0.0.46', 'enocean>=0.60.1', 'pyserial', 'pyserial-asyncio', 'aiocoap', 'zeroconf==0.132.2']
 
 
 
 setup(
     name='esp2_gateway_adapter',
-    version='0.1',
+    version='0.2',
     package_dir={"esp2_gateway_adapter":'src'},
     package=[""],
     include_package_data=True,
     install_requires=required,
     author="Philipp Grimm",
     description="Protocol adapter from esp3 to esp2 for Home Assistant Eltako Integration",
     long_description=long_description,
```

### Comparing `esp2_gateway_adapter-0.1/src/esp3_serial_com.py` & `esp2_gateway_adapter-0.2/src/esp3_serial_com.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
             body:bytes = bytes([in_or_out, org] + packet.data[1:2] + [0,0,0] + packet.data[2:])
 
         return prettify( ESP2Message(body) )
     
 
     def __callback_wrapper(self, msg: Packet):
         if msg.packet_type == PACKET.RESPONSE and msg.data[0] != RETURN_CODE.OK:
-            self.log.error(f"Received ESP3 response with with return code {RETURN_CODE(msg.data[0]).name} ({msg.data[0]}) - {str(msg)} ")
+            self.log.error(f"Received ESP3 response with return code {RETURN_CODE(msg.data[0]).name} ({msg.data[0]}) - {str(msg)} ")
             return
 
         if self._outside_callback:
             if self.esp2_translation_enabled:
                 # only when message is radio telegram
                 if msg.packet_type == PACKET.RADIO:
                     esp2_msg = ESP3SerialCommunicator.convert_esp3_to_esp2_message(msg)
```

