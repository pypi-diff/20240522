# Comparing `tmp/vectara-skunk-client-0.4.9.tar.gz` & `tmp/vectara_skunk_client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectara-skunk-client-0.4.9.tar", last modified: Fri Jan 12 21:39:23 2024, max compression
+gzip compressed data, was "vectara_skunk_client-0.5.0.tar", last modified: Wed May 22 01:25:26 2024, max compression
```

## Comparing `vectara-skunk-client-0.4.9.tar` & `vectara_skunk_client-0.5.0.tar`

### file list

```diff
@@ -1,44 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-01-12 21:39:23.366252 vectara-skunk-client-0.4.9/
--rw-rw-rw-   0        0        0    34918 2023-12-21 21:26:20.000000 vectara-skunk-client-0.4.9/LICENSE.md
--rw-rw-rw-   0        0        0      911 2024-01-12 21:39:23.365186 vectara-skunk-client-0.4.9/PKG-INFO
--rw-rw-rw-   0        0        0     5222 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/README.md
--rw-rw-rw-   0        0        0       42 2024-01-12 21:39:23.366252 vectara-skunk-client-0.4.9/setup.cfg
--rw-rw-rw-   0        0        0     1379 2024-01-12 21:38:33.000000 vectara-skunk-client-0.4.9/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-12 21:39:23.330890 vectara-skunk-client-0.4.9/test/
--rw-rw-rw-   0        0        0     5280 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/test/test_api_keys.py
--rw-rw-rw-   0        0        0     2400 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/test/test_arabic.py
--rw-rw-rw-   0        0        0     1348 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/test/test_basic_query.py
--rw-rw-rw-   0        0        0     1395 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/test/test_documents.py
--rw-rw-rw-   0        0        0     3080 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/test/test_filter_attributes.py
--rw-rw-rw-   0        0        0     1257 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/test/test_manager.py
--rw-rw-rw-   0        0        0      614 2024-01-05 23:56:06.000000 vectara-skunk-client-0.4.9/test/test_none_bool.py
--rw-rw-rw-   0        0        0     9025 2024-01-12 21:20:03.000000 vectara-skunk-client-0.4.9/test/test_query.py
--rw-rw-rw-   0        0        0      313 2023-12-29 23:40:50.000000 vectara-skunk-client-0.4.9/test/test_scratch.py
--rw-rw-rw-   0        0        0     2476 2024-01-04 21:17:59.000000 vectara-skunk-client-0.4.9/test/test_storage_quota.py
--rw-rw-rw-   0        0        0     2406 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/test/test_system_basic.py
--rw-rw-rw-   0        0        0     4780 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/test/test_util.py
-drwxrwxrwx   0        0        0        0 2024-01-12 21:39:23.331951 vectara-skunk-client-0.4.9/vectara/
--rw-rw-rw-   0        0        0        0 2023-12-22 03:08:32.000000 vectara-skunk-client-0.4.9/vectara/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-12 21:39:23.345756 vectara-skunk-client-0.4.9/vectara/client/
--rw-rw-rw-   0        0        0        0 2024-01-12 21:18:54.000000 vectara-skunk-client-0.4.9/vectara/client/__init__.py
--rw-rw-rw-   0        0        0     7940 2024-01-12 21:20:43.000000 vectara-skunk-client-0.4.9/vectara/client/admin.py
--rw-rw-rw-   0        0        0     4266 2023-12-28 02:17:55.000000 vectara-skunk-client-0.4.9/vectara/client/authn.py
--rw-rw-rw-   0        0        0     2157 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/vectara/client/chat.py
--rw-rw-rw-   0        0        0     7525 2023-12-29 00:18:13.000000 vectara-skunk-client-0.4.9/vectara/client/config.py
--rw-rw-rw-   0        0        0     4337 2024-01-12 21:20:03.000000 vectara-skunk-client-0.4.9/vectara/client/core.py
--rw-rw-rw-   0        0        0     3173 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/vectara/client/dao.py
--rw-rw-rw-   0        0        0     1472 2024-01-12 21:21:41.000000 vectara-skunk-client-0.4.9/vectara/client/document.py
--rw-rw-rw-   0        0        0    10583 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/vectara/client/domain.py
--rw-rw-rw-   0        0        0      640 2024-01-05 05:12:20.000000 vectara-skunk-client-0.4.9/vectara/client/enums.py
--rw-rw-rw-   0        0        0        0 2024-01-04 05:06:30.000000 vectara-skunk-client-0.4.9/vectara/client/error.py
--rw-rw-rw-   0        0        0     3886 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/vectara/client/index.py
--rw-rw-rw-   0        0        0     1593 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/vectara/client/manager.py
--rw-rw-rw-   0        0        0     5301 2024-01-12 21:21:14.000000 vectara-skunk-client-0.4.9/vectara/client/query.py
--rw-rw-rw-   0        0        0     5131 2024-01-12 05:54:06.000000 vectara-skunk-client-0.4.9/vectara/client/status.py
--rw-rw-rw-   0        0        0    19359 2024-01-12 21:20:02.000000 vectara-skunk-client-0.4.9/vectara/client/util.py
-drwxrwxrwx   0        0        0        0 2024-01-12 21:39:23.364120 vectara-skunk-client-0.4.9/vectara_skunk_client.egg-info/
--rw-rw-rw-   0        0        0      911 2024-01-12 21:39:23.000000 vectara-skunk-client-0.4.9/vectara_skunk_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      934 2024-01-12 21:39:23.000000 vectara-skunk-client-0.4.9/vectara_skunk_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-12 21:39:23.000000 vectara-skunk-client-0.4.9/vectara_skunk_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2024-01-12 21:39:23.000000 vectara-skunk-client-0.4.9/vectara_skunk_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-01-12 21:39:23.000000 vectara-skunk-client-0.4.9/vectara_skunk_client.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 01:25:26.736508 vectara_skunk_client-0.5.0/
+-rw-rw-rw-   0        0        0    34918 2023-12-21 21:26:20.000000 vectara_skunk_client-0.5.0/LICENSE.md
+-rw-rw-rw-   0        0        0      911 2024-05-22 01:25:26.735494 vectara_skunk_client-0.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5223 2024-04-30 03:30:49.000000 vectara_skunk_client-0.5.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 01:25:26.736508 vectara_skunk_client-0.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1830 2024-05-22 01:22:37.000000 vectara_skunk_client-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:25:26.583928 vectara_skunk_client-0.5.0/test/
+-rw-rw-rw-   0        0        0     1759 2024-05-22 01:11:31.000000 vectara_skunk_client-0.5.0/test/test_core_index.py
+-rw-rw-rw-   0        0        0      421 2024-05-22 01:03:28.000000 vectara_skunk_client-0.5.0/test/test_index.py
+-rw-rw-rw-   0        0        0     1259 2024-05-02 01:30:04.000000 vectara_skunk_client-0.5.0/test/test_manager.py
+-rw-rw-rw-   0        0        0      614 2024-01-05 23:56:06.000000 vectara_skunk_client-0.5.0/test/test_none_bool.py
+-rw-rw-rw-   0        0        0     9883 2024-02-06 04:39:48.000000 vectara_skunk_client-0.5.0/test/test_query.py
+-rw-rw-rw-   0        0        0      320 2024-01-12 22:21:17.000000 vectara_skunk_client-0.5.0/test/test_scratch.py
+-rw-rw-rw-   0        0        0     2476 2024-01-04 21:17:59.000000 vectara_skunk_client-0.5.0/test/test_storage_quota.py
+-rw-rw-rw-   0        0        0     2406 2024-01-12 21:20:02.000000 vectara_skunk_client-0.5.0/test/test_system_basic.py
+-rw-rw-rw-   0        0        0     4780 2024-01-12 22:21:17.000000 vectara_skunk_client-0.5.0/test/test_util.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:25:26.709491 vectara_skunk_client-0.5.0/vectara_client/
+-rw-rw-rw-   0        0        0        0 2023-12-22 03:08:32.000000 vectara_skunk_client-0.5.0/vectara_client/__init__.py
+-rw-rw-rw-   0        0        0    11506 2024-04-30 04:34:01.000000 vectara_skunk_client-0.5.0/vectara_client/admin.py
+-rw-rw-rw-   0        0        0     4350 2024-05-07 04:36:22.000000 vectara_skunk_client-0.5.0/vectara_client/authn.py
+-rw-rw-rw-   0        0        0     2232 2024-01-12 22:54:50.000000 vectara_skunk_client-0.5.0/vectara_client/chat.py
+-rw-rw-rw-   0        0        0     7769 2024-05-03 06:58:11.000000 vectara_skunk_client-0.5.0/vectara_client/config.py
+-rw-rw-rw-   0        0        0     4551 2024-05-17 00:41:53.000000 vectara_skunk_client-0.5.0/vectara_client/core.py
+-rw-rw-rw-   0        0        0     8778 2024-05-22 01:16:34.000000 vectara_skunk_client-0.5.0/vectara_client/corpus.py
+-rw-rw-rw-   0        0        0     3173 2024-01-12 22:21:17.000000 vectara_skunk_client-0.5.0/vectara_client/dao.py
+-rw-rw-rw-   0        0        0     1472 2024-01-12 22:21:17.000000 vectara_skunk_client-0.5.0/vectara_client/document.py
+-rw-rw-rw-   0        0        0    12369 2024-05-22 00:57:33.000000 vectara_skunk_client-0.5.0/vectara_client/domain.py
+-rw-rw-rw-   0        0        0      761 2024-04-09 05:47:51.000000 vectara_skunk_client-0.5.0/vectara_client/enums.py
+-rw-rw-rw-   0        0        0        0 2024-01-04 05:06:30.000000 vectara_skunk_client-0.5.0/vectara_client/error.py
+-rw-rw-rw-   0        0        0     5352 2024-05-22 00:59:33.000000 vectara_skunk_client-0.5.0/vectara_client/index.py
+-rw-rw-rw-   0        0        0     1594 2024-05-02 01:29:30.000000 vectara_skunk_client-0.5.0/vectara_client/manager.py
+-rw-rw-rw-   0        0        0     6086 2024-03-26 02:59:13.000000 vectara_skunk_client-0.5.0/vectara_client/query.py
+-rw-rw-rw-   0        0        0     5830 2024-03-04 06:43:34.000000 vectara_skunk_client-0.5.0/vectara_client/status.py
+-rw-rw-rw-   0        0        0    20575 2024-05-22 01:22:07.000000 vectara_skunk_client-0.5.0/vectara_client/util.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:25:26.733491 vectara_skunk_client-0.5.0/vectara_skunk_client.egg-info/
+-rw-rw-rw-   0        0        0      911 2024-05-22 01:25:26.000000 vectara_skunk_client-0.5.0/vectara_skunk_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      861 2024-05-22 01:25:26.000000 vectara_skunk_client-0.5.0/vectara_skunk_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 01:25:26.000000 vectara_skunk_client-0.5.0/vectara_skunk_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2024-05-22 01:25:26.000000 vectara_skunk_client-0.5.0/vectara_skunk_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-22 01:25:26.000000 vectara_skunk_client-0.5.0/vectara_skunk_client.egg-info/top_level.txt
```

### Comparing `vectara-skunk-client-0.4.9/LICENSE.md` & `vectara_skunk_client-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `vectara-skunk-client-0.4.9/PKG-INFO` & `vectara_skunk_client-0.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectara-skunk-client
-Version: 0.4.9
+Version: 0.5.0
 Summary: Vectara Skunk Client
 Home-page: https://github.com/davidglevy/vectara-skunk-client
 Author: David Levy
 Author-email: david.g.levy@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE v3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

### Comparing `vectara-skunk-client-0.4.9/README.md` & `vectara_skunk_client-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 5. Build awesome GenerativeAI applications.
 
 ```bash
 pip install vectara-skunk-client
 ```
 
 ```python
-from vectara.client.core import Factory
+from vectara_client.core import Factory
 
 client = Factory().build()
 # Upload our document
 client.indexer_service.upload(path="./santas_workshop_info.pdf", corpus_id=1)
 # Run query
 client.query_service.query("Where does Santa live?")
 
@@ -50,16 +50,16 @@
 2. Param `config_json`: If a JSON configuration is passed in then this will be used.
 3. If neither has been specified, we will look in the users home directory
 
 <img src="./resources/images/factory-build-flow.png" alt="factory build flow" style="width:600px;"/>
 
 ### Home Location
 The factory by default will automatically seek configuration in the following locations:
-* On Linux based systems from within $HOME/.vec/auth.yaml
-* On Windows based systems from within %USERHOME%\.vec\auth.yaml
+* On Linux based systems from within $HOME/.vec_auth.yaml
+* On Windows based systems from within %USERHOME%\\.vec_auth.yaml
 
 ### Configuration Format
 The configuration format should like below. You can define multiple configuration blocks. If not specified,
 the factory will load the profile "default". You must specify your customer_id but may 
 
 ```yaml
 default:
