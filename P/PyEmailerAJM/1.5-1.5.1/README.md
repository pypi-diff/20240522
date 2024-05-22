# Comparing `tmp/PyEmailerAJM-1.5.tar.gz` & `tmp/PyEmailerAJM-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyEmailerAJM-1.5.tar", last modified: Wed May 22 13:55:57 2024, max compression
+gzip compressed data, was "PyEmailerAJM-1.5.1.tar", last modified: Wed May 22 17:12:10 2024, max compression
```

## Comparing `PyEmailerAJM-1.5.tar` & `PyEmailerAJM-1.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 13:55:57.535041 PyEmailerAJM-1.5/
--rw-rw-rw-   0        0        0     1084 2023-09-12 19:19:18.000000 PyEmailerAJM-1.5/LICENSE.txt
--rw-rw-rw-   0        0        0      513 2024-05-22 13:55:57.535041 PyEmailerAJM-1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-22 13:55:57.511080 PyEmailerAJM-1.5/PyEmailerAJM/
--rw-rw-rw-   0        0        0    13448 2024-05-22 13:46:34.000000 PyEmailerAJM-1.5/PyEmailerAJM/PyEmailerAJM.py
--rw-rw-rw-   0        0        0      109 2023-09-13 15:44:18.000000 PyEmailerAJM-1.5/PyEmailerAJM/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 13:55:57.532023 PyEmailerAJM-1.5/PyEmailerAJM.egg-info/
--rw-rw-rw-   0        0        0      513 2024-05-22 13:55:57.000000 PyEmailerAJM-1.5/PyEmailerAJM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-05-22 13:55:57.000000 PyEmailerAJM-1.5/PyEmailerAJM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 13:55:57.000000 PyEmailerAJM-1.5/PyEmailerAJM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-22 13:55:57.000000 PyEmailerAJM-1.5/PyEmailerAJM.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-22 13:55:57.000000 PyEmailerAJM-1.5/PyEmailerAJM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      545 2024-05-16 12:24:41.000000 PyEmailerAJM-1.5/README.md
--rw-rw-rw-   0        0        0       86 2024-05-22 13:55:57.539021 PyEmailerAJM-1.5/setup.cfg
--rw-rw-rw-   0        0        0      600 2024-05-22 13:53:55.000000 PyEmailerAJM-1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:12:10.573605 PyEmailerAJM-1.5.1/
+-rw-rw-rw-   0        0        0     1084 2023-09-12 19:19:18.000000 PyEmailerAJM-1.5.1/LICENSE.txt
+-rw-rw-rw-   0        0        0      517 2024-05-22 17:12:10.574661 PyEmailerAJM-1.5.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 17:12:10.550402 PyEmailerAJM-1.5.1/PyEmailerAJM/
+-rw-rw-rw-   0        0        0    14577 2024-05-22 16:34:10.000000 PyEmailerAJM-1.5.1/PyEmailerAJM/PyEmailerAJM.py
+-rw-rw-rw-   0        0        0      109 2023-09-13 15:44:18.000000 PyEmailerAJM-1.5.1/PyEmailerAJM/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:12:10.570540 PyEmailerAJM-1.5.1/PyEmailerAJM.egg-info/
+-rw-rw-rw-   0        0        0      517 2024-05-22 17:12:10.000000 PyEmailerAJM-1.5.1/PyEmailerAJM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-05-22 17:12:10.000000 PyEmailerAJM-1.5.1/PyEmailerAJM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 17:12:10.000000 PyEmailerAJM-1.5.1/PyEmailerAJM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-22 17:12:10.000000 PyEmailerAJM-1.5.1/PyEmailerAJM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-22 17:12:10.000000 PyEmailerAJM-1.5.1/PyEmailerAJM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      545 2024-05-16 12:24:41.000000 PyEmailerAJM-1.5.1/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-22 17:12:10.577431 PyEmailerAJM-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      604 2024-05-22 17:00:17.000000 PyEmailerAJM-1.5.1/setup.py
```

### Comparing `PyEmailerAJM-1.5/LICENSE.txt` & `PyEmailerAJM-1.5.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyEmailerAJM-1.5/PKG-INFO` & `PyEmailerAJM-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: PyEmailerAJM
-Version: 1.5
+Version: 1.5.1
 Summary: Allows for automating sending Email with the Outlook Desktop client. Future releases will add more client support
 Home-page: https://github.com/amcsparron2793-Water/PyEmailer
 Author: Amcsparron
 Author-email: amcsparron@albanyny.gov
 License: MIT License
-Download-URL: https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.5.tar.gz
+Download-URL: https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.5.1.tar.gz
 Keywords: Outlook,Email,Automation
 Platform: UNKNOWN
 License-File: LICENSE.txt
 
 UNKNOWN
```

### Comparing `PyEmailerAJM-1.5/PyEmailerAJM/PyEmailerAJM.py` & `PyEmailerAJM-1.5.1/PyEmailerAJM/PyEmailerAJM.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # imports
 
 # install win32 with pip install pywin32
 import win32com.client as win32
 # This is installed as part of pywin32
 from pythoncom import com_error
 from logging import Logger
+from email_validator import validate_email, EmailNotValidError
 
 
 class EmailerNotSetupError(Exception):
     ...
 
 
 class DisplayManualQuit(Exception):
@@ -46,57 +47,81 @@
 
         self.email_app_name = email_app_name
 
         self.display_window = display_window
         self.auto_send = auto_send
         self.send_emails = send_emails
         self._setup_was_run = False
