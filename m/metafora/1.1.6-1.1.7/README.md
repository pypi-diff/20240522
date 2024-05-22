# Comparing `tmp/metafora-1.1.6.tar.gz` & `tmp/metafora-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metafora-1.1.6.tar", last modified: Wed May 22 09:28:37 2024, max compression
+gzip compressed data, was "metafora-1.1.7.tar", last modified: Wed May 22 12:12:30 2024, max compression
```

## Comparing `metafora-1.1.6.tar` & `metafora-1.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 09:28:37.433134 metafora-1.1.6/
--rw-rw-rw-   0        0        0      281 2024-05-22 09:28:37.431122 metafora-1.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     3935 2023-10-26 09:21:33.000000 metafora-1.1.6/README.rst
-drwxrwxrwx   0        0        0        0 2024-05-22 09:28:37.387378 metafora-1.1.6/metafora/
--rw-rw-rw-   0        0        0      206 2024-05-22 08:33:17.000000 metafora-1.1.6/metafora/__init__.py
--rw-rw-rw-   0        0        0    12281 2024-05-22 07:47:32.000000 metafora-1.1.6/metafora/common.py
--rw-rw-rw-   0        0        0    10737 2024-05-22 08:28:37.000000 metafora-1.1.6/metafora/engineering.py
--rw-rw-rw-   0        0        0     2551 2024-05-22 07:47:34.000000 metafora-1.1.6/metafora/enums.py
--rw-rw-rw-   0        0        0     7591 2024-05-22 07:35:15.000000 metafora-1.1.6/metafora/metar.py
--rw-rw-rw-   0        0        0     2649 2024-05-22 07:47:36.000000 metafora-1.1.6/metafora/parser.py
--rw-rw-rw-   0        0        0     9730 2024-05-22 07:47:38.000000 metafora-1.1.6/metafora/taf.py
--rw-rw-rw-   0        0        0     2446 2024-05-22 07:47:40.000000 metafora-1.1.6/metafora/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-22 09:28:37.427145 metafora-1.1.6/metafora.egg-info/
--rw-rw-rw-   0        0        0      281 2024-05-22 09:28:36.000000 metafora-1.1.6/metafora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2024-05-22 09:28:37.000000 metafora-1.1.6/metafora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 09:28:36.000000 metafora-1.1.6/metafora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2024-05-22 09:28:37.000000 metafora-1.1.6/metafora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-22 09:28:37.000000 metafora-1.1.6/metafora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 09:28:37.434124 metafora-1.1.6/setup.cfg
--rw-rw-rw-   0        0        0      521 2024-05-22 08:33:03.000000 metafora-1.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:12:30.513490 metafora-1.1.7/
+-rw-rw-rw-   0        0        0      281 2024-05-22 12:12:30.512494 metafora-1.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     3935 2023-10-26 09:21:33.000000 metafora-1.1.7/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-22 12:12:30.476486 metafora-1.1.7/metafora/
+-rw-rw-rw-   0        0        0      206 2024-05-22 12:12:11.000000 metafora-1.1.7/metafora/__init__.py
+-rw-rw-rw-   0        0        0    12286 2024-05-22 12:07:37.000000 metafora-1.1.7/metafora/common.py
+-rw-rw-rw-   0        0        0    11320 2024-05-22 12:07:03.000000 metafora-1.1.7/metafora/engineering.py
+-rw-rw-rw-   0        0        0     2551 2024-05-22 07:47:34.000000 metafora-1.1.7/metafora/enums.py
+-rw-rw-rw-   0        0        0     7591 2024-05-22 12:08:14.000000 metafora-1.1.7/metafora/metar.py
+-rw-rw-rw-   0        0        0     2649 2024-05-22 12:03:56.000000 metafora-1.1.7/metafora/parser.py
+-rw-rw-rw-   0        0        0     9730 2024-05-22 07:47:38.000000 metafora-1.1.7/metafora/taf.py
+-rw-rw-rw-   0        0        0     2446 2024-05-22 07:47:40.000000 metafora-1.1.7/metafora/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:12:30.508487 metafora-1.1.7/metafora.egg-info/
+-rw-rw-rw-   0        0        0      281 2024-05-22 12:12:30.000000 metafora-1.1.7/metafora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2024-05-22 12:12:30.000000 metafora-1.1.7/metafora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 12:12:30.000000 metafora-1.1.7/metafora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-22 12:12:30.000000 metafora-1.1.7/metafora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-22 12:12:30.000000 metafora-1.1.7/metafora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 12:12:30.514489 metafora-1.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      521 2024-05-22 12:12:08.000000 metafora-1.1.7/setup.py
```

### Comparing `metafora-1.1.6/README.rst` & `metafora-1.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `metafora-1.1.6/metafora/common.py` & `metafora-1.1.7/metafora/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -219,15 +219,15 @@
                 distance = convert_distance(distance, "SM")
 
             distance = min(distance, 9999)
 
         return cls(distance=distance, cavok=cavok)
 
 
-class WindShear:
+class WindShear(int):
     """
     Wind shear class
     """
 
     @classmethod
     def from_text(cls, token: str):
         """
```

### Comparing `metafora-1.1.6/metafora/engineering.py` & `metafora-1.1.7/metafora/engineering.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,40 +6,45 @@
 from metafora.taf import Forecast, Taf, propagate_forecasts
 from metafora.metar import Metar, runway_info_distance_max, runway_info_distance_min
 from metafora.common import simplify_clouds
 from metafora.enums import WeatherPrecipitation, WeatherObscuration, OtherWeather
 from typing import Union, Dict, List, Optional
 from pandas import DataFrame, json_normalize, to_datetime, Timestamp, NaT
 from datetime import datetime, timedelta
