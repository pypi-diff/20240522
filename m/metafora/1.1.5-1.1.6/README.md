# Comparing `tmp/metafora-1.1.5.tar.gz` & `tmp/metafora-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metafora-1.1.5.tar", last modified: Thu Nov  2 10:57:20 2023, max compression
+gzip compressed data, was "metafora-1.1.6.tar", last modified: Wed May 22 09:28:37 2024, max compression
```

## Comparing `metafora-1.1.5.tar` & `metafora-1.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-11-02 10:57:20.073312 metafora-1.1.5/
--rw-rw-rw-   0        0        0      281 2023-11-02 10:57:20.071280 metafora-1.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     3935 2023-10-26 09:21:33.000000 metafora-1.1.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-11-02 10:57:20.045062 metafora-1.1.5/metafora/
--rw-rw-rw-   0        0        0      208 2023-11-02 10:56:11.000000 metafora-1.1.5/metafora/__init__.py
--rw-rw-rw-   0        0        0    11804 2023-10-26 09:21:33.000000 metafora-1.1.5/metafora/common.py
--rw-rw-rw-   0        0        0     9942 2023-10-26 09:21:33.000000 metafora-1.1.5/metafora/engineering.py
--rw-rw-rw-   0        0        0     2533 2023-02-18 14:53:20.000000 metafora-1.1.5/metafora/enums.py
--rw-rw-rw-   0        0        0     7478 2023-08-23 05:46:31.000000 metafora-1.1.5/metafora/metar.py
--rw-rw-rw-   0        0        0     2649 2023-11-02 08:45:36.000000 metafora-1.1.5/metafora/parser.py
--rw-rw-rw-   0        0        0     9602 2023-11-02 10:54:56.000000 metafora-1.1.5/metafora/taf.py
--rw-rw-rw-   0        0        0     2518 2023-02-18 14:06:00.000000 metafora-1.1.5/metafora/utils.py
-drwxrwxrwx   0        0        0        0 2023-11-02 10:57:20.067279 metafora-1.1.5/metafora.egg-info/
--rw-rw-rw-   0        0        0      281 2023-11-02 10:57:19.000000 metafora-1.1.5/metafora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-11-02 10:57:19.000000 metafora-1.1.5/metafora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-02 10:57:19.000000 metafora-1.1.5/metafora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-11-02 10:57:19.000000 metafora-1.1.5/metafora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-11-02 10:57:19.000000 metafora-1.1.5/metafora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-11-02 10:57:20.073312 metafora-1.1.5/setup.cfg
--rw-rw-rw-   0        0        0      535 2023-11-02 10:56:07.000000 metafora-1.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:28:37.433134 metafora-1.1.6/
+-rw-rw-rw-   0        0        0      281 2024-05-22 09:28:37.431122 metafora-1.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3935 2023-10-26 09:21:33.000000 metafora-1.1.6/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-22 09:28:37.387378 metafora-1.1.6/metafora/
+-rw-rw-rw-   0        0        0      206 2024-05-22 08:33:17.000000 metafora-1.1.6/metafora/__init__.py
+-rw-rw-rw-   0        0        0    12281 2024-05-22 07:47:32.000000 metafora-1.1.6/metafora/common.py
+-rw-rw-rw-   0        0        0    10737 2024-05-22 08:28:37.000000 metafora-1.1.6/metafora/engineering.py
+-rw-rw-rw-   0        0        0     2551 2024-05-22 07:47:34.000000 metafora-1.1.6/metafora/enums.py
+-rw-rw-rw-   0        0        0     7591 2024-05-22 07:35:15.000000 metafora-1.1.6/metafora/metar.py
+-rw-rw-rw-   0        0        0     2649 2024-05-22 07:47:36.000000 metafora-1.1.6/metafora/parser.py
+-rw-rw-rw-   0        0        0     9730 2024-05-22 07:47:38.000000 metafora-1.1.6/metafora/taf.py
+-rw-rw-rw-   0        0        0     2446 2024-05-22 07:47:40.000000 metafora-1.1.6/metafora/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 09:28:37.427145 metafora-1.1.6/metafora.egg-info/
+-rw-rw-rw-   0        0        0      281 2024-05-22 09:28:36.000000 metafora-1.1.6/metafora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2024-05-22 09:28:37.000000 metafora-1.1.6/metafora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 09:28:36.000000 metafora-1.1.6/metafora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2024-05-22 09:28:37.000000 metafora-1.1.6/metafora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-22 09:28:37.000000 metafora-1.1.6/metafora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 09:28:37.434124 metafora-1.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      521 2024-05-22 08:33:03.000000 metafora-1.1.6/setup.py
```

### Comparing `metafora-1.1.5/README.rst` & `metafora-1.1.6/README.rst`

 * *Files identical despite different names*

### Comparing `metafora-1.1.5/metafora/common.py` & `metafora-1.1.6/metafora/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,17 @@
     convert_speed,
     convert_direction,
     Number,
 )
 from metafora.enums import *
 
 WEATHER_DESCRIPTOR = "|".join(WeatherDescriptor.set())
