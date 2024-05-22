# Comparing `tmp/py-gcode-metadata-0.1.0.tar.gz` & `tmp/py_gcode_metadata-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-gcode-metadata-0.1.0.tar", last modified: Mon Oct  9 12:18:51 2023, max compression
+gzip compressed data, was "py_gcode_metadata-0.2.0.tar", last modified: Wed May 22 12:08:58 2024, max compression
```

## Comparing `py-gcode-metadata-0.1.0.tar` & `py_gcode_metadata-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 mcbig     (1000) mcbig     (1000)        0 2023-10-09 12:18:51.640476 py-gcode-metadata-0.1.0/
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)       45 2023-09-12 06:53:20.000000 py-gcode-metadata-0.1.0/ChangeLog
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)    26451 2023-06-16 09:25:24.000000 py-gcode-metadata-0.1.0/LICENSE
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)      103 2023-09-12 06:53:20.000000 py-gcode-metadata-0.1.0/MANIFEST.in
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     1762 2023-10-09 12:18:51.640476 py-gcode-metadata-0.1.0/PKG-INFO
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)      572 2023-06-16 09:25:24.000000 py-gcode-metadata-0.1.0/README.md
-drwxr-xr-x   0 mcbig     (1000) mcbig     (1000)        0 2023-10-09 12:18:51.624476 py-gcode-metadata-0.1.0/gcode_metadata/
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)      840 2023-09-12 06:53:20.000000 py-gcode-metadata-0.1.0/gcode_metadata/__init__.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)    27285 2023-09-12 06:53:20.000000 py-gcode-metadata-0.1.0/gcode_metadata/metadata.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)        0 2023-06-16 09:25:24.000000 py-gcode-metadata-0.1.0/gcode_metadata/py.typed
-drwxr-xr-x   0 mcbig     (1000) mcbig     (1000)        0 2023-10-09 12:18:51.624476 py-gcode-metadata-0.1.0/py_gcode_metadata.egg-info/
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     1762 2023-10-09 12:18:51.000000 py-gcode-metadata-0.1.0/py_gcode_metadata.egg-info/PKG-INFO
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)      785 2023-10-09 12:18:51.000000 py-gcode-metadata-0.1.0/py_gcode_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)        1 2023-10-09 12:18:51.000000 py-gcode-metadata-0.1.0/py_gcode_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)       15 2023-10-09 12:18:51.000000 py-gcode-metadata-0.1.0/py_gcode_metadata.egg-info/top_level.txt
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     1412 2023-10-09 12:17:02.000000 py-gcode-metadata-0.1.0/pyproject.toml
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)       38 2023-10-09 12:18:51.640476 py-gcode-metadata-0.1.0/setup.cfg
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     1489 2023-10-09 12:17:52.000000 py-gcode-metadata-0.1.0/setup.py
-drwxr-xr-x   0 mcbig     (1000) mcbig     (1000)        0 2023-10-09 12:18:51.624476 py-gcode-metadata-0.1.0/tests/
-drwxr-xr-x   0 mcbig     (1000) mcbig     (1000)        0 2023-10-09 12:18:51.640476 py-gcode-metadata-0.1.0/tests/gcodes/
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)    13268 2023-07-26 06:06:38.000000 py-gcode-metadata-0.1.0/tests/gcodes/.fdn_filename.gcode.cache
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)    21829 2023-06-16 09:25:24.000000 py-gcode-metadata-0.1.0/tests/gcodes/.hidden_fdn_filename.gcode
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)        0 2023-06-16 09:25:24.000000 py-gcode-metadata-0.1.0/tests/gcodes/empty.sl1
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)        0 2023-06-16 09:25:24.000000 py-gcode-metadata-0.1.0/tests/gcodes/fdn_all_empty.gcode
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)    21829 2023-06-16 09:25:24.000000 py-gcode-metadata-0.1.0/tests/gcodes/fdn_filename.gcode
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)    21829 2023-06-16 09:25:24.000000 py-gcode-metadata-0.1.0/tests/gcodes/fdn_filename_empty.gcode
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)  5305022 2023-06-16 09:25:24.000000 py-gcode-metadata-0.1.0/tests/gcodes/fdn_full_0.15mm_PETG_MK3S_2h6m.gcode
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)        0 2023-06-16 09:25:24.000000 py-gcode-metadata-0.1.0/tests/gcodes/fdn_only_filename_0.25mm_PETG_MK3S_2h9m.gcode
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)   100717 2023-06-16 09:25:24.000000 py-gcode-metadata-0.1.0/tests/gcodes/full_m73_layers_0.2mm_PLA_MK3SMMU2S_11m.gcode
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)      323 2023-07-26 05:53:24.000000 py-gcode-metadata-0.1.0/tests/gcodes/mmu_attribute_test.gcode
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)    75757 2023-06-16 09:25:24.000000 py-gcode-metadata-0.1.0/tests/gcodes/pentagonal-hexecontahedron-1.sl1
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)    11618 2023-09-11 10:52:46.000000 py-gcode-metadata-0.1.0/tests/test_metadata.py
+drwxrwxr-x   0 mcbig     (1000) mcbig     (1000)        0 2024-05-22 12:08:58.341205 py_gcode_metadata-0.2.0/
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)      309 2024-05-22 12:03:22.000000 py_gcode_metadata-0.2.0/ChangeLog
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)    26451 2023-06-16 09:25:24.000000 py_gcode_metadata-0.2.0/LICENSE
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)      103 2023-09-12 06:53:20.000000 py_gcode_metadata-0.2.0/MANIFEST.in
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)     1762 2024-05-22 12:08:58.341205 py_gcode_metadata-0.2.0/PKG-INFO
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)      572 2023-06-16 09:25:24.000000 py_gcode_metadata-0.2.0/README.md
+drwxrwxr-x   0 mcbig     (1000) mcbig     (1000)        0 2024-05-22 12:08:58.325205 py_gcode_metadata-0.2.0/gcode_metadata/
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)      847 2024-05-22 12:03:22.000000 py_gcode_metadata-0.2.0/gcode_metadata/__init__.py
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)    33782 2024-05-22 10:55:07.000000 py_gcode_metadata-0.2.0/gcode_metadata/metadata.py
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)        0 2023-06-16 09:25:24.000000 py_gcode_metadata-0.2.0/gcode_metadata/py.typed
+drwxrwxr-x   0 mcbig     (1000) mcbig     (1000)        0 2024-05-22 12:08:58.341205 py_gcode_metadata-0.2.0/py_gcode_metadata.egg-info/
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)     1762 2024-05-22 12:08:58.000000 py_gcode_metadata-0.2.0/py_gcode_metadata.egg-info/PKG-INFO
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)      785 2024-05-22 12:08:58.000000 py_gcode_metadata-0.2.0/py_gcode_metadata.egg-info/SOURCES.txt
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)        1 2024-05-22 12:08:58.000000 py_gcode_metadata-0.2.0/py_gcode_metadata.egg-info/dependency_links.txt
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)       15 2024-05-22 12:08:58.000000 py_gcode_metadata-0.2.0/py_gcode_metadata.egg-info/top_level.txt
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)     1412 2024-05-22 12:03:22.000000 py_gcode_metadata-0.2.0/pyproject.toml
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)       38 2024-05-22 12:08:58.341205 py_gcode_metadata-0.2.0/setup.cfg
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)     1492 2024-05-22 10:55:07.000000 py_gcode_metadata-0.2.0/setup.py
+drwxrwxr-x   0 mcbig     (1000) mcbig     (1000)        0 2024-05-22 12:08:58.325205 py_gcode_metadata-0.2.0/tests/
+drwxrwxr-x   0 mcbig     (1000) mcbig     (1000)        0 2024-05-22 12:08:58.341205 py_gcode_metadata-0.2.0/tests/gcodes/
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)    24453 2024-05-22 10:55:07.000000 py_gcode_metadata-0.2.0/tests/gcodes/.fdn_filename.gcode.cache
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)    21829 2023-06-16 09:25:24.000000 py_gcode_metadata-0.2.0/tests/gcodes/.hidden_fdn_filename.gcode
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)        0 2023-06-16 09:25:24.000000 py_gcode_metadata-0.2.0/tests/gcodes/empty.sl1
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)        0 2023-06-16 09:25:24.000000 py_gcode_metadata-0.2.0/tests/gcodes/fdn_all_empty.gcode
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)    21829 2023-06-16 09:25:24.000000 py_gcode_metadata-0.2.0/tests/gcodes/fdn_filename.gcode
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)    21829 2023-06-16 09:25:24.000000 py_gcode_metadata-0.2.0/tests/gcodes/fdn_filename_empty.gcode
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)  5305022 2023-06-16 09:25:24.000000 py_gcode_metadata-0.2.0/tests/gcodes/fdn_full_0.15mm_PETG_MK3S_2h6m.gcode
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)        0 2023-06-16 09:25:24.000000 py_gcode_metadata-0.2.0/tests/gcodes/fdn_only_filename_0.25mm_PETG_MK3S_2h9m.gcode
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)   100717 2023-06-16 09:25:24.000000 py_gcode_metadata-0.2.0/tests/gcodes/full_m73_layers_0.2mm_PLA_MK3SMMU2S_11m.gcode
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)      323 2023-07-26 05:53:24.000000 py_gcode_metadata-0.2.0/tests/gcodes/mmu_attribute_test.gcode
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)    75757 2023-06-16 09:25:24.000000 py_gcode_metadata-0.2.0/tests/gcodes/pentagonal-hexecontahedron-1.sl1
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)    13206 2024-05-22 10:55:07.000000 py_gcode_metadata-0.2.0/tests/test_metadata.py
```

### Comparing `py-gcode-metadata-0.1.0/LICENSE` & `py_gcode_metadata-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-gcode-metadata-0.1.0/PKG-INFO` & `py_gcode_metadata-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-gcode-metadata
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python library for extraction of metadata from g-code files
 Home-page: https://github.com/prusa3d/gcode-metadata
 Author: Prusa Connect Developers
 Author-email: Prusa Connect Developers <link@prusa3d.cz>
 Maintainer: Prusa Connect Developers
 Maintainer-email: Ondřej Tůma <mcbig@zeropage.cz>, Michal Zoubek <michal.zoubek@prusa3d.cz>, Tomáš Jozífek <jozifektomas@gmail.com>, Šárka Faloutová <sarka.faloutova@prusa3d.cz>, Martin Užák <martin.uzak@prusa3d.cz>
 License: LGPLv2+
