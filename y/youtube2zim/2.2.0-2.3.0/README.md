# Comparing `tmp/youtube2zim-2.2.0.tar.gz` & `tmp/youtube2zim-2.3.0.tar.gz`

## Comparing `youtube2zim-2.2.0.tar` & `youtube2zim-2.3.0.tar`

### file list

```diff
@@ -1,44 +1,43 @@
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     6790 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/CHANGELOG
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/Dockerfile
--rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/entrypoint.sh
--rwxr-xr-x   0        0        0     2169 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/get_js_deps.sh
--rw-r--r--   0        0        0     3368 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/tasks.py
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/contrib/reencode_low_quality.py
--rw-r--r--   0        0        0    10975 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/contrib/video_encoding_tester.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/__about__.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/__main__.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/constants.py
--rwxr-xr-x   0        0        0     6180 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/entrypoint.py
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/processing.py
--rw-r--r--   0        0        0    37947 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/scraper.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/utils.py
--rw-r--r--   0        0        0    12262 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/youtube.py
--rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/locale/fr/LC_MESSAGES/messages.po
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/playlists/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/playlists/__main__.py
--rw-r--r--   0        0        0     3258 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/playlists/entrypoint.py
--rw-r--r--   0        0        0     7366 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/playlists/scraper.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/templates/article.html
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/templates/home.html
--rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/templates/assets/app.js
--rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/templates/assets/article.css
--rw-r--r--   0        0        0   300137 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/templates/assets/banner.jpg
--rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/templates/assets/db.js
--rw-r--r--   0        0        0     8046 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/templates/assets/home.css
--rw-r--r--   0        0        0    28658 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/templates/assets/sample.jpg
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/templates/assets/webp-trigger.js
--rwxr-xr-x   0        0        0   142472 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/templates/assets/font/Roboto-Black.ttf
--rwxr-xr-x   0        0        0   135820 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/templates/assets/font/Roboto-Bold.ttf
--rwxr-xr-x   0        0        0   140276 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/templates/assets/font/Roboto-Light.ttf
--rwxr-xr-x   0        0        0   145932 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/templates/assets/font/Roboto-LightItalic.ttf
--rwxr-xr-x   0        0        0   145348 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/src/youtube2zim/templates/assets/font/Roboto-Regular.ttf
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/tests/test_dummy.py
--rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/LICENSE
--rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/README.md
--rw-r--r--   0        0        0     1181 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/hatch_build.py
--rw-r--r--   0        0        0     5914 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     7404 2020-02-02 00:00:00.000000 youtube2zim-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     7397 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/CHANGELOG
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/Dockerfile
+-rwxr-xr-x   0        0        0       84 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/entrypoint.sh
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/openzim.toml
+-rw-r--r--   0        0        0     3374 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/tasks.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/contrib/reencode_low_quality.py
+-rw-r--r--   0        0        0    10975 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/contrib/video_encoding_tester.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/__about__.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/__main__.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/constants.py
+-rwxr-xr-x   0        0        0     6475 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/entrypoint.py
+-rw-r--r--   0        0        0     2423 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/processing.py
+-rw-r--r--   0        0        0    39385 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/scraper.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/utils.py
+-rw-r--r--   0        0        0    12262 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/youtube.py
+-rw-r--r--   0        0        0      982 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/locale/fr/LC_MESSAGES/messages.po
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/playlists/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/playlists/__main__.py
+-rw-r--r--   0        0        0     3664 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/playlists/entrypoint.py
+-rw-r--r--   0        0        0     7663 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/playlists/scraper.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/templates/article.html
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/templates/home.html
+-rw-r--r--   0        0        0     5594 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/templates/assets/app.js
+-rw-r--r--   0        0        0     2015 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/templates/assets/article.css
+-rw-r--r--   0        0        0   300137 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/templates/assets/banner.jpg
+-rw-r--r--   0        0        0     3003 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/templates/assets/db.js
+-rw-r--r--   0        0        0     8046 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/templates/assets/home.css
+-rw-r--r--   0        0        0    28658 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/templates/assets/sample.jpg
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/templates/assets/webp-trigger.js
+-rwxr-xr-x   0        0        0   142472 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/templates/assets/font/Roboto-Black.ttf
+-rwxr-xr-x   0        0        0   135820 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/templates/assets/font/Roboto-Bold.ttf
+-rwxr-xr-x   0        0        0   140276 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/templates/assets/font/Roboto-Light.ttf
+-rwxr-xr-x   0        0        0   145932 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/templates/assets/font/Roboto-LightItalic.ttf
+-rwxr-xr-x   0        0        0   145348 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/src/youtube2zim/templates/assets/font/Roboto-Regular.ttf
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/tests/test_dummy.py
+-rw-r--r--   0        0        0     7788 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/LICENSE
+-rw-r--r--   0        0        0     6231 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/README.md
+-rw-r--r--   0        0        0     5677 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     7850 2020-02-02 00:00:00.000000 youtube2zim-2.3.0/PKG-INFO
```

### Comparing `youtube2zim-2.2.0/.pre-commit-config.yaml` & `youtube2zim-2.3.0/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.4.0
+  rev: v4.5.0
   hooks:
   -   id: trailing-whitespace
   -   id: end-of-file-fixer
 - repo: https://github.com/psf/black
-  rev: "23.7.0"
+  rev: "24.4.2"
   hooks:
   -   id: black
 - repo: https://github.com/astral-sh/ruff-pre-commit
