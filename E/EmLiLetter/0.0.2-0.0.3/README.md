# Comparing `tmp/EmLiLetter-0.0.2.tar.gz` & `tmp/EmLiLetter-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "EmLiLetter-0.0.2.tar", last modified: Sun May 19 16:45:18 2024, max compression
+gzip compressed data, was "EmLiLetter-0.0.3.tar", last modified: Wed May 22 12:38:11 2024, max compression
```

## Comparing `EmLiLetter-0.0.2.tar` & `EmLiLetter-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 bridgearchitect  (1000) bridgearchitect  (1000)        0 2024-05-19 16:45:18.762411 EmLiLetter-0.0.2/
-drwxr-xr-x   0 bridgearchitect  (1000) bridgearchitect  (1000)        0 2024-05-19 16:45:18.760411 EmLiLetter-0.0.2/EmLiLetter.egg-info/
--rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)      220 2024-05-19 16:45:18.000000 EmLiLetter-0.0.2/EmLiLetter.egg-info/PKG-INFO
--rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)      339 2024-05-19 16:45:18.000000 EmLiLetter-0.0.2/EmLiLetter.egg-info/SOURCES.txt
--rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)        1 2024-05-19 16:45:18.000000 EmLiLetter-0.0.2/EmLiLetter.egg-info/dependency_links.txt
--rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)       40 2024-05-19 16:45:18.000000 EmLiLetter-0.0.2/EmLiLetter.egg-info/entry_points.txt
--rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)       10 2024-05-19 16:45:18.000000 EmLiLetter-0.0.2/EmLiLetter.egg-info/requires.txt
--rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)        5 2024-05-19 16:45:18.000000 EmLiLetter-0.0.2/EmLiLetter.egg-info/top_level.txt
--rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)     1058 2024-02-05 20:36:55.000000 EmLiLetter-0.0.2/LICENSE.txt
--rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)      220 2024-05-19 16:45:18.762411 EmLiLetter-0.0.2/PKG-INFO
--rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)     1862 2024-05-19 16:23:03.000000 EmLiLetter-0.0.2/README.md
-drwxr-xr-x   0 bridgearchitect  (1000) bridgearchitect  (1000)        0 2024-05-19 16:45:18.761411 EmLiLetter-0.0.2/emli/
--rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)      253 2024-05-13 16:47:24.000000 EmLiLetter-0.0.2/emli/__init__.py
--rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)     3179 2024-05-08 13:22:52.000000 EmLiLetter-0.0.2/emli/alltypes.py
--rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)     5963 2024-05-08 11:02:58.000000 EmLiLetter-0.0.2/emli/emli.glade
--rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)     2721 2024-05-19 16:13:36.000000 EmLiLetter-0.0.2/emli/emli.py
--rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)     7222 2024-05-13 16:55:19.000000 EmLiLetter-0.0.2/emli/gui.py
--rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)     2735 2024-05-13 16:56:12.000000 EmLiLetter-0.0.2/emli/mail.py
--rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)    10878 2024-05-13 16:42:58.000000 EmLiLetter-0.0.2/emli/reader.py
--rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)       38 2024-05-19 16:45:18.762411 EmLiLetter-0.0.2/setup.cfg
--rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)      672 2024-05-19 16:45:08.000000 EmLiLetter-0.0.2/setup.py
+drwxr-xr-x   0 bridgearchitect  (1000) bridgearchitect  (1000)        0 2024-05-22 12:38:11.759698 EmLiLetter-0.0.3/
+drwxr-xr-x   0 bridgearchitect  (1000) bridgearchitect  (1000)        0 2024-05-22 12:38:11.757698 EmLiLetter-0.0.3/EmLiLetter.egg-info/
+-rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)      220 2024-05-22 12:38:11.000000 EmLiLetter-0.0.3/EmLiLetter.egg-info/PKG-INFO
+-rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)      339 2024-05-22 12:38:11.000000 EmLiLetter-0.0.3/EmLiLetter.egg-info/SOURCES.txt
+-rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)        1 2024-05-22 12:38:11.000000 EmLiLetter-0.0.3/EmLiLetter.egg-info/dependency_links.txt
+-rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)       40 2024-05-22 12:38:11.000000 EmLiLetter-0.0.3/EmLiLetter.egg-info/entry_points.txt
+-rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)       10 2024-05-22 12:38:11.000000 EmLiLetter-0.0.3/EmLiLetter.egg-info/requires.txt
+-rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)        5 2024-05-22 12:38:11.000000 EmLiLetter-0.0.3/EmLiLetter.egg-info/top_level.txt
+-rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)     1058 2024-02-05 20:36:55.000000 EmLiLetter-0.0.3/LICENSE.txt
+-rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)      220 2024-05-22 12:38:11.758699 EmLiLetter-0.0.3/PKG-INFO
+-rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)     1862 2024-05-19 16:23:03.000000 EmLiLetter-0.0.3/README.md
+drwxr-xr-x   0 bridgearchitect  (1000) bridgearchitect  (1000)        0 2024-05-22 12:38:11.758699 EmLiLetter-0.0.3/emli/
+-rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)      253 2024-05-13 16:47:24.000000 EmLiLetter-0.0.3/emli/__init__.py
+-rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)     3179 2024-05-08 13:22:52.000000 EmLiLetter-0.0.3/emli/alltypes.py
+-rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)     5963 2024-05-08 11:02:58.000000 EmLiLetter-0.0.3/emli/emli.glade
+-rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)     2721 2024-05-19 16:13:36.000000 EmLiLetter-0.0.3/emli/emli.py
+-rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)     7218 2024-05-22 12:30:05.000000 EmLiLetter-0.0.3/emli/gui.py
+-rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)     2735 2024-05-13 16:56:12.000000 EmLiLetter-0.0.3/emli/mail.py
+-rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)    10878 2024-05-22 12:29:05.000000 EmLiLetter-0.0.3/emli/reader.py
+-rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)       38 2024-05-22 12:38:11.759698 EmLiLetter-0.0.3/setup.cfg
+-rw-r--r--   0 bridgearchitect  (1000) bridgearchitect  (1000)      672 2024-05-22 12:35:09.000000 EmLiLetter-0.0.3/setup.py
```

### Comparing `EmLiLetter-0.0.2/LICENSE.txt` & `EmLiLetter-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `EmLiLetter-0.0.2/README.md` & `EmLiLetter-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `EmLiLetter-0.0.2/emli/alltypes.py` & `EmLiLetter-0.0.3/emli/alltypes.py`

 * *Files identical despite different names*

### Comparing `EmLiLetter-0.0.2/emli/emli.glade` & `EmLiLetter-0.0.3/emli/emli.glade`

 * *Files identical despite different names*

### Comparing `EmLiLetter-0.0.2/emli/emli.py` & `EmLiLetter-0.0.3/emli/emli.py`

 * *Files identical despite different names*

### Comparing `EmLiLetter-0.0.2/emli/gui.py` & `EmLiLetter-0.0.3/emli/gui.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     while index < numMails:
         # extract data from arrays
         recipientEmail = recipientEmails[index]
         name = names[index]
         title = titles[index]
         try:
             # send one mail to end user seperatly