-WEATHER_PHENOMENA = "|".join(WeatherPrecipitation.set().union(WeatherObscuration.set()).union(OtherWeather.set()))
+WEATHER_PHENOMENA = "|".join(
+    WeatherPrecipitation.set().union(WeatherObscuration.set()).union(OtherWeather.set())
+)
 
 TIME_FORMAT = "(0[0-9]|1[0-9]|2[0-9]|3[0-1])(0[0-9]|1[0-9]|2[0-4])([0-5][0-9])"
 DIRECTION_FMT = "0[0-9][0-9]|1[0-9][0-9]|2[0-9][0-9]|3[0-5][0-9]|360"
 
 
 class Station(str):
     """
@@ -217,14 +219,35 @@
                 distance = convert_distance(distance, "SM")
 
             distance = min(distance, 9999)
 
         return cls(distance=distance, cavok=cavok)
 
 
+class WindShear:
+    """
+    Wind shear class
+    """
+
+    @classmethod
+    def from_text(cls, token: str):
+        """
+        Attempts to parse the wind shear from a token
+
+        :param token: token
+        :return: station instance or None if not successful
+        """
+        found = re.search("^(WS)$", token)
+
+        if not found:
+            return False
+
+        return True
+
+
 @dataclass_json
 @dataclass
 class Weather:
     """
     Weather conditions
     """
 
@@ -243,23 +266,23 @@
         """
         Attempts to parse the weather conditions from a token
 
         :param token: token
         :return: weather conditions instance or None if not successful
         """
         expression = (
-                "^([-+]|VC)?("
-                + WEATHER_DESCRIPTOR
-                + ")?("
-                + WEATHER_PHENOMENA
-                + ")?("
-                + WEATHER_PHENOMENA
-                + ")?("
-                + WEATHER_PHENOMENA
-                + ")?(NSW)?$"
+            "^([-+]|VC)?("
+            + WEATHER_DESCRIPTOR
+            + ")?("
+            + WEATHER_PHENOMENA
+            + ")?("
+            + WEATHER_PHENOMENA
+            + ")?("
+            + WEATHER_PHENOMENA
+            + ")?(NSW)?$"
         )
         found = re.search(expression, token)
 
         if not found:
             return None
 
         intensity = None
@@ -342,21 +365,26 @@
 
             if found[4] in CloudCover.set():
                 amount = found[4]
 
                 # VV is an special case
                 if amount == "VV":
                     vertical_visibility = height
-                    height = None 
+                    height = None
 
         # get cloud type
         if found[6] in CloudType.set():
             cloud = found[6]
 
-        return cls(amount=amount, height=height, vertical_visibility=vertical_visibility, cloud=cloud)
+        return cls(
+            amount=amount,
+            height=height,
+            vertical_visibility=vertical_visibility,
+            cloud=cloud,
+        )
 
 
 def clouds_height(clouds: Union[List[Clouds], None]) -> Union[Number, None]:
     """
     Computes the ceiling based on cloud layers
     A cloud ceiling is the height of the first cloud layer that constitutes at least a broken (BKN) layer
 
