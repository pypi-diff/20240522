# Comparing `tmp/langflow-1.0.0a8.tar.gz` & `tmp/langflow-1.0.0a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langflow-1.0.0a8.tar", max compression
+gzip compressed data, was "langflow-1.0.0a9.tar", max compression
```

## Comparing `langflow-1.0.0a8.tar` & `langflow-1.0.0a9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1065 2024-04-04 21:33:18.021038 langflow-1.0.0a8/LICENSE
--rw-r--r--   0        0        0     6999 2024-04-04 21:33:18.021038 langflow-1.0.0a8/README.md
--rw-r--r--   0        0        0     3669 2024-04-04 21:33:42.917050 langflow-1.0.0a8/pyproject.toml
--rw-r--r--   0        0        0       47 2024-04-04 21:33:18.489038 langflow-1.0.0a8/src/backend/langflow/version/__init__.py
--rw-r--r--   0        0        0      156 2024-04-04 21:33:18.489038 langflow-1.0.0a8/src/backend/langflow/version/version.py
--rw-r--r--   0        0        0    10162 1970-01-01 00:00:00.000000 langflow-1.0.0a8/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-08 15:14:37.339560 langflow-1.0.0a9/LICENSE
+-rw-r--r--   0        0        0     6985 2024-04-08 15:14:37.339560 langflow-1.0.0a9/README.md
+-rw-r--r--   0        0        0     3805 2024-04-08 15:15:23.071033 langflow-1.0.0a9/pyproject.toml
+-rw-r--r--   0        0        0       47 2024-04-08 15:14:37.803554 langflow-1.0.0a9/src/backend/langflow/version/__init__.py
+-rw-r--r--   0        0        0      156 2024-04-08 15:14:37.803554 langflow-1.0.0a9/src/backend/langflow/version/version.py
+-rw-r--r--   0        0        0    10148 1970-01-01 00:00:00.000000 langflow-1.0.0a9/PKG-INFO
```

### Comparing `langflow-1.0.0a8/LICENSE` & `langflow-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `langflow-1.0.0a8/README.md` & `langflow-1.0.0a9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 <!-- markdownlint-disable MD030 -->
 
-# [![Langflow](https://github.com/logspace-ai/langflow/blob/dev/docs/static/img/new_langflow_demo.gif)](https://www.langflow.org)
+# [![Langflow](https://github.com/logspace-ai/langflow/blob/dev/docs/static/img/hero.png)](https://www.langflow.org)
 ### [Langflow](https://www.langflow.org) is a new, visual way to build, iterate and deploy AI apps.
 
 # ⚡️ Documentation and Community
 - [Documentation](https://docs.langflow.org)
 - [Discord](https://discord.com/invite/EqksyE2EX9)
 
 # 📦 Installation
 
-Make sure you have **Python 3.10** installed on your system.
-
 You can install Langflow with pip:
 
 ```shell
+# Make sure you have Python 3.10 installed on your system.
 # Install the pre-release version
-pip install langflow --pre --force-reinstall
+python -m pip install langflow --pre --force-reinstall
 
 # or stable version
-pip install langflow -U
+python -m pip install langflow -U
 ```
 
 Then, run Langflow with:
 
 ```shell
 python -m langflow run
-# or
-langflow run
 ```
 
 You can also preview Langflow in [HuggingFace Spaces](https://huggingface.co/spaces/Logspace/Langflow-Preview). [Clone the space using this link](https://huggingface.co/spaces/Logspace/Langflow-Preview?duplicate=true), to create your own Langflow workspace in minutes.
 
 # 🎨 Creating Flows
 
 Creating flows with Langflow is easy. Simply drag components from the sidebar onto the canvas and connect them to start building your application.
```

