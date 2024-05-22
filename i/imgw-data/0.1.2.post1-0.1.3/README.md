# Comparing `tmp/imgw_data-0.1.2.post1.tar.gz` & `tmp/imgw_data-0.1.3.tar.gz`

## Comparing `imgw_data-0.1.2.post1.tar` & `imgw_data-0.1.3.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 imgw_data-0.1.2.post1/CHANGELOG.md
--rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 imgw_data-0.1.2.post1/CONTRIBUTING.md
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 imgw_data-0.1.2.post1/requirements-dev.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imgw_data-0.1.2.post1/src/imgw_data/__about__.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 imgw_data-0.1.2.post1/src/imgw_data/__init__.py
--rw-r--r--   0        0        0    91808 2020-02-02 00:00:00.000000 imgw_data-0.1.2.post1/src/imgw_data/consts.py
--rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 imgw_data-0.1.2.post1/src/imgw_data/get.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imgw_data-0.1.2.post1/src/imgw_data/export/__init__.py
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 imgw_data-0.1.2.post1/src/imgw_data/export/export.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imgw_data-0.1.2.post1/src/imgw_data/utils/__init__.py
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 imgw_data-0.1.2.post1/src/imgw_data/utils/parse.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 imgw_data-0.1.2.post1/src/imgw_data/utils/translate.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 imgw_data-0.1.2.post1/src/imgw_data/utils/urljoin.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imgw_data-0.1.2.post1/tests/__init__.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 imgw_data-0.1.2.post1/tests/test_load.py
--rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 imgw_data-0.1.2.post1/.gitignore
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 imgw_data-0.1.2.post1/LICENSE
--rw-r--r--   0        0        0     2048 2020-02-02 00:00:00.000000 imgw_data-0.1.2.post1/README.md
--rw-r--r--   0        0        0     1232 2020-02-02 00:00:00.000000 imgw_data-0.1.2.post1/pyproject.toml
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 imgw_data-0.1.2.post1/PKG-INFO
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 imgw_data-0.1.3/CHANGELOG.md
+-rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 imgw_data-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 imgw_data-0.1.3/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imgw_data-0.1.3/src/imgw_data/__about__.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 imgw_data-0.1.3/src/imgw_data/__init__.py
+-rw-r--r--   0        0        0    91808 2020-02-02 00:00:00.000000 imgw_data-0.1.3/src/imgw_data/consts.py
+-rw-r--r--   0        0        0     3156 2020-02-02 00:00:00.000000 imgw_data-0.1.3/src/imgw_data/get.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 imgw_data-0.1.3/src/imgw_data/stations.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imgw_data-0.1.3/src/imgw_data/export/__init__.py
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 imgw_data-0.1.3/src/imgw_data/export/export.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imgw_data-0.1.3/src/imgw_data/utils/__init__.py
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 imgw_data-0.1.3/src/imgw_data/utils/parse.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 imgw_data-0.1.3/src/imgw_data/utils/translate.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 imgw_data-0.1.3/src/imgw_data/utils/urljoin.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 imgw_data-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 imgw_data-0.1.3/tests/test_get_station_coordinates.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 imgw_data-0.1.3/tests/test_load.py
+-rw-r--r--   0        0        0     3837 2020-02-02 00:00:00.000000 imgw_data-0.1.3/.gitignore
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 imgw_data-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 imgw_data-0.1.3/README.md
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 imgw_data-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 imgw_data-0.1.3/PKG-INFO
```

### Comparing `imgw_data-0.1.2.post1/CONTRIBUTING.md` & `imgw_data-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `imgw_data-0.1.2.post1/src/imgw_data/consts.py` & `imgw_data-0.1.3/src/imgw_data/consts.py`

 * *Files identical despite different names*

### Comparing `imgw_data-0.1.2.post1/src/imgw_data/get.py` & `imgw_data-0.1.3/src/imgw_data/get.py`

 * *Files identical despite different names*

### Comparing `imgw_data-0.1.2.post1/src/imgw_data/export/export.py` & `imgw_data-0.1.3/src/imgw_data/export/export.py`

 * *Files identical despite different names*

### Comparing `imgw_data-0.1.2.post1/src/imgw_data/utils/parse.py` & `imgw_data-0.1.3/src/imgw_data/utils/parse.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     raise_error_if_missing : bool, default = False
         If any coordinates are missing then raise error.
 
     Returns
     -------
     : list[dict]
