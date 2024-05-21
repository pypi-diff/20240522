# Comparing `tmp/dicebear-cli-1.0.2.tar.gz` & `tmp/dicebear-cli-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicebear-cli-1.0.2.tar", last modified: Tue Jan 24 15:49:10 2023, max compression
+gzip compressed data, was "dicebear-cli-1.1.0.tar", last modified: Tue May 21 21:53:12 2024, max compression
```

## Comparing `dicebear-cli-1.0.2.tar` & `dicebear-cli-1.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-01-24 15:49:10.260849 dicebear-cli-1.0.2/
--rw-rw-rw-   0        0        0     1095 2022-09-08 14:16:35.000000 dicebear-cli-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     3170 2023-01-24 15:49:10.259870 dicebear-cli-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2285 2022-09-08 14:16:35.000000 dicebear-cli-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-01-24 15:49:10.247524 dicebear-cli-1.0.2/dicebear_cli/
--rw-rw-rw-   0        0        0     1161 2023-01-24 15:31:53.000000 dicebear-cli-1.0.2/dicebear_cli/__init__.py
--rw-rw-rw-   0        0        0     3672 2023-01-24 15:43:24.000000 dicebear-cli-1.0.2/dicebear_cli/__main__.py
-drwxrwxrwx   0        0        0        0 2023-01-24 15:49:10.257850 dicebear-cli-1.0.2/dicebear_cli.egg-info/
--rw-rw-rw-   0        0        0     3170 2023-01-24 15:49:10.000000 dicebear-cli-1.0.2/dicebear_cli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2023-01-24 15:49:10.000000 dicebear-cli-1.0.2/dicebear_cli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-24 15:49:10.000000 dicebear-cli-1.0.2/dicebear_cli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-01-24 15:49:10.000000 dicebear-cli-1.0.2/dicebear_cli.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       15 2023-01-24 15:49:10.000000 dicebear-cli-1.0.2/dicebear_cli.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-01-24 15:49:10.000000 dicebear-cli-1.0.2/dicebear_cli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2022-09-08 14:16:35.000000 dicebear-cli-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-01-24 15:49:10.260849 dicebear-cli-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2507 2023-01-24 15:48:36.000000 dicebear-cli-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:53:12.959846 dicebear-cli-1.1.0/
+-rw-rw-rw-   0        0        0     1095 2024-05-21 21:48:09.000000 dicebear-cli-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     4718 2024-05-21 21:53:12.958650 dicebear-cli-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2614 2024-05-21 21:46:54.000000 dicebear-cli-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 21:53:12.922216 dicebear-cli-1.1.0/dicebear_cli/
+-rw-rw-rw-   0        0        0     1186 2024-05-21 21:28:51.000000 dicebear-cli-1.1.0/dicebear_cli/__init__.py
+-rw-rw-rw-   0        0        0     3953 2024-05-21 21:50:47.000000 dicebear-cli-1.1.0/dicebear_cli/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:53:12.958650 dicebear-cli-1.1.0/dicebear_cli.egg-info/
+-rw-rw-rw-   0        0        0     4718 2024-05-21 21:53:12.000000 dicebear-cli-1.1.0/dicebear_cli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2024-05-21 21:53:12.000000 dicebear-cli-1.1.0/dicebear_cli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 21:53:12.000000 dicebear-cli-1.1.0/dicebear_cli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-21 21:53:12.000000 dicebear-cli-1.1.0/dicebear_cli.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       15 2024-05-21 21:53:12.000000 dicebear-cli-1.1.0/dicebear_cli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-21 21:53:12.000000 dicebear-cli-1.1.0/dicebear_cli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2022-09-08 14:16:35.000000 dicebear-cli-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 21:53:12.959846 dicebear-cli-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     3943 2024-05-21 21:37:22.000000 dicebear-cli-1.1.0/setup.py
```

### Comparing `dicebear-cli-1.0.2/LICENSE` & `dicebear-cli-1.1.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021 jvherck (on GitHub)
+Copyright (c) 2024 jvherck (on GitHub)
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `dicebear-cli-1.0.2/dicebear_cli/__init__.py` & `dicebear-cli-1.1.0/dicebear_cli/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022 jvherck (https://jvherck.github.io/dicebear/)
+# Copyright (c) 2024 jvherck (https://jvherck.github.io/dicebear/)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -15,7 +15,9 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+
+__version__ = "1.1.0"
```

