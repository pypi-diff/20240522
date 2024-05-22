# Comparing `tmp/servicenow_api-0.8.0-py2.py3-none-any.whl.zip` & `tmp/servicenow_api-0.9.0-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 8615 bytes, number of entries: 10
+Zip file size: 8638 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      294 b- defN 23-Feb-08 18:14 servicenow_api/__init__.py
 -rw-r--r--  2.0 unx      525 b- defN 23-Feb-08 18:14 servicenow_api/decorators.py
 -rw-r--r--  2.0 unx      463 b- defN 23-Feb-08 18:14 servicenow_api/exceptions.py
--rw-r--r--  2.0 unx    55258 b- defN 23-Feb-20 19:26 servicenow_api/servicenow_api.py
--rw-r--r--  2.0 unx      116 b- defN 23-Feb-20 19:26 servicenow_api/version.py
--rw-r--r--  2.0 unx     1211 b- defN 23-Feb-20 19:26 servicenow_api-0.8.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1784 b- defN 23-Feb-20 19:26 servicenow_api-0.8.0.dist-info/METADATA
--rw-r--r--  2.0 unx      110 b- defN 23-Feb-20 19:26 servicenow_api-0.8.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-Feb-20 19:26 servicenow_api-0.8.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      843 b- defN 23-Feb-20 19:26 servicenow_api-0.8.0.dist-info/RECORD
-10 files, 60619 bytes uncompressed, 7167 bytes compressed:  88.2%
+-rw-r--r--  2.0 unx    55392 b- defN 23-Feb-20 19:32 servicenow_api/servicenow_api.py
+-rw-r--r--  2.0 unx      116 b- defN 23-Feb-20 19:32 servicenow_api/version.py
+-rw-r--r--  2.0 unx     1211 b- defN 23-Feb-20 19:32 servicenow_api-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1784 b- defN 23-Feb-20 19:32 servicenow_api-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx      110 b- defN 23-Feb-20 19:32 servicenow_api-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-Feb-20 19:32 servicenow_api-0.9.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      843 b- defN 23-Feb-20 19:32 servicenow_api-0.9.0.dist-info/RECORD
+10 files, 60753 bytes uncompressed, 7190 bytes compressed:  88.2%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: servicenow_api/servicenow_api.py
 Comment: 
 
 Filename: servicenow_api/version.py
 Comment: 
 
-Filename: servicenow_api-0.8.0.dist-info/LICENSE
+Filename: servicenow_api-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: servicenow_api-0.8.0.dist-info/METADATA
+Filename: servicenow_api-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: servicenow_api-0.8.0.dist-info/WHEEL
+Filename: servicenow_api-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: servicenow_api-0.8.0.dist-info/top_level.txt
+Filename: servicenow_api-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: servicenow_api-0.8.0.dist-info/RECORD
+Filename: servicenow_api-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## servicenow_api/servicenow_api.py

```diff
@@ -618,15 +618,18 @@
             else:
                 offset = f'&sysparm_offset={page}'
             if responses:
                 response = self._session.get(f'{self.url}/sn_chg_rest/change/standard/template{parameters}{offset}',
                                              headers=self.headers, verify=self.verify, proxies=self.proxies)
                 try:
                     verified_response = response.json()
-                    response_length = len(verified_response['result'])
+                    if 'result' in verified_response:
+                        response_length = len(verified_response['result'])
+                    else: 
+                        return verified_response
                     if response_length > 1 and page < max_pages \
                             or response_length > 1 and max_pages == 0:
                         responses['result'] = responses['result'] + verified_response['result']
                 except ValueError or AttributeError:
                     return verified_response
             else:
                 responses = self._session.get(f'{self.url}/sn_chg_rest/change/standard/template{parameters}{offset}',
```

## servicenow_api/version.py

```diff
@@ -1,6 +1,6 @@
 #!/usr/bin/env python
 # coding: utf-8
 
-__version__ = '0.8.0'
+__version__ = '0.9.0'
 __author__ = 'Audel Rouhi'
 __credits__ = 'Audel Rouhi'
```

## Comparing `servicenow_api-0.8.0.dist-info/LICENSE` & `servicenow_api-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `servicenow_api-0.8.0.dist-info/METADATA` & `servicenow_api-0.9.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: servicenow-api
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python ServiceNow API Wrapper
 Home-page: https://github.com/Knuckles-Team/servicenow-api
 Author: Audel Rouhi
 Author-email: knucklessg1@gmail.com
 License: Unlicense
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests (>=2.28.1)
 Requires-Dist: urllib3 (>=1.26.13)
 
 # ServiceNow API
-*Version: 0.8.0*
+*Version: 0.9.0*
 
 ServiceNow API Python Wrapper
 
 This repository is actively maintained and will continue adding more API calls
 
 ### API Calls:
 - Table
```

### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: servicenow-api Version: 0.8.0 Summary: Python
+Metadata-Version: 2.1 Name: servicenow-api Version: 0.9.0 Summary: Python
 ServiceNow API Wrapper Home-page: https://github.com/Knuckles-Team/servicenow-
 api Author: Audel Rouhi Author-email: knucklessg1@gmail.com License: Unlicense
 Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: Public Domain Classifier: Environment :: Console
 Classifier: Operating System :: POSIX :: Linux Classifier: Programming Language
 :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
 Requires-Dist: requests (>=2.28.1) Requires-Dist: urllib3 (>=1.26.13) #
-ServiceNow API *Version: 0.8.0* ServiceNow API Python Wrapper This repository
+ServiceNow API *Version: 0.9.0* ServiceNow API Python Wrapper This repository
 is actively maintained and will continue adding more API calls ### API Calls: -
 Table - CI/CD - Import Sets Coming Soon: - Incident - CMDB - Application
 Service ### Usage: ```python #!/usr/bin/python # coding: utf-8 import
 servicenow_api username = "" password = "" servicenow_api_url = "" client =
 servicenow_api.Api(url=servicenow_api_url, username=username,
 password=password) table = client.get_table(table="
```

