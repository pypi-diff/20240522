# Comparing `tmp/imerit_ango-1.3.8-py3-none-any.whl.zip` & `tmp/imerit_ango-1.3.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 12906 bytes, number of entries: 13
+Zip file size: 12897 bytes, number of entries: 13
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-22 07:35 imerit_ango/__init__.py
 -rw-r--r--  2.0 unx     1609 b- defN 24-Jan-22 07:35 imerit_ango/plugin_logger.py
--rw-r--r--  2.0 unx     9912 b- defN 24-Feb-02 12:47 imerit_ango/plugins.py
+-rw-r--r--  2.0 unx     9915 b- defN 24-Feb-02 12:48 imerit_ango/plugins.py
 -rw-r--r--  2.0 unx    18106 b- defN 24-Feb-02 12:47 imerit_ango/sdk.py
 -rw-r--r--  2.0 unx     2461 b- defN 24-Jan-29 06:43 imerit_ango/test-integration.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Jan-22 07:35 imerit_ango/models/__init__.py
 -rw-r--r--  2.0 unx      467 b- defN 24-Jan-24 18:30 imerit_ango/models/enums.py
 -rw-r--r--  2.0 unx      916 b- defN 24-Jan-24 18:32 imerit_ango/models/invite.py
 -rw-r--r--  2.0 unx     5441 b- defN 24-Jan-22 07:35 imerit_ango/models/label_category.py
--rw-r--r--  2.0 unx     1094 b- defN 24-Feb-02 12:47 imerit_ango-1.3.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-02 12:47 imerit_ango-1.3.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 24-Feb-02 12:47 imerit_ango-1.3.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1063 b- defN 24-Feb-02 12:47 imerit_ango-1.3.8.dist-info/RECORD
-13 files, 41173 bytes uncompressed, 11122 bytes compressed:  73.0%
+-rw-r--r--  2.0 unx     1094 b- defN 24-Feb-02 12:48 imerit_ango-1.3.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Feb-02 12:48 imerit_ango-1.3.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 24-Feb-02 12:48 imerit_ango-1.3.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1063 b- defN 24-Feb-02 12:48 imerit_ango-1.3.9.dist-info/RECORD
+13 files, 41176 bytes uncompressed, 11113 bytes compressed:  73.0%
```

## zipnote {}

```diff
@@ -21,20 +21,20 @@
 
 Filename: imerit_ango/models/invite.py
 Comment: 
 
 Filename: imerit_ango/models/label_category.py
 Comment: 
 
-Filename: imerit_ango-1.3.8.dist-info/METADATA
+Filename: imerit_ango-1.3.9.dist-info/METADATA
 Comment: 
 
-Filename: imerit_ango-1.3.8.dist-info/WHEEL
+Filename: imerit_ango-1.3.9.dist-info/WHEEL
 Comment: 
 
-Filename: imerit_ango-1.3.8.dist-info/top_level.txt
+Filename: imerit_ango-1.3.9.dist-info/top_level.txt
 Comment: 
 
-Filename: imerit_ango-1.3.8.dist-info/RECORD
+Filename: imerit_ango-1.3.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## imerit_ango/plugins.py

```diff
@@ -129,15 +129,15 @@
         completed_at = None
         updated_at = None
         project_id = data.get('projectId')
         logger = super()._get_logger(data)
         api_key = data.get('apiKey')
         config_str = data.get('configJSON', "{}")
         config = json.loads(config_str)
-        include_key_frames_only = config.get('includeKeyFramesOnly', None)
+        include_key_frames_only = config.get('include_key_frames_only', None)
         sdk = SDK(api_key=api_key, host=self.host)
 
         if data.get("completed_at", None):
             completed_at = [datetime.datetime.fromisoformat(data.completed_at[0]),
                             datetime.datetime.fromisoformat(data.completed_at[1])]
         if data.get("updated_at", None):
             updated_at = [datetime.datetime.fromisoformat(data.updated_at[0]),
```

## Comparing `imerit_ango-1.3.8.dist-info/METADATA` & `imerit_ango-1.3.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imerit-ango
-Version: 1.3.8
+Version: 1.3.9
 Summary: Ango-Hub SDK
 Author: Faruk Karakaya
 Author-email: <faruk@ango.ai>
 License: UNKNOWN
 Keywords: imerit_ango,ango-hub,imerit_ango sdk,Ango,Ango-hub
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

## Comparing `imerit_ango-1.3.8.dist-info/RECORD` & `imerit_ango-1.3.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 imerit_ango/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 imerit_ango/plugin_logger.py,sha256=Zqp5Uunv_i9QigXW1Zom7Yz70k_xLX8zEINRBfWr9JE,1609
-imerit_ango/plugins.py,sha256=_SZx0XrGAE2YIPsfCKJEqnUpwXLiVvPnaxxiPXAXkUI,9912
+imerit_ango/plugins.py,sha256=bHq0pFGjy_XINgGGq6MFEfJU7lu3X_hkl5yQz06g1bA,9915
 imerit_ango/sdk.py,sha256=h8BUlJucHO1v6Smaa8w_DUrjon2uH3XkACF0p_2Pbt8,18106
 imerit_ango/test-integration.py,sha256=WSgoQlX5PH0e-xSFLO8B0FPwiDoF__8pQRXfrHhvetU,2461
 imerit_ango/models/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 imerit_ango/models/enums.py,sha256=EY9i270uvlzusvGmZJAu6fN8wm2IPsH16v1Qjm7FmxY,467
 imerit_ango/models/invite.py,sha256=zMPbkYzjdeW7-CC-UKt3jifAN53aKB-_nkR-IkrtQOc,916
 imerit_ango/models/label_category.py,sha256=MyokP-gGck8PvKyJjbUgx8vF_CieqgXmmmBWwQRTj3M,5441
-imerit_ango-1.3.8.dist-info/METADATA,sha256=qXHgNzuxRdwRsTqYpr4obJRvFrKSntslOKMeDR2lHrU,1094
-imerit_ango-1.3.8.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-imerit_ango-1.3.8.dist-info/top_level.txt,sha256=rL30Gcrxa2AgOWg8EXn6b4NzT5STPtJ20PSJPK9IgH0,12
-imerit_ango-1.3.8.dist-info/RECORD,,
+imerit_ango-1.3.9.dist-info/METADATA,sha256=O0iD6IYkXtAk0SNmekILdy5CG7N5Qr3cDlo-OSmcLbI,1094
+imerit_ango-1.3.9.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+imerit_ango-1.3.9.dist-info/top_level.txt,sha256=rL30Gcrxa2AgOWg8EXn6b4NzT5STPtJ20PSJPK9IgH0,12
+imerit_ango-1.3.9.dist-info/RECORD,,
```

