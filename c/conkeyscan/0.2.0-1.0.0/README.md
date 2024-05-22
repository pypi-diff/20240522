# Comparing `tmp/conkeyscan-0.2.0.tar.gz` & `tmp/conkeyscan-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conkeyscan-0.2.0.tar", last modified: Tue Mar  5 15:25:59 2024, max compression
+gzip compressed data, was "conkeyscan-1.0.0.tar", last modified: Wed May 22 06:53:15 2024, max compression
```

## Comparing `conkeyscan-0.2.0.tar` & `conkeyscan-1.0.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:25:59.188820 conkeyscan-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-05 15:25:55.000000 conkeyscan-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-03-05 15:25:59.188820 conkeyscan-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-03-05 15:25:55.000000 conkeyscan-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 15:25:59.188820 conkeyscan-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-05 15:25:58.000000 conkeyscan-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:25:59.184820 conkeyscan-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:25:59.184820 conkeyscan-0.2.0/src/conkeyscan/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 15:25:55.000000 conkeyscan-0.2.0/src/conkeyscan/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:25:59.188820 conkeyscan-0.2.0/src/conkeyscan/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 15:25:55.000000 conkeyscan-0.2.0/src/conkeyscan/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-05 15:25:55.000000 conkeyscan-0.2.0/src/conkeyscan/config/dict.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8550 2024-03-05 15:25:55.000000 conkeyscan-0.2.0/src/conkeyscan/conkeyscan.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:25:59.188820 conkeyscan-0.2.0/src/conkeyscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-03-05 15:25:59.000000 conkeyscan-0.2.0/src/conkeyscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-03-05 15:25:59.000000 conkeyscan-0.2.0/src/conkeyscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 15:25:59.000000 conkeyscan-0.2.0/src/conkeyscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-05 15:25:59.000000 conkeyscan-0.2.0/src/conkeyscan.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-05 15:25:59.000000 conkeyscan-0.2.0/src/conkeyscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-05 15:25:59.000000 conkeyscan-0.2.0/src/conkeyscan.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:53:15.331151 conkeyscan-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-22 06:53:10.000000 conkeyscan-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-22 06:53:10.000000 conkeyscan-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-22 06:53:15.331151 conkeyscan-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-22 06:53:10.000000 conkeyscan-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 06:53:15.331151 conkeyscan-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-22 06:53:14.000000 conkeyscan-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:53:15.331151 conkeyscan-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:53:15.331151 conkeyscan-1.0.0/src/conkeyscan/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 06:53:10.000000 conkeyscan-1.0.0/src/conkeyscan/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:53:15.331151 conkeyscan-1.0.0/src/conkeyscan/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 06:53:10.000000 conkeyscan-1.0.0/src/conkeyscan/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-22 06:53:10.000000 conkeyscan-1.0.0/src/conkeyscan/config/dict.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     8550 2024-05-22 06:53:10.000000 conkeyscan-1.0.0/src/conkeyscan/conkeyscan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 06:53:15.331151 conkeyscan-1.0.0/src/conkeyscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2419 2024-05-22 06:53:15.000000 conkeyscan-1.0.0/src/conkeyscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-22 06:53:15.000000 conkeyscan-1.0.0/src/conkeyscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 06:53:15.000000 conkeyscan-1.0.0/src/conkeyscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-22 06:53:15.000000 conkeyscan-1.0.0/src/conkeyscan.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-22 06:53:15.000000 conkeyscan-1.0.0/src/conkeyscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 06:53:15.000000 conkeyscan-1.0.0/src/conkeyscan.egg-info/top_level.txt
```

### Comparing `conkeyscan-0.2.0/PKG-INFO` & `conkeyscan-1.0.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,55 @@
-Metadata-Version: 2.1
-Name: conkeyscan
-Version: 0.2.0
-Summary: A Pentesters Confluence Keyword Scanner
-Home-page: https://github.com/CompassSecurity/conkeyscan
-Author: Jan Friedli
-Description-Content-Type: text/markdown
+<p align="center">
+    <img width="150" src="https://github.com/CompassSecurity/conkeyscan/blob/main/logo.svg" alt="Conkeyscan logo">
+</p>
 
 # Conkeyscan