+        self._current_user_email = None
 
         self._recipient = None
         self._subject = None
         self._text = None
         self.read_folder = None
 
         try:
-            self.email_app = win32.Dispatch(self.email_app_name)
-            self._mapi_ns = self.email_app.GetNamespace('MAPI')
+            if self.email_app_name.lower().startswith('outlook'):
+                self.email_app = win32.Dispatch(self.email_app_name).GetNamespace('MAPI')
+                self._logger.debug("MAPI namespace in use.")
+            else:
+                self.email_app = win32.Dispatch(self.email_app_name)
             self.email = self.email_app.CreateItem(0)
         except com_error as e:
             self._logger.error(e, exc_info=True)
             raise e
 
         self._email_signature = None
         self._send_success = False
         self.email_sig_filename = email_sig_filename
 
     @property
+    def current_user_email(self):
+        if self.email_app_name.lower().startswith('outlook'):
+            self._current_user_email = (
+                self.email_app.Application.Session.CurrentUser.AddressEntry.GetExchangeUser().PrimarySmtpAddress)
+        return self._current_user_email
+
+    @current_user_email.setter
+    def current_user_email(self, value):
+        try:
+            if validate_email(value, check_deliverability=False):
+                self._current_user_email = value
+        except EmailNotValidError as e:
+            self._logger.error(e, exc_info=True)
+            value = None
+        self._current_user_email = value
+
+    @property
     def email_signature(self):
         return self._email_signature
 
     @email_signature.getter
     def email_signature(self):
-        signature_full_path = join(self.signature_dir_path, self.email_sig_filename)
-        if isdir(self.signature_dir_path):
-            pass
-        else:
-            try:
-                raise NotADirectoryError(f"{self.signature_dir_path} does not exist.")
-            except NotADirectoryError as e:
-                self._logger.warning(e)
-                self._email_signature = None
-
-        if isfile(signature_full_path):
-            with open(signature_full_path, 'r', encoding='utf-16') as f:
-                self._email_signature = f.read().strip()
+        if self.email_sig_filename:
+            signature_full_path = join(self.signature_dir_path, self.email_sig_filename)
+            if isdir(self.signature_dir_path):
+                pass
+            else:
+                try:
+                    raise NotADirectoryError(f"{self.signature_dir_path} does not exist.")
+                except NotADirectoryError as e:
+                    self._logger.warning(e)
+                    self._email_signature = None
+
+            if isfile(signature_full_path):
+                with open(signature_full_path, 'r', encoding='utf-16') as f:
+                    self._email_signature = f.read().strip()
+            else:
+                try:
+                    raise FileNotFoundError(f"{signature_full_path} does not exist.")
+                except FileNotFoundError as e:
+                    self._logger.warning(e)
+                    self._email_signature = None
         else:
-            try:
-                raise FileNotFoundError(f"{signature_full_path} does not exist.")
-            except FileNotFoundError as e:
-                self._logger.warning(e)
-                self._email_signature = None
+            self._email_signature = None
 
         return self._email_signature
 
     @property
     def send_success(self):
         return self._send_success
 
@@ -125,15 +150,15 @@
                     raise DisplayManualQuit("User cancelled operation due to DisplayTrackingWarning.")
                 except DisplayManualQuit as e:
                     self._logger.error(e, exc_info=True)
                     raise e
 
     def _GetReadFolder(self, email_dir_index: int = 6):
         # 6 = inbox
-        self.read_folder = self._mapi_ns.GetDefaultFolder(email_dir_index)
+        self.read_folder = self.email_app.GetDefaultFolder(email_dir_index)
         return self.read_folder
 
     def GetMessages(self, folder_index=None):
         if isinstance(folder_index, int):
             self.read_folder = self._GetReadFolder(folder_index)
         elif not folder_index and self.read_folder:
             pass
```

### Comparing `PyEmailerAJM-1.5/PyEmailerAJM.egg-info/PKG-INFO` & `PyEmailerAJM-1.5.1/PyEmailerAJM.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: PyEmailerAJM
-Version: 1.5
+Version: 1.5.1
 Summary: Allows for automating sending Email with the Outlook Desktop client. Future releases will add more client support
 Home-page: https://github.com/amcsparron2793-Water/PyEmailer
 Author: Amcsparron
 Author-email: amcsparron@albanyny.gov
 License: MIT License
-Download-URL: https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.5.tar.gz
+Download-URL: https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.5.1.tar.gz
 Keywords: Outlook,Email,Automation
 Platform: UNKNOWN
 License-File: LICENSE.txt
 
 UNKNOWN
```

### Comparing `PyEmailerAJM-1.5/README.md` & `PyEmailerAJM-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `PyEmailerAJM-1.5/setup.py` & `PyEmailerAJM-1.5.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 setup(
     name='PyEmailerAJM',
-    version='1.5',
+    version='1.5.1',
     packages=['PyEmailerAJM'],
     url='https://github.com/amcsparron2793-Water/PyEmailer',
-    download_url='https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.5.tar.gz',
+    download_url='https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.5.1.tar.gz',
     keywords=["Outlook", "Email", "Automation"],
     install_requires=['pywin32'],
     license='MIT License',
     author='Amcsparron',
     author_email='amcsparron@albanyny.gov',
     description='Allows for automating sending Email with the Outlook Desktop client. Future releases will add more client support'
 )
```

