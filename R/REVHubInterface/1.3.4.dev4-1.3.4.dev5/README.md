# Comparing `tmp/revhubinterface-1.3.4.dev4.tar.gz` & `tmp/revhubinterface-1.3.4.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revhubinterface-1.3.4.dev4.tar", last modified: Tue May 21 02:45:41 2024, max compression
+gzip compressed data, was "revhubinterface-1.3.4.dev5.tar", last modified: Tue May 21 03:09:35 2024, max compression
```

## Comparing `revhubinterface-1.3.4.dev4.tar` & `revhubinterface-1.3.4.dev5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:45:41.322526 revhubinterface-1.3.4.dev4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:45:41.314526 revhubinterface-1.3.4.dev4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:45:41.318526 revhubinterface-1.3.4.dev4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/.github/workflows/flatpak.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/.github/workflows/pyinstaller.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-21 02:45:41.322526 revhubinterface-1.3.4.dev4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:45:41.318526 revhubinterface-1.3.4.dev4/REVHubInterface/
--rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REV2mSensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REVADC.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REVColorSensorV3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REVComPorts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REVDIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REVI2C.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REVModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REVMotor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REVServo.py
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REVcomm.py
--rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REVmessages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61395 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-21 02:45:41.000000 revhubinterface-1.3.4.dev4/REVHubInterface/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:45:41.322526 revhubinterface-1.3.4.dev4/REVHubInterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-21 02:45:41.000000 revhubinterface-1.3.4.dev4/REVHubInterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-21 02:45:41.000000 revhubinterface-1.3.4.dev4/REVHubInterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 02:45:41.000000 revhubinterface-1.3.4.dev4/REVHubInterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-21 02:45:41.000000 revhubinterface-1.3.4.dev4/REVHubInterface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-21 02:45:41.000000 revhubinterface-1.3.4.dev4/REVHubInterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 02:45:41.000000 revhubinterface-1.3.4.dev4/REVHubInterface.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:45:41.322526 revhubinterface-1.3.4.dev4/flatpak/
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/flatpak/flatpak-pip-generator
--rwxr-xr-x   0 runner    (1001) docker     (127)      174 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/flatpak/org.unofficialrevport.REVHubInterface.desktop
--rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/flatpak/org.unofficialrevport.REVHubInterface.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/flatpak/python3-requirements.json
--rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.Devel.svg
--rw-r--r--   0 runner    (1001) docker     (127)   384626 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.Source.svg
--rw-r--r--   0 runner    (1001) docker     (127)    99970 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.icns
--rw-r--r--   0 runner    (1001) docker     (127)    33388 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.ico
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.metainfo.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.svg
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/pyinstaller-build-reqs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 02:45:41.322526 revhubinterface-1.3.4.dev4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:09:35.411955 revhubinterface-1.3.4.dev5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:09:35.403955 revhubinterface-1.3.4.dev5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:09:35.407955 revhubinterface-1.3.4.dev5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/.github/workflows/flatpak.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/.github/workflows/pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-21 03:09:35.411955 revhubinterface-1.3.4.dev5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:09:35.411955 revhubinterface-1.3.4.dev5/REVHubInterface/
+-rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/REVHubInterface/REV2mSensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/REVHubInterface/REVADC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/REVHubInterface/REVColorSensorV3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/REVHubInterface/REVComPorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/REVHubInterface/REVDIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/REVHubInterface/REVI2C.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/REVHubInterface/REVModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/REVHubInterface/REVMotor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/REVHubInterface/REVServo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/REVHubInterface/REVcomm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/REVHubInterface/REVmessages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/REVHubInterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61395 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/REVHubInterface/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-21 03:09:35.000000 revhubinterface-1.3.4.dev5/REVHubInterface/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:09:35.411955 revhubinterface-1.3.4.dev5/REVHubInterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-21 03:09:35.000000 revhubinterface-1.3.4.dev5/REVHubInterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-21 03:09:35.000000 revhubinterface-1.3.4.dev5/REVHubInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 03:09:35.000000 revhubinterface-1.3.4.dev5/REVHubInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-21 03:09:35.000000 revhubinterface-1.3.4.dev5/REVHubInterface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-21 03:09:35.000000 revhubinterface-1.3.4.dev5/REVHubInterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 03:09:35.000000 revhubinterface-1.3.4.dev5/REVHubInterface.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/REVHubInterface.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/REVHubInterface.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:09:35.411955 revhubinterface-1.3.4.dev5/flatpak/
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/flatpak/flatpak-pip-generator
+-rwxr-xr-x   0 runner    (1001) docker     (127)      174 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/flatpak/org.unofficialrevport.REVHubInterface.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/flatpak/org.unofficialrevport.REVHubInterface.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/flatpak/python3-requirements.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/org.unofficialrevport.REVHubInterface.Devel.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   384626 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/org.unofficialrevport.REVHubInterface.Source.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    99970 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/org.unofficialrevport.REVHubInterface.icns
+-rw-r--r--   0 runner    (1001) docker     (127)    33388 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/org.unofficialrevport.REVHubInterface.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/org.unofficialrevport.REVHubInterface.metainfo.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/org.unofficialrevport.REVHubInterface.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/pyinstaller-build-reqs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-21 03:09:30.000000 revhubinterface-1.3.4.dev5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 03:09:35.411955 revhubinterface-1.3.4.dev5/setup.cfg
```

### Comparing `revhubinterface-1.3.4.dev4/.github/workflows/flatpak.yml` & `revhubinterface-1.3.4.dev5/.github/workflows/flatpak.yml`

 * *Files 18% similar despite different names*

```diff
@@ -8,12 +8,15 @@
     name: "Flatpak"
     runs-on: ubuntu-latest
     container:
       image: bilelmoussaoui/flatpak-github-actions:gnome-44
       options: --privileged
     steps:
     - uses: actions/checkout@v4
