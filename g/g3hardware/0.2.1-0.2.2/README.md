# Comparing `tmp/g3hardware-0.2.1.tar.gz` & `tmp/g3hardware-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "g3hardware-0.2.1.tar", last modified: Mon Apr 29 15:03:38 2024, max compression
+gzip compressed data, was "g3hardware-0.2.2.tar", last modified: Wed May 22 09:03:59 2024, max compression
```

## Comparing `g3hardware-0.2.1.tar` & `g3hardware-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-04-29 15:03:38.504942 g3hardware-0.2.1/
--rw-rw-rw-   0        0        0     1091 2023-06-02 14:34:32.000000 g3hardware-0.2.1/LICENCE
--rw-rw-rw-   0        0        0     1202 2024-04-29 15:03:38.497941 g3hardware-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      146 2024-04-29 14:39:19.000000 g3hardware-0.2.1/README.md
--rw-rw-rw-   0        0        0     1262 2024-04-29 15:02:24.000000 g3hardware-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-29 15:03:38.505945 g3hardware-0.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-29 15:03:38.414941 g3hardware-0.2.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-29 15:03:38.458942 g3hardware-0.2.1/src/g3hardware/
--rw-rw-rw-   0        0        0      410 2024-04-29 14:39:19.000000 g3hardware-0.2.1/src/g3hardware/__init__.py
--rw-rw-rw-   0        0        0    54505 2024-04-29 14:39:19.000000 g3hardware-0.2.1/src/g3hardware/_g3hardware.py
--rw-rw-rw-   0        0        0      949 2024-04-29 14:39:19.000000 g3hardware-0.2.1/src/g3hardware/api.py
--rw-rw-rw-   0        0        0    10190 2024-04-29 14:48:43.000000 g3hardware-0.2.1/src/g3hardware/config.yaml
--rw-rw-rw-   0        0        0        0 2023-09-26 20:40:57.000000 g3hardware-0.2.1/src/g3hardware/py.typed
-drwxrwxrwx   0        0        0        0 2024-04-29 15:03:38.495943 g3hardware-0.2.1/src/g3hardware.egg-info/
--rw-rw-rw-   0        0        0     1202 2024-04-29 15:03:38.000000 g3hardware-0.2.1/src/g3hardware.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      448 2024-04-29 15:03:38.000000 g3hardware-0.2.1/src/g3hardware.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-29 15:03:38.000000 g3hardware-0.2.1/src/g3hardware.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-04-29 15:03:38.000000 g3hardware-0.2.1/src/g3hardware.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-29 15:03:38.000000 g3hardware-0.2.1/src/g3hardware.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-29 15:03:38.491942 g3hardware-0.2.1/tests/
--rw-rw-rw-   0        0        0     2025 2024-04-29 14:39:19.000000 g3hardware-0.2.1/tests/test_module_config.py
--rw-rw-rw-   0        0        0        0 2024-04-29 14:39:19.000000 g3hardware-0.2.1/tests/test_module_factory.py
--rw-rw-rw-   0        0        0     2491 2024-04-29 14:39:19.000000 g3hardware-0.2.1/tests/test_module_template_formatter.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:03:59.818584 g3hardware-0.2.2/
+-rw-rw-rw-   0        0        0     1091 2024-05-21 20:22:51.000000 g3hardware-0.2.2/LICENCE
+-rw-rw-rw-   0        0        0     1202 2024-05-22 09:03:59.818584 g3hardware-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      146 2024-05-21 20:22:51.000000 g3hardware-0.2.2/README.md
+-rw-rw-rw-   0        0        0     1262 2024-05-22 08:59:20.000000 g3hardware-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 09:03:59.818584 g3hardware-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-22 09:03:59.802929 g3hardware-0.2.2/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 09:03:59.802929 g3hardware-0.2.2/src/g3hardware/
+-rw-rw-rw-   0        0        0      410 2024-05-21 20:22:51.000000 g3hardware-0.2.2/src/g3hardware/__init__.py
+-rw-rw-rw-   0        0        0    54505 2024-05-21 20:22:51.000000 g3hardware-0.2.2/src/g3hardware/_g3hardware.py
+-rw-rw-rw-   0        0        0      949 2024-05-21 20:22:51.000000 g3hardware-0.2.2/src/g3hardware/api.py
+-rw-rw-rw-   0        0        0    10146 2024-05-21 20:22:51.000000 g3hardware-0.2.2/src/g3hardware/config.yaml
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:22:51.000000 g3hardware-0.2.2/src/g3hardware/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-22 09:03:59.818584 g3hardware-0.2.2/src/g3hardware.egg-info/
+-rw-rw-rw-   0        0        0     1202 2024-05-22 09:03:59.000000 g3hardware-0.2.2/src/g3hardware.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      448 2024-05-22 09:03:59.000000 g3hardware-0.2.2/src/g3hardware.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 09:03:59.000000 g3hardware-0.2.2/src/g3hardware.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2024-05-22 09:03:59.000000 g3hardware-0.2.2/src/g3hardware.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-22 09:03:59.000000 g3hardware-0.2.2/src/g3hardware.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 09:03:59.818584 g3hardware-0.2.2/tests/
+-rw-rw-rw-   0        0        0     2025 2024-05-21 20:22:51.000000 g3hardware-0.2.2/tests/test_module_config.py
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:22:51.000000 g3hardware-0.2.2/tests/test_module_factory.py
+-rw-rw-rw-   0        0        0     2491 2024-05-21 20:22:51.000000 g3hardware-0.2.2/tests/test_module_template_formatter.py
```

### Comparing `g3hardware-0.2.1/LICENCE` & `g3hardware-0.2.2/LICENCE`

 * *Files identical despite different names*

### Comparing `g3hardware-0.2.1/PKG-INFO` & `g3hardware-0.2.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3hardware
-Version: 0.2.1
+Version: 0.2.2
 Summary: G3 PLC Hardware XML configuration generator
 Author: Elektroline a.s.
 Project-URL: Homepage, https://gitlab.elektroline.cz/plc/systemg3-py/SystemG3Hardware
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `g3hardware-0.2.1/pyproject.toml` & `g3hardware-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "g3hardware"
-version = "0.2.1"
+version = "0.2.2"
 description = "G3 PLC Hardware XML configuration generator"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [
   { name = "Elektroline a.s." },
 ]
 classifiers = [
```

