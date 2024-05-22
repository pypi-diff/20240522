# Comparing `tmp/MeepMeep-0.6.2.tar.gz` & `tmp/meepmeep-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MeepMeep-0.6.2.tar", last modified: Sat Feb  3 18:52:01 2024, max compression
+gzip compressed data, was "meepmeep-0.6.3.tar", last modified: Wed May 22 13:49:26 2024, max compression
```

## Comparing `MeepMeep-0.6.2.tar` & `meepmeep-0.6.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 hannu     (1000) hannu     (1000)        0 2024-02-03 18:52:01.700466 MeepMeep-0.6.2/
--rw-rw-r--   0 hannu     (1000) hannu     (1000)    35149 2022-01-26 19:18:59.000000 MeepMeep-0.6.2/LICENSE
-drwxrwxr-x   0 hannu     (1000) hannu     (1000)        0 2024-02-03 18:52:01.700466 MeepMeep-0.6.2/MeepMeep.egg-info/
--rw-r--r--   0 hannu     (1000) hannu     (1000)      713 2024-02-03 18:52:01.000000 MeepMeep-0.6.2/MeepMeep.egg-info/PKG-INFO
--rw-rw-r--   0 hannu     (1000) hannu     (1000)      489 2024-02-03 18:52:01.000000 MeepMeep-0.6.2/MeepMeep.egg-info/SOURCES.txt
--rw-rw-r--   0 hannu     (1000) hannu     (1000)        1 2024-02-03 18:52:01.000000 MeepMeep-0.6.2/MeepMeep.egg-info/dependency_links.txt
--rw-rw-r--   0 hannu     (1000) hannu     (1000)       18 2024-02-03 18:52:01.000000 MeepMeep-0.6.2/MeepMeep.egg-info/requires.txt
--rw-rw-r--   0 hannu     (1000) hannu     (1000)        9 2024-02-03 18:52:01.000000 MeepMeep-0.6.2/MeepMeep.egg-info/top_level.txt
--rw-r--r--   0 hannu     (1000) hannu     (1000)      713 2024-02-03 18:52:01.700466 MeepMeep-0.6.2/PKG-INFO
--rw-r--r--   0 hannu     (1000) hannu     (1000)       57 2023-04-19 11:48:24.000000 MeepMeep-0.6.2/README.md
-drwxrwxr-x   0 hannu     (1000) hannu     (1000)        0 2024-02-03 18:52:01.700466 MeepMeep-0.6.2/meepmeep/
--rw-r--r--   0 hannu     (1000) hannu     (1000)       62 2023-04-19 11:48:24.000000 MeepMeep-0.6.2/meepmeep/__init__.py
--rw-r--r--   0 hannu     (1000) hannu     (1000)     2893 2023-04-19 11:48:24.000000 MeepMeep-0.6.2/meepmeep/knot2d.py
--rw-r--r--   0 hannu     (1000) hannu     (1000)     2256 2023-04-19 11:48:24.000000 MeepMeep-0.6.2/meepmeep/knots.py
--rw-r--r--   0 hannu     (1000) hannu     (1000)     1904 2023-04-19 11:48:24.000000 MeepMeep-0.6.2/meepmeep/newton.py
--rw-r--r--   0 hannu     (1000) hannu     (1000)     5989 2023-04-19 11:48:24.000000 MeepMeep-0.6.2/meepmeep/orbit.py
--rw-r--r--   0 hannu     (1000) hannu     (1000)     8904 2023-04-19 11:48:24.000000 MeepMeep-0.6.2/meepmeep/tsorbit.py
--rw-r--r--   0 hannu     (1000) hannu     (1000)     4923 2023-04-19 11:48:24.000000 MeepMeep-0.6.2/meepmeep/utils.py
--rw-r--r--   0 hannu     (1000) hannu     (1000)      830 2023-04-19 11:48:24.000000 MeepMeep-0.6.2/meepmeep/version.py
-drwxrwxr-x   0 hannu     (1000) hannu     (1000)        0 2024-02-03 18:52:01.700466 MeepMeep-0.6.2/meepmeep/xy/
--rw-r--r--   0 hannu     (1000) hannu     (1000)      112 2023-04-19 11:48:24.000000 MeepMeep-0.6.2/meepmeep/xy/__init__.py
--rw-r--r--   0 hannu     (1000) hannu     (1000)     3777 2023-04-19 11:48:24.000000 MeepMeep-0.6.2/meepmeep/xy/derivatives.py
--rw-r--r--   0 hannu     (1000) hannu     (1000)      998 2023-04-19 11:48:24.000000 MeepMeep-0.6.2/meepmeep/xy/par_direct.py
--rw-r--r--   0 hannu     (1000) hannu     (1000)     4433 2023-04-19 11:48:24.000000 MeepMeep-0.6.2/meepmeep/xy/par_fitting.py
--rw-r--r--   0 hannu     (1000) hannu     (1000)     8217 2024-02-03 18:50:02.000000 MeepMeep-0.6.2/meepmeep/xy/position.py
--rw-r--r--   0 hannu     (1000) hannu     (1000)    12206 2023-04-19 11:48:24.000000 MeepMeep-0.6.2/meepmeep/xyz5.py
--rw-r--r--   0 hannu     (1000) hannu     (1000)      869 2024-02-03 18:51:24.000000 MeepMeep-0.6.2/pyproject.toml
--rw-rw-r--   0 hannu     (1000) hannu     (1000)       38 2024-02-03 18:52:01.700466 MeepMeep-0.6.2/setup.cfg
+drwxr-xr-x   0 hannu      (501) staff       (20)        0 2024-05-22 13:49:26.929974 meepmeep-0.6.3/
+-rw-r--r--   0 hannu      (501) staff       (20)    35149 2022-01-26 19:18:59.000000 meepmeep-0.6.3/LICENSE
+drwxr-xr-x   0 hannu      (501) staff       (20)        0 2024-05-22 13:49:26.928314 meepmeep-0.6.3/MeepMeep.egg-info/
+-rw-r--r--   0 hannu      (501) staff       (20)      713 2024-05-22 13:49:26.000000 meepmeep-0.6.3/MeepMeep.egg-info/PKG-INFO
+-rw-r--r--   0 hannu      (501) staff       (20)      489 2024-05-22 13:49:26.000000 meepmeep-0.6.3/MeepMeep.egg-info/SOURCES.txt
+-rw-r--r--   0 hannu      (501) staff       (20)        1 2024-05-22 13:49:26.000000 meepmeep-0.6.3/MeepMeep.egg-info/dependency_links.txt
+-rw-r--r--   0 hannu      (501) staff       (20)       18 2024-05-22 13:49:26.000000 meepmeep-0.6.3/MeepMeep.egg-info/requires.txt
+-rw-r--r--   0 hannu      (501) staff       (20)        9 2024-05-22 13:49:26.000000 meepmeep-0.6.3/MeepMeep.egg-info/top_level.txt
+-rw-r--r--   0 hannu      (501) staff       (20)      713 2024-05-22 13:49:26.929130 meepmeep-0.6.3/PKG-INFO
+-rw-r--r--   0 hannu      (501) staff       (20)       57 2023-04-19 11:48:24.000000 meepmeep-0.6.3/README.md
+drwxr-xr-x   0 hannu      (501) staff       (20)        0 2024-05-22 13:49:26.924069 meepmeep-0.6.3/meepmeep/
+-rw-r--r--   0 hannu      (501) staff       (20)      108 2024-05-08 16:07:49.000000 meepmeep-0.6.3/meepmeep/__init__.py
+-rw-r--r--   0 hannu      (501) staff       (20)     2893 2023-04-19 11:48:24.000000 meepmeep-0.6.3/meepmeep/knot2d.py
+-rw-r--r--   0 hannu      (501) staff       (20)     2256 2023-04-19 11:48:24.000000 meepmeep-0.6.3/meepmeep/knots.py
+-rw-r--r--   0 hannu      (501) staff       (20)     3296 2024-05-08 16:07:49.000000 meepmeep-0.6.3/meepmeep/newton.py
+-rw-r--r--   0 hannu      (501) staff       (20)     5989 2023-04-19 11:48:24.000000 meepmeep-0.6.3/meepmeep/orbit.py
+-rw-r--r--   0 hannu      (501) staff       (20)     8904 2023-04-19 11:48:24.000000 meepmeep-0.6.3/meepmeep/tsorbit.py
+-rw-r--r--   0 hannu      (501) staff       (20)     4923 2023-04-19 11:48:24.000000 meepmeep-0.6.3/meepmeep/utils.py
+-rw-r--r--   0 hannu      (501) staff       (20)      830 2023-04-19 11:48:24.000000 meepmeep-0.6.3/meepmeep/version.py
+drwxr-xr-x   0 hannu      (501) staff       (20)        0 2024-05-22 13:49:26.927230 meepmeep-0.6.3/meepmeep/xy/
+-rw-r--r--   0 hannu      (501) staff       (20)      112 2023-04-19 11:48:24.000000 meepmeep-0.6.3/meepmeep/xy/__init__.py
+-rw-r--r--   0 hannu      (501) staff       (20)     3777 2023-04-19 11:48:24.000000 meepmeep-0.6.3/meepmeep/xy/derivatives.py
+-rw-r--r--   0 hannu      (501) staff       (20)      998 2023-04-19 11:48:24.000000 meepmeep-0.6.3/meepmeep/xy/par_direct.py
+-rw-r--r--   0 hannu      (501) staff       (20)     4433 2023-04-19 11:48:24.000000 meepmeep-0.6.3/meepmeep/xy/par_fitting.py
+-rw-r--r--   0 hannu      (501) staff       (20)     8217 2024-02-03 18:50:02.000000 meepmeep-0.6.3/meepmeep/xy/position.py
+-rw-r--r--   0 hannu      (501) staff       (20)    12206 2023-04-19 11:48:24.000000 meepmeep-0.6.3/meepmeep/xyz5.py
+-rw-r--r--   0 hannu      (501) staff       (20)      869 2024-05-08 16:10:20.000000 meepmeep-0.6.3/pyproject.toml
+-rw-r--r--   0 hannu      (501) staff       (20)       38 2024-05-22 13:49:26.930145 meepmeep-0.6.3/setup.cfg
```

### Comparing `MeepMeep-0.6.2/LICENSE` & `meepmeep-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MeepMeep-0.6.2/MeepMeep.egg-info/PKG-INFO` & `meepmeep-0.6.3/MeepMeep.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeepMeep
-Version: 0.6.2
+Version: 0.6.3
 Summary: Fast Keplerian orbit computation using Taylor series expansions.
 Author-email: Hannu Parviainen <hpparvi@gmail.com>
 Project-URL: homepage, https://github.com/hpparvi/meepmeep
 Keywords: astronomy,astrophysics,exoplanets
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `MeepMeep-0.6.2/PKG-INFO` & `meepmeep-0.6.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MeepMeep
-Version: 0.6.2
+Version: 0.6.3
 Summary: Fast Keplerian orbit computation using Taylor series expansions.
 Author-email: Hannu Parviainen <hpparvi@gmail.com>
 Project-URL: homepage, https://github.com/hpparvi/meepmeep
 Keywords: astronomy,astrophysics,exoplanets
 Classifier: Topic :: Scientific/Engineering
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
```

