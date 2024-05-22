# Comparing `tmp/fastdev-0.0.3.tar.gz` & `tmp/fastdev-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastdev-0.0.3.tar", last modified: Sat May 18 01:36:01 2024, max compression
+gzip compressed data, was "fastdev-0.0.4.tar", last modified: Wed May 22 08:13:50 2024, max compression
```

## Comparing `fastdev-0.0.3.tar` & `fastdev-0.0.4.tar`

### file list

```diff
@@ -1,51 +1,49 @@
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.245540 fastdev-0.0.3/
--rw-r--r--   0 jianglong  (1000) jianglong  (1000)      888 2024-05-18 01:36:01.245540 fastdev-0.0.3/PKG-INFO
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       32 2024-05-13 08:49:05.000000 fastdev-0.0.3/README.md
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      849 2024-05-18 01:34:25.000000 fastdev-0.0.3/pyproject.toml
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       38 2024-05-18 01:36:01.245540 fastdev-0.0.3/setup.cfg
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.242540 fastdev-0.0.3/src/
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.243540 fastdev-0.0.3/src/fastdev/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       69 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      597 2024-05-14 01:25:51.000000 fastdev-0.0.3/src/fastdev/constants.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.243540 fastdev-0.0.3/src/fastdev/datasets/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/datasets/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)    17435 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/datasets/dexycb.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.243540 fastdev-0.0.3/src/fastdev/fileio/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       69 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/fileio/__init__.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.244540 fastdev-0.0.3/src/fastdev/fileio/handlers/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/fileio/handlers/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      533 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/fileio/handlers/base_handler.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      699 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/fileio/handlers/json_handler.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1737 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/fileio/handlers/yaml_handler.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     2722 2024-05-15 08:19:43.000000 fastdev-0.0.3/src/fastdev/fileio/io.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.244540 fastdev-0.0.3/src/fastdev/robotics/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       90 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/robotics/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      273 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/robotics/kinematics.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1028 2024-05-14 00:31:47.000000 fastdev-0.0.3/src/fastdev/robotics/urdf.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.244540 fastdev-0.0.3/src/fastdev/smplx/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      256 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/smplx/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     3778 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/smplx/smplx.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.244540 fastdev-0.0.3/src/fastdev/transforms/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1421 2024-05-18 00:55:47.000000 fastdev-0.0.3/src/fastdev/transforms/__init__.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.244540 fastdev-0.0.3/src/fastdev/transforms/numpy/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      103 2024-05-15 07:37:41.000000 fastdev-0.0.3/src/fastdev/transforms/numpy/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1007 2024-05-15 07:38:48.000000 fastdev-0.0.3/src/fastdev/transforms/numpy/transforms.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)    17378 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/transforms/rotation.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     5547 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/transforms/transforms.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     2881 2024-05-18 00:54:56.000000 fastdev-0.0.3/src/fastdev/transforms/utils.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.244540 fastdev-0.0.3/src/fastdev/utils/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       59 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/utils/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1188 2024-05-17 08:54:36.000000 fastdev-0.0.3/src/fastdev/utils/geometry.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1313 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/utils/timer.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.244540 fastdev-0.0.3/src/fastdev/visualization/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       79 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/visualization/__init__.py
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1680 2024-05-13 08:49:05.000000 fastdev-0.0.3/src/fastdev/visualization/image.py
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.244540 fastdev-0.0.3/src/fastdev.egg-info/
--rw-r--r--   0 jianglong  (1000) jianglong  (1000)      888 2024-05-18 01:36:01.000000 fastdev-0.0.3/src/fastdev.egg-info/PKG-INFO
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1135 2024-05-18 01:36:01.000000 fastdev-0.0.3/src/fastdev.egg-info/SOURCES.txt
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        1 2024-05-18 01:36:01.000000 fastdev-0.0.3/src/fastdev.egg-info/dependency_links.txt
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       50 2024-05-18 01:36:01.000000 fastdev-0.0.3/src/fastdev.egg-info/entry_points.txt
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      146 2024-05-18 01:36:01.000000 fastdev-0.0.3/src/fastdev.egg-info/requires.txt
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        8 2024-05-18 01:36:01.000000 fastdev-0.0.3/src/fastdev.egg-info/top_level.txt
-drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-18 01:36:01.244540 fastdev-0.0.3/tests/
--rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1199 2024-05-13 08:49:05.000000 fastdev-0.0.3/tests/test_fileio.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.105966 fastdev-0.0.4/
+-rw-r--r--   0 jianglong  (1000) jianglong  (1000)      959 2024-05-22 08:13:50.105966 fastdev-0.0.4/PKG-INFO
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       45 2024-05-22 06:56:45.000000 fastdev-0.0.4/README.md
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      943 2024-05-22 08:13:08.000000 fastdev-0.0.4/pyproject.toml
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       38 2024-05-22 08:13:50.105966 fastdev-0.0.4/setup.cfg
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.103966 fastdev-0.0.4/src/
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.103966 fastdev-0.0.4/src/fastdev/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       69 2024-05-13 08:49:05.000000 fastdev-0.0.4/src/fastdev/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      597 2024-05-14 01:25:51.000000 fastdev-0.0.4/src/fastdev/constants.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.104966 fastdev-0.0.4/src/fastdev/datasets/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-13 08:49:05.000000 fastdev-0.0.4/src/fastdev/datasets/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)    17763 2024-05-22 08:09:51.000000 fastdev-0.0.4/src/fastdev/datasets/dexycb.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.104966 fastdev-0.0.4/src/fastdev/fileio/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       69 2024-05-13 08:49:05.000000 fastdev-0.0.4/src/fastdev/fileio/__init__.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.104966 fastdev-0.0.4/src/fastdev/fileio/handlers/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-13 08:49:05.000000 fastdev-0.0.4/src/fastdev/fileio/handlers/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      501 2024-05-22 08:08:06.000000 fastdev-0.0.4/src/fastdev/fileio/handlers/base_handler.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      699 2024-05-13 08:49:05.000000 fastdev-0.0.4/src/fastdev/fileio/handlers/json_handler.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1737 2024-05-22 07:11:50.000000 fastdev-0.0.4/src/fastdev/fileio/handlers/yaml_handler.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     2789 2024-05-22 08:09:51.000000 fastdev-0.0.4/src/fastdev/fileio/io.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 07:27:36.000000 fastdev-0.0.4/src/fastdev/py.typed
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.104966 fastdev-0.0.4/src/fastdev/robotics/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       90 2024-05-13 08:49:05.000000 fastdev-0.0.4/src/fastdev/robotics/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1028 2024-05-22 08:09:51.000000 fastdev-0.0.4/src/fastdev/robotics/urdf.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.104966 fastdev-0.0.4/src/fastdev/smplx/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      275 2024-05-22 08:08:06.000000 fastdev-0.0.4/src/fastdev/smplx/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     3996 2024-05-22 08:09:51.000000 fastdev-0.0.4/src/fastdev/smplx/smplx.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.104966 fastdev-0.0.4/src/fastdev/transforms/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1421 2024-05-18 00:55:47.000000 fastdev-0.0.4/src/fastdev/transforms/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)    17378 2024-05-22 08:09:51.000000 fastdev-0.0.4/src/fastdev/transforms/rotation.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     6452 2024-05-22 08:09:51.000000 fastdev-0.0.4/src/fastdev/transforms/transforms.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     2964 2024-05-22 08:09:51.000000 fastdev-0.0.4/src/fastdev/transforms/utils.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.104966 fastdev-0.0.4/src/fastdev/utils/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      123 2024-05-22 07:54:17.000000 fastdev-0.0.4/src/fastdev/utils/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      782 2024-05-22 07:31:36.000000 fastdev-0.0.4/src/fastdev/utils/dispatch.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1188 2024-05-17 08:54:36.000000 fastdev-0.0.4/src/fastdev/utils/geometry.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1339 2024-05-22 07:11:15.000000 fastdev-0.0.4/src/fastdev/utils/timer.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.104966 fastdev-0.0.4/src/fastdev/visualization/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)       79 2024-05-13 08:49:05.000000 fastdev-0.0.4/src/fastdev/visualization/__init__.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1803 2024-05-22 08:09:51.000000 fastdev-0.0.4/src/fastdev/visualization/image.py
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.105966 fastdev-0.0.4/src/fastdev.egg-info/
+-rw-r--r--   0 jianglong  (1000) jianglong  (1000)      959 2024-05-22 08:13:50.000000 fastdev-0.0.4/src/fastdev.egg-info/PKG-INFO
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1054 2024-05-22 08:13:50.000000 fastdev-0.0.4/src/fastdev.egg-info/SOURCES.txt
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        1 2024-05-22 08:13:50.000000 fastdev-0.0.4/src/fastdev.egg-info/dependency_links.txt
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      158 2024-05-22 08:13:50.000000 fastdev-0.0.4/src/fastdev.egg-info/requires.txt
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)        8 2024-05-22 08:13:50.000000 fastdev-0.0.4/src/fastdev.egg-info/top_level.txt
+drwxrwxr-x   0 jianglong  (1000) jianglong  (1000)        0 2024-05-22 08:13:50.105966 fastdev-0.0.4/tests/
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)     1199 2024-05-13 08:49:05.000000 fastdev-0.0.4/tests/test_fileio.py
+-rw-rw-r--   0 jianglong  (1000) jianglong  (1000)      663 2024-05-22 06:55:51.000000 fastdev-0.0.4/tests/test_transforms.py
```

### Comparing `fastdev-0.0.3/PKG-INFO` & `fastdev-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: fastdev
-Version: 0.0.3
+Version: 0.0.4
 Summary: Type less, code more
 Author-email: Jianglong Ye <jianglong.yeh@gmail.com>
 License: MIT
 Project-URL: Repository, https://github.com/jianglongye/fastdev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: fastcore
 Requires-Dist: msgspec[toml,yaml]
 Requires-Dist: rich
 Requires-Dist: fsspec
 Requires-Dist: universal_pathlib
 Requires-Dist: huggingface_hub[cli,hf_transfer]
 Requires-Dist: GitPython
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
-Requires-Dist: lovely-tensors; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: types-PyYAML; extra == "dev"
 
 # FastDev
 
 Type Less, Code More