-  rev: v0.0.282
+  rev: v0.4.4
   hooks:
   - id: ruff
 - repo: https://github.com/RobertCraigie/pyright-python
-  rev: v1.1.331
+  rev: v1.1.363
   hooks:
   - id: pyright
     name: pyright (system)
     description: 'pyright static type checker'
     entry: pyright
     language: system
     'types_or': [python, pyi]
```

### Comparing `youtube2zim-2.2.0/CHANGELOG` & `youtube2zim-2.3.0/CHANGELOG`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,41 @@
 ## Changelog
 
 All notable changes to this project are documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html) (as of version 2.1.15).
 
+## [2.3.0] - 2024-05-22
+
+### Added
+
+- New `long_description` CLI argument to set the ZIM long description
+- New `disable_metadata_check` CLI argument to disable the metadata checks which are automated since zimscraperlib 3.x
+
+### Changed
+
+- Changed default publisher metadata to 'openZIM'
+- Validate ZIM metadata (tags, title, description, long_description) as early as possible
+- Migrate to zimscraperlib 3.3.2 (including **new VideoLowWebm encoder preset version 2**)
+- Upgrade Python dependencies, including migration to Python 3.12
+
 ## [2.2.0] - 2023-11-17
 
 ### Changed
 
 - Using zimscraperlib 2.0.0 (#171)
 - Using python 3.10 + debian bookworm (dropped support for older Python versions) (#180)
 - Adopt Python bootstrap conventions (including hatch) (#180)
 
 ### Fixed
 
 - Fixed local path media (profile, banner) not working (#178)
 - Unset `metadata_from` in `youtube2zim-playlists` (#185)
+- Do not move local banner and profile images, copy them instead #179
 
 ## [2.1.18] - 2022-11-09
 
 ### Changed
 
 - Switched to yt-dlp instead of youtube_dl
 - Added fallback for subtitle languages with IDs-like suffixes (#161)
```

### Comparing `youtube2zim-2.2.0/CONTRIBUTING.md` & `youtube2zim-2.3.0/CONTRIBUTING.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,40 +1,13 @@
 # youtube2zim devel
 
 
 ## setup
 