@@ -77,26 +77,26 @@
     auth_url : "https://vectara-prod-YOUR_CUSTOMER_ID.auth.us-west-2.amazoncognito.com/oauth2/token"
 ```
 
 ### Multiple Profiles
 You can load other configuration profiles using the property profile on the build command.
 
 ```python
-from vectara.client.core import Factory
+from vectara_client.core import Factory
 
 factory = Factory()
 client = factory.build(profile="admin")
 
 ```
 
 ### Dynamic Configuration
 You can also inject the configuration for the client by putting in a JSON string of the following formats
 
 ```python
-from vectara.client.core import Factory
+from vectara_client.core import Factory
 
 auth_config_json = "{...}"
 client = Factory().build(config=auth_config_json)
 ```
 
 #### JSON API Key
 ```json
```

### Comparing `vectara-skunk-client-0.4.9/setup.py` & `vectara_skunk_client-0.5.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,23 @@
 from setuptools import setup
+import unittest
+import logging
+from unittest import TestSuite
 
+logging.basicConfig(format='%(asctime)s:%(name)-35s %(levelname)s:%(message)s', level=logging.INFO,
+                    datefmt='%H:%M:%S %z')
+
+logger = logging.getLogger(__name__)
+
+
+def my_test_suite():
+    test_loader = unittest.TestLoader()
+
+    test_suites = test_loader.discover('test', pattern='*_test.py')
+    return test_suites
 
 def get_long_desc() -> str:
     with open('README.md', 'r') as file_handle:
         lines = []
         for line in next(file_handle):
             if len(line.strip()) == 0:
                 break