+
+## Features
```

### Comparing `fastdev-0.0.3/src/fastdev/constants.py` & `fastdev-0.0.4/src/fastdev/constants.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.3/src/fastdev/datasets/dexycb.py` & `fastdev-0.0.4/src/fastdev/datasets/dexycb.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,19 @@
         self._w = 640
         self._obj_file = {k: os.path.join(self._model_dir, v, "textured_simple.obj") for k, v in _YCB_CLASSES.items()}
 
         # ----------- Cache Metadata -----------
         if (not os.path.exists(self.config.metadata_cache_path)) or self.config.force_rebuild_cache:
             intrinsics = {}
             for serial in _SERIALS:
-                intr_file = os.path.join(self._calib_dir, "intrinsics", "{}_{}x{}.yml".format(serial, self._w, self._h))
+                intr_file = os.path.join(
+                    self._calib_dir,
+                    "intrinsics",
+                    "{}_{}x{}.yml".format(serial, self._w, self._h),
+                )
                 intr = load(intr_file)
                 intrinsics[serial] = intr["color"]
 
             extrinsics = {}
             extr_dirs = sorted(glob(os.path.join(self._calib_dir, "extrinsics_*")))
             for extr_dir in extr_dirs:
                 extr = load(os.path.join(extr_dir, "extrinsics.yml"))
