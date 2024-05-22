# Comparing `tmp/mkdocs_ai_summary-0.1.1.tar.gz` & `tmp/mkdocs_ai_summary-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_ai_summary-0.1.1.tar", last modified: Wed May 22 15:46:40 2024, max compression
+gzip compressed data, was "mkdocs_ai_summary-0.2.0.tar", last modified: Wed May 22 20:25:11 2024, max compression
```

## Comparing `mkdocs_ai_summary-0.1.1.tar` & `mkdocs_ai_summary-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:40.250344 mkdocs_ai_summary-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-22 15:46:30.000000 mkdocs_ai_summary-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-22 15:46:40.250344 mkdocs_ai_summary-0.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:40.246344 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:30.000000 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-22 15:46:30.000000 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2184 2024-05-22 15:46:30.000000 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary/tongyi_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:46:40.250344 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3718 2024-05-22 15:46:40.000000 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-05-22 15:46:40.000000 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:46:40.000000 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-22 15:46:40.000000 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 15:46:40.000000 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 15:46:40.000000 mkdocs_ai_summary-0.1.1/mkdocs_ai_summary.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-22 15:46:30.000000 mkdocs_ai_summary-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-22 15:46:30.000000 mkdocs_ai_summary-0.1.1/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:46:40.250344 mkdocs_ai_summary-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:25:11.945992 mkdocs_ai_summary-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-22 20:25:02.000000 mkdocs_ai_summary-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-22 20:25:11.945992 mkdocs_ai_summary-0.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:25:11.945992 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:25:02.000000 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-22 20:25:02.000000 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary/chatgpt_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-22 20:25:02.000000 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-22 20:25:02.000000 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary/tongyi_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:25:11.945992 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-22 20:25:11.000000 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-22 20:25:11.000000 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:25:11.000000 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-22 20:25:11.000000 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 20:25:11.000000 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 20:25:11.000000 mkdocs_ai_summary-0.2.0/mkdocs_ai_summary.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 20:25:02.000000 mkdocs_ai_summary-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2024-05-22 20:25:02.000000 mkdocs_ai_summary-0.2.0/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:25:11.945992 mkdocs_ai_summary-0.2.0/setup.cfg
```

### Comparing `mkdocs_ai_summary-0.1.1/LICENSE` & `mkdocs_ai_summary-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_ai_summary-0.1.1/PKG-INFO` & `mkdocs_ai_summary-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ai-summary
-Version: 0.1.1
+Version: 0.2.0
 Summary: A mkdocs plugin to generage summary with the help of AI.
 Author-email: Yang Zhang <mail@yangzhang.site>
 License: MIT License
         
         Copyright (c) 2024 Yang Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,66 +22,86 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/AIboy996/mkdocs-ai-summary
-Keywords: mkdocs,AI,blog
+Keywords: mkdocs,AI,blog,chatgpt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mkdocs>=1.5.3
 Provides-Extra: tongyi
 Requires-Dist: dashscope; extra == "tongyi"
