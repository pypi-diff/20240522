# Comparing `tmp/rgbmatrixdriver-0.1.1.tar.gz` & `tmp/rgbmatrixdriver-0.1.2.tar.gz`

## Comparing `rgbmatrixdriver-0.1.1.tar` & `rgbmatrixdriver-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 rgbmatrixdriver-0.1.1/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 rgbmatrixdriver-0.1.1/LICENSE
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 rgbmatrixdriver-0.1.1/README.md
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 rgbmatrixdriver-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 rgbmatrixdriver-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 rgbmatrixdriver-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 rgbmatrixdriver-0.1.2/LICENSE
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 rgbmatrixdriver-0.1.2/README.md
+-rw-r--r--   0        0        0     1173 2020-02-02 00:00:00.000000 rgbmatrixdriver-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 rgbmatrixdriver-0.1.2/PKG-INFO
```

### Comparing `rgbmatrixdriver-0.1.1/LICENSE` & `rgbmatrixdriver-0.1.2/LICENSE`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-MIT License
-
-Copyright (c) 2021 Tyler Porter
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+MIT License
+
+Copyright (c) 2021 Tyler Porter
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `rgbmatrixdriver-0.1.1/pyproject.toml` & `rgbmatrixdriver-0.1.2/pyproject.toml`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-[build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[project]
-name = "RGBMatrixDriver"
-dynamic = ["version"]
-description = "A driver middleware for LED matrix software compatible with rpi-rgb-led-matrix"
-readme = "README.md"
-license = "MIT"
-authors = [
-    { name = "Tyler Porter", email = "tyler.b.porter@gmail.com" },
-]
-keywords = [
-    "LED",
-    "LED matrix",
-    "RPI",
-    "matrix",
-    "raspberry",
-    "raspberry pi",
-]
-classifiers = [
-    "Development Status :: 3 - Alpha",
-    "Environment :: Console",
-    "Intended Audience :: Developers",
-    "Intended Audience :: Other Audience",
-    "License :: OSI Approved :: MIT License",
-    "Natural Language :: English",
-    "Operating System :: OS Independent",
-    "Programming Language :: Python :: 3",
-    "Topic :: Other/Nonlisted Topic",
-]
-dependencies = [
-    "RGBMatrixEmulator"
-]
-
-[project.urls]
-Homepage = "https://github.com/ty-porter/RGBMatrixDriver"
-
-[tool.hatch.version]
-path = "RGBMatrixDriver/version.py"
-
-[tool.hatch.build.targets.wheel.shared-data]
-LICENSE = "docs/LICENSE"
-"README.md" = "docs/README.md"
-
-[tool.hatch.build.targets.sdist]
-include = [
-    "/rgbmatrixdriver",
-]
+[build-system]
+requires = ["hatchling"]
+build-backend = "hatchling.build"
+
+[project]
+name = "RGBMatrixDriver"
+dynamic = ["version"]
+description = "A driver middleware for LED matrix software compatible with rpi-rgb-led-matrix"
+readme = "README.md"
+license = "MIT"
+authors = [
+    { name = "Tyler Porter", email = "tyler.b.porter@gmail.com" },
+]
+keywords = [
+    "LED",
+    "LED matrix",
+    "RPI",
+    "matrix",
+    "raspberry",
+    "raspberry pi",
+]
+classifiers = [
+    "Development Status :: 3 - Alpha",
+    "Environment :: Console",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Other Audience",
+    "License :: OSI Approved :: MIT License",
+    "Natural Language :: English",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Topic :: Other/Nonlisted Topic",
+]
+dependencies = [
+    "RGBMatrixEmulator"
+]
+
+[project.urls]
+Homepage = "https://github.com/ty-porter/RGBMatrixDriver"
+
+[tool.hatch.version]
+path = "RGBMatrixDriver/version.py"
+
+[tool.hatch.build.targets.wheel.shared-data]
+LICENSE = "docs/LICENSE"
+"README.md" = "docs/README.md"
+
+[tool.hatch.build.targets.sdist]
+include = [
+    "/rgbmatrixdriver",
+]
```

### Comparing `rgbmatrixdriver-0.1.1/PKG-INFO` & `rgbmatrixdriver-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: RGBMatrixDriver
-Version: 0.1.1
+Version: 0.1.2
 Summary: A driver middleware for LED matrix software compatible with rpi-rgb-led-matrix
 Project-URL: Homepage, https://github.com/ty-porter/RGBMatrixDriver
 Author-email: Tyler Porter <tyler.b.porter@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: LED,LED matrix,RPI,matrix,raspberry,raspberry pi
 Classifier: Development Status :: 3 - Alpha
```

