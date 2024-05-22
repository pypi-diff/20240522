# Comparing `tmp/credsmash-2.3.1.tar.gz` & `tmp/credsmash-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/credsmash-2.3.1.tar", last modified: Wed Mar 13 06:04:35 2019, max compression
+gzip compressed data, was "credsmash-3.0.0.tar", last modified: Wed May 22 03:02:59 2024, max compression
```

## Comparing `credsmash-2.3.1.tar` & `credsmash-3.0.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 06:04:35.000000 credsmash-2.3.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15657 2019-03-13 06:03:59.000000 credsmash-2.3.1/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 06:04:35.000000 credsmash-2.3.1/credsmash/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 06:04:35.000000 credsmash-2.3.1/credsmash/crypto/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5215 2019-03-13 06:03:59.000000 credsmash-2.3.1/credsmash/crypto/aes_ctr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1569 2019-03-13 06:03:59.000000 credsmash-2.3.1/credsmash/crypto/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1982 2019-03-13 06:03:59.000000 credsmash-2.3.1/credsmash/crypto/aes_gcm.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      708 2019-03-13 06:03:59.000000 credsmash-2.3.1/credsmash/cli_dynamodb.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12955 2019-03-13 06:03:59.000000 credsmash-2.3.1/credsmash/cli.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      686 2019-03-13 06:03:59.000000 credsmash-2.3.1/credsmash/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 06:04:35.000000 credsmash-2.3.1/credsmash/api/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1183 2019-03-13 06:03:59.000000 credsmash-2.3.1/credsmash/api/put.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      776 2019-03-13 06:03:59.000000 credsmash-2.3.1/credsmash/api/prune.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      238 2019-03-13 06:03:59.000000 credsmash-2.3.1/credsmash/api/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      592 2019-03-13 06:03:59.000000 credsmash-2.3.1/credsmash/api/delete.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      491 2019-03-13 06:03:59.000000 credsmash-2.3.1/credsmash/api/get.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      158 2019-03-13 06:03:59.000000 credsmash-2.3.1/credsmash/api/list.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2118 2019-03-13 06:03:59.000000 credsmash-2.3.1/credsmash/kms_key_service.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8699 2019-03-13 06:03:59.000000 credsmash-2.3.1/credsmash/templates.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        6 2019-03-13 06:03:59.000000 credsmash-2.3.1/credsmash/VERSION
--rw-rw-r--   0 travis    (2000) travis    (2000)     7088 2019-03-13 06:03:59.000000 credsmash-2.3.1/credsmash/util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5692 2019-03-13 06:03:59.000000 credsmash-2.3.1/credsmash/dynamodb_storage_service.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2222 2019-03-13 06:03:59.000000 credsmash-2.3.1/setup.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      132 2019-03-13 06:04:35.000000 credsmash-2.3.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)    18981 2019-03-13 06:04:35.000000 credsmash-2.3.1/PKG-INFO
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-03-13 06:04:35.000000 credsmash-2.3.1/credsmash.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)       10 2019-03-13 06:04:35.000000 credsmash-2.3.1/credsmash.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      109 2019-03-13 06:04:35.000000 credsmash-2.3.1/credsmash.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    18981 2019-03-13 06:04:35.000000 credsmash-2.3.1/credsmash.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-03-13 06:04:35.000000 credsmash-2.3.1/credsmash.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      302 2019-03-13 06:04:35.000000 credsmash-2.3.1/credsmash.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      641 2019-03-13 06:04:35.000000 credsmash-2.3.1/credsmash.egg-info/SOURCES.txt
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-22 03:02:59.482098 credsmash-3.0.0/
+-rw-r--r--   0 nathan    (1000) nathan    (1000)    11358 2018-05-16 01:54:08.000000 credsmash-3.0.0/LICENSE
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    16631 2024-05-22 03:02:59.482098 credsmash-3.0.0/PKG-INFO
+-rw-r--r--   0 nathan    (1000) nathan    (1000)    15657 2018-05-16 01:54:08.000000 credsmash-3.0.0/README.md
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-22 03:02:59.482098 credsmash-3.0.0/credsmash/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)        6 2024-05-22 03:02:35.000000 credsmash-3.0.0/credsmash/VERSION
+-rwxrwxr-x   0 nathan    (1000) nathan    (1000)      734 2024-05-22 02:32:09.000000 credsmash-3.0.0/credsmash/__init__.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-22 03:02:59.482098 credsmash-3.0.0/credsmash/api/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      238 2019-03-13 05:47:16.000000 credsmash-3.0.0/credsmash/api/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      592 2019-03-13 05:47:16.000000 credsmash-3.0.0/credsmash/api/delete.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      491 2019-03-13 05:47:16.000000 credsmash-3.0.0/credsmash/api/get.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      158 2019-03-13 05:47:16.000000 credsmash-3.0.0/credsmash/api/list.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      776 2019-03-13 05:47:16.000000 credsmash-3.0.0/credsmash/api/prune.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1183 2019-03-13 05:06:03.000000 credsmash-3.0.0/credsmash/api/put.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    12966 2024-05-22 02:38:51.000000 credsmash-3.0.0/credsmash/cli.py
+-rw-r--r--   0 nathan    (1000) nathan    (1000)      708 2018-05-16 01:54:08.000000 credsmash-3.0.0/credsmash/cli_dynamodb.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-22 03:02:59.482098 credsmash-3.0.0/credsmash/crypto/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1569 2019-03-13 05:47:16.000000 credsmash-3.0.0/credsmash/crypto/__init__.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     5211 2024-05-22 02:41:20.000000 credsmash-3.0.0/credsmash/crypto/aes_ctr.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     1982 2019-03-13 05:47:16.000000 credsmash-3.0.0/credsmash/crypto/aes_gcm.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     5692 2019-03-13 05:47:16.000000 credsmash-3.0.0/credsmash/dynamodb_storage_service.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2114 2024-05-22 02:41:29.000000 credsmash-3.0.0/credsmash/kms_key_service.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     8699 2022-05-02 04:30:48.000000 credsmash-3.0.0/credsmash/templates.py
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     7088 2019-03-13 05:58:16.000000 credsmash-3.0.0/credsmash/util.py
+drwxrwxr-x   0 nathan    (1000) nathan    (1000)        0 2024-05-22 03:02:59.482098 credsmash-3.0.0/credsmash.egg-info/
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)    16631 2024-05-22 03:02:59.000000 credsmash-3.0.0/credsmash.egg-info/PKG-INFO
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      649 2024-05-22 03:02:59.000000 credsmash-3.0.0/credsmash.egg-info/SOURCES.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)        1 2024-05-22 03:02:59.000000 credsmash-3.0.0/credsmash.egg-info/dependency_links.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      301 2024-05-22 03:02:59.000000 credsmash-3.0.0/credsmash.egg-info/entry_points.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      148 2024-05-22 03:02:59.000000 credsmash-3.0.0/credsmash.egg-info/requires.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)       10 2024-05-22 03:02:59.000000 credsmash-3.0.0/credsmash.egg-info/top_level.txt
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)      171 2024-05-22 03:02:59.482098 credsmash-3.0.0/setup.cfg
+-rw-rw-r--   0 nathan    (1000) nathan    (1000)     2289 2024-05-22 02:37:12.000000 credsmash-3.0.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `credsmash-2.3.1/README.md` & `credsmash-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `credsmash-2.3.1/credsmash/crypto/aes_ctr.py` & `credsmash-3.0.0/credsmash/crypto/aes_ctr.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,12 +171,12 @@
     b = s.encode('ascii')
     return base64.b64decode(b)
 
 
 class IntegrityError(Exception):
 
     def __init__(self, value=""):
-        self.value = "INTEGRITY ERROR: " + value if value is not "" else \
+        self.value = "INTEGRITY ERROR: " + value if value != "" else \
                      "INTEGRITY ERROR"
 
     def __str__(self):
         return self.value
```

### Comparing `credsmash-2.3.1/credsmash/crypto/__init__.py` & `credsmash-3.0.0/credsmash/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `credsmash-2.3.1/credsmash/crypto/aes_gcm.py` & `credsmash-3.0.0/credsmash/crypto/aes_gcm.py`

 * *Files identical despite different names*

### Comparing `credsmash-2.3.1/credsmash/cli_dynamodb.py` & `credsmash-3.0.0/credsmash/cli_dynamodb.py`

 * *Files identical despite different names*

### Comparing `credsmash-2.3.1/credsmash/cli.py` & `credsmash-3.0.0/credsmash/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import absolute_import, division, print_function
 
 import codecs
 import fnmatch
 import logging
 import operator
 import os
-import sys
 
 import boto3
 import click
-import pkg_resources
+import importlib_metadata
 import six
 
 import credsmash.api
 from credsmash.crypto import ALGO_AES_CTR
 from credsmash.util import set_stream_logger, detect_format, \
     parse_config, read_one, read_many, write_one, write_many
 
@@ -38,16 +37,16 @@
     def session(self):
         if self._session is None:
            self._session = boto3.Session()
         return self._session
 
     @staticmethod
     def load_entry_point(group, name):
