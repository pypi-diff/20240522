# Comparing `tmp/loopquest-0.2.7.tar.gz` & `tmp/loopquest-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopquest-0.2.7.tar", last modified: Tue May 21 05:28:48 2024, max compression
+gzip compressed data, was "loopquest-0.2.8.tar", last modified: Wed May 22 05:54:07 2024, max compression
```

## Comparing `loopquest-0.2.7.tar` & `loopquest-0.2.8.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-21 05:28:48.694895 loopquest-0.2.7/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)    11357 2024-04-19 04:42:45.000000 loopquest-0.2.7/LICENSE
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6567 2024-05-21 05:28:48.690895 loopquest-0.2.7/PKG-INFO
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5380 2024-05-21 03:41:05.000000 loopquest-0.2.7/README.md
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-21 05:28:48.690895 loopquest-0.2.7/loopquest/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       86 2024-04-24 04:38:12.000000 loopquest-0.2.7/loopquest/__init__.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1465 2024-05-21 03:27:00.000000 loopquest-0.2.7/loopquest/api.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9814 2024-05-21 05:03:28.000000 loopquest-0.2.7/loopquest/crud.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1943 2024-05-21 03:39:28.000000 loopquest-0.2.7/loopquest/datasets.py
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-21 05:28:48.690895 loopquest-0.2.7/loopquest/env/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 05:17:29.000000 loopquest-0.2.7/loopquest/env/__init__.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4768 2024-05-08 06:15:15.000000 loopquest-0.2.7/loopquest/env/api.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     6568 2024-05-21 05:15:32.000000 loopquest-0.2.7/loopquest/env/gym_wrappers.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9238 2024-04-19 04:43:26.000000 loopquest-0.2.7/loopquest/env/space_utils.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     6321 2024-05-18 04:12:03.000000 loopquest-0.2.7/loopquest/eval.py
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-21 05:28:48.690895 loopquest-0.2.7/loopquest/policy/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-04-19 04:43:26.000000 loopquest-0.2.7/loopquest/policy/__init__.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      281 2024-05-17 06:20:02.000000 loopquest-0.2.7/loopquest/policy/base.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1383 2024-04-19 04:43:26.000000 loopquest-0.2.7/loopquest/policy/sb3_policy.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1961 2024-05-21 05:27:59.000000 loopquest-0.2.7/loopquest/private_api.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5916 2024-05-21 03:48:15.000000 loopquest-0.2.7/loopquest/schema.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      168 2024-04-19 04:43:26.000000 loopquest-0.2.7/loopquest/typing.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      376 2024-04-19 04:42:45.000000 loopquest-0.2.7/loopquest/ui.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4740 2024-05-19 04:55:08.000000 loopquest-0.2.7/loopquest/utils.py
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-21 05:28:48.690895 loopquest-0.2.7/loopquest.egg-info/
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6567 2024-05-21 05:28:48.000000 loopquest-0.2.7/loopquest.egg-info/PKG-INFO
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      578 2024-05-21 05:28:48.000000 loopquest-0.2.7/loopquest.egg-info/SOURCES.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        1 2024-05-21 05:28:48.000000 loopquest-0.2.7/loopquest.egg-info/dependency_links.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      302 2024-05-21 05:28:48.000000 loopquest-0.2.7/loopquest.egg-info/requires.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       10 2024-05-21 05:28:48.000000 loopquest-0.2.7/loopquest.egg-info/top_level.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       38 2024-05-21 05:28:48.694895 loopquest-0.2.7/setup.cfg
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1144 2024-05-21 05:28:06.000000 loopquest-0.2.7/setup.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-22 05:54:07.216314 loopquest-0.2.8/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)    11357 2024-04-19 04:42:45.000000 loopquest-0.2.8/LICENSE
+-rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6567 2024-05-22 05:54:07.216314 loopquest-0.2.8/PKG-INFO
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5380 2024-05-21 03:41:05.000000 loopquest-0.2.8/README.md
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-22 05:54:07.212314 loopquest-0.2.8/loopquest/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       86 2024-04-24 04:38:12.000000 loopquest-0.2.8/loopquest/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1465 2024-05-21 03:27:00.000000 loopquest-0.2.8/loopquest/api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9814 2024-05-21 05:03:28.000000 loopquest-0.2.8/loopquest/crud.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1943 2024-05-21 03:39:28.000000 loopquest-0.2.8/loopquest/datasets.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-22 05:54:07.212314 loopquest-0.2.8/loopquest/env/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 05:17:29.000000 loopquest-0.2.8/loopquest/env/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4768 2024-05-08 06:15:15.000000 loopquest-0.2.8/loopquest/env/api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     6400 2024-05-22 05:47:04.000000 loopquest-0.2.8/loopquest/env/gym_wrappers.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9238 2024-04-19 04:43:26.000000 loopquest-0.2.8/loopquest/env/space_utils.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     6321 2024-05-18 04:12:03.000000 loopquest-0.2.8/loopquest/eval.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-22 05:54:07.216314 loopquest-0.2.8/loopquest/policy/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-04-19 04:43:26.000000 loopquest-0.2.8/loopquest/policy/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      281 2024-05-17 06:20:02.000000 loopquest-0.2.8/loopquest/policy/base.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1383 2024-04-19 04:43:26.000000 loopquest-0.2.8/loopquest/policy/sb3_policy.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1961 2024-05-22 05:53:20.000000 loopquest-0.2.8/loopquest/private_api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5916 2024-05-21 03:48:15.000000 loopquest-0.2.8/loopquest/schema.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      168 2024-04-19 04:43:26.000000 loopquest-0.2.8/loopquest/typing.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      376 2024-04-19 04:42:45.000000 loopquest-0.2.8/loopquest/ui.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4740 2024-05-19 04:55:08.000000 loopquest-0.2.8/loopquest/utils.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-22 05:54:07.216314 loopquest-0.2.8/loopquest.egg-info/
+-rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6567 2024-05-22 05:54:07.000000 loopquest-0.2.8/loopquest.egg-info/PKG-INFO
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      578 2024-05-22 05:54:07.000000 loopquest-0.2.8/loopquest.egg-info/SOURCES.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        1 2024-05-22 05:54:07.000000 loopquest-0.2.8/loopquest.egg-info/dependency_links.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      302 2024-05-22 05:54:07.000000 loopquest-0.2.8/loopquest.egg-info/requires.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       10 2024-05-22 05:54:07.000000 loopquest-0.2.8/loopquest.egg-info/top_level.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       38 2024-05-22 05:54:07.216314 loopquest-0.2.8/setup.cfg
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1144 2024-05-22 05:51:43.000000 loopquest-0.2.8/setup.py
```

### Comparing `loopquest-0.2.7/LICENSE` & `loopquest-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.7/PKG-INFO` & `loopquest-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopquest
-Version: 0.2.7
+Version: 0.2.8
 Summary: A Production Tool for Embodied AI.
 Home-page: https://github.com/LoopMind-AI/loopquest
 Author: LoopMind
 Author-email: contactus@loopmind.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `loopquest-0.2.7/README.md` & `loopquest-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.7/loopquest/api.py` & `loopquest-0.2.8/loopquest/api.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.7/loopquest/crud.py` & `loopquest-0.2.8/loopquest/crud.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.7/loopquest/datasets.py` & `loopquest-0.2.8/loopquest/datasets.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.7/loopquest/env/api.py` & `loopquest-0.2.8/loopquest/env/api.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.7/loopquest/env/gym_wrappers.py` & `loopquest-0.2.8/loopquest/env/gym_wrappers.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,38 +124,34 @@
                 observation=construct_space_val(self.observation_space, observation),
                 info=info_jsonable,
             ),
         )
         return observation, info
 
     def close(self):
+        self.env.close()
+        self.executor.shutdown()
         update_experiment(
             self.backend_url,
             self.exp_id,
             ExperimentUpdate(status=ExperimentStatus.FINISHED),
         )
         self._try_update_env_profile_image()
-        self.env.close()
-        self.executor.shutdown()
         # TODO: add a callback to compute custom metrics.
 
     def _try_update_env_profile_image(self):
         env_info = get_environment(self.backend_url, self.cloud_env_id)
         env_update = EnvironmentUpdate()
         if env_info.profile_image_id is None:
             image_ids = get_image_ids_by_step(
                 self.backend_url, f"{self.exp_id}-{self.cloud_env_id}-0-1"
             )
-            print(image_ids)
             if len(image_ids) > 0:
-                print("Setting profile image for environment.")
                 env_update.profile_image_id = image_ids[0]
                 update_environment(self.backend_url, self.cloud_env_id, env_update)
-            else:
-                print("No image found for environment.")
 
     def render(self):
         if self.render_mode == "human":
             raise ValueError(
                 "'human' mode is not supported for cloud rendering. Please use other render mode."
             )
         elif self.render_mode in ["ansi", "ansi_list"]:
```

