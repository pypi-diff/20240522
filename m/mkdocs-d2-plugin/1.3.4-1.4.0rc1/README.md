# Comparing `tmp/mkdocs_d2_plugin-1.3.4.tar.gz` & `tmp/mkdocs_d2_plugin-1.4.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_d2_plugin-1.3.4.tar", last modified: Wed May 22 15:18:26 2024, max compression
+gzip compressed data, was "mkdocs_d2_plugin-1.4.0rc1.tar", last modified: Wed May  8 08:54:19 2024, max compression
```

## Comparing `mkdocs_d2_plugin-1.3.4.tar` & `mkdocs_d2_plugin-1.4.0rc1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 landmaj    (501) staff       (20)        0 2024-05-22 15:18:26.753165 mkdocs_d2_plugin-1.3.4/
--rw-r--r--   0 landmaj    (501) staff       (20)     1061 2024-05-10 21:30:21.000000 mkdocs_d2_plugin-1.3.4/LICENSE
--rw-r--r--   0 landmaj    (501) staff       (20)     2170 2024-05-22 15:18:26.752863 mkdocs_d2_plugin-1.3.4/PKG-INFO
--rw-r--r--   0 landmaj    (501) staff       (20)     1153 2024-05-10 21:30:21.000000 mkdocs_d2_plugin-1.3.4/README.md
-drwxr-xr-x   0 landmaj    (501) staff       (20)        0 2024-05-22 15:18:26.751164 mkdocs_d2_plugin-1.3.4/d2/
--rw-r--r--   0 landmaj    (501) staff       (20)      318 2024-05-22 15:16:03.000000 mkdocs_d2_plugin-1.3.4/d2/__init__.py
--rw-r--r--   0 landmaj    (501) staff       (20)     1729 2024-05-22 15:16:03.000000 mkdocs_d2_plugin-1.3.4/d2/config.py
--rw-r--r--   0 landmaj    (501) staff       (20)     1713 2024-05-22 15:16:03.000000 mkdocs_d2_plugin-1.3.4/d2/fence.py
--rw-r--r--   0 landmaj    (501) staff       (20)     2569 2024-05-22 15:16:03.000000 mkdocs_d2_plugin-1.3.4/d2/img.py
--rw-r--r--   0 landmaj    (501) staff       (20)     3829 2024-05-22 15:16:03.000000 mkdocs_d2_plugin-1.3.4/d2/plugin.py
-drwxr-xr-x   0 landmaj    (501) staff       (20)        0 2024-05-22 15:18:26.752529 mkdocs_d2_plugin-1.3.4/mkdocs_d2_plugin.egg-info/
--rw-r--r--   0 landmaj    (501) staff       (20)     2170 2024-05-22 15:18:26.000000 mkdocs_d2_plugin-1.3.4/mkdocs_d2_plugin.egg-info/PKG-INFO
--rw-r--r--   0 landmaj    (501) staff       (20)      331 2024-05-22 15:18:26.000000 mkdocs_d2_plugin-1.3.4/mkdocs_d2_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 landmaj    (501) staff       (20)        1 2024-05-22 15:18:26.000000 mkdocs_d2_plugin-1.3.4/mkdocs_d2_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 landmaj    (501) staff       (20)       93 2024-05-22 15:18:26.000000 mkdocs_d2_plugin-1.3.4/mkdocs_d2_plugin.egg-info/entry_points.txt
--rw-r--r--   0 landmaj    (501) staff       (20)       62 2024-05-22 15:18:26.000000 mkdocs_d2_plugin-1.3.4/mkdocs_d2_plugin.egg-info/requires.txt
--rw-r--r--   0 landmaj    (501) staff       (20)        3 2024-05-22 15:18:26.000000 mkdocs_d2_plugin-1.3.4/mkdocs_d2_plugin.egg-info/top_level.txt
--rw-r--r--   0 landmaj    (501) staff       (20)       38 2024-05-22 15:18:26.753222 mkdocs_d2_plugin-1.3.4/setup.cfg
--rw-r--r--   0 landmaj    (501) staff       (20)     1492 2024-05-22 15:16:03.000000 mkdocs_d2_plugin-1.3.4/setup.py
+drwxr-xr-x   0 landmaj    (501) staff       (20)        0 2024-05-08 08:54:19.016018 mkdocs_d2_plugin-1.4.0rc1/
+-rw-r--r--   0 landmaj    (501) staff       (20)     1061 2024-04-17 23:00:44.000000 mkdocs_d2_plugin-1.4.0rc1/LICENSE
+-rw-r--r--   0 landmaj    (501) staff       (20)     2173 2024-05-08 08:54:19.015788 mkdocs_d2_plugin-1.4.0rc1/PKG-INFO
+-rw-r--r--   0 landmaj    (501) staff       (20)     1153 2024-04-17 23:00:44.000000 mkdocs_d2_plugin-1.4.0rc1/README.md
+drwxr-xr-x   0 landmaj    (501) staff       (20)        0 2024-05-08 08:54:19.014638 mkdocs_d2_plugin-1.4.0rc1/d2/
+-rw-r--r--   0 landmaj    (501) staff       (20)      360 2024-05-08 07:50:33.000000 mkdocs_d2_plugin-1.4.0rc1/d2/__init__.py
+-rw-r--r--   0 landmaj    (501) staff       (20)     2076 2024-05-08 08:43:06.000000 mkdocs_d2_plugin-1.4.0rc1/d2/config.py
+-rw-r--r--   0 landmaj    (501) staff       (20)     2041 2024-05-08 08:41:38.000000 mkdocs_d2_plugin-1.4.0rc1/d2/fence.py
+-rw-r--r--   0 landmaj    (501) staff       (20)     3263 2024-05-08 08:40:17.000000 mkdocs_d2_plugin-1.4.0rc1/d2/img.py
+-rw-r--r--   0 landmaj    (501) staff       (20)     5747 2024-05-08 08:37:54.000000 mkdocs_d2_plugin-1.4.0rc1/d2/plugin.py
+drwxr-xr-x   0 landmaj    (501) staff       (20)        0 2024-05-08 08:54:19.015601 mkdocs_d2_plugin-1.4.0rc1/mkdocs_d2_plugin.egg-info/
+-rw-r--r--   0 landmaj    (501) staff       (20)     2173 2024-05-08 08:54:19.000000 mkdocs_d2_plugin-1.4.0rc1/mkdocs_d2_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 landmaj    (501) staff       (20)      331 2024-05-08 08:54:19.000000 mkdocs_d2_plugin-1.4.0rc1/mkdocs_d2_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 landmaj    (501) staff       (20)        1 2024-05-08 08:54:19.000000 mkdocs_d2_plugin-1.4.0rc1/mkdocs_d2_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 landmaj    (501) staff       (20)       93 2024-05-08 08:54:19.000000 mkdocs_d2_plugin-1.4.0rc1/mkdocs_d2_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 landmaj    (501) staff       (20)       62 2024-05-08 08:54:19.000000 mkdocs_d2_plugin-1.4.0rc1/mkdocs_d2_plugin.egg-info/requires.txt
+-rw-r--r--   0 landmaj    (501) staff       (20)        3 2024-05-08 08:54:19.000000 mkdocs_d2_plugin-1.4.0rc1/mkdocs_d2_plugin.egg-info/top_level.txt
+-rw-r--r--   0 landmaj    (501) staff       (20)       38 2024-05-08 08:54:19.016059 mkdocs_d2_plugin-1.4.0rc1/setup.cfg
+-rw-r--r--   0 landmaj    (501) staff       (20)     1495 2024-05-08 08:53:00.000000 mkdocs_d2_plugin-1.4.0rc1/setup.py
```

### Comparing `mkdocs_d2_plugin-1.3.4/LICENSE` & `mkdocs_d2_plugin-1.4.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_d2_plugin-1.3.4/PKG-INFO` & `mkdocs_d2_plugin-1.4.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-d2-plugin
-Version: 1.3.4
+Version: 1.4.0rc1
 Summary: MkDocs plugin for D2
 Home-page: https://github.com/landmaj/mkdocs-d2-plugin
 Author: Michał Wieluński
 Author-email: michal@wielunski.net
 License: MIT
 Keywords: mkdocs python markdown d2 diagram
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs_d2_plugin-1.3.4/README.md` & `mkdocs_d2_plugin-1.4.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs_d2_plugin-1.3.4/d2/config.py` & `mkdocs_d2_plugin-1.4.0rc1/d2/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,28 +5,38 @@
 from pydantic import BaseModel
 
 
 class PluginConfig(Config):
     executable = config_options.Type(str, default="d2")
     cache = config_options.Type(bool, default=True)
     cache_dir = config_options.Type(str, default=".cache/plugin/d2")