@@ -406,44 +434,48 @@
     :return: the most restrictive (maximum) amount of clouds in oktas
     """
     if clouds is None:
         return None
 
     members = CloudCover.list()
     idx = None
-    
+
     for c in clouds:
         if c.amount is not None and c.amount != "VV":
             idx = max(members.index(c.amount), 0 if idx is None else idx)
 
     if idx is not None:
         return (idx + 1) * 2
     else:
         return None
 
 
-def clouds_vertical_visibility(clouds: Union[List[Clouds], None]) -> Union[Number, None]:
+def clouds_vertical_visibility(
+    clouds: Union[List[Clouds], None]
+) -> Union[Number, None]:
     """
     Computes the vertical_visibility from layers of cloudss
 
     :param clouds: layers of clouds
     :return: the most restrictive (minimum) vertical visibilitys
     """
     if clouds is None:
         return None
 
     vertical_visibility = None
 
     for c in clouds:
         if c.amount == "VV" and c.vertical_visibility is not None:
-            vertical_visibility = min(c.vertical_visibility, float(
-                "inf") if vertical_visibility is None else vertical_visibility)
+            vertical_visibility = min(
+                c.vertical_visibility,
+                float("inf") if vertical_visibility is None else vertical_visibility,
+            )
 
     return vertical_visibility
-    
+
 
 def simplify_clouds(clouds: List[Clouds]) -> Clouds:
     """
     Simplifies list of clouds
 
     :param clouds: layers of clouds
     :return: simplified clouds with the most restrictive information