@@ -12,29 +26,30 @@
         return "\n".join(lines)
 
 setup(
     name='vectara-skunk-client',
     description='Vectara Skunk Client',
     long_description=get_long_desc(),
     long_description_content_type='text/markdown',
-    version='0.4.9',
+    version='0.5.0',
     author='David Levy',
     author_email='david.g.levy@gmail.com',
     url='https://github.com/davidglevy/vectara-skunk-client',
     license='GNU AFFERO GENERAL PUBLIC LICENSE v3',
     package_dir={
-        'vectara.client': 'vectara/client'
+        'vectara_client': 'vectara_client'
     },
-    packages=['vectara.client'],
+    packages=['vectara_client'],
     install_requires=['requests', 'dacite>=1.8.1', 'Authlib==1.0.1', 'pyaml==23.9.7', 'tqdm==4.66.1',
                       'requests-toolbelt==1.0.0'],
     python_requires='>=3.4',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Environment :: Console',
         'License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python :: 3 :: Only',
         'Programming Language :: Python :: 3.12',
         'Topic :: Utilities'
-    ]
+    ],
+    test_suite='setup.my_test_suite'
 )
```

### Comparing `vectara-skunk-client-0.4.9/test/test_manager.py` & `vectara_skunk_client-0.5.0/test/test_manager.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 import logging
-from vectara.client.core import Factory
-from vectara.client.manager import VectaraManager
-from vectara.client.dao import ManagerDao, CorpusDao
+from vectara_client.core import Factory
+from vectara_client.manager import DatabaseManager
+from vectara_client.dao import ManagerDao, CorpusDao
 
 import os
 
 logging.basicConfig(
 format='%(levelname)-5s:%(name)-35s:%(message)s', level=logging.INFO
 )
 
@@ -29,15 +29,15 @@
         self.indexer_service = client.indexer_service
 
         # Check existing corpus doesn't exist
 
         self.managerDao = ManagerDao()
         self.corpusDao = CorpusDao()
 
-        self.target = VectaraManager(client, self.managerDao, self.corpusDao, self.admin_service)
+        self.target = DatabaseManager(client, self.managerDao, self.corpusDao, self.admin_service)
 
     def test(self):
         # TODO Extract the manager from this project!!
         pass
         #self.target.sync_local_db()
```

### Comparing `vectara-skunk-client-0.4.9/test/test_none_bool.py` & `vectara_skunk_client-0.5.0/test/test_none_bool.py`

 * *Files identical despite different names*

### Comparing `vectara-skunk-client-0.4.9/test/test_query.py` & `vectara_skunk_client-0.5.0/test/test_query.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from test.base import BaseClientTest
-from vectara.client.util import render_markdown, SimplePromptFactory, StandardPromptFactory
-from vectara.client.chat import ChatHelper
+from vectara_client.util import render_markdown, SimplePromptFactory, StandardPromptFactory
+from vectara_client.chat import ChatHelper
 from test.util import create_test_corpus
 from pathlib import Path
 
 
 class QueryIntegrationTest(BaseClientTest):
 
 
@@ -87,22 +87,35 @@
     def test_query_with_prompt_generator_standard(self):
         """
         Test out the promptText value
 
         :return:
         """
         qs = self.client.query_service
-        query = "At Vectara, Can I bring any birds to the Vectara Office?"
+        query = "Whats happening?"
         system_prompt = 'You are a human resources manager who takes the search results and summarizes them as a coherent response. Only use information provided in this chat. Respond in the language denoted by ISO 639 code \\"$vectaraLangCode\\".'
         user_prompt = 'Generate a detailed answer (that is no more than 300 words) for the query \\"$esc.java(${vectaraQuery})\\" solely based on the search results in this chat. You must only use information from the provided results. Cite search results using \\"[number]\\" notation. Only cite the most relevant results that answer the question accurately.'
 
         prompt_factory = StandardPromptFactory(system_prompt=system_prompt, user_prompt=user_prompt)
         prompt_text = prompt_factory.build()
 
