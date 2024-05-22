# Comparing `tmp/neo4j_runway-0.2.0.tar.gz` & `tmp/neo4j_runway-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo4j_runway-0.2.0.tar", max compression
+gzip compressed data, was "neo4j_runway-0.2.1.tar", max compression
```

## Comparing `neo4j_runway-0.2.0.tar` & `neo4j_runway-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11354 2024-05-01 12:35:47.639470 neo4j_runway-0.2.0/LICENSE
--rw-r--r--   0        0        0     4713 2024-05-15 19:25:39.876076 neo4j_runway-0.2.0/README.md
--rw-r--r--   0        0        0      205 2024-05-01 12:25:23.214243 neo4j_runway-0.2.0/neo4j_runway/__init__.py
--rw-r--r--   0        0        0       33 2024-04-29 23:04:42.985466 neo4j_runway-0.2.0/neo4j_runway/discovery/__init__.py
--rw-r--r--   0        0        0     4373 2024-05-20 15:27:42.152492 neo4j_runway-0.2.0/neo4j_runway/discovery/discovery.py
--rw-r--r--   0        0        0       79 2024-04-29 23:04:42.986387 neo4j_runway-0.2.0/neo4j_runway/ingestion/__init__.py
--rw-r--r--   0        0        0    15503 2024-05-20 16:02:28.192255 neo4j_runway-0.2.0/neo4j_runway/ingestion/generate_ingest.py
--rwxr-xr-x   0        0        0     4922 2024-05-20 15:50:27.701057 neo4j_runway-0.2.0/neo4j_runway/ingestion/pyingest.py
--rw-r--r--   0        0        0       21 2024-04-29 23:04:42.987658 neo4j_runway-0.2.0/neo4j_runway/llm/__init__.py
--rw-r--r--   0        0        0     4962 2024-05-20 18:43:19.227627 neo4j_runway-0.2.0/neo4j_runway/llm/llm.py
--rw-r--r--   0        0        0       38 2024-04-29 23:04:42.988650 neo4j_runway-0.2.0/neo4j_runway/modeler/__init__.py
--rw-r--r--   0        0        0    10072 2024-05-20 18:43:19.231514 neo4j_runway-0.2.0/neo4j_runway/modeler/modeler.py
--rw-r--r--   0        0        0      229 2024-05-02 11:43:53.434393 neo4j_runway-0.2.0/neo4j_runway/objects/__init__.py
--rw-r--r--   0        0        0     2990 2024-05-15 19:25:52.037594 neo4j_runway-0.2.0/neo4j_runway/objects/arrows.py
--rw-r--r--   0        0        0    11786 2024-05-20 18:43:19.232422 neo4j_runway-0.2.0/neo4j_runway/objects/data_model.py
--rw-r--r--   0        0        0     4828 2024-05-15 19:25:52.038524 neo4j_runway-0.2.0/neo4j_runway/objects/node.py
--rw-r--r--   0        0        0     2934 2024-05-15 19:25:52.039220 neo4j_runway-0.2.0/neo4j_runway/objects/property.py
--rw-r--r--   0        0        0     5438 2024-05-20 15:27:42.186513 neo4j_runway-0.2.0/neo4j_runway/objects/relationship.py
--rw-r--r--   0        0        0      904 2024-05-02 11:43:53.436909 neo4j_runway-0.2.0/neo4j_runway/objects/user_input.py
--rw-r--r--   0        0        0     2393 2024-05-20 18:43:19.233382 neo4j_runway-0.2.0/neo4j_runway/resources/prompts/prompts.py
--rw-r--r--   0        0        0      138 2024-04-29 23:04:43.003742 neo4j_runway-0.2.0/neo4j_runway/utils/__init__.py
--rw-r--r--   0        0        0     3429 2024-04-29 23:04:43.003938 neo4j_runway-0.2.0/neo4j_runway/utils/naming_conventions.py
--rw-r--r--   0        0        0      917 2024-05-01 12:25:23.223161 neo4j_runway-0.2.0/neo4j_runway/utils/test_connection.py
--rw-r--r--   0        0        0     1133 2024-05-20 18:56:18.317163 neo4j_runway-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5993 1970-01-01 00:00:00.000000 neo4j_runway-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11354 2024-05-01 12:35:47.639470 neo4j_runway-0.2.1/LICENSE
+-rw-r--r--   0        0        0     4780 2024-05-22 14:20:25.800919 neo4j_runway-0.2.1/README.md
+-rw-r--r--   0        0        0      216 2024-05-22 14:20:25.801566 neo4j_runway-0.2.1/neo4j_runway/__init__.py
+-rw-r--r--   0        0        0       33 2024-04-29 23:04:42.985466 neo4j_runway-0.2.1/neo4j_runway/discovery/__init__.py
+-rw-r--r--   0        0        0     4373 2024-05-21 12:37:17.143781 neo4j_runway-0.2.1/neo4j_runway/discovery/discovery.py
+-rw-r--r--   0        0        0       79 2024-04-29 23:04:42.986387 neo4j_runway-0.2.1/neo4j_runway/ingestion/__init__.py
+-rw-r--r--   0        0        0    15503 2024-05-21 12:37:17.144321 neo4j_runway-0.2.1/neo4j_runway/ingestion/generate_ingest.py
+-rwxr-xr-x   0        0        0     4922 2024-05-21 12:37:17.144800 neo4j_runway-0.2.1/neo4j_runway/ingestion/pyingest.py
+-rw-r--r--   0        0        0       21 2024-04-29 23:04:42.987658 neo4j_runway-0.2.1/neo4j_runway/llm/__init__.py
+-rw-r--r--   0        0        0     4962 2024-05-21 12:37:17.145297 neo4j_runway-0.2.1/neo4j_runway/llm/llm.py
+-rw-r--r--   0        0        0       38 2024-04-29 23:04:42.988650 neo4j_runway-0.2.1/neo4j_runway/modeler/__init__.py
+-rw-r--r--   0        0        0    10072 2024-05-21 12:37:17.146484 neo4j_runway-0.2.1/neo4j_runway/modeler/modeler.py
+-rw-r--r--   0        0        0      229 2024-05-02 11:43:53.434393 neo4j_runway-0.2.1/neo4j_runway/objects/__init__.py
+-rw-r--r--   0        0        0     2990 2024-05-21 12:37:17.147283 neo4j_runway-0.2.1/neo4j_runway/objects/arrows.py
+-rw-r--r--   0        0        0    11786 2024-05-21 12:37:17.147911 neo4j_runway-0.2.1/neo4j_runway/objects/data_model.py
+-rw-r--r--   0        0        0     4828 2024-05-21 12:37:17.148608 neo4j_runway-0.2.1/neo4j_runway/objects/node.py
+-rw-r--r--   0        0        0     2934 2024-05-21 12:37:17.149307 neo4j_runway-0.2.1/neo4j_runway/objects/property.py
+-rw-r--r--   0        0        0     5438 2024-05-21 12:37:17.149779 neo4j_runway-0.2.1/neo4j_runway/objects/relationship.py
+-rw-r--r--   0        0        0      904 2024-05-02 11:43:53.436909 neo4j_runway-0.2.1/neo4j_runway/objects/user_input.py
+-rw-r--r--   0        0        0     2393 2024-05-21 12:37:17.150388 neo4j_runway-0.2.1/neo4j_runway/resources/prompts/prompts.py
+-rw-r--r--   0        0        0      138 2024-04-29 23:04:43.003742 neo4j_runway-0.2.1/neo4j_runway/utils/__init__.py
+-rw-r--r--   0        0        0     3429 2024-04-29 23:04:43.003938 neo4j_runway-0.2.1/neo4j_runway/utils/naming_conventions.py
+-rw-r--r--   0        0        0      917 2024-05-01 12:25:23.223161 neo4j_runway-0.2.1/neo4j_runway/utils/test_connection.py
+-rw-r--r--   0        0        0     1133 2024-05-22 14:20:36.546370 neo4j_runway-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     6060 1970-01-01 00:00:00.000000 neo4j_runway-0.2.1/PKG-INFO
```

### Comparing `neo4j_runway-0.2.0/LICENSE` & `neo4j_runway-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.2.0/README.md` & `neo4j_runway-0.2.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from neo4j_runway import Discovery, GraphDataModeler, IngestionGenerator, LLM, PyIngest
 
 ```
 ### Discovery
 Now we define a General Description of our data, provide brief descriptions of the columns of interest and load the data with Pandas.
 ```Python
 USER_GENERATED_INPUT = {
-    'General Description': 'This is data on different countries.',
+    'general_description': 'This is data on different countries.',
     'id': 'unique id for a country.',
     'name': 'the country name.',
     'phone_code': 'country area code.',
     'capital': 'the capital of the country.',
     'currency_name': "name of the country's currency.",
     'region': 'primary region of the country.',
     'subregion': 'subregion location of the country.',
@@ -44,30 +44,30 @@
     'latitude': 'the latitude coordinate of the country center.',
     'longitude': 'the longitude coordinate of the country center.'
 }
 
 data = pd.read_csv("data/csv/countries.csv")
 ```
 
-We then initialize our llm. By default we use GPT-4 and define our OpenAI API key in an environment variable.
+We then initialize our llm. By default we use GPT-4o and define our OpenAI API key in an environment variable.
 ```Python
 llm = LLM()
 ```
 
 And we run discovery on our data.
 ```Python
 disc = Discovery(llm=llm, user_input=USER_GENERATED_INPUT, data=data)
 disc.run()
 ```
 
 ### Data Modeling
 We can now pass our Discovery object to a GraphDataModeler to generate our initial data model. A Discovery object isn't required here, but it provides rich context to the LLM to achieve the best results.
 ```Python
 gdm = GraphDataModeler(llm=llm, discovery=disc)