```

### Comparing `metafora-1.1.5/metafora/engineering.py` & `metafora-1.1.6/metafora/engineering.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,35 +8,53 @@
 from metafora.common import simplify_clouds
 from metafora.enums import WeatherPrecipitation, WeatherObscuration, OtherWeather
 from typing import Union, Dict, List, Optional
 from pandas import DataFrame, json_normalize, to_datetime, Timestamp, NaT
 from datetime import datetime, timedelta
 
 BASIC_COLS = [
-              "station", 
-              "visibility_cavok", "visibility_distance", 
-              "clouds_height", "clouds_amount", "clouds_vertical_visibility", 
-              "wind_speed", "wind_gust", "wind_compass",
-              ]
-
-BOOLEAN_COLS = ['precipitation', 
-                'obscuration',
-                'other', 
-                'thunderstorms', 
-                'freezing',
-                'snow', 
-                'clouds']
-
-METAR_SPECIFIC_COLS = ["temperature_temperature", 
-                       "temperature_dewpoint", 
-                       "pressure"]
-
-TAF_SPECIFIC_COLS = ["indicator", "probability", 
-                     "maxtemperature_value",
-                     "mintemperature_value"]
+    "station",
+    "visibility_cavok",
+    "visibility_distance",
+    "clouds_height",
+    "clouds_amount",
+    "clouds_vertical_visibility",
+    "wind_speed",
+    "wind_gust",
+    "wind_compass",
+]
+
+BOOLEAN_COLS = [
+    "precipitation",
+    "obscuration",
+    "other",
+    "thunderstorms",
+    "freezing",
+    "showers",
+    "snow",
+    "ice",
+    "hail",
+    "fog",
+    "clouds",
+    "wind_shear",
+]
+
+METAR_SPECIFIC_COLS = [
+    "temperature_temperature",
+    "temperature_dewpoint",
+    "pressure",
+]
+
+TAF_SPECIFIC_COLS = [
+    "indicator",
+    "probability",
+    "maxtemperature_value",
+    "mintemperature_value",
+]
+
 
 def simplify_report(report: Union[Metar, Forecast]) -> Dict:
     """
     Simplifies a report (TAF or METAR) and converts the result into a basic dictionary
 
     :param report: a raw METAR or TAF report
     :return: simplified dictionary representation of the report
@@ -44,16 +62,20 @@
     features = report.to_dict()
 
     # simplify clouds
     features["clouds"] = simplify_clouds(report.clouds).to_dict()
 
     # simplify runway visual range
     if features.pop("runway_info", None):
-        features["runway_info_min"] = runway_info_distance_min(report.runway_info).to_dict()
-        features["runway_info_max"] = runway_info_distance_max(report.runway_info).to_dict()
+        features["runway_info_min"] = runway_info_distance_min(
+            report.runway_info
+        ).to_dict()
+        features["runway_info_max"] = runway_info_distance_max(
+            report.runway_info
+        ).to_dict()
 
     # flatten weather
     for i, w in enumerate(features.pop("weather", [])):
         features["weather_{}".format(i)] = w
 
     return features
 
@@ -113,44 +135,45 @@
 
         # convert to isoformat
         time_iso = datetime.fromisoformat(time)
         try:
             # parse TAF from raw text
             report = Taf.from_text(t["report"])
 
-            # get station 
+            # get station
             station = report.station
 
             # unify forecasts
             forecasts = propagate_forecasts(report.forecasts)
 
             for f in forecasts:
                 # get validity period
-                start_time = time_from_reference(
-                    f.validity.start_time, time_iso)
+                start_time = time_from_reference(f.validity.start_time, time_iso)
                 end_time = time_from_reference(f.validity.end_time, time_iso)
 
                 # extract ml features
                 report = simplify_report(f)
 
                 # set station as well as release time and validity times in isoformat
                 report["time"] = time
                 report["station"] = station
                 report["validity"]["start_time"] = start_time.isoformat()
                 report["validity"]["end_time"] = end_time.isoformat()
 
                 # min and max temperatures are special cases ...
                 if f.mintemperature is not None and f.mintemperature.time is not None:
                     report["mintemperature"]["time"] = time_from_reference(
-                        f.mintemperature.time, time_iso).isoformat()
+                        f.mintemperature.time, time_iso
+                    ).isoformat()
 
                 if f.maxtemperature is not None and f.maxtemperature.time is not None:
                     report["maxtemperature"]["time"] = time_from_reference(
-                        f.maxtemperature.time, time_iso).isoformat()
-                
+                        f.maxtemperature.time, time_iso
+                    ).isoformat()
+
                 # append the report
                 reports.append(report)
         except Exception:
             if errors == "raise":
                 raise ValueError("{} is not a valid TAF".format(t["report"]))
 
     return reports
@@ -184,15 +207,14 @@
         except Exception:
             if errors == "raise":
                 raise ValueError("{} is not a valid METAR".format(m["report"]))
 
     return reports
 
 
-
 def machine_learning_features(df: DataFrame) -> DataFrame:
     """Simplifies the weather dataframe
        extracting only the most relevant information for aviation
 
     Args:
         weather (DataFrame): original weather dataframe
 
