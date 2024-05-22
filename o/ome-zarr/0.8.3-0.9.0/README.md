# Comparing `tmp/ome-zarr-0.8.3.tar.gz` & `tmp/ome-zarr-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ome-zarr-0.8.3.tar", last modified: Tue Nov 14 09:42:30 2023, max compression
+gzip compressed data, was "ome-zarr-0.9.0.tar", last modified: Wed May 22 09:15:23 2024, max compression
```

## Comparing `ome-zarr-0.8.3.tar` & `ome-zarr-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 09:42:30.996684 ome-zarr-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2023-11-14 09:42:29.000000 ome-zarr-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-11-14 09:42:29.000000 ome-zarr-0.8.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2023-11-14 09:42:30.996684 ome-zarr-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2023-11-14 09:42:29.000000 ome-zarr-0.8.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 09:42:30.992684 ome-zarr-0.8.3/ome_zarr/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-14 09:42:29.000000 ome-zarr-0.8.3/ome_zarr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4220 2023-11-14 09:42:29.000000 ome-zarr-0.8.3/ome_zarr/axes.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6079 2023-11-14 09:42:29.000000 ome-zarr-0.8.3/ome_zarr/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2023-11-14 09:42:29.000000 ome-zarr-0.8.3/ome_zarr/conversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2023-11-14 09:42:29.000000 ome-zarr-0.8.3/ome_zarr/csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     3445 2023-11-14 09:42:29.000000 ome-zarr-0.8.3/ome_zarr/dask_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5953 2023-11-14 09:42:29.000000 ome-zarr-0.8.3/ome_zarr/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11718 2023-11-14 09:42:29.000000 ome-zarr-0.8.3/ome_zarr/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     6477 2023-11-14 09:42:29.000000 ome-zarr-0.8.3/ome_zarr/io.py
--rw-r--r--   0 runner    (1001) docker     (127)    24028 2023-11-14 09:42:29.000000 ome-zarr-0.8.3/ome_zarr/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     9104 2023-11-14 09:42:29.000000 ome-zarr-0.8.3/ome_zarr/scale.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2023-11-14 09:42:29.000000 ome-zarr-0.8.3/ome_zarr/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2023-11-14 09:42:29.000000 ome-zarr-0.8.3/ome_zarr/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    33248 2023-11-14 09:42:29.000000 ome-zarr-0.8.3/ome_zarr/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-14 09:42:30.992684 ome-zarr-0.8.3/ome_zarr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2023-11-14 09:42:30.000000 ome-zarr-0.8.3/ome_zarr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2023-11-14 09:42:30.000000 ome-zarr-0.8.3/ome_zarr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-14 09:42:30.000000 ome-zarr-0.8.3/ome_zarr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2023-11-14 09:42:30.000000 ome-zarr-0.8.3/ome_zarr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2023-11-14 09:42:30.000000 ome-zarr-0.8.3/ome_zarr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-11-14 09:42:30.000000 ome-zarr-0.8.3/ome_zarr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-14 09:42:30.996684 ome-zarr-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2023-11-14 09:42:29.000000 ome-zarr-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:15:22.996597 ome-zarr-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-22 09:15:20.000000 ome-zarr-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-22 09:15:20.000000 ome-zarr-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-22 09:15:22.996597 ome-zarr-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-22 09:15:20.000000 ome-zarr-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:15:22.996597 ome-zarr-0.9.0/ome_zarr/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:15:20.000000 ome-zarr-0.9.0/ome_zarr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4221 2024-05-22 09:15:20.000000 ome-zarr-0.9.0/ome_zarr/axes.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6080 2024-05-22 09:15:20.000000 ome-zarr-0.9.0/ome_zarr/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-22 09:15:20.000000 ome-zarr-0.9.0/ome_zarr/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5359 2024-05-22 09:15:20.000000 ome-zarr-0.9.0/ome_zarr/csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-05-22 09:15:20.000000 ome-zarr-0.9.0/ome_zarr/dask_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6174 2024-05-22 09:15:20.000000 ome-zarr-0.9.0/ome_zarr/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-05-22 09:15:20.000000 ome-zarr-0.9.0/ome_zarr/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7124 2024-05-22 09:15:20.000000 ome-zarr-0.9.0/ome_zarr/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24113 2024-05-22 09:15:20.000000 ome-zarr-0.9.0/ome_zarr/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9268 2024-05-22 09:15:20.000000 ome-zarr-0.9.0/ome_zarr/scale.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-22 09:15:20.000000 ome-zarr-0.9.0/ome_zarr/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-05-22 09:15:20.000000 ome-zarr-0.9.0/ome_zarr/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34404 2024-05-22 09:15:20.000000 ome-zarr-0.9.0/ome_zarr/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:15:22.996597 ome-zarr-0.9.0/ome_zarr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-22 09:15:22.000000 ome-zarr-0.9.0/ome_zarr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-22 09:15:22.000000 ome-zarr-0.9.0/ome_zarr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 09:15:22.000000 ome-zarr-0.9.0/ome_zarr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-22 09:15:22.000000 ome-zarr-0.9.0/ome_zarr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-22 09:15:22.000000 ome-zarr-0.9.0/ome_zarr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 09:15:22.000000 ome-zarr-0.9.0/ome_zarr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 09:15:22.996597 ome-zarr-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-22 09:15:20.000000 ome-zarr-0.9.0/setup.py
```

### Comparing `ome-zarr-0.8.3/LICENSE` & `ome-zarr-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.8.3/PKG-INFO` & `ome-zarr-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ome-zarr
-Version: 0.8.3
+Version: 0.9.0
 Summary: Implementation of images in Zarr files.
 Home-page: https://github.com/ome/ome-zarr-py
 Author: The Open Microscopy Team
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -30,15 +30,15 @@
 Documentation
 -------------
 
 Documentation will be automatically built with `readthedocs`.
 
 It can be built locally with::
 
