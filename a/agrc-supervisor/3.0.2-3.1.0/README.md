# Comparing `tmp/agrc-supervisor-3.0.2.tar.gz` & `tmp/agrc-supervisor-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agrc-supervisor-3.0.2.tar", last modified: Thu Feb 23 18:55:02 2023, max compression
+gzip compressed data, was "agrc-supervisor-3.1.0.tar", last modified: Wed May 22 19:06:16 2024, max compression
```

## Comparing `agrc-supervisor-3.0.2.tar` & `agrc-supervisor-3.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:55:02.809129 agrc-supervisor-3.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-02-23 18:54:59.000000 agrc-supervisor-3.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-23 18:55:02.809129 agrc-supervisor-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-02-23 18:54:59.000000 agrc-supervisor-3.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-23 18:55:02.809129 agrc-supervisor-3.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-02-23 18:54:59.000000 agrc-supervisor-3.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:55:02.805128 agrc-supervisor-3.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:55:02.809129 agrc-supervisor-3.0.2/src/agrc_supervisor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-02-23 18:55:02.000000 agrc-supervisor-3.0.2/src/agrc_supervisor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-02-23 18:55:02.000000 agrc-supervisor-3.0.2/src/agrc_supervisor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 18:55:02.000000 agrc-supervisor-3.0.2/src/agrc_supervisor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-02-23 18:55:02.000000 agrc-supervisor-3.0.2/src/agrc_supervisor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-02-23 18:55:02.000000 agrc-supervisor-3.0.2/src/agrc_supervisor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 18:55:02.000000 agrc-supervisor-3.0.2/src/agrc_supervisor.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 18:55:02.809129 agrc-supervisor-3.0.2/src/supervisor/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-02-23 18:54:59.000000 agrc-supervisor-3.0.2/src/supervisor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-02-23 18:54:59.000000 agrc-supervisor-3.0.2/src/supervisor/example.py
--rw-r--r--   0 runner    (1001) docker     (123)    15812 2023-02-23 18:54:59.000000 agrc-supervisor-3.0.2/src/supervisor/message_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-02-23 18:54:59.000000 agrc-supervisor-3.0.2/src/supervisor/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-23 18:55:00.000000 agrc-supervisor-3.0.2/src/supervisor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:06:16.848972 agrc-supervisor-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-22 19:06:13.000000 agrc-supervisor-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-22 19:06:16.848972 agrc-supervisor-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-05-22 19:06:13.000000 agrc-supervisor-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-05-22 19:06:16.848972 agrc-supervisor-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-22 19:06:13.000000 agrc-supervisor-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:06:16.844972 agrc-supervisor-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:06:16.848972 agrc-supervisor-3.1.0/src/agrc_supervisor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-05-22 19:06:16.000000 agrc-supervisor-3.1.0/src/agrc_supervisor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-05-22 19:06:16.000000 agrc-supervisor-3.1.0/src/agrc_supervisor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:06:16.000000 agrc-supervisor-3.1.0/src/agrc_supervisor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-22 19:06:16.000000 agrc-supervisor-3.1.0/src/agrc_supervisor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 19:06:16.000000 agrc-supervisor-3.1.0/src/agrc_supervisor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 19:06:16.000000 agrc-supervisor-3.1.0/src/agrc_supervisor.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 19:06:16.848972 agrc-supervisor-3.1.0/src/supervisor/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-22 19:06:13.000000 agrc-supervisor-3.1.0/src/supervisor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-05-22 19:06:13.000000 agrc-supervisor-3.1.0/src/supervisor/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15841 2024-05-22 19:06:13.000000 agrc-supervisor-3.1.0/src/supervisor/message_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-22 19:06:13.000000 agrc-supervisor-3.1.0/src/supervisor/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-22 19:06:13.000000 agrc-supervisor-3.1.0/src/supervisor/version.py
```

### Comparing `agrc-supervisor-3.0.2/LICENSE` & `agrc-supervisor-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `agrc-supervisor-3.0.2/PKG-INFO` & `agrc-supervisor-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: agrc-supervisor
-Version: 3.0.2
+Version: 3.1.0
 Summary: A watchdog module for scheduled scripts that sends notifications, including any uncaught exceptions.
 Home-page: https://github.com/agrc/supervisor
-Author: Jake Adams, AGRC
+Author: Jake Adams, UGRC
 Author-email: jdadams@utah.gov
 License: MIT
 Project-URL: Issue Tracker, https://github.com/agrc/supervisor/issues
 Keywords: gis
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `agrc-supervisor-3.0.2/README.md` & `agrc-supervisor-3.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# agrc/python
+# Supervisor
 