-        response = qs.query(query, 126, promptText=prompt_text)
+        response = qs.query(query, 326, promptText=prompt_text)
+
+        self.logger.info(render_markdown(query, response))
+
+    def test_twitter_events(self):
+        qs = self.client.query_service
+        query = "Saudi Arabia"
+        system_prompt = 'You are a public relations manager looking at events from Twitter who takes the search results and summarizes them as a coherent response. Only use information provided in this chat. Respond in the language denoted by ISO 639 code \\"$vectaraLangCode\\".'
+        user_prompt = 'Please look through the previous answers and summarize, in less than 300 words, what is happening in relation to the topic \\"$esc.java(${{vectaraQuery}})\\" based only on the interactions in this chat'
+
+        prompt_factory = StandardPromptFactory(system_prompt=system_prompt, user_prompt=user_prompt)
+        prompt_text = prompt_factory.build()
+
+        response = qs.query(query, 326, promptText=prompt_text)
 
         self.logger.info(render_markdown(query, response))
 
     def test_query_with_prompt_generator_simple(self):
 
         """
         Test out the promptText value
```

### Comparing `vectara-skunk-client-0.4.9/test/test_storage_quota.py` & `vectara_skunk_client-0.5.0/test/test_storage_quota.py`

 * *Files identical despite different names*

### Comparing `vectara-skunk-client-0.4.9/test/test_system_basic.py` & `vectara_skunk_client-0.5.0/test/test_system_basic.py`

 * *Files identical despite different names*

### Comparing `vectara-skunk-client-0.4.9/test/test_util.py` & `vectara_skunk_client-0.5.0/test/test_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from unittest import TestCase
-from vectara.client.util import render_markdown, SimplePromptFactory
-from vectara.client.domain import ResponseSet
+from vectara_client.util import render_markdown, SimplePromptFactory
+from vectara_client.domain import ResponseSet
 from dacite import from_dict
 
 
 class RenderMarkdownTest(TestCase):
 
     def __init__(self, methodName="runTest"):
         super().__init__(methodName)
```

### Comparing `vectara-skunk-client-0.4.9/vectara/client/authn.py` & `vectara_skunk_client-0.5.0/vectara_client/authn.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,23 +5,28 @@
 import logging
 from authlib.integrations.requests_client import OAuth2Session
 import datetime
 import traceback
 from abc import ABC
 
 # TODO This should be discovered from the console
+# TODO Change this file to authc.py!!
 DEFAULT_OAUTH2_URL = "https://vectara-prod-{customer_id}.auth.us-west-2.amazoncognito.com/oauth2/token"
 
 logger = logging.getLogger(__name__)
 
+
 class BaseAuthUtil(ABC):
 
     def get_headers(self) -> dict:
         raise NotImplementedError("You must implement this on a subclass")
 
+    def authenticate(self):
+        pass
+
 class OAuthUtil(BaseAuthUtil):
 
     def __init__(self, auth_url: str, app_client_id: str, app_client_secret: str, customer_id: str):
         self.logger = logging.getLogger(str(__class__.__name__))
 
         if not customer_id:
             # Putting this in as I'm surprised we also need a customer Id on the header.
@@ -56,15 +61,14 @@
 
         self.expiry_ts = None
         self.expiry_txt = None
         self.expires_in = None
         self.expires_at = None
         self.access_token = None
 
-
     def authenticate(self):
         """Connect to the server and get a JWT token."""
 
 #        try:
         session = OAuth2Session(
             self.app_client_id, self.app_client_secret, scope="")
         token = session.fetch_token(self.auth_url, grant_type="client_credentials")
```

### Comparing `vectara-skunk-client-0.4.9/vectara/client/chat.py` & `vectara_skunk_client-0.5.0/vectara_client/chat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from vectara.client.util import ChatPromptFactory, render_markdown
-from vectara.client.query import QueryService
+from vectara_client.util import ChatPromptFactory, render_markdown
+from vectara_client.query import QueryService
 import logging
 
 
 class ChatHelper:
 
     def __init__(self, corpus_id: int, qs: QueryService, customer_name:str,
                  chat_persona="Customer Service", name="Fiona",
@@ -29,15 +29,16 @@
         prompt_text = self.prompt_factory.build()
         # self.logger.info(f"Prompt text is:\n {prompt_text}")
 
         #self.qs.query(query, self.corpus_id, prompt_text)
 
         response = self.qs.query(query, self.corpus_id, promptText=prompt_text, response_lang=self.resp_lang,
                                  context_config=self.context_config, re_rank=self.re_rank,
-                                 summary_result_count=self.summary_result_count, page_size=self.page_size)
+                                 summary_result_count=self.summary_result_count, page_size=self.page_size,
+                                 summarizer="vectara-summary-ext-v1.3.0")
 
         if self.log_response:
             self.logger.info(render_markdown(query, response, show_search_results=False))
 
         summary_response = response.summary[0].text
 
         # Now we add the additional context to  the factory.
```

### Comparing `vectara-skunk-client-0.4.9/vectara/client/config.py` & `vectara_skunk_client-0.5.0/vectara_client/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import logging
 from abc import ABC
 from dataclasses import dataclass
-from dacite import from_dict, Config, UnexpectedDataError
+from dacite import from_dict, Config, UnexpectedDataError, UnionMatchError
 from typing import Optional, Union, Any
 import json
 import yaml
 from os import path, sep
 from pathlib import Path
 
 """