### Comparing `loopquest-0.2.7/loopquest/env/space_utils.py` & `loopquest-0.2.8/loopquest/env/space_utils.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.7/loopquest/eval.py` & `loopquest-0.2.8/loopquest/eval.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.7/loopquest/policy/sb3_policy.py` & `loopquest-0.2.8/loopquest/policy/sb3_policy.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.7/loopquest/private_api.py` & `loopquest-0.2.8/loopquest/private_api.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.7/loopquest/schema.py` & `loopquest-0.2.8/loopquest/schema.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.7/loopquest/utils.py` & `loopquest-0.2.8/loopquest/utils.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.7/loopquest.egg-info/PKG-INFO` & `loopquest-0.2.8/loopquest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopquest
-Version: 0.2.7
+Version: 0.2.8
 Summary: A Production Tool for Embodied AI.
 Home-page: https://github.com/LoopMind-AI/loopquest
 Author: LoopMind
 Author-email: contactus@loopmind.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `loopquest-0.2.7/loopquest.egg-info/SOURCES.txt` & `loopquest-0.2.8/loopquest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.7/setup.py` & `loopquest-0.2.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="loopquest",
-    version="0.2.7",
+    version="0.2.8",
     description="A Production Tool for Embodied AI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="LoopMind",
     author_email="contactus@loopmind.ai",
     url="https://github.com/LoopMind-AI/loopquest",
     packages=find_packages(),
```