-    $ pip install sphinx
+    $ pip install -r docs/requirements.txt
     $ sphinx-build -b html docs/source/ docs/build/html
 
 Tests
 -----
 
 Tests can be run locally via `tox` with::
```

### Comparing `ome-zarr-0.8.3/README.rst` & `ome-zarr-0.9.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 Documentation
 -------------
 
 Documentation will be automatically built with `readthedocs`.
 
 It can be built locally with::
 
-    $ pip install sphinx
+    $ pip install -r docs/requirements.txt
     $ sphinx-build -b html docs/source/ docs/build/html
 
 Tests
 -----
 
 Tests can be run locally via `tox` with::
```

### Comparing `ome-zarr-0.8.3/ome_zarr/axes.py` & `ome-zarr-0.9.0/ome_zarr/axes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Axes class for validating and transforming axes
 """
+
 from typing import Any, Dict, List, Union
 
 from .format import CurrentFormat, Format
 
 KNOWN_AXES = {"x": "space", "y": "space", "z": "space", "c": "channel", "t": "time"}
```

### Comparing `ome-zarr-0.8.3/ome_zarr/cli.py` & `ome-zarr-0.9.0/ome_zarr/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Entrypoint for the `ome_zarr` command-line tool."""
+
 import argparse
 import logging
 import sys
 from typing import List, Union
 
 from .csv import csv_to_zarr
 from .data import astronaut, coins, create_zarr