-        entry_points = pkg_resources.iter_entry_points(
-            group, name
+        entry_points = importlib_metadata.entry_points(
+            group=group, name=name
         )
         for entry_point in entry_points:
             return entry_point.load()
         raise RuntimeError('Not found EntryPoint(group={0},name={1})'.format(group, name))
 
     @property
     def key_service(self):
@@ -392,12 +391,12 @@
             **ctx.obj.algorithm_options
         )
         logger.info('Stored {0} @ version {1}'.format(secret_name, stored_version))
     logger.debug('Stored {0} secrets'.format(len(secrets)))
 
 
 # Load any extra CLI's
-for ep in pkg_resources.iter_entry_points('credsmash.cli'):
+for ep in importlib_metadata.entry_points(group='credsmash.cli'):
     try:
         ep.load()
     except ImportError:
         pass
```

### Comparing `credsmash-2.3.1/credsmash/api/put.py` & `credsmash-3.0.0/credsmash/api/put.py`

 * *Files identical despite different names*

### Comparing `credsmash-2.3.1/credsmash/api/prune.py` & `credsmash-3.0.0/credsmash/api/prune.py`

 * *Files identical despite different names*

### Comparing `credsmash-2.3.1/credsmash/api/delete.py` & `credsmash-3.0.0/credsmash/api/delete.py`

 * *Files identical despite different names*

### Comparing `credsmash-2.3.1/credsmash/kms_key_service.py` & `credsmash-3.0.0/credsmash/kms_key_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,11 +44,11 @@
     def __repr__(self):
         return 'KmsKeyService(key_id={0},context={1})'.format(self.key_id, self.encryption_context)
 
 
 class KmsError(Exception):
 
     def __init__(self, value=""):
-        self.value = "KMS ERROR: " + value if value is not "" else "KMS ERROR"
+        self.value = "KMS ERROR: " + value if value != "" else "KMS ERROR"
 
     def __str__(self):
         return self.value
```

### Comparing `credsmash-2.3.1/credsmash/templates.py` & `credsmash-3.0.0/credsmash/templates.py`

 * *Files identical despite different names*

### Comparing `credsmash-2.3.1/credsmash/util.py` & `credsmash-3.0.0/credsmash/util.py`

 * *Files identical despite different names*

### Comparing `credsmash-2.3.1/credsmash/dynamodb_storage_service.py` & `credsmash-3.0.0/credsmash/dynamodb_storage_service.py`

 * *Files identical despite different names*

### Comparing `credsmash-2.3.1/setup.py` & `credsmash-3.0.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,20 +33,22 @@
 
     packages=find_packages(exclude=('tests',)),
 
     package_data={
         'credsmash': ['VERSION']
     },
 