@@ -75,16 +75,24 @@
 
     :param config: the input configuration in JSON format.
     :return: the parsed client configuration1
     :raises TypeError: if the configuration cannot be parsed correctly
     """
     logger.info(f"Loading config from {config}")
 
-    config_dict = json.loads(config)
+    try:
+        config_dict = json.loads(config)
+
+
 
+        return from_dict(ClientConfig, config_dict, config=Config(strict=True))
+    except UnionMatchError as e:
+        raise TypeError(e)
+    except UnexpectedDataError as e:
+        raise TypeError(e)
 
 class BaseConfigLoader(ABC):
     CONFIG_FILE_NAME = ".vec_auth.yaml"
 
     DEFAULT_CONFIG_NAME = "default"
 
     def __init__(self, profile: str = None):
```

### Comparing `vectara-skunk-client-0.4.9/vectara/client/core.py` & `vectara_skunk_client-0.5.0/vectara_client/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 import logging
-from vectara.client.config import JsonConfigLoader, PathConfigLoader, HomeConfigLoader
-from vectara.client.authn import OAuthUtil, ApiKeyUtil
-from vectara.client.admin import AdminService
-from vectara.client.document import DocumentService
-from vectara.client.index import IndexerService
-from vectara.client.query import QueryService
-from vectara.client.util import RequestUtil
+from vectara_client.config import JsonConfigLoader, PathConfigLoader, HomeConfigLoader
+from vectara_client.authn import OAuthUtil, ApiKeyUtil
+from vectara_client.admin import AdminService
+from vectara_client.document import DocumentService
+from vectara_client.index import IndexerService
+from vectara_client.query import QueryService
+from vectara_client.util import RequestUtil
+from vectara_client.corpus import CorpusManager
 
 
 class Client:
 
     def __init__(self, customer_id: str, admin_service: AdminService,
                  indexer_service: IndexerService, query_service: QueryService,
                  document_service: DocumentService,
-                 request_util: RequestUtil):
+                 request_util: RequestUtil, corpus_manager: CorpusManager):
         self.logging = logging.getLogger(self.__class__.__name__)
         logging.info("initializing Client")
         self.customer_id = customer_id
         self.admin_service = admin_service
         self.indexer_service = indexer_service
         self.query_service = query_service
         self.document_service = document_service
         self.request_util = request_util
+        self.corpus_manager = corpus_manager
 
     def get_requests(self):
         return self.request_util.requests
 
 class Factory():
 
     def __init__(self, config_path: str = None, config_json: str = None, profile: str = None):
@@ -86,10 +88,11 @@
         # TODO Use the type of authentication to validate whether we can enabled the admin service.
         request_util = RequestUtil(auth_util)
 
         admin_service = AdminService(request_util, int(client_config.customer_id))
         indexer_service = IndexerService(auth_util, request_util, int(client_config.customer_id))
         query_service = QueryService(request_util, int(client_config.customer_id))
         document_service = DocumentService(request_util)
+        corpus_manager = CorpusManager(admin_service, indexer_service)
 
         return Client(client_config.customer_id, admin_service, indexer_service, query_service, document_service,
-                      request_util)
+                      request_util, corpus_manager)
```

### Comparing `vectara-skunk-client-0.4.9/vectara/client/dao.py` & `vectara_skunk_client-0.5.0/vectara_client/dao.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from vectara.client.domain import Corpus
+from vectara_client.domain import Corpus
 from abc import ABC
 import sqlite3
 import logging
 from typing import List, Any
 from dataclasses import asdict
```

### Comparing `vectara-skunk-client-0.4.9/vectara/client/document.py` & `vectara_skunk_client-0.5.0/vectara_client/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from vectara.client.domain import *
+from vectara_client.domain import *
 from typing import List, TypeVar
-from vectara.client.util import RequestUtil, convertAttrListToDict
+from vectara_client.util import RequestUtil, convertAttrListToDict
 import logging
 
 T = TypeVar("T")
 
 class DocumentService():
 
     def __init__(self, request_util: RequestUtil):
```

### Comparing `vectara-skunk-client-0.4.9/vectara/client/domain.py` & `vectara_skunk_client-0.5.0/vectara_client/domain.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Optional, Union
 from enum import Enum
-from vectara.client.status import Status
-from vectara.client.enums import ApiKeyStatus, ApiKeyType
+from vectara_client.status import Status
+from vectara_client.enums import ApiKeyStatus, ApiKeyType
 
 from dataclasses import dataclass
 
 """
 Definitions taken from admin.proto in platform.
 """
 
@@ -27,16 +27,16 @@
     FILTER_ATTRIBUTE_LEVEL__DOCUMENT_PART = 10  # Part - level attribute
 
 
 @dataclass
 class Dimension:
     name: str
     description: str
-    serving_default: str
-    indexing_default: str
+    serving_default: float
+    indexing_default: float
 
 
 @dataclass
 class FilterAttribute:
     name: str
     description: Optional[str]
     indexed: bool
@@ -70,15 +70,16 @@
     customDimensions: Optional[List[Dimension]]
     filterAttributes: Optional[List[FilterAttribute]]
 
 
 @dataclass
 class ListCorpusResponse:
     corpus: List[Corpus]
-
+    pageKey: str
+    status: Optional[Status]
 
 @dataclass
 class ReadCorpusRequest:
     corpus_id: List[int]
     read_basic_info: bool
     read_size: bool
     read_recall: bool
@@ -120,15 +121,15 @@
             self.status = ApiKeyStatus[self.status]
 
 
 @dataclass
 class CorpusInfo:
     corpus: Corpus
     corpusStatus: Status  # Different from proto: corpus_status
-    size: CorpusSize
+    size: Optional[CorpusSize]
     sizeStatus: Status  # Different from proto: size_status
     recall: Optional[CorpusRecall]
     recallStatus: Optional[Status]
     apiKey: List[ApiKey]
     # Test from here
     apiKeyStatus: Optional[Status]
     customDimension: List[Dimension]
@@ -283,26 +284,47 @@
 
 
 @dataclass
 class RerankingConfig:
     rerankerId: int
     mmrConfig: Optional[MMRConfig]
 
+@dataclass
+class ModelParams:
+    maxTokens: Optional[int]
+    temperature: Optional[float]
+
+    # provides even more granular control to help ensure that the summarization decreases the likelihood of repeating words. The values range from 0.0 to 1.0
+    frequencyPenalty: Optional[float]
+
+    # provides more control over whether you want the summary to include new topics. The values also range from 0.0 to 1.0.
+    presencePenalty: Optional[float]
+
+
+@dataclass
+class ChatRequest:
+    store: Optional[bool]
+    conversationId: Optional[str]
+
 
 @dataclass
 class Summarizer:
     summarizerPromptName: str
     promptText: Optional[str]
     responseLang: str
     maxSummarizedResults: int
+    debug: Optional[bool]
+    chat: Optional[ChatRequest]
+    modelParams: Optional[ModelParams]
 
 
 @dataclass
 class QueryBody:
     query: str
+    queryContext: str
     start: Optional[int]
     numResults: Optional[int]
     contextConfig: Optional[QueryContextConfig]
     corpusKey: List[CorpusKey]
     rerankingConfig: Optional[RerankingConfig]
     summary: Optional[List[Summarizer]]
 
@@ -330,21 +352,28 @@
 
 
 @dataclass
 class ResponseDocument:
     id: str
     metadata: List[Attribute]
 
+@dataclass
+class ChatResponse:
+    conversationId: str
+    turnId: Optional[str]
+    rephrasedQuery: Optional[str]
+    status: Optional[Status]
 
 @dataclass
 class SummaryResponse:
     text: Optional[str]
     lang: str
     prompt: str
     status: List[Status]
+    chat: Optional[ChatResponse]
     # Do we need to serialize "futureId"?
 
 
 @dataclass
 class ResponseSet:
     response: List[Response]
     status: List[Status]
@@ -362,44 +391,80 @@
 
 @dataclass
 class BatchQueryResponse:
     responseSet: Optional[List[ResponseSet]]
     status: List[Status]
     metrics: Optional[PerformanceMetrics]
 
+@dataclass
+class CoreIndexDocumentPart:
+    text: str
+    context: Optional[str]
+    metadata_json: Optional[str]
+    custom_dims: Optional[List[CustomDimension]]
+
+@dataclass
+class CoreIndexDocument:
+    document_id: str
+    metadata_json: Optional[str]
+    parts: List[CoreIndexDocumentPart]
+
+@dataclass
+class CoreIndexDocumentRequest:
+    """
+    See core_services.proto
+    """
+    customer_id: int
+    corpus_id: int
+    document: CoreIndexDocument
+
+@dataclass
+class CoreIndexDocumentResponse:
+    """
+    See core_services.proto
+    """
+    status: Status
+    quotaConsumed: Optional[StorageQuota]
+
+    def __post_init__(self):
+        """
+        Funky behavior to clear the status if it doesn't have a code
+        """
+        if not self.status.code:
+            self.__setattr__("status", None)
 
 @dataclass
-class CoreDocumentPart:
+class DocumentSection:
     text: Optional[str]
     context: Optional[str]
     metadata_json: Optional[str]
     custom_dims: Optional[List[CustomDimension]]
 
 
 @dataclass
-class CoreDocument:
+class IndexDocument:
     """
     Something odd
     """
     document_id: str
     title: str
     metadata_json: Optional[str]
-    section: Optional[List[CoreDocumentPart]]
+    section: Optional[List[DocumentSection]]
     # default_part_context: Optional[str]
     custom_dims: Optional[List[CustomDimension]]
 
 
 @dataclass
 class IndexDocumentRequest:
     """
     See core_services.proto
     """
     customer_id: int
     corpus_id: int
-    document: CoreDocument
+    document: IndexDocument
 
 
 @dataclass
 class IndexDocumentResponse:
     """
     See core_services.proto
     """
@@ -464,24 +529,24 @@
 class ListDocumentItem:
     id: str
     metadata: Optional[List[Attribute]]
 
 @dataclass
 class DocumentDTO:
     id: str
-    metadata: dict[str, Union[str, int, float, bool]]
+    metadata: dict[str, Union[str, int, float, bool, List[str]]]
 
 
 @dataclass
 class ListDocumentsResponse:
     document: List[ListDocumentItem]
     nextPageKey: str
 
 
 @dataclass
 class PagedApiKeyResponse:
-    # FIXME Move this into vectara-client-manager
+    # FIXME Move this into vectara_client-client-manager
     total_results: int
     total_pages: int
     current_page: int
     page_size: int
 #    sort_field:
```

### Comparing `vectara-skunk-client-0.4.9/vectara/client/index.py` & `vectara_skunk_client-0.5.0/vectara_client/index.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,25 +8,26 @@
 @Links: https://docs.vectara.com/docs/api-reference/indexing-apis/deleting-documents
 
 Tasks
 * TODO We should provide a method to check prior uploads via sha1_hash as per BaseClientTest
 * TODO There's likely a higher abstraction here which will check for doc existing and allow overwrites (CorpusManager?)
 * TODO Investigate whether I need the lower level API too
 """
