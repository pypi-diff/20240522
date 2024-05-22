# Comparing `tmp/python_urlopen-0.0.1.3.tar.gz` & `tmp/python_urlopen-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_urlopen-0.0.1.3.tar", max compression
+gzip compressed data, was "python_urlopen-0.0.2.tar", max compression
```

## Comparing `python_urlopen-0.0.1.3.tar` & `python_urlopen-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_urlopen-0.0.1.3/LICENSE
--rw-r--r--   0        0        0     1279 2024-05-22 04:19:24.970192 python_urlopen-0.0.1.3/pyproject.toml
--rw-r--r--   0        0        0      839 2024-05-14 12:36:18.615669 python_urlopen-0.0.1.3/readme.md
--rwxr-xr-x   0        0        0     7264 2024-05-18 03:12:32.560748 python_urlopen-0.0.1.3/urlopen/__init__.py
--rwxr-xr-x   0        0        0     2471 2024-05-22 04:19:32.030634 python_urlopen-0.0.1.3/urlopen/__main__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_urlopen-0.0.1.3/urlopen/py.typed
--rw-r--r--   0        0        0     2023 1970-01-01 00:00:00.000000 python_urlopen-0.0.1.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_urlopen-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1277 2024-05-22 04:33:48.265466 python_urlopen-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      839 2024-05-14 12:36:18.615669 python_urlopen-0.0.2/readme.md
+-rwxr-xr-x   0        0        0     7264 2024-05-22 04:33:21.207997 python_urlopen-0.0.2/urlopen/__init__.py
+-rwxr-xr-x   0        0        0     2550 2024-05-22 04:32:31.992636 python_urlopen-0.0.2/urlopen/__main__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_urlopen-0.0.2/urlopen/py.typed
+-rw-r--r--   0        0        0     2021 1970-01-01 00:00:00.000000 python_urlopen-0.0.2/PKG-INFO
```

### Comparing `python_urlopen-0.0.1.3/LICENSE` & `python_urlopen-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_urlopen-0.0.1.3/pyproject.toml` & `python_urlopen-0.0.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-urlopen"
-version = "0.0.1.3"
+version = "0.0.2"
 description = "Python urlopen wrapper."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-urlopen"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-urlopen"
 keywords = ["urlopen"]
```

### Comparing `python_urlopen-0.0.1.3/readme.md` & `python_urlopen-0.0.2/readme.md`

 * *Files identical despite different names*

### Comparing `python_urlopen-0.0.1.3/urlopen/__init__.py` & `python_urlopen-0.0.2/urlopen/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 1)
+__version__ = (0, 0, 2)
 __all__ = ["urlopen", "download"]
 
 import errno
 
 from collections.abc import Callable, Generator, Mapping, Sequence
 from copy import copy
 from http.client import HTTPResponse
```

### Comparing `python_urlopen-0.0.1.3/urlopen/__main__.py` & `python_urlopen-0.0.2/urlopen/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,46 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__doc__ = "python url downloader"
+__doc__ = "python urlopen"
 
 from argparse import ArgumentParser, RawTextHelpFormatter
-
-parser = ArgumentParser(description=__doc__, formatter_class=RawTextHelpFormatter)
-parser.add_argument("url", nargs="?", help="URL to be downloaded")
-parser.add_argument("-o", "--output-file", help="file path to be downloaded, if omitted, print into stdout")
-parser.add_argument("-r", "--resume", action="store_true", help="skip downloaded data")
-parser.add_argument("-hs", "--headers", help="dictionary of HTTP Headers to send with")
-parser.add_argument("-v", "--version", action="store_true", help="print the current version")
-args = parser.parse_args()
-if args.version:
-    from urlopen import __version__
-    print(".".join(map(str, __version__)))
-    raise SystemExit(0)
-url = args.url
-if not url:
-    parser.parse_args(["-h"])
-
 from collections import deque
 from time import perf_counter
 
-from urlopen import download
+from . import download, __version__
+
+
+def parse_args():
+    parser = ArgumentParser(description=__doc__, formatter_class=RawTextHelpFormatter)
+
+    parser.add_argument("url", nargs="?", help="URL to be downloaded")
+    parser.add_argument("-o", "--output-file", help="file path to be downloaded, if omitted, print into stdout")
+    parser.add_argument("-r", "--resume", action="store_true", help="skip downloaded data")
+    parser.add_argument("-hs", "--headers", help="dictionary of HTTP Headers to send with")
+    parser.add_argument("-v", "--version", action="store_true", help="print the current version")
+
+    args = parser.parse_args()
+
+    if args.version:
+        print(".".join(map(str, __version__)))
+        raise SystemExit(0)
+
+    if not args.url:
+        parser.parse_args(["-h"])
+
 
 def headers_str_to_dict(headers: str, /) -> dict[str, str]:
     return dict(
         header.split(": ", 1) 
         for header in headers.strip("\n").split("\n")
     )
 
+
 def progress(total=None):
     dq: deque[tuple[int, float]] = deque(maxlen=64)
     read_num = 0
     dq.append((read_num, perf_counter()))
     while True:
         read_num += yield
         cur_t = perf_counter()
@@ -43,15 +48,19 @@
         if total:
             percentage = read_num / total * 100
             print(f"\r\x1b[K{read_num} / {total} | {speed:.2f} MB/s | {percentage:.2f} %", end="", flush=True)
         else:
             print(f"\r\x1b[K{read_num} | {speed:.2f} MB/s", end="", flush=True)
         dq.append((read_num, cur_t))
 
+
 def main():
+    args = parse_args()
+    url = args.url
+
     headers = args.headers
     if headers is not None:
         headers = headers_str_to_dict(headers)
 
     output_file = args.output_file
     if output_file:
         from os.path import dirname
@@ -68,14 +77,15 @@
             headers=headers, 
         )
     else: 
         from sys import stdout
 
         download(
             url, 
-            stdout, 
+            stdout.buffer, 
             headers=headers, 
         )
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `python_urlopen-0.0.1.3/PKG-INFO` & `python_urlopen-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-urlopen
-Version: 0.0.1.3
+Version: 0.0.2
 Summary: Python urlopen wrapper.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-urlopen
 License: MIT
 Keywords: urlopen
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