```

### Comparing `py-gcode-metadata-0.1.0/README.md` & `py_gcode_metadata-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `py-gcode-metadata-0.1.0/gcode_metadata/__init__.py` & `py_gcode_metadata-0.2.0/gcode_metadata/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Init file describing every importable object"""
 
 from .metadata import MetaData, FDMMetaData, SLMetaData, get_metadata, \
-    UnknownGcodeFileType, estimated_to_seconds, biggest_resolution, \
+    UnknownGcodeFileType, estimated_to_seconds, get_preview, get_icon, \
     get_meta_class
 
-__version__ = "0.1.0"
-__date__ = "11 Sep 2023"  # version date
+__version__ = "0.2.0"
+__date__ = "5 May 2024"  # version date
 __copyright__ = "(c) 2023 Prusa 3D"
 __author_name__ = "Prusa Connect Developers"
 __author_email__ = "link@prusa3d.cz"
 __author__ = f"{__author_name__} <{__author_email__}>"
 __description__ = "Python library for extraction of metadata from g-code files"
 
 __credits__ = "Ondřej Tůma, Michal Zoubek, Tomáš Jozífek, Šárka Faloutová"
 __url__ = "https://github.com/prusa3d/gcode-metadata"
 
 __all__ = [
     "MetaData", "FDMMetaData", "SLMetaData", "get_metadata",
-    "UnknownGcodeFileType", "estimated_to_seconds", "biggest_resolution",
+    "UnknownGcodeFileType", "estimated_to_seconds", "get_preview", "get_icon",
     "get_meta_class"
 ]
```

### Comparing `py-gcode-metadata-0.1.0/gcode_metadata/metadata.py` & `py_gcode_metadata-0.2.0/gcode_metadata/metadata.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,71 +5,128 @@
 import base64
 import json
 import re
 import os
 import zipfile
 from typing import Dict, Any, Type, Callable, List, Optional
 from logging import getLogger
+from importlib.metadata import version
 
 GCODE_EXTENSIONS = (".gcode", ".gc", ".g", ".gco")
+SLA_EXTENSIONS = ("sl1", "sl1s")
 CHARS_TO_REMOVE = ["/", "\\", "\"", "(", ")", "[", "]", "'"]
 
 log = getLogger("connect-printer")
 
 RE_ESTIMATED = re.compile(r"((?P<days>[0-9]+)d\s*)?"
                           r"((?P<hours>[0-9]+)h\s*)?"
                           r"((?P<minutes>[0-9]+)m\s*)?"
                           r"((?P<seconds>[0-9]+)s)?")
 
 PRINTERS = [
-    'MK4IS', 'MK4MMU3', 'MK4', 'MK3SMMU3', 'MK3MMU3', 'MK3SMMU2S', 'MK3MMU2',
-    'MK3S', 'MK3', 'MK2.5SMMU2S', 'MK2.5MMU2', 'MK2.5S', 'MK2.5', 'MINI',
-    'XL5', 'XL4', 'XL3', 'XL2', 'XL', 'iX', 'SL1', 'SHELF', 'EXTRACTOR',
-    'HARVESTER'
-]
+        'MK4IS', 'MK4MMU3', 'MK4', 'MK3SMMU3', 'MK3MMU3', 'MK3SMMU2S',
+        'MK3MMU2', 'MK3S', 'MK3', 'MK2.5SMMU2S', 'MK2.5MMU2', 'MK2.5S',
+        'MK2.5', 'MK3.5', 'MK3.9', 'MINI', 'MINIIS', 'XL5', 'XL4', 'XL3',
+        'XL2', 'XL', 'iX', 'SL1', 'SHELF', 'EXTRACTOR', 'HARVESTER'
+    ]
 
 PRINTERS.sort(key=len, reverse=True)
 
 MATERIALS = [
-    'PLA', 'PETG', 'ABS', 'ASA', 'FLEX', 'HIPS', 'EDGE', 'NGEN', 'PA', 'PVA',
-    'PCTG', 'PP', 'PC', 'TPU', 'PEBA', 'CPE', 'PVB', 'PET'
+    'PLA', 'PETG', 'ABS', 'ASA', 'FLEX', 'HIPS', 'EDGE', 'NGEN', 'PA',
+    'PVA', 'PCTG', 'PP', 'PC', 'PEBA', 'CPE', 'PVB', 'PET', 'PLA Tough',
+    'METAL', 'TPU', 'NYLON'
 ]
 
+IMAGE_FORMATS = ['PNG', 'JPG']
+
 
 class UnknownGcodeFileType(ValueError):
     # pylint: disable=missing-class-docstring
     ...
 
 
+class ImageInfo:
+    """A class to hold image info for thumbnail selection purposes"""
+
+    def __init__(self, width, height, format_):
+        self.width = width
+        self.height = height
+        self.format = format_
+
+    @property
+    def ratio(self):
+        """Gets the image ratio"""
+        return self.width / self.height
+
+    @staticmethod
+    def dimension_badness(width, target_width):
+        """Returns a badness score for the size difference between the image
+        and the target dimension. The score is higher when the dimension is
+        smaller than the target dimension"""
+        size_difference = width - target_width
+        if size_difference < 0:
+            return (abs(size_difference) + 2)**2
+        return size_difference
+
+    def badness(self, target: "ImageInfo", aspect_ratio_weight=1):
+        """Returns a badness score for this image compared to the target"""
+        # This gives a value between 1 and infinity
+        ar_badness = (max(self.ratio, target.ratio) /
+                      min(self.ratio, target.ratio))
+
+        width_badness = self.dimension_badness(self.width, target.width)
+        height_badness = self.dimension_badness(self.height, target.height)
+        size_badness = width_badness + height_badness
+
+        # The aspect ratio weight of 2 would square aspect ratio badness
+        # while using a square root on the size badness
+        # As the aspect ratio minimum is 1, let's make the lowest value
+        # 0.01 by subtracting 0.99
+        weighted_ar_badness = ar_badness**aspect_ratio_weight - 0.99
+        weighted_size_badness = size_badness**(1 / aspect_ratio_weight)
+
+        return weighted_ar_badness * weighted_size_badness
+
+    @staticmethod
+    def from_thumbnail_info(info: str):
+        """Parses thumbnail info from string thumbnail key format"""
+        string_resolution, format_ = info.split("_")
+        width, height = tuple(map(int, string_resolution.split('x')))
+        return ImageInfo(width, height, format_)
+
+    def to_thumbnail_info(self):
+        """Returns thumbnail info in string thumbnail key format"""
+        return f"{self.width}x{self.height}_{self.format}"
+
+    def __str__(self):
+        return self.to_thumbnail_info()
+
+    def __repr__(self):
+        return f'ImageInfo("{str(self)}")'
+
+
 def get_mmu_name(name):
     """Returns a name for the new list value item"""
     return f"{name} per tool"
 
 
 def check_gcode_completion(path):
     """Check g-code integrity"""
     log.debug(path)
 
 
-def thumbnail_from_bytes(data_input):
-    """Parse thumbnail from bytes to string format because
-    of JSON serialization requirements"""
-    converted_data = {}
-    for key, value in data_input.items():
-        if isinstance(value, bytes):
-            converted_data[key] = str(value, 'utf-8')
-    return converted_data
-
-
-def thumbnail_to_bytes(data_input):
-    """Parse thumbnail from string to original bytes format"""
-    converted_data = {}
-    for key, value in data_input.items():
-        converted_data[key] = bytes(value, 'utf-8')
-    return converted_data
+def from_bytes(data) -> str:
+    """Convert data in bytes to string"""
+    return str(data, 'utf-8')
+
+
+def to_bytes(data) -> bytes:
+    """Convert string to data in bytes"""
+    return bytes(data, 'utf-8')
 
 
 def estimated_to_seconds(value: str):
     """Convert string value to seconds.
 
     >>> estimated_to_seconds("2s")
     2
@@ -110,15 +167,15 @@
         'PETG'
         >>> extract_data("PLA_0.6n 0.32mm_MK3S_1d1h42m")['printer']
         'MK3S'
         >>> extract_data("42.gcode")['printer'] is None
         True
         >>> extract_data("Tisk tohoto souboru bude trvat 1d18h15m")['time']
         '1d18h15m'
-        >>> extract_data("+ěščřžýáíé \\/ -.:<>.gcode") #doctest: +ELLIPSIS
+        >>> extract_data("+ěščřžýáíé / -.:<>.gcode") #doctest: +ELLIPSIS
         {'name': None, ..., 'material': None, 'printer': None, 'time': None}
         >>> extract_data("Tohle je PLA, nebo PETG, nevim.gcode")['material']
         'PLA'
         >>> extract_data("ßüäö")['printer'] is None
         True
     """
 
@@ -179,70 +236,149 @@
 
         """
         path_ = os.path.split(self.path)
         new_path = path_[0] + "/." + path_[1] + ".cache"
         return new_path
 
     def is_cache_fresh(self):
-        """If cache is fresher than file, returns True"""
+        """Checks if we can use the current cache file"""
+        return self.is_cache_recent() and self.is_cache_correct_version()
+
+    def is_cache_recent(self):
+        """Checks if the cache file is newer than the source file"""
         try:
             file_time_created = os.path.getctime(self.path)
             cache_time_created = os.path.getctime(self.cache_name)
-            return file_time_created < cache_time_created
         except FileNotFoundError:
             return False
 
+        return file_time_created < cache_time_created
+
+    def is_cache_correct_version(self):
+        """Checks if the cache file was created with the same version
+        of gcode-metadata"""
+
+        def isallowed(char):
+            """Filters out disallowed characters, used with str.filter"""
+            return char not in "\",\n} "
+
+        # This expects the first item in the json file to be the
+        # gcode-metadata version, with which the cache was created.
+        # If it's not there, or the version is different, the cache is deleted
+        with open(self.cache_name, "r", encoding="utf-8") as file:
+            for line in file:
+                if text := "".join(filter(str.isalpha, line)):
+                    if text.startswith("version"):
+                        break
+                    return False
+            else:  # didn't reach break
+                return False
+            first_pair = line.split(",", 1)[0]
+            _, version_part = first_pair.split(":", 1)
+            file_version = "".join(filter(isallowed, version_part))
+            if file_version == version('py-gcode-metadata'):
+                return True
+
+        return False
+
     def save_cache(self):
         """Take metadata from source file and save them as JSON to