+Provides-Extra: chatgpt
+Requires-Dist: openai; extra == "chatgpt"
 
 # mkdocs-ai-summary
 
 [![PyPI - Version](https://img.shields.io/pypi/v/mkdocs-ai-summary)](https://pypi.org/project/mkdocs-ai-summary/)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/mkdocs-ai-summary)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-ai-summary)
 
 Generage an **ai-summary** for the page:
-![](assets/2024-05-22-22-00-32.png)
+![](assets/2024-05-23-04-11-20.png)
 
-Minimal demo [aiboy996.github.io/mkdocs-ai-summary](https://aiboy996.github.io/mkdocs-ai-summary)
+Minimal demo: [aiboy996.github.io/mkdocs-ai-summary](https://aiboy996.github.io/mkdocs-ai-summary)
 
 Live demo(my homepage): [yangzhang.site](https://yangzhang.site)
 
 ## Installation
 
 You should install the package with pip:
 ```
+pip install mkdocs-ai-summary[chatgpt]
+```
+or
+```
 pip install mkdocs-ai-summary[tongyi]
 ```
+> ⚠️⚠️⚠️⚠️
+> 
+> Only support [tongyi ai](https://tongyi.aliyun.com/) and [ChatGPT](https://chat.openai.com/) for now.
+>  
+>  To use **ChatGPT(default)**, you should set a Environmental Variable for **api key**:
+>  ```bash
+>  export OPENAI_API_KEY='sk-xxxxxxx'
+>  ```
+>
+>  To use **tongyi ai**, you should set a Environmental Variable for **api key**:
+>  ```bash
+>  export DASHSCOPE_API_KEY='sk-xxxxxxx'
+>  ```
 
-> Only support [tongyi ai](https://tongyi.aliyun.com/) for now. **Soon to support ChatGPT.**
-
-And you should include the [ai-summary.css](./docs/ai-summary.css)(optional, this is for the **custom admonition style**) in the config file as below:
+[optional] Then you can include the [ai-summary.css](./docs/ai-summary.css)(optional, this is for the **custom  ai summary admonition style**) in the config file as below:
 
 ## Configuration
 
 A demo for `mkdocs.yml`:
 
 ```yml
 site_name: mkdocs-ai-summary
 theme:
   name: material
 
 plugins:
   - ai-summary:
-      api: "tongyi"
-      ignore_code: true
+      # these are all default value
+      api: "chatgpt"
+      model: "gpt-3.5-turbo"
+      # we ignore ``` code block when do summary
+      ignore_code: true 
       cache: true
       cache_dir: "./"
       prompt: "请帮我把下面的内容总结为200字以内的摘要："
   - tags
 
 markdown_extensions:
   - admonition
@@ -101,12 +121,23 @@
 ---
 
 # h1
 
 ....
 ```
 
-# About Cache
+or you can use **tongyi ai** by setting:
+```yml
+plugins:
+  - ai-summary:
+      api: "tongyi"
+      ignore_code: true
+      cache: true
+      cache_dir: "./"
+      prompt: "请帮我把下面的内容总结为200字以内的摘要："
+```
+
+## About Cache
 
 Don't worry about duplicate api calls, we've made the cache function so that if you've done an ai-summary before and the content hasn't changed it will use the cache.
 
 Enjoy it.
```

### Comparing `mkdocs_ai_summary-0.1.1/mkdocs_ai_summary/plugin.py` & `mkdocs_ai_summary-0.2.0/mkdocs_ai_summary/plugin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 from mkdocs.config import config_options
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.plugins import BasePlugin
+from mkdocs.exceptions import ConfigurationError
 from mkdocs.structure.files import Files
 from mkdocs.structure.pages import Page
 
 import re
 import logging
 
 logger = logging.getLogger("mkdocs.plugins.ai-summary")
 
 
 class AiSummaryPlugin(BasePlugin):
     config_scheme = (
-        ("api", config_options.Type(str, default="tongyi")),
+        ("api", config_options.Type(str, default="chatgpt")),
         ("ignore_code", config_options.Type(bool, default=True)),
         ("cache", config_options.Type(bool, default=True)),
         ("cache_dir", config_options.Type(str, default="./")),
         (
+            "model",
+            config_options.Type(str, default="gpt-3.5-turbo"),
+        ),  # only used for gptapi
+        (
             "prompt",
             config_options.Type(
                 str, default="请帮我把下面的内容总结为200字以内的摘要："
             ),
         ),
     )
 
@@ -57,14 +62,38 @@
                     )
                 except AiSummaryError as e:
                     logger.warning("Ask AI Error", repr(e))
                     return markdown
                 except Exception as e:
                     logger.warning(repr(e))
                     return markdown
+            case "chatgpt":
+                try:
+                    from .chatgpt_api import get_summary_chatgpt
+                except ImportError as e:
+                    logger.warning("chatgpt is not available", repr(e))
+                    return markdown
+
+                logger.info(f"Asking AI summary for page {page.title}")
+                try:
+                    summary = get_summary_chatgpt(
+                        page=str(page.title),
+                        prompt=self.config["prompt"],
+                        markdown=markdown_to_summary,
+                        cache=self.config["cache"],
+                        cache_dir=self.config["cache_dir"],
+                        model=self.config["model"],
+                    )
+                except Exception as e:
+                    logger.warning(repr(e))
+                    return markdown
+            case _:
+                e = repr(ConfigurationError("unrecongnized api config."))
+                logger.warning(repr(e))
+                return markdown
         h1 = re.match(r"^# .*?\n", markdown)
         # if h1 exists, then insert summary after h1
         if h1:
             markdown = markdown[: h1.end()] + summary + markdown[h1.end() :]
         # else insert summary at the first beginning
         else:
             markdown = summary + markdown
```

### Comparing `mkdocs_ai_summary-0.1.1/mkdocs_ai_summary/tongyi_api.py` & `mkdocs_ai_summary-0.2.0/mkdocs_ai_summary/tongyi_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,11 @@
         else:
             ai_summary = ask(question)
             cache_dict[page] = {"content_md5": content_md5, "ai_summary": ai_summary}
             with open(f"{cache_dir}/_ai_summary_cache.json", "w+") as f:
                 cache_dict = json.dump(cache_dict, f)
     else:
         ai_summary = ask(question)
-    return f"""!!! ai-summary "AI摘要 powered by [通义千问](https://tongyi.aliyun.com/)"
+    return f"""!!! tongyiai-summary "AI Summary powered by [通义千问](https://tongyi.aliyun.com/)"
     {ai_summary}
 """
 
-
-if __name__ == "__main__":
-    ask()
```

### Comparing `mkdocs_ai_summary-0.1.1/mkdocs_ai_summary.egg-info/PKG-INFO` & `mkdocs_ai_summary-0.2.0/mkdocs_ai_summary.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-ai-summary
-Version: 0.1.1
+Version: 0.2.0
 Summary: A mkdocs plugin to generage summary with the help of AI.
 Author-email: Yang Zhang <mail@yangzhang.site>
 License: MIT License
         
         Copyright (c) 2024 Yang Zhang
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -22,66 +22,86 @@
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/AIboy996/mkdocs-ai-summary
-Keywords: mkdocs,AI,blog
+Keywords: mkdocs,AI,blog,chatgpt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mkdocs>=1.5.3
 Provides-Extra: tongyi
 Requires-Dist: dashscope; extra == "tongyi"
+Provides-Extra: chatgpt
+Requires-Dist: openai; extra == "chatgpt"
 
 # mkdocs-ai-summary
 
 [![PyPI - Version](https://img.shields.io/pypi/v/mkdocs-ai-summary)](https://pypi.org/project/mkdocs-ai-summary/)
 ![PyPI - Implementation](https://img.shields.io/pypi/implementation/mkdocs-ai-summary)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-ai-summary)
 
 Generage an **ai-summary** for the page:
-![](assets/2024-05-22-22-00-32.png)
+![](assets/2024-05-23-04-11-20.png)
 
-Minimal demo [aiboy996.github.io/mkdocs-ai-summary](https://aiboy996.github.io/mkdocs-ai-summary)
+Minimal demo: [aiboy996.github.io/mkdocs-ai-summary](https://aiboy996.github.io/mkdocs-ai-summary)
 
 Live demo(my homepage): [yangzhang.site](https://yangzhang.site)
 
 ## Installation
 
 You should install the package with pip:
 ```
+pip install mkdocs-ai-summary[chatgpt]
+```
+or
+```
 pip install mkdocs-ai-summary[tongyi]
 ```
+> ⚠️⚠️⚠️⚠️
+> 
+> Only support [tongyi ai](https://tongyi.aliyun.com/) and [ChatGPT](https://chat.openai.com/) for now.
+>  
+>  To use **ChatGPT(default)**, you should set a Environmental Variable for **api key**:
+>  ```bash
+>  export OPENAI_API_KEY='sk-xxxxxxx'
+>  ```
+>
+>  To use **tongyi ai**, you should set a Environmental Variable for **api key**:
+>  ```bash
+>  export DASHSCOPE_API_KEY='sk-xxxxxxx'
+>  ```
 
-> Only support [tongyi ai](https://tongyi.aliyun.com/) for now. **Soon to support ChatGPT.**
-
-And you should include the [ai-summary.css](./docs/ai-summary.css)(optional, this is for the **custom admonition style**) in the config file as below:
+[optional] Then you can include the [ai-summary.css](./docs/ai-summary.css)(optional, this is for the **custom  ai summary admonition style**) in the config file as below:
 
 ## Configuration
 
 A demo for `mkdocs.yml`:
 
 ```yml
 site_name: mkdocs-ai-summary
 theme:
   name: material
 
 plugins:
   - ai-summary:
-      api: "tongyi"
-      ignore_code: true
+      # these are all default value
+      api: "chatgpt"
+      model: "gpt-3.5-turbo"
+      # we ignore ``` code block when do summary
+      ignore_code: true 
       cache: true
       cache_dir: "./"
       prompt: "请帮我把下面的内容总结为200字以内的摘要："
   - tags
 
 markdown_extensions:
   - admonition
@@ -101,12 +121,23 @@
 ---
 
 # h1
 
 ....
 ```
 
-# About Cache
+or you can use **tongyi ai** by setting:
+```yml
+plugins:
+  - ai-summary:
+      api: "tongyi"
+      ignore_code: true
+      cache: true
+      cache_dir: "./"
+      prompt: "请帮我把下面的内容总结为200字以内的摘要："
+```
+
+## About Cache
 
 Don't worry about duplicate api calls, we've made the cache function so that if you've done an ai-summary before and the content hasn't changed it will use the cache.
 
 Enjoy it.
```

### Comparing `mkdocs_ai_summary-0.1.1/pyproject.toml` & `mkdocs_ai_summary-0.2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -3,37 +3,38 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.packages.find]
 where = ["."]
 
 [project]
 name = "mkdocs-ai-summary"
-version = "0.1.1"
+version = "0.2.0"
 requires-python = ">=3.10"
 dependencies = [
     "mkdocs>=1.5.3",
 ]
 authors = [
   { name="Yang Zhang", email="mail@yangzhang.site" },
 ]
 description = "A mkdocs plugin to generage summary with the help of AI."
 readme = "readme.md"
 license = {file = "LICENSE"}
-keywords = ["mkdocs", "AI", "blog"]
+keywords = ["mkdocs", "AI", "blog", "chatgpt"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.optional-dependencies]
 tongyi = ["dashscope"]
+chatgpt = ["openai"]
 
 [project.urls]
 Homepage = "https://github.com/AIboy996/mkdocs-ai-summary"
 
 [project.entry-points."mkdocs.plugins"]
 ai-summary = "mkdocs_ai_summary.plugin:AiSummaryPlugin"
```