@@ -164,15 +168,18 @@
                         if np.any(valid_frames):
                             valid_begin_frame, valid_end_frame = np.where(valid_frames)[0][[0, -1]]
                         else:
                             # no valid frames
                             valid_begin_frame, valid_end_frame = -1, -1
 
                         # range is always half-open
-                        seq_metas[seq]["valid_frame_range"][serial] = (valid_begin_frame, valid_end_frame + 1)
+                        seq_metas[seq]["valid_frame_range"][serial] = (
+                            valid_begin_frame,
+                            valid_end_frame + 1,
+                        )
                         seq_metas[seq]["joint_2d"][serial] = joint_2d
                         seq_metas[seq]["joint_3d"][serial] = np.stack([label["joint_3d"][0] for label in label_data])
                         seq_metas[seq]["pose_m"][serial] = np.stack([label["pose_m"][0] for label in label_data])
                         seq_metas[seq]["pose_y"][serial] = np.stack([label["pose_y"][0] for label in label_data])
 
             os.makedirs(os.path.dirname(self.config.metadata_cache_path), exist_ok=True)
             with open(self.config.metadata_cache_path, "wb") as f:
@@ -330,15 +337,18 @@
             "sequence": self._sequences[seq_idx],
             "serial": self._serials[serial_idx],
             "frame_range": torch.tensor(frame_range, dtype=torch.int32),
             "intrinsics": self._intrinsics[self._serials[serial_idx]],
             "extrinsics": extr,
             "ycb_grasp_id": seq_meta["ycb_ids"][seq_meta["ycb_grasp_ind"]],
             "mano_side": seq_meta["mano_sides"][0],