-        <file_name>.cache file"""
+        <file_name>.cache file.
+        Parse thumbnail from bytes to string format because of JSON
+        serialization requirements"""
+
+        def get_cache_data(info):
+            width, height = info.width, info.height
+
+            return {
+                "resolution": f"{width}x{height}",
+                "data": from_bytes(self.thumbnails[info.to_thumbnail_info()]),
+                "format": info.format
+            }
+
         try:
-            if self.thumbnails or self.data:
-                dict_data = {
-                    "thumbnails": thumbnail_from_bytes(self.thumbnails),
-                    "data": self.data
+            if self.data:
+                cache = {
+                    "version": version('py-gcode-metadata'),
+                    "metadata": self.data,
                 }
+
+                if self.thumbnails:
+
+                    if preview := get_preview(self.thumbnails):
+                        cache["preview"] = get_cache_data(preview)
+
+                    if icon := get_icon(self.thumbnails):
+                        cache["icon"] = get_cache_data(icon)
+
                 with open(self.cache_name, "w", encoding='utf-8') as file:
-                    json.dump(dict_data, file, indent=2)
+                    json.dump(cache, file, indent=2)
         except PermissionError:
             log.warning("You don't have permission to save file here")
 
     def load_cache(self):
         """Load metadata values from <file_name>.cache file"""
         try:
             with open(self.cache_name, "r", encoding='utf-8') as file:
                 cache_data = json.load(file)
-            self.thumbnails = thumbnail_to_bytes(cache_data["thumbnails"])
-            self.data = cache_data["data"]
+                preview = cache_data.get("preview")
+                icon = cache_data.get("icon")
+
+            self.thumbnails = {}
+
+            if preview:
+                key = f"{preview['resolution']}_{preview['format']}"
+                self.thumbnails[key] = to_bytes(preview["data"])
+            if icon:
+                key = f"{icon['resolution']}_{icon['format']}"
+                self.thumbnails[key] = to_bytes(icon["data"])
+
+            self.data = cache_data["metadata"]
         except (json.decoder.JSONDecodeError, FileNotFoundError, KeyError)\
                 as err:
             raise ValueError(
                 "JSON data not found or in incorrect format") from err
 
     def load(self, save_cache=True):
         """Extract and set metadata from `self.path`. Any metadata
         obtained from the path will be overwritten by metadata from
         the file if the metadata is contained there as well"""
+        cache_loaded = False
         if self.is_cache_fresh():
-            self.load_cache()
-        else:
-            self.load_from_path(self.path)
-            self.load_from_file(self.path)
-            if save_cache:
-                self.save_cache()
+            try:
+                self.load_cache()
+                cache_loaded = True
+            except Exception:  # pylint: disable=broad-except
+                log.warning("Failed loading cache for: %s", self.path)
+        if not cache_loaded:
+            try:
+                self.load_from_path(self.path)
+                self.load_from_file(self.path)
+            except Exception:  # pylint: disable=broad-except
+                log.exception("Failed loading metadata from: %s", self.path)
+            else:
+                if save_cache:
+                    self.save_cache()
 
     def load_from_file(self, path: str):
         """Load metadata and thumbnails from given `path`"""
         # pylint: disable=unused-argument
 
     def load_from_path(self, path: str):
         """Load metadata from given path (path, not its content),
         if possible.
         """
         # pylint: disable=unused-argument
 
+    def load_from_chunk(self, data: bytes, size: int):
+        """Process given chunk array of data.
+        :data: data of a chunk.
+        :size: size of the file."""
+        # pylint: disable=unused-argument
+
     def set_data(self, data: Dict):
         """Helper function to save all items from `data` that
         match `self.Attr` in `self.data`.
         """
         for attr, conv in self.Attrs.items():
             val = data.get(attr)
             if not val:
@@ -300,14 +436,15 @@
         except ValueError:
             single_value = None
         return parsed, single_value
 
 
 class FDMMetaData(MetaData):
     """Class for extracting Metadata for FDM gcodes"""
+    # pylint: disable=too-many-instance-attributes
 
     def set_attr(self, name, value):
         """Set an attribute, but add support for mmu list attributes"""
         if name in self.MMUAttrs:
             value_list, single_value = self.MMUAttrs[name].from_string(value)
             mmu_name = get_mmu_name(name)
             if value_list is not None:
@@ -369,15 +506,14 @@
         "quiet_left_present": bool,
         "quiet_change_in_present": bool,
         "normal_percent_present": bool,
         "normal_left_present": bool,
         "normal_change_in_present": bool,
         "layer_info_present": bool,
         "max_layer_z": float,
-        "thumbnails_format": str,
     }
 
     # Add attributes that have multiple values in MMU print gcodes
     # pylint: disable=no-value-for-parameter
     for name, mmu_attribute in MMUAttrs.items():
         mmu_name = get_mmu_name(name)
         Attrs[name] = mmu_attribute.value_type
@@ -421,17 +557,18 @@
 
     def __init__(self, path: str):
         super().__init__(path)
         self.last_filename = None
 
         # When in the process of parsing an image, these won't be None
         # Parsed as in currently being parsed
-        self.parsed_image_dimensions = None
-        self.parsed_image_size = None
-        self.parsed_image = None
+        self.img_format = None
+        self.img_dimensions = None
+        self.img_size = None
+        self.img = None
 
         self.m73_searched_bytes = 0
 
     def load_from_path(self, path):
         """Try to obtain any usable metadata from the path itself"""
         filename = os.path.basename(path)
         data = extract_data(filename)
@@ -448,34 +585,40 @@
         self.set_data(result)
 
     def from_comment_line(self, line):
         """Parses data from a line in the comments"""
         # thumbnail handling
         match = self.THUMBNAIL_BEGIN_PAT.match(line)
         if match:
-            self.parsed_image_dimensions = match.group("dim")
-            self.parsed_image_size = int(match.group("size"))
-            self.parsed_image = []
+            img_format = match.group("format")
+
+            # PNG is not explicitly described in thumbnails header
+            self.img_format = "PNG" if img_format == "" else img_format
+            self.img_dimensions = match.group("dim")
+            self.img_size = int(match.group("size"))
+            self.img = []
             return
 
         match = self.THUMBNAIL_END_PAT.match(line)
         if match:
-            image_data = "".join(self.parsed_image)
-            self.thumbnails[self.parsed_image_dimensions] = image_data.encode()
-            assert len(image_data) == self.parsed_image_size, len(image_data)
-
-            self.parsed_image_dimensions = None
-            self.parsed_image_size = None
-            self.parsed_image = None
+            img_data = "".join(self.img)
+            key = f"{self.img_dimensions}_{self.img_format}"
+            self.thumbnails[key] = img_data.encode()
+            assert len(img_data) == self.img_size, len(img_data)
+
+            self.img_format = None
+            self.img_dimensions = None
+            self.img_size = None
+            self.img = None
             return
 
         # We store the image data only during parsing. If actively parsing:
-        if self.parsed_image is not None:
+        if self.img is not None:
             line = line[2:].strip()
-            self.parsed_image.append(line)
+            self.img.append(line)
 
         # For the bulk of metadata comments
         match = self.KEY_VAL_PAT.match(line)
         if match:
             key, val = match.groups()
             self.set_attr(key, val)
 
@@ -632,15 +775,16 @@
         "min_initial_exposure_time": float,
         "min_exposure_time": float,
         "layer_height": float,
         "materialName": str,
         "fileCreationTimestamp": str,
     }
 
-    THUMBNAIL_NAME_PAT = re.compile(r"(?P<dim>\d+x\d+)")
+    THUMBNAIL_NAME_PAT = re.compile(
+        r".*?(?P<dim>\d+x\d+)\.(?P<format>qoi|jpg|png)")
 
     def load(self, save_cache=True):
         """Load metadata"""
         try:
             super().load(save_cache)
         except zipfile.BadZipFile:
             # NOTE can't import `log` from __init__.py because of
@@ -686,19 +830,21 @@
         :returns Dictionary with thumbnail dimensions as key and base64
             encoded image as value.
         """
         thumbnails: Dict[str, bytes] = {}
         with zipfile.ZipFile(path, "r") as zip_file:
             for info in zip_file.infolist():
                 if info.filename.startswith("thumbnail/"):
-                    data = zip_file.read(info.filename)
-                    data = base64.b64encode(data)
-                    dim = SLMetaData.THUMBNAIL_NAME_PAT.findall(
-                        info.filename)[-1]
-                    thumbnails[dim] = data
+                    match = SLMetaData.THUMBNAIL_NAME_PAT.match(info.filename)
+                    if match:
+                        img_format = match.group("format").upper()
+                        img_dim = match.group("dim")
+                        data = zip_file.read(info.filename)
+                        data = base64.b64encode(data)
+                        thumbnails[f"{img_dim}_{img_format}"] = data
         return thumbnails
 
 
 def get_metadata(path: str, save_cache=True, filename=None):
     """Returns the Metadata for given `path`
 
     :param path: Gcode file
@@ -722,56 +868,80 @@
         fnl = filename.lower()
     else:
         fnl = path.lower()
 
     meta_class: MetaData
     if fnl.lower().endswith(GCODE_EXTENSIONS):
         meta_class = FDMMetaData(path)
-    elif fnl.lower().endswith(".sl1"):
+    elif fnl.lower().endswith(SLA_EXTENSIONS):
         meta_class = SLMetaData(path)
     else:
         raise UnknownGcodeFileType(path)
     return meta_class
 
 
