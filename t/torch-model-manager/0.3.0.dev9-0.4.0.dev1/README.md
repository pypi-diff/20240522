# Comparing `tmp/torch_model_manager-0.3.0.dev9.tar.gz` & `tmp/torch_model_manager-0.4.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.3.0.dev9.tar", last modified: Sun May 12 22:27:39 2024, max compression
+gzip compressed data, was "torch_model_manager-0.4.0.dev1.tar", last modified: Wed May 22 10:46:26 2024, max compression
```

## Comparing `torch_model_manager-0.3.0.dev9.tar` & `torch_model_manager-0.4.0.dev1.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 22:27:39.137407 torch_model_manager-0.3.0.dev9/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8905 2024-05-12 22:27:39.137407 torch_model_manager-0.3.0.dev9/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev9/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-12 22:27:39.137407 torch_model_manager-0.3.0.dev9/setup.cfg
--rwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)     1975 2024-05-12 22:27:35.000000 torch_model_manager-0.3.0.dev9/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 22:27:39.097407 torch_model_manager-0.3.0.dev9/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 22:27:39.097407 torch_model_manager-0.3.0.dev9/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev9/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev9/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 22:27:39.097407 torch_model_manager-0.3.0.dev9/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev9/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev9/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 22:27:39.117407 torch_model_manager-0.3.0.dev9/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       94 2024-05-12 20:02:05.000000 torch_model_manager-0.3.0.dev9/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    31658 2024-05-12 19:39:19.000000 torch_model_manager-0.3.0.dev9/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     1774 2024-05-12 22:26:57.000000 torch_model_manager-0.3.0.dev9/torch_model_manager/notebook_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    18831 2024-05-09 18:52:45.000000 torch_model_manager-0.3.0.dev9/torch_model_manager/torch_model_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2442 2024-05-11 10:54:45.000000 torch_model_manager-0.3.0.dev9/torch_model_manager/wandb_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 22:27:39.137407 torch_model_manager-0.3.0.dev9/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8905 2024-05-12 22:27:39.000000 torch_model_manager-0.3.0.dev9/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      622 2024-05-12 22:27:39.000000 torch_model_manager-0.3.0.dev9/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-12 22:27:39.000000 torch_model_manager-0.3.0.dev9/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      116 2024-05-12 22:27:39.000000 torch_model_manager-0.3.0.dev9/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-12 22:27:39.000000 torch_model_manager-0.3.0.dev9/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-12 22:27:39.137407 torch_model_manager-0.3.0.dev9/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.3.0.dev9/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8619 2024-05-09 19:01:45.000000 torch_model_manager-0.3.0.dev9/utils/helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 10:46:26.726062 torch_model_manager-0.4.0.dev1/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9032 2024-05-22 10:46:26.722061 torch_model_manager-0.4.0.dev1/PKG-INFO
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     8105 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev1/README.md
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       38 2024-05-22 10:46:26.726062 torch_model_manager-0.4.0.dev1/setup.cfg
+-rwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)     2082 2024-05-22 10:46:24.000000 torch_model_manager-0.4.0.dev1/setup.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 10:46:26.718062 torch_model_manager-0.4.0.dev1/tests/
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 10:46:26.718062 torch_model_manager-0.4.0.dev1/tests/test_torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev1/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2462 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev1/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 10:46:26.718062 torch_model_manager-0.4.0.dev1/tests/test_utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev1/tests/test_utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     3018 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev1/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 10:46:26.722061 torch_model_manager-0.4.0.dev1/torch_model_manager/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      148 2024-05-22 10:34:37.000000 torch_model_manager-0.4.0.dev1/torch_model_manager/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    32749 2024-05-17 13:07:00.000000 torch_model_manager-0.4.0.dev1/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     1774 2024-05-13 09:13:42.000000 torch_model_manager-0.4.0.dev1/torch_model_manager/notebook_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    12708 2024-05-22 10:44:37.000000 torch_model_manager-0.4.0.dev1/torch_model_manager/segmentation_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)    18831 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev1/torch_model_manager/torch_model_manager.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     2442 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev1/torch_model_manager/wandb_manager.py
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 10:46:26.722061 torch_model_manager-0.4.0.dev1/torch_model_manager.egg-info/
+-rw-r--r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     9032 2024-05-22 10:46:26.000000 torch_model_manager-0.4.0.dev1/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      666 2024-05-22 10:46:26.000000 torch_model_manager-0.4.0.dev1/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        1 2024-05-22 10:46:26.000000 torch_model_manager-0.4.0.dev1/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)      168 2024-05-22 10:46:26.000000 torch_model_manager-0.4.0.dev1/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)       32 2024-05-22 10:46:26.000000 torch_model_manager-0.4.0.dev1/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-22 10:46:26.722061 torch_model_manager-0.4.0.dev1/utils/
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)        0 2024-05-13 08:52:52.000000 torch_model_manager-0.4.0.dev1/utils/__init__.py
+-rw-rw-r--   0 bimokhtari1  (1002) bimokhtari1  (1002)     8619 2024-05-13 08:53:31.000000 torch_model_manager-0.4.0.dev1/utils/helpers.py
```

### Comparing `torch_model_manager-0.3.0.dev9/PKG-INFO` & `torch_model_manager-0.4.0.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.3.0.dev9
+Version: 0.4.0.dev1
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,19 @@
 Requires-Dist: torchcam
 Requires-Dist: colorama
 Requires-Dist: neptune_pytorch
 Requires-Dist: torchview
 Requires-Dist: graphviz
 Requires-Dist: wandb
 Requires-Dist: ydata_profiling