### Comparing `dicebear-cli-1.0.2/dicebear_cli/__main__.py` & `dicebear-cli-1.1.0/dicebear_cli/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # MIT License
 #
-# Copyright (c) 2022 jvherck (https://jvherck.github.io/dicebear/)
+# Copyright (c) 2024 jvherck (on GitHub)
 #
 # Permission is hereby granted, free of charge, to any person obtaining a copy
 # of this software and associated documentation files (the "Software"), to deal
 # in the Software without restriction, including without limitation the rights
 # to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 # copies of the Software, and to permit persons to whom the Software is
 # furnished to do so, subject to the following conditions:
@@ -15,58 +15,70 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+
 import click
+from string import ascii_letters, digits
+from random import choices
 from dicebear import *
 
+from __init__ import __version__
+
 
 @click.group()
-@click.version_option(None, "--version", "-v")
+@click.version_option(__version__, "--version", "-v")
 @click.help_option("--help", "-h")
 def cli(): pass
 
 
 @cli.command(name="create", help="Create one or more new avatars (no customising possible through CLI).")
 @click.argument("style", type=click.STRING, default=None, required=False)
 # help="The style of the avatar. All styles can be found on https://avatars.dicebear.com/styles or `DStyle.list`")
 @click.option("--seed", "-s", show_default=True, type=click.STRING, default=None,
               help="The string to create the avatar (USE QUOTATION MARKS IF YOU WANT A MULTIPLE WORD SEED). Every unique string has their own unique avatar.")
 @click.option("--count", "-c", show_default=True, type=click.INT, default=1,
               help="The amount of avatars to make at once (they will all have the same style and seed if you add these to the command line, "
                    "leaving these options blank will create multiple random avatars.")
 @click.option("--format", "-f", show_default=True, type=click.STRING, default=DFormat.svg,
-              help="The format of the avatar. All formats can be found on https://github.com/jvherck/dicebear#formats or `DFormat.list`")
+              help="The format of the avatar. Get a list of all formats with `dicebear formats`.")
 @click.help_option("--help", "-h")
 def create(seed: str, style: str, count: int, format: str):
     avs = []
     try:
         if count > 1 and style and seed:
             click.echo("Both a style and seed have been given, generating multiple avatars just gives the same result. "
                        "(that's why only 1 is returned)")
             count = 1
         for _ in range(count):
+            if seed is None:
+                seed = "".join(choices(ascii_letters+digits, k=8))
             av = DAvatar(DStyle.random() if style is None else DStyle.from_str(str(style)), seed)
             if format == DFormat.svg: avs.append(av.url_svg)
             elif format == DFormat.png: avs.append(av.url_png)
             elif format == DFormat.jpg: avs.append(av.url_jpg)
             elif format == DFormat.json: avs.append(av.url_json)
             else:
-                log_error(ImageError("This format is not supported. Check https://github.com/jvherck/dicebear-cli#styles to see all supported formats."))
+                log_error(ImageError("This format is not supported. Use `dicebear formats` to see all supported formats."))
                 return
     except Error as e:
         log_error(e)
         return
     for x in avs: click.echo(x)
 
 
 @cli.command(name="styles", help="See a list of all available styles.")
 @click.help_option("--help", "-h")
 def styles():
-    for style in DStyle.list: click.echo(style)
+    for s in DStyle.list: click.echo(s)
+
+@cli.command(name="formats", help="See a list of all available formats.")
+@click.help_option("--help", "-h")
+def formats():
+    for f in DFormat.list: click.echo(f)
 
 
 if __name__ == '__main__':
     cli()
```