-def biggest_resolution(thumbnails: Dict[str, bytes]):
-    """Get the thumbnail with the biggest resolution from the list of
-    thumbnails
+def get_closest_image(thumbnails: Dict[str, bytes],
+                      target: ImageInfo,
+                      aspect_ratio_weight: float = 1.0) -> Optional[ImageInfo]:
+    """Get the image with the closest resolution
+    and aspect ratio to the target
+    The weight of aspect ratio to resolution proximity can be tweaked"""
+    valid_thumbnails: List[ImageInfo] = []
+    for thumbnail in thumbnails.keys():
+        info: ImageInfo = ImageInfo.from_thumbnail_info(thumbnail)
+        if info.format in IMAGE_FORMATS:
+            if info.width >= 50 and info.height >= 50:
+                valid_thumbnails.append(info)
 
-    >>> biggest_resolution({'8000x200': b'', '600x400': b'', '800x600': b''})
-    '800x600'
-    >>> biggest_resolution({'600x1': b'', '320x240': b'', '800x9000': b''})
-    '320x240'
-    >>> biggest_resolution({'500x100': b'', '50x50': b'', '900x400': b''})
-    '50x50'
-    >>> biggest_resolution({'500x200': b''})
-    '500x200'
-    """
-    max_resolution_key = None
-    max_res = 0
+    if not valid_thumbnails:
+        return None
 
-    for resolution in thumbnails:
-        width, height = map(int, resolution.split('x'))
+    sorted_thumbnails: List[ImageInfo] = sorted(
+        valid_thumbnails, key=lambda x: x.badness(target, aspect_ratio_weight))
 
-        # Calculate ratio and consider only values in between 1 and 2
-        ratio = width / height
-        res = width * height
-        if 1 <= ratio <= 2:
-            if res > max_res:
-                max_res = res
-                max_resolution_key = resolution
-        else:
-            log.info("Thumbnail ratio is not between 1 and 2: %s", ratio)
+    return sorted_thumbnails[0]
+
+
+def get_preview(thumbnails: Dict[str, bytes]) -> Optional[ImageInfo]:
+    """Get the preview with the biggest resolution from the list of
+    thumbnails
 
-    if max_resolution_key is None:
-        log.info("No thumbnail with ratio between 1 and 2 found. "
-                 "Using biggest thumbnail.")
-        max_resolution_key = max(thumbnails.keys())
+    >>> get_preview(
+    ... {'8000x20_PNG': b'', '600x400_PNG': b'', '800x600_PNG': b''})
+    ImageInfo("800x600_PNG")
+    >>> get_preview(
+    ... {'600x1_PNG': b'', '320x240_PNG': b'', '800x9000_PNG': b''})
+    ImageInfo("320x240_PNG")
+    >>> get_preview(
+    ... {'500x100_PNG': b'', '50x50_PNG': b'', '900x400_PNG': b''})
+    ImageInfo("900x400_PNG")
+    >>> get_preview({'500x200_PNG': b''})
+    ImageInfo("500x200_PNG")
+    """
 
-    return max_resolution_key
+    return get_closest_image(thumbnails,
+                             ImageInfo(640, 480, "PNG"),
+                             aspect_ratio_weight=1)
+
+
+def get_icon(thumbnails: Dict[str, bytes]) -> Optional[ImageInfo]:
+    """Get the icon which suits best according given parameters
+
+    >>> get_icon({'8000x20_PNG': b'', '600x400_PNG': b'', '800x600_PNG': b''})
+    ImageInfo("600x400_PNG")
+    >>> get_icon({'600x1_PNG': b'', '320x240_PNG': b'', '800x9000_PNG': b''})
+    ImageInfo("320x240_PNG")
+    >>> get_icon({'500x100_PNG': b'', '50x50_PNG': b'', '120x110_PNG': b''})
+    ImageInfo("120x110_PNG")
+    >>> get_icon({'50x20_PNG': b''}) is None
+    True
+    """
+    return get_closest_image(thumbnails,
+                             ImageInfo(100, 100, "PNG"),
+                             aspect_ratio_weight=1)
 
 
 if __name__ == "__main__":
     import argparse
 
     parser = argparse.ArgumentParser()
     parser.add_argument("file", help="gcode file")
```

### Comparing `py-gcode-metadata-0.1.0/py_gcode_metadata.egg-info/PKG-INFO` & `py_gcode_metadata-0.2.0/py_gcode_metadata.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-gcode-metadata
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python library for extraction of metadata from g-code files
 Home-page: https://github.com/prusa3d/gcode-metadata
 Author: Prusa Connect Developers
 Author-email: Prusa Connect Developers <link@prusa3d.cz>
 Maintainer: Prusa Connect Developers
 Maintainer-email: Ondřej Tůma <mcbig@zeropage.cz>, Michal Zoubek <michal.zoubek@prusa3d.cz>, Tomáš Jozífek <jozifektomas@gmail.com>, Šárka Faloutová <sarka.faloutova@prusa3d.cz>, Martin Užák <martin.uzak@prusa3d.cz>
 License: LGPLv2+
```

### Comparing `py-gcode-metadata-0.1.0/py_gcode_metadata.egg-info/SOURCES.txt` & `py_gcode_metadata-0.2.0/py_gcode_metadata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-gcode-metadata-0.1.0/pyproject.toml` & `py_gcode_metadata-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "py-gcode-metadata"
-version = "0.1.0"
+version = "0.2.0"
 description = "Python library for extraction of metadata from g-code files"
 readme = {file = "README.md", content-type="text/markdown"}
 license = {text = "LGPLv2+"}
 
 authors = [
     {name = "Prusa Connect Developers", email = "link@prusa3d.cz"},
 ]