+Requires-Dist: diffusers
+Requires-Dist: transformers
+Requires-Dist: accelerate
+Requires-Dist: scipy
+Requires-Dist: safetensors
 
 # Torch Model Manager
 
 
 **Torch Model Manager** is an open-source python project designed for Deep Learning developpers that aims to make the use of pytorch library easy. The version ![version](https://img.shields.io/badge/version-0.0.5-gray?labelColor=blue&style=flat) is still under developpment. The package allows us to access, search and delete layers by index, attributes or instance.
 
 ### Examples of Use
```

### Comparing `torch_model_manager-0.3.0.dev9/README.md` & `torch_model_manager-0.4.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev9/setup.py` & `torch_model_manager-0.4.0.dev1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='torch-model-manager',
-    version='0.3.0.dev9',
+    version='0.4.0.dev1',
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests', 
                                     'docs', 
                                     'build.sh', 
                                     'requirements.sh', 
@@ -43,15 +43,20 @@
         'torchviz',
         'torchcam',
         'colorama',
         'neptune_pytorch',
         'torchview',
         'graphviz',
         'wandb',
-        'ydata_profiling'
+        'ydata_profiling',
+        'diffusers',
+        'transformers',
+        'accelerate',
+        'scipy',
+        'safetensors'
         # Add any other dependencies here
     ],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
     ],
```

### Comparing `torch_model_manager-0.3.0.dev9/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.4.0.dev1/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev9/tests/test_utils/test_helpers.py` & `torch_model_manager-0.4.0.dev1/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev9/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.4.0.dev1/torch_model_manager/neptune_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -310,14 +310,27 @@
         
             print(Fore.GREEN+"The data is successfully fetched from Neptune.", Fore.WHITE)
             return data
             
         except:
             print(Fore.RED+"The data is not fetched from Neptune. Please check the namespace."+Fore.WHITE)
 
+    def fetch_csv_data(self, namespace: str, **kwargs):        
+        tmp_file = tempfile.NamedTemporaryFile(delete=True)
+        try :
+            NeptuneManager.project[namespace].download(tmp_file.name)
+
+            data = pd.read_csv(tmp_file.name, **kwargs)
+            print(Fore.GREEN+"The data is successfully fetched from Neptune.", Fore.WHITE)
+            return data
+            
+        except:
+            print(Fore.RED+"The data is not fetched from Neptune. Please check the namespace."+Fore.WHITE)
+
+
     class Run:
         """
         A class representing a Neptune run.
         """
         def __init__(self, 
                     name: str, 
                     description: str = None, 
@@ -367,14 +380,15 @@
                         capture_stderr=capture_strerr,
                         git_ref=git_ref,
                         **kwargs
                     ) 
                     # Retrieve the id of the run and store it in the file with its associated name
                     self.run_id = self.run["sys/id"].fetch()
                     helpers.add_to_json_file(NeptuneManager.run_ids_path, self.name, self.run_id)
