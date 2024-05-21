# Comparing `tmp/jzpypi-50.37.48.tar.gz` & `tmp/jzpypi-50.37.49.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jzpypi-50.37.48.tar", last modified: Tue May 21 23:35:01 2024, max compression
+gzip compressed data, was "jzpypi-50.37.49.tar", last modified: Tue May 21 23:40:34 2024, max compression
```

## Comparing `jzpypi-50.37.48.tar` & `jzpypi-50.37.49.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 23:35:01.483336 jzpypi-50.37.48/
--rw-rw-rw-   0        0        0      163 2024-05-21 23:35:01.479613 jzpypi-50.37.48/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-21 23:35:01.429545 jzpypi-50.37.48/jzpypi/
--rw-rw-rw-   0        0        0        0 2024-05-21 23:31:47.000000 jzpypi-50.37.48/jzpypi/__init__.py
--rw-rw-rw-   0        0        0     2353 2024-05-21 23:31:55.000000 jzpypi-50.37.48/jzpypi/upload.py
-drwxrwxrwx   0        0        0        0 2024-05-21 23:35:01.476962 jzpypi-50.37.48/jzpypi.egg-info/
--rw-rw-rw-   0        0        0      163 2024-05-21 23:35:01.000000 jzpypi-50.37.48/jzpypi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      226 2024-05-21 23:35:01.000000 jzpypi-50.37.48/jzpypi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 23:35:01.000000 jzpypi-50.37.48/jzpypi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-05-21 23:35:01.000000 jzpypi-50.37.48/jzpypi.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       43 2024-05-21 23:35:01.000000 jzpypi-50.37.48/jzpypi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-05-21 23:35:01.000000 jzpypi-50.37.48/jzpypi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 23:35:01.483336 jzpypi-50.37.48/setup.cfg
--rw-rw-rw-   0        0        0      402 2024-05-21 23:32:55.000000 jzpypi-50.37.48/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:40:34.072724 jzpypi-50.37.49/
+-rw-rw-rw-   0        0        0      163 2024-05-21 23:40:34.070215 jzpypi-50.37.49/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-21 23:40:34.017047 jzpypi-50.37.49/jzpypi/
+-rw-rw-rw-   0        0        0        0 2024-05-21 23:31:47.000000 jzpypi-50.37.49/jzpypi/__init__.py
+-rw-rw-rw-   0        0        0     3083 2024-05-21 23:40:15.000000 jzpypi-50.37.49/jzpypi/upload.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:40:34.066719 jzpypi-50.37.49/jzpypi.egg-info/
+-rw-rw-rw-   0        0        0      163 2024-05-21 23:40:33.000000 jzpypi-50.37.49/jzpypi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      226 2024-05-21 23:40:33.000000 jzpypi-50.37.49/jzpypi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 23:40:33.000000 jzpypi-50.37.49/jzpypi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2024-05-21 23:40:33.000000 jzpypi-50.37.49/jzpypi.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       43 2024-05-21 23:40:33.000000 jzpypi-50.37.49/jzpypi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 23:40:33.000000 jzpypi-50.37.49/jzpypi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 23:40:34.072724 jzpypi-50.37.49/setup.cfg
+-rw-rw-rw-   0        0        0      402 2024-05-21 23:40:23.000000 jzpypi-50.37.49/setup.py
```

### Comparing `jzpypi-50.37.48/jzpypi/upload.py` & `jzpypi-50.37.49/jzpypi/upload.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,40 @@
 import os
 import requests
 from requests.auth import HTTPBasicAuth
 from tqdm import tqdm
 from requests_toolbelt.multipart.encoder import MultipartEncoder, MultipartEncoderMonitor
 
-def upload_package(username, password, skip_existing, repository_url, dist_files):
+def check_existing_files(username, password, repository_url):
+    # Get a list of existing files on PyPI
+    response = requests.get(repository_url, auth=HTTPBasicAuth(username, password))
+    if response.status_code != 200:
+        print(f"Failed to fetch existing files from PyPI. Status code: {response.status_code}")
+        return []
+
+    # Extract the filenames from the response
+    lines = response.text.split('\n')
+    filenames = [line.split('<a href="')[1].split('">')[0] for line in lines if 'class="filename"' in line]
+    return filenames
+
+def upload_package(username, password, repository_url, dist_folder):
+    # Get a list of existing files on PyPI
+    existing_files = check_existing_files(username, password, repository_url)
+
+    # Get a list of files in the specified folder
+    dist_files = [os.path.join(dist_folder, filename) for filename in os.listdir(dist_folder)]
+
     for filepath in dist_files:
         filename = os.path.basename(filepath)
 
+        # Check if the file has already been uploaded
+        if filename in existing_files:
+            print(f"File {filename} already exists on PyPI. Skipping.")
+            continue
+
         # Check if the file exists before attempting to upload
         if not os.path.exists(filepath):
             print(f"File not found: {filepath}")
             continue
 
         with open(filepath, 'rb') as f:
             file_size = os.path.getsize(filepath)
@@ -30,25 +53,22 @@
                     auth=HTTPBasicAuth(username, password),
                     data=monitor,
                     headers={'Content-Type': monitor.content_type}
                 )
 
                 if response.status_code == 200:
                     print(f"Successfully uploaded {filename}")
-                elif response.status_code == 409 and skip_existing:
-                    print(f"File {filename} already exists. Skipping due to --skip-existing.")
                 else:
                     print(f"Failed to upload {filename}")
                     print(f"Status code: {response.status_code}")
                     print(f"Response: {response.text}")
 
 def main():
     username = '__token__'
     password = input("Enter your PyPI API token: ")
-    dist_files = input("Enter the paths of distribution files to upload (separated by spaces): ").split()
-    skip_existing = True  # You can change this if you want to skip existing files or not
+    dist_folder = input("Enter the path to the folder containing distribution files: ")
     repository_url = 'https://upload.pypi.org/legacy/'
 
-    upload_package(username, password, skip_existing, repository_url, dist_files)
+    upload_package(username, password, repository_url, dist_folder)
 
 if __name__ == "__main__":
     main()
```

