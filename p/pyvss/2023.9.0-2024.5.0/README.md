# Comparing `tmp/pyvss-2023.9.0.tar.gz` & `tmp/pyvss-2024.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvss-2023.9.0.tar", last modified: Wed Sep 27 20:03:14 2023, max compression
+gzip compressed data, was "pyvss-2024.5.0.tar", last modified: Wed May 22 13:52:38 2024, max compression
```

## Comparing `pyvss-2023.9.0.tar` & `pyvss-2024.5.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 20:03:14.413934 pyvss-2023.9.0/
--rw-rw-rw-   0 root         (0) root         (0)     1077 2023-09-26 19:49:56.000000 pyvss-2023.9.0/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       24 2023-09-26 19:49:56.000000 pyvss-2023.9.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7784 2023-09-27 20:03:14.413934 pyvss-2023.9.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6477 2023-09-26 19:49:56.000000 pyvss-2023.9.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-09-26 19:49:56.000000 pyvss-2023.9.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 20:03:14.413934 pyvss-2023.9.0/pyvss/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-27 20:03:10.000000 pyvss-2023.9.0/pyvss/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6751 2023-09-27 18:24:17.000000 pyvss-2023.9.0/pyvss/const.py
--rw-rw-rw-   0 root         (0) root         (0)     1409 2023-09-26 19:49:56.000000 pyvss-2023.9.0/pyvss/enums.py
--rw-rw-rw-   0 root         (0) root         (0)     1020 2023-09-26 19:49:56.000000 pyvss-2023.9.0/pyvss/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)     2808 2023-09-26 19:49:56.000000 pyvss-2023.9.0/pyvss/helper.py
--rw-rw-rw-   0 root         (0) root         (0)   281495 2023-09-27 18:24:17.000000 pyvss-2023.9.0/pyvss/manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-27 20:03:14.413934 pyvss-2023.9.0/pyvss.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7784 2023-09-27 20:03:14.000000 pyvss-2023.9.0/pyvss.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      390 2023-09-27 20:03:14.000000 pyvss-2023.9.0/pyvss.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-27 20:03:14.000000 pyvss-2023.9.0/pyvss.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      356 2023-09-27 20:03:14.000000 pyvss-2023.9.0/pyvss.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-09-27 20:03:14.000000 pyvss-2023.9.0/pyvss.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      122 2023-09-27 19:49:50.000000 pyvss-2023.9.0/requirements.dev.txt
--rw-rw-rw-   0 root         (0) root         (0)       13 2023-09-27 19:49:50.000000 pyvss-2023.9.0/requirements.stor.txt
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-09-27 19:49:50.000000 pyvss-2023.9.0/requirements.test.txt
--rw-rw-rw-   0 root         (0) root         (0)       29 2023-09-26 19:49:56.000000 pyvss-2023.9.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-09-27 20:03:14.413934 pyvss-2023.9.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3200 2023-09-27 19:49:50.000000 pyvss-2023.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:52:38.569071 pyvss-2024.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1077 2024-05-21 15:59:25.000000 pyvss-2024.5.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       24 2024-05-21 15:59:25.000000 pyvss-2024.5.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     8753 2024-05-22 13:52:38.569071 pyvss-2024.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6477 2024-05-21 15:59:25.000000 pyvss-2024.5.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-05-21 15:59:25.000000 pyvss-2024.5.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:52:38.565071 pyvss-2024.5.0/pyvss/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 13:52:33.000000 pyvss-2024.5.0/pyvss/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8148 2024-05-22 13:38:44.000000 pyvss-2024.5.0/pyvss/const.py
+-rw-rw-rw-   0 root         (0) root         (0)     1409 2024-05-21 15:59:25.000000 pyvss-2024.5.0/pyvss/enums.py
+-rw-rw-rw-   0 root         (0) root         (0)     1020 2024-05-21 15:59:25.000000 pyvss-2024.5.0/pyvss/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     2808 2024-05-21 15:59:25.000000 pyvss-2024.5.0/pyvss/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)   288508 2024-05-21 15:59:25.000000 pyvss-2024.5.0/pyvss/manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:52:38.569071 pyvss-2024.5.0/pyvss.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8753 2024-05-22 13:52:38.000000 pyvss-2024.5.0/pyvss.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-22 13:52:38.000000 pyvss-2024.5.0/pyvss.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 13:52:38.000000 pyvss-2024.5.0/pyvss.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      353 2024-05-22 13:52:38.000000 pyvss-2024.5.0/pyvss.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-05-22 13:52:38.000000 pyvss-2024.5.0/pyvss.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      122 2024-05-22 13:38:44.000000 pyvss-2024.5.0/requirements.dev.txt
+-rw-rw-rw-   0 root         (0) root         (0)       12 2024-05-22 13:38:44.000000 pyvss-2024.5.0/requirements.stor.txt
+-rw-rw-rw-   0 root         (0) root         (0)       69 2024-05-21 15:59:25.000000 pyvss-2024.5.0/requirements.test.txt
+-rw-rw-rw-   0 root         (0) root         (0)       29 2024-05-21 15:59:25.000000 pyvss-2024.5.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1263 2024-05-22 13:52:38.569071 pyvss-2024.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3200 2024-05-21 15:59:25.000000 pyvss-2024.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 13:52:38.569071 pyvss-2024.5.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    20920 2024-05-21 15:59:25.000000 pyvss-2024.5.0/tests/test_pyvss.py
```

### Comparing `pyvss-2023.9.0/LICENSE` & `pyvss-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvss-2023.9.0/PKG-INFO` & `pyvss-2024.5.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyvss
-Version: 2023.9.0
+Version: 2024.5.0
 Summary: ITS Private Cloud Python Client
 Home-page: https://gitlab-ee.eis.utoronto.ca/vss/py-vss
-Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/py-vss/archive/2023.9.0.zip
+Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/py-vss/archive/2024.5.0.zip
 Author: University of Toronto
 Author-email: vss-apps@eis.utoronto.ca
 Maintainer-email: vss-py@eis.utoronto.ca
 License: MIT
 Project-URL: Bug Reports, https://gitlab-ee.eis.utoronto.ca/vss/py-vss/issues
 Project-URL: Documentation, https://eis.utorotno.ca/~vss/py-vss/
 Project-URL: Source, https://gitlab-ee.eis.utoronto.ca/vss/py-vss
@@ -21,18 +21,39 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Systems Administration
 Requires-Python: >=3.7.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.28.2
+Requires-Dist: pyjwt>=2.6.0
 Provides-Extra: test
+Requires-Dist: flake8==6.0.0; extra == "test"
+Requires-Dist: nose==1.3.7; extra == "test"
+Requires-Dist: coverage==6.5.0; extra == "test"
+Requires-Dist: pytz==2022.6; extra == "test"
+Requires-Dist: wheel==0.38.4; extra == "test"
+Requires-Dist: minio==7.2.7; extra == "test"
 Provides-Extra: dev
+Requires-Dist: flake8==6.0.0; extra == "dev"
+Requires-Dist: nose==1.3.7; extra == "dev"
+Requires-Dist: coverage==6.5.0; extra == "dev"
+Requires-Dist: pytz==2022.6; extra == "dev"
+Requires-Dist: wheel==0.38.4; extra == "dev"
+Requires-Dist: minio==7.2.7; extra == "dev"
+Requires-Dist: minio==7.2.7; extra == "dev"
+Requires-Dist: sphinx-rtd-theme==1.3.0; extra == "dev"
+Requires-Dist: Sphinx==7.2.6; extra == "dev"
+Requires-Dist: bump2version==1.0.1; extra == "dev"
+Requires-Dist: sphinxcontrib-jquery==4.1; extra == "dev"
+Requires-Dist: sphinxcontrib-confluencebuilder==2.5.2; extra == "dev"
 Provides-Extra: stor
