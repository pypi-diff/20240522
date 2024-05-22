# Comparing `tmp/aigents-0.8.0.tar.gz` & `tmp/aigents-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aigents-0.8.0.tar", max compression
+gzip compressed data, was "aigents-0.8.1.tar", max compression
```

## Comparing `aigents-0.8.0.tar` & `aigents-0.8.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.8.0/LICENSE
--rw-r--r--   0        0        0     7402 2024-05-06 13:16:01.219386 aigents-0.8.0/README.md
--rw-r--r--   0        0        0     1044 2024-05-17 18:43:57.599711 aigents-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      843 2024-05-06 12:53:46.596803 aigents-0.8.0/src/aigents/__init__.py
--rw-r--r--   0        0        0    19580 2024-05-17 17:53:53.908658 aigents-0.8.0/src/aigents/base.py
--rw-r--r--   0        0        0     1238 2024-05-17 18:41:32.446222 aigents-0.8.0/src/aigents/constants.py
--rw-r--r--   0        0        0      376 2024-05-05 20:28:48.665557 aigents-0.8.0/src/aigents/context/__init__.py
--rw-r--r--   0        0        0     2023 2024-05-06 17:26:15.624797 aigents-0.8.0/src/aigents/context/base.py
--rw-r--r--   0        0        0    13227 2024-05-15 19:26:29.333058 aigents-0.8.0/src/aigents/context/core.py
--rw-r--r--   0        0        0      337 2024-05-03 19:26:39.754455 aigents-0.8.0/src/aigents/context/errors.py
--rw-r--r--   0        0        0        0 2024-05-03 19:26:39.754455 aigents-0.8.0/src/aigents/context/nlp/__init__.py
--rw-r--r--   0        0        0     1098 2024-05-06 12:34:29.130871 aigents-0.8.0/src/aigents/context/nlp/base.py
--rw-r--r--   0        0        0      105 2024-05-03 19:26:39.754455 aigents-0.8.0/src/aigents/context/nlp/constants.py
--rw-r--r--   0        0        0      149 2024-05-03 19:26:39.754455 aigents-0.8.0/src/aigents/context/nlp/errors.py
--rw-r--r--   0        0        0    17637 2024-05-10 12:40:21.261161 aigents-0.8.0/src/aigents/context/nlp/processors.py
--rw-r--r--   0        0        0     3101 2024-05-09 19:39:39.988951 aigents-0.8.0/src/aigents/context/nlp/utils.py
--rw-r--r--   0        0        0     4020 2024-05-10 17:24:48.875825 aigents-0.8.0/src/aigents/context/utils.py
--rw-r--r--   0        0        0    32013 2024-05-17 18:47:54.121371 aigents-0.8.0/src/aigents/core.py
--rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.8.0/src/aigents/data.py
--rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.8.0/src/aigents/errors.py
--rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.8.0/src/aigents/prompts.py
--rw-r--r--   0        0        0     2822 2024-05-05 20:28:48.665557 aigents-0.8.0/src/aigents/settings.py
--rw-r--r--   0        0        0     6814 2024-05-03 19:26:39.754455 aigents-0.8.0/src/aigents/utils.py
--rw-r--r--   0        0        0     8712 1970-01-01 00:00:00.000000 aigents-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-29 18:27:57.056767 aigents-0.8.1/LICENSE
+-rw-r--r--   0        0        0     7402 2024-05-06 13:16:01.219386 aigents-0.8.1/README.md
+-rw-r--r--   0        0        0     1044 2024-05-22 15:55:18.290255 aigents-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      843 2024-05-06 12:53:46.596803 aigents-0.8.1/src/aigents/__init__.py
+-rw-r--r--   0        0        0    19580 2024-05-17 17:53:53.908658 aigents-0.8.1/src/aigents/base.py
+-rw-r--r--   0        0        0     1238 2024-05-17 18:41:32.446222 aigents-0.8.1/src/aigents/constants.py
+-rw-r--r--   0        0        0      376 2024-05-05 20:28:48.665557 aigents-0.8.1/src/aigents/context/__init__.py
+-rw-r--r--   0        0        0     2023 2024-05-06 17:26:15.624797 aigents-0.8.1/src/aigents/context/base.py
+-rw-r--r--   0        0        0    13227 2024-05-15 19:26:29.333058 aigents-0.8.1/src/aigents/context/core.py
+-rw-r--r--   0        0        0      337 2024-05-03 19:26:39.754455 aigents-0.8.1/src/aigents/context/errors.py
+-rw-r--r--   0        0        0        0 2024-05-03 19:26:39.754455 aigents-0.8.1/src/aigents/context/nlp/__init__.py
+-rw-r--r--   0        0        0     1098 2024-05-06 12:34:29.130871 aigents-0.8.1/src/aigents/context/nlp/base.py
+-rw-r--r--   0        0        0      105 2024-05-03 19:26:39.754455 aigents-0.8.1/src/aigents/context/nlp/constants.py
+-rw-r--r--   0        0        0      149 2024-05-03 19:26:39.754455 aigents-0.8.1/src/aigents/context/nlp/errors.py
+-rw-r--r--   0        0        0    17637 2024-05-10 12:40:21.261161 aigents-0.8.1/src/aigents/context/nlp/processors.py
+-rw-r--r--   0        0        0     3101 2024-05-09 19:39:39.988951 aigents-0.8.1/src/aigents/context/nlp/utils.py
+-rw-r--r--   0        0        0     4020 2024-05-10 17:24:48.875825 aigents-0.8.1/src/aigents/context/utils.py
+-rw-r--r--   0        0        0    32020 2024-05-22 15:54:28.277864 aigents-0.8.1/src/aigents/core.py
+-rw-r--r--   0        0        0      188 2024-02-23 18:20:01.705095 aigents-0.8.1/src/aigents/data.py
+-rw-r--r--   0        0        0      640 2024-02-29 13:47:18.770982 aigents-0.8.1/src/aigents/errors.py
+-rw-r--r--   0        0        0    28395 2024-03-08 19:28:00.158179 aigents-0.8.1/src/aigents/prompts.py
+-rw-r--r--   0        0        0     2822 2024-05-05 20:28:48.665557 aigents-0.8.1/src/aigents/settings.py
+-rw-r--r--   0        0        0     6814 2024-05-03 19:26:39.754455 aigents-0.8.1/src/aigents/utils.py
+-rw-r--r--   0        0        0     8712 1970-01-01 00:00:00.000000 aigents-0.8.1/PKG-INFO
```

### Comparing `aigents-0.8.0/LICENSE` & `aigents-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aigents-0.8.0/README.md` & `aigents-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `aigents-0.8.0/pyproject.toml` & `aigents-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aigents"
-version = "0.8.0"
+version = "0.8.1"
 description = "Adapters for Large Language Models and Generative Pre-trained Transformers APIs"
 authors = ["Vagner Bessa <bessavagner@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [{include = "aigents", from = "src"}]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `aigents-0.8.0/src/aigents/__init__.py` & `aigents-0.8.1/src/aigents/__init__.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.0/src/aigents/base.py` & `aigents-0.8.1/src/aigents/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.0/src/aigents/constants.py` & `aigents-0.8.1/src/aigents/constants.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.0/src/aigents/context/base.py` & `aigents-0.8.1/src/aigents/context/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.0/src/aigents/context/core.py` & `aigents-0.8.1/src/aigents/context/core.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.0/src/aigents/context/nlp/base.py` & `aigents-0.8.1/src/aigents/context/nlp/base.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.0/src/aigents/context/nlp/processors.py` & `aigents-0.8.1/src/aigents/context/nlp/processors.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.0/src/aigents/context/nlp/utils.py` & `aigents-0.8.1/src/aigents/context/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.0/src/aigents/context/utils.py` & `aigents-0.8.1/src/aigents/context/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.0/src/aigents/core.py` & `aigents-0.8.1/src/aigents/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -433,15 +433,15 @@
         )
         self.last_response = response
         try:
             self._update(
                 ROLES[-1], response.text, use_agent=use_agent, agent=agent
             )
             return response.text
-        except ValueError:
+        except ValueError as err:
             if len(response.candidates[0].content.parts) == 0:
                 message = (
                     "Model didn't return any message. "
                     f"Finish reason: {response.candidates[0].finish_reason.name}"
                 )
                 raise AgentError(message) from err
             text = '\n'.join(
```

### Comparing `aigents-0.8.0/src/aigents/errors.py` & `aigents-0.8.1/src/aigents/errors.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.0/src/aigents/prompts.py` & `aigents-0.8.1/src/aigents/prompts.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.0/src/aigents/settings.py` & `aigents-0.8.1/src/aigents/settings.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.0/src/aigents/utils.py` & `aigents-0.8.1/src/aigents/utils.py`

 * *Files identical despite different names*

### Comparing `aigents-0.8.0/PKG-INFO` & `aigents-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aigents
-Version: 0.8.0
+Version: 0.8.1
 Summary: Adapters for Large Language Models and Generative Pre-trained Transformers APIs
 Home-page: https://github.com/bessavagner/aigents.git
 License: GPL-3.0-only
 Author: Vagner Bessa
 Author-email: bessavagner@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
```

