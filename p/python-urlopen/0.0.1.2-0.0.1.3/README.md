# Comparing `tmp/python_urlopen-0.0.1.2.tar.gz` & `tmp/python_urlopen-0.0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_urlopen-0.0.1.2.tar", max compression
+gzip compressed data, was "python_urlopen-0.0.1.3.tar", max compression
```

## Comparing `python_urlopen-0.0.1.2.tar` & `python_urlopen-0.0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_urlopen-0.0.1.2/LICENSE
--rw-r--r--   0        0        0     1181 2024-05-18 03:16:36.702759 python_urlopen-0.0.1.2/pyproject.toml
--rw-r--r--   0        0        0      839 2024-05-14 12:36:18.615669 python_urlopen-0.0.1.2/readme.md
--rwxr-xr-x   0        0        0     7264 2024-05-18 03:12:32.560748 python_urlopen-0.0.1.2/urlopen/__init__.py
--rwxr-xr-x   0        0        0     2768 2024-05-14 12:33:59.520772 python_urlopen-0.0.1.2/urlopen/__main__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_urlopen-0.0.1.2/urlopen/py.typed
--rw-r--r--   0        0        0     2023 1970-01-01 00:00:00.000000 python_urlopen-0.0.1.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_urlopen-0.0.1.3/LICENSE
+-rw-r--r--   0        0        0     1279 2024-05-22 04:19:24.970192 python_urlopen-0.0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      839 2024-05-14 12:36:18.615669 python_urlopen-0.0.1.3/readme.md
+-rwxr-xr-x   0        0        0     7264 2024-05-18 03:12:32.560748 python_urlopen-0.0.1.3/urlopen/__init__.py
+-rwxr-xr-x   0        0        0     2471 2024-05-22 04:19:32.030634 python_urlopen-0.0.1.3/urlopen/__main__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_urlopen-0.0.1.3/urlopen/py.typed
+-rw-r--r--   0        0        0     2023 1970-01-01 00:00:00.000000 python_urlopen-0.0.1.3/PKG-INFO
```

### Comparing `python_urlopen-0.0.1.2/LICENSE` & `python_urlopen-0.0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python_urlopen-0.0.1.2/pyproject.toml` & `python_urlopen-0.0.1.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-urlopen"
-version = "0.0.1.2"
+version = "0.0.1.3"
 description = "Python urlopen wrapper."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-urlopen"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-urlopen"
 keywords = ["urlopen"]
@@ -26,13 +26,17 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 http_response = "*"
 python-filewrap = "*"
 
+[tool.poetry.scripts]
+python-urlopen = "urlopen.__main__:main"
+urlopen = "urlopen.__main__:main"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [[tool.poetry.packages]]
 include = "urlopen"
```

### Comparing `python_urlopen-0.0.1.2/readme.md` & `python_urlopen-0.0.1.3/readme.md`

 * *Files identical despite different names*

### Comparing `python_urlopen-0.0.1.2/urlopen/__init__.py` & `python_urlopen-0.0.1.3/urlopen/__init__.py`

 * *Files identical despite different names*

### Comparing `python_urlopen-0.0.1.2/urlopen/__main__.py` & `python_urlopen-0.0.1.3/urlopen/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,27 +3,29 @@
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
 __doc__ = "python url downloader"
 
 from argparse import ArgumentParser, RawTextHelpFormatter
 
 parser = ArgumentParser(description=__doc__, formatter_class=RawTextHelpFormatter)
-parser.add_argument("urls", nargs="*", metavar="url", help="URL(s) to be downloaded (one URL per line), if omitted, read from stdin")
-parser.add_argument("-d", "--savedir", default="", help="directory to the downloading files")
+parser.add_argument("url", nargs="?", help="URL to be downloaded")
+parser.add_argument("-o", "--output-file", help="file path to be downloaded, if omitted, print into stdout")
 parser.add_argument("-r", "--resume", action="store_true", help="skip downloaded data")
 parser.add_argument("-hs", "--headers", help="dictionary of HTTP Headers to send with")
 parser.add_argument("-v", "--version", action="store_true", help="print the current version")
 args = parser.parse_args()
 if args.version:
     from urlopen import __version__
     print(".".join(map(str, __version__)))
     raise SystemExit(0)
+url = args.url
+if not url:
+    parser.parse_args(["-h"])
 
 from collections import deque
-from os import makedirs
 from time import perf_counter
 
 from urlopen import download
 
 def headers_str_to_dict(headers: str, /) -> dict[str, str]:
     return dict(
         header.split(": ", 1) 
@@ -41,39 +43,39 @@
         if total:
             percentage = read_num / total * 100
             print(f"\r\x1b[K{read_num} / {total} | {speed:.2f} MB/s | {percentage:.2f} %", end="", flush=True)
         else:
             print(f"\r\x1b[K{read_num} | {speed:.2f} MB/s", end="", flush=True)
         dq.append((read_num, cur_t))
 
-urls = args.urls
-if not urls:
-    from sys import stdin
-    urls = (l.removesuffix("\n") for l in stdin)
-savedir = args.savedir
-if savedir:
-    makedirs(savedir, exist_ok=True)
-
-try:
+def main():
     headers = args.headers
     if headers is not None:
         headers = headers_str_to_dict(headers)
-    for url in urls:
-        if not url:
-            continue
-        try:
-            file = download(
-                url, 
-                savedir, 
-                resume=args.resume, 
-                make_reporthook=progress, 
-                headers=headers, 
-            )
-            print(f"\r\x1b[K\x1b[1;32mDOWNLOADED\x1b[0m \x1b[4;34m{url!r}\x1b[0m\n |_ ⏬ \x1b[4;34m{file!r}\x1b[0m")
-        except BaseException as e:
-            print(f"\r\x1b[K\x1b[1;31mERROR\x1b[0m \x1b[4;34m{url!r}\x1b[0m\n  |_ 🙅 \x1b[1;31m{type(e).__qualname__}\x1b[0m: {e}")
-except (EOFError, KeyboardInterrupt):
-    pass
-except BrokenPipeError:
-    from sys import stderr
-    stderr.close()
+
+    output_file = args.output_file
+    if output_file:
+        from os.path import dirname
+        dir_ = dirname(output_file)
+        if dir_:
+            from os import makedirs
+            makedirs(dir_, exist_ok=True)
+
+        download(
+            url, 
+            output_file, 
+            resume=args.resume, 
+            make_reporthook=progress, 
+            headers=headers, 
+        )
+    else: 
+        from sys import stdout
+
+        download(
+            url, 
+            stdout, 
+            headers=headers, 
+        )
+
+if __name__ == "__main__":
+    main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `python_urlopen-0.0.1.2/PKG-INFO` & `python_urlopen-0.0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-urlopen
-Version: 0.0.1.2
+Version: 0.0.1.3
 Summary: Python urlopen wrapper.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-urlopen
 License: MIT
 Keywords: urlopen
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