+    rewrite_paths = config_options.Type(bool, default=True)
+    remove_sources = config_options.Type(bool, default=True)
+    raise_on_error = config_options.Type(bool, default=False)
 
     layout = config_options.Type(str, default="dagre")
     theme = config_options.Type(int, default=0)
     dark_theme = config_options.Type(int, default=-1)
     sketch = config_options.Type(bool, default=False)
     pad = config_options.Type(int, default=100)
     scale = config_options.Type(float, default=-1.0)
     force_appendix = config_options.Type(bool, default=False)
     target = config_options.Type(str, default="''")
 
     def d2_config(self):
         _dict = {}
         for k, v in self.items():
-            if k in {"executable", "cache", "cache_dir"}:
+            if k in {
+                "executable",
+                "cache",
+                "cache_dir",
+                "rewrite_paths",
+                "remove_sources",
+                "raise_on_error",
+            }:
                 continue
             _dict[k] = v
         return _dict
 
 
 class D2Config(BaseModel, extra="allow"):
     layout: str
```

### Comparing `mkdocs_d2_plugin-1.3.4/d2/fence.py` & `mkdocs_d2_plugin-1.4.0rc1/d2/fence.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from typing import Any, Dict
 
 from markdown import Markdown
+from mkdocs.exceptions import PluginError
 from pydantic import ValidationError
 from pymdownx.superfences import fence_code_format
 
 from d2 import Renderer, error
 from d2.config import D2Config
 
 
 class D2CustomFence:
     def __init__(
         self,
         config: Dict[str, Any],
         renderer: Renderer,
+        raise_on_error: bool,
     ) -> None:
         self.config = config
         self.renderer = renderer