-from vectara.client.authn import BaseAuthUtil
-from vectara.client.domain import UploadDocumentResponse, CoreDocument, IndexDocumentRequest, IndexDocumentResponse
-from vectara.client.util import RequestUtil
-from typing import Union
+from vectara_client.authn import BaseAuthUtil
+from vectara_client.domain import (UploadDocumentResponse, IndexDocumentRequest, IndexDocumentResponse,
+                                   IndexDocument, CoreIndexDocumentRequest, CoreIndexDocument,
+                                   CoreIndexDocumentResponse)
+from vectara_client.util import RequestUtil
+from typing import Union, List
 from pathlib import Path
 from dacite import from_dict
 from dataclasses import asdict
 import logging
 import json
 
-
 class IndexerService:
     """
     Wrapper for the Vectara index REST API
 
     One instantiation per customer id
 
     """
@@ -40,49 +41,78 @@
         :param customer_id: the customer id for this account
         """
         self.logger = logging.getLogger(__class__.__name__)
         self.request_util = request_util
         self.customer_id = customer_id
         self.auth_util = auth_util
 
-    def index_doc(self, corpus_id: int, document: Union[dict, CoreDocument]):
+    def index_doc(self, corpus_id: int, document: Union[dict, IndexDocument]) -> IndexDocumentResponse:
         """
         Indexes the give document which is already in a format that is ready to be added to the embedding.
 
         It is worth noting that this API can either take a dict or a CoreDocument, however the dict will
         be validated against the CoreDocument schema.
 
         :param corpus_id: the corpus to put the document in
         :param document: either a dict which will be validated against CoreDocument, or a CoreDocument.
         :return:
         """
         # Convert singular int to List of corpus ids.
         if type(document) is dict:
-            domain = from_dict(CoreDocument, document)
+            domain = from_dict(IndexDocument, document)
         else:
             domain = document
 
         # Now Convert back to dict, knowing that our parameter is type safe.
         # FIXME Ask Tallat why the customer ID for this API is an integer (unexpected)
         request = IndexDocumentRequest(int(self.customer_id), corpus_id, domain)
         payload = asdict(request)
 
         result = self.request_util.request('index', payload, to_class=IndexDocumentResponse)
         return result
 
+    def index_core_doc(self, corpus_id: int, document: Union[dict, CoreIndexDocument]) -> CoreIndexDocumentResponse:
+        """
+        Indexes the give document which is already in a format that is ready to be added to the embedding.
+
+        It is worth noting that this API can either take a dict or a CoreDocument, however the dict will
+        be validated against the CoreDocument schema.
+
+        :param corpus_id: the corpus to put the document in
+        :param document: either a dict which will be validated against CoreDocument, or a CoreDocument.
+        :return:
+        """
+        # Convert singular int to List of corpus ids.
+        if type(document) is dict:
+            domain = from_dict(CoreIndexDocument, document)
+        else:
+            domain = document
+
+        # Now Convert back to dict, knowing that our parameter is type safe.
+        # FIXME Ask Tallat why the customer ID for this API is an integer (unexpected)
+        request = CoreIndexDocumentRequest(int(self.customer_id), corpus_id, domain)
+        payload = asdict(request)
+
+        result = self.request_util.request('core/index', payload, to_class=CoreIndexDocumentResponse)
+        return result
+
+
 
     def upload(self, corpus_id: int, path: Union[str, Path] = None, input_contents: bytes = None, input_file_name: str = None,
-               return_extracted: bool = None, metadata: dict = None) -> UploadDocumentResponse:
+               return_extracted: bool = None, metadata: dict = None, ocr = False) -> UploadDocumentResponse:
         headers = {'c': str(self.customer_id), 'o': str(corpus_id)}
         self.logger.info(f"Headers: {json.dumps(headers)}")
 
         params = {'c': str(self.customer_id), 'o': str(corpus_id)}
         if return_extracted:
             params['d'] = str(True)
 
+        if ocr:
+            params['ocr'] = "true"
+
         if metadata:
             params['doc_metadata'] = json.dumps(metadata)
 
         return self.request_util.multipart_post("upload", path_str=path, input_contents=input_contents, input_file_name=input_file_name, params=params, headers=headers)
 
 
     def delete(self, corpus_id: int, document_id: str):
```

### Comparing `vectara-skunk-client-0.4.9/vectara/client/manager.py` & `vectara_skunk_client-0.5.0/vectara_client/manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 from typing import List
-from vectara.client.core import Client
-from vectara.client.dao import ManagerDao, CorpusDao
-from vectara.client.admin import AdminService
+from vectara_client.core import Client
+from vectara_client.dao import ManagerDao, CorpusDao
+from vectara_client.admin import AdminService
 
-class VectaraManager():
+class DatabaseManager():
 
     def __init__(self,client:Client, dao:ManagerDao, corpusDao:CorpusDao, adminService:AdminService):
         self.logger = logging.getLogger(__class__.__name__)
         self.client = client
         self.dao = dao
         self.corpusDao = corpusDao
         self.adminService = adminService
```

### Comparing `vectara-skunk-client-0.4.9/vectara/client/query.py` & `vectara_skunk_client-0.5.0/vectara_client/query.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from dataclasses import asdict
-from vectara.client.domain import *
+from vectara_client.domain import *
 from dacite import from_dict
 from typing import List, TypeVar, Union
-from vectara.client.status import StatusCode
-from vectara.client.util import _custom_asdict_factory, RequestUtil
+from vectara_client.status import StatusCode
+from vectara_client.util import _custom_asdict_factory, RequestUtil
 import logging
 import re
 
 T = TypeVar("T")
 
 
 class SummaryError(Exception):
@@ -23,16 +23,18 @@
     def __init__(self, request_util: RequestUtil, customer_id: int):
         self.logger = logging.getLogger(__class__.__name__)
         self.request_util = request_util
         self.customer_id = customer_id
 
     def query(self, query_text: str, corpus_id: Union[int, List[int]], start: int = 0, page_size: int = 10,
               summary: bool = True, response_lang: str = 'en', context_config=None, semantics='DEFAULT',
-              promptText=None, metadata: str = None, summarizer: str = "vectara-summary-ext-v1.3.0",
-              summary_result_count=5, re_rank=False):
+              promptText=None, metadata: str = None, summarizer: str = "vectara-summary-ext-v1.2.0",
+              summary_result_count=5, re_rank=False, custom_dimensions:List[dict]=None, _lambda=0.025,
+              temperature=None, debug: bool = None, chat=False, conversation_id:str=None,
+              query_context: str=""):
 
         # Convert singular int to List of corpus ids.
         if type(corpus_id) is list:
             corpus_ids = corpus_id
         else:
             corpus_ids = [corpus_id]
 
@@ -51,18 +53,22 @@
             corpus_key = {'customerId': self.customer_id,
                           'corpusId': id,
                           'semantics': semantics
                           }
             if metadata:
                 corpus_key['metadataFilter'] = metadata
 
+            if custom_dimensions:
+                corpus_key['dim'] = custom_dimensions
+
             corpus_keys.append(corpus_key)
 
         query_dict = {
             'query': query_text,
+            'queryContext': query_context,
             'numResults': page_size,
             'contextConfig': context_config,
             'corpusKey': corpus_keys
         }
 
         if re_rank:
             query_dict['rerankingConfig'] = {
@@ -75,38 +81,54 @@
         if summary:
             if response_lang:
                 self.logger.debug(f"Response Language set to [{response_lang}]")
             else:
                 raise TypeError("If you are going to change from the default language (en) you must set one.")
 
             # Old: vectara-summary-ext-v1.2.0
-            # New: vectara-summary-ext-v1.2.3
+            # New: vectara-summary-ext-v1.3.0
             query_dict['summary'] = [{"summarizerPromptName": summarizer,
                                       "responseLang": response_lang,
                                       "maxSummarizedResults": summary_result_count
                                       }]
             if promptText:
                 query_dict['summary'][0]['promptText'] = promptText
+
+            if temperature:
+                query_dict['summary'][0]['modelParams'] = {'temperature': temperature}
+
+            if debug:
+                query_dict['summary'][0]['debug'] = debug
+
+            if chat:
+                query_dict['summary'][0]['chat'] = {
+                    'store': True
+                }
+                if conversation_id:
+                    query_dict['summary'][0]['chat']['conversationId'] = conversation_id
+
         else:
             # Only put this in if we're not summarising.
             query_dict['start']: start
 
+
+
         batch_query_dict = {'query': [query_dict]}
 
         self.logger.debug(f"Query is:\n{json.dumps(batch_query_dict, indent=4)}\n")
 
         query = from_dict(BatchQueryRequest, batch_query_dict)
 
         # Omit nulls using our own dict factory.
         # Dataclasses feel like coding with the first XML serializers in Java in 2005 - very early.
         final_query_dict = asdict(query, dict_factory=_custom_asdict_factory)
 
         # Since we can't put in "lambda" to a dataclass field due to Python using it as a reserved word,
         # we inject it now.
-        final_query_dict['query'][0]['corpusKey'][0]['lexicalInterpolationConfig'] = {"lambda": 0.025}
+        final_query_dict['query'][0]['corpusKey'][0]['lexicalInterpolationConfig'] = {"lambda": _lambda}
 
         result = self.request_util.request("query", final_query_dict, BatchQueryResponse)
 
         summary_status = None
         if summary:
             if (result.responseSet[0].summary[0].status and result.responseSet[0].summary[0].status
                     and len(result.responseSet[0].summary[0].status and result.responseSet[0].summary[0].status) > 0):
```

### Comparing `vectara-skunk-client-0.4.9/vectara/client/status.py` & `vectara_skunk_client-0.5.0/vectara_client/status.py`

 * *Files 8% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     DISABLED_CUSTOMER = 1100
     INVALID_CUSTOMER_ID = 1101
     DISABLED_CORPUS = 1102
     INVALID_CORPUS_ID = 1103
     DISABLED_API_KEY = 1104
     EXPIRED_API_KEY = 1105
     INVALID_API_KEY = 1106
+    CMK_INACCESSIBLE = 1107
 
     # Serving Query - ------------------------------------------------------------
     QRY__DISABLED_CORPUS = 1500
     QRY__DOCUMENT_DB_FAILURE = 1505
     QRY__ENCODER_FAILURE = 1510
     QRY__INTERRUPTED = 1515
     QRY__INVALID_CORPUS = 1520
@@ -66,15 +67,25 @@
     QRY__INVALID_DIMENSION = 1565
     QRY__INVALID_CLIENTKEY = 1570
     QRY__DECRYPTION_FAILURE = 1575
     QRY__INVALID_RERANKER = 1580
     QRY__PARTIAL_RERANK = 1585
     QRY__RERANK_FAILURE = 1590
     QRY__TOO_MANY_RESULT_ROWS = 1595
-    QRY__SMRY__NO_QUERY_RESULTS = 1600 # TODO Validate this number!!
+
+    QRY__SMRY__INVALID_SUMMARIZER_PROMPT = 1660
+    QRY__SMRY__INVALID_SUMMARY_LANG = 1665
+    QRY__SMRY__UNSUPPORTED_SUMMARY_LANG = 1670
+    QRY__SMRY__PARTIAL_SUMMARY = 1675
+    QRY__SMRY__NO_QUERY_RESULTS = 1680
+    QRY__GEN__NO_QUERY_RESULTS = 1650
+    QRY__GEN__UNPARSEABLE_MODEL_PARAMS = 1651
+
+
+
 
     # Connection specs - ---------------------------------------------------------
     CX_SPECS__INVALID_JSON = 2000
     CX_SPECS__UNREGISTERED_TYPE = 2005
     CX_SPECS__MISSING_SPEC = 2010
     CX_SPECS__MISSING_TYPE = 2011
     CX_SPECS__UNPARSEABLE_SPEC = 2015
@@ -102,17 +113,22 @@
     ADM__SIGNUP_INVALID_ORG = 2517
     ADM__SIGNUP_INVALID_EMAIL = 2518
     ADM__SIGNUP_INVALID_PAYMENT = 2519
     ADM__SIGNUP_INVALID_PLAN = 2520
     ADM__SIGNUP_INVALID_PASSWORD = 2521
     ADM__SIGNUP_INVALID_ACCOUNT_ALIAS = 2530
     ADM__SIGNUP_INVALID_EMAIL_VALIDATION_CODE = 2531
+    ADM__SIGNUP_MISSING_COUNTRY_CODE = 2532
+    ADM__SIGNUP_ROOT_EMAIL_NOT_AVAILABLE = 2533
 
     ADM__CUST_MARK_DELETE_FAILED = 2522
     ADM__CUST_FAISS_DEALLOC_FAILED = 2523
+    ADM__CUST_ALREADY_ACTIVE = 2534
+    ADM__CUST_REACTIVATE_FAILED = 2535
+    ADM__CUST_ENABLEMENT_FAILED = 2536
 
     ADM__CORPUS_LIMIT_REACHED = 2524
 
     ADM__STRIPE_CARD_DECLINED = 2525
     ADM__STRIPE_PROCESSING_ERROR = 2526
 
     ADM__EMAIL_VALIDATION_REQUEST_NOT_FOUND = 2540
@@ -141,14 +157,22 @@
     REBUILD__NO_DATA = 4520
     REBUILD__EVALUATION = 4525
 
     # Indexing - -----------------------------------------------------------------
     IDX__TRANSIENT_PARTIAL_DELETION_FAILURE = 5000
     IDX__PERMANENT_PARTIAL_DELETION_FAILURE = 5001
 
+    # Calibration
+    CALB__INVALID_JSON = 5500
+    CALB__INVALID_SPEC = 5501
+    CALB__UNREGISTERED_TYPE = 5505
+    CALB__MISSING_SPEC = 5510
+    CALB__MISSING_TYPE = 5511
+    CALB__UNPARSABLE_SPEC = 5515
+
 
 @dataclass
 class Status:
     """
     Including these as optional because file upload response has this as an empty object on success
     """
     code: Optional[str | StatusCode]
```

### Comparing `vectara-skunk-client-0.4.9/vectara/client/util.py` & `vectara_skunk_client-0.5.0/vectara_client/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from abc import ABC
 from enum import Enum
-from vectara.client.authn import BaseAuthUtil
-from vectara.client.domain import UploadDocumentResponse, ResponseSet, Attribute
+from vectara_client.authn import BaseAuthUtil
+from vectara_client.domain import UploadDocumentResponse, ResponseSet, Attribute
 from typing import Type, TypeVar, List
 from dacite import from_dict
 from pathlib import Path
 from tqdm import tqdm
 from tqdm.contrib.logging import logging_redirect_tqdm
 from requests_toolbelt import MultipartEncoder, MultipartEncoderMonitor
 import logging
+import threading
 import json
 import requests
 import warnings
 
 T = TypeVar("T")
 
 def convertAttrListToDict(input:List[Attribute]):
@@ -56,28 +57,33 @@
         self.logger.debug(f"Headers: {json.dumps(headers)}")
 
         self.requests.append({'operation': operation, 'payload': payload})
 
         url = f"https://api.vectara.io/v1/{operation}"
         self.logger.info(f"URL for operation {operation} is: {url}")
         if self.logger.isEnabledFor(logging.DEBUG):
+
             self.logger.debug(f"Payload is: {json.dumps(payload, indent=4)}")
 
         payload_json = json.dumps(payload)
 
         response = requests.request(method, url, headers=headers, data=payload_json)
 
         if response.status_code == 200:
+            if self.logger.isEnabledFor(logging.DEBUG):
+                self.logger.debug(f"Response was:\n{json.dumps(json.loads(response.text), indent=4)}")
+
             if to_class:
                 return from_dict(to_class, json.loads(response.text))
             elif response.text:
                 return json.loads(response.text)
             else:
                 return
         else:
+            print(f"Received non 200 response: {response.text}")
             self.logger.error(f"Received non 200 response {response.status_code}, throwing exception")
             response.raise_for_status()
 
     def multipart_post(self, operation: str, path_str: str = None, input_contents: bytes = None,
                        input_file_name: str = None,
                        params=None, headers=None) -> UploadDocumentResponse:
 
@@ -97,15 +103,15 @@
         if path_str and input_file_name:
             raise TypeError("You must specify either the path or the file_name")
         elif path_str:
             path = Path(path_str)
             tracker_total_size = path.stat().st_size
             tracker_file_name = path.name
 
-            with warnings.catch_warnings(action="ignore"):
+            with warnings.catch_warnings():
                 """
                 Need to ignore tqdm std.py:580: DeprecationWarning: datetime.datetime.utcfromtimestamp()
                 
                 See more here: https://github.com/tqdm/tqdm/issues/1517                
                 """
                 with tqdm(
                         desc=tracker_file_name,
@@ -413,20 +419,22 @@
         return "".join(lines)
 
 
 class ChatPromptFactory(BasePromptFactory):
     SYSTEM_PROMPT_TEMPLATE = 'You are a {chat_persona} talking with a customer, respond to small talk in a nice way. You must not say you are an AI model. Provide a short answer from the search results, though you can go into more detail if requested from the user. Do not iterate over each question, just provide a short answer based on prior assistant answers in this chat. You may allow additional information you know in the results if nothing relevant is found. Respond in the language denoted by ISO 639 code \\"$vectaraLangCode\\".'
     USER_PROMPT_TEMPLATE = 'Generate a chat response which is part of a back-and-forth, that is no more than {max_word_count} words, for the query \\"$esc.java(${{vectaraQuery}})\\" preferably based on the interactions in this chat. Please ask for more information to help clarify if needed. If the response answers the question, please finish with a closing phrase that uses \\"does that answer your question\\" to confirm resolution.'
 
-    def __init__(self, chat_persona="Customer Support", name="Gary", max_word_count=300):
+    def __init__(self, chat_persona="Customer Support", name="Gary", max_word_count=300, prompt_metadata={}):
         super().__init__()
+        self.logger = logging.getLogger(self.__class__.__name__)
         self.chat_persona = chat_persona
         self.name = name
         self.messages = []
         self.max_word_count = max_word_count
+        self.prompt_metadata = prompt_metadata
 
     def add_user_message(self, user_message):
         self.messages.append({"role": "user", "content": user_message})
 
     def add_assistant_message(self, assistant_message):
         self.messages.append({"role": "assistant", "content": assistant_message})
 
@@ -444,20 +452,26 @@
         )
 
         lines = []
 
         # Append the system indicator.
         lines.append(f'[ {{"role": "system", "content": "{system_prompt}"}}, \n')
 
-        # Append the pre-requisite 'for-loop' for RAG.
-        lines.append('#foreach ($qResult in $vectaraQueryResults) \n')
-
         # Insert prior context user/assistant messages.
         for message in self.messages:
             lines.append(f'    {json.dumps(message)}, \n')
+        # Append the pre-requisite 'for-loop' for RAG.
+        lines.append('#foreach ($qResult in $vectaraQueryResults) \n')
+
+        metadata = ""
+        if (self.prompt_metadata):
+            bits = []
+            for key in self.prompt_metadata.keys():
+                value = self.prompt_metadata[key]
+                bits.append(f"{key}: ")
 
         # Insert the Retrieval results.
         lines.append('   #if ($foreach.first) \n')
         lines.append(
             '   {"role": "user", "content": "Search for \\"$esc.java(${vectaraQuery})\\", and give me the first search result."}, \n')
         lines.append('   {"role": "assistant", "content": "$esc.java(${qResult.getText()})" }, \n')
         lines.append('   #else \n')
@@ -466,11 +480,36 @@
         lines.append('   {"role": "assistant", "content": "$esc.java(${qResult.getText()})" }, \n')
         lines.append('   #end \n')
         lines.append(' #end \n')
 
         # Append the Final user phrasing.
         lines.append(f'{{"role": "user", "content": "{user_prompt}" }} ]')
 
-        return "".join(lines)
+        result = "".join(lines)
+        self.logger.info("Chat prompt is:\n" + result)
+        return result
+
+
+class CountDownLatch:
+    def __init__(self, count=1):
+        self.count = count
+        self.lock = threading.Condition()
+
+    def count_down(self):
+        self.lock.acquire()
+        self.count -= 1
+        if self.count <= 0:
+            self.lock.notify_all()
+        self.lock.release()
 
+    def sweat_it_out(self):
+        """
+        Because await is a keyword.
+
+        :return:
+        """
+        self.lock.acquire()
+        while self.count > 0:
+            self.lock.wait()
+        self.lock.release()
```

### Comparing `vectara-skunk-client-0.4.9/vectara_skunk_client.egg-info/PKG-INFO` & `vectara_skunk_client-0.5.0/vectara_skunk_client.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectara-skunk-client
-Version: 0.4.9
+Version: 0.5.0
 Summary: Vectara Skunk Client
 Home-page: https://github.com/davidglevy/vectara-skunk-client
 Author: David Levy
 Author-email: david.g.levy@gmail.com
 License: GNU AFFERO GENERAL PUBLIC LICENSE v3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