@@ -201,48 +223,76 @@
     """
     # boolean columns to False by default
     df[BOOLEAN_COLS] = False
 
     for c in df.columns:
         if c.endswith("phenomena"):
             # precipitation
-            status = df[c].str.startswith(
-                tuple(WeatherPrecipitation._member_names_)).fillna(False)
+            status = (
+                df[c]
+                .str.startswith(tuple(WeatherPrecipitation._member_names_))
+                .fillna(False)
+            )
             df["precipitation"] = df["precipitation"] | status
 
+            # important precipitation
             # snow
-            status = df[c].str.contains("SN").fillna(False)
+            status = df[c].str.contains(("SN", "SG")).fillna(False)
             df["snow"] = df["snow"] | status
 
+            # hail
+            status = df[c].str.contains(("GR", "GS")).fillna(False)
+            df["hail"] = df["hail"] | status
+
+            # ice
+            status = df[c].str.contains(("IC", "PL")).fillna(False)
+            df["ice"] = df["ice"] | status
+
             # obscuration
-            status = df[c].str.startswith(
-                tuple(WeatherObscuration._member_names_)).fillna(False)
+            status = (
+                df[c]
+                .str.startswith(tuple(WeatherObscuration._member_names_))
+                .fillna(False)
+            )
             df["obscuration"] = df["obscuration"] | status
 
+            # important obscuration
+            # fog
+            status = df[c].str.contains(("FG")).fillna(False)
+            df["fog"] = df["fog"] | status
+
             # other phenomena
-            status = df[c].str.startswith(
-                tuple(OtherWeather._member_names_)).fillna(False)
+            status = (
+                df[c].str.startswith(tuple(OtherWeather._member_names_)).fillna(False)
+            )
             df["other"] = df["other"] | status
+
         elif c.endswith("descriptor"):
             # thunderstorms
             status = (df[c] == "TS").fillna(False)
             df["thunderstorms"] = df["thunderstorms"] | status
 
+            # showers
+            status = (df[c] == "SH").fillna(False)
+            df["showers"] = df["showers"] | status
+
             # freezing
             status = (df[c] == "FZ").fillna(False)
             df["freezing"] = df["freezing"] | status
 
     # general clouds (TCU or CB)
     if "clouds_cloud" in df.columns:
-        df['clouds'] = df["clouds_cloud"].notnull()
+        df["clouds"] = df["clouds_cloud"].notnull()
 
     return df
 
 
-def reports_to_dataframe(reports: List[Dict], drop_invalid: Optional[bool] = False) -> DataFrame:
+def reports_to_dataframe(
+    reports: List[Dict], drop_invalid: Optional[bool] = False
+) -> DataFrame:
     """Converts list of processed reports (METARs or TAFs) to pandas dataframe
     where each row is a report and each column a feature
 
     Args:
         List (Dict): list of reports processed by metafora
         drop_invalid (Optional[bool], optional): drop invalid reports. Defaults to False.
 
