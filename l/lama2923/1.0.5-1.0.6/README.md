# Comparing `tmp/lama2923-1.0.5.tar.gz` & `tmp/lama2923-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lama2923-1.0.5.tar", last modified: Sat May 18 22:52:58 2024, max compression
+gzip compressed data, was "lama2923-1.0.6.tar", last modified: Wed May 22 00:48:46 2024, max compression
```

## Comparing `lama2923-1.0.5.tar` & `lama2923-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 22:52:58.452682 lama2923-1.0.5/
--rw-rw-rw-   0        0        0      962 2024-05-18 22:52:58.451682 lama2923-1.0.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-18 22:52:58.435685 lama2923-1.0.5/lama2923/
--rw-rw-rw-   0        0        0    32120 2024-05-18 22:52:44.000000 lama2923-1.0.5/lama2923/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-18 22:52:58.448681 lama2923-1.0.5/lama2923.egg-info/
--rw-rw-rw-   0        0        0      962 2024-05-18 22:52:57.000000 lama2923-1.0.5/lama2923.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-05-18 22:52:58.000000 lama2923-1.0.5/lama2923.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 22:52:57.000000 lama2923-1.0.5/lama2923.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2024-05-18 22:52:57.000000 lama2923-1.0.5/lama2923.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-18 22:52:57.000000 lama2923-1.0.5/lama2923.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 22:52:58.452682 lama2923-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1300 2024-05-18 22:52:35.000000 lama2923-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 00:48:46.366262 lama2923-1.0.6/
+-rw-rw-rw-   0        0        0      962 2024-05-22 00:48:46.365288 lama2923-1.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 00:48:46.314262 lama2923-1.0.6/lama2923/
+-rw-rw-rw-   0        0        0    22612 2024-05-22 00:47:13.000000 lama2923-1.0.6/lama2923/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 00:48:46.363263 lama2923-1.0.6/lama2923.egg-info/
+-rw-rw-rw-   0        0        0      962 2024-05-22 00:48:45.000000 lama2923-1.0.6/lama2923.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-05-22 00:48:45.000000 lama2923-1.0.6/lama2923.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 00:48:45.000000 lama2923-1.0.6/lama2923.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2024-05-22 00:48:45.000000 lama2923-1.0.6/lama2923.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-22 00:48:45.000000 lama2923-1.0.6/lama2923.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 00:48:46.366262 lama2923-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1300 2024-05-22 00:48:31.000000 lama2923-1.0.6/setup.py
```

### Comparing `lama2923-1.0.5/PKG-INFO` & `lama2923-1.0.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 1.0.5
+Version: 1.0.6
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lama2923-1.0.5/lama2923.egg-info/PKG-INFO` & `lama2923-1.0.6/lama2923.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lama2923
-Version: 1.0.5
+Version: 1.0.6
 Summary: Sikimsonik bir kütüphane
 Author: lama2923
 Author-email: lama2923.v2@gmail.com
 Keywords: example project setuptools development discord lama2923
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lama2923-1.0.5/setup.py` & `lama2923-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 # Komutlar.txt dosyasından komutlar ile terminalde setup dosyasını çalıştırım upload edebilirsin.
 
 setup(
     name='lama2923',
-    version='1.0.5',
+    version='1.0.6',
     description='Sikimsonik bir kütüphane',
     long_description="Discord Api ile işlemler, Webhook ile işlemler, lprint, linput gibi güzel görünümlü yazılar... kısacası projenizde kullanabilceğiniz tasarım olarak ve Api işlemleri için kullanabilceğiniz bir kütüphane, ayrıca bu kütüphanenin ana dili Türkçe.",
     author='lama2923',
     author_email='lama2923.v2@gmail.com',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
```

