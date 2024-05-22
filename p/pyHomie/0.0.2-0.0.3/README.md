# Comparing `tmp/pyhomie-0.0.2.tar.gz` & `tmp/pyhomie-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhomie-0.0.2.tar", last modified: Wed May 22 13:49:13 2024, max compression
+gzip compressed data, was "pyhomie-0.0.3.tar", last modified: Wed May 22 13:59:35 2024, max compression
```

## Comparing `pyhomie-0.0.2.tar` & `pyhomie-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 13:49:13.951217 pyhomie-0.0.2/
--rw-rw-rw-   0        0        0       54 2024-05-22 13:49:13.949220 pyhomie-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1242 2024-04-02 13:39:48.000000 pyhomie-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 13:49:13.872973 pyhomie-0.0.2/pyHomie/
--rw-rw-rw-   0        0        0       34 2024-05-22 12:50:53.000000 pyhomie-0.0.2/pyHomie/__init__.py
--rw-rw-rw-   0        0        0     5191 2024-05-22 12:40:28.000000 pyhomie-0.0.2/pyHomie/device.py
--rw-rw-rw-   0        0        0     4820 2024-04-25 21:50:24.000000 pyhomie-0.0.2/pyHomie/mqttClient.py
--rw-rw-rw-   0        0        0     2129 2024-05-22 12:40:28.000000 pyhomie-0.0.2/pyHomie/node.py
--rw-rw-rw-   0        0        0    10885 2024-05-17 22:08:42.000000 pyhomie-0.0.2/pyHomie/properties.py
--rw-rw-rw-   0        0        0     7612 2024-05-22 12:48:29.000000 pyhomie-0.0.2/pyHomie/pyHomie.py
--rw-rw-rw-   0        0        0      894 2024-04-02 11:37:16.000000 pyhomie-0.0.2/pyHomie/watchdog.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:49:13.945180 pyhomie-0.0.2/pyHomie.egg-info/
--rw-rw-rw-   0        0        0       54 2024-05-22 13:49:13.000000 pyhomie-0.0.2/pyHomie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2024-05-22 13:49:13.000000 pyhomie-0.0.2/pyHomie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 13:49:13.000000 pyhomie-0.0.2/pyHomie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-22 13:49:13.000000 pyhomie-0.0.2/pyHomie.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 13:49:13.952216 pyhomie-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      202 2024-05-22 13:49:07.000000 pyhomie-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:59:35.497247 pyhomie-0.0.3/
+-rw-rw-rw-   0        0        0      854 2024-05-22 13:59:35.493217 pyhomie-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1242 2024-04-02 13:39:48.000000 pyhomie-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 13:59:35.459724 pyhomie-0.0.3/pyHomie/
+-rw-rw-rw-   0        0        0       34 2024-05-22 12:50:53.000000 pyhomie-0.0.3/pyHomie/__init__.py
+-rw-rw-rw-   0        0        0     5191 2024-05-22 12:40:28.000000 pyhomie-0.0.3/pyHomie/device.py
+-rw-rw-rw-   0        0        0     4820 2024-04-25 21:50:24.000000 pyhomie-0.0.3/pyHomie/mqttClient.py
+-rw-rw-rw-   0        0        0     2129 2024-05-22 12:40:28.000000 pyhomie-0.0.3/pyHomie/node.py
+-rw-rw-rw-   0        0        0    10885 2024-05-17 22:08:42.000000 pyhomie-0.0.3/pyHomie/properties.py
+-rw-rw-rw-   0        0        0     7612 2024-05-22 12:48:29.000000 pyhomie-0.0.3/pyHomie/pyHomie.py
+-rw-rw-rw-   0        0        0      894 2024-04-02 11:37:16.000000 pyhomie-0.0.3/pyHomie/watchdog.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:59:35.490761 pyhomie-0.0.3/pyHomie.egg-info/
+-rw-rw-rw-   0        0        0      854 2024-05-22 13:59:35.000000 pyhomie-0.0.3/pyHomie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2024-05-22 13:59:35.000000 pyhomie-0.0.3/pyHomie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 13:59:35.000000 pyhomie-0.0.3/pyHomie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-22 13:59:35.000000 pyhomie-0.0.3/pyHomie.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 13:59:35.498242 pyhomie-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1062 2024-05-22 13:58:57.000000 pyhomie-0.0.3/setup.py
```

### Comparing `pyhomie-0.0.2/README.md` & `pyhomie-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyhomie-0.0.2/pyHomie/device.py` & `pyhomie-0.0.3/pyHomie/device.py`

 * *Files identical despite different names*

### Comparing `pyhomie-0.0.2/pyHomie/mqttClient.py` & `pyhomie-0.0.3/pyHomie/mqttClient.py`

 * *Files identical despite different names*

### Comparing `pyhomie-0.0.2/pyHomie/node.py` & `pyhomie-0.0.3/pyHomie/node.py`

 * *Files identical despite different names*

### Comparing `pyhomie-0.0.2/pyHomie/properties.py` & `pyhomie-0.0.3/pyHomie/properties.py`

 * *Files identical despite different names*

### Comparing `pyhomie-0.0.2/pyHomie/pyHomie.py` & `pyhomie-0.0.3/pyHomie/pyHomie.py`

 * *Files identical despite different names*

### Comparing `pyhomie-0.0.2/pyHomie/watchdog.py` & `pyhomie-0.0.3/pyHomie/watchdog.py`

 * *Files identical despite different names*

