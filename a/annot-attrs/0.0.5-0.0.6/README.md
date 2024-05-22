# Comparing `tmp/annot_attrs-0.0.5.tar.gz` & `tmp/annot_attrs-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annot_attrs-0.0.5.tar", last modified: Wed Mar 27 07:58:08 2024, max compression
+gzip compressed data, was "annot_attrs-0.0.6.tar", last modified: Wed May 22 07:21:57 2024, max compression
```

## Comparing `annot_attrs-0.0.5.tar` & `annot_attrs-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 07:58:08.505166 annot_attrs-0.0.5/
--rw-rw-rw-   0        0        0     1082 2024-03-27 07:25:26.000000 annot_attrs-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     3772 2024-03-27 07:58:08.504167 annot_attrs-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2879 2024-03-27 07:54:57.000000 annot_attrs-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-03-27 07:58:08.500167 annot_attrs-0.0.5/annot_attrs/
--rw-rw-rw-   0        0        0       21 2024-03-27 07:25:26.000000 annot_attrs-0.0.5/annot_attrs/__init__.py
--rw-rw-rw-   0        0        0     4347 2024-03-27 07:44:29.000000 annot_attrs-0.0.5/annot_attrs/main.py
-drwxrwxrwx   0        0        0        0 2024-03-27 07:58:08.504167 annot_attrs-0.0.5/annot_attrs.egg-info/
--rw-rw-rw-   0        0        0     3772 2024-03-27 07:58:08.000000 annot_attrs-0.0.5/annot_attrs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2024-03-27 07:58:08.000000 annot_attrs-0.0.5/annot_attrs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 07:58:08.000000 annot_attrs-0.0.5/annot_attrs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-03-27 07:58:08.000000 annot_attrs-0.0.5/annot_attrs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-27 07:58:08.505166 annot_attrs-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     2184 2024-03-27 07:54:43.000000 annot_attrs-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:21:57.328238 annot_attrs-0.0.6/
+-rw-rw-rw-   0        0        0     1082 2024-03-27 07:25:26.000000 annot_attrs-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     3772 2024-05-22 07:21:57.327737 annot_attrs-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2879 2024-05-22 07:21:07.000000 annot_attrs-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 07:21:57.320761 annot_attrs-0.0.6/annot_attrs/
+-rw-rw-rw-   0        0        0       62 2024-05-22 07:07:35.000000 annot_attrs-0.0.6/annot_attrs/__init__.py
+-rw-rw-rw-   0        0        0     5626 2024-05-22 07:20:33.000000 annot_attrs-0.0.6/annot_attrs/main.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:21:57.326672 annot_attrs-0.0.6/annot_attrs.egg-info/
+-rw-rw-rw-   0        0        0     3772 2024-05-22 07:21:57.000000 annot_attrs-0.0.6/annot_attrs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2024-05-22 07:21:57.000000 annot_attrs-0.0.6/annot_attrs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 07:21:57.000000 annot_attrs-0.0.6/annot_attrs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-22 07:21:57.000000 annot_attrs-0.0.6/annot_attrs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 07:21:57.329481 annot_attrs-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     2184 2024-03-27 07:54:43.000000 annot_attrs-0.0.6/setup.py
```

### Comparing `annot_attrs-0.0.5/LICENSE` & `annot_attrs-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `annot_attrs-0.0.5/PKG-INFO` & `annot_attrs-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annot_attrs
-Version: 0.0.5
+Version: 0.0.6
 Summary: work with annotated but not defined/not used attrs in class
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/annot_attrs
 Keywords: annotations,annots,not defined attributes,attributes
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# annot_attrs (v0.0.5)
+# annot_attrs (v0.0.6)
 
 ## DESCRIPTION_SHORT
 work with annotated but not defined/not used attrs in class
 
 ## DESCRIPTION_LONG
 Designed to get list of annotated but not defined/not used attrs from class (not instance!).  
     may be helpful further in instance to check that really have values.
```

### Comparing `annot_attrs-0.0.5/README.md` & `annot_attrs-0.0.6/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# annot_attrs (v0.0.5)
+# annot_attrs (v0.0.6)
 
 ## DESCRIPTION_SHORT
 work with annotated but not defined/not used attrs in class
 
 ## DESCRIPTION_LONG
 Designed to get list of annotated but not defined/not used attrs from class (not instance!).  
     may be helpful further in instance to check that really have values.
```

### Comparing `annot_attrs-0.0.5/annot_attrs.egg-info/PKG-INFO` & `annot_attrs-0.0.6/annot_attrs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annot_attrs
-Version: 0.0.5
+Version: 0.0.6
 Summary: work with annotated but not defined/not used attrs in class
 Home-page: https://github.com/centroid457/
 Author: Andrei Starichenko
 Author-email: centroid@mail.ru
 Project-URL: Source, https://github.com/centroid457/annot_attrs
 Keywords: annotations,annots,not defined attributes,attributes
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -16,15 +16,15 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Typing :: Typed
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# annot_attrs (v0.0.5)
+# annot_attrs (v0.0.6)
 
 ## DESCRIPTION_SHORT
 work with annotated but not defined/not used attrs in class
 
 ## DESCRIPTION_LONG
 Designed to get list of annotated but not defined/not used attrs from class (not instance!).  
     may be helpful further in instance to check that really have values.
```

### Comparing `annot_attrs-0.0.5/setup.py` & `annot_attrs-0.0.6/setup.py`

 * *Files identical despite different names*