-    python_requires=">=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*",
+    python_requires=">=3.8",
     install_requires=[
         'cryptography',
         'boto3',
         'click',
-        'six'
+        'six',
+        'importlib_resources',
+        'importlib_metadata'
     ],
     tests_require=[
         'pytest',
     ],
     extras_require={
         'yaml': ['PyYAML'],
         'templates': ['jinja2'],
@@ -70,14 +72,15 @@
     },
 
     classifiers=[
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
-        'Programming Language :: Python :: 2.7',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

### Comparing `credsmash-2.3.1/PKG-INFO` & `credsmash-3.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,321 +1,325 @@
 Metadata-Version: 2.1
 Name: credsmash
-Version: 2.3.1
+Version: 3.0.0
 Summary: A utility for managing secrets in the cloud using AWS KMS and DynamoDB
 Home-page: https://github.com/3stack-software/credsmash
 Maintainer: Nathan Muir
 Maintainer-email: ndmuir@gmail.com
 License: Apache2
-Description: # Cred*Smash*
-        
-        This is a fork of [credstash](https://github.com/fugue/credstash), to add 
-        some utilities I find useful, see `HISTORY.md` for details.
-        
-        ## Quick Installation
-        1. `pip install credsmash[yaml, templates]`
-        2. Set up a key called `credsmash` in KMS
-        3. Make sure you have AWS creds in a place that boto/botocore can read 
-           them (eg, [Use environment `AWS_CONFIG_FILE`](http://boto3.readthedocs.io/en/latest/guide/configuration.html#environment-variables))
-        4. `credsmash setup-dynamodb`
-        
-        
-        ## What is this?
-        Software systems often need access to some shared credential. For example, 
-        your web application needs access to a database password, or an API key for some 
-        third party service.
-        
-        Some organizations build complete credential-management systems, but for most of us, 
-        managing these credentials is usually an afterthought. In the best case, people use 
-        systems like ansible-vault, which does a pretty good job, but leads to other management 
-        issues (like where/how to store the master key). A lot of credential management schemes 
-        amount to just SCP'ing a `secrets` file out to the fleet, or in the worst case, burning 
-        secrets into the SCM (do a github search on `password`).
-        
-        CredSmash is a very simple, easy to use credential management and distribution system 
-        that uses AWS Key Management Service (KMS) for key wrapping and master-key storage, 
-        and DynamoDB for credential storage and sharing.
-        
-        ## How does it work?
-        After you complete the steps in the `Setup` section, you will have an encryption key 
-        in KMS (in this README, we will refer to that key as the `master key`), and a credential
-        storage table in DDB.
-        
-        ### Stashing Secrets
-        Whenever you want to store/share a credential, such as a database password, you simply 
-        run `echo [credential-value] | credsmash put [credential-name] -`. 
-        For example, `echo 'supersecretpassword1234' | credsmash put myapp.db.prod -`. credsmash will
-        go to the KMS and generate a unique data encryption key, which itself is encrypted by the
-        master key (this is called key wrapping). credsmash will use the data encryption key to
-        encrypt the credential value. It will then store the encrypted credential, along with the 
-        wrapped (encrypted) data encryption key in the credential store in DynamoDB.
-        
-        ### Getting Secrets
-        When you want to fetch the credential, for example as part of the bootstrap process on 
-        your web-server, you simply do `credsmash get [credential-name]`. For example, 
-        `export DB_PASSWORD=$(credsmash get myapp.db.prod)`. When you run `get`, 
-        credsmash will go and fetch the encrypted credential and the wrapped encryption 
-        key from the credential store (DynamoDB). It will then send the wrapped encryption key to 
-        KMS, where it is decrypted with the master key. credsmash then uses the decrypted data 
-        encryption key to decrypt the credential. The credential is printed to `stdout`, so you 
-        can use it in scripts or assign it to environment variables.
-        
-        ### Controlling and Auditing Secrets
-        Optionally, you can include any number of [Encryption Context](http://docs.aws.amazon.com/kms/latest/developerguide/encrypt-context.html)
-        key value pairs to associate with the credential. The exact set of encryption context 
-        key value pairs that were associated with the credential when it was `put` in DynamoDB 
-        must be provided in the `get` request to successfully decrypt the credential. These 
-        encryption context key value pairs are useful to provide auditing context to the encryption
-        and decryption operations in your CloudTrail logs. They are also useful for constraining 
-        access to a given credsmash stored credential by using KMS Key Policy conditions and KMS 
-        Grant conditions. Doing so allows you to, for example, make sure that your database servers 
-        and web-servers can read the web-server DB user password but your database servers can not 
-        read your web-servers TLS/SSL certificate's private key. A `put` request with encryption 
-        context would look like 
-        `echo 'supersecretpassword1234' | credsmash put myapp.db.prod - --context app.tier db --context environment prod`. 
-        In order for your web-servers to read that same credential they would execute a `get` call 
-        like `export DB_PASSWORD=$(credsmash get myapp.db.prod  --context environment prod --context app.tier db)`
-        
-        ### Versioning Secrets
-        Credentials stored in the credential-store are versioned and immutable. That is, if 
-        you `put` a credential called `foo` with a version of `1` and a value of `bar`, 
-        then foo version 1 will always have a value of bar, and there is no way in `credsmash` to 
-        change its value (although you could go fiddle with the bits in DDB, but you shouldn't do that). 
-        Credential rotation is handed through versions. Suppose you do `echo 'bar' | credsmash put foo -`, and 
-        then decide later to rotate `foo`, you can put version 2 of `foo` by doing 
-        `echo 'baz' | credsmash put foo - -v 2 `. 
-        The next time you do `credsmash get foo`, it will return `baz`. You can get specific credential versions
-        as well (with the same `-v` flag). You can fetch a list of all credentials in the 
-        credential-store and their versions with the `list` command.
-        
-        If you use incrementing integer version numbers (for example, `[1, 2, 3, ...]`), then you can 
-        simply skip the `-v` flag with the `put` command to automatically increment the version number. 
-        However, because of the lexicographical sorting in DynamoDB, `credsmash` will left-pad 
-        the version representation with zeros (for example, `[001, 025, 103, ...]`, except to 19 characters,
-        enough to handle `sys.maxint` on 64-bit systems).
-        
-        ## Dependencies
-        credsmash uses the following AWS services:
-        * AWS Key Management Service (KMS) - for master key management and key wrapping
-        * AWS Identity and Access Management - for access control
-        * Amazon DynamoDB - for credential storage
-        
-        ## Setup
-        ### tl;dr
-        1. Set up a key called `credsmash` in KMS
-        2. `pip install credsmash`
-        3. Make sure you have AWS creds in a place that boto/botocore can read them
-        4. Run `credsmash setup-dynamodb`
-        
-        ### Setting up KMS
-        `credsmash` will not currently set up your KMS master key. To create a KMS master key,
-        
-        1. Go to the AWS console
-        2. Go to the IAM console/tab
-        3. Click "Encryption Keys" in the left
-        4. Click "Create Key". For alias, put "credsmash". If you want to use a different name, be sure to pass it to credsmash with the `-k` flag
-        5. Decide what IAM principals you want to be able to manage the key
-        6. On the "Key Usage Permissions" screen, pick the IAM users/roles that will be using credsmash (you can change your mind later)
-        7. Done!
-        
-        ### Setting up credsmash
-        The easiest thing to do is to just run `pip install credsmash`. That will download and install credsmash and its dependencies (boto and PyCypto).
-        
-        The second easiest thing to do is to do `python setup.py install` in the `credsmash` directory.
-        
-        The python dependencies for credsmash are in the `requirements.txt` file. You can install them with `pip install -r requirements.txt`.
-        
-        In all cases, you will need a C compiler for building `PyCrypto` (you can install `gcc` by doing `apt-get install gcc` or `yum install gcc`).
-        
-        You will need to have AWS credentials accessible to boto/botocore. The easiest thing to do is to run credsmash on an EC2 instance with an IAM role. Alternatively, you can put AWS credentials in the `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY` environment variables. Or, you can put them in a file (see http://boto.readthedocs.org/en/latest/boto_config_tut.html).
-        
-        You can specify the region in which `credsmash` should operate by using the `-r` flag, or by setting the `AWS_DEFAULT_REGION` environment variable. Note that the command line flag takes precedence over the environment variable. If you set neither, then `credsmash` will operate against us-east-1.
-        
-        Once credentials are in place, run `credsmash setup-dynamodb`. This will create the DDB table needed for credential storage.
-        
-        ### Working with multiple AWS accounts (profiles)
-        
-        If you need to work with multiple AWS accounts, an easy thing to do is to set up multiple profiles in 
-        your `~/.aws/credentials` file. For example,
-        
-        ```
-        [dev]
-        aws_access_key_id = AKIDEXAMPLEASDFASDF
-        aws_secret_access_key = SKIDEXAMPLE2103429812039423
-        [prod]
-        aws_access_key_id= AKIDEXAMPLEASDFASDF
-        aws_secret_access_key= SKIDEXAMPLE2103429812039423
-        ```
-        
-        Then, by setting the `AWS_PROFILE` environment variable to the name of the profile, (dev or prod, in this case), 
-        you can point credsmash at the appropriate account.
-        
-        See https://blogs.aws.amazon.com/security/post/Tx3D6U6WSFGOK2H/A-New-and-Standardized-Way-to-Manage-Credentials-in-the-AWS-SDKs for more information.
-        
-        ## Usage
-        ```
-        Usage: credsmash [OPTIONS] COMMAND [ARGS]...
-        
-        Options:
-          -c, --config PATH
-          -t, --table-name TEXT     DynamoDB table to use for credential storage
-          -k, --key-id TEXT         the KMS key-id of the master key to use. See the
-                                    README for more information. Defaults to
-                                    alias/credsmash
-          --context <TEXT TEXT>...  the KMS encryption context to use.Only works if
-                                    --key-id is passed.
-          --help                    Show this message and exit.
-        
-        Commands:
-          delete            Delete every version of a single secret
-          delete-many       Delete every version of all matching secrets
-          find-many         Find all secrets matching <pattern>
-          find-one          Find exactly one secret matching <pattern>
-          get               Fetch the latest, or a specific version of a...
-          get-all           Fetch the latest version of all secrets
-          list              List all secrets & their versions.
-          prune             Delete all but the latest version of a single...
-          prune-many        Delete all but the latest version of all...
-          put               Store a secret
-          put-many          Store many secrets
-          render-template   Render a configuration template....
-          render-templates  Render multiple configuration templates -...
-          setup-dynamodb    Setup the credential table in AWS DynamoDB
-        ```
-        
-        ## IAM Policies
-        
-        ### Secret Writer
-        You can put or write secrets to credsmash by either using KMS Key Grants, KMS Key Policies,
-        or IAM Policies. If you are using IAM Policies, the following IAM permissions are the minimum 
-        required to be able to put or write secrets:
-        
-        ```
-        {
-          "Version": "2012-10-17",
-          "Statement": [
-            {
-              "Action": [
-                "kms:GenerateDataKey"
-              ],
-              "Effect": "Allow",
-              "Resource": "arn:aws:kms:us-east-1:AWSACCOUNTID:key/KEY-GUID"
-            },
-            {
-              "Action": [
-                "dynamodb:PutItem"
-              ],
-              "Effect": "Allow",
-              "Resource": "arn:aws:dynamodb:us-east-1:AWSACCOUNTID:table/credential-store"
-            }
-          ]
-        }
-        ```
-        If you are using Key Policies or Grants, then the `kms:GenerateDataKey` is not required in the policy for the 
-        IAM user/group/role. Replace `AWSACCOUNTID` with the account ID for your table, and replace the KEY-GUID with the 
-        identifier for your KMS key (which you can find in the KMS console).
-        
-        ### Secret Reader
-        You can read secrets from credsmash with the get or getall actions by either using KMS Key Grants, KMS Key 
-        Policies, or IAM Policies. If you are using IAM Policies, the following IAM permissions are the minimum 
-        required to be able to get or read secrets:
-        ```
-        {
-          "Version": "2012-10-17",
-          "Statement": [
-            {
-              "Action": [
-                "kms:Decrypt"
-              ],
-              "Effect": "Allow",
-              "Resource": "arn:aws:kms:us-east-1:AWSACCOUNTID:key/KEY-GUID"
-            },
-            {
-              "Action": [
-                "dynamodb:GetItem",
-                "dynamodb:Query",
-                "dynamodb:Scan"
-              ],
-              "Effect": "Allow",
-              "Resource": "arn:aws:dynamodb:us-east-1:AWSACCOUNTID:table/credential-store"
-            }
-          ]
-        }
-        ```
-        If you are using Key Policies or Grants, then the `kms:Decrypt` is not required in the policy for
-        the IAM user/group/role. Replace `AWSACCOUNTID` with the account ID for your table, and replace 
-        the KEY-GUID with the identifier for your KMS key (which you can find in the KMS console). Note 
-        that the `dynamodb:Scan` permission is not required if you do not use wildcards in your `get`s.
-        
-        ## Security Notes
-        Any IAM principal who can get items from the credential store DDB table, and can call KMS.Decrypt,
-        can read stored credentials.
-        
-        The target deployment-story for `credsmash` is an EC2 instance running with an IAM role that has 
-        permissions to read the credential store and use the master key. Since IAM role credentials are 
-        vended by the instance metadata service, by default, any user on the system can fetch creds and 
-        use them to retrieve credentials. That means that by default, the instance boundary is the security
-        boundary for this system. If you are worried about unauthorized users on your instance, you should 
-        take steps to secure access to the Instance Metadata Service (for example, use iptables to block 
-        connections to 169.254.169.254 except for privileged users). Also, because credsmash is written in 
-        python, if an attacker can dump the memory of the credsmash process, they may be able to recover 
-        credentials. This is a known issue, but again, in the target deployment case, the security boundary 
-        is assumed to be the instance boundary.
-        
-        ## Frequently Asked Questions (FAQ)
-        
-        ### 1. Where is the master key stored?
-        The master key is stored in AWS Key Management Service (KMS), where it is stored in secure 
-        HSM-backed storage. The Master Key never leaves the KMS service.
-        
-        ### 2. How is credential rotation handled?
-        Every credential in the store has a version number. Whenever you want to a credential to a new 
-        value, you have to do a `put` with a new credential version. For example, if you have `foo` 
-        version 1 in the database, then to update `foo`, you can put version 2. You can either specify 
-        the version manually (i.e. `echo 'bar' | credsmash put foo - -v 2`), or you can omit the `-v` flag, 
-        which  will attempt to autoincrement the version number (for example, `echo 'baz' | credsmash put foo -`). 
-        Whenever you do a `get` operation, credsmash will fetch the most recent (highest version) version of that 
-        credential. So, to do credential rotation, simply put a new version of the credential, and clients fetching 
-        the credential will get the new version.
-        
-        ### 3. How much do the AWS services needed to run credsmash cost?
-        tl;dr: If you are using less than 25 reads/sec and 25 writes per second on DDB today, 
-        it will cost ~$1/month to use credsmash.
-        
-        The master key in KMS costs $1 per month.
-        
-        The credential store DDB table uses 1 provisioned read and 1 provisioned write throughput, along 
-        with a small amount of actual storage. This falls well below the free tier for DDB (25 reads and 
-        25 writes per second). If you are already a heavy DDB user and exceed the free tier, the credential 
-        store table will cost about $0.53 per month (mostly from the write throughput).
-        
-        If you are using credsmash heavily and need to increase the provisioned reads/writes, you may incur 
-        additional charges. You can estimate your bill using the AWS Simple Monthly Calculator 
-        (http://calculator.s3.amazonaws.com/index.html#s=DYNAMODB).
-        
-        ### 4. Why DynamoDB for the credential store? Why not S3?
-        DDB fits the application really well. Having very low latency fetches are really nice if credsmash is 
-        in the critical path of spinning up an application. Being able to turn throughput up or down based on
-        load and requirements are also great things to have in a config management tool. Also, as credsmash gets 
-        into more complex credential management functions, the query capabilities of DDB get super handy.
-        
-        That said, S3 support may happen someday.
-        
-        ### 5. Where can I learn more about use cases and context for something like credsmash?
-        Check out this blog post: http://blog.fugue.it/2015-04-21-aws-kms-secrets.html
-        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: documentation
 Provides-Extra: yaml
 Provides-Extra: templates
+Provides-Extra: documentation
 Provides-Extra: dev
+License-File: LICENSE
+
+# Cred*Smash*
+
+This is a fork of [credstash](https://github.com/fugue/credstash), to add 
+some utilities I find useful, see `HISTORY.md` for details.
+
+## Quick Installation
+1. `pip install credsmash[yaml, templates]`
+2. Set up a key called `credsmash` in KMS
+3. Make sure you have AWS creds in a place that boto/botocore can read 
+   them (eg, [Use environment `AWS_CONFIG_FILE`](http://boto3.readthedocs.io/en/latest/guide/configuration.html#environment-variables))
+4. `credsmash setup-dynamodb`
+
+
+## What is this?
+Software systems often need access to some shared credential. For example, 
+your web application needs access to a database password, or an API key for some 
+third party service.
+
+Some organizations build complete credential-management systems, but for most of us, 
+managing these credentials is usually an afterthought. In the best case, people use 
+systems like ansible-vault, which does a pretty good job, but leads to other management 
+issues (like where/how to store the master key). A lot of credential management schemes 
+amount to just SCP'ing a `secrets` file out to the fleet, or in the worst case, burning 
+secrets into the SCM (do a github search on `password`).
+
+CredSmash is a very simple, easy to use credential management and distribution system 
+that uses AWS Key Management Service (KMS) for key wrapping and master-key storage, 
+and DynamoDB for credential storage and sharing.
+
+## How does it work?
+After you complete the steps in the `Setup` section, you will have an encryption key 
+in KMS (in this README, we will refer to that key as the `master key`), and a credential
+storage table in DDB.
+
+### Stashing Secrets
+Whenever you want to store/share a credential, such as a database password, you simply 
+run `echo [credential-value] | credsmash put [credential-name] -`. 
+For example, `echo 'supersecretpassword1234' | credsmash put myapp.db.prod -`. credsmash will
+go to the KMS and generate a unique data encryption key, which itself is encrypted by the
+master key (this is called key wrapping). credsmash will use the data encryption key to
+encrypt the credential value. It will then store the encrypted credential, along with the 
+wrapped (encrypted) data encryption key in the credential store in DynamoDB.
+
+### Getting Secrets
+When you want to fetch the credential, for example as part of the bootstrap process on 
+your web-server, you simply do `credsmash get [credential-name]`. For example, 
+`export DB_PASSWORD=$(credsmash get myapp.db.prod)`. When you run `get`, 
+credsmash will go and fetch the encrypted credential and the wrapped encryption 
+key from the credential store (DynamoDB). It will then send the wrapped encryption key to 
+KMS, where it is decrypted with the master key. credsmash then uses the decrypted data 
+encryption key to decrypt the credential. The credential is printed to `stdout`, so you 
+can use it in scripts or assign it to environment variables.
+
+### Controlling and Auditing Secrets
+Optionally, you can include any number of [Encryption Context](http://docs.aws.amazon.com/kms/latest/developerguide/encrypt-context.html)
+key value pairs to associate with the credential. The exact set of encryption context 
+key value pairs that were associated with the credential when it was `put` in DynamoDB 
+must be provided in the `get` request to successfully decrypt the credential. These 
+encryption context key value pairs are useful to provide auditing context to the encryption
+and decryption operations in your CloudTrail logs. They are also useful for constraining 
+access to a given credsmash stored credential by using KMS Key Policy conditions and KMS 
+Grant conditions. Doing so allows you to, for example, make sure that your database servers 
+and web-servers can read the web-server DB user password but your database servers can not 
+read your web-servers TLS/SSL certificate's private key. A `put` request with encryption 
+context would look like 
+`echo 'supersecretpassword1234' | credsmash put myapp.db.prod - --context app.tier db --context environment prod`. 
+In order for your web-servers to read that same credential they would execute a `get` call 
+like `export DB_PASSWORD=$(credsmash get myapp.db.prod  --context environment prod --context app.tier db)`
+
+### Versioning Secrets
+Credentials stored in the credential-store are versioned and immutable. That is, if 
+you `put` a credential called `foo` with a version of `1` and a value of `bar`, 
+then foo version 1 will always have a value of bar, and there is no way in `credsmash` to 
+change its value (although you could go fiddle with the bits in DDB, but you shouldn't do that). 
+Credential rotation is handed through versions. Suppose you do `echo 'bar' | credsmash put foo -`, and 
+then decide later to rotate `foo`, you can put version 2 of `foo` by doing 
+`echo 'baz' | credsmash put foo - -v 2 `. 
+The next time you do `credsmash get foo`, it will return `baz`. You can get specific credential versions
+as well (with the same `-v` flag). You can fetch a list of all credentials in the 
+credential-store and their versions with the `list` command.
+
+If you use incrementing integer version numbers (for example, `[1, 2, 3, ...]`), then you can 
+simply skip the `-v` flag with the `put` command to automatically increment the version number. 
+However, because of the lexicographical sorting in DynamoDB, `credsmash` will left-pad 
+the version representation with zeros (for example, `[001, 025, 103, ...]`, except to 19 characters,
+enough to handle `sys.maxint` on 64-bit systems).
+
+## Dependencies
+credsmash uses the following AWS services:
+* AWS Key Management Service (KMS) - for master key management and key wrapping
+* AWS Identity and Access Management - for access control
+* Amazon DynamoDB - for credential storage
+
+## Setup
+### tl;dr
+1. Set up a key called `credsmash` in KMS
+2. `pip install credsmash`
+3. Make sure you have AWS creds in a place that boto/botocore can read them
+4. Run `credsmash setup-dynamodb`
+
+### Setting up KMS
+`credsmash` will not currently set up your KMS master key. To create a KMS master key,
+
+1. Go to the AWS console
+2. Go to the IAM console/tab
+3. Click "Encryption Keys" in the left
+4. Click "Create Key". For alias, put "credsmash". If you want to use a different name, be sure to pass it to credsmash with the `-k` flag
+5. Decide what IAM principals you want to be able to manage the key
+6. On the "Key Usage Permissions" screen, pick the IAM users/roles that will be using credsmash (you can change your mind later)
+7. Done!
+
+### Setting up credsmash
+The easiest thing to do is to just run `pip install credsmash`. That will download and install credsmash and its dependencies (boto and PyCypto).
+
+The second easiest thing to do is to do `python setup.py install` in the `credsmash` directory.
+
+The python dependencies for credsmash are in the `requirements.txt` file. You can install them with `pip install -r requirements.txt`.
+
+In all cases, you will need a C compiler for building `PyCrypto` (you can install `gcc` by doing `apt-get install gcc` or `yum install gcc`).
+
+You will need to have AWS credentials accessible to boto/botocore. The easiest thing to do is to run credsmash on an EC2 instance with an IAM role. Alternatively, you can put AWS credentials in the `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY` environment variables. Or, you can put them in a file (see http://boto.readthedocs.org/en/latest/boto_config_tut.html).
+
+You can specify the region in which `credsmash` should operate by using the `-r` flag, or by setting the `AWS_DEFAULT_REGION` environment variable. Note that the command line flag takes precedence over the environment variable. If you set neither, then `credsmash` will operate against us-east-1.
+
+Once credentials are in place, run `credsmash setup-dynamodb`. This will create the DDB table needed for credential storage.
+
+### Working with multiple AWS accounts (profiles)
+
+If you need to work with multiple AWS accounts, an easy thing to do is to set up multiple profiles in 
+your `~/.aws/credentials` file. For example,
+
+```
+[dev]
+aws_access_key_id = AKIDEXAMPLEASDFASDF
+aws_secret_access_key = SKIDEXAMPLE2103429812039423
+[prod]
+aws_access_key_id= AKIDEXAMPLEASDFASDF
+aws_secret_access_key= SKIDEXAMPLE2103429812039423
+```
+
+Then, by setting the `AWS_PROFILE` environment variable to the name of the profile, (dev or prod, in this case), 
+you can point credsmash at the appropriate account.
+
+See https://blogs.aws.amazon.com/security/post/Tx3D6U6WSFGOK2H/A-New-and-Standardized-Way-to-Manage-Credentials-in-the-AWS-SDKs for more information.
+
+## Usage
+```
+Usage: credsmash [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  -c, --config PATH
+  -t, --table-name TEXT     DynamoDB table to use for credential storage
+  -k, --key-id TEXT         the KMS key-id of the master key to use. See the
+                            README for more information. Defaults to
+                            alias/credsmash
+  --context <TEXT TEXT>...  the KMS encryption context to use.Only works if
+                            --key-id is passed.
+  --help                    Show this message and exit.
+
+Commands:
+  delete            Delete every version of a single secret
+  delete-many       Delete every version of all matching secrets
+  find-many         Find all secrets matching <pattern>
+  find-one          Find exactly one secret matching <pattern>
+  get               Fetch the latest, or a specific version of a...
+  get-all           Fetch the latest version of all secrets
+  list              List all secrets & their versions.
+  prune             Delete all but the latest version of a single...
+  prune-many        Delete all but the latest version of all...
+  put               Store a secret
+  put-many          Store many secrets
+  render-template   Render a configuration template....
+  render-templates  Render multiple configuration templates -...
+  setup-dynamodb    Setup the credential table in AWS DynamoDB
+```
+
+## IAM Policies
+
+### Secret Writer
+You can put or write secrets to credsmash by either using KMS Key Grants, KMS Key Policies,
+or IAM Policies. If you are using IAM Policies, the following IAM permissions are the minimum 
+required to be able to put or write secrets:
+
+```
+{
+  "Version": "2012-10-17",
+  "Statement": [
+    {
+      "Action": [
+        "kms:GenerateDataKey"
+      ],
+      "Effect": "Allow",
+      "Resource": "arn:aws:kms:us-east-1:AWSACCOUNTID:key/KEY-GUID"
+    },
+    {
+      "Action": [
+        "dynamodb:PutItem"
+      ],
+      "Effect": "Allow",
+      "Resource": "arn:aws:dynamodb:us-east-1:AWSACCOUNTID:table/credential-store"
+    }
+  ]
+}
+```
+If you are using Key Policies or Grants, then the `kms:GenerateDataKey` is not required in the policy for the 
+IAM user/group/role. Replace `AWSACCOUNTID` with the account ID for your table, and replace the KEY-GUID with the 
+identifier for your KMS key (which you can find in the KMS console).
+
+### Secret Reader
+You can read secrets from credsmash with the get or getall actions by either using KMS Key Grants, KMS Key 
+Policies, or IAM Policies. If you are using IAM Policies, the following IAM permissions are the minimum 
+required to be able to get or read secrets:
+```
+{
+  "Version": "2012-10-17",
+  "Statement": [
+    {
+      "Action": [
+        "kms:Decrypt"
+      ],
+      "Effect": "Allow",
+      "Resource": "arn:aws:kms:us-east-1:AWSACCOUNTID:key/KEY-GUID"
+    },
+    {
+      "Action": [
+        "dynamodb:GetItem",
+        "dynamodb:Query",
+        "dynamodb:Scan"
+      ],
+      "Effect": "Allow",
+      "Resource": "arn:aws:dynamodb:us-east-1:AWSACCOUNTID:table/credential-store"
+    }
+  ]
+}
+```
+If you are using Key Policies or Grants, then the `kms:Decrypt` is not required in the policy for
+the IAM user/group/role. Replace `AWSACCOUNTID` with the account ID for your table, and replace 
+the KEY-GUID with the identifier for your KMS key (which you can find in the KMS console). Note 
+that the `dynamodb:Scan` permission is not required if you do not use wildcards in your `get`s.
+
+## Security Notes
+Any IAM principal who can get items from the credential store DDB table, and can call KMS.Decrypt,
+can read stored credentials.
+
+The target deployment-story for `credsmash` is an EC2 instance running with an IAM role that has 
+permissions to read the credential store and use the master key. Since IAM role credentials are 
+vended by the instance metadata service, by default, any user on the system can fetch creds and 
+use them to retrieve credentials. That means that by default, the instance boundary is the security
+boundary for this system. If you are worried about unauthorized users on your instance, you should 
+take steps to secure access to the Instance Metadata Service (for example, use iptables to block 
+connections to 169.254.169.254 except for privileged users). Also, because credsmash is written in 
+python, if an attacker can dump the memory of the credsmash process, they may be able to recover 
+credentials. This is a known issue, but again, in the target deployment case, the security boundary 
+is assumed to be the instance boundary.
+
+## Frequently Asked Questions (FAQ)
+
+### 1. Where is the master key stored?
+The master key is stored in AWS Key Management Service (KMS), where it is stored in secure 
+HSM-backed storage. The Master Key never leaves the KMS service.
+
+### 2. How is credential rotation handled?
+Every credential in the store has a version number. Whenever you want to a credential to a new 
+value, you have to do a `put` with a new credential version. For example, if you have `foo` 
+version 1 in the database, then to update `foo`, you can put version 2. You can either specify 
+the version manually (i.e. `echo 'bar' | credsmash put foo - -v 2`), or you can omit the `-v` flag, 
+which  will attempt to autoincrement the version number (for example, `echo 'baz' | credsmash put foo -`). 
+Whenever you do a `get` operation, credsmash will fetch the most recent (highest version) version of that 
+credential. So, to do credential rotation, simply put a new version of the credential, and clients fetching 
+the credential will get the new version.
+
+### 3. How much do the AWS services needed to run credsmash cost?
+tl;dr: If you are using less than 25 reads/sec and 25 writes per second on DDB today, 
+it will cost ~$1/month to use credsmash.
+
+The master key in KMS costs $1 per month.
+
+The credential store DDB table uses 1 provisioned read and 1 provisioned write throughput, along 
+with a small amount of actual storage. This falls well below the free tier for DDB (25 reads and 
+25 writes per second). If you are already a heavy DDB user and exceed the free tier, the credential 
+store table will cost about $0.53 per month (mostly from the write throughput).
+
+If you are using credsmash heavily and need to increase the provisioned reads/writes, you may incur 
+additional charges. You can estimate your bill using the AWS Simple Monthly Calculator 
+(http://calculator.s3.amazonaws.com/index.html#s=DYNAMODB).
+
+### 4. Why DynamoDB for the credential store? Why not S3?
+DDB fits the application really well. Having very low latency fetches are really nice if credsmash is 
+in the critical path of spinning up an application. Being able to turn throughput up or down based on
+load and requirements are also great things to have in a config management tool. Also, as credsmash gets 
+into more complex credential management functions, the query capabilities of DDB get super handy.
+
+That said, S3 support may happen someday.
+
+### 5. Where can I learn more about use cases and context for something like credsmash?
+Check out this blog post: http://blog.fugue.it/2015-04-21-aws-kms-secrets.html
+
+
```

### Comparing `credsmash-2.3.1/credsmash.egg-info/PKG-INFO` & `credsmash-3.0.0/credsmash.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,321 +1,325 @@
 Metadata-Version: 2.1
 Name: credsmash
-Version: 2.3.1
+Version: 3.0.0
 Summary: A utility for managing secrets in the cloud using AWS KMS and DynamoDB
 Home-page: https://github.com/3stack-software/credsmash
 Maintainer: Nathan Muir
 Maintainer-email: ndmuir@gmail.com
 License: Apache2
-Description: # Cred*Smash*
-        
-        This is a fork of [credstash](https://github.com/fugue/credstash), to add 
-        some utilities I find useful, see `HISTORY.md` for details.
-        
-        ## Quick Installation
-        1. `pip install credsmash[yaml, templates]`
-        2. Set up a key called `credsmash` in KMS
-        3. Make sure you have AWS creds in a place that boto/botocore can read 
-           them (eg, [Use environment `AWS_CONFIG_FILE`](http://boto3.readthedocs.io/en/latest/guide/configuration.html#environment-variables))
-        4. `credsmash setup-dynamodb`
-        
-        
-        ## What is this?
-        Software systems often need access to some shared credential. For example, 
-        your web application needs access to a database password, or an API key for some 
-        third party service.
-        
-        Some organizations build complete credential-management systems, but for most of us, 
-        managing these credentials is usually an afterthought. In the best case, people use 
-        systems like ansible-vault, which does a pretty good job, but leads to other management 
-        issues (like where/how to store the master key). A lot of credential management schemes 
-        amount to just SCP'ing a `secrets` file out to the fleet, or in the worst case, burning 
-        secrets into the SCM (do a github search on `password`).
-        
-        CredSmash is a very simple, easy to use credential management and distribution system 
-        that uses AWS Key Management Service (KMS) for key wrapping and master-key storage, 
-        and DynamoDB for credential storage and sharing.
-        
-        ## How does it work?
-        After you complete the steps in the `Setup` section, you will have an encryption key 
-        in KMS (in this README, we will refer to that key as the `master key`), and a credential
-        storage table in DDB.
-        
-        ### Stashing Secrets
-        Whenever you want to store/share a credential, such as a database password, you simply 
-        run `echo [credential-value] | credsmash put [credential-name] -`. 
-        For example, `echo 'supersecretpassword1234' | credsmash put myapp.db.prod -`. credsmash will
-        go to the KMS and generate a unique data encryption key, which itself is encrypted by the
-        master key (this is called key wrapping). credsmash will use the data encryption key to
-        encrypt the credential value. It will then store the encrypted credential, along with the 
-        wrapped (encrypted) data encryption key in the credential store in DynamoDB.
-        
-        ### Getting Secrets
-        When you want to fetch the credential, for example as part of the bootstrap process on 
-        your web-server, you simply do `credsmash get [credential-name]`. For example, 
-        `export DB_PASSWORD=$(credsmash get myapp.db.prod)`. When you run `get`, 
-        credsmash will go and fetch the encrypted credential and the wrapped encryption 
-        key from the credential store (DynamoDB). It will then send the wrapped encryption key to 
-        KMS, where it is decrypted with the master key. credsmash then uses the decrypted data 
-        encryption key to decrypt the credential. The credential is printed to `stdout`, so you 
-        can use it in scripts or assign it to environment variables.
-        
-        ### Controlling and Auditing Secrets
-        Optionally, you can include any number of [Encryption Context](http://docs.aws.amazon.com/kms/latest/developerguide/encrypt-context.html)
-        key value pairs to associate with the credential. The exact set of encryption context 
-        key value pairs that were associated with the credential when it was `put` in DynamoDB 
-        must be provided in the `get` request to successfully decrypt the credential. These 
-        encryption context key value pairs are useful to provide auditing context to the encryption
-        and decryption operations in your CloudTrail logs. They are also useful for constraining 
-        access to a given credsmash stored credential by using KMS Key Policy conditions and KMS 
-        Grant conditions. Doing so allows you to, for example, make sure that your database servers 
-        and web-servers can read the web-server DB user password but your database servers can not 
-        read your web-servers TLS/SSL certificate's private key. A `put` request with encryption 
-        context would look like 
-        `echo 'supersecretpassword1234' | credsmash put myapp.db.prod - --context app.tier db --context environment prod`. 
-        In order for your web-servers to read that same credential they would execute a `get` call 
-        like `export DB_PASSWORD=$(credsmash get myapp.db.prod  --context environment prod --context app.tier db)`
-        
-        ### Versioning Secrets
-        Credentials stored in the credential-store are versioned and immutable. That is, if 
-        you `put` a credential called `foo` with a version of `1` and a value of `bar`, 
-        then foo version 1 will always have a value of bar, and there is no way in `credsmash` to 
-        change its value (although you could go fiddle with the bits in DDB, but you shouldn't do that). 
-        Credential rotation is handed through versions. Suppose you do `echo 'bar' | credsmash put foo -`, and 
-        then decide later to rotate `foo`, you can put version 2 of `foo` by doing 
-        `echo 'baz' | credsmash put foo - -v 2 `. 
-        The next time you do `credsmash get foo`, it will return `baz`. You can get specific credential versions
-        as well (with the same `-v` flag). You can fetch a list of all credentials in the 
-        credential-store and their versions with the `list` command.
-        
-        If you use incrementing integer version numbers (for example, `[1, 2, 3, ...]`), then you can 
-        simply skip the `-v` flag with the `put` command to automatically increment the version number. 
-        However, because of the lexicographical sorting in DynamoDB, `credsmash` will left-pad 
-        the version representation with zeros (for example, `[001, 025, 103, ...]`, except to 19 characters,
-        enough to handle `sys.maxint` on 64-bit systems).
-        
-        ## Dependencies
-        credsmash uses the following AWS services:
-        * AWS Key Management Service (KMS) - for master key management and key wrapping
-        * AWS Identity and Access Management - for access control
-        * Amazon DynamoDB - for credential storage
-        
-        ## Setup
-        ### tl;dr
-        1. Set up a key called `credsmash` in KMS
-        2. `pip install credsmash`
-        3. Make sure you have AWS creds in a place that boto/botocore can read them
-        4. Run `credsmash setup-dynamodb`
-        
-        ### Setting up KMS
-        `credsmash` will not currently set up your KMS master key. To create a KMS master key,
-        
-        1. Go to the AWS console
-        2. Go to the IAM console/tab
-        3. Click "Encryption Keys" in the left
-        4. Click "Create Key". For alias, put "credsmash". If you want to use a different name, be sure to pass it to credsmash with the `-k` flag
-        5. Decide what IAM principals you want to be able to manage the key
-        6. On the "Key Usage Permissions" screen, pick the IAM users/roles that will be using credsmash (you can change your mind later)
-        7. Done!
-        
-        ### Setting up credsmash
-        The easiest thing to do is to just run `pip install credsmash`. That will download and install credsmash and its dependencies (boto and PyCypto).
-        
-        The second easiest thing to do is to do `python setup.py install` in the `credsmash` directory.
-        
-        The python dependencies for credsmash are in the `requirements.txt` file. You can install them with `pip install -r requirements.txt`.
-        
-        In all cases, you will need a C compiler for building `PyCrypto` (you can install `gcc` by doing `apt-get install gcc` or `yum install gcc`).
-        
-        You will need to have AWS credentials accessible to boto/botocore. The easiest thing to do is to run credsmash on an EC2 instance with an IAM role. Alternatively, you can put AWS credentials in the `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY` environment variables. Or, you can put them in a file (see http://boto.readthedocs.org/en/latest/boto_config_tut.html).
-        
-        You can specify the region in which `credsmash` should operate by using the `-r` flag, or by setting the `AWS_DEFAULT_REGION` environment variable. Note that the command line flag takes precedence over the environment variable. If you set neither, then `credsmash` will operate against us-east-1.
-        
-        Once credentials are in place, run `credsmash setup-dynamodb`. This will create the DDB table needed for credential storage.
-        
-        ### Working with multiple AWS accounts (profiles)
-        
-        If you need to work with multiple AWS accounts, an easy thing to do is to set up multiple profiles in 
-        your `~/.aws/credentials` file. For example,
-        
-        ```
-        [dev]
-        aws_access_key_id = AKIDEXAMPLEASDFASDF
-        aws_secret_access_key = SKIDEXAMPLE2103429812039423
-        [prod]
-        aws_access_key_id= AKIDEXAMPLEASDFASDF
-        aws_secret_access_key= SKIDEXAMPLE2103429812039423
-        ```
-        
-        Then, by setting the `AWS_PROFILE` environment variable to the name of the profile, (dev or prod, in this case), 
-        you can point credsmash at the appropriate account.
-        
-        See https://blogs.aws.amazon.com/security/post/Tx3D6U6WSFGOK2H/A-New-and-Standardized-Way-to-Manage-Credentials-in-the-AWS-SDKs for more information.
-        
-        ## Usage
-        ```
-        Usage: credsmash [OPTIONS] COMMAND [ARGS]...
-        
-        Options:
-          -c, --config PATH
-          -t, --table-name TEXT     DynamoDB table to use for credential storage
-          -k, --key-id TEXT         the KMS key-id of the master key to use. See the
-                                    README for more information. Defaults to
-                                    alias/credsmash
-          --context <TEXT TEXT>...  the KMS encryption context to use.Only works if
-                                    --key-id is passed.
-          --help                    Show this message and exit.
-        
-        Commands:
-          delete            Delete every version of a single secret
-          delete-many       Delete every version of all matching secrets
-          find-many         Find all secrets matching <pattern>
-          find-one          Find exactly one secret matching <pattern>
-          get               Fetch the latest, or a specific version of a...
-          get-all           Fetch the latest version of all secrets
-          list              List all secrets & their versions.
-          prune             Delete all but the latest version of a single...
-          prune-many        Delete all but the latest version of all...
-          put               Store a secret
-          put-many          Store many secrets
-          render-template   Render a configuration template....
-          render-templates  Render multiple configuration templates -...
-          setup-dynamodb    Setup the credential table in AWS DynamoDB
-        ```
-        
-        ## IAM Policies
-        
-        ### Secret Writer
-        You can put or write secrets to credsmash by either using KMS Key Grants, KMS Key Policies,
-        or IAM Policies. If you are using IAM Policies, the following IAM permissions are the minimum 
-        required to be able to put or write secrets:
-        
-        ```
-        {
-          "Version": "2012-10-17",
-          "Statement": [
-            {
-              "Action": [
-                "kms:GenerateDataKey"
-              ],
-              "Effect": "Allow",
-              "Resource": "arn:aws:kms:us-east-1:AWSACCOUNTID:key/KEY-GUID"
-            },
-            {
-              "Action": [
-                "dynamodb:PutItem"
-              ],
-              "Effect": "Allow",
-              "Resource": "arn:aws:dynamodb:us-east-1:AWSACCOUNTID:table/credential-store"
-            }
-          ]
-        }
-        ```
-        If you are using Key Policies or Grants, then the `kms:GenerateDataKey` is not required in the policy for the 
-        IAM user/group/role. Replace `AWSACCOUNTID` with the account ID for your table, and replace the KEY-GUID with the 
-        identifier for your KMS key (which you can find in the KMS console).
-        
-        ### Secret Reader
-        You can read secrets from credsmash with the get or getall actions by either using KMS Key Grants, KMS Key 
-        Policies, or IAM Policies. If you are using IAM Policies, the following IAM permissions are the minimum 
-        required to be able to get or read secrets:
-        ```
-        {
-          "Version": "2012-10-17",
-          "Statement": [
-            {
-              "Action": [
-                "kms:Decrypt"
-              ],
-              "Effect": "Allow",
-              "Resource": "arn:aws:kms:us-east-1:AWSACCOUNTID:key/KEY-GUID"
-            },
-            {
-              "Action": [
-                "dynamodb:GetItem",
-                "dynamodb:Query",
-                "dynamodb:Scan"
-              ],
-              "Effect": "Allow",
-              "Resource": "arn:aws:dynamodb:us-east-1:AWSACCOUNTID:table/credential-store"
-            }
-          ]
-        }
-        ```
-        If you are using Key Policies or Grants, then the `kms:Decrypt` is not required in the policy for
-        the IAM user/group/role. Replace `AWSACCOUNTID` with the account ID for your table, and replace 
-        the KEY-GUID with the identifier for your KMS key (which you can find in the KMS console). Note 
-        that the `dynamodb:Scan` permission is not required if you do not use wildcards in your `get`s.
-        
-        ## Security Notes
-        Any IAM principal who can get items from the credential store DDB table, and can call KMS.Decrypt,
-        can read stored credentials.
-        
-        The target deployment-story for `credsmash` is an EC2 instance running with an IAM role that has 
-        permissions to read the credential store and use the master key. Since IAM role credentials are 
-        vended by the instance metadata service, by default, any user on the system can fetch creds and 
-        use them to retrieve credentials. That means that by default, the instance boundary is the security
-        boundary for this system. If you are worried about unauthorized users on your instance, you should 
-        take steps to secure access to the Instance Metadata Service (for example, use iptables to block 
-        connections to 169.254.169.254 except for privileged users). Also, because credsmash is written in 
-        python, if an attacker can dump the memory of the credsmash process, they may be able to recover 
-        credentials. This is a known issue, but again, in the target deployment case, the security boundary 
-        is assumed to be the instance boundary.
-        
-        ## Frequently Asked Questions (FAQ)
-        
-        ### 1. Where is the master key stored?
-        The master key is stored in AWS Key Management Service (KMS), where it is stored in secure 
-        HSM-backed storage. The Master Key never leaves the KMS service.
-        
-        ### 2. How is credential rotation handled?
-        Every credential in the store has a version number. Whenever you want to a credential to a new 
-        value, you have to do a `put` with a new credential version. For example, if you have `foo` 
-        version 1 in the database, then to update `foo`, you can put version 2. You can either specify 
-        the version manually (i.e. `echo 'bar' | credsmash put foo - -v 2`), or you can omit the `-v` flag, 
-        which  will attempt to autoincrement the version number (for example, `echo 'baz' | credsmash put foo -`). 
-        Whenever you do a `get` operation, credsmash will fetch the most recent (highest version) version of that 
-        credential. So, to do credential rotation, simply put a new version of the credential, and clients fetching 
-        the credential will get the new version.
-        
-        ### 3. How much do the AWS services needed to run credsmash cost?
-        tl;dr: If you are using less than 25 reads/sec and 25 writes per second on DDB today, 
-        it will cost ~$1/month to use credsmash.
-        
-        The master key in KMS costs $1 per month.
-        
-        The credential store DDB table uses 1 provisioned read and 1 provisioned write throughput, along 
-        with a small amount of actual storage. This falls well below the free tier for DDB (25 reads and 
-        25 writes per second). If you are already a heavy DDB user and exceed the free tier, the credential 
-        store table will cost about $0.53 per month (mostly from the write throughput).
-        
-        If you are using credsmash heavily and need to increase the provisioned reads/writes, you may incur 
-        additional charges. You can estimate your bill using the AWS Simple Monthly Calculator 
-        (http://calculator.s3.amazonaws.com/index.html#s=DYNAMODB).
-        
-        ### 4. Why DynamoDB for the credential store? Why not S3?
-        DDB fits the application really well. Having very low latency fetches are really nice if credsmash is 
-        in the critical path of spinning up an application. Being able to turn throughput up or down based on
-        load and requirements are also great things to have in a config management tool. Also, as credsmash gets 
-        into more complex credential management functions, the query capabilities of DDB get super handy.
-        
-        That said, S3 support may happen someday.
-        
-        ### 5. Where can I learn more about use cases and context for something like credsmash?
-        Check out this blog post: http://blog.fugue.it/2015-04-21-aws-kms-secrets.html
-        
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=2.7,!=3.0.*,!=3.1.*,!=3.2.*,!=3.3.*,!=3.4.*,!=3.5.*
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: documentation
 Provides-Extra: yaml
 Provides-Extra: templates
+Provides-Extra: documentation
 Provides-Extra: dev
+License-File: LICENSE
+
+# Cred*Smash*
+
+This is a fork of [credstash](https://github.com/fugue/credstash), to add 
+some utilities I find useful, see `HISTORY.md` for details.
+
+## Quick Installation
+1. `pip install credsmash[yaml, templates]`
+2. Set up a key called `credsmash` in KMS
+3. Make sure you have AWS creds in a place that boto/botocore can read 
+   them (eg, [Use environment `AWS_CONFIG_FILE`](http://boto3.readthedocs.io/en/latest/guide/configuration.html#environment-variables))
+4. `credsmash setup-dynamodb`
+
+
+## What is this?
+Software systems often need access to some shared credential. For example, 
+your web application needs access to a database password, or an API key for some 
+third party service.
+
+Some organizations build complete credential-management systems, but for most of us, 
+managing these credentials is usually an afterthought. In the best case, people use 
+systems like ansible-vault, which does a pretty good job, but leads to other management 
+issues (like where/how to store the master key). A lot of credential management schemes 
+amount to just SCP'ing a `secrets` file out to the fleet, or in the worst case, burning 
+secrets into the SCM (do a github search on `password`).
+
+CredSmash is a very simple, easy to use credential management and distribution system 
+that uses AWS Key Management Service (KMS) for key wrapping and master-key storage, 
+and DynamoDB for credential storage and sharing.
+
+## How does it work?
+After you complete the steps in the `Setup` section, you will have an encryption key 
+in KMS (in this README, we will refer to that key as the `master key`), and a credential
+storage table in DDB.
+
+### Stashing Secrets
+Whenever you want to store/share a credential, such as a database password, you simply 
+run `echo [credential-value] | credsmash put [credential-name] -`. 
+For example, `echo 'supersecretpassword1234' | credsmash put myapp.db.prod -`. credsmash will
+go to the KMS and generate a unique data encryption key, which itself is encrypted by the
+master key (this is called key wrapping). credsmash will use the data encryption key to
+encrypt the credential value. It will then store the encrypted credential, along with the 
+wrapped (encrypted) data encryption key in the credential store in DynamoDB.
+
+### Getting Secrets
+When you want to fetch the credential, for example as part of the bootstrap process on 
+your web-server, you simply do `credsmash get [credential-name]`. For example, 
+`export DB_PASSWORD=$(credsmash get myapp.db.prod)`. When you run `get`, 
+credsmash will go and fetch the encrypted credential and the wrapped encryption 
+key from the credential store (DynamoDB). It will then send the wrapped encryption key to 
+KMS, where it is decrypted with the master key. credsmash then uses the decrypted data 
+encryption key to decrypt the credential. The credential is printed to `stdout`, so you 
+can use it in scripts or assign it to environment variables.
+
+### Controlling and Auditing Secrets
+Optionally, you can include any number of [Encryption Context](http://docs.aws.amazon.com/kms/latest/developerguide/encrypt-context.html)
+key value pairs to associate with the credential. The exact set of encryption context 
+key value pairs that were associated with the credential when it was `put` in DynamoDB 
+must be provided in the `get` request to successfully decrypt the credential. These 
+encryption context key value pairs are useful to provide auditing context to the encryption
+and decryption operations in your CloudTrail logs. They are also useful for constraining 
+access to a given credsmash stored credential by using KMS Key Policy conditions and KMS 
+Grant conditions. Doing so allows you to, for example, make sure that your database servers 
+and web-servers can read the web-server DB user password but your database servers can not 
+read your web-servers TLS/SSL certificate's private key. A `put` request with encryption 
+context would look like 
+`echo 'supersecretpassword1234' | credsmash put myapp.db.prod - --context app.tier db --context environment prod`. 
+In order for your web-servers to read that same credential they would execute a `get` call 
+like `export DB_PASSWORD=$(credsmash get myapp.db.prod  --context environment prod --context app.tier db)`
+
+### Versioning Secrets
+Credentials stored in the credential-store are versioned and immutable. That is, if 
+you `put` a credential called `foo` with a version of `1` and a value of `bar`, 
+then foo version 1 will always have a value of bar, and there is no way in `credsmash` to 
+change its value (although you could go fiddle with the bits in DDB, but you shouldn't do that). 
+Credential rotation is handed through versions. Suppose you do `echo 'bar' | credsmash put foo -`, and 
+then decide later to rotate `foo`, you can put version 2 of `foo` by doing 
+`echo 'baz' | credsmash put foo - -v 2 `. 
+The next time you do `credsmash get foo`, it will return `baz`. You can get specific credential versions
+as well (with the same `-v` flag). You can fetch a list of all credentials in the 
+credential-store and their versions with the `list` command.
+
+If you use incrementing integer version numbers (for example, `[1, 2, 3, ...]`), then you can 
+simply skip the `-v` flag with the `put` command to automatically increment the version number. 
+However, because of the lexicographical sorting in DynamoDB, `credsmash` will left-pad 
+the version representation with zeros (for example, `[001, 025, 103, ...]`, except to 19 characters,
+enough to handle `sys.maxint` on 64-bit systems).
+
+## Dependencies
+credsmash uses the following AWS services:
+* AWS Key Management Service (KMS) - for master key management and key wrapping
+* AWS Identity and Access Management - for access control
+* Amazon DynamoDB - for credential storage
+
+## Setup
+### tl;dr
+1. Set up a key called `credsmash` in KMS
+2. `pip install credsmash`
+3. Make sure you have AWS creds in a place that boto/botocore can read them
+4. Run `credsmash setup-dynamodb`
+
+### Setting up KMS
+`credsmash` will not currently set up your KMS master key. To create a KMS master key,
+
+1. Go to the AWS console
+2. Go to the IAM console/tab
+3. Click "Encryption Keys" in the left
+4. Click "Create Key". For alias, put "credsmash". If you want to use a different name, be sure to pass it to credsmash with the `-k` flag
+5. Decide what IAM principals you want to be able to manage the key
+6. On the "Key Usage Permissions" screen, pick the IAM users/roles that will be using credsmash (you can change your mind later)
+7. Done!
+
+### Setting up credsmash
+The easiest thing to do is to just run `pip install credsmash`. That will download and install credsmash and its dependencies (boto and PyCypto).
+
+The second easiest thing to do is to do `python setup.py install` in the `credsmash` directory.
+
+The python dependencies for credsmash are in the `requirements.txt` file. You can install them with `pip install -r requirements.txt`.
+
+In all cases, you will need a C compiler for building `PyCrypto` (you can install `gcc` by doing `apt-get install gcc` or `yum install gcc`).
+
+You will need to have AWS credentials accessible to boto/botocore. The easiest thing to do is to run credsmash on an EC2 instance with an IAM role. Alternatively, you can put AWS credentials in the `AWS_ACCESS_KEY_ID` and `AWS_SECRET_ACCESS_KEY` environment variables. Or, you can put them in a file (see http://boto.readthedocs.org/en/latest/boto_config_tut.html).
+
+You can specify the region in which `credsmash` should operate by using the `-r` flag, or by setting the `AWS_DEFAULT_REGION` environment variable. Note that the command line flag takes precedence over the environment variable. If you set neither, then `credsmash` will operate against us-east-1.
+
+Once credentials are in place, run `credsmash setup-dynamodb`. This will create the DDB table needed for credential storage.
+
+### Working with multiple AWS accounts (profiles)
+
+If you need to work with multiple AWS accounts, an easy thing to do is to set up multiple profiles in 
+your `~/.aws/credentials` file. For example,
+
+```
+[dev]
+aws_access_key_id = AKIDEXAMPLEASDFASDF
+aws_secret_access_key = SKIDEXAMPLE2103429812039423
+[prod]
+aws_access_key_id= AKIDEXAMPLEASDFASDF
+aws_secret_access_key= SKIDEXAMPLE2103429812039423
+```
+
+Then, by setting the `AWS_PROFILE` environment variable to the name of the profile, (dev or prod, in this case), 
+you can point credsmash at the appropriate account.
+
+See https://blogs.aws.amazon.com/security/post/Tx3D6U6WSFGOK2H/A-New-and-Standardized-Way-to-Manage-Credentials-in-the-AWS-SDKs for more information.
+
+## Usage
+```
+Usage: credsmash [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  -c, --config PATH
+  -t, --table-name TEXT     DynamoDB table to use for credential storage
+  -k, --key-id TEXT         the KMS key-id of the master key to use. See the
+                            README for more information. Defaults to
+                            alias/credsmash
+  --context <TEXT TEXT>...  the KMS encryption context to use.Only works if
+                            --key-id is passed.
+  --help                    Show this message and exit.
+
+Commands:
+  delete            Delete every version of a single secret
+  delete-many       Delete every version of all matching secrets
+  find-many         Find all secrets matching <pattern>
+  find-one          Find exactly one secret matching <pattern>
+  get               Fetch the latest, or a specific version of a...
+  get-all           Fetch the latest version of all secrets
+  list              List all secrets & their versions.
+  prune             Delete all but the latest version of a single...
+  prune-many        Delete all but the latest version of all...
+  put               Store a secret
+  put-many          Store many secrets
+  render-template   Render a configuration template....
+  render-templates  Render multiple configuration templates -...
+  setup-dynamodb    Setup the credential table in AWS DynamoDB
+```
+
+## IAM Policies
+
+### Secret Writer
+You can put or write secrets to credsmash by either using KMS Key Grants, KMS Key Policies,
+or IAM Policies. If you are using IAM Policies, the following IAM permissions are the minimum 
+required to be able to put or write secrets:
+
+```
+{
+  "Version": "2012-10-17",
+  "Statement": [
+    {
+      "Action": [
+        "kms:GenerateDataKey"
+      ],
+      "Effect": "Allow",
+      "Resource": "arn:aws:kms:us-east-1:AWSACCOUNTID:key/KEY-GUID"
+    },
+    {
+      "Action": [
+        "dynamodb:PutItem"
+      ],
+      "Effect": "Allow",
+      "Resource": "arn:aws:dynamodb:us-east-1:AWSACCOUNTID:table/credential-store"
+    }
+  ]
+}
+```
+If you are using Key Policies or Grants, then the `kms:GenerateDataKey` is not required in the policy for the 
+IAM user/group/role. Replace `AWSACCOUNTID` with the account ID for your table, and replace the KEY-GUID with the 
+identifier for your KMS key (which you can find in the KMS console).
+
+### Secret Reader
+You can read secrets from credsmash with the get or getall actions by either using KMS Key Grants, KMS Key 
+Policies, or IAM Policies. If you are using IAM Policies, the following IAM permissions are the minimum 
+required to be able to get or read secrets:
+```
+{
+  "Version": "2012-10-17",
+  "Statement": [
+    {
+      "Action": [
+        "kms:Decrypt"
+      ],
+      "Effect": "Allow",
+      "Resource": "arn:aws:kms:us-east-1:AWSACCOUNTID:key/KEY-GUID"
+    },
+    {
+      "Action": [
+        "dynamodb:GetItem",
+        "dynamodb:Query",
+        "dynamodb:Scan"
+      ],
+      "Effect": "Allow",
+      "Resource": "arn:aws:dynamodb:us-east-1:AWSACCOUNTID:table/credential-store"
+    }
+  ]
+}
+```
+If you are using Key Policies or Grants, then the `kms:Decrypt` is not required in the policy for
+the IAM user/group/role. Replace `AWSACCOUNTID` with the account ID for your table, and replace 
+the KEY-GUID with the identifier for your KMS key (which you can find in the KMS console). Note 
+that the `dynamodb:Scan` permission is not required if you do not use wildcards in your `get`s.
+
+## Security Notes
+Any IAM principal who can get items from the credential store DDB table, and can call KMS.Decrypt,
+can read stored credentials.
+
+The target deployment-story for `credsmash` is an EC2 instance running with an IAM role that has 
+permissions to read the credential store and use the master key. Since IAM role credentials are 
+vended by the instance metadata service, by default, any user on the system can fetch creds and 
+use them to retrieve credentials. That means that by default, the instance boundary is the security
+boundary for this system. If you are worried about unauthorized users on your instance, you should 
+take steps to secure access to the Instance Metadata Service (for example, use iptables to block 
+connections to 169.254.169.254 except for privileged users). Also, because credsmash is written in 
+python, if an attacker can dump the memory of the credsmash process, they may be able to recover 
+credentials. This is a known issue, but again, in the target deployment case, the security boundary 
+is assumed to be the instance boundary.
+
+## Frequently Asked Questions (FAQ)
+
+### 1. Where is the master key stored?
+The master key is stored in AWS Key Management Service (KMS), where it is stored in secure 
+HSM-backed storage. The Master Key never leaves the KMS service.
+
+### 2. How is credential rotation handled?
+Every credential in the store has a version number. Whenever you want to a credential to a new 
+value, you have to do a `put` with a new credential version. For example, if you have `foo` 
+version 1 in the database, then to update `foo`, you can put version 2. You can either specify 
+the version manually (i.e. `echo 'bar' | credsmash put foo - -v 2`), or you can omit the `-v` flag, 
+which  will attempt to autoincrement the version number (for example, `echo 'baz' | credsmash put foo -`). 
+Whenever you do a `get` operation, credsmash will fetch the most recent (highest version) version of that 
+credential. So, to do credential rotation, simply put a new version of the credential, and clients fetching 
+the credential will get the new version.
+
+### 3. How much do the AWS services needed to run credsmash cost?
+tl;dr: If you are using less than 25 reads/sec and 25 writes per second on DDB today, 
+it will cost ~$1/month to use credsmash.
+
+The master key in KMS costs $1 per month.
+
+The credential store DDB table uses 1 provisioned read and 1 provisioned write throughput, along 
+with a small amount of actual storage. This falls well below the free tier for DDB (25 reads and 
+25 writes per second). If you are already a heavy DDB user and exceed the free tier, the credential 
+store table will cost about $0.53 per month (mostly from the write throughput).
+
+If you are using credsmash heavily and need to increase the provisioned reads/writes, you may incur 
+additional charges. You can estimate your bill using the AWS Simple Monthly Calculator 
+(http://calculator.s3.amazonaws.com/index.html#s=DYNAMODB).
+
+### 4. Why DynamoDB for the credential store? Why not S3?
+DDB fits the application really well. Having very low latency fetches are really nice if credsmash is 
+in the critical path of spinning up an application. Being able to turn throughput up or down based on
+load and requirements are also great things to have in a config management tool. Also, as credsmash gets 
+into more complex credential management functions, the query capabilities of DDB get super handy.
+
+That said, S3 support may happen someday.
+
+### 5. Where can I learn more about use cases and context for something like credsmash?
+Check out this blog post: http://blog.fugue.it/2015-04-21-aws-kms-secrets.html
+
+
```

### Comparing `credsmash-2.3.1/credsmash.egg-info/SOURCES.txt` & `credsmash-3.0.0/credsmash.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.cfg
 setup.py
 credsmash/VERSION
 credsmash/__init__.py
 credsmash/cli.py
 credsmash/cli_dynamodb.py
```

