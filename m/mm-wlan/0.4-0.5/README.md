# Comparing `tmp/mm_wlan-0.4.tar.gz` & `tmp/mm_wlan-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mm_wlan-0.4.tar", last modified: Mon May 20 13:15:56 2024, max compression
+gzip compressed data, was "mm_wlan-0.5.tar", last modified: Wed May 22 09:09:59 2024, max compression
```

## Comparing `mm_wlan-0.4.tar` & `mm_wlan-0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 si         (502) staff       (20)        0 2024-05-20 13:15:56.125109 mm_wlan-0.4/
--rw-r--r--   0 si         (502) staff       (20)     1062 2023-10-05 12:41:54.000000 mm_wlan-0.4/LICENSE.txt
--rw-r--r--   0 si         (502) staff       (20)      701 2024-05-20 13:15:56.124828 mm_wlan-0.4/PKG-INFO
--rw-r--r--   0 si         (502) staff       (20)     2053 2024-05-20 13:05:12.000000 mm_wlan-0.4/README.md
-drwxr-xr-x   0 si         (502) staff       (20)        0 2024-05-20 13:15:56.121532 mm_wlan-0.4/mm_wlan/
--rw-r--r--   0 si         (502) staff       (20)       61 2024-01-11 15:35:33.000000 mm_wlan-0.4/mm_wlan/__init__.py
--rw-r--r--   0 si         (502) staff       (20)     1119 2024-05-20 13:05:12.000000 mm_wlan-0.4/mm_wlan/mm_wlan.py
-drwxr-xr-x   0 si         (502) staff       (20)        0 2024-05-20 13:15:56.124203 mm_wlan-0.4/mm_wlan.egg-info/
--rw-r--r--   0 si         (502) staff       (20)      701 2024-05-20 13:15:56.000000 mm_wlan-0.4/mm_wlan.egg-info/PKG-INFO
--rw-r--r--   0 si         (502) staff       (20)      203 2024-05-20 13:15:56.000000 mm_wlan-0.4/mm_wlan.egg-info/SOURCES.txt
--rw-r--r--   0 si         (502) staff       (20)        1 2024-05-20 13:15:56.000000 mm_wlan-0.4/mm_wlan.egg-info/dependency_links.txt
--rw-r--r--   0 si         (502) staff       (20)        8 2024-05-20 13:15:56.000000 mm_wlan-0.4/mm_wlan.egg-info/top_level.txt
--rw-r--r--   0 si         (502) staff       (20)       79 2024-05-20 13:15:56.125723 mm_wlan-0.4/setup.cfg
--rw-r--r--   0 si         (502) staff       (20)      913 2024-05-20 13:14:39.000000 mm_wlan-0.4/setup.py
+drwxr-xr-x   0 si         (502) staff       (20)        0 2024-05-22 09:09:59.439902 mm_wlan-0.5/
+-rw-r--r--   0 si         (502) staff       (20)     1062 2023-10-05 12:41:54.000000 mm_wlan-0.5/LICENSE.txt
+-rw-r--r--   0 si         (502) staff       (20)      701 2024-05-22 09:09:59.439670 mm_wlan-0.5/PKG-INFO
+-rw-r--r--   0 si         (502) staff       (20)     2053 2024-05-20 13:05:12.000000 mm_wlan-0.5/README.md
+drwxr-xr-x   0 si         (502) staff       (20)        0 2024-05-22 09:09:59.436573 mm_wlan-0.5/mm_wlan/
+-rw-r--r--   0 si         (502) staff       (20)       69 2024-05-22 09:05:01.000000 mm_wlan-0.5/mm_wlan/__init__.py
+-rw-r--r--   0 si         (502) staff       (20)     1889 2024-05-22 09:05:01.000000 mm_wlan-0.5/mm_wlan/mm_wlan.py
+drwxr-xr-x   0 si         (502) staff       (20)        0 2024-05-22 09:09:59.439009 mm_wlan-0.5/mm_wlan.egg-info/
+-rw-r--r--   0 si         (502) staff       (20)      701 2024-05-22 09:09:59.000000 mm_wlan-0.5/mm_wlan.egg-info/PKG-INFO
+-rw-r--r--   0 si         (502) staff       (20)      203 2024-05-22 09:09:59.000000 mm_wlan-0.5/mm_wlan.egg-info/SOURCES.txt
+-rw-r--r--   0 si         (502) staff       (20)        1 2024-05-22 09:09:59.000000 mm_wlan-0.5/mm_wlan.egg-info/dependency_links.txt
+-rw-r--r--   0 si         (502) staff       (20)        8 2024-05-22 09:09:59.000000 mm_wlan-0.5/mm_wlan.egg-info/top_level.txt
+-rw-r--r--   0 si         (502) staff       (20)       79 2024-05-22 09:09:59.440526 mm_wlan-0.5/setup.cfg
+-rw-r--r--   0 si         (502) staff       (20)      913 2024-05-22 09:05:19.000000 mm_wlan-0.5/setup.py
```

### Comparing `mm_wlan-0.4/LICENSE.txt` & `mm_wlan-0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mm_wlan-0.4/PKG-INFO` & `mm_wlan-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mm_wlan
-Version: 0.4
+Version: 0.5
 Summary: WLAN Connection functions in MicroPython
 Home-page: https://github.com/monkmakes/mm_wlan
 Download-URL: https://github.com/monkmakes/mm_wlan/archive/refs/tags/v_02.tar.gz
 Author: Simon Monk and José Antonio Vacas
 Author-email: simon@monkmakes.com
 License: MIT
 Keywords: WLAN,micropython,webserver