```

### Comparing `ome-zarr-0.8.3/ome_zarr/conversions.py` & `ome-zarr-0.9.0/ome_zarr/conversions.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.8.3/ome_zarr/csv.py` & `ome-zarr-0.9.0/ome_zarr/csv.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.8.3/ome_zarr/dask_utils.py` & `ome-zarr-0.9.0/ome_zarr/dask_utils.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.8.3/ome_zarr/data.py` & `ome-zarr-0.9.0/ome_zarr/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Functions for generating synthetic data."""
+
 from random import randrange
 from typing import Callable, List, Optional, Tuple, Union
 
 import numpy as np
 import zarr
 from scipy.ndimage import zoom
 from skimage import data
@@ -132,46 +133,56 @@
         chunks = list(pyramid[-1].shape)
         # setting any z, c, t sizes to 1
         for zct in range(3):
             if zct + 2 < len(chunks):
                 chunks[zct] = 1
 
     storage_options = dict(chunks=tuple(chunks))
-    write_multiscale(pyramid, grp, axes=axes, storage_options=storage_options)
 
     if size_c == 1:
         image_data = {
-            "channels": [{"window": {"start": 0, "end": 255}, "color": "FF0000"}],
+            "channels": [
+                {
+                    "window": {"start": 0, "end": 255, "min": 0, "max": 255},
+                    "color": "FF0000",
+                }
+            ],
             "rdefs": {"model": "greyscale"},
         }
     else:
         image_data = {
             "channels": [
                 {
                     "color": "FF0000",
-                    "window": {"start": 0, "end": 255},
+                    "window": {"start": 0, "end": 255, "min": 0, "max": 255},
                     "label": "Red",
                     "active": True,
                 },
                 {
                     "color": "00FF00",
-                    "window": {"start": 0, "end": 255},
+                    "window": {"start": 0, "end": 255, "min": 0, "max": 255},
                     "label": "Green",
                     "active": True,
                 },
                 {
                     "color": "0000FF",
-                    "window": {"start": 0, "end": 255},
+                    "window": {"start": 0, "end": 255, "min": 0, "max": 255},
                     "label": "Blue",
                     "active": True,
                 },
             ],
             "rdefs": {"model": "color"},
         }
-    grp.attrs["omero"] = image_data
+    write_multiscale(
+        pyramid,
+        grp,
+        axes=axes,
+        storage_options=storage_options,
+        metadata={"omero": image_data},
+    )
 
     if labels:
         labels_grp = grp.create_group("labels")
         labels_grp.attrs["labels"] = [label_name]
 
         label_grp = labels_grp.create_group(label_name)
         if axes is not None:
```

### Comparing `ome-zarr-0.8.3/ome_zarr/format.py` & `ome-zarr-0.9.0/ome_zarr/format.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.8.3/ome_zarr/io.py` & `ome-zarr-0.9.0/ome_zarr/io.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,30 +24,37 @@
     data access.
 
     No assumptions about the existence of the given path string are made.
     Attempts are made to load various metadata files and cache them internally.
     """
 
     def __init__(
-        self, path: Union[Path, str], mode: str = "r", fmt: Format = CurrentFormat()
+        self,
+        path: Union[Path, str, FSStore],
+        mode: str = "r",
+        fmt: Format = CurrentFormat(),
     ) -> None:
         LOGGER.debug("ZarrLocation.__init__ path: %s, fmt: %s", path, fmt.version)
         self.__fmt = fmt
         self.__mode = mode
         if isinstance(path, Path):
             self.__path = str(path.resolve())
         elif isinstance(path, str):
             self.__path = path
+        elif isinstance(path, FSStore):
+            self.__path = path.path
         else:
             raise TypeError(f"not expecting: {type(path)}")
 
         loader = fmt
         if loader is None:
             loader = CurrentFormat()
