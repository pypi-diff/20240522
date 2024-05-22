# Comparing `tmp/e2tapi-0.0.3.tar.gz` & `tmp/e2tapi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2tapi-0.0.3.tar", last modified: Wed May 22 19:36:20 2024, max compression
+gzip compressed data, was "e2tapi-0.0.4.tar", last modified: Wed May 22 20:10:04 2024, max compression
```

## Comparing `e2tapi-0.0.3.tar` & `e2tapi-0.0.4.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-22 19:36:20.287986 e2tapi-0.0.3/
--rw-r--r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6641 2024-05-22 19:36:20.287986 e2tapi-0.0.3/PKG-INFO
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6188 2024-05-22 15:19:56.000000 e2tapi-0.0.3/README.md
-drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-22 19:36:20.279986 e2tapi-0.0.3/e2tapi.egg-info/
--rw-r--r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6641 2024-05-22 19:36:20.000000 e2tapi-0.0.3/e2tapi.egg-info/PKG-INFO
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)      301 2024-05-22 19:36:20.000000 e2tapi-0.0.3/e2tapi.egg-info/SOURCES.txt
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        1 2024-05-22 19:36:20.000000 e2tapi-0.0.3/e2tapi.egg-info/dependency_links.txt
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       16 2024-05-22 19:36:20.000000 e2tapi-0.0.3/e2tapi.egg-info/requires.txt
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       12 2024-05-22 19:36:20.000000 e2tapi-0.0.3/e2tapi.egg-info/top_level.txt
-drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-22 19:36:20.283986 e2tapi-0.0.3/mktdata/
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    42596 2024-05-22 19:35:52.000000 e2tapi-0.0.3/mktdata/IBKR_MDG_Messages_pb2.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       23 2024-05-22 19:35:52.000000 e2tapi-0.0.3/mktdata/__init__.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6011 2024-05-22 19:35:52.000000 e2tapi-0.0.3/mktdata/ibkr_api.py
-drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-22 19:36:20.283986 e2tapi-0.0.3/oms/
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    26353 2024-05-20 17:41:14.000000 e2tapi-0.0.3/oms/IBKR_OMS_Messages_pb2.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       23 2024-05-22 16:24:57.000000 e2tapi-0.0.3/oms/__init__.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     4490 2024-05-22 17:14:31.000000 e2tapi-0.0.3/oms/ibkr_api.py
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       38 2024-05-22 19:36:20.287986 e2tapi-0.0.3/setup.cfg
--rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)      697 2024-05-22 19:36:06.000000 e2tapi-0.0.3/setup.py
+drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-22 20:10:04.732421 e2tapi-0.0.4/
+-rw-r--r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6641 2024-05-22 20:10:04.732421 e2tapi-0.0.4/PKG-INFO
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6188 2024-05-22 15:19:56.000000 e2tapi-0.0.4/README.md
+drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-22 20:10:04.724420 e2tapi-0.0.4/e2t/
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       40 2024-05-22 20:09:16.000000 e2tapi-0.0.4/e2t/__init__.py
+drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-22 20:10:04.724420 e2tapi-0.0.4/e2t/mktdata/
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    42596 2024-05-22 19:35:52.000000 e2tapi-0.0.4/e2t/mktdata/IBKR_MDG_Messages_pb2.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       19 2024-05-22 20:08:02.000000 e2tapi-0.0.4/e2t/mktdata/__init__.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6011 2024-05-22 19:54:27.000000 e2tapi-0.0.4/e2t/mktdata/ibkr.py
+drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-22 20:10:04.728420 e2tapi-0.0.4/e2t/oms/
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)    26353 2024-05-20 17:41:14.000000 e2tapi-0.0.4/e2t/oms/IBKR_OMS_Messages_pb2.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       19 2024-05-22 20:08:02.000000 e2tapi-0.0.4/e2t/oms/__init__.py
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     4494 2024-05-22 20:08:02.000000 e2tapi-0.0.4/e2t/oms/ibkr.py
+drwxrwxr-x   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        0 2024-05-22 20:10:04.732421 e2tapi-0.0.4/e2tapi.egg-info/
+-rw-r--r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)     6641 2024-05-22 20:10:04.000000 e2tapi-0.0.4/e2tapi.egg-info/PKG-INFO
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)      333 2024-05-22 20:10:04.000000 e2tapi-0.0.4/e2tapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        1 2024-05-22 20:10:04.000000 e2tapi-0.0.4/e2tapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       16 2024-05-22 20:10:04.000000 e2tapi-0.0.4/e2tapi.egg-info/requires.txt
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)        4 2024-05-22 20:10:04.000000 e2tapi-0.0.4/e2tapi.egg-info/top_level.txt
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)       38 2024-05-22 20:10:04.732421 e2tapi-0.0.4/setup.cfg
+-rw-rw-r--   0 alvaroodescalchi  (1002) alvaroodescalchi  (1002)      697 2024-05-22 20:09:35.000000 e2tapi-0.0.4/setup.py
```

### Comparing `e2tapi-0.0.3/PKG-INFO` & `e2tapi-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: e2tapi
-Version: 0.0.3
-Summary: SDK for E2T OMS
+Version: 0.0.4
+Summary: SDK for e2t OMS
 Home-page: http://gitlab.event2trading.com/utilities/e2tapi.git
 Author: Event2trading
 Author-email: admin@event2trading.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `e2tapi-0.0.3/README.md` & `e2tapi-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `e2tapi-0.0.3/e2tapi.egg-info/PKG-INFO` & `e2tapi-0.0.4/e2tapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: e2tapi