### Comparing `langflow-1.0.0a8/pyproject.toml` & `langflow-1.0.0a9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langflow"
-version = "1.0.0a8"
+version = "1.0.0a9"
 description = "A Python package with a built-in web application"
 authors = ["Logspace <contact@logspace.ai>"]
 maintainers = [
     "Carlos Coelho <carlos@logspace.ai>",
     "Cristhian Zanforlin <cristhian.lousa@gmail.com>",
     "Gabriel Almeida <gabriel@logspace.ai>",
     "Igor Carvalho <igorr.ackerman@gmail.com>",
@@ -22,15 +22,15 @@
 
 [tool.poetry.scripts]
 langflow = "langflow.__main__:main"
 
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
-langflow-base = "^0.0.20"
+langflow-base = "^0.0.21"
 beautifulsoup4 = "^4.12.2"
 google-search-results = "^2.4.1"
 google-api-python-client = "^2.118.0"
 huggingface-hub = { version = "^0.20.0", extras = ["inference"] }
 llama-cpp-python = { version = "~0.2.0", optional = true }
 networkx = "^3.1"
 pysrt = "^1.1.2"
@@ -98,15 +98,19 @@
 pytest-xdist = "^3.5.0"
 types-pywin32 = "^306.0.0.4"
 types-google-cloud-ndb = "^2.2.0.0"
 pytest-sugar = "^1.0.0"
 pytest-instafail = "^0.5.0"
 pytest-asyncio = "^0.23.0"
 respx = "^0.20.2"
-
+chromadb = "^0.4.24"
+langchain-anthropic = "^0.1.6"
+langchain-astradb = "^0.1.0"
+langchain-openai = "^0.1.1"
+langchain-cohere = "^0.1.0"
 
 [tool.poetry.extras]
 deploy = ["celery", "redis", "flower"]
 local = ["llama-cpp-python", "sentence-transformers", "ctransformers"]
 all = ["deploy", "local"]
```

### Comparing `langflow-1.0.0a8/PKG-INFO` & `langflow-1.0.0a9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langflow
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: A Python package with a built-in web application
 Home-page: https://github.com/logspace-ai/langflow
 License: MIT
 Keywords: nlp,langchain,openai,gpt,gui
 Author: Logspace
 Author-email: contact@logspace.ai
 Maintainer: Carlos Coelho
@@ -33,15 +33,15 @@
 Requires-Dist: flower (>=2.0.0,<3.0.0) ; extra == "deploy"
 Requires-Dist: google-api-python-client (>=2.118.0,<3.0.0)
 Requires-Dist: google-search-results (>=2.4.1,<3.0.0)
 Requires-Dist: html2text (>=2024.2.26,<2025.0.0)
 Requires-Dist: huggingface-hub[inference] (>=0.20.0,<0.21.0)
 Requires-Dist: langchain-cohere (>=0.1.0rc1,<0.2.0)
 Requires-Dist: langchain-google-genai (>=1.0.1,<2.0.0)
-Requires-Dist: langflow-base (>=0.0.20,<0.0.21)
+Requires-Dist: langflow-base (>=0.0.21,<0.0.22)
 Requires-Dist: langfuse (>=2.9.0,<3.0.0)
 Requires-Dist: litellm (>=1.34.22,<2.0.0)
 Requires-Dist: llama-cpp-python (>=0.2.0,<0.3.0) ; extra == "local"
 Requires-Dist: llama-index (>=0.10.13,<0.11.0)
 Requires-Dist: markupsafe (>=2.1.3,<3.0.0)
 Requires-Dist: metal-sdk (>=2.5.0,<3.0.0)
 Requires-Dist: metaphor-python (>=0.1.11,<0.2.0)
@@ -69,41 +69,38 @@
 Requires-Dist: wikipedia (>=1.4.0,<2.0.0)
 Project-URL: Documentation, https://docs.langflow.org
 Project-URL: Repository, https://github.com/logspace-ai/langflow
 Description-Content-Type: text/markdown
 
 <!-- markdownlint-disable MD030 -->
 
-# [![Langflow](https://github.com/logspace-ai/langflow/blob/dev/docs/static/img/new_langflow_demo.gif)](https://www.langflow.org)
+# [![Langflow](https://github.com/logspace-ai/langflow/blob/dev/docs/static/img/hero.png)](https://www.langflow.org)
 ### [Langflow](https://www.langflow.org) is a new, visual way to build, iterate and deploy AI apps.
 
 # ⚡️ Documentation and Community
 - [Documentation](https://docs.langflow.org)
 - [Discord](https://discord.com/invite/EqksyE2EX9)
 
 # 📦 Installation
 
-Make sure you have **Python 3.10** installed on your system.
-
 You can install Langflow with pip:
 
 ```shell
+# Make sure you have Python 3.10 installed on your system.
 # Install the pre-release version
-pip install langflow --pre --force-reinstall
+python -m pip install langflow --pre --force-reinstall
 
 # or stable version
-pip install langflow -U
+python -m pip install langflow -U
 ```
 
 Then, run Langflow with:
 
 ```shell
 python -m langflow run
-# or
-langflow run
 ```
 
 You can also preview Langflow in [HuggingFace Spaces](https://huggingface.co/spaces/Logspace/Langflow-Preview). [Clone the space using this link](https://huggingface.co/spaces/Logspace/Langflow-Preview?duplicate=true), to create your own Langflow workspace in minutes.
 
 # 🎨 Creating Flows
 
 Creating flows with Langflow is easy. Simply drag components from the sidebar onto the canvas and connect them to start building your application.
```