-            "mano_betas": torch.tensor(self._mano_calibs[seq_meta["mano_calib"][0]]["betas"], dtype=torch.float32),
+            "mano_betas": torch.tensor(
+                self._mano_calibs[seq_meta["mano_calib"][0]]["betas"],
+                dtype=torch.float32,
+            ),
         }
 
         frames_data = [self._load_frame_data(data_dir, frame_idx) for frame_idx in range(*frame_range)]
         for key in frames_data[0].keys():
             sample[key] = torch.stack([frame_data[key] for frame_data in frames_data], dim=0)
             if not self.config.return_as_sequence:
                 sample[key].squeeze_(0)
@@ -387,15 +397,21 @@
                 )
             )[0]
 
     def build_collate_fn(self):
         def _seq_collate_fn(batch):
             collated_batch = {}
             for key in batch[0].keys():
-                if key in ["color", "depth", "mano_global_orient", "mano_hand_pose", "mano_transl"]:
+                if key in [
+                    "color",
+                    "depth",
+                    "mano_global_orient",
+                    "mano_hand_pose",
+                    "mano_transl",
+                ]:
                     collated_batch[key] = pad_sequence([sample[key] for sample in batch], batch_first=True)
                 else:
                     collated_batch[key] = default_collate([sample[key] for sample in batch])
             return collated_batch
 
         if not self.config.return_as_sequence:
             return default_collate
```

### Comparing `fastdev-0.0.3/src/fastdev/fileio/handlers/json_handler.py` & `fastdev-0.0.4/src/fastdev/fileio/handlers/json_handler.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.3/src/fastdev/fileio/handlers/yaml_handler.py` & `fastdev-0.0.4/src/fastdev/fileio/handlers/yaml_handler.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.3/src/fastdev/fileio/io.py` & `fastdev-0.0.4/src/fastdev/fileio/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from functools import lru_cache
 from pathlib import Path
-from typing import IO, Any, Dict, Optional, Union, cast
+from typing import IO, Any, Dict, Mapping, Optional, Type, Union, cast
 
-import fsspec
+import fsspec  # type: ignore
 
 from fastdev.fileio.handlers.base_handler import BaseFileHandler
 from fastdev.fileio.handlers.json_handler import JSONHandler
 from fastdev.fileio.handlers.yaml_handler import YAMLHandler
 
