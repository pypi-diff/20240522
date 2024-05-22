# Comparing `tmp/qsharp-1.5.0-cp37-abi3-win_arm64.whl.zip` & `tmp/qsharp-1.5.1.dev0-cp37-abi3-win_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 1650955 bytes, number of entries: 14
--rw-r--r--  4.6 unx     2093 b- defN 24-May-16 19:08 qsharp-1.5.0.dist-info/METADATA
--rw-r--r--  4.6 unx       94 b- defN 24-May-16 19:08 qsharp-1.5.0.dist-info/WHEEL
--rw-r--r--  4.6 unx     3090 b- defN 24-May-16 19:08 qsharp/.data/qsharp_codemirror.js
--rw-r--r--  4.6 unx    38836 b- defN 24-May-16 19:08 qsharp/estimator/_estimator.py
--rw-r--r--  4.6 unx      859 b- defN 24-May-16 19:08 qsharp/estimator/__init__.py
--rw-r--r--  4.6 unx     1706 b- defN 24-May-16 19:08 qsharp/utils/_utils.py
--rw-r--r--  4.6 unx      146 b- defN 24-May-16 19:08 qsharp/utils/__init__.py
--rw-r--r--  4.6 unx      864 b- defN 24-May-16 19:08 qsharp/_fs.py
--rw-r--r--  4.6 unx     1848 b- defN 24-May-16 19:08 qsharp/_ipython.py
--rw-r--r--  4.6 unx     6534 b- defN 24-May-16 19:08 qsharp/_native.pyi
--rw-r--r--  4.6 unx    12906 b- defN 24-May-16 19:08 qsharp/_qsharp.py
--rw-r--r--  4.6 unx      902 b- defN 24-May-16 19:08 qsharp/__init__.py
--rwxr-xr-x  4.6 unx  4009472 b- defN 24-May-16 19:08 qsharp/_native.pyd
--rw-r--r--  4.6 unx     1070 b- defN 24-May-16 19:08 qsharp-1.5.0.dist-info/RECORD
-14 files, 4080420 bytes uncompressed, 1649215 bytes compressed:  59.6%
+Zip file size: 1675564 bytes, number of entries: 14
+-rw-r--r--  4.6 unx     2098 b- defN 24-May-22 04:08 qsharp-1.5.1.dev0.dist-info/METADATA
+-rw-r--r--  4.6 unx       94 b- defN 24-May-22 04:08 qsharp-1.5.1.dev0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     3090 b- defN 24-May-22 04:08 qsharp/.data/qsharp_codemirror.js
+-rw-r--r--  4.6 unx    38836 b- defN 24-May-22 04:08 qsharp/estimator/_estimator.py
+-rw-r--r--  4.6 unx      859 b- defN 24-May-22 04:08 qsharp/estimator/__init__.py
+-rw-r--r--  4.6 unx     1706 b- defN 24-May-22 04:08 qsharp/utils/_utils.py
+-rw-r--r--  4.6 unx      146 b- defN 24-May-22 04:08 qsharp/utils/__init__.py
+-rw-r--r--  4.6 unx      864 b- defN 24-May-22 04:08 qsharp/_fs.py
+-rw-r--r--  4.6 unx     1848 b- defN 24-May-22 04:08 qsharp/_ipython.py
+-rw-r--r--  4.6 unx     6534 b- defN 24-May-22 04:08 qsharp/_native.pyi
+-rw-r--r--  4.6 unx    13377 b- defN 24-May-22 04:08 qsharp/_qsharp.py
+-rw-r--r--  4.6 unx      902 b- defN 24-May-22 04:08 qsharp/__init__.py
+-rwxr-xr-x  4.6 unx  4053504 b- defN 24-May-22 04:08 qsharp/_native.pyd
+-rw-r--r--  4.6 unx     1085 b- defN 24-May-22 04:08 qsharp-1.5.1.dev0.dist-info/RECORD
+14 files, 4124943 bytes uncompressed, 1673794 bytes compressed:  59.4%
```

## zipnote {}

```diff
@@ -1,11 +1,11 @@
-Filename: qsharp-1.5.0.dist-info/METADATA
+Filename: qsharp-1.5.1.dev0.dist-info/METADATA
 Comment: 
 
-Filename: qsharp-1.5.0.dist-info/WHEEL
+Filename: qsharp-1.5.1.dev0.dist-info/WHEEL
 Comment: 
 
 Filename: qsharp/.data/qsharp_codemirror.js
 Comment: 
 
 Filename: qsharp/estimator/_estimator.py
 Comment: 
@@ -33,11 +33,11 @@
 
 Filename: qsharp/__init__.py
 Comment: 
 
 Filename: qsharp/_native.pyd
 Comment: 
 
-Filename: qsharp-1.5.0.dist-info/RECORD
+Filename: qsharp-1.5.1.dev0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qsharp/_qsharp.py

```diff
@@ -27,16 +27,14 @@
         self,
         target_profile: TargetProfile,
         language_features: Optional[List[str]],
         manifest: Optional[str],
     ):
         if target_profile == TargetProfile.Adaptive_RI:
             self._config = {"targetProfile": "adaptive_ri"}
-            warn("The Adaptive_RI target profile is a preview feature.")
-            warn("Functionality may be incomplete or incorrect.")
         elif target_profile == TargetProfile.Base:
             self._config = {"targetProfile": "base"}
         elif target_profile == TargetProfile.Unrestricted:
             self._config = {"targetProfile": "unrestricted"}
 
         self._config["languageFeatures"] = language_features
         self._config["manifest"] = manifest
@@ -56,31 +54,46 @@
     ) -> Dict[str, Dict[str, str]]:
         return {"application/x.qsharp-config": self._config}
 
 
 def init(
     *,
     target_profile: TargetProfile = TargetProfile.Unrestricted,
+    target_name: Optional[str] = None,
     project_root: Optional[str] = None,
     language_features: Optional[List[str]] = None,
 ) -> Config:
     """
     Initializes the Q# interpreter.
 
     :param target_profile: Setting the target profile allows the Q#
         interpreter to generate programs that are compatible
         with a specific target. See :py:class: `qsharp.TargetProfile`.
 
+    :param target_name: An optional name of the target machine to use for inferring the compatible
+        target_profile setting.
+
     :param project_root: An optional path to a root directory with a Q# project to include.
         It must contain a qsharp.json project manifest.
     """
     from ._fs import read_file, list_directory, exists, join
 
     global _interpreter
 
+    if isinstance(target_name, str):
+        target = target_name.split(".")[0].lower()
+        if target == "ionq" or target == "rigetti":
+            target_profile = TargetProfile.Base
+        elif target == "quantinuum":
+            target_profile = TargetProfile.Adaptive_RI
+        else:
+            raise QSharpError(
+                f'target_name "{target_name}" not recognized. Please set target_profile directly.'
+            )
+
     manifest_contents = None
     manifest_descriptor = None
     if project_root is not None:
         qsharp_json = join(project_root, "qsharp.json")
         if not exists(qsharp_json):
             raise QSharpError(
                 f"{qsharp_json} not found. qsharp.json should exist at the project root and be a valid JSON file."
```

## Comparing `qsharp-1.5.0.dist-info/METADATA` & `qsharp-1.5.1.dev0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qsharp
-Version: 1.5.0
+Version: 1.5.1.dev0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

