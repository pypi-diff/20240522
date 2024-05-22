# Comparing `tmp/radprompter-1.1.7.tar.gz` & `tmp/radprompter-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radprompter-1.1.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "radprompter-1.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `radprompter-1.1.7.tar` & `radprompter-1.1.8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     3179 2024-05-20 13:36:09.252853 radprompter-1.1.7/.gitignore
--rw-r--r--   0        0        0    11357 2024-05-20 13:12:44.869856 radprompter-1.1.7/LICENSE
--rw-r--r--   0        0        0     3574 2024-05-20 16:41:16.503560 radprompter-1.1.7/README.md
--rw-r--r--   0        0        0    91362 2024-05-20 13:12:44.870856 radprompter-1.1.7/logo.png
--rw-r--r--   0        0        0      704 2024-05-20 17:15:57.479302 radprompter-1.1.7/pyproject.toml
--rw-r--r--   0        0        0      244 2024-05-20 14:12:23.709526 radprompter-1.1.7/radprompter/__init__.py
--rw-r--r--   0        0        0       21 2024-05-20 17:16:45.822784 radprompter-1.1.7/radprompter/__version__.py
--rw-r--r--   0        0        0      146 2024-05-20 13:12:44.874856 radprompter-1.1.7/radprompter/clients/__init__.py
--rw-r--r--   0        0        0      586 2024-05-20 14:15:49.896582 radprompter-1.1.7/radprompter/clients/clients.py
--rw-r--r--   0        0        0     3231 2024-05-20 16:16:17.141616 radprompter-1.1.7/radprompter/clients/huggingface/clients.py
--rw-r--r--   0        0        0     3022 2024-05-20 13:12:44.878856 radprompter-1.1.7/radprompter/clients/openai/clients.py
--rw-r--r--   0        0        0       27 2024-05-20 13:12:44.879856 radprompter-1.1.7/radprompter/prompts/__init__.py
--rw-r--r--   0        0        0     9976 2024-05-20 17:14:25.909389 radprompter-1.1.7/radprompter/prompts/prompts.py
--rw-r--r--   0        0        0     7303 2024-05-20 15:54:59.559882 radprompter-1.1.7/radprompter/radprompter.py
--rw-r--r--   0        0        0     1089 2024-05-20 13:12:44.882856 radprompter-1.1.7/sample_reports/sample_report_1.txt
--rw-r--r--   0        0        0     1388 2024-05-20 13:12:44.883856 radprompter-1.1.7/sample_reports/sample_report_2.txt
--rw-r--r--   0        0        0     1374 2024-05-20 13:12:44.883856 radprompter-1.1.7/sample_reports/sample_report_3.txt
--rw-r--r--   0        0        0    16815 2024-05-20 16:30:13.090948 radprompter-1.1.7/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb
--rw-r--r--   0        0        0      386 2024-05-20 13:12:44.887856 radprompter-1.1.7/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml
--rw-r--r--   0        0        0    17861 2024-05-20 16:30:17.748995 radprompter-1.1.7/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb
--rw-r--r--   0        0        0     1716 2024-05-20 13:12:44.889856 radprompter-1.1.7/tutorials/02_RDP-Templating/02_RDP-Templating.toml
--rw-r--r--   0        0        0    19275 2024-05-20 16:30:22.519042 radprompter-1.1.7/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb
--rw-r--r--   0        0        0     1884 2024-05-20 13:12:44.891856 radprompter-1.1.7/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml
--rw-r--r--   0        0        0    27143 2024-05-20 16:30:26.061077 radprompter-1.1.7/tutorials/04_Using-Schemas/04_Using-Schemas.ipynb
--rw-r--r--   0        0        0     4478 2024-05-20 15:54:06.767356 radprompter-1.1.7/tutorials/04_Using-Schemas/04_Using-Schemas.toml
--rw-r--r--   0        0        0    24106 2024-05-20 16:30:31.627133 radprompter-1.1.7/tutorials/05_JSON-Prefill/05_JSON-Prefill.ipynb
--rw-r--r--   0        0        0     3277 2024-05-20 13:12:44.895856 radprompter-1.1.7/tutorials/05_JSON-Prefill/05_JSON-Prefill.toml
--rw-r--r--   0        0        0    18209 2024-05-20 16:30:37.859195 radprompter-1.1.7/tutorials/06_HuggingFace-Client/06_HuggingFace-Client.ipynb
--rw-r--r--   0        0        0     1922 2024-05-20 16:01:46.474938 radprompter-1.1.7/tutorials/06_HuggingFace-Client/06_HuggingFace-Client.toml
--rw-r--r--   0        0        0     1825 2024-05-20 16:41:50.526900 radprompter-1.1.7/tutorials/README.md
--rw-r--r--   0        0        0     4154 1970-01-01 00:00:00.000000 radprompter-1.1.7/PKG-INFO
+-rw-r--r--   0        0        0     3179 2024-05-20 13:29:10.318934 radprompter-1.1.8/.gitignore
+-rw-r--r--   0        0        0    35149 2024-05-22 15:01:58.548435 radprompter-1.1.8/LICENSE
+-rw-r--r--   0        0        0     3574 2024-05-20 18:02:28.892553 radprompter-1.1.8/README.md
+-rw-r--r--   0        0        0    91362 2024-05-19 21:36:28.548393 radprompter-1.1.8/logo.png
+-rw-r--r--   0        0        0      704 2024-05-22 15:01:24.749407 radprompter-1.1.8/pyproject.toml
+-rw-r--r--   0        0        0      244 2024-05-20 18:02:28.893874 radprompter-1.1.8/radprompter/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-22 15:01:36.269039 radprompter-1.1.8/radprompter/__version__.py
+-rw-r--r--   0        0        0      146 2024-05-20 02:33:21.208331 radprompter-1.1.8/radprompter/clients/__init__.py
+-rw-r--r--   0        0        0      586 2024-05-19 22:16:28.933183 radprompter-1.1.8/radprompter/clients/clients.py
+-rw-r--r--   0        0        0     3231 2024-05-20 18:02:28.894660 radprompter-1.1.8/radprompter/clients/huggingface/clients.py
+-rw-r--r--   0        0        0     3022 2024-05-19 22:09:18.270492 radprompter-1.1.8/radprompter/clients/openai/clients.py
+-rw-r--r--   0        0        0       27 2024-05-14 22:18:09.544596 radprompter-1.1.8/radprompter/prompts/__init__.py
+-rw-r--r--   0        0        0     9976 2024-05-20 18:02:28.895187 radprompter-1.1.8/radprompter/prompts/prompts.py
+-rw-r--r--   0        0        0     7303 2024-05-20 18:02:28.895411 radprompter-1.1.8/radprompter/radprompter.py
+-rw-r--r--   0        0        0     1089 2024-05-14 18:23:37.434577 radprompter-1.1.8/sample_reports/sample_report_1.txt
+-rw-r--r--   0        0        0     1388 2024-05-14 18:23:37.434671 radprompter-1.1.8/sample_reports/sample_report_2.txt
+-rw-r--r--   0        0        0     1374 2024-05-14 18:23:37.434764 radprompter-1.1.8/sample_reports/sample_report_3.txt
+-rw-r--r--   0        0        0    16815 2024-05-20 18:02:28.895704 radprompter-1.1.8/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb
+-rw-r--r--   0        0        0      386 2024-05-19 18:49:48.028574 radprompter-1.1.8/tutorials/01_Basic-Usecase/01_Basic-Usecase.toml
+-rw-r--r--   0        0        0    17861 2024-05-20 18:02:28.896056 radprompter-1.1.8/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb
+-rw-r--r--   0        0        0     1716 2024-05-19 18:34:44.363741 radprompter-1.1.8/tutorials/02_RDP-Templating/02_RDP-Templating.toml
+-rw-r--r--   0        0        0    19275 2024-05-20 18:02:28.896577 radprompter-1.1.8/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb
+-rw-r--r--   0        0        0     1884 2024-05-19 19:04:34.358936 radprompter-1.1.8/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml
+-rw-r--r--   0        0        0    27143 2024-05-20 18:02:28.896937 radprompter-1.1.8/tutorials/04_Using-Schemas/04_Using-Schemas.ipynb
+-rw-r--r--   0        0        0     4478 2024-05-19 19:55:16.714928 radprompter-1.1.8/tutorials/04_Using-Schemas/04_Using-Schemas.toml
+-rw-r--r--   0        0        0    24106 2024-05-20 18:02:28.897096 radprompter-1.1.8/tutorials/05_JSON-Prefill/05_JSON-Prefill.ipynb
+-rw-r--r--   0        0        0     3277 2024-05-20 18:02:28.897513 radprompter-1.1.8/tutorials/05_JSON-Prefill/05_JSON-Prefill.toml
+-rw-r--r--   0        0        0    18209 2024-05-20 18:02:28.897622 radprompter-1.1.8/tutorials/06_HuggingFace-Client/06_HuggingFace-Client.ipynb
+-rw-r--r--   0        0        0     1922 2024-05-20 18:02:28.897715 radprompter-1.1.8/tutorials/06_HuggingFace-Client/06_HuggingFace-Client.toml
+-rw-r--r--   0        0        0     1825 2024-05-20 18:02:28.897911 radprompter-1.1.8/tutorials/README.md
+-rw-r--r--   0        0        0     4154 1970-01-01 00:00:00.000000 radprompter-1.1.8/PKG-INFO
```

### Comparing `radprompter-1.1.7/.gitignore` & `radprompter-1.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/README.md` & `radprompter-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/logo.png` & `radprompter-1.1.8/logo.png`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/pyproject.toml` & `radprompter-1.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,12 +6,12 @@
 name = "radprompter"
 authors = [{name = "Bardia Khosravi", email = "bardiakhosravi95@gmail.com"}, {name = "Theo Dapamede", email = "theo.dapamede@emory.edu"}]
 maintainers = [{name = "Bardia Khosravi", email = "bardiakhosravi95@gmail.com"}, {name = "Theo Dapamede", email = "theo.dapamede@emory.edu"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)"]
 dynamic = ["version", "description"]
-requires-python = ">=3.9"
+requires-python = ">=3.7"
 dependencies = ["pandas","openai"]
 
 [project.urls]
 Home = "https://github.com/BardiaKh/RadPrompter"
```