-__Note__: make sure you've installed non-python dependencies first, as mentioned in the [README](README.md).
-
-Then, setup a python `virtualenv` using `python 3.8+` and install our python dependencies using `pip`:
-
-```bash
-curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
-python get-pip.py  # you may use sudo
-pip install -U virtualenv  # sudo to install globally
-virtualenv -p python3.6 youtube-env
-source youtube-env/bin/activate
-pip install -r requirements.txt
-```
-
-You now have an isolated python installation in the `./youtube-env/` folder, containing all the python dependencies.
-
-__Note__: you must activate the `virtualenv` before running the scraper so it uses this virtual python installation
-
-``` bash
-source youtube-venv/bin/activate
-```
-
-and then run it:
-
-``` bash
-python youtube2zim --help
-# or, without activating the virtualenv:
-youtube-env/bin/python youtube2zim --help
-```
+See [README](README.md) for details about how to install with hatch virtualenv.
 
 ## contributions
 
 * Open issues, bug reports and send PRs [on github](https://github.com/openzim/youtube).
 * Make sure it's `py3.6+` compatible.
 * Use [black](https://github.com/psf/black) code formatting.
```

### Comparing `youtube2zim-2.2.0/Dockerfile` & `youtube2zim-2.3.0/Dockerfile`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM python:3.10-bookworm
+FROM python:3.12-bookworm
 LABEL org.opencontainers.image.source https://github.com/openzim/youtube
 
 # Install necessary packages
 RUN apt-get update \
  && apt-get install -y --no-install-recommends \
       locales-all \
       wget \
@@ -16,15 +16,15 @@
 # Custom entrypoint
 COPY entrypoint.sh /usr/local/bin/entrypoint.sh
 ENTRYPOINT ["entrypoint.sh"]
 RUN mkdir -p /output
 WORKDIR /output
 
 # Copy pyproject.toml and its dependencies
-COPY pyproject.toml README.md get_js_deps.sh hatch_build.py /src/
+COPY pyproject.toml README.md openzim.toml /src/
 COPY src/youtube2zim/__about__.py /src/src/youtube2zim/__about__.py
 
 # Install Python dependencies
 RUN pip install --no-cache-dir /src
 
 # Copy code + associated artifacts
 COPY src /src/src
```

### Comparing `youtube2zim-2.2.0/tasks.py` & `youtube2zim-2.3.0/tasks.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     ctx.run(f"black {args}", pty=use_pty)
 
 
 @task(optional=["args"], help={"args": "ruff additional arguments"})
 def fix_ruff(ctx: Context, args: str = "."):
     """fix all ruff rules"""
     args = args or "."  # needed for hatch script
-    ctx.run(f"ruff --fix {args}", pty=use_pty)
+    ctx.run(f"ruff check --fix {args}", pty=use_pty)
 
 
 @task(
     optional=["args"],
     help={
         "args": "linting tools (black, ruff) additional arguments, typically a path",
     },
```

### Comparing `youtube2zim-2.2.0/contrib/reencode_low_quality.py` & `youtube2zim-2.3.0/contrib/reencode_low_quality.py`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/contrib/video_encoding_tester.py` & `youtube2zim-2.3.0/contrib/video_encoding_tester.py`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/src/youtube2zim/constants.py` & `youtube2zim-2.3.0/src/youtube2zim/constants.py`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/src/youtube2zim/entrypoint.py` & `youtube2zim-2.3.0/src/youtube2zim/entrypoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,15 @@
 #!/usr/bin/env python3
 # vim: ai ts=4 sts=4 et sw=4 nu
 
 import argparse
 import logging
 import sys
 
-from youtube2zim.constants import (
-    CHANNEL,
-    NAME,
-    PLAYLIST,
-    SCRAPER,
-    USER,
-    logger,
-)
+from youtube2zim.constants import CHANNEL, NAME, PLAYLIST, SCRAPER, USER, logger
 from youtube2zim.scraper import Youtube2Zim
 
 
 def main():
     parser = argparse.ArgumentParser(
         prog=NAME,
         description="Scraper to create a ZIM file from a Youtube Channel or Playlists",
@@ -120,20 +113,25 @@
     parser.add_argument(
         "--description",
         help="Custom description for your project and ZIM. "
         "Default to Channel name (of first video if playlists)",
     )
 
     parser.add_argument(
+        "--long-description",
+        help="Custom long description for your ZIM.",
+    )
+
+    parser.add_argument(
         "--creator",
         help="Name of content creator. Defaults to Channel name or “Youtue Channels”",
     )
 
     parser.add_argument(
-        "--publisher", help="Custom publisher name (ZIM metadata)", default="Kiwix"
+        "--publisher", help="Custom publisher name (ZIM metadata)", default="openZIM"
     )
 
     parser.add_argument(
         "--tags",
         help="List of comma-separated Tags for the ZIM file. "
         "_videos:yes added automatically",
         default="youtube",
@@ -188,14 +186,21 @@
         "--version",
         help="Display scraper version and exit",
         action="version",
         version=SCRAPER,
     )
 
     parser.add_argument(
+        "--disable-metadata-checks",
+        help="Disable validity checks of metadata according to openZIM conventions",
+        action="store_true",
+        default=False,
+    )
+
+    parser.add_argument(
         "--dateafter",
         help="Custom filter to download videos uploaded on or after specified date. "
         "Format: YYYYMMDD or (now|today)[+-][0-9](day|week|month|year)(s)?",
     )
 
     parser.add_argument(
         "--optimization-cache",
```

### Comparing `youtube2zim-2.2.0/src/youtube2zim/processing.py` & `youtube2zim-2.3.0/src/youtube2zim/processing.py`

 * *Files 11% similar despite different names*

```diff
@@ -54,10 +54,19 @@
 
     # don't reencode if not requesting low-quality and received wanted format
     if not low_quality and src_path.suffix[1:] == video_format:
         return
 
     dst_path = src_path.with_name(f"video.{video_format}")
     logger.info(f"Reencode video to {dst_path}")
-    reencode(
-        src_path, dst_path, preset.to_ffmpeg_args(), delete_src=True, failsafe=False
-    )
+    success, process = reencode(
+        src_path,
+        dst_path,
+        preset.to_ffmpeg_args(),
+        delete_src=True,
+        with_process=True,
+        failsafe=True,
+    )  # pyright: ignore[reportGeneralTypeIssues]
+    if not success:
+        if process:
+            logger.error(process.stdout)
+        raise Exception(f"Exception while re-encoding {src_path} for {video_id}")
```

### Comparing `youtube2zim-2.2.0/src/youtube2zim/scraper.py` & `youtube2zim-2.3.0/src/youtube2zim/scraper.py`

 * *Files 5% similar despite different names*

```diff
@@ -25,19 +25,27 @@
 from babel.dates import format_date
 from dateutil import parser as dt_parser
 from kiwixstorage import KiwixStorage
 from pif import get_public_ip
 from zimscraperlib.download import stream_file
 from zimscraperlib.fix_ogvjs_dist import fix_source_dir
 from zimscraperlib.i18n import NotFound, get_language_details, setlocale
+from zimscraperlib.image.convertion import convert_image
 from zimscraperlib.image.presets import WebpHigh
 from zimscraperlib.image.probing import get_colors, is_hex_color
 from zimscraperlib.image.transformation import resize_image
+from zimscraperlib.inputs import compute_descriptions
 from zimscraperlib.video.presets import VideoMp4Low, VideoWebmLow
 from zimscraperlib.zim import make_zim_file
+from zimscraperlib.zim.metadata import (
+    validate_description,
+    validate_longdescription,
+    validate_tags,
+    validate_title,
+)
 
 from youtube2zim.constants import (
     CHANNEL,
     PLAYLIST,
     ROOT_DIR,
     SCRAPER,
     USER,
@@ -88,18 +96,20 @@
         max_concurrency,
         language,
         locale_name,
         tags,
         dateafter,
         use_any_optimized_version,
         s3_url_with_credentials,
+        publisher,
+        disable_metadata_checks,
         title=None,
         description=None,
+        long_description=None,
         creator=None,
-        publisher=None,
         name=None,
         profile_image=None,
         banner_image=None,
         main_color=None,
         secondary_color=None,
     ):
         # data-retrieval info
@@ -117,21 +127,34 @@
         self.all_subtitles = all_subtitles
         self.autoplay = autoplay
         self.fname = fname
         self.language = language
         self.tags = [t.strip() for t in tags.split(",")]
         self.title = title
         self.description = description
+        self.long_description = long_description
         self.creator = creator
         self.publisher = publisher
         self.name = name
         self.profile_image = profile_image
         self.banner_image = banner_image
         self.main_color = main_color
         self.secondary_color = secondary_color
+        self.disable_metadata_checks = disable_metadata_checks
+
+        if not self.disable_metadata_checks:
+            # Validate ZIM metadata early so that we do not waste time doing operations
+            # for a scraper which will fail anyway in the end
+            validate_tags("Tags", self.tags)
+            if self.title:
+                validate_title("Title", self.title)
+            if self.description:
+                validate_description("Description", self.description)
+            if self.long_description:
+                validate_longdescription("LongDescription", self.long_description)
 
         # directory setup
         self.output_dir = Path(output_dir).expanduser().resolve()
         if tmp_dir:
             tmp_dir = Path(tmp_dir).expanduser().resolve()
             tmp_dir.mkdir(parents=True, exist_ok=True)
         self.build_dir = Path(tempfile.mkdtemp(dir=tmp_dir))
@@ -345,22 +368,24 @@
             )
             logger.info("building ZIM file")
             make_zim_file(
                 build_dir=self.build_dir,
                 fpath=self.output_dir / self.fname,
                 name=self.name,
                 main_page="home.html",
-                favicon="favicon.jpg",
+                illustration="favicon.png",
                 title=self.title,
                 description=self.description,
+                long_description=self.long_description,  # pyright: ignore[reportArgumentType]
                 language=self.language,
                 creator=self.creator,
-                publisher="Kiwix",
+                publisher=self.publisher,
                 tags=self.tags,
                 scraper=SCRAPER,
+                disable_metadata_checks=self.disable_metadata_checks,
             )
 
             if not self.keep_build_dir:
                 logger.info("removing temp folder")
                 shutil.rmtree(self.build_dir, ignore_errors=True)
 
         logger.info("all done!")
@@ -792,26 +817,29 @@
             if self.is_playlist and len(self.playlists) == 1
             else main_channel_json["snippet"]["title"].strip()
         )
         auto_description = (
             clean_text(self.playlists[0].description)
             if self.is_playlist and len(self.playlists) == 1
             else clean_text(main_channel_json["snippet"]["description"])
-        )
+        ) or "-"
         self.title = self.title or auto_title or "-"
-        self.description = self.description or auto_description or "-"
+        self.description, self.long_description = compute_descriptions(
+            default_description=auto_description,
+            user_description=self.description,
+            user_long_description=self.long_description,
+        )
 
         if self.creator is None:
             if self.is_single_channel:
                 self.creator = _("Youtube Channel “{title}”").format(
                     title=main_channel_json["snippet"]["title"]
                 )
             else:
                 self.creator = _("Youtube Channels")
-        self.publisher = self.publisher or "Kiwix"
 
         self.tags = self.tags or ["youtube"]
         if "_videos:yes" not in self.tags:
             self.tags.append("_videos:yes")
 
         # copy our main_channel branding into /(profile|banner).jpg if not supplied
         if not self.profile_path.exists():
@@ -827,20 +855,24 @@
 
         # set colors from images if not supplied
         if self.main_color is None or self.secondary_color is None:
             profile_main, profile_secondary = get_colors(self.profile_path)
             self.main_color = self.main_color or profile_main
             self.secondary_color = self.secondary_color or profile_secondary
 
+        # convert profile image to png for favicon
+        png_profile_path = self.build_dir.joinpath("profile.png")
+        convert_image(self.profile_path, png_profile_path)
+
         resize_image(
-            self.profile_path,
+            png_profile_path,
             width=48,
             height=48,
             method="thumbnail",
-            dst=self.build_dir.joinpath("favicon.jpg"),
+            dst=self.build_dir.joinpath("favicon.png"),
         )
 
     def make_html_files(self, actual_videos_ids):
         """make up HTML structure to read the content
 
         /home.html                                  Homepage
```

### Comparing `youtube2zim-2.2.0/src/youtube2zim/utils.py` & `youtube2zim-2.3.0/src/youtube2zim/utils.py`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/src/youtube2zim/youtube.py` & `youtube2zim-2.3.0/src/youtube2zim/youtube.py`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/src/youtube2zim/locale/fr/LC_MESSAGES/messages.po` & `youtube2zim-2.3.0/src/youtube2zim/locale/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/src/youtube2zim/playlists/entrypoint.py` & `youtube2zim-2.3.0/src/youtube2zim/playlists/entrypoint.py`

 * *Files 12% similar despite different names*

```diff
@@ -54,32 +54,44 @@
         help="Custom title format for individual playlist ZIM",
     )
     parser.add_argument(
         "--playlists-description",
         help="Custom description format for individual playlist ZIM",
     )
     parser.add_argument(
+        "--playlists-long-description",
+        help="Custom long description for individual playlist ZIM.",
+    )
+    parser.add_argument(
         "--metadata-from",
         help="File path or URL to a JSON file holding custom metadata "
         "for individual playlists. Format in README",
     )
     parser.add_argument(
         "--debug", help="Enable verbose output", action="store_true", default=False
     )
     parser.add_argument(
         "--version",
         help="Display scraper version and exit",
         action="version",
         version=SCRAPER,
     )
 
+    parser.add_argument(
+        "--disable-metadata-checks",
+        help="Disable validity checks of metadata according to openZIM conventions",
+        action="store_true",
+        default=False,
+        dest="disable_metadata_checks",
+    )
+
     args, extra_args = parser.parse_known_args()
 
     # prevent setting --title and --description
-    for arg in ("name", "title", "description", "zim-file"):
+    for arg in ("name", "title", "description", "long-description", "zim-file"):
         if args.playlists_mode and has_argument(arg, extra_args):
             parser.error(
                 f"Can't use --{arg} in playlists mode. "
                 f"Use --playlists-{arg} to set format."
             )
 
     # playlists-name mandatory in playlist-mode
```

### Comparing `youtube2zim-2.2.0/src/youtube2zim/playlists/scraper.py` & `youtube2zim-2.3.0/src/youtube2zim/playlists/scraper.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         self,
         options,
         extra_args,
     ):
         # extract values from options
         self.api_key = options["api_key"]
         self.debug = options["debug"]
+        self.disable_metadata_checks = options["disable_metadata_checks"]
         self.playlists_mode = options["playlists_mode"]
         self.collection_type = options["collection_type"]
         self.youtube_id = options["youtube_id"]
 
         self.extra_args = extra_args
 
         self.build_dir = pathlib.Path(tempfile.mkdtemp())
@@ -133,21 +134,25 @@
             playlist_id,
             "--api-key",
             self.api_key,
         ]
         if self.debug:
             args.append("--debug")
 
+        if self.disable_metadata_checks:
+            args.append("--disable-metadata-checks")
+
         # set metadata args for playlist
         metadata = self.metadata.get(playlist_id, {})
         for key in (
             "name",
             "zim-file",
             "title",
             "description",
+            "long-description",
             "tags",
             "creator",
             "profile",
             "banner",
         ):
             # use value from metadata JSON if present else from command-line
             value = metadata.get(
@@ -181,14 +186,18 @@
             self.youtube_id,
             "--api-key",
             self.api_key,
             *self.extra_args,
         ]
         if self.debug:
             args.append("--debug")
+
+        if self.disable_metadata_checks:
+            args.append("--disable-metadata-checks")
+
         return subprocess.run(args).returncode  # noqa: PLW1510
 
     @staticmethod
     def compute_format(playlist, fmt):
         return fmt.format(**playlist.__dict__(), **{"period": "{period}"})
 
     def fetch_metadata(self):
```

### Comparing `youtube2zim-2.2.0/src/youtube2zim/templates/article.html` & `youtube2zim-2.3.0/src/youtube2zim/templates/article.html`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/src/youtube2zim/templates/home.html` & `youtube2zim-2.3.0/src/youtube2zim/templates/home.html`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/src/youtube2zim/templates/assets/app.js` & `youtube2zim-2.3.0/src/youtube2zim/templates/assets/app.js`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/src/youtube2zim/templates/assets/article.css` & `youtube2zim-2.3.0/src/youtube2zim/templates/assets/article.css`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/src/youtube2zim/templates/assets/banner.jpg` & `youtube2zim-2.3.0/src/youtube2zim/templates/assets/banner.jpg`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/src/youtube2zim/templates/assets/db.js` & `youtube2zim-2.3.0/src/youtube2zim/templates/assets/db.js`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/src/youtube2zim/templates/assets/home.css` & `youtube2zim-2.3.0/src/youtube2zim/templates/assets/home.css`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/src/youtube2zim/templates/assets/sample.jpg` & `youtube2zim-2.3.0/src/youtube2zim/templates/assets/sample.jpg`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/src/youtube2zim/templates/assets/webp-trigger.js` & `youtube2zim-2.3.0/src/youtube2zim/templates/assets/webp-trigger.js`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/src/youtube2zim/templates/assets/font/Roboto-Black.ttf` & `youtube2zim-2.3.0/src/youtube2zim/templates/assets/font/Roboto-Black.ttf`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/src/youtube2zim/templates/assets/font/Roboto-Bold.ttf` & `youtube2zim-2.3.0/src/youtube2zim/templates/assets/font/Roboto-Bold.ttf`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/src/youtube2zim/templates/assets/font/Roboto-Light.ttf` & `youtube2zim-2.3.0/src/youtube2zim/templates/assets/font/Roboto-Light.ttf`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/src/youtube2zim/templates/assets/font/Roboto-LightItalic.ttf` & `youtube2zim-2.3.0/src/youtube2zim/templates/assets/font/Roboto-LightItalic.ttf`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/src/youtube2zim/templates/assets/font/Roboto-Regular.ttf` & `youtube2zim-2.3.0/src/youtube2zim/templates/assets/font/Roboto-Regular.ttf`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/.gitignore` & `youtube2zim-2.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/LICENSE` & `youtube2zim-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `youtube2zim-2.2.0/README.md` & `youtube2zim-2.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -10,53 +10,61 @@
 from a Youtube Channel/Username or one-or-more Playlists.
 
 It downloads the video (`webm` or `mp4` extension – optionnaly
 recompress them in lower-quality, smaller size), the thumbnails, the
 subtitles and the authors' profile pictures ; then, it create a static
 HTML files folder of it before creating a ZIM off of it.
 
+This project adheres to openZIM's Contribution Guidelines.
+
+This project has implemented openZIM's Python bootstrap, conventions and policies v1.0.1.
+
 Requirements
 ------------
 
 * [`ffmpeg`](https://ffmpeg.org/) for video transcoding (only used with `--lower-quality`).
 * `curl` and `unzip` to install Javascript dependencies. See `get_js_deps.sh` if you want to do it manually.
 
 Installation
 ------------
 
 Here comes a few different ways to install `youtube2zim`.
 
 ## Virtualenv
 
-`youtube2zim` is a Python3 software. If you are not using the
-[Docker](https://docker.com) image, you are advised to use it in a
-[virtualenv](https://virtualenv.pypa.io) to avoid installing software
-dependences on your system.
+`youtube2zim` is a Python3 software. If you are not using the [Docker](https://docker.com) image,
+you are advised to use it in a [virtualenv](https://virtualenv.pypa.io) to avoid installing software
+dependencies on your system. [Hatch](https://hatch.pypa.io/) is the proper tool to create the
+virtualenv and install the software locally. Ensure to use proper Python version as well (see
+pyproject.toml).
+
+If you do not already have it on your system, install hatch to build the software and manage virtual
+environments (you might be interested by our detailed
+[Developer Setup](https://github.com/openzim/_python-bootstrap/wiki/Developer-Setup) as well,
+especially regarding how to configure hatch globally for proper detection of its virtual environments
+by Visual Studio Code).
 
-```bash
-virtualenv -p python3 ./ # Create virtualenv
-source bin/activate      # Activate the virtualenv
-pip3 install youtube2zim # Install dependencies
-youtube2zim --help       # Display youtube2zim help
+``` bash
+pip3 install hatch
 ```
 
-At the end, call `deactivate` to quit the virtual environment.
-
-See `pyproject.toml` for the list of python dependencies.
+Start a hatch shell: this will install software including dependencies in an isolated virtual environment.
 
-## Docker
+``` bash
+hatch shell
+```
 
 ```bash
-docker run -v my_dir:/output ghcr.io/openzim/youtube youtube2zim --help
+youtube2zim --help       # Display youtube2zim help
 ```
 
-## Globally (on GNU/Linux)
+## Docker
 
 ```bash
-sudo pip3 install -U youtube2zim
+docker run -v my_dir:/output ghcr.io/openzim/youtube youtube2zim --help
 ```
 
 Usage
 -----
 
 `youtube2zim` uses Youtube API v3 to fetch data from Youtube. You thus need to provide an `API_KEY` to use the scraper.
 
@@ -76,19 +84,19 @@
 * If you encounter issues reading ZIM files created using this scraper, please take a look at the [Compatibility Matrix](https://github.com/openzim/youtube/wiki/Compatibility) before opening a ticket.
 
 youtube2zim-playlists
 ---------------------
 
 `youtube2zim` produces a single ZIM file for a youtube request (`channel`, `user`, `playlist`).
 
-`youtube2zim-playlists` allows you to ** automatically create one ZIM file per playlist** of a given channel or user instead.
+`youtube2zim-playlists` allows you to **automatically create one ZIM file per playlist** of a given channel or user instead.
 
 This script is a wrapper around `youtube2zim` and is bundled with the main package.
 
-The difference between a channel and a user is due to Youtube legacy. Some old users have to be searched as a user, while more recent ones have to be searched as a channel. Try your best bet, and if it fails try the ohter type.
+The difference between a channel and a user is due to Youtube legacy. Some old users have to be searched as a user, while more recent ones have to be searched as a channel. Try your best bet, and if it fails try the other type.
 
 ## Usage
 
 `youtube2zim-playlists --help`
 
 Sample usage:
```

### Comparing `youtube2zim-2.2.0/pyproject.toml` & `youtube2zim-2.3.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,71 +1,68 @@
 [build-system]
-requires = ["hatchling"]
+requires = ["hatchling", "hatch-openzim==0.2.1"]
 build-backend = "hatchling.build"
 
 [project]
 name = "youtube2zim"
-authors = [{ name = "Kiwix", email = "dev@kiwix.org" }]
-keywords = ["kiwix", "zim", "offline", "youtube"]
-requires-python = ">=3.10,<3.11"
+requires-python = ">=3.12,<3.13"
 description = "Make ZIM file from a Youtube channel, user or playlist(s)"
 readme = "README.md"
-license = { text = "GPL-3.0-or-later" }
-classifiers = [
-  "Programming Language :: Python :: 3",
-  "Programming Language :: Python :: 3.10",
-  "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-]
 dependencies = [
   "python-slugify==3.0.3",
   "yt-dlp",                      # youtube-dl should be updated as frequently as possible
-  "python-dateutil==2.8.0",
-  "jinja2>=2.11,<3.0",
-  "MarkupSafe==2.0.1",           # jinja2 dependency (https://github.com/pallets/markupsafe/issues/284)
-  "zimscraperlib>=2.0.0,<2.1.0",
-  "requests==2.31.0",
+  "python-dateutil==2.9.0.post0",
+  "jinja2==3.1.4",
+  "zimscraperlib==3.3.2",
+  "requests==2.32.0",
   "kiwixstorage==0.8.3",
   "pif==0.8.2",
 ]
-dynamic = ["version"]
+dynamic = ["authors", "classifiers", "keywords", "license", "version", "urls"]
+
+[tool.hatch.metadata]
+allow-direct-references = true
+
+[tool.hatch.metadata.hooks.openzim-metadata]
+kind = "scraper"
+additional-keywords = ["youtube"]
+
+[tool.hatch.build.hooks.openzim-build]
+dependencies = [ "zimscraperlib==3.3.2"] # required for fix_ogv_dist
 
 [project.optional-dependencies]
 scripts = ["invoke==2.2.0"]
-lint = ["black==23.9.1", "ruff==0.0.292"]
-check = ["pyright==1.1.331"]
-test = ["pytest==7.4.2", "coverage==7.3.2"]
+lint = ["black==24.4.2", "ruff==0.4.4"]
+check = ["pyright==1.1.363"]
+test = ["pytest==8.1.1", "coverage==7.4.4"]
 dev = [
-  "pre-commit==3.4.0",
-  "debugpy==1.8.0",
+  "pre-commit==3.7.1",
+  "debugpy==1.8.1",
   "youtube2zim[scripts]",
   "youtube2zim[lint]",
   "youtube2zim[test]",
   "youtube2zim[check]",
-  # hatchling is a dev dependency only needed for hook development on developer machine
-  "hatchling==1.18.0",
   "humanfriendly==10.0"
 ]
 
-[project.urls]
-Homepage = "https://github.com/openzim/youtube"
-Donate = "https://www.kiwix.org/en/support-us/"
-
 [project.scripts]
 youtube2zim = "youtube2zim.__main__:main"
 youtube2zim-playlists = "youtube2zim.playlists.__main__:main"
 
 [tool.hatch.version]
 path = "src/youtube2zim/__about__.py"
 
 [tool.hatch.build]
 exclude = ["/.github"]
 
-[tool.hatch.build.hooks.custom]
-path = "hatch_build.py"
-dependencies = ["zimscraperlib>=2.0.0,<2.1.0"]
+[tool.hatch.build.targets.wheel]
+packages = ["src/youtube2zim"]
+artifacts = [
+  "src/youtube2zim/templates/assets/**",
+]
 
 [tool.hatch.envs.default]
 features = ["dev"]
 
 [tool.hatch.envs.test]
 features = ["scripts", "test"]
 
@@ -74,15 +71,15 @@
 run-cov = "inv test-cov --args '{args}'"
 report-cov = "inv report-cov"
 coverage = "inv coverage --args '{args}'"
 html = "inv coverage --html --args '{args}'"
 
 [tool.hatch.envs.lint]
 template = "lint"
-python = "py311"
+python = "py312"
 skip-install = false
 features = ["scripts", "lint"]
 
 [tool.hatch.envs.lint.scripts]
 black = "inv lint-black --args '{args}'"
 ruff = "inv lint-ruff --args '{args}'"
 all = "inv lintall --args '{args}'"
@@ -95,21 +92,23 @@
 
 [tool.hatch.envs.check.scripts]
 pyright = "inv check-pyright --args '{args}'"
 all = "inv checkall --args '{args}'"
 
 [tool.black]
 line-length = 88
-target-version = ['py311']
+target-version = ['py312']
 exclude = "(src/youtube2zim/templates/.*|.hatch/.*)"
 
 [tool.ruff]
-target-version = "py311"
+target-version = "py312"
 line-length = 88
 src = ["src"]
+
+[tool.ruff.lint]
 select = [
   "A", # flake8-builtins
   # "ANN",  # flake8-annotations
   "ARG", # flake8-unused-arguments
   # "ASYNC",  # flake8-async
   "B", # flake8-bugbear
   # "BLE",  # flake8-blind-except
@@ -186,21 +185,21 @@
   "PLR0915",
 ]
 unfixable = [
   # Don't touch unused imports
   "F401",
 ]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["youtube2zim"]
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
 [tool.pytest.ini_options]
 minversion = "7.3"
 testpaths = ["tests"]
 pythonpath = [".", "src"]
@@ -218,9 +217,10 @@
 [tool.coverage.report]
 exclude_lines = ["no cov", "if __name__ == .__main__.:", "if TYPE_CHECKING:"]
 
 [tool.pyright]
 include = ["src", "tests", "tasks.py"]
 exclude = [".env/**", ".venv/**", "src/youtube2zim/templates", ".hatch"]
 extraPaths = ["src"]
-pythonVersion = "3.10"
+pythonVersion = "3.12"
 typeCheckingMode = "basic"
+disableBytesTypePromotions = true
```

### Comparing `youtube2zim-2.2.0/PKG-INFO` & `youtube2zim-2.3.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 Metadata-Version: 2.1
 Name: youtube2zim
-Version: 2.2.0
+Version: 2.3.0
 Summary: Make ZIM file from a Youtube channel, user or playlist(s)
-Project-URL: Homepage, https://github.com/openzim/youtube
 Project-URL: Donate, https://www.kiwix.org/en/support-us/
-Author-email: Kiwix <dev@kiwix.org>
+Project-URL: Homepage, https://github.com/openzim/youtube
+Author-email: openZIM <dev@openzim.org>
 License: GPL-3.0-or-later
 License-File: LICENSE
-Keywords: kiwix,offline,youtube,zim
+Keywords: offline,openzim,youtube,zim
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: <3.11,>=3.10
-Requires-Dist: jinja2<3.0,>=2.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: <3.13,>=3.12
+Requires-Dist: jinja2==3.1.4
 Requires-Dist: kiwixstorage==0.8.3
-Requires-Dist: markupsafe==2.0.1
 Requires-Dist: pif==0.8.2
-Requires-Dist: python-dateutil==2.8.0
+Requires-Dist: python-dateutil==2.9.0.post0
 Requires-Dist: python-slugify==3.0.3
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests==2.32.0
 Requires-Dist: yt-dlp
-Requires-Dist: zimscraperlib<2.1.0,>=2.0.0
+Requires-Dist: zimscraperlib==3.3.2
 Provides-Extra: check
-Requires-Dist: pyright==1.1.331; extra == 'check'
+Requires-Dist: pyright==1.1.363; extra == 'check'
 Provides-Extra: dev
-Requires-Dist: debugpy==1.8.0; extra == 'dev'
-Requires-Dist: hatchling==1.18.0; extra == 'dev'
+Requires-Dist: debugpy==1.8.1; extra == 'dev'
 Requires-Dist: humanfriendly==10.0; extra == 'dev'
-Requires-Dist: pre-commit==3.4.0; extra == 'dev'
+Requires-Dist: pre-commit==3.7.1; extra == 'dev'
 Requires-Dist: youtube2zim[check]; extra == 'dev'
 Requires-Dist: youtube2zim[lint]; extra == 'dev'
 Requires-Dist: youtube2zim[scripts]; extra == 'dev'
 Requires-Dist: youtube2zim[test]; extra == 'dev'
 Provides-Extra: lint
-Requires-Dist: black==23.9.1; extra == 'lint'
-Requires-Dist: ruff==0.0.292; extra == 'lint'
+Requires-Dist: black==24.4.2; extra == 'lint'
+Requires-Dist: ruff==0.4.4; extra == 'lint'
 Provides-Extra: scripts
 Requires-Dist: invoke==2.2.0; extra == 'scripts'
 Provides-Extra: test
-Requires-Dist: coverage==7.3.2; extra == 'test'
-Requires-Dist: pytest==7.4.2; extra == 'test'
+Requires-Dist: coverage==7.4.4; extra == 'test'
+Requires-Dist: pytest==8.1.1; extra == 'test'
 Description-Content-Type: text/markdown
 
 Youtube2zim
 =============
 
 [![CodeFactor](https://www.codefactor.io/repository/github/openzim/youtube/badge)](https://www.codefactor.io/repository/github/openzim/youtube)
 [![Docker](https://ghcr-badge.deta.dev/openzim/youtube/latest_tag?label=docker)](https://ghcr.io/openzim/youtube)
@@ -54,53 +52,61 @@
 from a Youtube Channel/Username or one-or-more Playlists.
 
 It downloads the video (`webm` or `mp4` extension – optionnaly
 recompress them in lower-quality, smaller size), the thumbnails, the
 subtitles and the authors' profile pictures ; then, it create a static
 HTML files folder of it before creating a ZIM off of it.
 
+This project adheres to openZIM's Contribution Guidelines.
+
+This project has implemented openZIM's Python bootstrap, conventions and policies v1.0.1.
+
 Requirements
 ------------
 
 * [`ffmpeg`](https://ffmpeg.org/) for video transcoding (only used with `--lower-quality`).
 * `curl` and `unzip` to install Javascript dependencies. See `get_js_deps.sh` if you want to do it manually.
 
 Installation
 ------------
 
 Here comes a few different ways to install `youtube2zim`.
 
 ## Virtualenv
 
-`youtube2zim` is a Python3 software. If you are not using the
-[Docker](https://docker.com) image, you are advised to use it in a
-[virtualenv](https://virtualenv.pypa.io) to avoid installing software
-dependences on your system.
+`youtube2zim` is a Python3 software. If you are not using the [Docker](https://docker.com) image,
+you are advised to use it in a [virtualenv](https://virtualenv.pypa.io) to avoid installing software
+dependencies on your system. [Hatch](https://hatch.pypa.io/) is the proper tool to create the
+virtualenv and install the software locally. Ensure to use proper Python version as well (see
+pyproject.toml).
+
+If you do not already have it on your system, install hatch to build the software and manage virtual
+environments (you might be interested by our detailed
+[Developer Setup](https://github.com/openzim/_python-bootstrap/wiki/Developer-Setup) as well,
+especially regarding how to configure hatch globally for proper detection of its virtual environments
+by Visual Studio Code).
 
-```bash
-virtualenv -p python3 ./ # Create virtualenv
-source bin/activate      # Activate the virtualenv
-pip3 install youtube2zim # Install dependencies
-youtube2zim --help       # Display youtube2zim help
+``` bash
+pip3 install hatch
 ```
 
-At the end, call `deactivate` to quit the virtual environment.
-
-See `pyproject.toml` for the list of python dependencies.
+Start a hatch shell: this will install software including dependencies in an isolated virtual environment.
 
-## Docker
+``` bash
+hatch shell
+```
 
 ```bash
-docker run -v my_dir:/output ghcr.io/openzim/youtube youtube2zim --help
+youtube2zim --help       # Display youtube2zim help
 ```
 
-## Globally (on GNU/Linux)
+## Docker
 
 ```bash
-sudo pip3 install -U youtube2zim
+docker run -v my_dir:/output ghcr.io/openzim/youtube youtube2zim --help
 ```
 
 Usage
 -----
 
 `youtube2zim` uses Youtube API v3 to fetch data from Youtube. You thus need to provide an `API_KEY` to use the scraper.
 
@@ -120,19 +126,19 @@
 * If you encounter issues reading ZIM files created using this scraper, please take a look at the [Compatibility Matrix](https://github.com/openzim/youtube/wiki/Compatibility) before opening a ticket.
 
 youtube2zim-playlists
 ---------------------
 
 `youtube2zim` produces a single ZIM file for a youtube request (`channel`, `user`, `playlist`).
 
-`youtube2zim-playlists` allows you to ** automatically create one ZIM file per playlist** of a given channel or user instead.
+`youtube2zim-playlists` allows you to **automatically create one ZIM file per playlist** of a given channel or user instead.
 
 This script is a wrapper around `youtube2zim` and is bundled with the main package.
 
-The difference between a channel and a user is due to Youtube legacy. Some old users have to be searched as a user, while more recent ones have to be searched as a channel. Try your best bet, and if it fails try the ohter type.
+The difference between a channel and a user is due to Youtube legacy. Some old users have to be searched as a user, while more recent ones have to be searched as a channel. Try your best bet, and if it fails try the other type.
 
 ## Usage
 
 `youtube2zim-playlists --help`
 
 Sample usage:
```