-initial_model = gdm.create_initial_model()
+gdm.create_initial_model()
 ```
 If we have graphviz installed, we can take a look at our model.
 ```Python
 gdm.current_model.visualize()
 ```
 ![countries-first-model.png](./images/countries-first-model.png)
 
@@ -104,16 +104,16 @@
 ```
 Here's a snapshot of our new graph!
 
 ![countries-graph.png](./images/countries-graph-white-background.png)
 
 ## Limitations
 The current project is in beta and has the following limitations:
-- Single CSV input only
+- Single CSV input only for data model generation
 - Nodes may only have a single label
-- Only uniqueness constraints are supported
+- Only uniqueness and node / relationship key constraints are supported
 - Relationships may not have uniqueness constraints
-- CSV columns that refer to the same node property are not supported
+- CSV columns that refer to the same node property are not supported in model generation
 - Only OpenAI models may be used at this time
-- The modified PyIngest function included with Runway only supports loading a local Pandas DataFrame
+- The modified PyIngest function included with Runway only supports loading a local Pandas DataFrame or CSVs
```

### Comparing `neo4j_runway-0.2.0/neo4j_runway/discovery/discovery.py` & `neo4j_runway-0.2.1/neo4j_runway/discovery/discovery.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.2.0/neo4j_runway/ingestion/generate_ingest.py` & `neo4j_runway-0.2.1/neo4j_runway/ingestion/generate_ingest.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.2.0/neo4j_runway/ingestion/pyingest.py` & `neo4j_runway-0.2.1/neo4j_runway/ingestion/pyingest.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.2.0/neo4j_runway/llm/llm.py` & `neo4j_runway-0.2.1/neo4j_runway/llm/llm.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.2.0/neo4j_runway/modeler/modeler.py` & `neo4j_runway-0.2.1/neo4j_runway/modeler/modeler.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.2.0/neo4j_runway/objects/arrows.py` & `neo4j_runway-0.2.1/neo4j_runway/objects/arrows.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.2.0/neo4j_runway/objects/data_model.py` & `neo4j_runway-0.2.1/neo4j_runway/objects/data_model.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.2.0/neo4j_runway/objects/node.py` & `neo4j_runway-0.2.1/neo4j_runway/objects/node.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.2.0/neo4j_runway/objects/property.py` & `neo4j_runway-0.2.1/neo4j_runway/objects/property.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.2.0/neo4j_runway/objects/relationship.py` & `neo4j_runway-0.2.1/neo4j_runway/objects/relationship.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.2.0/neo4j_runway/objects/user_input.py` & `neo4j_runway-0.2.1/neo4j_runway/objects/user_input.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.2.0/neo4j_runway/resources/prompts/prompts.py` & `neo4j_runway-0.2.1/neo4j_runway/resources/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.2.0/neo4j_runway/utils/naming_conventions.py` & `neo4j_runway-0.2.1/neo4j_runway/utils/naming_conventions.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.2.0/neo4j_runway/utils/test_connection.py` & `neo4j_runway-0.2.1/neo4j_runway/utils/test_connection.py`

 * *Files identical despite different names*

### Comparing `neo4j_runway-0.2.0/pyproject.toml` & `neo4j_runway-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "neo4j-runway"
-version = "0.2.0"
+version = "0.2.1"
 description = "A Python library that contains tools for data discovery, data model generation and ingestion for the Neo4j graph database."
 authors = ["Alex Gilmore", "Jason Booth", "Dan Bukowski"]
 license = "MIT"
 readme = "README.md"
 keywords = ["graph", "neo4j", "data model"]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `neo4j_runway-0.2.0/PKG-INFO` & `neo4j_runway-0.2.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neo4j-runway
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Python library that contains tools for data discovery, data model generation and ingestion for the Neo4j graph database.
 License: MIT
 Keywords: graph,neo4j,data model
 Author: Alex Gilmore
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -59,15 +59,15 @@
 from neo4j_runway import Discovery, GraphDataModeler, IngestionGenerator, LLM, PyIngest
 
 ```
 ### Discovery
 Now we define a General Description of our data, provide brief descriptions of the columns of interest and load the data with Pandas.
 ```Python
 USER_GENERATED_INPUT = {
-    'General Description': 'This is data on different countries.',
+    'general_description': 'This is data on different countries.',
     'id': 'unique id for a country.',
     'name': 'the country name.',
     'phone_code': 'country area code.',
     'capital': 'the capital of the country.',
     'currency_name': "name of the country's currency.",
     'region': 'primary region of the country.',
     'subregion': 'subregion location of the country.',
@@ -75,30 +75,30 @@
     'latitude': 'the latitude coordinate of the country center.',
     'longitude': 'the longitude coordinate of the country center.'
 }
 
 data = pd.read_csv("data/csv/countries.csv")
 ```
 