@@ -250,26 +300,34 @@
         DataFrame: reports dataframe
     """
     # json normalize, back to pandas
     df = json_normalize(reports, sep="_")
 
     # convert time columns to datetime
     TIME_COLS = []
-    for c in ["time", "validity_start_time", "validity_end_time", "maxtemperature_time", "mintemperature_time"]:
+    for c in [
+        "time",
+        "validity_start_time",
+        "validity_end_time",
+        "maxtemperature_time",
+        "mintemperature_time",
+    ]:
         if c in df.columns:
             df[c] = to_datetime(df[c], errors="coerce")
             TIME_COLS.append(c)
 
     # specific columns
     if "validity_start_time" in TIME_COLS and "validity_end_time" in TIME_COLS:
         # TAF case
         SPECIFIC_COLS = TAF_SPECIFIC_COLS
         if drop_invalid:
-            df.dropna(subset=["station", "time",
-                      "validity_start_time", "validity_end_time"], inplace=True)
+            df.dropna(
+                subset=["station", "time", "validity_start_time", "validity_end_time"],
+                inplace=True,
+            )
 
         # if max and min temperature times are missing
         for c in ["maxtemperature_time", "mintemperature_time"]:
             if c not in TIME_COLS:
                 df[c] = NaT
     else:
         # METAR case
@@ -285,10 +343,10 @@
 
     # create simplified columns
     df = machine_learning_features(df)
 
     # enforce basic and specific columns
     for c in BASIC_COLS + SPECIFIC_COLS:
         if c not in df.columns:
-            df[c] = None 
+            df[c] = None
 
     return df[BASIC_COLS + TIME_COLS + BOOLEAN_COLS + SPECIFIC_COLS]
```

### Comparing `metafora-1.1.5/metafora/enums.py` & `metafora-1.1.6/metafora/enums.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,47 +30,51 @@
         return list(k for k in cls.__members__.keys())
 
 
 class CloudCover(CustomEnum):
     """
     Enumerator of cloud covers
     """
+
     FEW = "a few"
     SCT = "scattered"
     BKN = "broken sky"
     OVC = "overcast sky"
     VV = "vertical visibility"
 
 
 class CloudType(CustomEnum):
     """
     Enumerator of cloud types
     """
+
     TCU = "towering cumulus"
     CB = "cumulonimbus"
 
 
 class WeatherDescriptor(CustomEnum):
     """
     Enumerator of weather descriptors
     """
+
     MI = "shallow"
     PR = "partial"
     BC = "patches of"
     DR = "low drifting"
     BL = "blowing"
     SH = "showers of"
     TS = "thunderstorms"
     FZ = "freezing"
 
 
 class WeatherPrecipitation(CustomEnum):
     """
     Enumerator of weather precipitation
     """
+
     DZ = "drizzle"
     RA = "rain"
     SN = "snow"
     SG = "snow grains"
     IC = "ice crystals"
     PL = "ice pellets"
     GR = "hail"
@@ -78,53 +82,58 @@
     UP = "unknown"
 
 
 class WeatherObscuration(CustomEnum):
     """
     Enumerator of weather obscuration
     """
+
     BR = "mist"
     FG = "fog"
     FU = "smoke"
     DU = "widespread dust"
     SA = "sand"
     HZ = "haze"
 
 
 class OtherWeather(CustomEnum):
     """
     Enumerator of other weather phenomena
     """
+
     PY = "spray"
     VA = "volcanic ash"
     PO = "well-developed dust/sand whirls"
     SQ = "squalls"
     FC = "funnel cloud, tornado, or waterspout"
     SS = "sandstorm"
     DS = "duststorm"
 
 
 class RunwayVisualRangeTrend(CustomEnum):
     """
     Enumerator of event tendencies
     """
+
     D = "decreasing"
     U = "increasing"
     N = "no tendency"
 
 
 class ChangeEu(CustomEnum):
     """
     Enumerator of change indicators
     """
+
     BECMG = "expected to arise soon"
     TEMPO = "expected to arise temporarily"
     INTER = "expected to arise intermittent"
 
 
 class ChangeUS(CustomEnum):
     """
     Enumerator of time indicators
     """
+
     FM = "from"
     AT = "at"
     TL = "until"
```

### Comparing `metafora-1.1.5/metafora/metar.py` & `metafora-1.1.6/metafora/metar.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     Station,
     Timestamp,
     Wind,
     Visibility,
     Clouds,
     Weather,
     Number,
+    WindShear,
 )
 from metafora.parser import ParserMixIn
 from metafora.utils import convert_distance, convert_pressure, convert_direction
 
 
 @dataclass_json
 @dataclass
@@ -206,23 +207,26 @@
     )
     temperature: Optional[Temperature] = field(
         default=None, metadata=config(exclude=lambda x: x is None)
     )
     pressure: Optional[Pressure] = field(
         default=None, metadata=config(exclude=lambda x: x is None)
     )
+    wind_shear: Optional[WindShear] = field(
+        default=None, metadata=config(exclude=lambda x: x is None)
+    )
 
 
 def runway_info_distance_min(runway_info: List[RunwayVisualRange]) -> RunwayVisualRange:
     """
     Gets compass of the runway with minimum distance
 
     :param clouds: list of RVR
     :return: compass and distance
-    """    
+    """
     distance = None
     compass = None
 
     if runway_info is not None:
         for r in runway_info:
             if r.distance is not None:
                 if distance is None or r.distance < distance:
