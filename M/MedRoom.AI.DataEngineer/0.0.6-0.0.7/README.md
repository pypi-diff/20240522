# Comparing `tmp/medroom_ai_dataengineer-0.0.6.tar.gz` & `tmp/medroom_ai_dataengineer-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "medroom_ai_dataengineer-0.0.6.tar", last modified: Wed May 15 19:00:54 2024, max compression
+gzip compressed data, was "medroom_ai_dataengineer-0.0.7.tar", last modified: Wed May 22 16:01:45 2024, max compression
```

## Comparing `medroom_ai_dataengineer-0.0.6.tar` & `medroom_ai_dataengineer-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 19:00:54.732989 medroom_ai_dataengineer-0.0.6/
--rw-rw-rw-   0        0        0    11558 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.6/LICENSE
-drwxrwxrwx   0        0        0        0 2024-05-15 19:00:54.730969 medroom_ai_dataengineer-0.0.6/MedRoom.AI.DataEngineer.egg-info/
--rw-rw-rw-   0        0        0    13755 2024-05-15 19:00:54.000000 medroom_ai_dataengineer-0.0.6/MedRoom.AI.DataEngineer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2024-05-15 19:00:54.000000 medroom_ai_dataengineer-0.0.6/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      115 2024-05-15 19:00:54.000000 medroom_ai_dataengineer-0.0.6/MedRoom.AI.DataEngineer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-04-12 17:49:13.000000 medroom_ai_dataengineer-0.0.6/MedRoom.AI.DataEngineer.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      139 2024-05-15 19:00:54.000000 medroom_ai_dataengineer-0.0.6/MedRoom.AI.DataEngineer.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-15 19:00:54.000000 medroom_ai_dataengineer-0.0.6/MedRoom.AI.DataEngineer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13755 2024-05-15 19:00:54.731994 medroom_ai_dataengineer-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     8428 2024-05-15 18:52:35.000000 medroom_ai_dataengineer-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 19:00:54.659638 medroom_ai_dataengineer-0.0.6/medroom/
-drwxrwxrwx   0        0        0        0 2024-05-15 19:00:54.659638 medroom_ai_dataengineer-0.0.6/medroom/dna/
-drwxrwxrwx   0        0        0        0 2024-05-15 19:00:54.725872 medroom_ai_dataengineer-0.0.6/medroom/dna/processors/
--rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.6/medroom/dna/processors/__init__.py
--rw-rw-rw-   0        0        0      663 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.6/medroom/dna/processors/config.py
--rw-rw-rw-   0        0        0      606 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.6/medroom/dna/processors/main.py
-drwxrwxrwx   0        0        0        0 2024-05-15 19:00:54.730913 medroom_ai_dataengineer-0.0.6/medroom/dna/processors/utils/
--rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.6/medroom/dna/processors/utils/__init__.py
--rw-rw-rw-   0        0        0     4385 2024-04-12 20:49:37.000000 medroom_ai_dataengineer-0.0.6/medroom/dna/processors/utils/evalmetrics.py
--rw-rw-rw-   0        0        0     4949 2024-04-20 21:31:01.000000 medroom_ai_dataengineer-0.0.6/medroom/dna/processors/utils/mlflow_helper.py
--rw-rw-rw-   0        0        0     2908 2024-04-12 22:02:34.000000 medroom_ai_dataengineer-0.0.6/medroom/dna/processors/utils/textclean.py
--rw-rw-rw-   0        0        0       42 2024-05-15 19:00:54.732989 medroom_ai_dataengineer-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1298 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:01:45.244986 medroom_ai_dataengineer-0.0.7/
+-rw-rw-rw-   0        0        0    11558 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.7/LICENSE
+drwxrwxrwx   0        0        0        0 2024-05-22 16:01:45.243030 medroom_ai_dataengineer-0.0.7/MedRoom.AI.DataEngineer.egg-info/
+-rw-rw-rw-   0        0        0    13823 2024-05-22 16:01:45.000000 medroom_ai_dataengineer-0.0.7/MedRoom.AI.DataEngineer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      578 2024-05-22 16:01:45.000000 medroom_ai_dataengineer-0.0.7/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      115 2024-05-22 16:01:45.000000 medroom_ai_dataengineer-0.0.7/MedRoom.AI.DataEngineer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-12 17:49:13.000000 medroom_ai_dataengineer-0.0.7/MedRoom.AI.DataEngineer.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      151 2024-05-22 16:01:45.000000 medroom_ai_dataengineer-0.0.7/MedRoom.AI.DataEngineer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-22 16:01:45.000000 medroom_ai_dataengineer-0.0.7/MedRoom.AI.DataEngineer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13823 2024-05-22 16:01:45.244024 medroom_ai_dataengineer-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     8428 2024-05-15 18:52:35.000000 medroom_ai_dataengineer-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 16:01:45.198265 medroom_ai_dataengineer-0.0.7/medroom/
+drwxrwxrwx   0        0        0        0 2024-05-22 16:01:45.198265 medroom_ai_dataengineer-0.0.7/medroom/dna/
+drwxrwxrwx   0        0        0        0 2024-05-22 16:01:45.238899 medroom_ai_dataengineer-0.0.7/medroom/dna/processors/
+-rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.7/medroom/dna/processors/__init__.py
+-rw-rw-rw-   0        0        0      663 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.7/medroom/dna/processors/config.py
+-rw-rw-rw-   0        0        0      606 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.7/medroom/dna/processors/main.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:01:45.241947 medroom_ai_dataengineer-0.0.7/medroom/dna/processors/utils/
+-rw-rw-rw-   0        0        0        0 2024-02-15 13:42:00.000000 medroom_ai_dataengineer-0.0.7/medroom/dna/processors/utils/__init__.py
+-rw-rw-rw-   0        0        0     4385 2024-04-12 20:49:37.000000 medroom_ai_dataengineer-0.0.7/medroom/dna/processors/utils/evalmetrics.py
+-rw-rw-rw-   0        0        0     4949 2024-04-20 21:31:01.000000 medroom_ai_dataengineer-0.0.7/medroom/dna/processors/utils/mlflow_helper.py
+-rw-rw-rw-   0        0        0     2908 2024-04-12 22:02:34.000000 medroom_ai_dataengineer-0.0.7/medroom/dna/processors/utils/textclean.py
+-rw-rw-rw-   0        0        0       42 2024-05-22 16:01:45.244986 medroom_ai_dataengineer-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1390 2024-05-22 15:59:39.000000 medroom_ai_dataengineer-0.0.7/setup.py
```

### Comparing `medroom_ai_dataengineer-0.0.6/LICENSE` & `medroom_ai_dataengineer-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.6/MedRoom.AI.DataEngineer.egg-info/PKG-INFO` & `medroom_ai_dataengineer-0.0.7/MedRoom.AI.DataEngineer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedRoom.AI.DataEngineer
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Natural Language Processing Data Engineer
 Home-page: https://github.com/MedRoomGitHub/MedRoom.AI.DataEngineer
 Author: Team IA
 Author-email: medroom@medroom.com.br
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -208,13 +208,14 @@
            limitations under the License.
         
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: nltk==3.8.1
 Requires-Dist: spacy==3.7.1
 Requires-Dist: unidecode==1.3.7
