# Comparing `tmp/direnumerate-3.3rc1.tar.gz` & `tmp/direnumerate-4.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "direnumerate-3.3rc1.tar", last modified: Mon May 13 14:33:40 2024, max compression
+gzip compressed data, was "direnumerate-4.0a1.tar", last modified: Wed May 22 03:09:39 2024, max compression
```

## Comparing `direnumerate-3.3rc1.tar` & `direnumerate-4.0a1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-13 14:33:40.543056 direnumerate-3.3rc1/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    18092 2024-05-13 13:43:54.000000 direnumerate-3.3rc1/LICENSE
--rw-r--r--   0 estoque   (1000) estoque   (1000)     3708 2024-05-13 14:33:40.543056 direnumerate-3.3rc1/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2282 2024-05-13 13:44:29.000000 direnumerate-3.3rc1/README.md
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-13 14:33:40.539056 direnumerate-3.3rc1/direnumerate/
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      553 2024-05-13 13:43:54.000000 direnumerate-3.3rc1/direnumerate/__init__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    16991 2024-05-13 14:27:59.000000 direnumerate-3.3rc1/direnumerate/__main__.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      125 2024-05-13 13:43:54.000000 direnumerate-3.3rc1/direnumerate/banner.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     3401 2024-05-13 14:31:54.000000 direnumerate-3.3rc1/direnumerate/cli.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      394 2024-05-13 13:43:54.000000 direnumerate-3.3rc1/direnumerate/colors.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)    23461 2024-05-13 13:43:54.000000 direnumerate-3.3rc1/direnumerate/createlist.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      229 2024-05-13 13:43:54.000000 direnumerate-3.3rc1/direnumerate/exceptions.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      170 2024-05-13 13:43:54.000000 direnumerate-3.3rc1/direnumerate/getinfo.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      981 2024-05-13 13:43:54.000000 direnumerate-3.3rc1/direnumerate/help.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     2966 2024-05-13 13:43:54.000000 direnumerate-3.3rc1/direnumerate/ipcalculator.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       78 2024-05-13 14:25:50.000000 direnumerate-3.3rc1/direnumerate/list_urls_accounts.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       75 2024-05-13 13:45:37.000000 direnumerate-3.3rc1/direnumerate/version.py
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      334 2024-05-13 14:28:03.000000 direnumerate-3.3rc1/direnumerate/warning.py
-drwxrwxr-x   0 estoque   (1000) estoque   (1000)        0 2024-05-13 14:33:40.543056 direnumerate-3.3rc1/direnumerate.egg-info/
--rw-r--r--   0 estoque   (1000) estoque   (1000)     3708 2024-05-13 14:33:40.000000 direnumerate-3.3rc1/direnumerate.egg-info/PKG-INFO
--rw-rw-r--   0 estoque   (1000) estoque   (1000)      577 2024-05-13 14:33:40.000000 direnumerate-3.3rc1/direnumerate.egg-info/SOURCES.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        1 2024-05-13 14:33:40.000000 direnumerate-3.3rc1/direnumerate.egg-info/dependency_links.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       55 2024-05-13 14:33:40.000000 direnumerate-3.3rc1/direnumerate.egg-info/entry_points.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)        9 2024-05-13 14:33:40.000000 direnumerate-3.3rc1/direnumerate.egg-info/requires.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       13 2024-05-13 14:33:40.000000 direnumerate-3.3rc1/direnumerate.egg-info/top_level.txt
--rw-rw-r--   0 estoque   (1000) estoque   (1000)     1569 2024-05-13 14:32:04.000000 direnumerate-3.3rc1/pyproject.toml
--rw-rw-r--   0 estoque   (1000) estoque   (1000)       38 2024-05-13 14:33:40.543056 direnumerate-3.3rc1/setup.cfg
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-22 03:09:39.405815 direnumerate-4.0a1/
+-rw-rw-r--   0 juan      (1000) juan      (1000)    18092 2024-05-22 01:51:31.000000 direnumerate-4.0a1/LICENSE
+-rw-r--r--   0 juan      (1000) juan      (1000)     3707 2024-05-22 03:09:39.401815 direnumerate-4.0a1/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2282 2024-05-22 01:52:16.000000 direnumerate-4.0a1/README.md
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-22 03:09:39.393814 direnumerate-4.0a1/direnumerate/
+-rw-rw-r--   0 juan      (1000) juan      (1000)      553 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/__init__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    16553 2024-05-22 03:07:23.000000 direnumerate-4.0a1/direnumerate/__main__.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      125 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/banner.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     3401 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/cli.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      394 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/colors.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)    23461 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/createlist.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      229 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/exceptions.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      170 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/getinfo.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      981 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/help.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)     2966 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/ipcalculator.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)       78 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/list_urls_accounts.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)       73 2024-05-22 03:08:07.000000 direnumerate-4.0a1/direnumerate/version.py
+-rw-rw-r--   0 juan      (1000) juan      (1000)      334 2024-05-22 01:51:31.000000 direnumerate-4.0a1/direnumerate/warning.py
+drwxrwxr-x   0 juan      (1000) juan      (1000)        0 2024-05-22 03:09:39.401815 direnumerate-4.0a1/direnumerate.egg-info/
+-rw-r--r--   0 juan      (1000) juan      (1000)     3707 2024-05-22 03:09:39.000000 direnumerate-4.0a1/direnumerate.egg-info/PKG-INFO
+-rw-rw-r--   0 juan      (1000) juan      (1000)      577 2024-05-22 03:09:39.000000 direnumerate-4.0a1/direnumerate.egg-info/SOURCES.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)        1 2024-05-22 03:09:39.000000 direnumerate-4.0a1/direnumerate.egg-info/dependency_links.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       55 2024-05-22 03:09:39.000000 direnumerate-4.0a1/direnumerate.egg-info/entry_points.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)        9 2024-05-22 03:09:39.000000 direnumerate-4.0a1/direnumerate.egg-info/requires.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)       13 2024-05-22 03:09:39.000000 direnumerate-4.0a1/direnumerate.egg-info/top_level.txt
+-rw-rw-r--   0 juan      (1000) juan      (1000)     1567 2024-05-22 03:08:00.000000 direnumerate-4.0a1/pyproject.toml
+-rw-rw-r--   0 juan      (1000) juan      (1000)       38 2024-05-22 03:09:39.405815 direnumerate-4.0a1/setup.cfg
```

### Comparing `direnumerate-3.3rc1/LICENSE` & `direnumerate-4.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `direnumerate-3.3rc1/PKG-INFO` & `direnumerate-4.0a1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 3.3rc1
+Version: 4.0a1
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 3.3rc1 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 4.0a1 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```

