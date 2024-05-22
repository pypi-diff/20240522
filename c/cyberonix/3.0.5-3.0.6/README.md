# Comparing `tmp/cyberonix-3.0.5.tar.gz` & `tmp/cyberonix-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberonix-3.0.5.tar", last modified: Tue May 21 04:26:31 2024, max compression
+gzip compressed data, was "cyberonix-3.0.6.tar", last modified: Wed May 22 16:17:23 2024, max compression
```

## Comparing `cyberonix-3.0.5.tar` & `cyberonix-3.0.6.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 04:26:31.445461 cyberonix-3.0.5/
--rw-r--r--   0 root         (0) root         (0)    23928 2024-05-21 04:26:31.445461 cyberonix-3.0.5/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)    23115 2024-03-14 18:35:27.000000 cyberonix-3.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 04:26:31.437461 cyberonix-3.0.5/cyberonix/
--rwxr-xr-x   0 root         (0) root         (0)       44 2024-05-12 16:31:41.000000 cyberonix-3.0.5/cyberonix/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13538 2024-05-21 04:26:04.000000 cyberonix-3.0.5/cyberonix/cyberonix.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 04:26:31.437461 cyberonix-3.0.5/cyberonix/main/
--rw-r--r--   0 root         (0) root         (0)    24214 2024-05-21 04:01:49.000000 cyberonix-3.0.5/cyberonix/main/Bug_Bounty.py
--rw-r--r--   0 root         (0) root         (0)       50 2024-05-17 14:30:27.000000 cyberonix-3.0.5/cyberonix/main/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31514 2024-05-21 04:01:32.000000 cyberonix-3.0.5/cyberonix/main/arguments.py
--rw-r--r--   0 root         (0) root         (0)     2827 2024-05-21 04:01:59.000000 cyberonix-3.0.5/cyberonix/main/tool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 04:26:31.445461 cyberonix-3.0.5/cyberonix/main/tools/
--rw-r--r--   0 root         (0) root         (0)     4424 2024-05-21 04:02:32.000000 cyberonix-3.0.5/cyberonix/main/tools/Anonymity.py
--rw-r--r--   0 root         (0) root         (0)     7887 2024-05-21 04:02:42.000000 cyberonix-3.0.5/cyberonix/main/tools/Authentication.py
--rw-r--r--   0 root         (0) root         (0)     9826 2024-05-21 04:02:52.000000 cyberonix-3.0.5/cyberonix/main/tools/Authorization.py
--rw-r--r--   0 root         (0) root         (0)    13287 2024-05-21 04:03:15.000000 cyberonix-3.0.5/cyberonix/main/tools/Configuration_Management.py
--rw-r--r--   0 root         (0) root         (0)     5964 2024-05-21 04:03:30.000000 cyberonix-3.0.5/cyberonix/main/tools/Cryptography.py
--rw-r--r--   0 root         (0) root         (0)    10863 2024-05-21 04:04:02.000000 cyberonix-3.0.5/cyberonix/main/tools/Exploitation_Tools.py
--rw-r--r--   0 root         (0) root         (0)     5238 2024-05-21 04:04:11.000000 cyberonix-3.0.5/cyberonix/main/tools/File_Upload.py
--rw-r--r--   0 root         (0) root         (0)      410 2024-05-21 04:04:36.000000 cyberonix-3.0.5/cyberonix/main/tools/Framework.py
--rw-r--r--   0 root         (0) root         (0)    28889 2024-05-21 04:05:17.000000 cyberonix-3.0.5/cyberonix/main/tools/Password_Hacking.py
--rw-r--r--   0 root         (0) root         (0)     4881 2024-05-21 04:05:32.000000 cyberonix-3.0.5/cyberonix/main/tools/Pentesting_Bug_Bounty.py
--rw-r--r--   0 root         (0) root         (0)    16560 2024-05-21 04:05:45.000000 cyberonix-3.0.5/cyberonix/main/tools/PostExploitationAttacks.py
--rw-r--r--   0 root         (0) root         (0)   171224 2024-05-21 04:05:55.000000 cyberonix-3.0.5/cyberonix/main/tools/Recommended_Tool.py
--rw-r--r--   0 root         (0) root         (0)     5992 2024-05-21 04:06:19.000000 cyberonix-3.0.5/cyberonix/main/tools/RiskyFuncPayment.py
--rw-r--r--   0 root         (0) root         (0)     5204 2024-05-21 04:06:31.000000 cyberonix-3.0.5/cyberonix/main/tools/Secure_Transmission.py
--rw-r--r--   0 root         (0) root         (0)    11474 2024-05-21 04:06:42.000000 cyberonix-3.0.5/cyberonix/main/tools/Session_Management.py
--rw-r--r--   0 root         (0) root         (0)    10736 2024-05-21 04:06:51.000000 cyberonix-3.0.5/cyberonix/main/tools/Sniffing_and_Spoofing.py
--rw-r--r--   0 root         (0) root         (0)     7140 2024-05-21 04:07:13.000000 cyberonix-3.0.5/cyberonix/main/tools/Vulnerability_Analysis.py
--rw-r--r--   0 root         (0) root         (0)    13445 2024-05-21 04:07:26.000000 cyberonix-3.0.5/cyberonix/main/tools/WEB_Application_Analysis.py
--rw-r--r--   0 root         (0) root         (0)     6825 2024-05-21 04:07:40.000000 cyberonix-3.0.5/cyberonix/main/tools/Wireless_Hacking.py
--rw-r--r--   0 root         (0) root         (0)      359 2024-05-17 14:30:27.000000 cyberonix-3.0.5/cyberonix/main/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7351 2024-05-21 04:03:01.000000 cyberonix-3.0.5/cyberonix/main/tools/banner.py
--rw-r--r--   0 root         (0) root         (0)      207 2024-05-17 14:30:27.000000 cyberonix-3.0.5/cyberonix/main/tools/colors.py
--rw-r--r--   0 root         (0) root         (0)    27322 2024-05-21 04:03:43.000000 cyberonix-3.0.5/cyberonix/main/tools/data_validation.py
--rw-r--r--   0 root         (0) root         (0)     5787 2024-05-21 04:03:52.000000 cyberonix-3.0.5/cyberonix/main/tools/dos.py
--rw-r--r--   0 root         (0) root         (0)     4864 2024-05-21 04:04:21.000000 cyberonix-3.0.5/cyberonix/main/tools/forensic.py
--rw-r--r--   0 root         (0) root         (0)     5252 2024-05-21 04:04:48.000000 cyberonix-3.0.5/cyberonix/main/tools/html5.py
--rw-r--r--   0 root         (0) root         (0)    18178 2024-05-21 04:05:05.000000 cyberonix-3.0.5/cyberonix/main/tools/information_gathering.py
--rw-r--r--   0 root         (0) root         (0)      654 2024-05-17 14:30:27.000000 cyberonix-3.0.5/cyberonix/main/tools/run_on_browser.py
--rw-r--r--   0 root         (0) root         (0)    16802 2024-05-21 04:07:02.000000 cyberonix-3.0.5/cyberonix/main/tools/template.py
--rw-r--r--   0 root         (0) root         (0)       78 2024-05-17 14:30:27.000000 cyberonix-3.0.5/cyberonix/main/tools/waiting.py
--rw-r--r--   0 root         (0) root         (0)      907 2024-05-21 04:07:51.000000 cyberonix-3.0.5/cyberonix/main/tools/writeup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 04:26:31.437461 cyberonix-3.0.5/cyberonix.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23928 2024-05-21 04:26:31.000000 cyberonix-3.0.5/cyberonix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1575 2024-05-21 04:26:31.000000 cyberonix-3.0.5/cyberonix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 04:26:31.000000 cyberonix-3.0.5/cyberonix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2024-05-21 04:26:31.000000 cyberonix-3.0.5/cyberonix.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       68 2024-05-21 04:26:31.000000 cyberonix-3.0.5/cyberonix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2024-05-21 04:26:31.000000 cyberonix-3.0.5/cyberonix.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-21 04:26:31.445461 cyberonix-3.0.5/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     1330 2024-05-21 04:26:24.000000 cyberonix-3.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:17:23.508551 cyberonix-3.0.6/
+-rw-r--r--   0 root         (0) root         (0)    24892 2024-05-22 16:17:23.508551 cyberonix-3.0.6/PKG-INFO
+-rw-------   0 root         (0) root         (0)    24079 2024-05-22 16:01:00.000000 cyberonix-3.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:17:23.496552 cyberonix-3.0.6/cyberonix/
+-rwxr-xr-x   0 root         (0) root         (0)       44 2024-05-12 16:31:41.000000 cyberonix-3.0.6/cyberonix/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13538 2024-05-21 04:26:04.000000 cyberonix-3.0.6/cyberonix/cyberonix.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:17:23.500552 cyberonix-3.0.6/cyberonix/main/
+-rw-r--r--   0 root         (0) root         (0)    24214 2024-05-21 04:01:49.000000 cyberonix-3.0.6/cyberonix/main/Bug_Bounty.py
+-rw-r--r--   0 root         (0) root         (0)       50 2024-05-17 14:30:27.000000 cyberonix-3.0.6/cyberonix/main/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    31514 2024-05-21 04:01:32.000000 cyberonix-3.0.6/cyberonix/main/arguments.py
+-rw-r--r--   0 root         (0) root         (0)     2827 2024-05-21 04:01:59.000000 cyberonix-3.0.6/cyberonix/main/tool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:17:23.508551 cyberonix-3.0.6/cyberonix/main/tools/
+-rw-r--r--   0 root         (0) root         (0)     4424 2024-05-21 04:02:32.000000 cyberonix-3.0.6/cyberonix/main/tools/Anonymity.py
+-rw-r--r--   0 root         (0) root         (0)     7887 2024-05-21 04:02:42.000000 cyberonix-3.0.6/cyberonix/main/tools/Authentication.py
+-rw-r--r--   0 root         (0) root         (0)     9826 2024-05-21 04:02:52.000000 cyberonix-3.0.6/cyberonix/main/tools/Authorization.py
+-rw-r--r--   0 root         (0) root         (0)    13287 2024-05-21 04:03:15.000000 cyberonix-3.0.6/cyberonix/main/tools/Configuration_Management.py
+-rw-r--r--   0 root         (0) root         (0)     5964 2024-05-21 04:03:30.000000 cyberonix-3.0.6/cyberonix/main/tools/Cryptography.py
+-rw-r--r--   0 root         (0) root         (0)    10863 2024-05-21 04:04:02.000000 cyberonix-3.0.6/cyberonix/main/tools/Exploitation_Tools.py
+-rw-r--r--   0 root         (0) root         (0)     5238 2024-05-21 04:04:11.000000 cyberonix-3.0.6/cyberonix/main/tools/File_Upload.py
+-rw-r--r--   0 root         (0) root         (0)      410 2024-05-21 04:04:36.000000 cyberonix-3.0.6/cyberonix/main/tools/Framework.py
+-rw-r--r--   0 root         (0) root         (0)    28889 2024-05-21 04:05:17.000000 cyberonix-3.0.6/cyberonix/main/tools/Password_Hacking.py
+-rw-r--r--   0 root         (0) root         (0)     4881 2024-05-21 04:05:32.000000 cyberonix-3.0.6/cyberonix/main/tools/Pentesting_Bug_Bounty.py
+-rw-r--r--   0 root         (0) root         (0)    16560 2024-05-21 04:05:45.000000 cyberonix-3.0.6/cyberonix/main/tools/PostExploitationAttacks.py
+-rw-r--r--   0 root         (0) root         (0)   171224 2024-05-21 04:05:55.000000 cyberonix-3.0.6/cyberonix/main/tools/Recommended_Tool.py
+-rw-r--r--   0 root         (0) root         (0)     5992 2024-05-21 04:06:19.000000 cyberonix-3.0.6/cyberonix/main/tools/RiskyFuncPayment.py
+-rw-r--r--   0 root         (0) root         (0)     5204 2024-05-21 04:06:31.000000 cyberonix-3.0.6/cyberonix/main/tools/Secure_Transmission.py
+-rw-r--r--   0 root         (0) root         (0)    11474 2024-05-21 04:06:42.000000 cyberonix-3.0.6/cyberonix/main/tools/Session_Management.py
+-rw-r--r--   0 root         (0) root         (0)    10736 2024-05-21 04:06:51.000000 cyberonix-3.0.6/cyberonix/main/tools/Sniffing_and_Spoofing.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2024-05-21 04:07:13.000000 cyberonix-3.0.6/cyberonix/main/tools/Vulnerability_Analysis.py
+-rw-r--r--   0 root         (0) root         (0)    13445 2024-05-21 04:07:26.000000 cyberonix-3.0.6/cyberonix/main/tools/WEB_Application_Analysis.py
+-rw-r--r--   0 root         (0) root         (0)     6825 2024-05-21 04:07:40.000000 cyberonix-3.0.6/cyberonix/main/tools/Wireless_Hacking.py
+-rw-r--r--   0 root         (0) root         (0)      359 2024-05-17 14:30:27.000000 cyberonix-3.0.6/cyberonix/main/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7351 2024-05-21 04:03:01.000000 cyberonix-3.0.6/cyberonix/main/tools/banner.py
+-rw-r--r--   0 root         (0) root         (0)      207 2024-05-17 14:30:27.000000 cyberonix-3.0.6/cyberonix/main/tools/colors.py
+-rw-r--r--   0 root         (0) root         (0)    27322 2024-05-21 04:03:43.000000 cyberonix-3.0.6/cyberonix/main/tools/data_validation.py
+-rw-r--r--   0 root         (0) root         (0)     5787 2024-05-21 04:03:52.000000 cyberonix-3.0.6/cyberonix/main/tools/dos.py
+-rw-r--r--   0 root         (0) root         (0)     4864 2024-05-21 04:04:21.000000 cyberonix-3.0.6/cyberonix/main/tools/forensic.py
+-rw-r--r--   0 root         (0) root         (0)     5252 2024-05-21 04:04:48.000000 cyberonix-3.0.6/cyberonix/main/tools/html5.py
+-rw-r--r--   0 root         (0) root         (0)    18178 2024-05-21 04:05:05.000000 cyberonix-3.0.6/cyberonix/main/tools/information_gathering.py
+-rw-r--r--   0 root         (0) root         (0)      654 2024-05-17 14:30:27.000000 cyberonix-3.0.6/cyberonix/main/tools/run_on_browser.py
+-rw-r--r--   0 root         (0) root         (0)    16802 2024-05-21 04:07:02.000000 cyberonix-3.0.6/cyberonix/main/tools/template.py
+-rw-r--r--   0 root         (0) root         (0)       78 2024-05-17 14:30:27.000000 cyberonix-3.0.6/cyberonix/main/tools/waiting.py
+-rw-r--r--   0 root         (0) root         (0)      907 2024-05-21 04:07:51.000000 cyberonix-3.0.6/cyberonix/main/tools/writeup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 16:17:23.500552 cyberonix-3.0.6/cyberonix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    24892 2024-05-22 16:17:23.000000 cyberonix-3.0.6/cyberonix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1575 2024-05-22 16:17:23.000000 cyberonix-3.0.6/cyberonix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 16:17:23.000000 cyberonix-3.0.6/cyberonix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2024-05-22 16:17:23.000000 cyberonix-3.0.6/cyberonix.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2024-05-22 16:17:23.000000 cyberonix-3.0.6/cyberonix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2024-05-22 16:17:23.000000 cyberonix-3.0.6/cyberonix.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-22 16:17:23.508551 cyberonix-3.0.6/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     1330 2024-05-22 16:17:15.000000 cyberonix-3.0.6/setup.py
```

### Comparing `cyberonix-3.0.5/PKG-INFO` & `cyberonix-3.0.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberonix
-Version: 3.0.5
+Version: 3.0.6
 Summary: Cyberonix is a complete resource hub for Cyber Security Community.
 Home-page: https://github.com/TeamDefronix/Cyberonix
 Author: Defronix
 Author-email: hello@defronix.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -527,15 +527,19 @@
 ## ![Information Gathering](https://imgur.com/f1jai90.png)
 
 ![Nmap](https://imgur.com/CoYpmNC.png)
 
 <h1 align="left">Socials</h1>
 
 <p align="left">
-<a href="https://github.com/TeamDefronix"><img src="https://user-images.githubusercontent.com/696094/196835284-c52d4bd1-7034-439e-848b-47d4f2933dff.svg" width="64" height="64" alt="Github Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/> <a href="https://discord.gg/defronix"><img src="https://user-images.githubusercontent.com/696094/196835282-f5c47d66-29b7-4210-9ee0-d9cdecde3559.svg" width="64" height="64" alt="Discord Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/> <a href="https://twitter.com/niteshlike123"><img src="https://user-images.githubusercontent.com/696094/196835281-52617611-ede6-40da-a4bc-8c5025622bbf.svg" width="64" height="64" alt="Twitter Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/>
+<a href="https://github.com/TeamDefronix"><img src="https://github.com/gauravghongde/social-icons/raw/master/SVG/Color/Github.svg" width="64" height="64" alt="Github Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/> <a href="https://www.facebook.com/defronix"><img src="https://raw.githubusercontent.com/gauravghongde/social-icons/master/SVG/Color/Facebook.svg" width="64" height="64" alt="Facebook Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/> <a href="https://twitter.com/teamdefronix"><img src="https://github.com/gauravghongde/social-icons/raw/master/SVG/Color/Twitter.svg" width="64" height="64" alt="Twitter Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/>
+<a href="https://instagram.com/teamdefronix"><img src="https://github.com/gauravghongde/social-icons/raw/master/SVG/Color/Instagram.svg" width="64" height="64" alt="Instagram Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/>
+<a href="https://whatsapp.com/channel/0029VaGltobEKyZ8eX8Ki82w"><img src="https://github.com/gauravghongde/social-icons/raw/master/SVG/Color/WhatsApp.svg" width="64" height="64" alt="WhatsApp Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/>
+<a href="https://youtube.com/@defronix"><img src="https://github.com/gauravghongde/social-icons/raw/master/SVG/Color/Youtube.svg" width="64" height="64" alt="Youtube Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/>
+<a href="https://www.linkedin.com/company/defronix/"><img src="https://github.com/gauravghongde/social-icons/raw/master/SVG/Color/LinkedIN.svg" width="64" height="64" alt="LinkedIN Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/>
 </p>
 
 <h1 align="left">Support</h1>
 
 <p><a href="https://www.buymeacoffee.com/metaxone" target="_blank"> <img align="left" src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="50" width="210" alt="Buymeacoffee" /></a></p><br><br><br>
 <p><a href="https://paypal.me/niteshsinghhacker" target="_blank"> <img align="left" src="https://raw.githubusercontent.com/andreostrovsky/donate-with-paypal/master/blue.svg" height="70" width="210" alt="Donate with paypal" /></a></p><br><br><br>
 <p><a href="https://tools.apgy.in/upi/Nitesh+Singh/niteshkumar5@ybl/" target="_blank"> <img align="left" style="border-radius:8px" src="https://user-images.githubusercontent.com/122822828/216837693-3480fcd2-b4fc-40ff-94f8-c5d7d4b82ad5.png" height="50" width="210" alt="Donate with paypal" /></a></p><br><br><br>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberonix Version: 3.0.5 Summary: Cyberonix is a
+Metadata-Version: 2.1 Name: cyberonix Version: 3.0.6 Summary: Cyberonix is a
 complete resource hub for Cyber Security Community. Home-page: https://
 github.com/TeamDefronix/Cyberonix Author: Defronix Author-email:
 hello@defronix.com License: MIT Classifier: Development Status :: 5 -
 Production/Stable Classifier: Intended Audience :: Developers Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.6 Classifier: Programming Language ::
@@ -212,16 +212,19 @@
 www.offsec.com/courses/web-300/) - ## Bug Bounty - Bug Bounty for Beginners -
 Reconnaissance - Intel Discovery - Enumeration - Vulnerability Analysis -
 Exploitation - Reporting # Screenshots ## ![Main Menu](https://imgur.com/
 e2b26Mf.png) ## ![Bug Bounty](https://imgur.com/Sa4fdLU.png) ## ![Tools](https:
 //imgur.com/3pc76rB.png) ## ![Information Gathering](https://imgur.com/
 f1jai90.png) ![Nmap](https://imgur.com/CoYpmNC.png)
 ************ SSoocciiaallss ************
-_[_G_i_t_h_u_b_ _L_o_g_o_][assets/misc/transparent.png]_[_D_i_s_c_o_r_d_ _L_o_g_o_][assets/misc/
-transparent.png]_[_T_w_i_t_t_e_r_ _L_o_g_o_][assets/misc/transparent.png]
+_[_G_i_t_h_u_b_ _L_o_g_o_][assets/misc/transparent.png]_[_F_a_c_e_b_o_o_k_ _L_o_g_o_][assets/misc/
+transparent.png]_[_T_w_i_t_t_e_r_ _L_o_g_o_][assets/misc/transparent.png]_[_I_n_s_t_a_g_r_a_m_ _L_o_g_o_]
+[assets/misc/transparent.png]_[_W_h_a_t_s_A_p_p_ _L_o_g_o_][assets/misc/transparent.png]
+_[_Y_o_u_t_u_b_e_ _L_o_g_o_][assets/misc/transparent.png]_[_L_i_n_k_e_d_I_N_ _L_o_g_o_][assets/misc/
+transparent.png]
 ************ SSuuppppoorrtt ************
 _[_B_u_y_m_e_a_c_o_f_f_e_e_]
 
 
 
 _[_D_o_n_a_t_e_ _w_i_t_h_ _p_a_y_p_a_l_]
```

### Comparing `cyberonix-3.0.5/README.md` & `cyberonix-3.0.6/cyberonix.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: cyberonix
+Version: 3.0.6
+Summary: Cyberonix is a complete resource hub for Cyber Security Community.
+Home-page: https://github.com/TeamDefronix/Cyberonix
+Author: Defronix
+Author-email: hello@defronix.com
+License: MIT
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Security
+Description-Content-Type: text/markdown
+
 <div align="center"><p>
     <h1>CYBERONIX</h1>
     <img style="filter: brightness(200%)" src="https://user-images.githubusercontent.com/122822828/216810369-34904b5a-d063-48a9-a87d-11caf293243b.png" width="50%"><br>
     <img src="https://forthebadge.com/images/badges/made-with-python.svg">
     <img src="https://forthebadge.com/images/badges/built-with-love.svg">
     <br><br>
     <a href="https://github.com/TeamDefronix/Cyberonix/releases/latest">
@@ -506,15 +527,19 @@
 ## ![Information Gathering](https://imgur.com/f1jai90.png)
 
 ![Nmap](https://imgur.com/CoYpmNC.png)
 
 <h1 align="left">Socials</h1>
 
 <p align="left">
-<a href="https://github.com/TeamDefronix"><img src="https://user-images.githubusercontent.com/696094/196835284-c52d4bd1-7034-439e-848b-47d4f2933dff.svg" width="64" height="64" alt="Github Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/> <a href="https://discord.gg/defronix"><img src="https://user-images.githubusercontent.com/696094/196835282-f5c47d66-29b7-4210-9ee0-d9cdecde3559.svg" width="64" height="64" alt="Discord Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/> <a href="https://twitter.com/niteshlike123"><img src="https://user-images.githubusercontent.com/696094/196835281-52617611-ede6-40da-a4bc-8c5025622bbf.svg" width="64" height="64" alt="Twitter Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/>
+<a href="https://github.com/TeamDefronix"><img src="https://github.com/gauravghongde/social-icons/raw/master/SVG/Color/Github.svg" width="64" height="64" alt="Github Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/> <a href="https://www.facebook.com/defronix"><img src="https://raw.githubusercontent.com/gauravghongde/social-icons/master/SVG/Color/Facebook.svg" width="64" height="64" alt="Facebook Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/> <a href="https://twitter.com/teamdefronix"><img src="https://github.com/gauravghongde/social-icons/raw/master/SVG/Color/Twitter.svg" width="64" height="64" alt="Twitter Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/>
+<a href="https://instagram.com/teamdefronix"><img src="https://github.com/gauravghongde/social-icons/raw/master/SVG/Color/Instagram.svg" width="64" height="64" alt="Instagram Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/>
+<a href="https://whatsapp.com/channel/0029VaGltobEKyZ8eX8Ki82w"><img src="https://github.com/gauravghongde/social-icons/raw/master/SVG/Color/WhatsApp.svg" width="64" height="64" alt="WhatsApp Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/>
+<a href="https://youtube.com/@defronix"><img src="https://github.com/gauravghongde/social-icons/raw/master/SVG/Color/Youtube.svg" width="64" height="64" alt="Youtube Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/>
+<a href="https://www.linkedin.com/company/defronix/"><img src="https://github.com/gauravghongde/social-icons/raw/master/SVG/Color/LinkedIN.svg" width="64" height="64" alt="LinkedIN Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/>
 </p>
 
 <h1 align="left">Support</h1>
 
 <p><a href="https://www.buymeacoffee.com/metaxone" target="_blank"> <img align="left" src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="50" width="210" alt="Buymeacoffee" /></a></p><br><br><br>
 <p><a href="https://paypal.me/niteshsinghhacker" target="_blank"> <img align="left" src="https://raw.githubusercontent.com/andreostrovsky/donate-with-paypal/master/blue.svg" height="70" width="210" alt="Donate with paypal" /></a></p><br><br><br>
 <p><a href="https://tools.apgy.in/upi/Nitesh+Singh/niteshkumar5@ybl/" target="_blank"> <img align="left" style="border-radius:8px" src="https://user-images.githubusercontent.com/122822828/216837693-3480fcd2-b4fc-40ff-94f8-c5d7d4b82ad5.png" height="50" width="210" alt="Donate with paypal" /></a></p><br><br><br>
```

#### html2text {}

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1 Name: cyberonix Version: 3.0.6 Summary: Cyberonix is a
+complete resource hub for Cyber Security Community. Home-page: https://
+github.com/TeamDefronix/Cyberonix Author: Defronix Author-email:
+hello@defronix.com License: MIT Classifier: Development Status :: 5 -
+Production/Stable Classifier: Intended Audience :: Developers Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Topic :: Security Description-Content-Type: text/
+markdown
                             ************ CCYYBBEERROONNIIXX ************
  [https://user-images.githubusercontent.com/122822828/216810369-34904b5a-d063-
                           48a9-a87d-11caf293243b.png]
      [https://forthebadge.com/images/badges/made-with-python.svg][https://
               forthebadge.com/images/badges/built-with-love.svg]
 
   _[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]_[_S_t_a_r_s_]_[_I_s_s_u_e_s_]_[_R_e_p_o_ _S_i_z_e_]_[_f_o_l_l_o_w_ _o_n
@@ -200,16 +212,19 @@
 www.offsec.com/courses/web-300/) - ## Bug Bounty - Bug Bounty for Beginners -
 Reconnaissance - Intel Discovery - Enumeration - Vulnerability Analysis -
 Exploitation - Reporting # Screenshots ## ![Main Menu](https://imgur.com/
 e2b26Mf.png) ## ![Bug Bounty](https://imgur.com/Sa4fdLU.png) ## ![Tools](https:
 //imgur.com/3pc76rB.png) ## ![Information Gathering](https://imgur.com/
 f1jai90.png) ![Nmap](https://imgur.com/CoYpmNC.png)
 ************ SSoocciiaallss ************
-_[_G_i_t_h_u_b_ _L_o_g_o_][assets/misc/transparent.png]_[_D_i_s_c_o_r_d_ _L_o_g_o_][assets/misc/
-transparent.png]_[_T_w_i_t_t_e_r_ _L_o_g_o_][assets/misc/transparent.png]
+_[_G_i_t_h_u_b_ _L_o_g_o_][assets/misc/transparent.png]_[_F_a_c_e_b_o_o_k_ _L_o_g_o_][assets/misc/
+transparent.png]_[_T_w_i_t_t_e_r_ _L_o_g_o_][assets/misc/transparent.png]_[_I_n_s_t_a_g_r_a_m_ _L_o_g_o_]
+[assets/misc/transparent.png]_[_W_h_a_t_s_A_p_p_ _L_o_g_o_][assets/misc/transparent.png]
+_[_Y_o_u_t_u_b_e_ _L_o_g_o_][assets/misc/transparent.png]_[_L_i_n_k_e_d_I_N_ _L_o_g_o_][assets/misc/
+transparent.png]
 ************ SSuuppppoorrtt ************
 _[_B_u_y_m_e_a_c_o_f_f_e_e_]
 
 
 
 _[_D_o_n_a_t_e_ _w_i_t_h_ _p_a_y_p_a_l_]
```

### Comparing `cyberonix-3.0.5/cyberonix/cyberonix.py` & `cyberonix-3.0.6/cyberonix/cyberonix.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/Bug_Bounty.py` & `cyberonix-3.0.6/cyberonix/main/Bug_Bounty.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/arguments.py` & `cyberonix-3.0.6/cyberonix/main/arguments.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tool.py` & `cyberonix-3.0.6/cyberonix/main/tool.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/Anonymity.py` & `cyberonix-3.0.6/cyberonix/main/tools/Anonymity.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/Authentication.py` & `cyberonix-3.0.6/cyberonix/main/tools/Authentication.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/Authorization.py` & `cyberonix-3.0.6/cyberonix/main/tools/Authorization.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/Configuration_Management.py` & `cyberonix-3.0.6/cyberonix/main/tools/Configuration_Management.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/Cryptography.py` & `cyberonix-3.0.6/cyberonix/main/tools/Cryptography.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/Exploitation_Tools.py` & `cyberonix-3.0.6/cyberonix/main/tools/Exploitation_Tools.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/File_Upload.py` & `cyberonix-3.0.6/cyberonix/main/tools/File_Upload.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/Password_Hacking.py` & `cyberonix-3.0.6/cyberonix/main/tools/Password_Hacking.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/Pentesting_Bug_Bounty.py` & `cyberonix-3.0.6/cyberonix/main/tools/Pentesting_Bug_Bounty.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/PostExploitationAttacks.py` & `cyberonix-3.0.6/cyberonix/main/tools/PostExploitationAttacks.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/Recommended_Tool.py` & `cyberonix-3.0.6/cyberonix/main/tools/Recommended_Tool.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/RiskyFuncPayment.py` & `cyberonix-3.0.6/cyberonix/main/tools/RiskyFuncPayment.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/Secure_Transmission.py` & `cyberonix-3.0.6/cyberonix/main/tools/Secure_Transmission.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/Session_Management.py` & `cyberonix-3.0.6/cyberonix/main/tools/Session_Management.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/Sniffing_and_Spoofing.py` & `cyberonix-3.0.6/cyberonix/main/tools/Sniffing_and_Spoofing.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/Vulnerability_Analysis.py` & `cyberonix-3.0.6/cyberonix/main/tools/Vulnerability_Analysis.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/WEB_Application_Analysis.py` & `cyberonix-3.0.6/cyberonix/main/tools/WEB_Application_Analysis.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/Wireless_Hacking.py` & `cyberonix-3.0.6/cyberonix/main/tools/Wireless_Hacking.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/banner.py` & `cyberonix-3.0.6/cyberonix/main/tools/banner.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/data_validation.py` & `cyberonix-3.0.6/cyberonix/main/tools/data_validation.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/dos.py` & `cyberonix-3.0.6/cyberonix/main/tools/dos.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/forensic.py` & `cyberonix-3.0.6/cyberonix/main/tools/forensic.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/html5.py` & `cyberonix-3.0.6/cyberonix/main/tools/html5.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/information_gathering.py` & `cyberonix-3.0.6/cyberonix/main/tools/information_gathering.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/run_on_browser.py` & `cyberonix-3.0.6/cyberonix/main/tools/run_on_browser.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/template.py` & `cyberonix-3.0.6/cyberonix/main/tools/template.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix/main/tools/writeup.py` & `cyberonix-3.0.6/cyberonix/main/tools/writeup.py`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/cyberonix.egg-info/PKG-INFO` & `cyberonix-3.0.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: cyberonix
-Version: 3.0.5
-Summary: Cyberonix is a complete resource hub for Cyber Security Community.
-Home-page: https://github.com/TeamDefronix/Cyberonix
-Author: Defronix
-Author-email: hello@defronix.com
-License: MIT
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: Security
-Description-Content-Type: text/markdown
-
 <div align="center"><p>
     <h1>CYBERONIX</h1>
     <img style="filter: brightness(200%)" src="https://user-images.githubusercontent.com/122822828/216810369-34904b5a-d063-48a9-a87d-11caf293243b.png" width="50%"><br>
     <img src="https://forthebadge.com/images/badges/made-with-python.svg">
     <img src="https://forthebadge.com/images/badges/built-with-love.svg">
     <br><br>
     <a href="https://github.com/TeamDefronix/Cyberonix/releases/latest">
@@ -527,15 +506,19 @@
 ## ![Information Gathering](https://imgur.com/f1jai90.png)
 
 ![Nmap](https://imgur.com/CoYpmNC.png)
 
 <h1 align="left">Socials</h1>
 
 <p align="left">
-<a href="https://github.com/TeamDefronix"><img src="https://user-images.githubusercontent.com/696094/196835284-c52d4bd1-7034-439e-848b-47d4f2933dff.svg" width="64" height="64" alt="Github Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/> <a href="https://discord.gg/defronix"><img src="https://user-images.githubusercontent.com/696094/196835282-f5c47d66-29b7-4210-9ee0-d9cdecde3559.svg" width="64" height="64" alt="Discord Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/> <a href="https://twitter.com/niteshlike123"><img src="https://user-images.githubusercontent.com/696094/196835281-52617611-ede6-40da-a4bc-8c5025622bbf.svg" width="64" height="64" alt="Twitter Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/>
+<a href="https://github.com/TeamDefronix"><img src="https://github.com/gauravghongde/social-icons/raw/master/SVG/Color/Github.svg" width="64" height="64" alt="Github Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/> <a href="https://www.facebook.com/defronix"><img src="https://raw.githubusercontent.com/gauravghongde/social-icons/master/SVG/Color/Facebook.svg" width="64" height="64" alt="Facebook Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/> <a href="https://twitter.com/teamdefronix"><img src="https://github.com/gauravghongde/social-icons/raw/master/SVG/Color/Twitter.svg" width="64" height="64" alt="Twitter Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/>
+<a href="https://instagram.com/teamdefronix"><img src="https://github.com/gauravghongde/social-icons/raw/master/SVG/Color/Instagram.svg" width="64" height="64" alt="Instagram Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/>
+<a href="https://whatsapp.com/channel/0029VaGltobEKyZ8eX8Ki82w"><img src="https://github.com/gauravghongde/social-icons/raw/master/SVG/Color/WhatsApp.svg" width="64" height="64" alt="WhatsApp Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/>
+<a href="https://youtube.com/@defronix"><img src="https://github.com/gauravghongde/social-icons/raw/master/SVG/Color/Youtube.svg" width="64" height="64" alt="Youtube Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/>
+<a href="https://www.linkedin.com/company/defronix/"><img src="https://github.com/gauravghongde/social-icons/raw/master/SVG/Color/LinkedIN.svg" width="64" height="64" alt="LinkedIN Logo"/></a> <img src="assets/misc/transparent.png" height="1" width="5"/>
 </p>
 
 <h1 align="left">Support</h1>
 
 <p><a href="https://www.buymeacoffee.com/metaxone" target="_blank"> <img align="left" src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" height="50" width="210" alt="Buymeacoffee" /></a></p><br><br><br>
 <p><a href="https://paypal.me/niteshsinghhacker" target="_blank"> <img align="left" src="https://raw.githubusercontent.com/andreostrovsky/donate-with-paypal/master/blue.svg" height="70" width="210" alt="Donate with paypal" /></a></p><br><br><br>
 <p><a href="https://tools.apgy.in/upi/Nitesh+Singh/niteshkumar5@ybl/" target="_blank"> <img align="left" style="border-radius:8px" src="https://user-images.githubusercontent.com/122822828/216837693-3480fcd2-b4fc-40ff-94f8-c5d7d4b82ad5.png" height="50" width="210" alt="Donate with paypal" /></a></p><br><br><br>
```

#### html2text {}

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1 Name: cyberonix Version: 3.0.5 Summary: Cyberonix is a
-complete resource hub for Cyber Security Community. Home-page: https://
-github.com/TeamDefronix/Cyberonix Author: Defronix Author-email:
-hello@defronix.com License: MIT Classifier: Development Status :: 5 -
-Production/Stable Classifier: Intended Audience :: Developers Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python :: 3 Classifier:
-Programming Language :: Python :: 3.6 Classifier: Programming Language ::
-Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
-Programming Language :: Python :: 3.9 Classifier: Programming Language ::
-Python :: 3.10 Classifier: Topic :: Security Description-Content-Type: text/
-markdown
                             ************ CCYYBBEERROONNIIXX ************
  [https://user-images.githubusercontent.com/122822828/216810369-34904b5a-d063-
                           48a9-a87d-11caf293243b.png]
      [https://forthebadge.com/images/badges/made-with-python.svg][https://
               forthebadge.com/images/badges/built-with-love.svg]
 
   _[_L_a_t_e_s_t_ _r_e_l_e_a_s_e_]_[_L_a_s_t_ _c_o_m_m_i_t_]_[_L_i_c_e_n_s_e_]_[_S_t_a_r_s_]_[_I_s_s_u_e_s_]_[_R_e_p_o_ _S_i_z_e_]_[_f_o_l_l_o_w_ _o_n
@@ -212,16 +200,19 @@
 www.offsec.com/courses/web-300/) - ## Bug Bounty - Bug Bounty for Beginners -
 Reconnaissance - Intel Discovery - Enumeration - Vulnerability Analysis -
 Exploitation - Reporting # Screenshots ## ![Main Menu](https://imgur.com/
 e2b26Mf.png) ## ![Bug Bounty](https://imgur.com/Sa4fdLU.png) ## ![Tools](https:
 //imgur.com/3pc76rB.png) ## ![Information Gathering](https://imgur.com/
 f1jai90.png) ![Nmap](https://imgur.com/CoYpmNC.png)
 ************ SSoocciiaallss ************
-_[_G_i_t_h_u_b_ _L_o_g_o_][assets/misc/transparent.png]_[_D_i_s_c_o_r_d_ _L_o_g_o_][assets/misc/
-transparent.png]_[_T_w_i_t_t_e_r_ _L_o_g_o_][assets/misc/transparent.png]
+_[_G_i_t_h_u_b_ _L_o_g_o_][assets/misc/transparent.png]_[_F_a_c_e_b_o_o_k_ _L_o_g_o_][assets/misc/
+transparent.png]_[_T_w_i_t_t_e_r_ _L_o_g_o_][assets/misc/transparent.png]_[_I_n_s_t_a_g_r_a_m_ _L_o_g_o_]
+[assets/misc/transparent.png]_[_W_h_a_t_s_A_p_p_ _L_o_g_o_][assets/misc/transparent.png]
+_[_Y_o_u_t_u_b_e_ _L_o_g_o_][assets/misc/transparent.png]_[_L_i_n_k_e_d_I_N_ _L_o_g_o_][assets/misc/
+transparent.png]
 ************ SSuuppppoorrtt ************
 _[_B_u_y_m_e_a_c_o_f_f_e_e_]
 
 
 
 _[_D_o_n_a_t_e_ _w_i_t_h_ _p_a_y_p_a_l_]
```

### Comparing `cyberonix-3.0.5/cyberonix.egg-info/SOURCES.txt` & `cyberonix-3.0.6/cyberonix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberonix-3.0.5/setup.py` & `cyberonix-3.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup,find_packages 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="cyberonix",
-    version="3.0.5",
+    version="3.0.6",
     author="Defronix",
     author_email="hello@defronix.com",
     description="Cyberonix is a complete resource hub for Cyber Security Community.",
     url='https://github.com/TeamDefronix/Cyberonix',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='MIT',
```