### Comparing `MeepMeep-0.6.2/meepmeep/knot2d.py` & `meepmeep-0.6.3/meepmeep/knot2d.py`

 * *Files identical despite different names*

### Comparing `MeepMeep-0.6.2/meepmeep/knots.py` & `meepmeep-0.6.3/meepmeep/knots.py`

 * *Files identical despite different names*

### Comparing `MeepMeep-0.6.2/meepmeep/orbit.py` & `meepmeep-0.6.3/meepmeep/orbit.py`

 * *Files identical despite different names*

### Comparing `MeepMeep-0.6.2/meepmeep/tsorbit.py` & `meepmeep-0.6.3/meepmeep/tsorbit.py`

 * *Files identical despite different names*

### Comparing `MeepMeep-0.6.2/meepmeep/utils.py` & `meepmeep-0.6.3/meepmeep/utils.py`

 * *Files identical despite different names*

### Comparing `MeepMeep-0.6.2/meepmeep/version.py` & `meepmeep-0.6.3/meepmeep/version.py`

 * *Files identical despite different names*

### Comparing `MeepMeep-0.6.2/meepmeep/xy/derivatives.py` & `meepmeep-0.6.3/meepmeep/xy/derivatives.py`

 * *Files identical despite different names*

### Comparing `MeepMeep-0.6.2/meepmeep/xy/par_direct.py` & `meepmeep-0.6.3/meepmeep/xy/par_direct.py`

 * *Files identical despite different names*

### Comparing `MeepMeep-0.6.2/meepmeep/xy/par_fitting.py` & `meepmeep-0.6.3/meepmeep/xy/par_fitting.py`

 * *Files identical despite different names*

### Comparing `MeepMeep-0.6.2/meepmeep/xy/position.py` & `meepmeep-0.6.3/meepmeep/xy/position.py`

 * *Files identical despite different names*

### Comparing `MeepMeep-0.6.2/meepmeep/xyz5.py` & `meepmeep-0.6.3/meepmeep/xyz5.py`

 * *Files identical despite different names*

### Comparing `MeepMeep-0.6.2/pyproject.toml` & `meepmeep-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "MeepMeep"
-version = "0.6.2"
+version = "0.6.3"
 description = 'Fast Keplerian orbit computation using Taylor series expansions.'
 authors=[{name='Hannu Parviainen', email='hpparvi@gmail.com'}]
 classifiers=[
   "Topic :: Scientific/Engineering",
   "Intended Audience :: Science/Research",
   "Intended Audience :: Developers",
   "Development Status :: 4 - Beta",
```