-            emli.sendMail(senderEmail, recipientEmail, smtpServer, username, appPassword, subject, title, name, bodyHTML, filenamesAttach, alltypes.smtpPort)
+            emli.sendMail(senderEmail, recipientEmail, smtpServer, username, appPassword, subject, title, name, bodyHTML, filenamesAttach, emli.smtpPort)
         except Exception as error:
             # handle exception situation
             errorLabel.set_text(str(error))
             # finish working
             return
         # go to the next mail box
         index = index + 1
```

### Comparing `EmLiLetter-0.0.2/emli/mail.py` & `EmLiLetter-0.0.3/emli/mail.py`

 * *Files identical despite different names*

### Comparing `EmLiLetter-0.0.2/emli/reader.py` & `EmLiLetter-0.0.3/emli/reader.py`

 * *Files identical despite different names*

### Comparing `EmLiLetter-0.0.2/setup.py` & `EmLiLetter-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 # define constants for working
 NAME = 'EmLiLetter'
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'EmLi software to send mails for several users'
 AUTHOR = 'Artem Tomilo'
 REQUIRED = ['pygobject']
 URL = 'https://gitlab.com/bridgearchitect/emli'
 LICENSE = 'MIT'
 PACKAGES = ['emli']
 PACKAGE_DATA = 'emli.glade'
```

