# Comparing `tmp/fmi-weather-client-0.2.2.tar.gz` & `tmp/fmi_weather_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fmi-weather-client-0.2.2.tar", last modified: Thu May  9 19:59:30 2024, max compression
+gzip compressed data, was "fmi_weather_client-0.3.0.tar", last modified: Wed May 22 18:40:09 2024, max compression
```

## Comparing `fmi-weather-client-0.2.2.tar` & `fmi_weather_client-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 mika       (501) staff       (20)        0 2024-05-09 19:59:30.329298 fmi-weather-client-0.2.2/
--rw-r--r--   0 mika       (501) staff       (20)    35149 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.2/LICENSE
--rw-r--r--   0 mika       (501) staff       (20)     5722 2024-05-09 19:59:30.329121 fmi-weather-client-0.2.2/PKG-INFO
--rw-r--r--   0 mika       (501) staff       (20)     4118 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.2/README.md
-drwxr-xr-x   0 mika       (501) staff       (20)        0 2024-05-09 19:59:30.327027 fmi-weather-client-0.2.2/fmi_weather_client/
--rw-r--r--   0 mika       (501) staff       (20)     3776 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.2/fmi_weather_client/__init__.py
--rw-r--r--   0 mika       (501) staff       (20)      507 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.2/fmi_weather_client/errors.py
--rw-r--r--   0 mika       (501) staff       (20)     5064 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.2/fmi_weather_client/http.py
--rw-r--r--   0 mika       (501) staff       (20)     2027 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.2/fmi_weather_client/models.py
-drwxr-xr-x   0 mika       (501) staff       (20)        0 2024-05-09 19:59:30.328115 fmi-weather-client-0.2.2/fmi_weather_client/parsers/
--rw-r--r--   0 mika       (501) staff       (20)        0 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.2/fmi_weather_client/parsers/__init__.py
--rw-r--r--   0 mika       (501) staff       (20)     8290 2024-05-09 19:56:15.000000 fmi-weather-client-0.2.2/fmi_weather_client/parsers/forecast.py
-drwxr-xr-x   0 mika       (501) staff       (20)        0 2024-05-09 19:59:30.327823 fmi-weather-client-0.2.2/fmi_weather_client.egg-info/
--rw-r--r--   0 mika       (501) staff       (20)     5722 2024-05-09 19:59:30.000000 fmi-weather-client-0.2.2/fmi_weather_client.egg-info/PKG-INFO
--rw-r--r--   0 mika       (501) staff       (20)      515 2024-05-09 19:59:30.000000 fmi-weather-client-0.2.2/fmi_weather_client.egg-info/SOURCES.txt
--rw-r--r--   0 mika       (501) staff       (20)        1 2024-05-09 19:59:30.000000 fmi-weather-client-0.2.2/fmi_weather_client.egg-info/dependency_links.txt
--rw-r--r--   0 mika       (501) staff       (20)       35 2024-05-09 19:59:30.000000 fmi-weather-client-0.2.2/fmi_weather_client.egg-info/requires.txt
--rw-r--r--   0 mika       (501) staff       (20)       19 2024-05-09 19:59:30.000000 fmi-weather-client-0.2.2/fmi_weather_client.egg-info/top_level.txt
--rw-r--r--   0 mika       (501) staff       (20)       38 2024-05-09 19:59:30.329359 fmi-weather-client-0.2.2/setup.cfg
--rw-r--r--   0 mika       (501) staff       (20)      907 2024-05-09 19:56:15.000000 fmi-weather-client-0.2.2/setup.py
-drwxr-xr-x   0 mika       (501) staff       (20)        0 2024-05-09 19:59:30.328817 fmi-weather-client-0.2.2/test/
--rw-r--r--   0 mika       (501) staff       (20)     1161 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.2/test/test_http.py
--rw-r--r--   0 mika       (501) staff       (20)     7694 2024-05-09 19:56:15.000000 fmi-weather-client-0.2.2/test/test_init.py
--rw-r--r--   0 mika       (501) staff       (20)      694 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.2/test/test_models.py
--rw-r--r--   0 mika       (501) staff       (20)     2044 2024-02-27 18:12:28.000000 fmi-weather-client-0.2.2/test/test_parsers_forecast.py
+drwxr-xr-x   0 saaste    (1000) saaste    (1000)        0 2024-05-22 18:40:09.886726 fmi_weather_client-0.3.0/
+-rw-r--r--   0 saaste    (1000) saaste    (1000)    35149 2023-10-26 03:11:24.000000 fmi_weather_client-0.3.0/LICENSE
+-rw-r--r--   0 saaste    (1000) saaste    (1000)     4914 2024-05-22 18:40:09.885726 fmi_weather_client-0.3.0/PKG-INFO
+-rw-r--r--   0 saaste    (1000) saaste    (1000)     4118 2024-05-22 18:33:06.000000 fmi_weather_client-0.3.0/README.md
+drwxr-xr-x   0 saaste    (1000) saaste    (1000)        0 2024-05-22 18:40:09.884726 fmi_weather_client-0.3.0/fmi_weather_client/
+-rw-r--r--   0 saaste    (1000) saaste    (1000)     3776 2023-10-26 03:11:24.000000 fmi_weather_client-0.3.0/fmi_weather_client/__init__.py
+-rw-r--r--   0 saaste    (1000) saaste    (1000)      507 2023-10-26 03:11:24.000000 fmi_weather_client-0.3.0/fmi_weather_client/errors.py
+-rw-r--r--   0 saaste    (1000) saaste    (1000)     5064 2024-05-22 18:33:06.000000 fmi_weather_client-0.3.0/fmi_weather_client/http.py
+-rw-r--r--   0 saaste    (1000) saaste    (1000)     2027 2024-05-22 18:33:06.000000 fmi_weather_client-0.3.0/fmi_weather_client/models.py
+drwxr-xr-x   0 saaste    (1000) saaste    (1000)        0 2024-05-22 18:40:09.885726 fmi_weather_client-0.3.0/fmi_weather_client/parsers/
+-rw-r--r--   0 saaste    (1000) saaste    (1000)        0 2023-10-26 03:11:24.000000 fmi_weather_client-0.3.0/fmi_weather_client/parsers/__init__.py
+-rw-r--r--   0 saaste    (1000) saaste    (1000)     8290 2024-05-22 18:33:06.000000 fmi_weather_client-0.3.0/fmi_weather_client/parsers/forecast.py
+drwxr-xr-x   0 saaste    (1000) saaste    (1000)        0 2024-05-22 18:40:09.885726 fmi_weather_client-0.3.0/fmi_weather_client.egg-info/
+-rw-r--r--   0 saaste    (1000) saaste    (1000)     4914 2024-05-22 18:40:09.000000 fmi_weather_client-0.3.0/fmi_weather_client.egg-info/PKG-INFO
+-rw-r--r--   0 saaste    (1000) saaste    (1000)      515 2024-05-22 18:40:09.000000 fmi_weather_client-0.3.0/fmi_weather_client.egg-info/SOURCES.txt
+-rw-r--r--   0 saaste    (1000) saaste    (1000)        1 2024-05-22 18:40:09.000000 fmi_weather_client-0.3.0/fmi_weather_client.egg-info/dependency_links.txt
+-rw-r--r--   0 saaste    (1000) saaste    (1000)       35 2024-05-22 18:40:09.000000 fmi_weather_client-0.3.0/fmi_weather_client.egg-info/requires.txt
+-rw-r--r--   0 saaste    (1000) saaste    (1000)       19 2024-05-22 18:40:09.000000 fmi_weather_client-0.3.0/fmi_weather_client.egg-info/top_level.txt
+-rw-r--r--   0 saaste    (1000) saaste    (1000)       38 2024-05-22 18:40:09.886726 fmi_weather_client-0.3.0/setup.cfg
+-rw-r--r--   0 saaste    (1000) saaste    (1000)     1057 2024-05-22 18:39:24.000000 fmi_weather_client-0.3.0/setup.py
+drwxr-xr-x   0 saaste    (1000) saaste    (1000)        0 2024-05-22 18:40:09.885726 fmi_weather_client-0.3.0/test/
+-rw-r--r--   0 saaste    (1000) saaste    (1000)     1161 2023-10-26 03:11:24.000000 fmi_weather_client-0.3.0/test/test_http.py
+-rw-r--r--   0 saaste    (1000) saaste    (1000)     7694 2024-05-22 18:33:06.000000 fmi_weather_client-0.3.0/test/test_init.py
+-rw-r--r--   0 saaste    (1000) saaste    (1000)      694 2023-10-26 03:11:24.000000 fmi_weather_client-0.3.0/test/test_models.py
+-rw-r--r--   0 saaste    (1000) saaste    (1000)     2044 2024-05-22 18:33:06.000000 fmi_weather_client-0.3.0/test/test_parsers_forecast.py
```

### Comparing `fmi-weather-client-0.2.2/LICENSE` & `fmi_weather_client-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fmi-weather-client-0.2.2/README.md` & `fmi_weather_client-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `fmi-weather-client-0.2.2/fmi_weather_client/__init__.py` & `fmi_weather_client-0.3.0/fmi_weather_client/__init__.py`

 * *Files identical despite different names*

