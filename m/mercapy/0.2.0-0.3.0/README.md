# Comparing `tmp/mercapy-0.2.0.tar.gz` & `tmp/mercapy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mercapy-0.2.0.tar", last modified: Mon May 20 21:21:05 2024, max compression
+gzip compressed data, was "mercapy-0.3.0.tar", last modified: Tue May 21 12:56:56 2024, max compression
```

## Comparing `mercapy-0.2.0.tar` & `mercapy-0.3.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:21:05.793660 mercapy-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-20 21:21:00.000000 mercapy-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-20 21:21:05.793660 mercapy-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-20 21:21:00.000000 mercapy-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:21:05.789661 mercapy-0.2.0/mercapy/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:21:05.789661 mercapy-0.2.0/mercapy/elements/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/elements/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/elements/photo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7788 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/elements/product.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/elements/season.py
--rw-r--r--   0 runner    (1001) docker     (127)     4531 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/merca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:21:05.793660 mercapy-0.2.0/mercapy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/utils/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-20 21:21:00.000000 mercapy-0.2.0/mercapy/utils/warehouses.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 21:21:05.793660 mercapy-0.2.0/mercapy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-20 21:21:05.000000 mercapy-0.2.0/mercapy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-20 21:21:05.000000 mercapy-0.2.0/mercapy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 21:21:05.000000 mercapy-0.2.0/mercapy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 21:21:05.000000 mercapy-0.2.0/mercapy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 21:21:05.000000 mercapy-0.2.0/mercapy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 21:21:05.793660 mercapy-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-20 21:21:00.000000 mercapy-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:56:56.835744 mercapy-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-21 12:56:51.000000 mercapy-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-21 12:56:56.835744 mercapy-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-05-21 12:56:51.000000 mercapy-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:56:56.831743 mercapy-0.3.0/mercapy/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:56:56.831743 mercapy-0.3.0/mercapy/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/elements/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/elements/category.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/elements/photo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7802 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/elements/product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/elements/season.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5237 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/merca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:56:56.835744 mercapy-0.3.0/mercapy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/utils/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-21 12:56:51.000000 mercapy-0.3.0/mercapy/utils/warehouses.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:56:56.835744 mercapy-0.3.0/mercapy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-21 12:56:56.000000 mercapy-0.3.0/mercapy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-21 12:56:56.000000 mercapy-0.3.0/mercapy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 12:56:56.000000 mercapy-0.3.0/mercapy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 12:56:56.000000 mercapy-0.3.0/mercapy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 12:56:56.000000 mercapy-0.3.0/mercapy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 12:56:56.835744 mercapy-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1148 2024-05-21 12:56:51.000000 mercapy-0.3.0/setup.py
```

### Comparing `mercapy-0.2.0/LICENSE` & `mercapy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mercapy-0.2.0/PKG-INFO` & `mercapy-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercapy
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Mercadona interface for Python to track product prices, amounts, and more.
 Author: Joel Taylor
 Author-email: contact@joeltaylor.business
 License: MIT
 Keywords: mercadona,api,sdk,data science,prices,information
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mercapy Version: 0.2.0 Summary: A Mercadona
+Metadata-Version: 2.1 Name: mercapy Version: 0.3.0 Summary: A Mercadona
 interface for Python to track product prices, amounts, and more. Author: Joel
 Taylor Author-email: contact@joeltaylor.business License: MIT Keywords:
 mercadona,api,sdk,data science,prices,information Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.12 Classifier: Programming Language ::
 Python :: Implementation :: CPython Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: requests
```

### Comparing `mercapy-0.2.0/README.md` & `mercapy-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mercapy-0.2.0/mercapy/constants.py` & `mercapy-0.3.0/mercapy/constants.py`

 * *Files identical despite different names*

### Comparing `mercapy-0.2.0/mercapy/elements/photo.py` & `mercapy-0.3.0/mercapy/elements/photo.py`

 * *Files identical despite different names*

### Comparing `mercapy-0.2.0/mercapy/elements/product.py` & `mercapy-0.3.0/mercapy/elements/product.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         warehouse (str): Warehouse or distribution center postal code. Defaults to the one in Níjar, Almería.
         lang (str): The language in which the API responds. Defaults to spanish ("es"), and can also be english ("en").
     """
 
     id: Union[str, dict]
     warehouse: str = MAD1
     lang: Literal["es", "en"] = "es"
-    _endpoint: str = field(init=False, repr=False)
+    _endpoint: str = field(default=None, init=False, repr=False)
     _response: dict = field(default=None, init=False, repr=False)
 
     def __post_init__(self):
         if isinstance(self.id, dict):
             self._response = self.id
             self.id = self._response.get("id")
             if not self.id:
```

### Comparing `mercapy-0.2.0/mercapy/elements/season.py` & `mercapy-0.3.0/mercapy/elements/season.py`

 * *Files identical despite different names*

### Comparing `mercapy-0.2.0/mercapy/merca.py` & `mercapy-0.3.0/mercapy/merca.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Literal
 from urllib.parse import urljoin
 
 from .constants import WAREHOUSES, MAD1
 from .utils.warehouses import get_warehouse_code
 from .utils.api import *
-from .elements import Product, Season
+from .elements import Product, Season, Category
 
 
 class Mercadona:
 
     def __init__(
         self,
         warehouse: Literal[
@@ -42,14 +42,17 @@
 
             # Raise error if the postcode isn't in Mercadona's network
             if self.warehouse is None:
                 raise ValueError(
                     "The postcode specified isn't available in Mercadona's network... Try using any of the warehouse codes in constants.WAREHOUSES."
                 )
 
+    def _get_with_context(self, url: str):
+        return fetch_json(url, {"lang": self.language, "wh": self.warehouse})
+
     def search(self, query: str) -> list[Product]:
         """
         Queries Mercadona's products using their provider "Algolia".
 
         Args:
             query (str): Search query (e.g. Dish Soap).
             lang (str): Language code. Defaults to spanish. Can be "en" too.
