# Comparing `tmp/mbu_dev_shared_components-0.0.8.post1.tar.gz` & `tmp/mbu_dev_shared_components-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbu_dev_shared_components-0.0.8.post1.tar", last modified: Fri May 17 17:39:34 2024, max compression
+gzip compressed data, was "mbu_dev_shared_components-0.0.9.tar", last modified: Fri May 17 17:48:42 2024, max compression
```

## Comparing `mbu_dev_shared_components-0.0.8.post1.tar` & `mbu_dev_shared_components-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-17 17:39:34.244841 mbu_dev_shared_components-0.0.8.post1/
--rw-rw-rw-   0        0        0     3238 2024-05-16 14:14:30.000000 mbu_dev_shared_components-0.0.8.post1/.gitignore
--rw-rw-rw-   0        0        0     1085 2024-05-16 14:14:30.000000 mbu_dev_shared_components-0.0.8.post1/LICENSE
--rw-rw-rw-   0        0        0      995 2024-05-17 17:39:34.244841 mbu_dev_shared_components-0.0.8.post1/PKG-INFO
--rw-rw-rw-   0        0        0      498 2024-05-16 15:19:15.000000 mbu_dev_shared_components-0.0.8.post1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-17 17:39:34.112638 mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components/
-drwxrwxrwx   0        0        0        0 2024-05-17 17:39:34.186815 mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components/office365/
--rw-rw-rw-   0        0        0        0 2024-05-16 14:20:13.000000 mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components/office365/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 17:39:34.193108 mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components/office365/excel/
--rw-rw-rw-   0        0        0        0 2024-05-16 20:18:44.000000 mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components/office365/excel/__init__.py
--rw-rw-rw-   0        0        0     7181 2024-05-17 13:55:50.000000 mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components/office365/excel/excel_reader.py
-drwxrwxrwx   0        0        0        0 2024-05-17 17:39:34.221321 mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components/office365/sharepoint_api/
--rw-rw-rw-   0        0        0        0 2024-05-16 14:20:46.000000 mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components/office365/sharepoint_api/__init__.py
--rw-rw-rw-   0        0        0     8970 2024-05-16 15:09:46.000000 mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components/office365/sharepoint_api/files.py
-drwxrwxrwx   0        0        0        0 2024-05-17 17:39:34.225939 mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components/os2forms_api/
--rw-rw-rw-   0        0        0        0 2024-05-16 15:12:48.000000 mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components/os2forms_api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-17 17:39:34.238416 mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components/utils/
--rw-rw-rw-   0        0        0        0 2024-05-17 14:24:58.000000 mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components/utils/__init__.py
--rw-rw-rw-   0        0        0     1976 2024-05-17 14:30:40.000000 mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components/utils/json.py
-drwxrwxrwx   0        0        0        0 2024-05-17 17:39:34.243765 mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components.egg-info/
--rw-rw-rw-   0        0        0      995 2024-05-17 17:39:33.000000 mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      705 2024-05-17 17:39:34.000000 mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-17 17:39:33.000000 mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2024-05-17 17:39:33.000000 mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-17 17:39:33.000000 mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      683 2024-05-17 17:38:50.000000 mbu_dev_shared_components-0.0.8.post1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-17 17:39:34.250592 mbu_dev_shared_components-0.0.8.post1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-17 17:48:42.956336 mbu_dev_shared_components-0.0.9/
+-rw-rw-rw-   0        0        0     3238 2024-05-16 14:14:30.000000 mbu_dev_shared_components-0.0.9/.gitignore
+-rw-rw-rw-   0        0        0     1085 2024-05-16 14:14:30.000000 mbu_dev_shared_components-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      989 2024-05-17 17:48:42.954348 mbu_dev_shared_components-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2024-05-16 15:19:15.000000 mbu_dev_shared_components-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-17 17:48:42.881364 mbu_dev_shared_components-0.0.9/mbu_dev_shared_components/
+drwxrwxrwx   0        0        0        0 2024-05-17 17:48:42.932712 mbu_dev_shared_components-0.0.9/mbu_dev_shared_components/office365/
+-rw-rw-rw-   0        0        0        0 2024-05-16 14:20:13.000000 mbu_dev_shared_components-0.0.9/mbu_dev_shared_components/office365/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 17:48:42.936237 mbu_dev_shared_components-0.0.9/mbu_dev_shared_components/office365/excel/
+-rw-rw-rw-   0        0        0        0 2024-05-16 20:18:44.000000 mbu_dev_shared_components-0.0.9/mbu_dev_shared_components/office365/excel/__init__.py
+-rw-rw-rw-   0        0        0     7181 2024-05-17 13:55:50.000000 mbu_dev_shared_components-0.0.9/mbu_dev_shared_components/office365/excel/excel_reader.py
+drwxrwxrwx   0        0        0        0 2024-05-17 17:48:42.940240 mbu_dev_shared_components-0.0.9/mbu_dev_shared_components/office365/sharepoint_api/
+-rw-rw-rw-   0        0        0        0 2024-05-16 14:20:46.000000 mbu_dev_shared_components-0.0.9/mbu_dev_shared_components/office365/sharepoint_api/__init__.py
+-rw-rw-rw-   0        0        0     8970 2024-05-16 15:09:46.000000 mbu_dev_shared_components-0.0.9/mbu_dev_shared_components/office365/sharepoint_api/files.py
+drwxrwxrwx   0        0        0        0 2024-05-17 17:48:42.943695 mbu_dev_shared_components-0.0.9/mbu_dev_shared_components/os2forms_api/
+-rw-rw-rw-   0        0        0        0 2024-05-16 15:12:48.000000 mbu_dev_shared_components-0.0.9/mbu_dev_shared_components/os2forms_api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-17 17:48:42.950194 mbu_dev_shared_components-0.0.9/mbu_dev_shared_components/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-17 14:24:58.000000 mbu_dev_shared_components-0.0.9/mbu_dev_shared_components/utils/__init__.py
+-rw-rw-rw-   0        0        0     3136 2024-05-17 17:47:19.000000 mbu_dev_shared_components-0.0.9/mbu_dev_shared_components/utils/json.py
+drwxrwxrwx   0        0        0        0 2024-05-17 17:48:42.952190 mbu_dev_shared_components-0.0.9/mbu_dev_shared_components.egg-info/
+-rw-rw-rw-   0        0        0      989 2024-05-17 17:48:42.000000 mbu_dev_shared_components-0.0.9/mbu_dev_shared_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      705 2024-05-17 17:48:42.000000 mbu_dev_shared_components-0.0.9/mbu_dev_shared_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-17 17:48:42.000000 mbu_dev_shared_components-0.0.9/mbu_dev_shared_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2024-05-17 17:48:42.000000 mbu_dev_shared_components-0.0.9/mbu_dev_shared_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-17 17:48:42.000000 mbu_dev_shared_components-0.0.9/mbu_dev_shared_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      683 2024-05-17 17:38:50.000000 mbu_dev_shared_components-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-17 17:48:42.957508 mbu_dev_shared_components-0.0.9/setup.cfg
```

### Comparing `mbu_dev_shared_components-0.0.8.post1/.gitignore` & `mbu_dev_shared_components-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `mbu_dev_shared_components-0.0.8.post1/LICENSE` & `mbu_dev_shared_components-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mbu_dev_shared_components-0.0.8.post1/PKG-INFO` & `mbu_dev_shared_components-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbu_dev_shared_components
-Version: 0.0.8.post1
+Version: 0.0.9
 Summary: Shared components to use in RPA projects
 Author-email: MBU <rpa@mbu.aarhus.dk>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components/office365/excel/excel_reader.py` & `mbu_dev_shared_components-0.0.9/mbu_dev_shared_components/office365/excel/excel_reader.py`

 * *Files identical despite different names*