@@ -238,23 +242,23 @@
 
 def runway_info_distance_max(runway_info: List[RunwayVisualRange]) -> RunwayVisualRange:
     """
     Gets compass of the runway with maximum distance
 
     :param clouds: list of RVR
     :return: compass and distance
-    """    
+    """
     distance = None
     compass = None
 
     if runway_info is not None:
         for r in runway_info:
             if r.distance is not None:
                 if distance is None or r.distance > distance:
                     distance = r.distance
                     compass = convert_direction(int(r.runway[:2]))
             elif r.distance_max is not None:
                 if distance is None or r.distance_max > distance:
                     distance = r.distance_max
                     compass = convert_direction(int(r.runway[:2]))
-                
+
     return RunwayVisualRange(runway=compass, distance=distance)
```

### Comparing `metafora-1.1.5/metafora/parser.py` & `metafora-1.1.6/metafora/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     """
     Remove duplicates spaces, newlines and tabs from string
 
     :param raw:
     :return:
     """
     sane = " ".join(raw.split())
-    return sane.strip().rstrip('=')
+    return sane.strip().rstrip("=")
 
 
 @dataclass
 class ParserMixIn:
     """
     Text parser
     """
```

### Comparing `metafora-1.1.5/metafora/taf.py` & `metafora-1.1.6/metafora/taf.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,17 @@
 from metafora.common import (
     Station,
     Timestamp,
     Wind,
     Clouds,
     Weather,
     Visibility,
+    WindShear,
     TIME_FORMAT,
-    Number
+    Number,
 )
 from metafora.parser import ParserMixIn, sanitise_string
 from metafora.enums import ChangeEu
 
 HOUR_FORMAT = "(0[0-9]|1[0-9]|2[0-9]|3[0-1])(0[0-9]|1[0-9]|2[0-4])"
 CHANGE_SEARCH = (
     r"^(PROB[0-9]{2}\sTEMPO)|(TEMPO)|(PROB[0-9]{2})|(INTER)|(BECMG)|(FM"
@@ -198,15 +199,15 @@
         if not found:
             return None
 
         value = int(found[1].replace("M", "-"))
         time = Timestamp.from_text(str(found[2]) + "00Z")
 
         return cls(value=value, time=time)
-    
+
 
 @dataclass_json
 @dataclass
 class Forecast(ParserMixIn):
     """
     Weather forecast dataclass
     """
@@ -234,19 +235,24 @@
     )
     maxtemperature: Optional[MaximumTemperature] = field(
         default=None, metadata=config(exclude=lambda x: x is None)
     )
     mintemperature: Optional[MinimumTemperature] = field(
         default=None, metadata=config(exclude=lambda x: x is None)
     )
+    wind_shear: Optional[WindShear] = field(
+        default=None, metadata=config(exclude=lambda x: x is None)
+    )
+
     def __post_init__(self):
         if self.validity is None:
             # just for compatibility ... In Python 3.10 we could use kw_only of dataclasses
             raise ValueError("Validity is mandatory in forecasts")
 
+
 """         if self.indicator is None:
             if self.validity.start_time is None and self.validity.end_time is not None:
                 self.indicator = Indicator("TL")
             elif (
                 self.validity.end_time is None and self.validity.start_time is not None
             ):
                 self.indicator = Indicator("FM")
@@ -276,17 +282,17 @@
     def from_text(cls, token: str):
         """
         Attempts to parse the TAF from a token
 
         :param token: token
         :return: TAF instance or False if not successful
         """
-        # sanitise 
-        token = sanitise_string(token) 
-        
+        # sanitise
+        token = sanitise_string(token)
+
         # check if it follows a TAF format
         found = re.search(
             "^(PROV\\s)?TAF\\s(AMD\\s|COR\\s)?([A-Z]{4})\\s(" + TIME_FORMAT + "Z)?",
             sanitise_string(token),
         )
 
         if not found:
