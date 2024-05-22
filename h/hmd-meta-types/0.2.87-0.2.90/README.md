# Comparing `tmp/hmd_meta_types-0.2.87-py3-none-any.whl.zip` & `tmp/hmd_meta_types-0.2.90-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 8011 bytes, number of entries: 12
--rw-r--r--  2.0 unx       47 b- defN 22-Sep-12 13:31 hmd_meta_types/__init__.py
--rw-r--r--  2.0 unx    10491 b- defN 22-Sep-12 13:31 hmd_meta_types/entity.py
--rw-r--r--  2.0 unx      280 b- defN 22-Sep-12 13:31 hmd_meta_types/utils.py
--rw-r--r--  2.0 unx        0 b- defN 22-Sep-12 13:31 test/__init__.py
--rw-r--r--  2.0 unx     4007 b- defN 22-Sep-12 13:31 test/conftest.py
--rw-r--r--  2.0 unx     7521 b- defN 22-Sep-12 13:31 test/test_noun.py
--rw-r--r--  2.0 unx     3533 b- defN 22-Sep-12 13:31 test/test_relationship.py
--rw-r--r--  2.0 unx      323 b- defN 22-Sep-12 13:31 test/test_utils.py
--rw-r--r--  2.0 unx      463 b- defN 22-Sep-12 13:31 hmd_meta_types-0.2.87.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-Sep-12 13:31 hmd_meta_types-0.2.87.dist-info/WHEEL
--rw-r--r--  2.0 unx       20 b- defN 22-Sep-12 13:31 hmd_meta_types-0.2.87.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      944 b- defN 22-Sep-12 13:31 hmd_meta_types-0.2.87.dist-info/RECORD
-12 files, 27721 bytes uncompressed, 6427 bytes compressed:  76.8%
+Zip file size: 8027 bytes, number of entries: 12
+-rw-rw-rw-  2.0 unx       47 b- defN 24-Apr-01 19:21 hmd_meta_types/__init__.py
+-rw-rw-rw-  2.0 unx    10559 b- defN 24-Apr-01 19:21 hmd_meta_types/entity.py
+-rw-rw-rw-  2.0 unx      280 b- defN 24-Apr-01 19:21 hmd_meta_types/utils.py
+-rw-rw-rw-  2.0 unx        0 b- defN 24-Apr-01 19:21 test/__init__.py
+-rw-rw-rw-  2.0 unx     4007 b- defN 24-Apr-01 19:21 test/conftest.py
+-rw-rw-rw-  2.0 unx     7521 b- defN 24-Apr-01 19:21 test/test_noun.py
+-rw-rw-rw-  2.0 unx     3533 b- defN 24-Apr-01 19:21 test/test_relationship.py
+-rw-rw-rw-  2.0 unx      323 b- defN 24-Apr-01 19:21 test/test_utils.py
+-rw-rw-rw-  2.0 unx      463 b- defN 24-Apr-01 19:22 hmd_meta_types-0.2.90.dist-info/METADATA
+-rw-rw-rw-  2.0 unx       92 b- defN 24-Apr-01 19:22 hmd_meta_types-0.2.90.dist-info/WHEEL
+-rw-rw-rw-  2.0 unx       20 b- defN 24-Apr-01 19:22 hmd_meta_types-0.2.90.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      944 b- defN 24-Apr-01 19:22 hmd_meta_types-0.2.90.dist-info/RECORD
+12 files, 27789 bytes uncompressed, 6443 bytes compressed:  76.8%
```

## zipnote {}

```diff
@@ -18,20 +18,20 @@
 
 Filename: test/test_relationship.py
 Comment: 
 
 Filename: test/test_utils.py
 Comment: 
 
-Filename: hmd_meta_types-0.2.87.dist-info/METADATA
+Filename: hmd_meta_types-0.2.90.dist-info/METADATA
 Comment: 
 
-Filename: hmd_meta_types-0.2.87.dist-info/WHEEL
+Filename: hmd_meta_types-0.2.90.dist-info/WHEEL
 Comment: 
 
-Filename: hmd_meta_types-0.2.87.dist-info/top_level.txt
+Filename: hmd_meta_types-0.2.90.dist-info/top_level.txt
 Comment: 
 
-Filename: hmd_meta_types-0.2.87.dist-info/RECORD
+Filename: hmd_meta_types-0.2.90.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hmd_meta_types/entity.py

```diff
@@ -175,21 +175,21 @@
                         value = b64encode(
                             dumps(value).encode(encoding="latin-1")
                         ).decode("latin-1")
                 elif definition["type"] == "blob":
                     value = b64encode(value).decode("latin-1")
                 result[attr] = value
 
-        if hasattr(self, "ref_to"):
+        if hasattr(self, "ref_to") and hasattr(self, "ref_to_type"):
             if isinstance(self.ref_to, self.ref_to_type()):
                 result["ref_to"] = self.ref_to.identifier
             else:
                 result["ref_to"] = self.ref_to
 
-        if hasattr(self, "ref_from"):
+        if hasattr(self, "ref_from") and hasattr(self, "ref_from_type"):
             if isinstance(self.ref_from, self.ref_from_type()):
                 result["ref_from"] = self.ref_from.identifier
             else:
                 result["ref_from"] = self.ref_from
 
         if include_schema:
             result["__schema"] = self.get_namespace_name()
```