-Version: 0.0.3
-Summary: SDK for E2T OMS
+Version: 0.0.4
+Summary: SDK for e2t OMS
 Home-page: http://gitlab.event2trading.com/utilities/e2tapi.git
 Author: Event2trading
 Author-email: admin@event2trading.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `e2tapi-0.0.3/mktdata/IBKR_MDG_Messages_pb2.py` & `e2tapi-0.0.4/e2t/mktdata/IBKR_MDG_Messages_pb2.py`

 * *Files identical despite different names*

### Comparing `e2tapi-0.0.3/mktdata/ibkr_api.py` & `e2tapi-0.0.4/e2t/mktdata/ibkr.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,55 +13,55 @@
 class E2T_MKTDATA():
 
     @abstractmethod
     def snapshot(self, message):
         pass
 
     @abstractmethod
-    def bid(self, type, symbol, value):
+    def bid(self, symbol, type, value):
         pass
 
     @abstractmethod
-    def bidQty(self, type, symbol, value):
+    def bidQty(self, symbol, type, value):
         pass
 
     @abstractmethod
-    def offer(self, type, symbol, value):
+    def offer(self, symbol, type, value):
         pass
 
     @abstractmethod
-    def offerQty(self, type, symbol, value):
+    def offerQty(self, symbol, type, value):
         pass
 
     @abstractmethod
-    def last(self, type, symbol, value):
+    def last(self, symbol, type, value):
         pass
 
     @abstractmethod
-    def lastQty(self, type, symbol, value):
+    def lastQty(self, symbol, type, value):
         pass
 
     @abstractmethod
-    def open(self, type, symbol, value):
+    def open(self, symbol, type, value):
         pass
 
     @abstractmethod
-    def close(self, type, symbol, value):
+    def close(self, symbol, type, value):
         pass
 
     @abstractmethod
-    def high(self, type, symbol, value):
+    def high(self, symbol, type, value):
         pass
 
     @abstractmethod
-    def low(self, type, symbol, value):
+    def low(self, symbol, type, value):
         pass
 
     @abstractmethod
-    def volume(self, type, symbol, value):
+    def volume(self, symbol, type, value):
         pass
 
     def connect(self, HOST, PORT):
         self.client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self.client.connect((HOST, PORT))
         print(f"Conectado a {HOST}:{PORT}...")
 