```

### Comparing `mm_wlan-0.4/README.md` & `mm_wlan-0.5/README.md`

 * *Files identical despite different names*

### Comparing `mm_wlan-0.4/mm_wlan/mm_wlan.py` & `mm_wlan-0.5/mm_wlan/mm_wlan.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,41 +2,53 @@
 mm_wlan
 --------
 The ``mm_wlan`` module defines a couple of methods to simplify connecting to a 
 wireless network. https://github.com/monkmakes/mm_wlan
 
 """
 
-
 import network, time, sys
 
 wlan = network.WLAN(network.STA_IF)
 
 def connect_to_network(ssid, password, retries=10, verbose=True):
     wlan.active(True)
     if sys.platform != 'esp32':
         wlan.config(pm = 0xa11140)  # Disable power-save mode
     wlan.connect(ssid, password)
     if verbose: print('Connecting to ' + ssid, end=' ')
         
-    while retries > 0 and wlan.status() != network.STAT_GOT_IP:
+    while retries > 0 and wlan.status() in (network.STAT_CONNECTING ,2) : # 2 STAT_NOIP https://github.com/orgs/micropython/discussions/10746
         retries -= 1
         if verbose: print('.', end='')
         time.sleep(1)    
-        
-    if is_connected():
-        if verbose: print('\nConnection failed. Check ssid and password')
+    # wifi status https://docs.micropython.org/en/latest/library/network.WLAN.html    
+    if not is_connected():
+        if verbose:
+            if wlan.status() == network.STAT_CONNECTING :
+                print('\nStill connecting, try later')
+            elif wlan.status() == network.STAT_WRONG_PASSWORD:
+                print('\nConnection failed. Check password')
+            elif wlan.status() == network.STAT_NO_AP_FOUND:  
+                print('\nConnection failed. Check ssid')
+                print('Available networks:')
+                for red in wlan.scan():
+                    print(red[0])
+            elif wlan.status() == network.STAT_CONNECT_FAIL:
+                print('\nConnection failed. Unkown error')
+            else :
+                print(f'\nStatus:{wlan.status()}')
         raise RuntimeError('WLAN connection failed')
     else:
         if verbose: print('\nConnected. IP Address = ' + get_ip())
 
 def get_ip():
     if is_connected():
         return wlan.ifconfig()[0]
     else:
         if verbose: print('\nNot connected')
         return None
         
-
 def is_connected():
     return wlan.status() == network.STAT_GOT_IP
 
+
```

### Comparing `mm_wlan-0.4/mm_wlan.egg-info/PKG-INFO` & `mm_wlan-0.5/mm_wlan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mm_wlan
-Version: 0.4
+Version: 0.5
 Summary: WLAN Connection functions in MicroPython
 Home-page: https://github.com/monkmakes/mm_wlan
 Download-URL: https://github.com/monkmakes/mm_wlan/archive/refs/tags/v_02.tar.gz
 Author: Simon Monk and José Antonio Vacas
 Author-email: simon@monkmakes.com
 License: MIT
 Keywords: WLAN,micropython,webserver
```

### Comparing `mm_wlan-0.4/setup.py` & `mm_wlan-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'mm_wlan',         
   packages = ['mm_wlan'],   
-  version = '0.4',      
+  version = '0.5',      
   license='MIT',       
   description = 'WLAN Connection functions in MicroPython',  
   author = 'Simon Monk and José Antonio Vacas',                  
   author_email = 'simon@monkmakes.com',      
   url = 'https://github.com/monkmakes/mm_wlan',  
   download_url = 'https://github.com/monkmakes/mm_wlan/archive/refs/tags/v_02.tar.gz',   
   keywords = ['WLAN', 'micropython', 'webserver'],
```

