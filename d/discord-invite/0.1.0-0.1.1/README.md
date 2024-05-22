# Comparing `tmp/discord_invite-0.1.0.tar.gz` & `tmp/discord_invite-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord_invite-0.1.0.tar", last modified: Wed May 22 11:49:39 2024, max compression
+gzip compressed data, was "discord_invite-0.1.1.tar", last modified: Wed May 22 11:57:08 2024, max compression
```

## Comparing `discord_invite-0.1.0.tar` & `discord_invite-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 11:49:39.540806 discord_invite-0.1.0/
--rw-rw-rw-   0        0        0      632 2024-05-22 11:49:39.540806 discord_invite-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      203 2024-05-22 11:47:32.000000 discord_invite-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 11:49:39.539806 discord_invite-0.1.0/discord_invite.egg-info/
--rw-rw-rw-   0        0        0      632 2024-05-22 11:49:39.000000 discord_invite-0.1.0/discord_invite.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      207 2024-05-22 11:49:39.000000 discord_invite-0.1.0/discord_invite.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 11:49:39.000000 discord_invite-0.1.0/discord_invite.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-05-22 11:49:39.000000 discord_invite-0.1.0/discord_invite.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 11:49:39.000000 discord_invite-0.1.0/discord_invite.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 11:49:39.540806 discord_invite-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      669 2024-05-22 11:48:25.000000 discord_invite-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:57:08.608170 discord_invite-0.1.1/
+-rw-rw-rw-   0        0        0      608 2024-05-22 11:57:08.607170 discord_invite-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      179 2024-05-22 11:55:50.000000 discord_invite-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 11:57:08.607170 discord_invite-0.1.1/discord_invite.egg-info/
+-rw-rw-rw-   0        0        0      608 2024-05-22 11:57:08.000000 discord_invite-0.1.1/discord_invite.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      207 2024-05-22 11:57:08.000000 discord_invite-0.1.1/discord_invite.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 11:57:08.000000 discord_invite-0.1.1/discord_invite.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-05-22 11:57:08.000000 discord_invite-0.1.1/discord_invite.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 11:57:08.000000 discord_invite-0.1.1/discord_invite.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 11:57:08.608170 discord_invite-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      669 2024-05-22 11:55:27.000000 discord_invite-0.1.1/setup.py
```

### Comparing `discord_invite-0.1.0/PKG-INFO` & `discord_invite-0.1.1/discord_invite.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
-Name: discord_invite
-Version: 0.1.0
+Name: discord-invite
+Version: 0.1.1
 Summary: A python of discord joiner
 Home-page: https://github.com/LaciaHax/discord_joiner
 Author: Lacia Hax
 Author-email: yuitanmiruku@outlook.jp
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 discord joiner lib
 
 usage
 ```
-from discord_invite import create_tls_session
+from discord_invite import joiner
 
 token = 'YOUR_DISCORD_TOKEN'
 invite = 'INVITE_CODE'
-response = create_tls_session(token, invite)
+response = joiner(token, invite)
 print(response)
 ```
```

### Comparing `discord_invite-0.1.0/setup.py` & `discord_invite-0.1.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='discord_invite',
-    version='0.1.0',
+    version='0.1.1',
     packages=find_packages(),
     install_requires=[
         'tls-client',
     ],
     author='Lacia Hax',
     author_email='yuitanmiruku@outlook.jp',
     description='A python of discord joiner',
```