-![Build Status](https://github.com/agrc/supervisor/workflows/Build%20and%20Test/badge.svg)
-<!-- [![codecov](https://codecov.io/gh/agrc/python/branch/main/graph/badge.svg)](https://codecov.io/gh/agrc/python) -->
+[![Push Events](https://github.com/agrc/supervisor/actions/workflows/push.yml/badge.svg)](https://github.com/agrc/supervisor/actions/workflows/push.yml)
+[![codecov](https://codecov.io/gh/agrc/supervisor/branch/main/graph/badge.svg)](https://codecov.io/gh/agrc/supervisor)
 
 A module for watching over scheduled processes: catching errors and sending messages for errors and/or summary logs.
 
 ## Rationale
 
 supervisor provides a framework for scripts scheduled through Windows' Task Scheduler to send messages via the handlers in `message_handlers.py`. The messages can include gziped log files, progress reports, or execution summaries. The message handlers provide access to channels not supported by Task Scheduler like email, slack, and any other custom handler. It also can send any uncaught exceptions via the registered message handlers if desired.
```

### Comparing `agrc-supervisor-3.0.2/setup.cfg` & `agrc-supervisor-3.1.0/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -14,13 +14,13 @@
 
 [tool:pytest]
 testpaths = tests src
 norecursedirs = .env data maps
 show_capture = True
 minversion = 3.5
 console_output_style = count
-addopts = --pylint --cov-branch --cov=supervisor --cov-report term --cov-report xml:cov.xml --instafail
+addopts = --cov-branch --cov=supervisor --cov-report term --cov-report xml:cov.xml --instafail
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `agrc-supervisor-3.0.2/setup.py` & `agrc-supervisor-3.1.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     exec(fp.read(), version)
 
 setup(
     name='agrc-supervisor',
     version=version['__version__'],
     license='MIT',
     description='A watchdog module for scheduled scripts that sends notifications, including any uncaught exceptions.',
-    author='Jake Adams, AGRC',
+    author='Jake Adams, UGRC',
     author_email='jdadams@utah.gov',
     url='https://github.com/agrc/supervisor',
     packages=find_packages('src'),
     package_dir={'': 'src'},
     py_modules=[splitext(basename(path))[0] for path in glob('src/*.py')],
     include_package_data=True,
     zip_safe=True,
@@ -33,28 +33,28 @@
         'Topic :: Utilities',
     ],
     project_urls={
         'Issue Tracker': 'https://github.com/agrc/supervisor/issues',
     },
     keywords=['gis'],
     install_requires=[
-        'requests==2.28.*',
-        'sendgrid==6.9.*',
+        'requests~=2.32',
+        'sendgrid~=6.11',
     ],
     extras_require={
         'tests': [
-            'pylint-quotes==0.2.*',
-            'pylint==2.16.*',
-            'pytest-cov==4.*',
-            'pytest-instafail==0.4.*',
-            'pytest-isort==3.1.*',
-            'pytest-mock==3.10.*',
-            'pytest-pylint==0.19.*',
-            'pytest-watch==4.2.*',
-            'pytest==7.2.*',
-            'yapf==0.32.*',
+            'pylint-quotes~=0.2',
+            'pylint>=2.17,<4.0',
+            'pytest-cov>=4.1,<6.0',
+            'pytest-instafail~=0.5',
+            'pytest-isort>=3.1,<5.0',
+            'pytest-mock~=3.11',
+            # 'pytest-pylint~=0.19',  #: Causes pytest to fail
+            'pytest-watch~=4.2',
+            'pytest>=7.4,<9.0',
+            'yapf~=0.40',
         ]
     },
     setup_requires=[
         'pytest-runner',
     ],
 )
```

### Comparing `agrc-supervisor-3.0.2/src/agrc_supervisor.egg-info/PKG-INFO` & `agrc-supervisor-3.1.0/src/agrc_supervisor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: agrc-supervisor
-Version: 3.0.2
+Version: 3.1.0
 Summary: A watchdog module for scheduled scripts that sends notifications, including any uncaught exceptions.
 Home-page: https://github.com/agrc/supervisor
-Author: Jake Adams, AGRC
+Author: Jake Adams, UGRC
 Author-email: jdadams@utah.gov
 License: MIT
 Project-URL: Issue Tracker, https://github.com/agrc/supervisor/issues
 Keywords: gis
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `agrc-supervisor-3.0.2/src/supervisor/example.py` & `agrc-supervisor-3.1.0/src/supervisor/example.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 import datetime
 import logging
 import logging.handlers
 import socket
 from pathlib import Path
 
 from supervisor import secrets
-from supervisor.message_handlers import EmailHandler, SendGridHandler
+from supervisor.message_handlers import SendGridHandler
 from supervisor.models import MessageDetails, Supervisor
 
 if __name__ == '__main__':
 
     #: Set up a rotating file handler for the report log
     test_path = Path(r'd:\temp\supervisor_log.txt')
     test_logger = logging.getLogger('supervisor')
     test_handler = logging.handlers.RotatingFileHandler(test_path, backupCount=2)
     test_handler.doRollover()  #: Rotate the log on each run
     test_handler.setLevel(logging.DEBUG)
     test_logger.addHandler(test_handler)
     test_logger.setLevel(logging.DEBUG)
 
-    #: Add somethign to the log
+    #: Add something to the log
     test_logger.info(f'test run: {datetime.datetime.now()}')
 
     #: Instantiate a Supervisor object
     sim_sup = Supervisor(logger=test_logger, log_path=test_path)
 
     #: ============
     #: EmailHandler
```

### Comparing `agrc-supervisor-3.0.2/src/supervisor/message_handlers.py` & `agrc-supervisor-3.1.0/src/supervisor/message_handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         self.client_version = client_version
 
     def send_message(self, message_details):
         """Build a message, create an SMTP object, and send the message
 
         Parameters
         ----------
-        mesage_details : MessageDetails
+        message_details : MessageDetails
             Passed through to _build_message. Must have .message, .subject; may have .attachments
         """
 
         #: Configure outgoing settings
         try:
             from_address = self.email_settings['from_address']
             to_addresses = self.email_settings['to_addresses']
@@ -98,15 +98,15 @@
             smtp.sendmail(from_address, to_addresses, message.as_string())
 
     def _build_message(self, message_details):
         """Create email to be sent as a MIMEMultipart object
 
         Parameters
         ----------
-        mesage_details : MessageDetails
+        message_details : MessageDetails
             Must have .message, .subject; may have .attachments
 
         Returns
         -------
         message : MIMEMultipart
             A formatted message that can be passed to smtp.sendmail as message.as_string()
         """
@@ -368,15 +368,17 @@
 
         Returns:
             str: Path to the new zipfile
         """
 
         attachment_dir = Path(dir_to_be_zipped)
         zip_base_name = Path(working_dir, attachment_dir.name)
-        zip_out_path = make_archive(zip_base_name, 'zip', root_dir=attachment_dir.parent, base_dir=attachment_dir.name)
+        zip_out_path = make_archive(
+            str(zip_base_name), 'zip', root_dir=attachment_dir.parent, base_dir=attachment_dir.name
+        )
         return zip_out_path
 
     @staticmethod
     def _zip_single_file(working_dir, attachment):
         """Create a zipfile containing a single file
 
         Args:
```

### Comparing `agrc-supervisor-3.0.2/src/supervisor/models.py` & `agrc-supervisor-3.1.0/src/supervisor/models.py`

 * *Files identical despite different names*