-        self.__store = loader.init_store(self.__path, mode)
+        self.__store: FSStore = (
+            path if isinstance(path, FSStore) else loader.init_store(self.__path, mode)
+        )
 
         self.__init_metadata()
         detected = detect_format(self.__metadata, loader)
         LOGGER.debug("ZarrLocation.__init__ %s detected: %s", path, detected)
         if detected != fmt:
             LOGGER.warning(
                 "version mismatch: detected: %s, requested: %s", detected, fmt
@@ -108,15 +115,15 @@
         return dict(self.__metadata)
 
     def load(self, subpath: str = "") -> da.core.Array:
         """Use dask.array.from_zarr to load the subpath."""
         return da.from_zarr(self.__store, subpath)
 
     def __eq__(self, rhs: object) -> bool:
-        if type(self) != type(rhs):
+        if type(self) is not type(rhs):
             return False
         if not isinstance(rhs, ZarrLocation):
             return False
         return self.subpath() == rhs.subpath()
 
     def basename(self) -> str:
         """Return the last element of the underlying location.
@@ -155,35 +162,53 @@
             LOGGER.debug("JSON not found: %s", subpath)
             return {}
         except Exception:
             LOGGER.exception("Error while loading JSON")
             return {}
 
     def parts(self) -> List[str]:
-        if self.__store.fs.protocol == "file":
+        if self._isfile():
             return list(Path(self.__path).parts)
         else:
             return self.__path.split("/")
 
     def subpath(self, subpath: str = "") -> str:
-        if self.__store.fs.protocol == "file":
+        if self._isfile():
             filename = Path(self.__path) / subpath
             filename = filename.resolve()
             return str(filename)
-        if self.__store.fs.protocol in ["http", "https"]:
+        elif self._ishttp():
             url = str(self.__path)
             if not url.endswith("/"):
                 url = f"{url}/"
             return urljoin(url, subpath)
         else:
+            # Might require a warning
             if self.__path.endswith("/"):
                 return f"{self.__path}{subpath}"
             else:
                 return f"{self.__path}/{subpath}"
 
+    def _isfile(self) -> bool:
+        """
+        Return whether the current underlying implementation
+        points to a local file or not.
+        """
+        return self.__store.fs.protocol == "file" or self.__store.fs.protocol == (
+            "file",
+            "local",
+        )
+
+    def _ishttp(self) -> bool:
+        """
+        Return whether the current underlying implementation
+        points to a URL
+        """
+        return self.__store.fs.protocol in ["http", "https"]
+
 
 def parse_url(
     path: Union[Path, str], mode: str = "r", fmt: Format = CurrentFormat()
 ) -> Optional[ZarrLocation]:
     """Convert a path string or URL to a ZarrLocation subclass.
 
     >>> parse_url('does-not-exist')
```

### Comparing `ome-zarr-0.8.3/ome_zarr/reader.py` & `ome-zarr-0.9.0/ome_zarr/reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,18 +58,20 @@
             self.specs.append(Plate(self))
             # self.add(zarr, plate_labels=True)
         if Well.matches(zarr):
             self.specs.append(Well(self))
 
     @overload
     def first(self, spectype: Type["Well"]) -> Optional["Well"]:
+        # Handled by the generic case
         ...
 
     @overload
     def first(self, spectype: Type["Plate"]) -> Optional["Plate"]:
+        # Handled by the generic case
         ...
 
     def first(self, spectype: Type["Spec"]) -> Optional["Spec"]:
         for spec in self.specs:
             if isinstance(spec, spectype):
                 return spec
         return None
@@ -378,15 +380,15 @@
                     end = window.get("end", None)
                     if start is None or end is None:
                         # Disable contrast limits settings if one is missing
                         contrast_limits = None
                     elif contrast_limits is not None:
                         contrast_limits[idx] = [start, end]
 
-            node.metadata["name"] = names
+            node.metadata["channel_names"] = names
             node.metadata["visible"] = visibles
             node.metadata["contrast_limits"] = contrast_limits
             node.metadata["colormap"] = colormaps
 
         except Exception:
             LOGGER.exception("Failed to parse metadata")
```

### Comparing `ome-zarr-0.8.3/ome_zarr/scale.py` & `ome-zarr-0.9.0/ome_zarr/scale.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Module for downsampling numpy arrays via various methods.
 
 See the :class:`~ome_zarr.scale.Scaler` class for details.
 """
+
 import inspect
 import logging
 import os
 from collections.abc import MutableMapping
 from dataclasses import dataclass
 from typing import Any, Callable, Iterator, List, Tuple, Union
 
@@ -72,31 +73,37 @@
                 continue
             if name.startswith("_"):
                 continue
             yield name
 
     def scale(self, input_array: str, output_directory: str) -> None:
         """Perform downsampling to disk."""
-        func = getattr(self, self.method, None)
-        if not func:
-            raise Exception
+        func = self.func
 
         store = self.__check_store(output_directory)
         base = zarr.open_array(input_array)
         pyramid = func(base)
 
         if self.labeled:
             self.__assert_values(pyramid)
 
         grp = self.__create_group(store, base, pyramid)
 
         if self.copy_metadata:
             print(f"copying attribute keys: {list(base.attrs.keys())}")
             grp.attrs.update(base.attrs)
 
+    @property
+    def func(self) -> Callable[[np.ndarray], List[np.ndarray]]:
+        """Get downsample function."""
+        func = getattr(self, self.method, None)
+        if not func:
+            raise Exception
+        return func
+
     def __check_store(self, output_directory: str) -> MutableMapping:
         """Return a Zarr store if it doesn't already exist."""
         assert not os.path.exists(output_directory)
         loc = parse_url(output_directory, mode="w")
         assert loc
         return loc.store
```

### Comparing `ome-zarr-0.8.3/ome_zarr/utils.py` & `ome-zarr-0.9.0/ome_zarr/utils.py`

 * *Files identical despite different names*

### Comparing `ome-zarr-0.8.3/ome_zarr/writer.py` & `ome-zarr-0.9.0/ome_zarr/writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Image writer utility
 
 """
+
 import logging
 import warnings
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import dask.array as da
 import numpy as np
@@ -317,14 +318,37 @@
         if fmt.version in ("0.1", "0.2"):
             LOGGER.info("axes ignored for version 0.1 or 0.2")
             axes = None
         else:
             axes = _get_valid_axes(axes=axes, fmt=fmt)
             if axes is not None:
                 ndim = len(axes)
+    if (
+        isinstance(metadata, dict)
+        and metadata.get("metadata")
+        and isinstance(metadata["metadata"], dict)
+        and "omero" in metadata["metadata"]
+    ):
+        omero_metadata = metadata["metadata"].get("omero")
+        if omero_metadata is None:
+            raise KeyError("If `'omero'` is present, value cannot be `None`.")
+        for c in omero_metadata["channels"]:
+            if "color" in c:
+                if not isinstance(c["color"], str) or len(c["color"]) != 6:
+                    raise TypeError("`'color'` must be a hex code string.")
+            if "window" in c:
+                if not isinstance(c["window"], dict):
+                    raise TypeError("`'window'` must be a dict.")
+                for p in ["min", "max", "start", "end"]:
+                    if p not in c["window"]:
+                        raise KeyError(f"`'{p}'` not found in `'window'`.")
+                    if not isinstance(c["window"][p], (int, float)):
+                        raise TypeError(f"`'{p}'` must be an int or float.")
+
+        group.attrs["omero"] = omero_metadata
 
     # note: we construct the multiscale metadata via dict(), rather than {}
     # to avoid duplication of protected keys like 'version' in **metadata
     # (for {} this would silently over-write it, with dict() it explicitly fails)
     multiscales = [
         dict(
             version=fmt.version,
@@ -878,33 +902,32 @@
 
     if scaler is not None:
         if image.shape[-1] == 1 or image.shape[-2] == 1:
             raise ValueError(
                 "Can't downsample if size of x or y dimension is 1. "
                 "Shape: %s" % (image.shape,)
             )
-        mip = scaler.nearest(image)
+        mip = scaler.func(image)
     else:
         LOGGER.debug("disabling pyramid")
         mip = [image]
     return mip, axes
 
 
 def _retuple(
     chunks: Union[Tuple[Any, ...], int], shape: Tuple[Any, ...]
 ) -> Tuple[Any, ...]:
     """
     Expand chunks to match shape.
 
     E.g. if chunks is (64, 64) and shape is (3, 4, 5, 1028, 1028)
     return (3, 4, 5, 64, 64)
+
+    If chunks is an integer, it is applied to all dimensions, to match
+    the behaviour of zarr-python.
     """
 
-    _chunks: Tuple[Any, ...]
     if isinstance(chunks, int):
-        _chunks = (chunks,)
-    else:
-        _chunks = chunks
-
-    dims_to_add = len(shape) - len(_chunks)
+        return tuple([chunks] * len(shape))
 
-    return (*shape[:dims_to_add], *_chunks)
+    dims_to_add = len(shape) - len(chunks)
+    return (*shape[:dims_to_add], *chunks)
```

### Comparing `ome-zarr-0.8.3/ome_zarr.egg-info/PKG-INFO` & `ome-zarr-0.9.0/ome_zarr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ome-zarr
-Version: 0.8.3
+Version: 0.9.0
 Summary: Implementation of images in Zarr files.
 Home-page: https://github.com/ome/ome-zarr-py
 Author: The Open Microscopy Team
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -30,15 +30,15 @@
 Documentation
 -------------
 
 Documentation will be automatically built with `readthedocs`.
 
 It can be built locally with::
 
-    $ pip install sphinx
+    $ pip install -r docs/requirements.txt
     $ sphinx-build -b html docs/source/ docs/build/html
 
 Tests
 -----
 
 Tests can be run locally via `tox` with::
```

### Comparing `ome-zarr-0.8.3/setup.py` & `ome-zarr-0.9.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,25 +15,25 @@
 install_requires: List[List[str]] = []
 install_requires += (["dataclasses;python_version<'3.7'"],)
 install_requires += (["tifffile<2020.09.22;python_version<'3.7'"],)
 install_requires += (["numpy"],)
 install_requires += (["dask"],)
 install_requires += (["distributed"],)
 install_requires += (["zarr>=2.8.1"],)
-install_requires += (["fsspec[s3]>=0.8,!=2021.07.0,!=2023.09.0"],)
+install_requires += (["fsspec[s3]>=0.8,!=2021.07.0"],)
 # See https://github.com/fsspec/filesystem_spec/issues/819
 install_requires += (["aiohttp<4"],)
 install_requires += (["requests"],)
 install_requires += (["scikit-image"],)
 install_requires += (["toolz"],)
 
 
 setup(
     name="ome-zarr",
-    version="0.8.3",
+    version="0.9.0",
     author="The Open Microscopy Team",
     url="https://github.com/ome/ome-zarr-py",
     description="Implementation of images in Zarr files.",
     long_description=read("README.rst"),
     packages=["ome_zarr"],
     py_modules=["ome_zarr"],
     python_requires=">=3.6",
```

