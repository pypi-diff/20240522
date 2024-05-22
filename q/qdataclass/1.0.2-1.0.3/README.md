# Comparing `tmp/qdataclass-1.0.2.tar.gz` & `tmp/qdataclass-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qdataclass-1.0.2.tar", last modified: Sat Apr 20 09:07:05 2024, max compression
+gzip compressed data, was "qdataclass-1.0.3.tar", last modified: Wed May 22 14:17:15 2024, max compression
```

## Comparing `qdataclass-1.0.2.tar` & `qdataclass-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-20 09:07:05.461144 qdataclass-1.0.2/
--rw-rw-rw-   0        0        0     1070 2023-10-16 13:48:08.000000 qdataclass-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      257 2024-04-20 09:07:05.460140 qdataclass-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      115 2023-10-16 14:09:31.000000 qdataclass-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-20 09:07:05.430112 qdataclass-1.0.2/qdataclass/
--rw-rw-rw-   0        0        0      290 2024-04-14 13:41:16.000000 qdataclass-1.0.2/qdataclass/__init__.py
--rw-rw-rw-   0        0        0     1404 2024-04-20 08:46:41.000000 qdataclass-1.0.2/qdataclass/qdataclass.py
-drwxrwxrwx   0        0        0        0 2024-04-20 09:07:05.457137 qdataclass-1.0.2/qdataclass.egg-info/
--rw-rw-rw-   0        0        0      257 2024-04-20 09:07:05.000000 qdataclass-1.0.2/qdataclass.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2024-04-20 09:07:05.000000 qdataclass-1.0.2/qdataclass.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-20 09:07:05.000000 qdataclass-1.0.2/qdataclass.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-04-20 09:07:05.000000 qdataclass-1.0.2/qdataclass.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-20 09:07:05.461144 qdataclass-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      308 2024-04-20 09:06:57.000000 qdataclass-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 14:17:15.512964 qdataclass-1.0.3/
+-rw-rw-rw-   0        0        0     1070 2023-10-16 13:48:08.000000 qdataclass-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      257 2024-05-22 14:17:15.511963 qdataclass-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      115 2023-10-16 14:09:31.000000 qdataclass-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 14:17:15.493946 qdataclass-1.0.3/qdataclass/
+-rw-rw-rw-   0        0        0      290 2024-04-14 13:41:16.000000 qdataclass-1.0.3/qdataclass/__init__.py
+-rw-rw-rw-   0        0        0      129 2024-05-22 13:05:56.000000 qdataclass-1.0.3/qdataclass/__init__.pyi
+-rw-rw-rw-   0        0        0        0 2024-05-22 13:05:39.000000 qdataclass-1.0.3/qdataclass/py.typed
+-rw-rw-rw-   0        0        0     1419 2024-05-22 13:00:28.000000 qdataclass-1.0.3/qdataclass/qdataclass.py
+-rw-rw-rw-   0        0        0      135 2024-05-22 13:05:56.000000 qdataclass-1.0.3/qdataclass/qdataclass.pyi
+drwxrwxrwx   0        0        0        0 2024-05-22 14:17:15.510961 qdataclass-1.0.3/qdataclass.egg-info/
+-rw-rw-rw-   0        0        0      257 2024-05-22 14:17:15.000000 qdataclass-1.0.3/qdataclass.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2024-05-22 14:17:15.000000 qdataclass-1.0.3/qdataclass.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 14:17:15.000000 qdataclass-1.0.3/qdataclass.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-22 14:17:15.000000 qdataclass-1.0.3/qdataclass.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 14:17:15.512964 qdataclass-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      366 2024-05-22 13:21:04.000000 qdataclass-1.0.3/setup.py
```

### Comparing `qdataclass-1.0.2/LICENSE` & `qdataclass-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `qdataclass-1.0.2/qdataclass/qdataclass.py` & `qdataclass-1.0.3/qdataclass/qdataclass.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,13 +33,13 @@
             continue
         if prop_type in {Property, Signal}:
             continue
         getter, setter = _getter_setter(prop_name)
         signal = Signal(prop_type)
         setattr(cls, prop_name+"Changed", signal)
         setattr(cls, prop_name, Property(
-            prop_type, getter, setter, notify=signal))
+            prop_type, getter, setter, notify=signal)) # type: ignore
     new_class = types.new_class(
         cls.__name__, cls.__bases__, exec_body=lambda ns: ns.update(cls.__dict__))
     sys.modules[cls.__module__].__dict__[cls.__name__] = new_class
     del cls
     return new_class
```

