# Comparing `tmp/dicebear-cli-1.1.0.tar.gz` & `tmp/dicebear-cli-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicebear-cli-1.1.0.tar", last modified: Tue May 21 21:53:12 2024, max compression
+gzip compressed data, was "dicebear-cli-1.1.1.tar", last modified: Tue May 21 22:11:26 2024, max compression
```

## Comparing `dicebear-cli-1.1.0.tar` & `dicebear-cli-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 21:53:12.959846 dicebear-cli-1.1.0/
--rw-rw-rw-   0        0        0     1095 2024-05-21 21:48:09.000000 dicebear-cli-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     4718 2024-05-21 21:53:12.958650 dicebear-cli-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2614 2024-05-21 21:46:54.000000 dicebear-cli-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 21:53:12.922216 dicebear-cli-1.1.0/dicebear_cli/
--rw-rw-rw-   0        0        0     1186 2024-05-21 21:28:51.000000 dicebear-cli-1.1.0/dicebear_cli/__init__.py
--rw-rw-rw-   0        0        0     3953 2024-05-21 21:50:47.000000 dicebear-cli-1.1.0/dicebear_cli/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:53:12.958650 dicebear-cli-1.1.0/dicebear_cli.egg-info/
--rw-rw-rw-   0        0        0     4718 2024-05-21 21:53:12.000000 dicebear-cli-1.1.0/dicebear_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2024-05-21 21:53:12.000000 dicebear-cli-1.1.0/dicebear_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 21:53:12.000000 dicebear-cli-1.1.0/dicebear_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-21 21:53:12.000000 dicebear-cli-1.1.0/dicebear_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2024-05-21 21:53:12.000000 dicebear-cli-1.1.0/dicebear_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-21 21:53:12.000000 dicebear-cli-1.1.0/dicebear_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-09-08 14:16:35.000000 dicebear-cli-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-21 21:53:12.959846 dicebear-cli-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     3943 2024-05-21 21:37:22.000000 dicebear-cli-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:26.309911 dicebear-cli-1.1.1/
+-rw-rw-rw-   0        0        0     1095 2024-05-21 21:48:09.000000 dicebear-cli-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     4667 2024-05-21 22:11:26.309911 dicebear-cli-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2614 2024-05-21 21:46:54.000000 dicebear-cli-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:26.289774 dicebear-cli-1.1.1/dicebear_cli/
+-rw-rw-rw-   0        0        0     1161 2024-05-21 22:11:03.000000 dicebear-cli-1.1.1/dicebear_cli/__init__.py
+-rw-rw-rw-   0        0        0     3908 2024-05-21 22:08:01.000000 dicebear-cli-1.1.1/dicebear_cli/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:26.308515 dicebear-cli-1.1.1/dicebear_cli.egg-info/
+-rw-rw-rw-   0        0        0     4667 2024-05-21 22:11:26.000000 dicebear-cli-1.1.1/dicebear_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-05-21 22:11:26.000000 dicebear-cli-1.1.1/dicebear_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 22:11:26.000000 dicebear-cli-1.1.1/dicebear_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-21 22:11:26.000000 dicebear-cli-1.1.1/dicebear_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2024-05-21 22:11:26.000000 dicebear-cli-1.1.1/dicebear_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-21 22:11:26.000000 dicebear-cli-1.1.1/dicebear_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-09-08 14:16:35.000000 dicebear-cli-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 22:11:26.309911 dicebear-cli-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     3851 2024-05-21 22:10:52.000000 dicebear-cli-1.1.1/setup.py
```

### Comparing `dicebear-cli-1.1.0/LICENSE` & `dicebear-cli-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dicebear-cli-1.1.0/PKG-INFO` & `dicebear-cli-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicebear-cli
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python CLI for DiceBear's avatar generating API.
 Home-page: https://github.com/jvherck/dicebear-cli
 Author: jvherck
 Author-email: jan@vhjan.me
 Maintainer: jvherck
 Maintainer-email: jan@vhjan.me
 License: MIT License
@@ -14,15 +14,14 @@
 Keywords: python,dicebear,avatar,avatars,generating,generation,generator,API,wrapper,image,images,picture,pictures,png,jpg,svg,json,cli,pillow,pil,requests,adventurer,adventurer-neutral,avataaars,avataaars-neutral,big-ears,big-ears-neutral,big-smile,bottts,bottts-neutral,croodles,croodles-neutral,fun-emoji,icons,identicon,initials,lorelei,lorelei-neutral,micah,miniavs,notionists,notionists-neutral,open-peeps,personas,pixel-art,pixel-art-neutral,shapes,thumbs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
```

### Comparing `dicebear-cli-1.1.0/README.md` & `dicebear-cli-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `dicebear-cli-1.1.0/dicebear_cli/__init__.py` & `dicebear-cli-1.1.1/dicebear_cli/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,9 +15,7 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
-
-__version__ = "1.1.0"
```

### Comparing `dicebear-cli-1.1.0/dicebear_cli/__main__.py` & `dicebear-cli-1.1.1/dicebear_cli/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,19 +21,16 @@
 # SOFTWARE.
 
 import click
 from string import ascii_letters, digits
 from random import choices
 from dicebear import *
 
-from __init__ import __version__
-
-
 @click.group()
-@click.version_option(__version__, "--version", "-v")
+@click.version_option(None, "--version", "-v")
 @click.help_option("--help", "-h")
 def cli(): pass
 
 
 @cli.command(name="create", help="Create one or more new avatars (no customising possible through CLI).")
 @click.argument("style", type=click.STRING, default=None, required=False)
 # help="The style of the avatar. All styles can be found on https://avatars.dicebear.com/styles or `DStyle.list`")
```

### Comparing `dicebear-cli-1.1.0/dicebear_cli.egg-info/PKG-INFO` & `dicebear-cli-1.1.1/dicebear_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicebear-cli
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python CLI for DiceBear's avatar generating API.
 Home-page: https://github.com/jvherck/dicebear-cli
 Author: jvherck
 Author-email: jan@vhjan.me
 Maintainer: jvherck
 Maintainer-email: jan@vhjan.me
 License: MIT License
@@ -14,15 +14,14 @@
 Keywords: python,dicebear,avatar,avatars,generating,generation,generator,API,wrapper,image,images,picture,pictures,png,jpg,svg,json,cli,pillow,pil,requests,adventurer,adventurer-neutral,avataaars,avataaars-neutral,big-ears,big-ears-neutral,big-smile,bottts,bottts-neutral,croodles,croodles-neutral,fun-emoji,icons,identicon,initials,lorelei,lorelei-neutral,micah,miniavs,notionists,notionists-neutral,open-peeps,personas,pixel-art,pixel-art-neutral,shapes,thumbs
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Other Audience
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
```

### Comparing `dicebear-cli-1.1.0/setup.py` & `dicebear-cli-1.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,21 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 from setuptools import setup, find_packages
-from dicebear_cli import __version__
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="dicebear-cli",
-    version=__version__,
+    version="1.1.1",
     license="MIT License",
     author="jvherck",
     author_email="jan@vhjan.me",
     maintainer="jvherck",
     maintainer_email="jan@vhjan.me",
     url="https://github.com/jvherck/dicebear-cli",
     project_urls={"Documentation": "https://github.com/jvherck/dicebear-cli/blob/main/README.md", "Source": "https://github.com/jvherck/dicebear-cli", "Tracker": "https://github.com/jvherck/dicebear-cli/issues"},
@@ -55,15 +54,14 @@
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Other Audience",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "Operating System :: Unix",
         "Operating System :: MacOS", # :: MacOS X
```

