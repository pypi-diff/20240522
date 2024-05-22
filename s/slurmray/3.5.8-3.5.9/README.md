# Comparing `tmp/slurmray-3.5.8.tar.gz` & `tmp/slurmray-3.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slurmray-3.5.8.tar", max compression
+gzip compressed data, was "slurmray-3.5.9.tar", max compression
```

## Comparing `slurmray-3.5.8.tar` & `slurmray-3.5.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2023-11-02 15:45:02.729834 slurmray-3.5.8/LICENSE
--rw-r--r--   0        0        0     2591 2024-02-21 14:55:58.866123 slurmray-3.5.8/README.md
--rw-r--r--   0        0        0      753 2024-02-21 14:56:35.596122 slurmray-3.5.8/pyproject.toml
--rw-r--r--   0        0        0    22617 2024-02-21 14:21:02.206136 slurmray-3.5.8/slurmray/RayLauncher.py
--rw-r--r--   0        0        0        0 2023-11-02 16:26:02.359793 slurmray-3.5.8/slurmray/__init__.py
--rw-r--r--   0        0        0     2273 2023-11-02 15:45:02.729834 slurmray-3.5.8/slurmray/assets/sbatch_template.sh
--rw-r--r--   0        0        0      638 2024-02-21 14:10:44.516140 slurmray-3.5.8/slurmray/assets/slurmray_server.sh
--rw-r--r--   0        0        0      575 2024-02-21 14:18:41.636137 slurmray-3.5.8/slurmray/assets/slurmray_server_template.py
--rw-r--r--   0        0        0      597 2023-12-04 17:09:52.015256 slurmray-3.5.8/slurmray/assets/spython_template.py
--rw-r--r--   0        0        0     3395 1970-01-01 00:00:00.000000 slurmray-3.5.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-03 09:04:55.530868 slurmray-3.5.9/LICENSE
+-rw-r--r--   0        0        0     2591 2024-05-22 08:54:20.413962 slurmray-3.5.9/README.md
+-rw-r--r--   0        0        0      751 2024-05-22 09:01:26.563863 slurmray-3.5.9/pyproject.toml
+-rw-r--r--   0        0        0    22617 2024-05-22 08:54:20.413962 slurmray-3.5.9/slurmray/RayLauncher.py
+-rw-r--r--   0        0        0        0 2023-11-03 09:04:55.530868 slurmray-3.5.9/slurmray/__init__.py
+-rw-r--r--   0        0        0     2273 2023-11-03 09:04:55.530868 slurmray-3.5.9/slurmray/assets/sbatch_template.sh
+-rw-r--r--   0        0        0      638 2023-12-11 23:26:19.853300 slurmray-3.5.9/slurmray/assets/slurmray_server.sh
+-rw-r--r--   0        0        0      575 2024-05-22 08:54:20.413962 slurmray-3.5.9/slurmray/assets/slurmray_server_template.py
+-rw-r--r--   0        0        0      597 2023-12-05 14:46:52.657175 slurmray-3.5.9/slurmray/assets/spython_template.py
+-rw-r--r--   0        0        0     3549 1970-01-01 00:00:00.000000 slurmray-3.5.9/PKG-INFO
```

### Comparing `slurmray-3.5.8/LICENSE` & `slurmray-3.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `slurmray-3.5.8/README.md` & `slurmray-3.5.9/README.md`

 * *Files identical despite different names*

### Comparing `slurmray-3.5.8/pyproject.toml` & `slurmray-3.5.9/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "slurmray"
-version = "3.5.8"
+version = "3.5.9"
 description = "SlurmRay is a module for effortlessly distributing tasks on a Slurm cluster using the Ray library. "
 authors = ["Henri Jamet <henri.jamet@unil.ch>"]
 license = "Apache License"
 homepage = "https://henri-jamet.vercel.app/"
 documentation = "https://henri-jamet.vercel.app/cards/documentation/slurm-ray/slurm-ray/"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "3.9.13"
+python = "^3.9"
 dill = "^0.3.7"
 ray = {extras = ["data", "serve", "train", "tune"], version = "^2.7.1"}
 pdoc3 = "^0.10.0"
 paramiko = "^3.3.1"
 torch = "^2.1.1"
 pip-chill = "^1.0.3"
```

### Comparing `slurmray-3.5.8/slurmray/RayLauncher.py` & `slurmray-3.5.9/slurmray/RayLauncher.py`

 * *Files identical despite different names*

### Comparing `slurmray-3.5.8/slurmray/assets/sbatch_template.sh` & `slurmray-3.5.9/slurmray/assets/sbatch_template.sh`

 * *Files identical despite different names*

### Comparing `slurmray-3.5.8/slurmray/assets/slurmray_server.sh` & `slurmray-3.5.9/slurmray/assets/slurmray_server.sh`

 * *Files identical despite different names*

### Comparing `slurmray-3.5.8/slurmray/assets/slurmray_server_template.py` & `slurmray-3.5.9/slurmray/assets/slurmray_server_template.py`

 * *Files identical despite different names*

### Comparing `slurmray-3.5.8/slurmray/assets/spython_template.py` & `slurmray-3.5.9/slurmray/assets/spython_template.py`

 * *Files identical despite different names*

### Comparing `slurmray-3.5.8/PKG-INFO` & `slurmray-3.5.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 Metadata-Version: 2.1
 Name: slurmray
-Version: 3.5.8
+Version: 3.5.9
 Summary: SlurmRay is a module for effortlessly distributing tasks on a Slurm cluster using the Ray library. 
 Home-page: https://henri-jamet.vercel.app/
 License: Apache License
 Author: Henri Jamet
 Author-email: henri.jamet@unil.ch
-Requires-Python: ==3.9.13
+Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: dill (>=0.3.7,<0.4.0)
 Requires-Dist: paramiko (>=3.3.1,<4.0.0)
 Requires-Dist: pdoc3 (>=0.10.0,<0.11.0)
 Requires-Dist: pip-chill (>=1.0.3,<2.0.0)
 Requires-Dist: ray[data,serve,train,tune] (>=2.7.1,<3.0.0)
 Requires-Dist: torch (>=2.1.1,<3.0.0)
 Project-URL: Documentation, https://henri-jamet.vercel.app/cards/documentation/slurm-ray/slurm-ray/
```