+      with:
+        fetch-tags: true
+        fetch-depth: 0
     - uses: flatpak/flatpak-github-actions/flatpak-builder@v6
       with:
         bundle: org.unofficialrevport.REVHubInterface.flatpak
         manifest-path: flatpak/org.unofficialrevport.REVHubInterface.yml
         cache-key: flatpak-builder-${{ github.sha }}
```

### Comparing `revhubinterface-1.3.4.dev4/.github/workflows/pyinstaller.yml` & `revhubinterface-1.3.4.dev5/.github/workflows/pyinstaller.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/.github/workflows/python-publish.yml` & `revhubinterface-1.3.4.dev5/.github/workflows/python-publish.yml`

 * *Files 9% similar despite different names*

```diff
@@ -22,14 +22,15 @@
   release-build:
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
         with:
           fetch-depth: 0
+          fetch-tags: true
 
       - uses: actions/setup-python@v5
         with:
           python-version: "3.x"
 
       - name: build release distributions
         run: |
```

### Comparing `revhubinterface-1.3.4.dev4/LICENSE.txt` & `revhubinterface-1.3.4.dev5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/PKG-INFO` & `revhubinterface-1.3.4.dev5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.4.dev4
+Version: 1.3.4.dev5
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.4.dev4/README.md` & `revhubinterface-1.3.4.dev5/README.md`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/REVHubInterface/REV2mSensor.py` & `revhubinterface-1.3.4.dev5/REVHubInterface/REV2mSensor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/REVHubInterface/REVADC.py` & `revhubinterface-1.3.4.dev5/REVHubInterface/REVADC.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/REVHubInterface/REVColorSensorV3.py` & `revhubinterface-1.3.4.dev5/REVHubInterface/REVColorSensorV3.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/REVHubInterface/REVComPorts.py` & `revhubinterface-1.3.4.dev5/REVHubInterface/REVComPorts.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/REVHubInterface/REVDIO.py` & `revhubinterface-1.3.4.dev5/REVHubInterface/REVDIO.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/REVHubInterface/REVI2C.py` & `revhubinterface-1.3.4.dev5/REVHubInterface/REVI2C.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/REVHubInterface/REVModule.py` & `revhubinterface-1.3.4.dev5/REVHubInterface/REVModule.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/REVHubInterface/REVMotor.py` & `revhubinterface-1.3.4.dev5/REVHubInterface/REVMotor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/REVHubInterface/REVServo.py` & `revhubinterface-1.3.4.dev5/REVHubInterface/REVServo.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/REVHubInterface/REVcomm.py` & `revhubinterface-1.3.4.dev5/REVHubInterface/REVcomm.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/REVHubInterface/REVmessages.py` & `revhubinterface-1.3.4.dev5/REVHubInterface/REVmessages.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/REVHubInterface/__main__.py` & `revhubinterface-1.3.4.dev5/REVHubInterface/__main__.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/REVHubInterface.egg-info/PKG-INFO` & `revhubinterface-1.3.4.dev5/REVHubInterface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.4.dev4
+Version: 1.3.4.dev5
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.4.dev4/REVHubInterface.egg-info/SOURCES.txt` & `revhubinterface-1.3.4.dev5/REVHubInterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/REVHubInterface.spec` & `revhubinterface-1.3.4.dev5/REVHubInterface.spec`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/flatpak/flatpak-pip-generator` & `revhubinterface-1.3.4.dev5/flatpak/flatpak-pip-generator`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/flatpak/org.unofficialrevport.REVHubInterface.yml` & `revhubinterface-1.3.4.dev5/flatpak/org.unofficialrevport.REVHubInterface.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/flatpak/python3-requirements.json` & `revhubinterface-1.3.4.dev5/flatpak/python3-requirements.json`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.Devel.svg` & `revhubinterface-1.3.4.dev5/org.unofficialrevport.REVHubInterface.Devel.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.Source.svg` & `revhubinterface-1.3.4.dev5/org.unofficialrevport.REVHubInterface.Source.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.icns` & `revhubinterface-1.3.4.dev5/org.unofficialrevport.REVHubInterface.icns`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.ico` & `revhubinterface-1.3.4.dev5/org.unofficialrevport.REVHubInterface.ico`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.metainfo.xml` & `revhubinterface-1.3.4.dev5/org.unofficialrevport.REVHubInterface.metainfo.xml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.svg` & `revhubinterface-1.3.4.dev5/org.unofficialrevport.REVHubInterface.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev4/pyproject.toml` & `revhubinterface-1.3.4.dev5/pyproject.toml`

 * *Files identical despite different names*