-License-File: LICENSE
+Requires-Dist: minio==7.2.7; extra == "stor"
 
 # ITS Private Cloud Python Client ``pyvss``
 
 [![CI][build-img]](https://gitlab-ee.eis.utoronto.ca/vss/py-vss/commits/master)
 [![PyPI][pypi-img]](https://pypi.python.org/pypi/pyvss)
 [![PyPI version][pyver-img]](https://pypi.python.org/pypi/pyvss)
 [![Docker Image Pulls][docker-pulls-img]][docker-image]
```

### Comparing `pyvss-2023.9.0/README.md` & `pyvss-2024.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyvss-2023.9.0/pyvss/const.py` & `pyvss-2024.5.0/pyvss/const.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Constants package for PyVSS."""
 PACKAGE_NAME = "pyvss"
 
-__version__ = '2023.9.0'
+__version__ = '2024.5.0'
 
 
 API_ENDPOINT_BASE = 'https://cloud-api.eis.utoronto.ca'
 
 VSS_S3_URL = 'https://vskey-stor.eis.utoronto.ca'
 VSS_S3_SVC_URL = '{s3_server}/s3/minio-svc/index.php'
 VSS_S3_STS_URL = '{s3_svc_url}?status=json'
@@ -142,39 +142,53 @@
     },
     {"type": "sharingnone", "description": "The virtual disk is not shared."},
 ]
 
 VALID_VM_VMX = [
     {"description": "ESXi 6.5", "type": "vmx-13"},
     {
-        "description": "Fusion 8.x/Workstation Pro 12.x/Workstation "
-        "Player 12.x",
+        "description": "Fusion 8.x/Workstation "
+        "Pro 12.x/Workstation Player 12.x",
         "type": "vmx-12",
     },
     {
         "description": "ESXi 6.0/Fusion 7.x/Workstation 11.x/Player 7.x",
         "type": "vmx-11",
     },
     {
         "description": "ESXi 5.5/Fusion 6.x/Workstation 10.x/Player 6.x",
         "type": "vmx-10",
     },
     {
+        "description": "ESXi/ESX 4.x/Fusion 3.x/Fusion 2.x/Workstation "
+        "7.x/Workstation 6.5.x/Player 3.x/Server 2.x",
+        "type": "vmx-07",
+    },
+    {
         "description": "ESXi 5.1/Fusion 5.x/Workstation 9.x/Player 5.x",
-        "type": "vmx-9",
+        "type": "vmx-09",
     },
     {
         "description": "ESXi 5.0/Fusion 4.x/Workstation 8.x/Player 4.x",
-        "type": "vmx-8",
+        "type": "vmx-08",
     },
+    {"description": "ESXi 6.7", "type": "vmx-14"},
+    {"description": "ESXi 6.7 U2", "type": "vmx-15"},
     {
-        "description": "ESXi/ESX 4.x/Fusion 3.x/Fusion 2.x/Workstation "
-        "7.x/Workstation 6.5.x/Player 3.x/Server 2.x",
-        "type": "vmx-7",
+        "description": "Fusion 11.x Workstation Pro "
+        "15.x Workstation Player 15.x",
+        "type": "vmx-16",
     },
+    {"description": "ESXi 7.0  (7.0.0)", "type": "vmx-17"},
+    {
+        "description": "ESXi 7.0 U1 (7.0.1) Fusion 12.x "
+        "Workstation Pro 16.x Workstation Player 16.x",
+        "type": "vmx-18",
+    },
+    {"description": "ESXi 7.0 U2 (7.0.2)", "type": "vmx-19"},
 ]
 
 VALID_VM_EXTRA_CFG = [
     {
         "description": "Enable disk UUID on virtual machines",
         "option": "disk.EnableUUID",
     },
@@ -211,7 +225,38 @@
         'option': 'ssd',
     },
     {
         'description': 'Storage Clusters backed by Hard disk drives.',
         'option': 'HDD',
     },
 ]
+VM_VALID_GPU_TYPE = [
+    {
+        "description": "Frame Buffer 4GB. Virtual workstations",
+        "type": "grid_p6-4q",
+    },
+    {
+        "description": "Frame Buffer 8GB. Virtual Workstations",
+        "type": "grid_p6-8q",
+    },
+    {
+        "description": "Frame Buffer 16GB. Virtual Workstations",
+        "type": "grid_p6-16q",
+    },
+    {
+        "description": "Frame Buffer 4GB. "
+        "App streaming or session-based solutions for "
+        "virtual applications users.",
+        "type": "grid_p6-4a",
+    },
+    {
+        "description": "Frame Buffer 8GB. "
+        "App streaming or session-based solutions for "
+        "virtual applications users.",
+        "type": "grid_p6-8a",
+    },
+    {
+        "description": "Frame Buffer 16GB. Virtual desktops for "
+        "business professionals and knowledge workers.",
+        "type": "grid_p6-16a",
+    },
+]
```

### Comparing `pyvss-2023.9.0/pyvss/enums.py` & `pyvss-2024.5.0/pyvss/enums.py`

 * *Files identical despite different names*

### Comparing `pyvss-2023.9.0/pyvss/exceptions.py` & `pyvss-2024.5.0/pyvss/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyvss-2023.9.0/pyvss/helper.py` & `pyvss-2024.5.0/pyvss/helper.py`

 * *Files identical despite different names*

### Comparing `pyvss-2023.9.0/pyvss/manager.py` & `pyvss-2024.5.0/pyvss/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 
 `API Reference <https://utor.cloud/vssapi-docs-ref>`__.
 """
 import datetime
 import os
 import platform
 import re
-from typing import Dict, List, Optional, Tuple, Union
 import warnings
+from typing import Dict, List, Optional, Tuple, Union
 
 import requests
 
 from pyvss.const import (
     API_ENDPOINT_BASE, DATETIME_FMT, DEFAULT_DEBUG, DEFAULT_DRY_RUN,
     DEFAULT_TIMEOUT, PACKAGE_NAME, VALID_VM_BUILD_PROCESS, VALID_VM_DISK_MODE,
     VALID_VM_DISK_SHARING, VALID_VM_EXTRA_CFG, VALID_VM_FIRMWARE_TYPE,
     VALID_VM_NIC_TYPE, VALID_VM_SCSI_CONTROLLER, VALID_VM_STORAGE_TYPE,
-    VALID_VM_USAGE, VALID_VM_VMX, VSS_S3_STS_URL, VSS_S3_SVC_URL, VSS_S3_URL,
-    __version__ as product_version)
+    VALID_VM_USAGE, VALID_VM_VMX, VM_VALID_GPU_TYPE, VSS_S3_STS_URL,
+    VSS_S3_SVC_URL, VSS_S3_URL)
+from pyvss.const import __version__ as product_version
 from pyvss.enums import RequestStatus
 from pyvss.exceptions import VssError
 from pyvss.helper import HTTPBasicAuth, is_list_of, normalize_str
 
 warnings.simplefilter('always')
 
 
@@ -109,14 +110,15 @@
         self.s_vss_options = None
         self.s_vss_preferences = None
         self.s_disk_back_sharing = None
         self.s_scsi_controllers_sharing = None
         self.s_extra_config_options = None
         self.s_firmware_types = None
         self.s_storage_types = None
+        self.s_vm_gpu_profiles = None
         # other services
         self.vskey_stor = None
         self.vskey_stor_s3api = None
         self.vskey_stor_s3_gui = None
         self.vskey_stor_s3_ak = None
         self.vskey_stor_s3_sk = None
 
@@ -165,14 +167,15 @@
         self.s_extra_config_options = self.get_supported_extra_cfg_options(
             only_option=True
         )
         self.s_firmware_types = self.get_supported_firmware_types(
             only_type=True
         )
         self.s_storage_types = self.get_supported_storage_types(only_type=True)
+        self.s_vm_gpu_profiles = self.get_supported_gpu_types(only_type=True)
 
     @staticmethod
     def _default_user_agent(
         name=PACKAGE_NAME, version=product_version, extensions=''
     ):
         """Generate default user agent."""
         environment = {
@@ -438,17 +441,18 @@
              object_name='jammy-server-cloudimg-amd64.ova',
              file_path=os.path.expanduser('~/Downloads/jammy-server-cloudimg-amd64.ova')
              )
         """
         if not HAS_MINIO:
             raise VssError('minio library is required')
 
-        from minio import Minio
         from urllib.parse import urlparse
 
+        from minio import Minio
+
         self.vskey_stor_s3api = os.environ.get('VSS_S3_API', s3_endpoint)
         self.vskey_stor_s3_ak = os.environ.get('VSS_S3_ACCESS_KEY', access_key)
         self.vskey_stor_s3_sk = os.environ.get('VSS_S3_SECRET_KEY', secret_key)
 
         if not all(
             [
                 self.vskey_stor_s3api,
@@ -5811,14 +5815,36 @@
         json = self.request(
             f'/vm/{vm_id}/memory',
             payload=payload,
             method=self.PUT,
         )
         return json.get('data')
 
+    def set_vm_memory_reservation(self, vm_id, size, **kwargs):
+        """Update Virtual Machine Memory size.
+
+        :param vm_id: virtual machine moref or uuid
+        :type vm_id: str
+        :param size: memory to reserve in GB
+        :type size: int
+        :return: change request object
+
+        .. note:: keyword arguments include schedule to process request
+         on a given date and time
+
+        """
+        payload = dict(value=int(size))
+        payload.update(kwargs)
+        json = self.request(
+            f'/vm/{vm_id}/memory/reservation',
+            payload=payload,
+            method=self.PUT,
+        )
+        return json.get('data')
+
     def get_vm_cpu(self, vm_id):
         """Get VM cpu information.
 
         - cores_per_socket
         - cpu
         - hot_add
         - hot_remove
@@ -6451,15 +6477,42 @@
         :type vm_id: str
         :return: list of objects
         """
         json = self.request(f'/vm/{vm_id}/controller')
         data = json.get('data')
         if not data:
             return None
-        del data['scsi']['_links']
+        if '_links' in data['scsi']:
+            del data['scsi']['_links']
+        return data
+
+    def get_vm_usb_devices(self, vm_id):
+        """Get virtual machine USB devices.
+
+        :param vm_id: virtual machine moref or uuid
+        :type vm_id: str
+        :return: list of objects
+        """
+        json = self.request(f'/vm/{vm_id}/controller/usb')
+        data = json.get('data')
+        if not data:
+            return None
+        return data
+
+    def get_vm_usb_xhci_devices(self, vm_id):
+        """Get virtual machine USB devices.
+
+        :param vm_id: virtual machine moref or uuid
+        :type vm_id: str
+        :return: list of objects
+        """
+        json = self.request(f'/vm/{vm_id}/controller/usb-xhci')
+        data = json.get('data')
+        if not data:
+            return None
         return data
 
     def get_vm_scsi_devices(self, vm_id):
         """Get Virtual machine available SCSI controllers.
 
         :param vm_id: virtual machine moref or uuid
         :type vm_id: str
@@ -6467,15 +6520,16 @@
         """
         json = self.request(f'/vm/{vm_id}/controller/scsi')
         data = json.get('data')
         if not data:
             return None
         scsi = []
         for c in data:
-            del c['_links']
+            if isinstance(c, dict) and '_links' in c:
+                del c['_links']
             scsi.append(c)
         return scsi
 
     def get_vm_scsi_device(self, vm_id, bus, devices=None):
         """Get Virtual Machine available SCSI bus.
 
         :param vm_id: virtual machine moref or uuid
@@ -8052,14 +8106,110 @@
         """
         rv = self.request(
             f'/vm/{vm_id}/gpu',
             method=self.GET,
         )
         return rv.get('data')
 
+    def _get_vm_host_profile_status(self, host, vm_profiles):
+        """Get vm host profile status."""
+        gpu_profiles = host['gpu_profiles']
+        if gpu_profiles:
+            # 2. Check for bound profiles
+            gpu_profiles_bound = host['gpu_profiles_bound']
+            if gpu_profiles_bound:
+                gpu_profiles_bound = gpu_profiles_bound.split(',')
+                gpu_profiles_bound = list(
+                    set(gpu_profiles_bound) - set(vm_profiles)
+                )
+                if not gpu_profiles_bound:
+                    return gpu_profiles
+                return gpu_profiles_bound
+            else:
+                return gpu_profiles
+        else:
+            raise VssError(f'Host {host["moref"]} does not have GPU available')
+
+    def _get_vm_by_id(self, vm_id: str):
+        """Get vm by id."""
+        vm = self.get_vms(filter=f'moref,eq,{vm_id}')
+        if not vm:
+            raise VssError(f'Instance not found: {vm_id}')
+        return vm[0]
+
+    def get_vm_host_gpu_profiles(self, vm_id: str):
+        """Get vm host gpu profiles."""
+        vm = self._get_vm_by_id(vm_id)
+        profiles = vm.get('gpu_profiles').split(',')
+        # get host from vm attribute
+        host = vm.get('host', {})
+        if not host:
+            raise VssError('Could not fetch VM host.')
+        # get current available profiles in host
+        return self._get_vm_host_profile_status(host, profiles)
+
+    def _validate_vm_gpu(self, vm_id, profile) -> str:
+        """Validate VM gpu."""
+        # 0. Validate given profile
+        _ = self.validate_vm_gpu_profile(profile)
+        # 1. Look for any restricting gpu profiles at VM host level
+        ex_gpu_profiles = self.get_vm_host_gpu_profiles(vm_id)
+        if profile not in ex_gpu_profiles:
+            raise VssError(
+                f'{profile} unavailable on current host. '
+                f'Currently available {ex_gpu_profiles}'
+            )
+        return profile
+
+    def create_vm_gpu(self, vm_id: str, profile: str, **kwargs):
+        """Create GPU on VM.
+
+        :param vm_id: virtual machine moref or uuid
+        :type vm_id: str
+        :param profile: vGPU profile to use. Supported profiles are
+         available here :py:func:`get_supported_gpu_types` or through
+         :py:func:`get_vm_host_gpu_profiles` for existing bound profiles.
+        :return: change request object
+        """
+        payload = dict(value=self._validate_vm_gpu(vm_id, profile))
+        payload.update(kwargs)
+        rv = self.request(
+            f'/vm/{vm_id}/gpu', method=self.POST, payload=payload
+        )
+        return rv.get('data')
+
+    def update_vm_gpu(self, vm_id: str, profile: str, **kwargs):
+        """Update vm gpu profile.
+
+        :param vm_id: virtual machine moref or uuid
+        :type vm_id: str
+        :param profile: vGPU profile to use. Supported profiles are
+         available here :py:func:`get_supported_gpu_types` or through
+         :py:func:`get_vm_host_gpu_profiles` for existing bound profiles.
+        :return: change request object
+        """
+        payload = dict(value=self._validate_vm_gpu(vm_id, profile))
+        payload.update(kwargs)
+        rv = self.request(f'/vm/{vm_id}/gpu', method=self.PUT, payload=payload)
+        return rv.get('data')
+
+    def delete_vm_gpu(self, vm_id: str, **kwargs):
+        """Delete vm gpu device.
+
+        :param vm_id: virtual machine moref or uuid
+        :type vm_id: str
+        :return: change request object
+        """
+        payload = {}
+        payload.update(kwargs)
+        rv = self.request(
+            f'/vm/{vm_id}/gpu', method=self.DELETE, payload=payload
+        )
+        return rv.get('data')
+
     def create_vm_extra_cfg_options(self, vm_id, options):
         """Create VM extra configuration settings.
 
         Extra configuration options are either guestinfo.* or allowed
         options.
 
         Extra config guestinfo.* options can be queried from the
@@ -8142,22 +8292,51 @@
         :param moref: Folder managed object id
         :type moref: str
         :return: list of key value objects
         """
         json = self.request(f'/folder/{moref}/perm')
         return json.get('data')
 
-    def get_vm_restore_points(self, moref):
+    def restore_vm(self, moref, timestamp, **kwargs):
+        """Submit a vm restore request.
+
+        :param moref: virtual machine moref
+        :type moref: str
+        :param timestamp: restore point timestamp
+        :type timestamp: str
+        :return:
+        """
+        payload = dict(value=timestamp)
+        payload.update(kwargs)
+        json = self.request(
+            f'/vm/{moref}/restore', payload=payload, method=self.POST
+        )
+        return json.get('data')
+
+    def get_vm_restore_points(
+        self, moref, show_all=False, per_page=250, **kwargs
+    ):
         """Get vm restore points.
 
         :param moref: virtual machine moref
         :type moref: str
+        :param show_all: Whether to show all ISO images or just
+         the default count
+        :type show_all: bool
+        :param per_page: how many results per page
+        :type per_page: int
+        :return: list of objects
         """
-        rv = self.request(f'/vm/{moref}/restore-point')
-        return rv.get('data')
+        kwargs.update({'per_page': per_page})
+        data = self._get_objects(
+            pag_resource=f'/vm/{moref}/restore-point',
+            show_all=show_all,
+            **kwargs,
+        )
+        return data
 
     def request(
         self,
         url,
         headers=None,
         params=None,
         payload=None,
@@ -8447,14 +8626,36 @@
                 only_type=True
             )
         if self.dry_run:
             return n_type
         else:
             return self.validate_options(n_type, self.s_disk_back_sharing)
 
+    def get_supported_gpu_types(
+        self, only_type: bool = True
+    ) -> Union[Dict, List[str]]:
+        """Get supported vM GPU types."""
+        if self.dry_run:
+            data = VM_VALID_GPU_TYPE
+        else:
+            json = self.request('/vss/gpu')
+            data = json.get('data')
+        return [i['type'] for i in data] if only_type else data
+
+    def validate_vm_gpu_profile(self, g_type):
+        """Validate supported vm gpu profiles."""
+        if self.s_vm_gpu_profiles is None:
+            self.s_vm_gpu_profiles = self.get_supported_gpu_types(
+                only_type=True
+            )
+        if self.dry_run:
+            return g_type
+        else:
+            return self.validate_options(g_type, self.s_vm_gpu_profiles)
+
     @property
     def status(self):
         """Return status of the api.
 
         :return: dict
         """
         return self.request('/status').get('data')
```

### Comparing `pyvss-2023.9.0/pyvss.egg-info/PKG-INFO` & `pyvss-2024.5.0/pyvss.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: pyvss
-Version: 2023.9.0
+Version: 2024.5.0
 Summary: ITS Private Cloud Python Client
 Home-page: https://gitlab-ee.eis.utoronto.ca/vss/py-vss
-Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/py-vss/archive/2023.9.0.zip
+Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/py-vss/archive/2024.5.0.zip
 Author: University of Toronto
 Author-email: vss-apps@eis.utoronto.ca
 Maintainer-email: vss-py@eis.utoronto.ca
 License: MIT
 Project-URL: Bug Reports, https://gitlab-ee.eis.utoronto.ca/vss/py-vss/issues
 Project-URL: Documentation, https://eis.utorotno.ca/~vss/py-vss/
 Project-URL: Source, https://gitlab-ee.eis.utoronto.ca/vss/py-vss
@@ -21,18 +21,39 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Systems Administration
 Requires-Python: >=3.7.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests>=2.28.2
+Requires-Dist: pyjwt>=2.6.0
 Provides-Extra: test
+Requires-Dist: flake8==6.0.0; extra == "test"
+Requires-Dist: nose==1.3.7; extra == "test"
+Requires-Dist: coverage==6.5.0; extra == "test"
+Requires-Dist: pytz==2022.6; extra == "test"
+Requires-Dist: wheel==0.38.4; extra == "test"
+Requires-Dist: minio==7.2.7; extra == "test"
 Provides-Extra: dev
+Requires-Dist: flake8==6.0.0; extra == "dev"
+Requires-Dist: nose==1.3.7; extra == "dev"
+Requires-Dist: coverage==6.5.0; extra == "dev"
+Requires-Dist: pytz==2022.6; extra == "dev"
+Requires-Dist: wheel==0.38.4; extra == "dev"
+Requires-Dist: minio==7.2.7; extra == "dev"
+Requires-Dist: minio==7.2.7; extra == "dev"
+Requires-Dist: sphinx-rtd-theme==1.3.0; extra == "dev"
+Requires-Dist: Sphinx==7.2.6; extra == "dev"
+Requires-Dist: bump2version==1.0.1; extra == "dev"
+Requires-Dist: sphinxcontrib-jquery==4.1; extra == "dev"
+Requires-Dist: sphinxcontrib-confluencebuilder==2.5.2; extra == "dev"
 Provides-Extra: stor
-License-File: LICENSE
+Requires-Dist: minio==7.2.7; extra == "stor"
 
 # ITS Private Cloud Python Client ``pyvss``
 
 [![CI][build-img]](https://gitlab-ee.eis.utoronto.ca/vss/py-vss/commits/master)
 [![PyPI][pypi-img]](https://pypi.python.org/pypi/pyvss)
 [![PyPI version][pyver-img]](https://pypi.python.org/pypi/pyvss)
 [![Docker Image Pulls][docker-pulls-img]][docker-image]
```

### Comparing `pyvss-2023.9.0/setup.cfg` & `pyvss-2024.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyvss-2023.9.0/setup.py` & `pyvss-2024.5.0/setup.py`

 * *Files identical despite different names*