### Comparing `mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components/office365/sharepoint_api/files.py` & `mbu_dev_shared_components-0.0.9/mbu_dev_shared_components/office365/sharepoint_api/files.py`

 * *Files identical despite different names*

### Comparing `mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components/utils/json.py` & `mbu_dev_shared_components-0.0.9/mbu_dev_shared_components/utils/json.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,14 +13,17 @@
     """
     A class used to manipulate JSON objects.
 
     Methods
     -------
     transform_all_lists(json_obj: Dict[str, Union[List[Any], Dict[str, Any]]], key_map: List[str]) -> Dict[str, Dict[str, Any]]:
         Transforms all lists in the JSON object into dictionaries with specified keys.
+
+    add_key_value(json_obj: Dict[str, Any], keys: List[str], value: Any) -> Dict[str, Any]:
+            Adds a new key-value pair to the JSON object, supporting nested JSON structures.
     """
 
     @staticmethod
     def transform_all_lists(json_obj: Dict[str, Union[List[Any], Dict[str, Any]]], key_map: List[str]) -> Dict[str, Dict[str, Any]]:
         """
         Transforms all lists in the JSON object into dictionaries with specified keys.
 
@@ -44,7 +47,38 @@
                 if len(value) == len(key_map):
                     json_obj[key] = {key_map[i]: value[i] for i in range(len(key_map))}
                 else:
                     raise ValueError(f"The length of the list for key '{key}' and the key_map must match.")
             else:
                 raise TypeError(f"The value for key '{key}' is not a list.")
         return json_obj
+
+    @staticmethod
+    def add_key_value(json_obj: Dict[str, Any], keys: List[str], value: Any) -> Dict[str, Any]:
+        """
+        Adds a new key-value pair to the JSON object, supporting nested JSON structures.
+
+        Parameters
+        ----------
+        json_obj : dict
+            The JSON object to be manipulated.
+        keys : list
+            The list of keys representing the path to where the value should be added.
+        value : Any
+            The value to be added.
+
+        Returns
+        -------
+        dict
+            The updated JSON object with the new key-value pair added.
+        """
+        if not isinstance(json_obj, dict):
+            raise TypeError("The input must be a dictionary.")
+
+        d = json_obj
+        for key in keys[:-1]:
+            if key not in d or not isinstance(d[key], dict):
+                d[key] = {}
+            d = d[key]
+
+        d[keys[-1]] = value
+        return json_obj
```

### Comparing `mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components.egg-info/PKG-INFO` & `mbu_dev_shared_components-0.0.9/mbu_dev_shared_components.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbu_dev_shared_components
-Version: 0.0.8.post1
+Version: 0.0.9
 Summary: Shared components to use in RPA projects
 Author-email: MBU <rpa@mbu.aarhus.dk>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mbu_dev_shared_components-0.0.8.post1/mbu_dev_shared_components.egg-info/SOURCES.txt` & `mbu_dev_shared_components-0.0.9/mbu_dev_shared_components.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mbu_dev_shared_components-0.0.8.post1/pyproject.toml` & `mbu_dev_shared_components-0.0.9/pyproject.toml`

 * *Files identical despite different names*