@@ -73,15 +76,15 @@
         """
         Retrieves product recommendations for the home page grouped by sections.
 
         Returns:
             dict: Dictionary where keys are layout names and values are lists of recommended products. The lists of products can also include banners which often are Season objects.
         """
         url = urljoin(API_URL, f"/api/home/")
-        response = fetch_json(url, {"lang": self.language, "wh": self.warehouse})
+        response = self._get_with_context(url)
 
         sections = response.get("sections", [])
 
         # Dictionary to store products grouped by sections
         section_products = {}
 
         for section in sections:
@@ -110,16 +113,35 @@
         Args:
             lang (str): Language code. Defaults to spanish. Can be "en" too.
 
         Returns:
             list[Product]: List of new product arrivals.
         """
         url = urljoin(API_URL, f"/api/home/new-arrivals/")
-        response = fetch_json(url, {"lang": self.language, "wh": self.warehouse})
+        response = self._get_with_context(url)
 
         products = []
         for item in response.get("items", []):
             product = Product(item)
             if product.exists():
                 products.append(product)
 
         return products
+
+    def get_categories(self) -> list[Category]:
+        url = urljoin(API_URL, "/api/categories/")
+        response = self._get_with_context(url)
+
+        # Get all level 1 categories
+        lvl1_categories = []
+
+        results = response.get("results", [])
+        for result in results:
+            categories = result.get("categories", [])
+            for category_data in categories:
+                id = category_data.get("id")
+                name = category_data.get("name")
+
+                category = Category(id, name, self.warehouse, self.language)
+                lvl1_categories.append(category)
+
+        return lvl1_categories
```

### Comparing `mercapy-0.2.0/mercapy/utils/api.py` & `mercapy-0.3.0/mercapy/utils/api.py`

 * *Files identical despite different names*

### Comparing `mercapy-0.2.0/mercapy/utils/warehouses.py` & `mercapy-0.3.0/mercapy/utils/warehouses.py`

 * *Files identical despite different names*

### Comparing `mercapy-0.2.0/mercapy.egg-info/PKG-INFO` & `mercapy-0.3.0/mercapy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mercapy
-Version: 0.2.0
+Version: 0.3.0
 Summary: A Mercadona interface for Python to track product prices, amounts, and more.
 Author: Joel Taylor
 Author-email: contact@joeltaylor.business
 License: MIT
 Keywords: mercadona,api,sdk,data science,prices,information
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mercapy Version: 0.2.0 Summary: A Mercadona
+Metadata-Version: 2.1 Name: mercapy Version: 0.3.0 Summary: A Mercadona
 interface for Python to track product prices, amounts, and more. Author: Joel
 Taylor Author-email: contact@joeltaylor.business License: MIT Keywords:
 mercadona,api,sdk,data science,prices,information Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3.12 Classifier: Programming Language ::
 Python :: Implementation :: CPython Description-Content-Type: text/markdown
 License-File: LICENSE Requires-Dist: requests
```

### Comparing `mercapy-0.2.0/setup.py` & `mercapy-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from setuptools import setup, find_packages
 from codecs import open
 from os import path
 
 # Read version from VERSION file
 here = path.abspath(path.dirname(__file__))
 
-VERSION = "0.2.0"
-DESCRIPTION = "A Mercadona interface for Python to track product prices, amounts, and more."
+VERSION = "0.3.0"
+DESCRIPTION = (
+    "A Mercadona interface for Python to track product prices, amounts, and more."
+)
 
 # Get the long description from the README file
 with open(path.join(here, "README.md"), encoding="utf-8") as f:
     LONG_DESCRIPTION = f.read()
 
 setup(
     name="mercapy",
```

