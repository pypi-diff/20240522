# Comparing `tmp/PyEmailerAJM-1.4.tar.gz` & `tmp/PyEmailerAJM-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyEmailerAJM-1.4.tar", last modified: Thu May 16 12:31:58 2024, max compression
+gzip compressed data, was "PyEmailerAJM-1.5.tar", last modified: Wed May 22 13:55:57 2024, max compression
```

## Comparing `PyEmailerAJM-1.4.tar` & `PyEmailerAJM-1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:31:58.052281 PyEmailerAJM-1.4/
--rw-rw-rw-   0        0        0     1084 2023-09-12 19:19:18.000000 PyEmailerAJM-1.4/LICENSE.txt
--rw-rw-rw-   0        0        0      513 2024-05-16 12:31:58.053320 PyEmailerAJM-1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 12:31:58.027365 PyEmailerAJM-1.4/PyEmailerAJM/
--rw-rw-rw-   0        0        0    11749 2024-05-16 11:47:45.000000 PyEmailerAJM-1.4/PyEmailerAJM/PyEmailerAJM.py
--rw-rw-rw-   0        0        0      109 2023-09-13 15:44:18.000000 PyEmailerAJM-1.4/PyEmailerAJM/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:31:58.050323 PyEmailerAJM-1.4/PyEmailerAJM.egg-info/
--rw-rw-rw-   0        0        0      513 2024-05-16 12:31:57.000000 PyEmailerAJM-1.4/PyEmailerAJM.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-05-16 12:31:57.000000 PyEmailerAJM-1.4/PyEmailerAJM.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:31:57.000000 PyEmailerAJM-1.4/PyEmailerAJM.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-16 12:31:57.000000 PyEmailerAJM-1.4/PyEmailerAJM.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-16 12:31:57.000000 PyEmailerAJM-1.4/PyEmailerAJM.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      545 2024-05-16 12:24:41.000000 PyEmailerAJM-1.4/README.md
--rw-rw-rw-   0        0        0       86 2024-05-16 12:31:58.057267 PyEmailerAJM-1.4/setup.cfg
--rw-rw-rw-   0        0        0      600 2024-05-16 11:59:38.000000 PyEmailerAJM-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:55:57.535041 PyEmailerAJM-1.5/
+-rw-rw-rw-   0        0        0     1084 2023-09-12 19:19:18.000000 PyEmailerAJM-1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0      513 2024-05-22 13:55:57.535041 PyEmailerAJM-1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 13:55:57.511080 PyEmailerAJM-1.5/PyEmailerAJM/
+-rw-rw-rw-   0        0        0    13448 2024-05-22 13:46:34.000000 PyEmailerAJM-1.5/PyEmailerAJM/PyEmailerAJM.py
+-rw-rw-rw-   0        0        0      109 2023-09-13 15:44:18.000000 PyEmailerAJM-1.5/PyEmailerAJM/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:55:57.532023 PyEmailerAJM-1.5/PyEmailerAJM.egg-info/
+-rw-rw-rw-   0        0        0      513 2024-05-22 13:55:57.000000 PyEmailerAJM-1.5/PyEmailerAJM.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-05-22 13:55:57.000000 PyEmailerAJM-1.5/PyEmailerAJM.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 13:55:57.000000 PyEmailerAJM-1.5/PyEmailerAJM.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-22 13:55:57.000000 PyEmailerAJM-1.5/PyEmailerAJM.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-22 13:55:57.000000 PyEmailerAJM-1.5/PyEmailerAJM.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      545 2024-05-16 12:24:41.000000 PyEmailerAJM-1.5/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-22 13:55:57.539021 PyEmailerAJM-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      600 2024-05-22 13:53:55.000000 PyEmailerAJM-1.5/setup.py
```

### Comparing `PyEmailerAJM-1.4/LICENSE.txt` & `PyEmailerAJM-1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyEmailerAJM-1.4/PKG-INFO` & `PyEmailerAJM-1.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: PyEmailerAJM
-Version: 1.4
+Version: 1.5
 Summary: Allows for automating sending Email with the Outlook Desktop client. Future releases will add more client support
 Home-page: https://github.com/amcsparron2793-Water/PyEmailer
 Author: Amcsparron
 Author-email: amcsparron@albanyny.gov
 License: MIT License
-Download-URL: https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.4.tar.gz
+Download-URL: https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.5.tar.gz
 Keywords: Outlook,Email,Automation
 Platform: UNKNOWN
 License-File: LICENSE.txt
 
 UNKNOWN
```

### Comparing `PyEmailerAJM-1.4/PyEmailerAJM/PyEmailerAJM.py` & `PyEmailerAJM-1.5/PyEmailerAJM/PyEmailerAJM.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,20 +16,26 @@
 from logging import Logger
 
 
 class EmailerNotSetupError(Exception):
     ...
 
 
+class DisplayManualQuit(Exception):
+    ...
+
+
 class PyEmailer:
     # the email tab_char
     tab_char = '&emsp;'
     signature_dir_path = join((environ['USERPROFILE']),
                               'AppData\\Roaming\\Microsoft\\Signatures\\')
 
+    DisplayEmailSendTrackingWarning = "THIS TYPE OF SEND CANNOT BE DETECTED FOR SEND SUCCESS AUTOMATICALLY."
+
     def __init__(self, display_window: bool,
                  send_emails: bool, logger: Logger = None,
                  email_sig_filename: str = None,
                  auto_send: bool = False,
                  email_app_name: str = 'outlook.application'):
 
         if logger:
@@ -55,14 +61,15 @@
             self._mapi_ns = self.email_app.GetNamespace('MAPI')
             self.email = self.email_app.CreateItem(0)
         except com_error as e:
             self._logger.error(e, exc_info=True)
             raise e
 
         self._email_signature = None