### Comparing `direnumerate-3.3rc1/README.md` & `direnumerate-4.0a1/README.md`

 * *Files identical despite different names*

### Comparing `direnumerate-3.3rc1/direnumerate/__init__.py` & `direnumerate-4.0a1/direnumerate/__init__.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.3rc1/direnumerate/__main__.py` & `direnumerate-4.0a1/direnumerate/__main__.py`

 * *Files 16% similar despite different names*

```diff
@@ -88,85 +88,72 @@
         """
         self.wordlist_file = wordlist_file
         
 
         if verbose:
             try:
                 with open(self.wordlist_file, "r") as self.wordlist_file:
+                    results_list = []
                     for line in self.wordlist_file:
                         path = line.strip()
                         full_url = self.url + "/" + path
                         response = requests.get(full_url)
                         
                         if response.status_code == 200:
                             results = f"{Color.GREEN}[Found]:{Color.RESET} {full_url}"
-                            print(results)
-                            
+                            results_list.append(f'[Found] {full_url}')
                         elif response.status_code == 204:
                             results = f"{Color.BLUE}[No Content]:{Color.RESET} {full_url}"
-                            print(results)
-                            
+                            results_list.append(f'[No Content] {full_url}')
                         elif response.status_code == 400:
                             results = f"{Color.YELLOW}[Bad Request]:{Color.RESET} {full_url}"
-                            print(results)
-                            
+                            results_list.append(f'[Bad Request] {full_url}')
                         elif response.status_code == 401:
                             results = f"{Color.RED}[Unauthorized]:{Color.RESET} {full_url}"
-                            print(results)
-                            
+                            results_list.append(f'[Unauthorized] {full_url}')
                         elif response.status_code == 403:
                             results = f"{Color.RED}[Forbidden]:{Color.RESET} {full_url}"
-                            print(results)
-                            
+                            results_list.append(f'[Forbidden] {full_url}')
                         elif response.status_code == 404:
                             results =f"{Color.YELLOW}[Not Found]:{Color.RESET} {full_url}"
-                            print(results)
-                            
+                            results_list.append(f'[Not Found] {full_url}')
                         elif response.status_code == 500:
                             results = f"{Color.BLUE}[Internal Server Error]:{Color.RESET} {full_url}"
-                            print(results)
-                            
+                            results_list.append(f'[Internal Server Error] {full_url}')
+
+                        
+                        
 
             except FileNotFoundError:
                 print(Color.RED + "Word list file not found." + Color.RESET)
                 
             except TypeError:
                 print(Color.GREEN + "-------------------- Scan Finished --------------------" + Color.RESET)
                 
             except KeyboardInterrupt:
                 print(Color.GREEN + "-------------- Attempt interrupted by user ------------" + Color.RESET)
 
             except requests.exceptions.ConnectionError as rec:
                 print(rec)
                 print(Color.RED + "[Error] " + Color.RESET)
 
-        else:
-            try:
-                with open(self.wordlist_file, "r") as self.wordlist_file:
-                        for line in self.wordlist_file:
-                            path = line.strip()
-                            full_url = self.url + "/" + path
-                            response = requests.get(full_url)
+        
+        with open(self.wordlist_file, "r") as self.wordlist_file:
+                for line in self.wordlist_file:
+                    results_list = []
+                    path = line.strip()
+                    full_url = self.url + "/" + path
+                    response = requests.get(full_url)
+                            
+                    if response.status_code == 200:
+                        results = f"{Color.GREEN}[Found]:{Color.RESET} {full_url}"
+                        results_list.append('[Found]', full_url)
                             
-                            if response.status_code == 200:
-                                results = f"{Color.GREEN}[Found]:{Color.RESET} {full_url}"
-                                print(results)
-            
-            except FileNotFoundError:
-                print(Color.RED + "Word list file not found." + Color.RESET)
-                
-            except TypeError:
-                print(Color.GREEN + "-------------------- Scan Finished --------------------" + Color.RESET)
-                
-            except KeyboardInterrupt:
-                print(Color.GREEN + "-------------- Attempt interrupted by user ------------" + Color.RESET)
+        return results_list
 
-            except requests.exceptions.ConnectionError as rec:
-                print(rec)
-                print(Color.RED + "[Error]" + Color.RESET)
 
 class PortScan:
     """
     A class for port scanning.
 
     Attributes:
         host (str): The host to scan for open ports.
```

