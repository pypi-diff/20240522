# Comparing `tmp/zur_ecu_client-0.0.7.tar.gz` & `tmp/zur_ecu_client-0.0.8.tar.gz`

## Comparing `zur_ecu_client-0.0.7.tar` & `zur_ecu_client-0.0.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/__about__.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/requirements.txt
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.github/workflows/black.yml
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.github/workflows/publish-to-test-pypi.yaml
--rw-r--r--   0        0        0     1353 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.idea/.gitignore
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.idea/ECU-Client.iml
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.idea/misc.xml
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.idea/modules.xml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.idea/vcs.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.idea/runConfigurations/pytest.xml
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.vscode/settings.json
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/__init__.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/ecu_client.py
--rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/messages.py
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/mock_ecu.py
--rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/udp_server.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/senml/__init__.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml_msg.py
--rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml_msg_dv.py
--rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml_msg_ecu.py
--rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml_unit.py
--rw-r--r--   0        0        0     6423 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml_zur_names.py
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/src/zur_ecu_client/senml/util.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/tests/test_messages.py
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/tests/test_sample.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/LICENSE.txt
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/README.md
--rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/__about__.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/requirements.txt
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/.github/workflows/black.yml
+-rw-r--r--   0        0        0     3362 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/.github/workflows/publish-to-test-pypi.yaml
+-rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/.idea/.gitignore
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/.idea/ECU-Client.iml
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/.idea/misc.xml
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/.idea/modules.xml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/.idea/vcs.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     1050 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/.idea/runConfigurations/pytest.xml
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/.vscode/settings.json
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/src/zur_ecu_client/__init__.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/src/zur_ecu_client/ecu_client.py
+-rw-r--r--   0        0        0     2531 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/src/zur_ecu_client/messages.py
+-rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/src/zur_ecu_client/mock_ecu.py
+-rw-r--r--   0        0        0     1028 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/src/zur_ecu_client/udp_server.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/src/zur_ecu_client/senml/__init__.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/src/zur_ecu_client/senml/senml.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/src/zur_ecu_client/senml/senml_msg.py
+-rw-r--r--   0        0        0     3452 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/src/zur_ecu_client/senml/senml_msg_dv.py
+-rw-r--r--   0        0        0     5305 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/src/zur_ecu_client/senml/senml_msg_ecu.py
+-rw-r--r--   0        0        0     1334 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/src/zur_ecu_client/senml/senml_unit.py
+-rw-r--r--   0        0        0     6467 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/src/zur_ecu_client/senml/senml_zur_names.py
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/src/zur_ecu_client/senml/util.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/tests/test_messages.py
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/tests/test_sample.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/LICENSE.txt
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/README.md
+-rw-r--r--   0        0        0     2041 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 zur_ecu_client-0.0.8/PKG-INFO
```

### Comparing `zur_ecu_client-0.0.7/.github/workflows/publish-to-test-pypi.yaml` & `zur_ecu_client-0.0.8/.github/workflows/publish-to-test-pypi.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 on:
   workflow_dispatch:
   push:
     tags:
        - '*.*.*'
     branches:
-      - develop
       - main
 jobs:
   build:
     name: Build distribution 📦
     runs-on: ubuntu-latest
 
     steps:
```

### Comparing `zur_ecu_client-0.0.7/.github/workflows/python-package.yml` & `zur_ecu_client-0.0.8/.github/workflows/python-package.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 # This workflow will install Python dependencies, run tests and lint with a variety of Python versions
 # For more information see: https://docs.github.com/en/actions/automating-builds-and-tests/building-and-testing-python
 
 name: Python package
 
 on:
-  push:
+  pull_request:
     branches: [ "develop" ]
     paths:
       - 'src/**'
       - 'tests/**'
-  pull_request:
-    branches: [ "develop" ]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     strategy:
       fail-fast: false
```

### Comparing `zur_ecu_client-0.0.7/.idea/runConfigurations/pytest.xml` & `zur_ecu_client-0.0.8/.idea/runConfigurations/pytest.xml`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.7/src/zur_ecu_client/ecu_client.py` & `zur_ecu_client-0.0.8/src/zur_ecu_client/ecu_client.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import json
 import logging
 import sched
 import time
 from threading import Thread
 
-from .senml import SenmlNames
+from .senml import SenmlNames, Dv, Ecu
 from .udp_server import UdpServer
 
 
 class EcuClient:
 
     def __init__(
         self, listener, ecu_ip: str, ecu_port: int, calls_per_second: int
     ) -> None:
+        logging.basicConfig(level=logging.DEBUG)
         self.listener = listener
         self.requestInterval = 1.0 / calls_per_second
         self.subscriptions: dict[SenmlNames, list[callable]] = {}
         self.compiledMessages = []
 
         self.ecuIP = ecu_ip
         self.ecuPort = ecu_port
 
-        self.udpServer = UdpServer(ecu_ip, ecu_port, "127.0.0.1", 9000)
+        self.udpServer = UdpServer("127.0.0.1", 9000, ecu_ip, ecu_port)
 
         self.thread1 = Thread(target=self.__receive_msg)
-        self.thread1.daemon = True
+        # self.thread1.daemon = True
         self.thread2 = Thread(target=self.__schedule_requests)
-        self.thread2.daemon = True
+        # self.thread2.daemon = True
 
     def start(self):
         self.thread1.start()
         self.thread2.start()
 
     def subscribe(self, data_field: SenmlNames, subscriber: callable):
         if data_field in self.subscriptions:
@@ -43,31 +44,50 @@
         if data_field in self.subscriptions:
             self.subscriptions.get(data_field).remove(subscriber)
             if not self.subscriptions[data_field]:
                 self.subscriptions.pop(data_field)
             self.__compile_subscriptions()
 
     def send_msg(self, msg):
-        msg = json.dumps(msg).encode("utf-8")
+        msg = json.dumps(msg)
         self.udpServer.send_data(msg)
 
     def __compile_subscriptions(self):
         for msg in self.subscriptions:
             self.compiledMessages.append({"bn": "ECU", "n": msg, "v": "request"})
 
     def __receive_msg(self):
         while True:
             data = self.udpServer.receive_data()
             if data:
-                data = data.decode("utf-8")
                 logging.info(f"Received -> {data}")
 
     def __request_messages(self):
         bn_request = []
 
-        self.send_msg(bn_request)
+        self.send_msg(self.compiledMessages)
 
     def __schedule_requests(self):
         scheduler = sched.scheduler(time.time, time.sleep)
         while True:
             scheduler.enter(self.requestInterval, 1, self.__request_messages, ())
             scheduler.run()
+
+
+def __main__():
+    mock_ecu = EcuClient(None, "127.0.0.1", 9001, 1)
+    # msg = Ecu.Pedal(0, 0, 0).get()
+    msg = Dv.Ctrl(0, 0, 0, "Hello World!").get()
+
+    try:
+        mock_ecu.start()
+        # mock_ecu.subscribe("ECU:accu:sensor", None)  # Send a request to server
+        for item in msg:
+            mock_ecu.compiledMessages.append(item)  # for sending data to server
+        # mock_ecu.send_msg(msg)
+
+    except KeyboardInterrupt:
+        mock_ecu.udpServer.close()
+
+
+if __name__ == "__main__":
+    __main__()
```