+        self._send_success = False
         self.email_sig_filename = email_sig_filename
 
     @property
     def email_signature(self):
         return self._email_signature
 
     @email_signature.getter
@@ -85,14 +92,45 @@
                 raise FileNotFoundError(f"{signature_full_path} does not exist.")
             except FileNotFoundError as e:
                 self._logger.warning(e)
                 self._email_signature = None
 
         return self._email_signature
 
+    @property
+    def send_success(self):
+        return self._send_success
+
+    @send_success.setter
+    def send_success(self, value):
+        self._send_success = value
+
+    def _display_tracking_warning_confirm(self):
+        while True:
+            q = input(f"{self.DisplayEmailSendTrackingWarning}. Do you understand? (y/n): ").lower().strip()
+            if q == 'y':
+                self._logger.warning(self.DisplayEmailSendTrackingWarning)
+                return True
+            elif q == 'n':
+                return False
+            else:
+                print("Please respond with 'y' or 'n'.")
+
+    def display_tracker_check(self) -> bool:
+        if self.display_window:
+            c = self._display_tracking_warning_confirm()
+            if c:
+                return c
+            else:
+                try:
+                    raise DisplayManualQuit("User cancelled operation due to DisplayTrackingWarning.")
+                except DisplayManualQuit as e:
+                    self._logger.error(e, exc_info=True)
+                    raise e
+
     def _GetReadFolder(self, email_dir_index: int = 6):
         # 6 = inbox
         self.read_folder = self._mapi_ns.GetDefaultFolder(email_dir_index)
         return self.read_folder
 
     def GetMessages(self, folder_index=None):
         if isinstance(folder_index, int):
@@ -121,28 +159,38 @@
                 self._logger.error(e, exc_info=True)
                 raise e
 
     def FindMsgBySubject(self, subject: str, forwarded_message_match: bool = True,
                          reply_msg_match: bool = True) -> list:
         """Matches the message.Subject string to the subject attr string and returns a list of messages.
         If forward_message_match is True than messages are matched without
-        regard to if they start with 'FW:' or 'FWD:'"""
+        regard to if they start with 'FW:' or 'FWD:'
+
+        If reply_msg_match is True than messages are matched without
+        regard to if they start with 'RE:'
+        """
         matched_messages = []
+        subject = subject.lower().strip()
+        fw_str = 'FW:'.lower()
+        fwd_str = 'FWD:'.lower()
+        re_str = 'RE:'.lower()
+
         for message in self.GetMessages():
+            message.Subject = message.Subject.lower()
             if forwarded_message_match:
                 if (message.Subject == subject or
-                        (message.Subject.startswith('FW:')
-                         and message.Subject.split('FW:')[1].strip() == subject) or
-                        (message.Subject.startswith('FWD:')
-                         and message.Subject.split('FWD:')[1].strip() == subject)):
+                        (message.Subject.startswith(fw_str)
+                         and message.Subject.split(fw_str)[1].strip() == subject) or
+                        (message.Subject.startswith(fwd_str)
+                         and message.Subject.split(fwd_str)[1].strip() == subject)):
                     matched_messages.append(message)
             if reply_msg_match:
                 if (message.Subject == subject or
-                        (message.Subject.startswith('RE:')
-                         and message.Subject.split('RE:')[1].strip() == subject)):
+                        (message.Subject.startswith(re_str)
+                         and message.Subject.split(re_str)[1].strip() == subject)):
                     matched_messages.append(message)
             else:
                 if message.Subject == subject:
                     matched_messages.append(message)
 
         return matched_messages
 
@@ -218,16 +266,18 @@
             self.email.Display(True)
         except Exception as e:
             self._logger.error(e, exc_info=True)
             raise e
 
     def _send(self):
         try:
+            self.send_success = False
             self.email.Send()
             # print(f"Mail sent to {self._recipient}")
+            self.send_success = True
             self._logger.info(f"Mail successfully sent to {self._recipient}")
         except Exception as e:
             self._logger.error(e, exc_info=True)
             raise e
 
     def _manual_send_loop(self):
         while True:
```

### Comparing `PyEmailerAJM-1.4/PyEmailerAJM.egg-info/PKG-INFO` & `PyEmailerAJM-1.5/PyEmailerAJM.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: PyEmailerAJM
-Version: 1.4
+Version: 1.5
 Summary: Allows for automating sending Email with the Outlook Desktop client. Future releases will add more client support
 Home-page: https://github.com/amcsparron2793-Water/PyEmailer
 Author: Amcsparron
 Author-email: amcsparron@albanyny.gov
 License: MIT License
-Download-URL: https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.4.tar.gz
+Download-URL: https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.5.tar.gz
 Keywords: Outlook,Email,Automation
 Platform: UNKNOWN
 License-File: LICENSE.txt
 
 UNKNOWN
```

### Comparing `PyEmailerAJM-1.4/README.md` & `PyEmailerAJM-1.5/README.md`

 * *Files identical despite different names*

### Comparing `PyEmailerAJM-1.4/setup.py` & `PyEmailerAJM-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 setup(
     name='PyEmailerAJM',
-    version='1.4',
+    version='1.5',
     packages=['PyEmailerAJM'],
     url='https://github.com/amcsparron2793-Water/PyEmailer',
-    download_url='https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.4.tar.gz',
+    download_url='https://github.com/amcsparron2793-Water/PyEmailer/archive/refs/tags/1.5.tar.gz',
     keywords=["Outlook", "Email", "Automation"],
     install_requires=['pywin32'],
     license='MIT License',
     author='Amcsparron',
     author_email='amcsparron@albanyny.gov',
     description='Allows for automating sending Email with the Outlook Desktop client. Future releases will add more client support'
 )
```