-FILE_HANDLER_CLASSES = {
+FILE_HANDLER_CLASSES: Mapping[str, Type[BaseFileHandler]] = {
     "json": JSONHandler,
     "yaml": YAMLHandler,
     "yml": YAMLHandler,
 }
 FILE_HANDLERS: Dict[str, BaseFileHandler] = {}
 
 
-
 @lru_cache()
 def get_file_handler(file_format: str) -> BaseFileHandler:
     if file_format not in FILE_HANDLERS:
         if file_format not in FILE_HANDLER_CLASSES:
             raise ValueError(f"Unsupported file format: {file_format}")
         else:
             FILE_HANDLERS[file_format] = FILE_HANDLER_CLASSES[file_format]()
```

### Comparing `fastdev-0.0.3/src/fastdev/robotics/urdf.py` & `fastdev-0.0.4/src/fastdev/robotics/urdf.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.3/src/fastdev/smplx/smplx.py` & `fastdev-0.0.4/src/fastdev/smplx/smplx.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import os
 from typing import Literal, Optional, Tuple
 
 import torch
-from huggingface_hub import hf_hub_download
+from huggingface_hub import hf_hub_download  # type: ignore
 
 try:
-    from smplx import MANO
-    from smplx.lbs import blend_shapes, vertices2joints
+    from smplx import MANO  # type: ignore
+    from smplx.lbs import blend_shapes, vertices2joints  # type: ignore
 except ImportError:
     raise ImportError("Please install smplx to use this feature. \nYou can install it by running `pip install smplx`.")
 
 import fastdev.transforms as tf
 from fastdev.constants import FDEV_HF_CACHE_ROOT, FDEV_HF_REPO_ID
 
 
 def get_local_mano_model_path(hand_side: Literal["left", "right"] = "left") -> str:
     mano_path = os.path.join(FDEV_HF_CACHE_ROOT, "smplx", "mano", f"MANO_{hand_side.upper()}.pkl")
     if not os.path.exists(mano_path):
         hf_hub_download(
-            repo_id=FDEV_HF_REPO_ID, filename=f"smplx/mano/MANO_{hand_side.upper()}.pkl", local_dir=FDEV_HF_CACHE_ROOT
+            repo_id=FDEV_HF_REPO_ID,
+            filename=f"smplx/mano/MANO_{hand_side.upper()}.pkl",
+            local_dir=FDEV_HF_CACHE_ROOT,
         )
     return mano_path
 
 
 def build_mano_layer(
     hand_side: Literal["left", "right"] = "left",
     create_transl: bool = False,
@@ -39,15 +41,18 @@
         is_rhand=(hand_side == "right"),
     )
 
     # workround for https://github.com/vchoutas/smplx/issues/192#issue-2272600127
     mano.use_pca = use_pca
     mano.num_pca_comps = num_pca_comps
     if mano.use_pca:
-        mano.register_buffer("hand_components", torch.tensor(mano.np_hand_components, dtype=torch.float32))
+        mano.register_buffer(
+            "hand_components",
+            torch.tensor(mano.np_hand_components, dtype=torch.float32),
+        )
 
     return mano
 
 
 def build_mano_layer_manopth(
     hand_side: Literal["left", "right"] = "left",
     flat_hand_mean: bool = False,
@@ -61,19 +66,27 @@
     # fix for chumpy
     np.bool = np.bool_  # type: ignore
     np.int = np.int_  # type: ignore
     np.float = np.float_  # type: ignore
     np.complex = np.complex_  # type: ignore
     np.object = np.object_  # type: ignore
     np.str = np.str_  # type: ignore
-    from manopth.manolayer import ManoLayer
+    from manopth.manolayer import ManoLayer  # type: ignore
 
     if not os.path.exists(os.path.join(FDEV_HF_CACHE_ROOT, "smplx", "mano", "MANO_LEFT.pkl")):
-        hf_hub_download(repo_id=FDEV_HF_REPO_ID, filename="smplx/mano/MANO_LEFT.pkl", local_dir=FDEV_HF_CACHE_ROOT)
-        hf_hub_download(repo_id=FDEV_HF_REPO_ID, filename="smplx/mano/MANO_RIGHT.pkl", local_dir=FDEV_HF_CACHE_ROOT)
+        hf_hub_download(
+            repo_id=FDEV_HF_REPO_ID,
+            filename="smplx/mano/MANO_LEFT.pkl",
+            local_dir=FDEV_HF_CACHE_ROOT,
+        )
+        hf_hub_download(
+            repo_id=FDEV_HF_REPO_ID,
+            filename="smplx/mano/MANO_RIGHT.pkl",
+            local_dir=FDEV_HF_CACHE_ROOT,
+        )
 
     warnings.filterwarnings("ignore", category=UserWarning, module="manopth")
     return ManoLayer(
         flat_hand_mean=flat_hand_mean,
         ncomps=num_pca_comps,
         side=hand_side,
         mano_root=os.path.join(FDEV_HF_CACHE_ROOT, "smplx", "mano"),
```

### Comparing `fastdev-0.0.3/src/fastdev/transforms/__init__.py` & `fastdev-0.0.4/src/fastdev/transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.3/src/fastdev/transforms/rotation.py` & `fastdev-0.0.4/src/fastdev/transforms/rotation.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.3/src/fastdev/transforms/transforms.py` & `fastdev-0.0.4/src/fastdev/transforms/transforms.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,54 @@
-from typing import Optional, Tuple, Union, overload
+from typing import Literal, Optional, Tuple, Union, overload
 
+import numpy as np
 import torch
+from numpy import ndarray
+from torch import Tensor
 
+from fastdev.utils.dispatch import typedispatch
 
-def transform(pts: torch.Tensor, tf_mat: torch.Tensor) -> torch.Tensor:
+
+@overload
+@typedispatch()
+def transform(pts: Tensor, tf_mat: Tensor) -> Tensor:
+    if pts.ndim != tf_mat.ndim:
+        raise ValueError("The dimension number of pts and tf_mat should be the same.")
+    homo_pts = to_homo(pts)
+    # `homo_pts @ tf_mat.T` or `(tf_mat @ homo_pts.T).T`
+    new_pts = torch.matmul(homo_pts, torch.transpose(tf_mat, -2, -1))
+    return new_pts[..., :3]
+
+
+@overload
+@typedispatch()
+def transform(pts: ndarray, tf_mat: ndarray) -> ndarray:
+    if pts.ndim != tf_mat.ndim:
+        raise ValueError("The dimension number of pts and tf_mat should be the same.")
+
+    homo_pts = to_homo(pts)
+    new_pts = np.matmul(homo_pts, np.swapaxes(tf_mat, -2, -1))
+    return new_pts[..., :3]
+
+
+@typedispatch(is_impl=False)
+def transform(pts: Union[Tensor, ndarray], tf_mat: Union[Tensor, ndarray]) -> Union[Tensor, ndarray]:  # type: ignore
     """
     Apply a transformation matrix on a set of 3D points.
 
     Args:
         pts: 3D points, could be [..., N, 3]
         tf_mat: Transformation matrix, could be [..., 4, 4]
 
         The dimension number of pts and tf_mat should be the same.
 
     Returns:
         Transformed pts.
     """
-    if pts.ndim != tf_mat.ndim:
-        raise ValueError("The dimension number of pts and tf_mat should be the same.")
-
-    homo_pts = to_homo(pts)
-    # `homo_pts @ tf_mat.T` or `(tf_mat @ homo_pts.T).T`
-    new_pts = torch.matmul(homo_pts, torch.transpose(tf_mat, -2, -1))
-    return new_pts[..., :3]
+    ...
 
 
 def rotate(pts: torch.Tensor, rot_mat: torch.Tensor) -> torch.Tensor:
     """
     Apply a rotation matrix on a set of 3D points.
 
     Args:
@@ -45,20 +67,20 @@
 
     # `pts @ rot_mat.T` or `(rot_mat @ pts.T).T`
     new_pts = torch.matmul(pts, torch.transpose(rot_mat, -2, -1))
     return new_pts
 
 
 @overload
-def project(pts: torch.Tensor, intr_mat: torch.Tensor, return_depth: bool = False) -> torch.Tensor: ...
+def project(pts: torch.Tensor, intr_mat: torch.Tensor, return_depth: Literal[False]) -> torch.Tensor: ...
 
 
 @overload
 def project(
-    pts: torch.Tensor, intr_mat: torch.Tensor, return_depth: bool = True
+    pts: torch.Tensor, intr_mat: torch.Tensor, return_depth: Literal[True]
 ) -> Tuple[torch.Tensor, torch.Tensor]: ...
 
 
 def project(
     pts: torch.Tensor, intr_mat: torch.Tensor, return_depth: bool = False
 ) -> Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]:
     """
@@ -133,24 +155,37 @@
     tf_mat = torch.eye(4, device=rot_mat.device, dtype=rot_mat.dtype).repeat(rot_mat.shape[:-2] + (1, 1))
     tf_mat[..., :3, :3] = rot_mat
     if tl is not None:
         tf_mat[..., :3, 3] = tl
     return tf_mat
 
 
-def to_homo(pts_3d: torch.Tensor) -> torch.Tensor:
+@overload
+@typedispatch()
+def to_homo(pts_3d: Tensor) -> Tensor:
+    return torch.cat([pts_3d, torch.ones_like(pts_3d[..., :1])], dim=-1)
+
+
+@overload
+@typedispatch()
+def to_homo(pts_3d: ndarray) -> ndarray:
+    return np.concatenate([pts_3d, np.ones_like(pts_3d[..., :1])], axis=-1)
+
+
+@typedispatch(is_impl=False)
+def to_homo(pts_3d: Union[Tensor, ndarray]) -> Union[Tensor, ndarray]:  # type: ignore
     """
     Convert Cartesian 3D points to Homogeneous 4D points.
 
     Args:
       pts_3d: 3D points in Cartesian coord, could be ...x3.
     Returns:
       ...x4 points in the Homogeneous coord.
     """
-    return torch.cat([pts_3d, torch.ones_like(pts_3d[..., :1])], dim=-1)
+    ...
 
 
 def expand_tf_mat(tf_mat: torch.Tensor) -> torch.Tensor:
     """
     Expand transformation matrix to [..., 4, 4].
 
     Args:
```

### Comparing `fastdev-0.0.3/src/fastdev/transforms/utils.py` & `fastdev-0.0.4/src/fastdev/transforms/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,22 @@
                 dirs = [dirs[axis] for axis in ["x", "y", "z"]]
                 coords[idx] = dirs  # type: ignore
             else:
                 coords[idx] = [x.strip() for x in coord.split(",")]  # type: ignore
 
         src_coord, dst_coord = coords
 
-        opp_dirs = {"left": "right", "right": "left", "up": "down", "down": "up", "front": "back", "back": "front"}
+        opp_dirs = {
+            "left": "right",
+            "right": "left",
+            "up": "down",
+            "down": "up",
+            "front": "back",
+            "back": "front",
+        }
         src_axes = [
             ["x", "y", "z"][src_coord.index(dir)]
             if dir in src_coord
             else "-" + ["x", "y", "z"][src_coord.index(opp_dirs[dir])]
             for dir in dst_coord
         ]
     else:
```

### Comparing `fastdev-0.0.3/src/fastdev/utils/geometry.py` & `fastdev-0.0.4/src/fastdev/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `fastdev-0.0.3/src/fastdev/utils/timer.py` & `fastdev-0.0.4/src/fastdev/utils/timer.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 class Timer(ContextDecorator):
     def __init__(self, start: bool = True, print_tmpl: Optional[str] = None):
         self.print_tmpl = print_tmpl if print_tmpl is not None else "{:.4f}"
 
         self._is_paused: bool = False
         self._total_paused: float = 0.0
+        self._last: float
 
         if start:
             self.start()
 
     def __enter__(self):
         self.start()
         return self
```

### Comparing `fastdev-0.0.3/src/fastdev/visualization/image.py` & `fastdev-0.0.4/src/fastdev/visualization/image.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,39 +10,52 @@
     "yellow": (255, 255, 0),
     "white": (255, 255, 255),
     "black": (0, 0, 0),
 }
 
 
 def draw_points(
-    img: np.ndarray, pts: np.ndarray, colors: Optional[np.ndarray] = None, radius=1, order="uv"
+    img: np.ndarray,
+    pts: np.ndarray,
+    colors: Optional[np.ndarray] = None,
+    radius=1,
+    order="uv",
 ) -> np.ndarray:
     """
     Args:
         img (ndarray): original image
         pts (ndarray): points in xy order, shaped (n x 2) or (2)
         colors (ndarray): color, shaped (n x 3) or (3)
         radius (int): radius of points
         order (str): order of points, "uv" or "xy", default "uv" (since most keypoints dataset use uv order)
     """
     assert order in ["xy", "uv"], "order should be xy or uv"
     if colors is None:
-        colors = COMMON_COLOR["red"]
+        colors = np.asarray(COMMON_COLOR["red"])
     pts, colors = np.asarray(pts), np.asarray(colors)
 
     assert (pts.ndim == 1 or pts.ndim == 2) and pts.shape[-1] == 2, f"wrong pts shape: {pts.shape}"
-    assert (colors.ndim == 1 or colors.ndim == 2) and colors.shape[-1] in [3, 4], f"wrong colors shape: {colors.shape}"
+    assert (colors.ndim == 1 or colors.ndim == 2) and colors.shape[-1] in [
+        3,
+        4,
+    ], f"wrong colors shape: {colors.shape}"
 
     if pts.ndim == 1:
         pts = pts[None, :]
     if colors.ndim == 2:
         assert colors.shape[0] == pts.shape[0], "colors and pts should in the same number"
     if order == "xy":
         pts = pts[:, ::-1]
 
     vis_img = img.copy()  # avoid modifying the original image
     pts = pts.astype(int)  # round to int
     for i in range(pts.shape[0]):
         # opencv use the uv order
         color = colors if colors.ndim == 1 else colors[i]
-        cv2.circle(vis_img, center=tuple(pts[i].tolist()), color=tuple(color.tolist()), radius=radius, thickness=-1)
+        cv2.circle(
+            vis_img,
+            center=tuple(pts[i].tolist()),
+            color=tuple(color.tolist()),
+            radius=radius,
+            thickness=-1,
+        )
     return vis_img
```

### Comparing `fastdev-0.0.3/src/fastdev.egg-info/PKG-INFO` & `fastdev-0.0.4/src/fastdev.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 Metadata-Version: 2.1
 Name: fastdev
-Version: 0.0.3
+Version: 0.0.4
 Summary: Type less, code more
 Author-email: Jianglong Ye <jianglong.yeh@gmail.com>
 License: MIT
 Project-URL: Repository, https://github.com/jianglongye/fastdev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Requires-Dist: fastcore
 Requires-Dist: msgspec[toml,yaml]
 Requires-Dist: rich
 Requires-Dist: fsspec
 Requires-Dist: universal_pathlib
 Requires-Dist: huggingface_hub[cli,hf_transfer]
 Requires-Dist: GitPython
 Provides-Extra: dev
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: ipython; extra == "dev"
 Requires-Dist: ruff; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
-Requires-Dist: lovely-tensors; extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: types-PyYAML; extra == "dev"
 
 # FastDev
 
 Type Less, Code More
+
+## Features
```

### Comparing `fastdev-0.0.3/src/fastdev.egg-info/SOURCES.txt` & `fastdev-0.0.4/src/fastdev.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 README.md
 pyproject.toml
 src/fastdev/__init__.py
 src/fastdev/constants.py
+src/fastdev/py.typed
 src/fastdev.egg-info/PKG-INFO
 src/fastdev.egg-info/SOURCES.txt
 src/fastdev.egg-info/dependency_links.txt
-src/fastdev.egg-info/entry_points.txt
 src/fastdev.egg-info/requires.txt
 src/fastdev.egg-info/top_level.txt
 src/fastdev/datasets/__init__.py
 src/fastdev/datasets/dexycb.py
 src/fastdev/fileio/__init__.py
 src/fastdev/fileio/io.py
 src/fastdev/fileio/handlers/__init__.py
 src/fastdev/fileio/handlers/base_handler.py
 src/fastdev/fileio/handlers/json_handler.py
 src/fastdev/fileio/handlers/yaml_handler.py
 src/fastdev/robotics/__init__.py
-src/fastdev/robotics/kinematics.py
 src/fastdev/robotics/urdf.py
 src/fastdev/smplx/__init__.py
 src/fastdev/smplx/smplx.py
 src/fastdev/transforms/__init__.py
 src/fastdev/transforms/rotation.py
 src/fastdev/transforms/transforms.py
 src/fastdev/transforms/utils.py
-src/fastdev/transforms/numpy/__init__.py
-src/fastdev/transforms/numpy/transforms.py
 src/fastdev/utils/__init__.py
+src/fastdev/utils/dispatch.py
 src/fastdev/utils/geometry.py
 src/fastdev/utils/timer.py
 src/fastdev/visualization/__init__.py
 src/fastdev/visualization/image.py
-tests/test_fileio.py
+tests/test_fileio.py
+tests/test_transforms.py
```

### Comparing `fastdev-0.0.3/tests/test_fileio.py` & `fastdev-0.0.4/tests/test_fileio.py`

 * *Files identical despite different names*