```

### Comparing `metafora-1.1.5/metafora/utils.py` & `metafora-1.1.6/metafora/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,33 +4,33 @@
 metafora utilities
 """
 from typing import Union
 
 Number = Union[float, int]
 
 COMPASS = [
-            "N",
-            "NNE",
-            "NE",
-            "ENE",
-            "E",
-            "ESE",
-            "SE",
-            "SSE",
-            "S",
-            "SSW",
-            "SW",
-            "WSW",
-            "W",
-            "WNW",
-            "NW",
-            "NNW",
-        ]
+    "N",
+    "NNE",
+    "NE",
+    "ENE",
+    "E",
+    "ESE",
+    "SE",
+    "SSE",
+    "S",
+    "SSW",
+    "SW",
+    "WSW",
+    "W",
+    "WNW",
+    "NW",
+    "NNW",
+]
+
 
-        
 def convert_speed(speed: Number, unit: str) -> float:
     """
     Convets speed to meters per second
 
     :param speed: speed in the original units
     :param unit: units in KT, KPH or MPS
     :return: speed in meters per second
@@ -38,15 +38,17 @@
     if unit == "KT":
         return round(0.514444 * speed, 2)
     elif unit == "KPH":
         return round(0.277778 * speed, 2)
     elif unit == "MPS":
         return round(speed, 2)
     else:
-        raise ValueError("Unknown speed unit {}. Speed unit must be KT, KPH or MPS".format(unit))
+        raise ValueError(
+            "Unknown speed unit {}. Speed unit must be KT, KPH or MPS".format(unit)
+        )
 
 
 def convert_distance(distance: Number, unit: str) -> float:
     """
     Converts distance to meters
 
     :param distance: distance in the original units
@@ -56,15 +58,17 @@
     if unit == "FT":
         return round(0.3048 * distance)
     elif unit == "SM":
         return round(1609.34 * distance)
     elif unit == "M":
         return round(distance)
     else:
-        raise ValueError("Unknown distance unit {}. Distance unit must be FT, SM or M".format(unit))
+        raise ValueError(
+            "Unknown distance unit {}. Distance unit must be FT, SM or M".format(unit)
+        )
 
 
 def convert_pressure(pressure: Number, unit: str) -> float:
     """
     Converts pressure to hPa
 
     :param pressure: pressure in the original units
@@ -72,15 +76,17 @@
     :return: pressure in hPa
     """
     if unit == "A":
         return round(pressure / 0.02953)
     elif unit == "Q":
         return round(pressure)
     else:
-        raise ValueError("Unknown pressure unit {}. Pressure unit must be A or Q".format(unit))
+        raise ValueError(
+            "Unknown pressure unit {}. Pressure unit must be A or Q".format(unit)
+        )
 
 
 def convert_direction(direction: Number) -> str:
     """
     Returns the compass of a wind direction in degrees
 
     :param direction: direction in degrees
```

### Comparing `metafora-1.1.5/setup.py` & `metafora-1.1.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 #!/usr/bin/env python
 from setuptools import setup
 
-setup(name='metafora',
-      version="1.1.5",
-      description='METAR and TAF parser with dataclasses and regular expressions',
-      author='Ramon Dalmau-Codina',
-      author_email='ramon.dalmau.codina@gmail.com',
-      url='https://github.com/ramondalmau/metafora.git',
-      packages=["metafora"],
-      python_requires='>=3.7',
-      install_requires=[
-          'dataclasses>=0.6',
-          'marshmallow>=3.17.0',
-          'dataclasses-json>=0.5.7']
-      )
+setup(
+    name="metafora",
+    version="1.1.6",
+    description="METAR and TAF parser with dataclasses and regular expressions",
+    author="Ramon Dalmau-Codina",
+    author_email="ramon.dalmau.codina@gmail.com",
+    url="https://github.com/ramondalmau/metafora.git",
+    packages=["metafora"],
+    python_requires=">=3.7",
+    install_requires=[
+        "dataclasses>=0.6",
+        "marshmallow>=3.17.0",
+        "dataclasses-json>=0.5.7",
+    ],
+)
```