### Comparing `direnumerate-3.3rc1/direnumerate/cli.py` & `direnumerate-4.0a1/direnumerate/cli.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.3rc1/direnumerate/createlist.py` & `direnumerate-4.0a1/direnumerate/createlist.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.3rc1/direnumerate/help.py` & `direnumerate-4.0a1/direnumerate/help.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.3rc1/direnumerate/ipcalculator.py` & `direnumerate-4.0a1/direnumerate/ipcalculator.py`

 * *Files identical despite different names*

### Comparing `direnumerate-3.3rc1/direnumerate.egg-info/PKG-INFO` & `direnumerate-4.0a1/direnumerate.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: direnumerate
-Version: 3.3rc1
+Version: 4.0a1
 Summary: Python 3 library for directory enumeration tool in web applications.
 Author-email: Juan Bindez <juanbindez780@gmail.com>
 License: GPLv2 license
 Project-URL: Homepage, https://github.com/juanbindez/direnumerate
 Project-URL: Bug Reports, https://github.com/juanbindez/direnumerate/issues
 Project-URL: Read the Docs, http://direnumerate.readthedocs.io/
 Keywords: web,enumerate,directory,tools,cli,scan
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: direnumerate Version: 3.3rc1 Summary: Python 3
+Metadata-Version: 2.1 Name: direnumerate Version: 4.0a1 Summary: Python 3
 library for directory enumeration tool in web applications. Author-email: Juan
 Bindez
 gmail.com> License: GPLv2 license Project-URL: Homepage, https://github.com/
 juanbindez/direnumerate Project-URL: Bug Reports, https://github.com/
 juanbindez/direnumerate/issues Project-URL: Read the Docs, http://
 direnumerate.readthedocs.io/ Keywords: web,enumerate,directory,tools,cli,scan
 Classifier: Development Status :: 5 - Production/Stable Classifier: Environment
```

### Comparing `direnumerate-3.3rc1/direnumerate.egg-info/SOURCES.txt` & `direnumerate-4.0a1/direnumerate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `direnumerate-3.3rc1/pyproject.toml` & `direnumerate-4.0a1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.4.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "direnumerate"
-version = "3.3-rc1"
+version = "4.0a1"
 authors = [
   { name="Juan Bindez", email="juanbindez780@gmail.com" },
 ]
 description = "Python 3 library for directory enumeration tool in web applications."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "GPLv2 license"}
```