### Comparing `fmi-weather-client-0.2.2/fmi_weather_client/http.py` & `fmi_weather_client-0.3.0/fmi_weather_client/http.py`

 * *Files identical despite different names*

### Comparing `fmi-weather-client-0.2.2/fmi_weather_client/models.py` & `fmi_weather_client-0.3.0/fmi_weather_client/models.py`

 * *Files identical despite different names*

### Comparing `fmi-weather-client-0.2.2/fmi_weather_client/parsers/forecast.py` & `fmi_weather_client-0.3.0/fmi_weather_client/parsers/forecast.py`

 * *Files identical despite different names*

### Comparing `fmi-weather-client-0.2.2/fmi_weather_client.egg-info/SOURCES.txt` & `fmi_weather_client-0.3.0/fmi_weather_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fmi-weather-client-0.2.2/setup.py` & `fmi_weather_client-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fmi-weather-client",
-    version="0.2.2",
+    version="0.3.0",
     author="Mika Hiltunen",
     author_email="saaste@gmail.com",
     description="Library for fetching weather information from Finnish Meteorological Institute (FMI)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/saaste/fmi-weather-client",
     packages=setuptools.find_packages(exclude=["*test", "*test.*"]),
     install_requires=[
-        'requests>=2.31.0',
+        'requests>=2.32.2',
         'xmltodict>=0.13.0'
     ],
     classifiers=[
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.7.17',
+    python_requires='>=3.8.19',
 )
```

### Comparing `fmi-weather-client-0.2.2/test/test_http.py` & `fmi_weather_client-0.3.0/test/test_http.py`

 * *Files identical despite different names*

### Comparing `fmi-weather-client-0.2.2/test/test_init.py` & `fmi_weather_client-0.3.0/test/test_init.py`

 * *Files identical despite different names*

### Comparing `fmi-weather-client-0.2.2/test/test_models.py` & `fmi_weather_client-0.3.0/test/test_models.py`

 * *Files identical despite different names*

### Comparing `fmi-weather-client-0.2.2/test/test_parsers_forecast.py` & `fmi_weather_client-0.3.0/test/test_parsers_forecast.py`

 * *Files identical despite different names*