### Comparing `zur_ecu_client-0.0.7/src/zur_ecu_client/messages.py` & `zur_ecu_client-0.0.8/src/zur_ecu_client/messages.py`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.7/src/zur_ecu_client/udp_server.py` & `zur_ecu_client-0.0.8/src/zur_ecu_client/udp_server.py`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml.py` & `zur_ecu_client-0.0.8/src/zur_ecu_client/senml/senml.py`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml_msg.py` & `zur_ecu_client-0.0.8/src/zur_ecu_client/senml/senml_msg.py`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml_msg_dv.py` & `zur_ecu_client-0.0.8/src/zur_ecu_client/senml/senml_msg_dv.py`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml_msg_ecu.py` & `zur_ecu_client-0.0.8/src/zur_ecu_client/senml/senml_msg_ecu.py`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml_unit.py` & `zur_ecu_client-0.0.8/src/zur_ecu_client/senml/senml_unit.py`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.7/src/zur_ecu_client/senml/senml_zur_names.py` & `zur_ecu_client-0.0.8/src/zur_ecu_client/senml/senml_zur_names.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 from enum import Enum
 
 
 class SenmlNames(Enum):
     # ========== DV ==========
     # DV:cfg
-    DV_CFG = "DV:cfg"
+    DV_CFG = "DV:cfg:controller"
     DV_CFG_AS = "DV:cfg:AS"
     DV_CFG_EBS = "DV:cfg:EBS"
     DV_CFG_AMI = "DV:cfg:AMI"
     # DV:ctrl
-    DV_CTRL = "DV:ctrl"
+    DV_CTRL = "DV:ctrl:controller"
     DV_CTRL_BRAKE = "DV:ctrl:brake"
     DV_CTRL_STEERING = "DV:ctrl:steering"
     DV_CTRL_THROTTLE = "DV:ctrl:throttle"
     DV_CTRL_STATUS = "DV:ctrl:status"
     # DV:stat
-    DV_STAT = "DV:stat"
+    DV_STAT = "DV:stat:controller"
     DV_STAT_LAPS = "DV:stat:laps"
     DV_STAT_CONESACT = "DV:stat:conesAct"
     DV_STAT_CONESALL = "DV:stat:conesAll"
     # DV:acc
-    DV_ACC = "DV:acc"
+    DV_ACC = "DV:acc:controller"
     DV_ACC_X = "DV:acc:X"
     DV_ACC_Y = "DV:acc:Y"
     DV_ACC_Z = "DV:acc:Z"
     # ========== ECU ==========
     # ECU:pedal
     ECU_PEDAL = "ECU:pedal:sensor"
     ECU_PEDAL_BRAKE = "ECU:pedal:sensor:brake"
```

### Comparing `zur_ecu_client-0.0.7/tests/test_messages.py` & `zur_ecu_client-0.0.8/tests/test_messages.py`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.7/tests/test_sample.py` & `zur_ecu_client-0.0.8/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.7/.gitignore` & `zur_ecu_client-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.7/LICENSE.txt` & `zur_ecu_client-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.7/pyproject.toml` & `zur_ecu_client-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zur_ecu_client-0.0.7/PKG-INFO` & `zur_ecu_client-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: zur_ecu_client
-Version: 0.0.7
+Version: 0.0.8
 Summary: Internal Python library which provides an interface to the ECU
 Project-URL: Homepage, https://zurichuasracing.ch
 Project-URL: Bug Reports, https://github.com/zurich-uas-racing/issues
 Project-URL: Source, https://github.com/zurich-uas-racing/ecu-client
 Author-email: ZUR Driverless <driverless@zurichuasracing.ch>, Finn Scheller <finn.scheller@zurichuasracing.ch>, Cèline Brun <bruncel1@students.zhaw.ch>
 Maintainer-email: ZUR Driverless <driverless@zurichuasracing.ch>
 License: MIT License
```