```

### Comparing `py-gcode-metadata-0.1.0/setup.py` & `py_gcode_metadata-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     """Return README.md content."""
     with open('README.md', 'r', encoding="utf-8") as readme:
         return readme.read().strip()
 
 
 setup(
     name='py-gcode-metadata',
-    version='0.1.0',
+    version='0.2.0dev',
     packages=['gcode_metadata'],
     url='https://github.com/prusa3d/gcode-metadata',
     license='LGPLv2+',
     author='Prusa Connect Developers',
     author_email='link@prusa3d.com',
     maintainer='Prusa Connect Developers',
     maintainer_email='link@prusa3d.com',
```

### Comparing `py-gcode-metadata-0.1.0/tests/gcodes/.fdn_filename.gcode.cache` & `py_gcode_metadata-0.2.0/tests/gcodes/.fdn_filename.gcode.cache`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('metadata', OrderedDict([('normal_percent_present', True), "*

 * *            "('normal_left_present', True), ('filament used [mm] per tool', [7003.4]), ('filament "*

 * *            "used [mm]', 7003.4), ('filament used [cm3] per tool', [16.8]), ('filament used "*

 * *            "[cm3]', 16.8), ('filament used [g] per tool', [21.4]), ('filament used [g]', 21.4), "*

 * *            "('filament cost per tool', [0.6]), ('filament cost', 0.6), ('estimated printing time "*

 * *            "(normal mode)', '2 […]*

```diff
@@ -1,9 +1,14 @@
 {
-    "data": {
+    "icon": {
+        "data": "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",
+        "format": "PNG",
+        "resolution": "220x124"
+    },
+    "metadata": {
         "bed_temperature": 90,
         "bed_temperature per tool": [
             90
         ],
         "brim_width": 0,
         "estimated printing time (normal mode)": "2h 9m 24s",
         "filament cost": 0.6,
@@ -37,12 +42,13 @@
         "printer_model": "MINI",
         "support_material": 0,
         "temperature": 240,
         "temperature per tool": [
             240
         ]
     },
-    "thumbnails": {
-        "16x16": "iVBORw0KGgoAAAANSUhEUgAAABAAAAAQCAYAAAAf8/9hAAABjUlEQVR4AbWQTUsCURSGZ2Wr3AVpVpYGIWJ+po7OOOM44zh+jSRJoOVHSkSLolW7fkAE0a5F7ou20S7oj/hT3jw3EKGyGmjg3MvMfZ/nzD0c9x/P4vycuxNzXVIVNhfa9B502iXaZ0IUvsh6hm/HCXxXJPpScFP1vc4Cp4v+7FP338LTxWCyWYEfWqERE5wK7qEVwWQe46X90o9ZEtDAOZvNZun+j60QHPY5iYvH47jaifwJfj6MoZncQCQSGXGiKEIVefRTHjzth3+Ge1Fc17agCDzS6TSYQJZllFQZZ6Ibw0YA97sB3NX9NOlJx1vTh962C+3EOnRFgiRJEAQBHC0kyOfzMA0N3ZgLzbATg8QyzjNrOEmtojsGD6JL6Ke9KOsqyxIzEZBNVVUUi0U0qkV0eQ+OkitMthd0sL3Le1GvGDAMg2VJkMlkPgR0jWw2y8ylUgm1Wg0dncdA9qMlh9DSEjBNk51RhrLE5HI5cNSdimyKokDTNNalXC4zqFKpMJC+0RnBlC0UCtB1He91MLXiB9IHtQAAAABJRU5ErkJggg==",
-        "220x124": "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"
+    "preview": {
+        "data": "iVBORw0KGgoAAAANSUhEUgAAANwAAAB8CAYAAAACRt5vAAAh/0lEQVR4Ae2d+XMU17XHVRVnK8dOYsBmR4h9FyABEtpBLAKxb9pgEIsQYLABY4xZjbfEy7PjeHneKMcVO7bj91zlGDt5lSJxJb/lL/Av/Cn39ed0n1ar1TPTs0oj3VN1araeme57z/d+zz3n3NtlZVasWLEylmTiAz8t3zx/QkK1zIoVK4WRyskPNn3es/ze9yfXmKC+vn3h3cPVU2+UWbFiJXeB1QBUGGhRCiA5FnCWWbFiJb5kAjQLPitWchDAhquYLdiiwGddTytWQpIrq2XKfvxfJueGwpioBm74HfSpllm3UYCN8h+oDe5YGZGCYUYFRYoFvmSAycd/WLfWyogRWANDLzbQiq0WdFaGVYrlPo4UhS0zcWGtWMmbYHjD4T6OBNCVWbFSDNGAw1hitShlflhmxUq+RIFFEESDEGORzVKpTU9YyViigFVKRj/catMFVoaI5p4052SBlV+1kUsrImMtgmhBZ2VYBTYrJaMtZbWRSytl1m0srtrI5RgW3MlSMlYLOislLdadHD4lKFVmZWyJdSeHV7WYuszK6BfrTo4szXQJkZUSE0LUpWSQY0Ut641Sse5kaQDPst4oEOtOlh74bHlYCYt1J0sXeNbdLEGx7uToAJ51N0tArDs5+sBnazRHsFh3cvSpTaKPYBkLm/iMNbVF0SNUrDs5OtXWZo5AGaub+YwFvbxulgXcSBILttGtNlUwgsSu5h792jZ/wo0yK8MrduuEsaP1Mx9KlFkZPsn3HWmsjmyd9OBPm8qsDI/Y+drY0jtHqy3ghkusCzn29Iue5eaBn95XXmaleGLna2MbcGVWiidj5RZQVqP1hbZ5tsqkWGLna1ZftIArjtgdt6yiR1dNs1UmhRZb8W9VdX/lJLtSoNBi2c2qatXUX94os1J4+SqxsqQMw2ph1O51UiQ5UzfjbikZhtXCqd1qoQiydNIDiU+6KkvKMKwWRu2K7yLJ0+tmlZRhWC2c2n1NiiAHq6bc/f2OhSVlGFYLo3abhSLIsskPJJ5qqTD/c2hFSRmH1cKoXYhaBLniuJW/3TKvpAzDauHUBlAKLE608t5lB3QfdywrKcOwWhi1AZQCizNZTlxdP9uca5hZUoZhtXBqAygFlmutsw1zuVfbF5SUYVgtjNoASoHl8Ybye7DchcaZ5ouDy0vKOKwWRm0ApYCyfMqDiRsbXJa7tXFOSRmG1cKpDaAUUJ5xgHZl/SxhuY8OLC0pw7BaGLU7MhdQzjXOvHfdm8s92VxRUoZhtXBqAygFEtzKm8Jysw1BlFIyCquFUwu4Aspzm+Ya5nIvbZ1fUkZhtTBqt18osBCtvLlhjnl716KSMgyr+dVvj1ab3+9cZCbb/SoLKyunPpiA5WzQZGyD7VxDuWlf+LANmBRDnt88l8RnSRmJ1fzoHQ9sncsn37O7MRdJjq2edvfrXrv9wljTN3YsNMfXTDN9jjbPGmfrKYslK6f+MvF/x1eVlLFYzV5hNcDmDLQCONitzErxxN5WeAyB7UiVOVtf7oMNdps34f5EmZXiiQXc2AWbZbciywMPPNC0o3bpvVIyHKuZ6+vbF5reVVMHgQ21aYAiyU9+8pPySZMm3Vi5cqXp31RdUsZjNb7Cagq2ow7YAFyfDZQUVwDbkiVL7gE29PI2C7jRCrbnnJRPb/UA2JTdDq8pN3NnTrOAK7QoqwX1w+7VJWVIVuOB7fTaGS7YhriS0037qvnS93PnzrXJ7kIIrObI7TDYLOBGp1LIcNgB25EA2AbYbeag/sfbYS5fZiU/Mm7cuEQU0FS/OmIBN9r0csssAVvYlTxRM9201qwwmzdvHmIHDMhlVrKXYGAkmfb19Zmbpw6WlDFZTa24k8nA1lM7x9TV1Zna2lqzadOmIfZg2S5LCQdGwtrQ0GCOHTtmtm/fbtauXWu2rV1u/nvPYvPdURtAKXXFnfTB5gEOsPXWVJiNa6sEcKr0fZR9MFCXWUkvcVitvb3dnDt3zjQ1NUmDa+N31y2UQlbckbd32+U6paovtM0LzdumC+D21y4YBDbVmpoas27duki2w57KrEQLjUPUKRnQ6uvrxYXs7OwcBLSgHm2YJ6B7rL7cXGqpMG/ZdXIlpbiTR1cNdSVht6j+DmpjY6Nlu7iSjtVozJs3b5rW1takYFM91jDfnG+caR53gHemboY5VTvd/H7nQlk3VUrGNxYVdzKcAgBwW2or0wJO2W7jxo1D7MemDzxJ50LSiLAa87U4DY4219WYE/WzBHQwHfV3gI6O4/lr2+3dd0aqBpfcKNh6aueKdxO3/xmQ169fbwMqYUkXGIHVrl69arZs2ZKW1VTpGHR9fY0A7kKTAzqH6R51mI5EKh3IhPxR5/l/bVtgvnFcmFIyyNGubAgVBNwRx5VscQZQ7de4oNNIJsG1Me9ixg33X7hwQUAXt4G1U1Tb6leZJxzAsW/lOXEvywV0/Q7o6FSqGA5WTREQvudEOEvJMEejfhFyJ+mXXbVLhvRrpqAb0+mDdKymgZG9e/fGZrUosKGMbtvqVsielRcdPefN62C7k46LyQhK2VDCAV33isnS0Z/aWxoPmw52J6eZnpo50odRfZsJ6NAophuVbBeHzVQJ8z/99NMS4s0EbFGAo4FVO9YulIjlxeaZfjDlbD3BFNfFZFSljKhn5RRRuz/K8Cj3iujzUgG9NTPNuvpavw9zBZwGVDZs2DB6Ayrp2CwcGEkkEhkDLR3YUNzS443zBXSw3RNNFXKrKwIqj4ZdTAdwvH/HRjSLqrS3shuP7Y5nEu7HfIBu1AZUgqy2ePFiM3v2bEaSSFZ74403zIEDB6RRcwVbGHCATfVUy0LDjRzVxRS2q3dTB/3iYk6TkiIe+ayUDLbUlbSNJrr31y70+ywV4LIFHd/bsWOHaWlpGWKPJVmPGS42Bmjjx483c+bMGXRxJ06cMM8884yAjUgkdJ9PdguCDWC3NKwV9iISBtsRUPGZjnydF8WE8Xh93W6fXhQlUgzQOpZPNgeqZkhfBfsunyynYCNXB+C2bdtW+mwXnrNVVlaaefPmDaqDxIXcvXu3aW5ultdtbW0COBo7LtPFZTd+U3VDU51ELQEdbHepOQQ8B3REM2E4Hu2OzvlVKkmYI3+4b4lhP1ECWdsWPWz2LJ1oOh2wrW+s8/sq3yxHbICBHZsLf1bSAZVUQRLqIJ944gm56PB8jcYFhICPBs8nu6H8J7qlqUYAxySdustLnot5IQC8Jz0gEmD58tCKkjLq4VYYC31v7xLzvqO3Ns3lPtzirssqAO+R+fKBykkSJT60eqbZ3LBG+icMuFxZjmOoUNq1a1fSwZyAStTcjoDKiK/HjAKchvu7urpSBkZoEEaiPXv2SCMla9Bs2E0BhyuxvaXW3Gh1Qfe0w3QYhICu0Y1kuu85QGxyX1vQDdW/eMB618lhXt8wx9xwlLbqclIsnY57eAggOaqLSI/5e5JMF7ARGUYPOmDbuXaZ3z/BPsuV5TieFSVxpyv8Vsm5mGHA0WC3bt2Si44TheSiAQV+NgsNo9guW3bjd1FAva9hudx5h1tdqXspARUninnNASI3e5T3W1wG/N/E2AYdAKOtqNw5smqa2bdsktmPOiwFU3Uun+QAabKkVnRrBK3276txy7R43eOBLUEqZpUDtrplfr+EQZcLy2E/zNEyDcbBdlHJ8hGZPgiCDXDBamgmFxx0Mbdu3SpApTO0YXNlNwUc2lm/WEZmgAeriYvpAIz3rg9iwArDXXpKCSD5UuZdr21fIMUBgMwH2jIFGiBzGe1w9eDdtU7UTJMgFIUGfHbIAVvCY75uB2x76iulH5IBLhuW4zvYTSoPKZ1SocL3RyzbhRPcNMq1a9fkwrPJrQWZDN+6p6dHRqyoxs6G3VB+V367dp6Ai9H7igMuAMbtjLnZo+92OmzHZ6+0j6370H3mBDgohwMkuIqDGW2yuIaAR7exY8GoRnoVaH01AzlOjqWcrmtVuTAb7a/9kSvLoRoY4Xeztbkw8EZcQAXEBxPcMNqTTz6ZUR1kOtDxW7iXuAh0Qj7YTQHHSJaomy+Au9rqupLPOhG0Z53JPsCD7eQzz8V8eQyATveDTHisBWBgOEL3PAKcRGB+dtyr7AdgpFcAKRFfnnOsVvGgLtgq/fZPB7g4LMdrBuSdO3dmlc9N52JG5eyKvsA1zGoaGNm/f39OrJZMNaBCFBOQ0AHpABcHbChu6+H6+cJmsB0h6+cDoLvpge6aB0jC2vk28r/0Vol+0lVpPukcnppOBZrumNUbiCwqyFy3ceogl5EyOcBF/vJsXbmf24TVAGjPCndu11ldbrY0r/XbPS7oUgGO48mt8f1821x44B82tguXbdEoLKXJpg4y04uWKKMTeWJiy/Nc3EkFG8oIeXDtPAEdy/xfdJTH59tc0F1tnSWpAvJzjOZ8FjZWVSrfP3BAqfpq+wJhSvkd5/cxSFIOGC85qN3oEtVH5D0M/RXne8UqqOa8cacJiOgmPkcD0cXglnXqLiqTnfFAhpJa8fb9F7AJ4Jw5HmBrW9/st3c2gAuCjue4j9iBej2FBJyyXVHrMcOsxknAaocPHy74xSrg1MVkfsh2C3RMFNjSAS7Ibgq4Xa0NEmnDmDAuRnSCBO0LHzab5k8wG+eNH6KA40Sgyh2DPCqs4BqpG/6eIqN9zwpGfFelsqLSDT7sdX5j37KJ8ojyPnOmjkpXu5xjn2isEOAWAmhU6vt5ssBuWeE9IZXNTgvIZkgR+OMeyDSlwmAE2LpWDACue80s09bqRp6DgFPQZepWcgzfhdmCbFcMG4RQkrmYeQ2ohPcc4eJffPFFmVsVktWiAKego1Pw25nbKfCycScxBBQQ79rmaMNKcaEIEOxc/Egk0IK62QFjh3MsQNXRH3fruDe/gTXUPUtUe8EDndN4easDXjACAGKkClTC5xLZC0T4MHpcvzs5LqC9vX+psNKx1V6ubM0AwIJAI7TPfz7qAU0ZGoDB+qRSzjug4/wUbAq4vWsXS8EDxem0r4IuW7eS71AOyLG5lnrlogVd4BrOrcFqjz32WN4nqHHBFpy70Tm4FYCOzsjWneT7VCMwajKI7G1cKfMSDIz5iOz6W+2CEFBQkhQG3pYFEyTAwJYOMq+pneEvpgSAfcp+3pKgwwomL7DQvXIgaRxcG9YX2MFKtx4Ql88BMgzz5s5F4sbGZrWj1VJtE9yKbjDABrY4UGVuBsiEzZpmyqoLgKZ1qTJHC4Ftd4O7aSsK6Pbt2+fXMmbqVvKc3+C3gq7lcIMOtzZvbBcV7gdsGGaxWC0d4FA6hGAKHaJzu7iA43hGTIyB31AD4Xl/yyLf8HiErY7J3Gaq7y72eCVKu5y5F2y41QHdDucx6H6d8pYBaci8z3PXAMxg19MFIL9/2ov2qZ4Kqf++gNudT1Exc2vjXPPO7sVJgSYLPQMrq4+HbgGl13pizXT/nFFWzV/wGI0CAXKTRG35X4AmYAsAbo8zYAXbk3bmkWkA9sPzuIADoPQtj7mWehXKNnMOqIQDI1ww4X4ao9hgSwc4dSXpMKKkjKJx5m9cE+VmClQ1CgwFZfTqa17k55kUGEGXsNtzCXVO5iaHJwoDYniw4xlPMc6TgTyVGvMxL0Bx1AMzBq9BCNWzgUeCFGfrdB41+Bg+cz8vFwDCfm/uWiRbBiozhtksyGTBPFpQARtAu+SBjeenvIR2T4DVaBPARttpOyrgUPUm+vv7/QR1MsDxmkGRPuW9bKtOisV2XGvGAZVkgRGSz8MBtLiAU9BpRzGS0ulBwOloSicyyhLtpJEwgmSA29m2UYwMgwZkJG67Q0Db7wFtrwM0Zbodix6R5x3LJwlAz0rI3AWIy1juXO+kN+frrx0of+K1BiH0ET3X6BZYu+q6d+cDz1Upv6KcigGA+eUmx90Vne+6vZyXuq59YaAF5qF6frxWZoPVcCUTVW7a4LCXo0Npn90O2ABSKsCp8hrPgv5Q0Gl/8ZqtNhgMM6k6GU775Lo559guZpjVMq2DHAmAk7VvgVpMgMX5K+DoZIBGsCXc+VGAoxH3bW6WShMMW0C30gWdBjkAG9HKXU5YX8Dm6DYnsrl1wcN+ES8hfwx3MBu580N1C096hk9wQhfKXtQaz2Z3m4iLXpBCNkhqqhgETJhNUw3bHcBHzTNVAR/uLxFYGPmgVwPZ7wHtVEB5zf/BmAwWBHCOeIzf6zGc5OlqKqS94gBO58/0Ax4JxyvL8R1WjvA80zKv4bBN7A3G/uCDD8yVK1fMwYMHxcZSLnANLxxlL0gWiQ7nqJEt4JTpcFfoUJTOxhC6u7v9+UMwQqlgiwIceqCtRZLi5KoABGBTlttfOZBDgz0EcI6xb104QVwtjJFgCUwI42nwQcEHUKQywwu04A7CJJe9UjNqPFFcuUui7sp13TYC8JJyADwAjf/nPLY6rzfPH582yupGWsfL9132c5fN4Ooq03HOnJumDdz558Dc83DNLLO9bWNSwCnogoBT1573jxw54nsdqLqVIx1wXMehQ4fMb37zG/Pxxx+bv/3tb+bNN98U/DBdiWI7Ybbgmy+88II5fvz4sLNaroBTV5JOP336tOno6JDOjkoJhAGHwQQBJ/O9reul6oQIHwbI/EfyZcsneW7lRGEXWG67AzhYDmBKvWH1VH+O1uOx5PmAi/h4AHi8pqLlqujsQapr+QAa/0/eToHG/+4J5PEADwMBx8DEOs8EUB1ePeQB77y1TpLv4xrzPU1VoBzv10N655/wqk64rs51q6SNgoBT0KUDHMpxMAM5XV5nW8hcLHvk3I4ePWpeffVV88knn0iK7J///Kf57LPPzB/+8AdZ9wkQeQyDruy+++4bBLjq6mr5MQyUyWCpAg6lIxkxZT7mMB2jTjYMhzEx2e/aVC8VI5R5aeBAI3MAD+N23UuXaTBmZQHdM0XzdRg5bKFb+D3muZk8h01VKaLWmk5cS8ALyFD3P1zm1LmU5vaCQARAWumv4fseAY0OBlP9O9Vwfsq4gIp5oMwFvUeYEwbnPw9UlZu9TVXSNmHAxWE4Hukf+gWXn89wMXlvpAKOayGuAcj++te/mq+//tq89tpr5p133jHvvfeeuJcEGNlChOOHAA5ZunSpiVo4ev78+aLm2/IFONhN5wJ0LEynyW0MQ/NBceZwQcCh3Q7oWMmsa+lgKmGuFVN88GkgBfC5OTO3JpF8HCF3jBpXkCoVQKmvz3pbPFz3QMaqBdxKgA3TYOi7PRbTQIVGS7sCyucCDA+UCjrOR11b/b4urSFBry4jv7nDmwfyfYDa5SXkdZcz8pIdDrNpu6QCXNQcjs8Y1Hk/GDShv3T1P++PFMDx+7DWp59+Ksz2+uuvC8i+/PJLYTnSSwRNKHNkOrYyyc4HAjgninIjvNEPWlVVJbeHokGHk+0yDZpQ2RAVpaQzeZ+G4ZrSRSmjACcjcnurFDfrKgICCgRVqBtk/uOWcU0WV0xD7xqO16JfAhCwGolkjB4w9EvOy913hUAIDCMgc8DS4bmnQbdOwTYIcF7ktN1jIpnTee6mlo7pEptun+ncnagVrB1BFqxy3UaNZmoZGGCjLbIBHN9jZb+CLRyl1EQ3xyjohhNweh2XL182//rXv8wPP/xg3n33XWE5AotMWSAngNiY5E4+gwCH3H///TemT58eeRCGeurUqWGb18UFnLoj2mnJ8nBSO+lM0hlhMZBMAYce2LJeopfXvbV0uJo8l1ssVQ/k7GAvvZNPsPwLt00rOHRbdk0toIBDy7wSgaqUYB6wJwA6wK7gg8F2Lh6Y17lzs4HFo9Ro6po2N/jjvb/cZTKNWsLcOjjIzmZr3Nybgi1TwPEa157cWrDaJFnim+ekePhNBV2xAcd5/u53vzPff/+9eeutt8zdu3fN7du3zZ07d8yNGzfEHQZsqVgtEnDIj370o/IJEybcZT/J8IHM7Z577rlhSROkA5zO1+JUmuhEHdBhGHQo7kC40iQYOMGYFHRqaIB7b9t6CdXjXrKC4LnNc8UNJD+GQeOeAbbgLbQwXrdyZZqfx8JN3ORFFDfNc3Nn7V7QZQjYBq0xm+zpYADy31oUrauzAVNHgNWUzfYtG2A0Qv693vYI7kBR7hcou5UwLth0YFPAafskC5hoeVdvb6+/LWImBcyas+P4YgMO++K8P/roI/OnP/1JgiN//vOfZdAguAgmuO44YBsCuCDbJXMxcdc4gWK6mKkAR4dhANnUUiro1IC0ljIV4BR0HIt2bW6QEP1vt8wTZWnPrU1zxM0EIFL54Rit5OMcELQtGLrywAXZBPkMJUHNHIzHNidQAfN1rpg82KWsCqjnYh7yazMHXExdj6af62e81h203JIyt4aSAYGVAAwaBIbOeGvbDq2p8MGm7RVkt2SA45FBTZdVZbtERwMsHK9MVyjAcS3ck5DgIc/5b675+vXr5tKlSxL2v3jxotx0Ji7QUgLOS4Q3TZ482USxHWuD8GfjbGlXSNDh4+tK8FxWC0jBsjOv4/doWAwnjlvJsZK83ep8f8089249je496Y5768IAkEb1BqKIk/w8XpBxtHIFgKHBfB/zOKKEuIl8potCE+pyejoQFdVVCtO8VdtTBvKCgbVuusbtUa8ShmuQzZOcxPppb9X2QQdsezav8xPVcd1JjiEAEgxS5bJaAMWFC66DyyfY1K5IUXz11Vfm3//+t7iPRB8JmHBOEA7ztrguZGzAqYv561//+m4ytmOySIMWg+2CjUtn4WJkuh4uCnAKOk2OkwvCxcSI4riVCjrmhAc3rJFK+sfrg6Cb5AcrdHV0f2AnK4y/17uTz8FAxLHDy6f1equvVQ/JOr2JEgyhWoTfTnh7i2hAQ1cX8HjIu0NQb2ARaXDpjZv7c+aRAM1hNHKAPPpM6oBt97YtPtjiuJModoGR6kLRZOvhogIm6VICfAcvSzcLygfgOE9Yi5UwXA+EwnyNKCSsBpsRQCQ6GbU0J46Co7I48vOf/zyRLKBCI509e7YogONCNbKoOzfna8W3gk5dTOpHAZGO3OlYTkG3b0urMAPztkfXDtylRyJ7XqRRtyGQgmbvTj59IfBpuL4/oqj4hFf3yO92eqxIsp3f5zc45ogk2d2o6aA7iwYKljmOuaXWSWrdqK6E6Fy3Wq5Jry8Ou/Fa2y4q/5aPFd/BVSL8Zy6pK62DfPbZZ83LL78shR/ffvutVI+88sorQipc55kzZyT/lg3Q2IG8oqLi3i9+8YsbZXElVUAFtmOnLhq4UGzX6K301h28ct2xK1nFiUbTMCpYVN3WOCynoNu9zWHKhkXCdKcDoMO1k6JnBxj9XpHyuYaB2kq9aaSCD3AEVw0Ajsf10XsefB9AwaTMFXFh3TV004asBDgZiJi6dZIVfi2mrP2rnSUDRxhsqdhN6k6d9iKYoGvXovJvubiTUQETHSSjtjFPp/wOkeqnnnpKSrJgMypFuMnMF198IQMHriMuZNTaNwXTlClT7j3yyCNmwYIFkZ9PnDjxHvgpy0YIqMycOTPyz2l0RoF8g063q6ZRs6k4ibvNQrjqROsvAR1GFxU8iXItBXSOS7W3eZWbAqib4dciEunToAevT2mxcuBWWnpXH9zSJ70CZtVLgaJmLWwml9fvJcfbpXDaDbzs9JLWGiABwLpCgfPhESaWVeqs96ubY3qal8u563UkA1uQ3XiPOTCuOK+TVZfkur1Csugkx+G+6krwODbFdTFX47oAFKF/SrHefvttYTfcRw2QxJ2XOV7g7SDQcCEzYrVUbAdqo9hu1apVwnb52FSIxqUTNRwcJx+XL5YLRisxvJMnT/oJ8ziupYJuZ/sW079uibiX7qrvaf42c2e8O7Lqejj/vgbeigKU2kndNeyalnxtcB85HuYaSFhP8mspdUvxgTndNH8ZEMuDjq0ZcEcld1ft5AG3tA4BWypXEuVzBiXaJl11Sb7ZLTh/41HK75ygSirQ8fuwMHO1f/zjH1KWRfE0czMq/ulvmA0Q5uJCgo+8gC0oqdIHnCxgyZbttHOCo1a4odOxnHZgLiynoKMzMSo6FAPMBHS7t281p1uXidvWLwtB3QDGOW9vEHc1dYWAAODpEh5cRS3xYjX3lXWzhQn7vGCIrmvT1ICmAg4GdkJ26yPdpUB6TzzKzDQCmqidbQ61NYgRZgI2HvkOLMHrdLWTcdkt7hZ5ySKUHK9lYWGb4n2qQajspxyLMqz333/f/PGPf5T3YTWS2NRB8ruZAm3ZsmXCag899NDdrF3IdKLpA/4sfAJcfKb1mFyoLqtvjNhQtpAsF4xYRoFOR3Q1TjXAZKBDmdcQSib62bOt1fRtrROwAQR1C5lDkbfTJTm81y8rqt0Ai+7L3+VvMDTV3ydSK1qCgRZYVMP9p72KFhhWAzdSslUzy3S3rvFBQ65Mrysd2LQQnMdkhcpxIpP5Yrcoz0jPg2P4Da6LSCMAoyzrP//5jxQfEyzRPVWJUmbCatg8On/+fMM0a/z48flntSjR9AF/HMV2XCgdlY7taBhYkQ5J1pipAJfNXC5VxDIKdMxR1I3SjYeiQMdndCJgY+KNQQvbebrHYb3O9Ws8N88FB0A5LIGVgdIsyryoj1Q3VBd+yq7I3vPewIqE46sHgKbbOwC+7oCb2UNezfn/4PngRqEMEJo7C4NNayDpI104GrUMJ9fIZDJ2yzTZrYuRKcFibvb3v/9dXEeeAzqq+hk46B/qIlPVQQIsplAKLodk7o0bN+7egw8+ePtnP/tZAuIpK7akqsfkwlm6kGxep3mvOMn0YrBcqqJmZTtARDVCmOkUkISUNeiirprvZirwnM92t9abA42Vfu7L3zavcnDt4z6vah9ABjds1T1XTnibF+E+HgsltyX1UD/H7G9Z7f938Jw4Z95jPgPjhQcTnnOufB6uKEm3sruY7BZlV59//rnUQRKFpIKEc9XrxAOjRCsKYAougPWrX/3qroLrxz/+cVPZSJF09ZhMRml8BZ7WQmpgJK7bWQiWyxR0GB7GSIQM8KlRMmICNNhCDTc8t4sEnsM6e5zI5v6q8iFlWOFt8454G86Km+nMw3rqFppOB7T7GyrlsavJ1W4e1y4Q9zEZ0IKRSJ4zVyWxrNfEd4jWaRVOIcGWD3YLf6YFyDAcfaUuJlsiwNZRCWrcQwhkRIErlaQKqMB0mlCkw7LZGz5blisE6DBS8jkYJYYK2HAnk+XqUgFPde+OdtPlgARXknwagRWY67gTuk84Ob4OwLWxwezcvF7AGtao34wCWlTYX3OQuFtcD66m5iILAbZ8shvHwlrPP/+8nBvv6f/DahRpoARM+CwcXZwxY0Zx5mGFkFQBFTrvww8/FMPMFGxRgMvGtcwWdGHgYawYKMyGe6JgC87rkgEvDL4wAEkr7GqqNvsccO3YtC4SSMk0/Lvh/40CmrqQHA/gGETUJU4WjcwGbLm4klGA4/t6nlwbLiSuJCVa5NUYOOgXWI2lZmF7JGmdU4J6pEiqekxcTAIqNFI26YN8upbZgE5zdMzjNIhCZ/MadywqihkEXhzwpWPCKGDFAVkyoOkclIGD5wyMGDJRVlxNLezOBmyFciU5hvP67rvvpCyLSCR5tpdeesl88803soQG4BH6D9dBZlV2lYP8Pz9x9iRvP6JDAAAAAElFTkSuQmCC",
+        "format": "PNG",
+        "resolution": "220x124"
     }
 }
```

### Comparing `py-gcode-metadata-0.1.0/tests/gcodes/.hidden_fdn_filename.gcode` & `py_gcode_metadata-0.2.0/tests/gcodes/.hidden_fdn_filename.gcode`

 * *Files identical despite different names*

### Comparing `py-gcode-metadata-0.1.0/tests/gcodes/fdn_filename.gcode` & `py_gcode_metadata-0.2.0/tests/gcodes/fdn_filename.gcode`

 * *Files identical despite different names*

### Comparing `py-gcode-metadata-0.1.0/tests/gcodes/fdn_filename_empty.gcode` & `py_gcode_metadata-0.2.0/tests/gcodes/fdn_filename_empty.gcode`

 * *Files identical despite different names*

### Comparing `py-gcode-metadata-0.1.0/tests/gcodes/fdn_full_0.15mm_PETG_MK3S_2h6m.gcode` & `py_gcode_metadata-0.2.0/tests/gcodes/fdn_full_0.15mm_PETG_MK3S_2h6m.gcode`

 * *Files identical despite different names*

### Comparing `py-gcode-metadata-0.1.0/tests/gcodes/full_m73_layers_0.2mm_PLA_MK3SMMU2S_11m.gcode` & `py_gcode_metadata-0.2.0/tests/gcodes/full_m73_layers_0.2mm_PLA_MK3SMMU2S_11m.gcode`

 * *Files identical despite different names*

### Comparing `py-gcode-metadata-0.1.0/tests/gcodes/pentagonal-hexecontahedron-1.sl1` & `py_gcode_metadata-0.2.0/tests/gcodes/pentagonal-hexecontahedron-1.sl1`

 * *Files identical despite different names*

### Comparing `py-gcode-metadata-0.1.0/tests/test_metadata.py` & `py_gcode_metadata-0.2.0/tests/test_metadata.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 """Tests for gcode-metadata tool for g-code files."""
+import json
 import os
 import tempfile
 import shutil
+from importlib.metadata import version
+
 import time
 import pytest
 
 from gcode_metadata import (get_metadata, UnknownGcodeFileType, MetaData,
                             get_meta_class)
 
 gcodes_dir = os.path.join(os.path.dirname(os.path.realpath(__file__)),
@@ -19,48 +22,57 @@
     """Temporary directory creation fixture"""
     # pylint: disable=consider-using-with
     temp = tempfile.TemporaryDirectory()
     yield temp.name
     del temp
 
 
+def chunk_read_file(meta_class, filepath, chunk_size=None):
+    """Util method which reads the file in chunk and call load_from_chunk
+    on the blocks of data from given meta_class."""
+    chunk_size = chunk_size or 10 * 1024  # 10 KiB test on small chunks
+    with open(filepath, 'rb') as file:
+        # find out file size
+        file_size = file.seek(0, os.SEEK_END)
+        file.seek(0)
+        while True:
+            chunk = file.read(chunk_size)
+            if not chunk:
+                break
+            meta_class.load_from_chunk(chunk, file_size)
+
+
+def give_cache_version(path, version_to_give):
+    """Modifies the cache file and adds a valid version number"""
+    with open(path, "r", encoding='utf-8') as cache_file:
+        cache = json.load(cache_file)
+    my_cache = {"version": version_to_give}
+    my_cache.update(cache)
+    with open(path, "w", encoding='utf-8') as cache_file:
+        json.dump(my_cache, cache_file)
+
+
 def test_get_metadata_file_does_not_exist():
     """Test get_metadata() with a non-existing file"""
     fname = '/somehwere/in/the/rainbow/my.gcode'
-    with pytest.raises(FileNotFoundError):
-        get_metadata(fname)
+    metadata = get_metadata(fname)
+    assert not metadata.data
 
 
 def test_save_cache_empty_file():
     """Test save-cache() with empty file"""
     fname = os.path.join(gcodes_dir, "fdn_all_empty.gcode")
     fn_cache = os.path.join(gcodes_dir, ".fdn_all_empty.gcode")
     meta = get_metadata(fname)
     meta.save_cache()
     with pytest.raises(FileNotFoundError):
         with open(fn_cache, "r", encoding='utf-8'):
             pass
 
 
-def test_save_load_and_compare_cache_file(tmp_dir):
-    """Test save-cache() with correct data"""
-    fname = os.path.join(gcodes_dir, "fdn_filename.gcode")
-    meta = get_metadata(fname)
-
-    temp_gcode = shutil.copy(fname, tmp_dir)
-    temp_meta = get_metadata(temp_gcode)
-    temp_meta.save_cache()
-
-    new_meta = MetaData(temp_gcode)
-    new_meta.load_cache()
-
-    assert meta.thumbnails == temp_meta.thumbnails == new_meta.thumbnails
-    assert meta.data == temp_meta.data == new_meta.data
-
-
 def test_load_cache_file_does_not_exist(tmp_dir):
     """Test load_cache() with a non-existing cache file"""
     with pytest.raises(ValueError):
         fname = os.path.join(gcodes_dir, "fdn_all_empty.gcode")
         temp_gcode = shutil.copy(fname, tmp_dir)
         MetaData(temp_gcode).load_cache()
 
@@ -68,60 +80,80 @@
 def test_load_cache_key_error():
     """test load_cache() with incorrect, or missing key"""
     fname = os.path.join(gcodes_dir, "fdn_filename_empty.gcode")
     with pytest.raises(ValueError):
         MetaData(fname).load_cache()
 
 
-def test_is_cache_fresh_fresher(tmp_dir):
-    """is_cache_fresh, when cache file is fresher, than original file"""
+def test_is_cache_recent_fresher(tmp_dir):
+    """is_cache_recent, when cache file is fresher, than original file"""
     fn_gcode = os.path.join(gcodes_dir, "fdn_filename.gcode")
     temp_gcode = shutil.copy(fn_gcode, tmp_dir)
     # Create the time difference
     time.sleep(0.01)
     fn_cache = os.path.join(gcodes_dir, ".fdn_filename.gcode.cache")
-    shutil.copy(fn_cache, tmp_dir)
-    assert MetaData(temp_gcode).is_cache_fresh()
+    cache_path = shutil.copy(fn_cache, tmp_dir)
+    assert MetaData(temp_gcode).is_cache_recent()
+    os.remove(cache_path)
+    os.remove(temp_gcode)
 
 
-def test_is_cache_fresh_older(tmp_dir):
-    """is_cache_fresh, when cache file is older, than original file"""
+def test_is_cache_recent_older(tmp_dir):
+    """is_cache_recent, when cache file is older, than original file"""
     fn_cache = os.path.join(gcodes_dir, ".fdn_filename.gcode.cache")
-    shutil.copy(fn_cache, tmp_dir)
+    cache_path = shutil.copy(fn_cache, tmp_dir)
     # Create the time difference
     time.sleep(0.01)
     fn_gcode = os.path.join(gcodes_dir, "fdn_filename.gcode")
     temp_gcode = shutil.copy(fn_gcode, tmp_dir)
-    assert MetaData(temp_gcode).is_cache_fresh() is False
+    assert MetaData(temp_gcode).is_cache_recent() is False
+    os.remove(cache_path)
+    os.remove(temp_gcode)
+
+
+def test_is_cache_correct_version_none():
+    """is_cache_correct_version, when cache file has no version"""
+    fn_gcode = os.path.join(gcodes_dir, "fdn_filename.gcode")
+    assert not MetaData(fn_gcode).is_cache_correct_version()
+
+
+def test_is_cache_correct_version_mismatch(tmp_dir):
+    """is_cache_correct_version, when cache file has different version"""
+    fn_cache = os.path.join(gcodes_dir, ".fdn_filename.gcode.cache")
+    fn_gcode = os.path.join(gcodes_dir, "fdn_filename.gcode")
+    temp_gcode = shutil.copy(fn_gcode, tmp_dir)
+    cache_path = shutil.copy(fn_cache, tmp_dir)
+    give_cache_version(cache_path, "0.0.0")
+    assert MetaData(temp_gcode).is_cache_correct_version() is False
+    os.remove(cache_path)
+    os.remove(temp_gcode)
+
+
+def test_is_cache_correct_version_match(tmp_dir):
+    """is_cache_correct_version, when cache file has the same version"""
+    fn_cache = os.path.join(gcodes_dir, ".fdn_filename.gcode.cache")
+    fn_gcode = os.path.join(gcodes_dir, "fdn_filename.gcode")
+    temp_gcode = shutil.copy(fn_gcode, tmp_dir)
+    cache_path = shutil.copy(fn_cache, tmp_dir)
+    give_cache_version(cache_path, version('py-gcode-metadata'))
+    assert MetaData(temp_gcode).is_cache_correct_version() is True
+    os.remove(cache_path)
+    os.remove(temp_gcode)
 
 
 def test_get_metadata_invalid_file():
     """Test get_metadata() with a file that has a wrong ending"""
     fname = tempfile.mkstemp()[1]
     with pytest.raises(UnknownGcodeFileType):
         get_metadata(fname)
 
 
 class TestFDNMetaData:
     """Tests for standard gcode metadata."""
 
-    def chunk_read_file(self, meta_class, filepath, chunk_size=None):
-        """Util method which reads the file in chunk and call load_from_chunk
-        on the blocks of data from given meta_class."""
-        chunk_size = chunk_size or 10 * 1024  # 10 KiB test on small chunks
-        with open(filepath, 'rb') as file:
-            # find out file size
-            file_size = file.seek(0, os.SEEK_END)
-            file.seek(0)
-            while True:
-                chunk = file.read(chunk_size)
-                if not chunk:
-                    break
-                meta_class.load_from_chunk(chunk, file_size)
-
     def test_full(self):
         """Both the file and filename contain metadata. There are thumbnails.
         """
         fname = os.path.join(gcodes_dir,
                              "fdn_full_0.15mm_PETG_MK3S_2h6m.gcode")
         meta = get_metadata(fname, False)
         assert meta.data == {
@@ -150,15 +182,15 @@
             'ironing': 0,
             'layer_info_present': True,
             'normal_left_present': True,
             'normal_percent_present': True,
             'quiet_left_present': True,
             'quiet_percent_present': True,
         }
-        assert len(meta.thumbnails['640x480']) == 158644
+        assert len(meta.thumbnails['640x480_PNG']) == 158644
 
     def test_m73_and_layer_info(self):
         """Tests an updated file with additional suppported info"""
         fname = os.path.join(gcodes_dir,
                              "full_m73_layers_0.2mm_PLA_MK3SMMU2S_11m.gcode")
         meta = get_metadata(fname, False)
         assert meta.data['estimated printing time (normal mode)'] == '10m 32s'
@@ -173,15 +205,15 @@
         assert meta.data['quiet_percent_present'] is True
         assert meta.data['quiet_left_present'] is True
         assert meta.data['layer_info_present'] is True
         assert meta.data['brim_width'] == 0
         assert meta.data['fill_density'] == '15%'
         assert meta.data['ironing'] == 0
         assert meta.data['support_material'] == 0
-        assert len(meta.thumbnails['160x120']) == 5616
+        assert len(meta.thumbnails['160x120_PNG']) == 5616
 
     def test_only_path(self):
         """Only the filename contains metadata. There are no thumbnails."""
         fname = os.path.join(gcodes_dir,
                              "fdn_only_filename_0.25mm_PETG_MK3S_2h9m.gcode")
         meta = get_metadata(fname, False)
         assert meta.data == {
@@ -218,15 +250,15 @@
     @pytest.mark.parametrize('chunk_size',
                              [10 * 1024, 20 * 1024 * 1024, 2 * 1024 * 1024])
     def test_from_chunks(self, chunk_size):
         """Test chunks from file read ok. Test on several chunk size."""
         fname = os.path.join(gcodes_dir,
                              "fdn_full_0.15mm_PETG_MK3S_2h6m.gcode")
         chunk_meta = get_meta_class(fname)
-        self.chunk_read_file(chunk_meta, fname, chunk_size)
+        chunk_read_file(chunk_meta, fname, chunk_size)
         # check that same result came from parsing metadata as a whole file
         meta = get_metadata(fname, False)
         assert meta.thumbnails == chunk_meta.thumbnails
         assert meta.data == chunk_meta.data
 
     def test_from_chunks_fake_data(self):
         """Test chunks fake file without metadata with string"""
@@ -239,30 +271,30 @@
         assert not chunk_meta.data
 
     def test_from_chunks_meta_only_path(self):
         """Test chunks from file with no metadata."""
         fname = os.path.join(gcodes_dir,
                              "fdn_only_filename_0.25mm_PETG_MK3S_2h9m.gcode")
         chunk_meta = get_meta_class(fname)
-        self.chunk_read_file(chunk_meta, fname)
+        chunk_read_file(chunk_meta, fname)
         assert chunk_meta.data == {}
         chunk_meta.load_from_path(fname)
         assert chunk_meta.data == {
             'estimated printing time (normal mode)': '2h9m',
             'filament_type': 'PETG',
             'printer_model': 'MK3S',
             'layer_height': 0.25,
         }
         assert not chunk_meta.thumbnails
 
     def test_from_chunks_empty_file(self):
         """Test chunks from file with no metadata."""
         fname = os.path.join(gcodes_dir, "fdn_all_empty.gcode")
         chunk_meta = get_meta_class(fname)
-        self.chunk_read_file(chunk_meta, fname)
+        chunk_read_file(chunk_meta, fname)
         assert chunk_meta.data == {}
 
     def test_from_chunks_invalid_file(self):
         """Test reading metadata as chunks invalid file."""
         fname = tempfile.mkstemp()[1]
         with pytest.raises(UnknownGcodeFileType):
             get_meta_class(fname)
@@ -287,17 +319,24 @@
             'min_initial_exposure_time': 1.0,
             'min_exposure_time': 1.0,
             'layer_height': 0.05,
             'materialName': 'Prusa Orange Tough @0.05',
             'fileCreationTimestamp': '2020-09-17 at 13:53:21 UTC'
         }
 
-        assert len(meta.thumbnails["400x400"]) == 19688
-        assert len(meta.thumbnails["800x480"]) == 64524
+        assert len(meta.thumbnails["400x400_PNG"]) == 19688
+        assert len(meta.thumbnails["800x480_PNG"]) == 64524
 
     def test_sl_empty_file(self):
         """Test a file that is empty"""
         fname = os.path.join(gcodes_dir, "empty.sl1")
         meta = get_metadata(fname, False)
 
         assert not meta.data
         assert not meta.thumbnails
+
+    def test_sl1_chunk_read(self):
+        """TODO For now when chunk reading sl file metadata are not loaded"""
+        fname = os.path.join(gcodes_dir, "empty.sl1")
+        chunk_meta = get_meta_class(fname)
+        chunk_read_file(chunk_meta, fname)
+        assert chunk_meta.data == {}
```