@@ -75,76 +75,76 @@
                     # Decode the length prefix
                     size, new_pos = _DecodeVarint32(data, 0)
                     message.ParseFromString(data[new_pos:new_pos + size])
                     if message.messageType == pb.MessageType.SNAPSHOT:
                         print(message)
                     elif message.messageType == pb.MessageType.BID:
                         self.bid(
-                            'BID',
                             message.bid.symbol,
+                            'BID',
                             message.bid.bid
                         )
                     elif message.messageType == pb.MessageType.BIDQTY:
                         self.bidQty(
-                            'BIDQTY',
                             message.bidQty.symbol,
+                            'BIDQTY',
                             message.bidQty.bidQty
                         )
                     elif message.messageType == pb.MessageType.OFFER:
                         self.offer(
-                            'OFFER',
                             message.offer.symbol,
+                            'OFFER',
                             message.offer.offer
                         )
                     elif message.messageType == pb.MessageType.OFFERQTY:
                         self.offerQty(
-                            'OFFERQTY',
                             message.offerQty.symbol,
+                            'OFFERQTY',
                             message.offerQty.offerQty
                         )
                     elif message.messageType == pb.MessageType.LAST:
                         self.last(
-                            'LAST',
                             message.last.symbol,
+                            'LAST',
                             message.last.last
                         )
                     elif message.messageType == pb.MessageType.LASTQTY:
                         self.lastQty(
-                            'LASTQTY',
                             message.lastQty.symbol,
+                            'LASTQTY',
                             message.lastQty.lastQty
                         )
                     elif message.messageType == pb.MessageType.OPEN:
                         self.open(
-                            'OPEN',
                             message.open.symbol,
+                            'OPEN',
                             message.open.open
                         )
                     elif message.messageType == pb.MessageType.CLOSE:
                         self.close(
-                            'CLOSE',
                             message.close.symbol,
+                            'CLOSE',
                             message.close.close
                         )
                     elif message.messageType == pb.MessageType.HIGH:
                         self.high(
-                            'HIGH',
                             message.high.symbol,
+                            'HIGH',
                             message.high.high
                         )
                     elif message.messageType == pb.MessageType.LOW:
                         self.low(
-                            'LOW',
                             message.low.symbol,
+                            'LOW',
                             message.low.low
                         )
                     elif message.messageType == pb.MessageType.VOLUME:
                         self.volume(
-                            'VOLUME',
                             message.volume.symbol,
+                            'VOLUME',
                             message.volume.volume
                         )
                 except DecodeError as e:
                     print(f"Error decoding message: {e}")
                     break
 
         threading.Thread(target=handle_client, daemon=True).start()
```

### Comparing `e2tapi-0.0.3/oms/IBKR_OMS_Messages_pb2.py` & `e2tapi-0.0.4/e2t/oms/IBKR_OMS_Messages_pb2.py`

 * *Files identical despite different names*

### Comparing `e2tapi-0.0.3/oms/ibkr_api.py` & `e2tapi-0.0.4/e2t/oms/ibkr.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import random
 import string
 from google.protobuf.message import DecodeError
 from google.protobuf.internal.encoder import _VarintBytes
 from google.protobuf.internal.decoder import _DecodeVarint32
 from abc import abstractmethod
 
-from oms import IBKR_OMS_Messages_pb2 as pb
+from e2t.oms import IBKR_OMS_Messages_pb2 as pb
 
 
 class E2T_OMS:
 
     @abstractmethod
     def status(self, requestId, orderId, live, cumQty, leavesQty, avgPx, lastPx):
         pass
```

### Comparing `e2tapi-0.0.3/setup.py` & `e2tapi-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from setuptools import setup, find_packages
 
 setup(
     name='e2tapi',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     install_requires=[
         'protobuf>=3.0.0',
     ],
     include_package_data=True,
-    description='SDK for E2T OMS',
+    description='SDK for e2t OMS',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='http://gitlab.event2trading.com/utilities/e2tapi.git',
     author='Event2trading',
     author_email='admin@event2trading.com',
     license='MIT',
     classifiers=[
```