-We then initialize our llm. By default we use GPT-4 and define our OpenAI API key in an environment variable.
+We then initialize our llm. By default we use GPT-4o and define our OpenAI API key in an environment variable.
 ```Python
 llm = LLM()
 ```
 
 And we run discovery on our data.
 ```Python
 disc = Discovery(llm=llm, user_input=USER_GENERATED_INPUT, data=data)
 disc.run()
 ```
 
 ### Data Modeling
 We can now pass our Discovery object to a GraphDataModeler to generate our initial data model. A Discovery object isn't required here, but it provides rich context to the LLM to achieve the best results.
 ```Python
 gdm = GraphDataModeler(llm=llm, discovery=disc)
-initial_model = gdm.create_initial_model()
+gdm.create_initial_model()
 ```
 If we have graphviz installed, we can take a look at our model.
 ```Python
 gdm.current_model.visualize()
 ```
 ![countries-first-model.png](./images/countries-first-model.png)
 
@@ -135,17 +135,17 @@
 ```
 Here's a snapshot of our new graph!
 
 ![countries-graph.png](./images/countries-graph-white-background.png)
 
 ## Limitations
 The current project is in beta and has the following limitations:
-- Single CSV input only
+- Single CSV input only for data model generation
 - Nodes may only have a single label
-- Only uniqueness constraints are supported
+- Only uniqueness and node / relationship key constraints are supported
 - Relationships may not have uniqueness constraints
-- CSV columns that refer to the same node property are not supported
+- CSV columns that refer to the same node property are not supported in model generation
 - Only OpenAI models may be used at this time
-- The modified PyIngest function included with Runway only supports loading a local Pandas DataFrame
+- The modified PyIngest function included with Runway only supports loading a local Pandas DataFrame or CSVs
```