### Comparing `g3hardware-0.2.1/src/g3hardware/_g3hardware.py` & `g3hardware-0.2.2/src/g3hardware/_g3hardware.py`

 * *Files identical despite different names*

### Comparing `g3hardware-0.2.1/src/g3hardware/api.py` & `g3hardware-0.2.2/src/g3hardware/api.py`

 * *Files identical despite different names*

### Comparing `g3hardware-0.2.1/src/g3hardware/config.yaml` & `g3hardware-0.2.2/src/g3hardware/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -164,20 +164,20 @@
     <Parameter ID="InternetFileSystemDomainName" Value="ELEKTROLINE"/>
     <Parameter ID="EthernetHostName" Value="{{ cpuhostname }}"/>
     <Parameter ID="ActivateDns" Value="1"/>
     <Parameter ID="DnsDefaultDomain" Value="plc-SystemG3"/>
     <Parameter ID="GetDnsFromDhcp" Value="2"/>
     <Group ID="FtpUser1"/>
     <Parameter ID="FtpUsername1" Value="ftp"/>
-    <Parameter ID="FtpUserPassword1" Value="f72tDAVhahnyOV/IZfssRCMEbGjPNzns7ewwnoH9x2E="/>
+    <Parameter ID="FtpUserPassword1" Value="{{ ftpuserpassword1 }}"/>
     <Parameter ID="FtpUserSalt1" Value="hvIOd8JU"/>
     <Parameter ID="FTPMSpath1" Value="/data/log_Elesys/"/>
     <Group ID="FtpUser2"/>
     <Parameter ID="FtpUsername2" Value="ellmaster"/>
-    <Parameter ID="FtpUserPassword2" Value="GaMcdopx+SyN+D6x9NJxAUX+N1h+sr3jR7JPFHN9AQM="/>
+    <Parameter ID="FtpUserPassword2" Value="{{ ftpuserpassword2 }}"/>
     <Parameter ID="FtpUserSalt2" Value="DYK6g03a"/>
     <Parameter ID="FTPAccessRight2" Value="0"/>
     <Parameter ID="FTPMSpath2" Value="/data/"/>
     <Parameter ID="WebServerPort" Value="8080"/>
     <Parameter ID="TemperatureCPUType" Value="INT"/>
     <Parameter ID="TemperatureENVType" Value="INT"/>
   tb: null
```

### Comparing `g3hardware-0.2.1/src/g3hardware.egg-info/PKG-INFO` & `g3hardware-0.2.2/src/g3hardware.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: g3hardware
-Version: 0.2.1
+Version: 0.2.2
 Summary: G3 PLC Hardware XML configuration generator
 Author: Elektroline a.s.
 Project-URL: Homepage, https://gitlab.elektroline.cz/plc/systemg3-py/SystemG3Hardware
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `g3hardware-0.2.1/tests/test_module_config.py` & `g3hardware-0.2.2/tests/test_module_config.py`

 * *Files identical despite different names*

### Comparing `g3hardware-0.2.1/tests/test_module_template_formatter.py` & `g3hardware-0.2.2/tests/test_module_template_formatter.py`

 * *Files identical despite different names*