+                    
             except:
                 print(Fore.RED+"The JSON file is not found. Please check the path."+Fore.WHITE)
             
         def log_tensors(self, 
                         tensors, 
                         descriptions: List[str] = None, 
                         names: List[str] = None, 
@@ -698,14 +712,27 @@
             
                 print(Fore.GREEN+"The data is successfully fetched from Neptune.", Fore.WHITE)
                 return data
                 
             except:
                 print(Fore.RED+"The data is not fetched from Neptune. Please check the namespace."+Fore.WHITE)
 
+        def fetch_csv_data(self, namespace: str, **kwargs):        
+            tmp_file = tempfile.NamedTemporaryFile(delete=True)
+            try :
+                self.run.project[namespace].download(tmp_file.name)
+
+                data = pd.read_csv(tmp_file.name, **kwargs)
+                print(Fore.GREEN+"The data is successfully fetched from Neptune.", Fore.WHITE)
+                return data
+                
+            except:
+                print(Fore.RED+"The data is not fetched from Neptune. Please check the namespace."+Fore.WHITE)
+
+
         def load_model_checkpoint(self, namespace, **kwargs):
             """
             Loads a model checkpoint from Neptune.
 
             Args:
                 namespace (str): The namespace where the checkpoint is stored.
                 **kwargs: Additional keyword arguments for torch.load().
```

### Comparing `torch_model_manager-0.3.0.dev9/torch_model_manager/notebook_manager.py` & `torch_model_manager-0.4.0.dev1/torch_model_manager/notebook_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev9/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.4.0.dev1/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev9/torch_model_manager/wandb_manager.py` & `torch_model_manager-0.4.0.dev1/torch_model_manager/wandb_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.3.0.dev9/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.4.0.dev1/torch_model_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.3.0.dev9
+Version: 0.4.0.dev1
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -18,14 +18,19 @@
 Requires-Dist: torchcam
 Requires-Dist: colorama
 Requires-Dist: neptune_pytorch
 Requires-Dist: torchview
 Requires-Dist: graphviz
 Requires-Dist: wandb
 Requires-Dist: ydata_profiling
+Requires-Dist: diffusers
+Requires-Dist: transformers
+Requires-Dist: accelerate
+Requires-Dist: scipy
+Requires-Dist: safetensors
 
 # Torch Model Manager
 
 
 **Torch Model Manager** is an open-source python project designed for Deep Learning developpers that aims to make the use of pytorch library easy. The version ![version](https://img.shields.io/badge/version-0.0.5-gray?labelColor=blue&style=flat) is still under developpment. The package allows us to access, search and delete layers by index, attributes or instance.
 
 ### Examples of Use
```

### Comparing `torch_model_manager-0.3.0.dev9/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.4.0.dev1/torch_model_manager.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 tests/test_torch_model_manager/__init__.py
 tests/test_torch_model_manager/test_torch_model_manager.py
 tests/test_utils/__init__.py
 tests/test_utils/test_helpers.py
 torch_model_manager/__init__.py
 torch_model_manager/neptune_manager.py
 torch_model_manager/notebook_manager.py
+torch_model_manager/segmentation_manager.py
 torch_model_manager/torch_model_manager.py
 torch_model_manager/wandb_manager.py
 torch_model_manager.egg-info/PKG-INFO
 torch_model_manager.egg-info/SOURCES.txt
 torch_model_manager.egg-info/dependency_links.txt
 torch_model_manager.egg-info/requires.txt
 torch_model_manager.egg-info/top_level.txt
```

### Comparing `torch_model_manager-0.3.0.dev9/utils/helpers.py` & `torch_model_manager-0.4.0.dev1/utils/helpers.py`

 * *Files identical despite different names*