-Requires-Dist: matplotlib==3.7.0
 Requires-Dist: pandas==2.1.1
 Requires-Dist: numpy==1.26.0
-Requires-Dist: seaborn==0.13.0
 Requires-Dist: scikit-learn==1.3.1
 Requires-Dist: mlflow==2.12.2
+Provides-Extra: plotting
+Requires-Dist: matplotlib==3.7.0; extra == "plotting"
+Requires-Dist: seaborn==0.13.0; extra == "plotting"
```

### Comparing `medroom_ai_dataengineer-0.0.6/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt` & `medroom_ai_dataengineer-0.0.7/MedRoom.AI.DataEngineer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.6/PKG-INFO` & `medroom_ai_dataengineer-0.0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MedRoom.AI.DataEngineer
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Natural Language Processing Data Engineer
 Home-page: https://github.com/MedRoomGitHub/MedRoom.AI.DataEngineer
 Author: Team IA
 Author-email: medroom@medroom.com.br
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -208,13 +208,14 @@
            limitations under the License.
         
 Requires-Python: >=3.8
 License-File: LICENSE
 Requires-Dist: nltk==3.8.1
 Requires-Dist: spacy==3.7.1
 Requires-Dist: unidecode==1.3.7
-Requires-Dist: matplotlib==3.7.0
 Requires-Dist: pandas==2.1.1
 Requires-Dist: numpy==1.26.0
-Requires-Dist: seaborn==0.13.0
 Requires-Dist: scikit-learn==1.3.1
 Requires-Dist: mlflow==2.12.2
+Provides-Extra: plotting
+Requires-Dist: matplotlib==3.7.0; extra == "plotting"
+Requires-Dist: seaborn==0.13.0; extra == "plotting"
```

### Comparing `medroom_ai_dataengineer-0.0.6/README.md` & `medroom_ai_dataengineer-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.6/medroom/dna/processors/config.py` & `medroom_ai_dataengineer-0.0.7/medroom/dna/processors/config.py`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.6/medroom/dna/processors/main.py` & `medroom_ai_dataengineer-0.0.7/medroom/dna/processors/main.py`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.6/medroom/dna/processors/utils/evalmetrics.py` & `medroom_ai_dataengineer-0.0.7/medroom/dna/processors/utils/evalmetrics.py`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.6/medroom/dna/processors/utils/mlflow_helper.py` & `medroom_ai_dataengineer-0.0.7/medroom/dna/processors/utils/mlflow_helper.py`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.6/medroom/dna/processors/utils/textclean.py` & `medroom_ai_dataengineer-0.0.7/medroom/dna/processors/utils/textclean.py`

 * *Files identical despite different names*

### Comparing `medroom_ai_dataengineer-0.0.6/setup.py` & `medroom_ai_dataengineer-0.0.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,13 +18,16 @@
     version=INFO['version'],
     author=INFO['author'],
     author_email=INFO['author_email'],
     url=INFO['url'],    
     license=open(os.path.join(PROJECT_DIR, 'LICENSE')).read(),
     packages=find_namespace_packages(include=['medroom','medroom.dna', 'medroom.dna.processors', 'medroom.dna.processors.*', 'medroom.dna.processors.utils']),
     install_requires=[d for d in DEPENDENCIES if '://' not in d],
+    extras_require={
+        'plotting': ['matplotlib==3.7.0', 'seaborn==0.13.0']
+    },
     python_requires='>=3.8',
     #TO-DO: Fix dependency links : not working with bdist_wheel
     dependency_links = ["git+https://github.com/explosion/spacy-models/releases/download/pt_core_news_sm-3.2.0/pt_core_news_sm-3.2.0.tar.gz"],
     tests_require=['pytest', 'parameterized'],
     zip_safe=False
 )
```