+        self.raise_on_error = raise_on_error
 
     def validator(
         self,
         language: str,
         inputs: Dict[str, str],
         options: Dict[str, Any],
         attrs: Dict[str, Any],
@@ -28,16 +31,19 @@
         options["render"] = falsy(inputs.pop("render", "True"))
 
         cfg = self.config.copy()
         cfg.update(**inputs)
         try:
             cfg = D2Config(**cfg)
         except ValidationError as e:
-            error(e)
-            return False
+            if self.raise_on_error:
+                raise PluginError(e)
+            else:
+                error(e)
+                return False
 
         options["opts"] = cfg.opts()
         return True
 
     def formatter(
         self,
         source: str,
@@ -50,18 +56,21 @@
         if not options["render"]:
             return fence_code_format(
                 source, language, class_name, options, md, **kwargs
             )
 
         result, ok = self.renderer(source.encode(), options["opts"])
         if not ok:
-            error(result)
-            return fence_code_format(
-                source, language, class_name, options, md, **kwargs
-            )
+            if self.raise_on_error:
+                raise PluginError(result)
+            else:
+                error(result)
+                return fence_code_format(
+                    source, language, class_name, options, md, **kwargs
+                )
 
         return f"<div><style>svg>a:hover {{ text-decoration: underline }}</style>{result}</div>"
 
 
 def falsy(value: str) -> bool:
     if value.lower() in {"0", "false", "no", "off"}:
         return False
```

### Comparing `mkdocs_d2_plugin-1.3.4/d2/img.py` & `mkdocs_d2_plugin-1.4.0rc1/d2/img.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,47 @@
 import xml.etree.ElementTree as etree
 from io import StringIO
 from pathlib import Path
 from typing import Any, Dict, Optional
 
 from markdown import Extension, Markdown
 from markdown.treeprocessors import Treeprocessor
+from mkdocs.exceptions import PluginError
 from pydantic import ValidationError
 
 from d2 import Renderer, error, warning
 from d2.config import D2Config
 
 
 class D2ImgTreeprocessor(Treeprocessor):
     def __init__(
         self,
         md: Markdown,
         base_dir: str,
         config: Dict[str, Any],
         renderer: Renderer,
+        raise_on_error: bool,
     ):
         self.base_dir = base_dir
         self.config = config
         self.renderer = renderer
+        self.raise_on_error = raise_on_error
         super().__init__(md)
 
     def run(self, root: etree.Element) -> Optional[etree.Element]:
         for elem in root.iter("img"):
             src = Path(elem.get("src", ""))
             if src.suffix == ".d2":
                 diagram = Path(self.base_dir, src).resolve()
                 if not diagram.exists():
-                    warning(f"File not found: {diagram}")
-                    continue
+                    if self.raise_on_error:
+                        raise PluginError(f"File not found: {diagram}")
+                    else :
+                        warning(f"File not found: {diagram}")
+                        continue
                 with diagram.open("rb") as f:
                     source = f.read()
 
                 if source.strip() == b"":
                     warning(f"{src}: empty diagram file")
                     continue
 
@@ -43,21 +49,27 @@
                 cfg.update(elem.attrib)
                 cfg.pop("src")
                 cfg.pop("alt")
 
                 try:
                     cfg = D2Config(**cfg)
                 except ValidationError as e:
-                    error(e)
-                    continue
+                    if self.raise_on_error:
+                        raise PluginError(e)
+                    else:
+                        error(e)
+                        continue
 
                 result, ok = self.renderer(source, cfg.opts())
                 if not ok:
-                    error(result)
-                    continue
+                    if self.raise_on_error:
+                        raise PluginError(result)
+                    else:
+                        error(result)
+                        continue
 
                 svg = etree.iterparse(StringIO(result))
                 for _, el in svg:
                     # strip namespace
                     _, _, el.tag = el.tag.rpartition("}")
                 elem.tag = "div"
                 elem.clear()
@@ -66,18 +78,25 @@
 
 class D2ImgExtension(Extension):
     def __init__(self, **kwargs):
         self.config = {
             "base_dir": ["", "base directory for diagrams"],
             "config": [dict(), "global configuration"],
             "renderer": [Renderer, "render function"],
+            "raise_on_error": [False, "raise on error"],
         }
         super().__init__(**kwargs)
 
     def extendMarkdown(self, md: Markdown):
         md.registerExtension(self)
         cfg = self.getConfigs()
         md.treeprocessors.register(
-            D2ImgTreeprocessor(md, cfg["base_dir"], cfg["config"], cfg["renderer"]),
+            D2ImgTreeprocessor(
+                md,
+                cfg["base_dir"],
+                cfg["config"],
+                cfg["renderer"],
+                cfg["raise_on_error"],
+            ),
             "d2_img",
             7,
         )
```

### Comparing `mkdocs_d2_plugin-1.3.4/mkdocs_d2_plugin.egg-info/PKG-INFO` & `mkdocs_d2_plugin-1.4.0rc1/mkdocs_d2_plugin.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-d2-plugin
-Version: 1.3.4
+Version: 1.4.0rc1
 Summary: MkDocs plugin for D2
 Home-page: https://github.com/landmaj/mkdocs-d2-plugin
 Author: Michał Wieluński
 Author-email: michal@wielunski.net
 License: MIT
 Keywords: mkdocs python markdown d2 diagram
 Classifier: Development Status :: 4 - Beta
```

### Comparing `mkdocs_d2_plugin-1.3.4/setup.py` & `mkdocs_d2_plugin-1.4.0rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 PROJ_DIR = Path(__file__).resolve().parent
 with open(PROJ_DIR / "README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="mkdocs-d2-plugin",
-    version="1.3.4",
+    version="1.4.0rc1",
     description="MkDocs plugin for D2",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs python markdown d2 diagram",
     url="https://github.com/landmaj/mkdocs-d2-plugin",
     author="Michał Wieluński",
     author_email="michal@wielunski.net",
```

