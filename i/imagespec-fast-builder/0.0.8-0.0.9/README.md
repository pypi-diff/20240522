# Comparing `tmp/imagespec_fast_builder-0.0.8.tar.gz` & `tmp/imagespec_fast_builder-0.0.9.tar.gz`

## Comparing `imagespec_fast_builder-0.0.8.tar` & `imagespec_fast_builder-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/.github/workflows/wheel.yaml
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/dockerfiles/Dockerfile
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/dockerfiles/Dockerfile.base
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/experiments/build_wf.py
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/experiments/check_builder.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/src/imagespec_fast_builder/__init__.py
--rw-r--r--   0        0        0     6337 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/src/imagespec_fast_builder/_image_builder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/tests/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/LICENSE
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/README.md
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.9/.github/workflows/wheel.yaml
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.9/dockerfiles/Dockerfile
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.9/dockerfiles/Dockerfile.base
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.9/experiments/build_wf.py
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.9/experiments/check_builder.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.9/src/imagespec_fast_builder/__init__.py
+-rw-r--r--   0        0        0     6580 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.9/src/imagespec_fast_builder/_image_builder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.9/tests/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.9/README.md
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 imagespec_fast_builder-0.0.9/PKG-INFO
```

### Comparing `imagespec_fast_builder-0.0.8/.github/workflows/wheel.yaml` & `imagespec_fast_builder-0.0.9/.github/workflows/wheel.yaml`

 * *Files identical despite different names*

### Comparing `imagespec_fast_builder-0.0.8/dockerfiles/Dockerfile` & `imagespec_fast_builder-0.0.9/dockerfiles/Dockerfile`

 * *Files identical despite different names*

### Comparing `imagespec_fast_builder-0.0.8/src/imagespec_fast_builder/_image_builder.py` & `imagespec_fast_builder-0.0.9/src/imagespec_fast_builder/_image_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -185,14 +185,19 @@
         "base_image",
         "pip_index",
         # "registry_config",
         "commands",
     }
 
     def build_image(self, image_spec: ImageSpec) -> str:
+        return self._build_image(image_spec)
+
+    def _build_image(self, image_spec: ImageSpec, *, push: bool = True) -> str:
+        # For testing, set `push=False`` to just build the image locally and not push to
+        # registry
         unsupported_parameters = [
             name
             for name, value in vars(image_spec).items()
             if value is not None
             and name not in self._SUPPORTED_IMAGE_SPEC_PARAMETERS
             and not name.startswith("_")
         ]
@@ -213,15 +218,15 @@
                 "build",
                 "--tag",
                 f"{image_spec.image_name()}",
                 "--platform",
                 image_spec.platform,
             ]
 
-            if image_spec.registry:
+            if image_spec.registry and push:
                 command.append("--push")
             command.append(tmp_dir)
 
             concat_command = " ".join(command)
             click.secho(f"Run command: {concat_command} ", fg="blue")
             subprocess.run(command, check=True)
```

### Comparing `imagespec_fast_builder-0.0.8/.gitignore` & `imagespec_fast_builder-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `imagespec_fast_builder-0.0.8/LICENSE` & `imagespec_fast_builder-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `imagespec_fast_builder-0.0.8/README.md` & `imagespec_fast_builder-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `imagespec_fast_builder-0.0.8/pyproject.toml` & `imagespec_fast_builder-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `imagespec_fast_builder-0.0.8/PKG-INFO` & `imagespec_fast_builder-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: imagespec-fast-builder
-Version: 0.0.8
+Version: 0.0.9
 Summary: A faster ImageSpec builder for flytekit
 Project-URL: Issues, https://github.com/thomasjpfan/imagespec-fast-builder/issues
 Project-URL: Source, https://github.com/thomasjpfan/imagespec-fast-builder
 Author-email: "Thomas J. Fan" <thomasjpfan@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
```