+import re
+
+PRECIPITATION_MEMBERS = frozenset(WeatherPrecipitation._member_names_)
+OBSCURATION_MEMBERS = frozenset(WeatherObscuration._member_names_)
+OTHER_MEMBERS = frozenset(OtherWeather._member_names_)
 
 BASIC_COLS = [
     "station",
     "visibility_cavok",
     "visibility_distance",
     "clouds_height",
     "clouds_amount",
     "clouds_vertical_visibility",
     "wind_speed",
     "wind_gust",
     "wind_compass",
+    "wind_shear",
 ]
 
 BOOLEAN_COLS = [
     "precipitation",
     "obscuration",
     "other",
     "thunderstorms",
     "freezing",
     "showers",
     "snow",
     "ice",
     "hail",
     "fog",
     "clouds",
-    "wind_shear",
 ]
 
 METAR_SPECIFIC_COLS = [
     "temperature_temperature",
     "temperature_dewpoint",
     "pressure",
 ]
@@ -222,55 +227,59 @@
         DataFrame: simplified weather dataframe
     """
     # boolean columns to False by default
     df[BOOLEAN_COLS] = False
 
     for c in df.columns:
         if c.endswith("phenomena"):
-            # precipitation
-            status = (
-                df[c]
-                .str.startswith(tuple(WeatherPrecipitation._member_names_))
-                .fillna(False)
+            # precipitation phenomena
+            phenomena = df[c].apply(
+                lambda x: frozenset() if x is None else frozenset(re.findall("..", x))
             )
-            df["precipitation"] = df["precipitation"] | status
+            precipitation = phenomena.apply(
+                lambda x: x.intersection(PRECIPITATION_MEMBERS)
+            )
+
+            # note that different types of precipitation occurring at the time of observation
+            # are to be reported as one single group
+            # with the dominant type of precipitation reported first
+            df["precipitation"] = df["precipitation"] | precipitation.apply(any)
 
-            # important precipitation
             # snow
-            status = df[c].str.contains(("SN", "SG")).fillna(False)
-            df["snow"] = df["snow"] | status
+            snow = precipitation.apply(
+                lambda x: any(frozenset(["SN", "SG"]).intersection(x))
+            )
+            df["snow"] = df["snow"] | snow
 
             # hail
-            status = df[c].str.contains(("GR", "GS")).fillna(False)
-            df["hail"] = df["hail"] | status
+            hail = precipitation.apply(
+                lambda x: any(frozenset(["GR", "GS"]).intersection(x))
+            )
+            df["hail"] = df["hail"] | hail
 
             # ice
-            status = df[c].str.contains(("IC", "PL")).fillna(False)
-            df["ice"] = df["ice"] | status
-
-            # obscuration
-            status = (
-                df[c]
-                .str.startswith(tuple(WeatherObscuration._member_names_))
-                .fillna(False)
+            ice = precipitation.apply(
+                lambda x: any(frozenset(["IC", "PL"]).intersection(x))
             )
-            df["obscuration"] = df["obscuration"] | status
+            df["ice"] = df["ice"] | ice
+
+            # obscuration phenomena
+            obscuration = phenomena.apply(lambda x: x.intersection(OBSCURATION_MEMBERS))
 
-            # important obscuration
-            # fog
-            status = df[c].str.contains(("FG")).fillna(False)
-            df["fog"] = df["fog"] | status
+            df["obscuration"] = df["obscuration"] | obscuration.apply(any)
+
+            fog = obscuration.apply(lambda x: "FG" in x)
+            df["fog"] = df["fog"] | fog
 
             # other phenomena
-            status = (
-                df[c].str.startswith(tuple(OtherWeather._member_names_)).fillna(False)
-            )
-            df["other"] = df["other"] | status
+            other = phenomena.apply(lambda x: x.intersection(OTHER_MEMBERS))
+            df["other"] = df["other"] | other.apply(any)
 
         elif c.endswith("descriptor"):
+            # only one descriptor per weather level
             # thunderstorms
             status = (df[c] == "TS").fillna(False)
             df["thunderstorms"] = df["thunderstorms"] | status
 
             # showers
             status = (df[c] == "SH").fillna(False)
             df["showers"] = df["showers"] | status
```

### Comparing `metafora-1.1.6/metafora/enums.py` & `metafora-1.1.7/metafora/enums.py`

 * *Files identical despite different names*

### Comparing `metafora-1.1.6/metafora/metar.py` & `metafora-1.1.7/metafora/metar.py`

 * *Files identical despite different names*

### Comparing `metafora-1.1.6/metafora/parser.py` & `metafora-1.1.7/metafora/parser.py`

 * *Files identical despite different names*

### Comparing `metafora-1.1.6/metafora/taf.py` & `metafora-1.1.7/metafora/taf.py`

 * *Files identical despite different names*

### Comparing `metafora-1.1.6/metafora/utils.py` & `metafora-1.1.7/metafora/utils.py`

 * *Files identical despite different names*

### Comparing `metafora-1.1.6/setup.py` & `metafora-1.1.7/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name="metafora",
-    version="1.1.6",
+    version="1.1.7",
     description="METAR and TAF parser with dataclasses and regular expressions",
     author="Ramon Dalmau-Codina",
     author_email="ramon.dalmau.codina@gmail.com",
     url="https://github.com/ramondalmau/metafora.git",
     packages=["metafora"],
     python_requires=">=3.7",
     install_requires=[
```