-        Readings woth additional keys: ``lon`` | ``lat``.
+        Readings with additional keys: ``lon`` | ``lat``.
     """
 
     transformed = []
     transformed_ids = set()
     all_ids = set()
 
     for reading in readings:
```

### Comparing `imgw_data-0.1.2.post1/src/imgw_data/utils/translate.py` & `imgw_data-0.1.3/src/imgw_data/utils/translate.py`

 * *Files identical despite different names*

### Comparing `imgw_data-0.1.2.post1/src/imgw_data/utils/urljoin.py` & `imgw_data-0.1.3/src/imgw_data/utils/urljoin.py`

 * *Files identical despite different names*

### Comparing `imgw_data-0.1.2.post1/.gitignore` & `imgw_data-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `imgw_data-0.1.2.post1/LICENSE` & `imgw_data-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `imgw_data-0.1.2.post1/README.md` & `imgw_data-0.1.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 - 'temperatura': 'temperature'
 - 'predkosc_wiatru': 'wind_speed'
 - 'kierunek_wiatru': 'wind_direction'
 - 'wilgotnosc_wzgledna': 'relative_humidity'
 - 'suma_opadu': 'precipitation'
 - 'cisnienie': 'pressure'
 
-### Download as a Python object
+#### Download as a Python object
 
 ```python
 from imgw_data import get_current_weather
 
 
 current_weather_json = get_current_weather()  # downloads data as JSON
 current_weather_csv = get_current_weather(as_csv=True)  # downloads data as string csv
@@ -55,24 +55,41 @@
    'precipitation': '0',
    'pressure': '1028.6'}, 
    {...},
 ]
 
 ```
 
-### Download and export to file
+#### Download and export to file
 
 ```python
 from imgw_data import get_current_weather
 
 
 current_weather_json = get_current_weather(fname='data.json')  # stores data as JSON
 current_weather_csv = get_current_weather(fname='data.csv', as_csv=True)  # stores data as string csv
 current_weather_xml = get_current_weather(fname='data.xml', as_xml=True)  # stores data as string xml
 current_weather_html = get_current_weather(fname='data.html', as_html=True)  # stores data as string html
 
 ```
 
+### `get_active_stations_coordinates()`
+
+Returns list with station id, station longitude, station latitude among the current active stations.
+
+```python
+from imgw_data.stations import get_active_stations_coordinates
+
+
+active_stations = get_active_stations_coordinates()
+print(active_stations[0])
+
+```
+
+```shell
+['12295', 23.162281307080264, 53.10725901708551]
+```
+
 ## Dependencies
 
 - Python >= 3.8
 - `requests`
```

### Comparing `imgw_data-0.1.2.post1/pyproject.toml` & `imgw_data-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "imgw-data"
-version = "0.1.2.post1"
+version = "0.1.3"
 description = 'Python API for public IMGW data - atmospheric measurement from Polish weather stations'
 readme = "README.md"
 requires-python = ">=3.8"
 license = "BSD-3-Clause"
 keywords = ["weather", "weather stations", "poland", "api", "atmospheric science"]
 authors = [
   { name = "Szymon Moliński", email = "simon@ml-gis-service.com" },
```

### Comparing `imgw_data-0.1.2.post1/PKG-INFO` & `imgw_data-0.1.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: imgw-data
-Version: 0.1.2.post1
+Version: 0.1.3
 Summary: Python API for public IMGW data - atmospheric measurement from Polish weather stations
 Project-URL: Documentation, https://github.com/SimonMolinsky/imgw-data-loader#readme
 Project-URL: Issues, https://github.com/SimonMolinsky/imgw-data-loader/issues
 Project-URL: Source, https://github.com/SimonMolinsky/imgw-data-loader
 Author-email: Szymon Moliński <simon@ml-gis-service.com>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
@@ -48,15 +48,15 @@
 - 'temperatura': 'temperature'
 - 'predkosc_wiatru': 'wind_speed'
 - 'kierunek_wiatru': 'wind_direction'
 - 'wilgotnosc_wzgledna': 'relative_humidity'
 - 'suma_opadu': 'precipitation'
 - 'cisnienie': 'pressure'
 
-### Download as a Python object
+#### Download as a Python object
 
 ```python
 from imgw_data import get_current_weather
 
 
 current_weather_json = get_current_weather()  # downloads data as JSON
 current_weather_csv = get_current_weather(as_csv=True)  # downloads data as string csv
@@ -82,24 +82,41 @@
    'precipitation': '0',
    'pressure': '1028.6'}, 
    {...},
 ]
 
 ```
 
-### Download and export to file
+#### Download and export to file
 
 ```python
 from imgw_data import get_current_weather
 
 
 current_weather_json = get_current_weather(fname='data.json')  # stores data as JSON
 current_weather_csv = get_current_weather(fname='data.csv', as_csv=True)  # stores data as string csv
 current_weather_xml = get_current_weather(fname='data.xml', as_xml=True)  # stores data as string xml
 current_weather_html = get_current_weather(fname='data.html', as_html=True)  # stores data as string html
 
 ```
 
+### `get_active_stations_coordinates()`
+
+Returns list with station id, station longitude, station latitude among the current active stations.
+
+```python
+from imgw_data.stations import get_active_stations_coordinates
+
+
+active_stations = get_active_stations_coordinates()
+print(active_stations[0])
+
+```
+
+```shell
+['12295', 23.162281307080264, 53.10725901708551]
+```
+
 ## Dependencies
 
 - Python >= 3.8
 - `requests`
```