### Comparing `radprompter-1.1.7/radprompter/clients/clients.py` & `radprompter-1.1.8/radprompter/clients/clients.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/radprompter/clients/huggingface/clients.py` & `radprompter-1.1.8/radprompter/clients/huggingface/clients.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/radprompter/clients/openai/clients.py` & `radprompter-1.1.8/radprompter/clients/openai/clients.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/radprompter/prompts/prompts.py` & `radprompter-1.1.8/radprompter/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/radprompter/radprompter.py` & `radprompter-1.1.8/radprompter/radprompter.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/sample_reports/sample_report_1.txt` & `radprompter-1.1.8/sample_reports/sample_report_1.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/sample_reports/sample_report_2.txt` & `radprompter-1.1.8/sample_reports/sample_report_2.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/sample_reports/sample_report_3.txt` & `radprompter-1.1.8/sample_reports/sample_report_3.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb` & `radprompter-1.1.8/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb` & `radprompter-1.1.8/tutorials/02_RDP-Templating/02_RDP-Templating.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/tutorials/02_RDP-Templating/02_RDP-Templating.toml` & `radprompter-1.1.8/tutorials/02_RDP-Templating/02_RDP-Templating.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb` & `radprompter-1.1.8/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml` & `radprompter-1.1.8/tutorials/03_Multiturn-Prompting/03_Multiturn-Prompting.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/tutorials/04_Using-Schemas/04_Using-Schemas.ipynb` & `radprompter-1.1.8/tutorials/04_Using-Schemas/04_Using-Schemas.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/tutorials/04_Using-Schemas/04_Using-Schemas.toml` & `radprompter-1.1.8/tutorials/04_Using-Schemas/04_Using-Schemas.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/tutorials/05_JSON-Prefill/05_JSON-Prefill.ipynb` & `radprompter-1.1.8/tutorials/05_JSON-Prefill/05_JSON-Prefill.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/tutorials/05_JSON-Prefill/05_JSON-Prefill.toml` & `radprompter-1.1.8/tutorials/05_JSON-Prefill/05_JSON-Prefill.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/tutorials/06_HuggingFace-Client/06_HuggingFace-Client.ipynb` & `radprompter-1.1.8/tutorials/06_HuggingFace-Client/06_HuggingFace-Client.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/tutorials/06_HuggingFace-Client/06_HuggingFace-Client.toml` & `radprompter-1.1.8/tutorials/06_HuggingFace-Client/06_HuggingFace-Client.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/tutorials/README.md` & `radprompter-1.1.8/tutorials/README.md`

 * *Files identical despite different names*

### Comparing `radprompter-1.1.7/PKG-INFO` & `radprompter-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: radprompter
-Version: 1.1.7
+Version: 1.1.8
 Summary: A package for simplified and reproducible LLM prompting.
 Author-email: Bardia Khosravi <bardiakhosravi95@gmail.com>, Theo Dapamede <theo.dapamede@emory.edu>
 Maintainer-email: Bardia Khosravi <bardiakhosravi95@gmail.com>, Theo Dapamede <theo.dapamede@emory.edu>
-Requires-Python: >=3.9
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Dist: pandas
 Requires-Dist: openai
 Project-URL: Home, https://github.com/BardiaKh/RadPrompter
 
 ![RadPrompter](./logo.png)
```