+[![PyPI version](https://badge.fury.io/py/conkeyscan.svg)](https://badge.fury.io/py/conkeyscan)
 
-Scan Confluence Wikis for keywords.
+> A Pentesters Confluence Keyword Scanner
 
-The approach is using the search functionality and CQL queries to search for keywords in Confluence.
+Using the Confluence API search functionality and CQL queries to search for keywords.
 
-# PyPI
+# Installation
 
-`pip install conkeyscan`
-
-# Run It
-
-1. Download the latest release [here](https://github.com/CompassSecurity/conkeyscan/releases).
-
-2. Create a dictionary with search terms per line or copy the default `dict.txt` from this repository.
-
-3. and then run it 
+1. Install from PyPI `pip install conkeyscan`
+2. Create a custom dictionary with search terms per line (recommended but optional).
+3. And then run it 
 ```bash
-./conkeyscan -url 'https://example.atlassian.net'  --username 'ex@amp.le' --password 'ATAT...' -p 'socks5://127.0.0.1:1337' -d ./dict.txt 
+conkeyscan -url 'https://example.atlassian.net'  --username 'ex@amp.le' --password 'ATAT...' -p 'socks5://127.0.0.1:1337' -d ./dict.txt 
 ```
+4. Ask for further help `conkeyscan -h`
 
 # Get Up And Running Manually
 
 1. Install dependencies `pip install -r requirements.txt`
 
-2. Update the `dict.txt` file, containing keywords you want to search for. One per line.
+2. Update the `src/conkeyscan/config/dict.txt` file, containing keywords you want to search for. One per line.
 
 3. run it `python3 -m conkeyscan.conkeyscan --url http://192.168.1.2:8090/ --username someUsr --password somePassOrAPIkey`
 
-4. Profit 🍾 check the generated logfile or stdout
-
-5. Further Help `python3 -m conkeyscan.conkeyscan -h`
-
-
 # Authentication
 
 > It is possible to use a password or an API key.
 
-To create an API key in the cloud go to: https://id.atlassian.com/manage-profile/security/api-tokens
+To create an API key in the cloud go to: https://id.atlassian.com/manage-profile/security/api-tokens.
+
 If testing against OnPrem instance you can create an API key in the user settings.
 
 # Dictionary
 
-The default `dict.txt` file was taken from from [Conf-Thief](https://raw.githubusercontent.com/antman1p/Conf-Thief/master/dictionaries/secrets-keywords.txt)
+The default `dict.txt` file was taken from from [Conf-Thief](https://raw.githubusercontent.com/antman1p/Conf-Thief/master/dictionaries/secrets-keywords.txt).
 
 # Features
 
 * Search for provided keywords
 * Handle rate limiting by itself, as long as the returned status code equals `HTTP 429`, or specify max requests per second in CLI
 * The user agent is randomized
 * Proxying is supported either via HTTP or socks. See cli help for examples
 * Custom CQL
 * SSL/TLS checks are disabled by default
 
 # Alternatives 
 
 * https://spark1.us/n0s1 actually great, supports Jira and others as well, has some drawbacks in on-prem engagements e.g disable TLS verification, missing Proxying, rate-limiting adaption?. Scans everything, nice for CI.
 * https://github.com/BluBracket/confluence-risk-scanner
-* https://github.com/antman1p/Conf-Thief
+* https://github.com/antman1p/Conf-Thief
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `conkeyscan-0.2.0/README.md` & `conkeyscan-1.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,65 @@
-# Conkeyscan
-
-Scan Confluence Wikis for keywords.
-
-The approach is using the search functionality and CQL queries to search for keywords in Confluence.
+Metadata-Version: 2.1
+Name: conkeyscan
+Version: 1.0.0
+Summary: A Pentesters Confluence Keyword Scanner
+Home-page: https://github.com/CompassSecurity/conkeyscan
+Author: Jan Friedli
+License: mit
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+    <img width="150" src="https://github.com/CompassSecurity/conkeyscan/blob/main/logo.svg" alt="Conkeyscan logo">
+</p>
 
-# PyPI
-
-`pip install conkeyscan`
+# Conkeyscan
+[![PyPI version](https://badge.fury.io/py/conkeyscan.svg)](https://badge.fury.io/py/conkeyscan)
 
-# Run It
+> A Pentesters Confluence Keyword Scanner
 
-1. Download the latest release [here](https://github.com/CompassSecurity/conkeyscan/releases).
+Using the Confluence API search functionality and CQL queries to search for keywords.
 
-2. Create a dictionary with search terms per line or copy the default `dict.txt` from this repository.
+# Installation
 
-3. and then run it 
+1. Install from PyPI `pip install conkeyscan`
+2. Create a custom dictionary with search terms per line (recommended but optional).
+3. And then run it 
 ```bash
-./conkeyscan -url 'https://example.atlassian.net'  --username 'ex@amp.le' --password 'ATAT...' -p 'socks5://127.0.0.1:1337' -d ./dict.txt 
+conkeyscan -url 'https://example.atlassian.net'  --username 'ex@amp.le' --password 'ATAT...' -p 'socks5://127.0.0.1:1337' -d ./dict.txt 
 ```
+4. Ask for further help `conkeyscan -h`
 
 # Get Up And Running Manually
 
 1. Install dependencies `pip install -r requirements.txt`
 
-2. Update the `dict.txt` file, containing keywords you want to search for. One per line.
+2. Update the `src/conkeyscan/config/dict.txt` file, containing keywords you want to search for. One per line.
 
 3. run it `python3 -m conkeyscan.conkeyscan --url http://192.168.1.2:8090/ --username someUsr --password somePassOrAPIkey`
 
-4. Profit 🍾 check the generated logfile or stdout
-
-5. Further Help `python3 -m conkeyscan.conkeyscan -h`
-
-
 # Authentication
 
 > It is possible to use a password or an API key.
 
-To create an API key in the cloud go to: https://id.atlassian.com/manage-profile/security/api-tokens
+To create an API key in the cloud go to: https://id.atlassian.com/manage-profile/security/api-tokens.
+
 If testing against OnPrem instance you can create an API key in the user settings.
 
 # Dictionary
 
-The default `dict.txt` file was taken from from [Conf-Thief](https://raw.githubusercontent.com/antman1p/Conf-Thief/master/dictionaries/secrets-keywords.txt)
+The default `dict.txt` file was taken from from [Conf-Thief](https://raw.githubusercontent.com/antman1p/Conf-Thief/master/dictionaries/secrets-keywords.txt).
 
 # Features
 
 * Search for provided keywords
 * Handle rate limiting by itself, as long as the returned status code equals `HTTP 429`, or specify max requests per second in CLI
 * The user agent is randomized
 * Proxying is supported either via HTTP or socks. See cli help for examples
 * Custom CQL
 * SSL/TLS checks are disabled by default
 
 # Alternatives 
 
 * https://spark1.us/n0s1 actually great, supports Jira and others as well, has some drawbacks in on-prem engagements e.g disable TLS verification, missing Proxying, rate-limiting adaption?. Scans everything, nice for CI.
 * https://github.com/BluBracket/confluence-risk-scanner
-* https://github.com/antman1p/Conf-Thief
+* https://github.com/antman1p/Conf-Thief
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `conkeyscan-0.2.0/setup.py` & `conkeyscan-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name="conkeyscan",
     author="Jan Friedli",
     url="https://github.com/CompassSecurity/conkeyscan",
     description="A Pentesters Confluence Keyword Scanner",
-    version="0.2.0",
+    version="1.0.0",
+    license="mit",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     py_modules=["conkeyscan"],
     install_requires=[
         "loguru",
         "atlassian-python-api>=3",
         "beautifulsoup4>=4",
```

### Comparing `conkeyscan-0.2.0/src/conkeyscan/config/dict.txt` & `conkeyscan-1.0.0/src/conkeyscan/config/dict.txt`

 * *Files identical despite different names*

### Comparing `conkeyscan-0.2.0/src/conkeyscan/conkeyscan.py` & `conkeyscan-1.0.0/src/conkeyscan/conkeyscan.py`

 * *Files identical despite different names*

### Comparing `conkeyscan-0.2.0/src/conkeyscan.egg-info/PKG-INFO` & `conkeyscan-1.0.0/src/conkeyscan.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,59 +1,57 @@
 Metadata-Version: 2.1
 Name: conkeyscan
-Version: 0.2.0
+Version: 1.0.0
 Summary: A Pentesters Confluence Keyword Scanner
 Home-page: https://github.com/CompassSecurity/conkeyscan
 Author: Jan Friedli
+License: mit
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
-# Conkeyscan
-
-Scan Confluence Wikis for keywords.
-
-The approach is using the search functionality and CQL queries to search for keywords in Confluence.
+<p align="center">
+    <img width="150" src="https://github.com/CompassSecurity/conkeyscan/blob/main/logo.svg" alt="Conkeyscan logo">
+</p>
 
-# PyPI
-
-`pip install conkeyscan`
+# Conkeyscan
+[![PyPI version](https://badge.fury.io/py/conkeyscan.svg)](https://badge.fury.io/py/conkeyscan)
 
-# Run It
+> A Pentesters Confluence Keyword Scanner
 
-1. Download the latest release [here](https://github.com/CompassSecurity/conkeyscan/releases).
+Using the Confluence API search functionality and CQL queries to search for keywords.
 
-2. Create a dictionary with search terms per line or copy the default `dict.txt` from this repository.
+# Installation
 
-3. and then run it 
+1. Install from PyPI `pip install conkeyscan`
+2. Create a custom dictionary with search terms per line (recommended but optional).
+3. And then run it 
 ```bash
-./conkeyscan -url 'https://example.atlassian.net'  --username 'ex@amp.le' --password 'ATAT...' -p 'socks5://127.0.0.1:1337' -d ./dict.txt 
+conkeyscan -url 'https://example.atlassian.net'  --username 'ex@amp.le' --password 'ATAT...' -p 'socks5://127.0.0.1:1337' -d ./dict.txt 
 ```
+4. Ask for further help `conkeyscan -h`
 
 # Get Up And Running Manually
 
 1. Install dependencies `pip install -r requirements.txt`
 
-2. Update the `dict.txt` file, containing keywords you want to search for. One per line.
+2. Update the `src/conkeyscan/config/dict.txt` file, containing keywords you want to search for. One per line.
 
 3. run it `python3 -m conkeyscan.conkeyscan --url http://192.168.1.2:8090/ --username someUsr --password somePassOrAPIkey`
 
-4. Profit 🍾 check the generated logfile or stdout
-
-5. Further Help `python3 -m conkeyscan.conkeyscan -h`
-
-
 # Authentication
 
 > It is possible to use a password or an API key.
 
-To create an API key in the cloud go to: https://id.atlassian.com/manage-profile/security/api-tokens
+To create an API key in the cloud go to: https://id.atlassian.com/manage-profile/security/api-tokens.
+
 If testing against OnPrem instance you can create an API key in the user settings.
 
 # Dictionary
 
-The default `dict.txt` file was taken from from [Conf-Thief](https://raw.githubusercontent.com/antman1p/Conf-Thief/master/dictionaries/secrets-keywords.txt)
+The default `dict.txt` file was taken from from [Conf-Thief](https://raw.githubusercontent.com/antman1p/Conf-Thief/master/dictionaries/secrets-keywords.txt).
 
 # Features
 
 * Search for provided keywords
 * Handle rate limiting by itself, as long as the returned status code equals `HTTP 429`, or specify max requests per second in CLI
 * The user agent is randomized
 * Proxying is supported either via HTTP or socks. See cli help for examples
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

