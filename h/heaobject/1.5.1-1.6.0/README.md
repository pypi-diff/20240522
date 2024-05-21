# Comparing `tmp/heaobject-1.5.1.tar.gz` & `tmp/heaobject-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaobject-1.5.1.tar", last modified: Fri May  3 23:00:45 2024, max compression
+gzip compressed data, was "heaobject-1.6.0.tar", last modified: Tue May 21 22:49:58 2024, max compression
```

## Comparing `heaobject-1.5.1.tar` & `heaobject-1.6.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-03 23:00:45.340875 heaobject-1.5.1/
--rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:08.000000 heaobject-1.5.1/LICENSE
--rw-rw-rw-   0        0        0     4832 2024-05-03 23:00:45.338737 heaobject-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     3326 2024-04-24 17:43:21.000000 heaobject-1.5.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-03 23:00:45.340875 heaobject-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0     2603 2024-05-03 22:59:57.000000 heaobject-1.5.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:00:45.271629 heaobject-1.5.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-03 23:00:45.328738 heaobject-1.5.1/src/heaobject/
--rw-rw-rw-   0        0        0     1247 2023-12-16 22:23:08.000000 heaobject-1.5.1/src/heaobject/__init__.py
--rw-rw-rw-   0        0        0     4970 2024-05-03 22:46:44.000000 heaobject-1.5.1/src/heaobject/account.py
--rw-rw-rw-   0        0        0    15629 2024-04-09 20:34:56.000000 heaobject-1.5.1/src/heaobject/activity.py
--rw-rw-rw-   0        0        0     4030 2023-12-16 22:23:08.000000 heaobject-1.5.1/src/heaobject/aws.py
--rw-rw-rw-   0        0        0     6945 2023-12-16 22:23:08.000000 heaobject-1.5.1/src/heaobject/awss3key.py
--rw-rw-rw-   0        0        0     7587 2024-04-09 20:34:56.000000 heaobject-1.5.1/src/heaobject/bucket.py
--rw-rw-rw-   0        0        0     9934 2024-05-03 22:47:48.000000 heaobject-1.5.1/src/heaobject/data.py
--rw-rw-rw-   0        0        0     2604 2023-12-16 22:23:08.000000 heaobject-1.5.1/src/heaobject/dataadapter.py
--rw-rw-rw-   0        0        0      272 2022-03-11 01:28:08.000000 heaobject-1.5.1/src/heaobject/dataelement.py
--rw-rw-rw-   0        0        0     1601 2022-03-11 01:28:08.000000 heaobject-1.5.1/src/heaobject/datamodel.py
--rw-rw-rw-   0        0        0      430 2022-03-11 01:28:08.000000 heaobject-1.5.1/src/heaobject/datapattern.py
--rw-rw-rw-   0        0        0      238 2023-12-16 22:23:08.000000 heaobject-1.5.1/src/heaobject/datatransform.py
--rw-rw-rw-   0        0        0      353 2023-12-16 22:23:08.000000 heaobject-1.5.1/src/heaobject/error.py
--rw-rw-rw-   0        0        0    22016 2024-04-09 20:34:56.000000 heaobject-1.5.1/src/heaobject/folder.py
--rw-rw-rw-   0        0        0     4662 2024-04-26 23:28:37.000000 heaobject-1.5.1/src/heaobject/keychain.py
--rw-rw-rw-   0        0        0     2859 2024-04-09 20:34:56.000000 heaobject-1.5.1/src/heaobject/mimetype.py
--rw-rw-rw-   0        0        0    14028 2024-05-03 22:46:44.000000 heaobject-1.5.1/src/heaobject/organization.py
--rw-rw-rw-   0        0        0    10911 2024-05-03 22:46:44.000000 heaobject-1.5.1/src/heaobject/person.py
--rw-rw-rw-   0        0        0     5129 2024-04-09 20:34:56.000000 heaobject-1.5.1/src/heaobject/project.py
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:08.000000 heaobject-1.5.1/src/heaobject/py.typed
--rw-rw-rw-   0        0        0      211 2024-04-09 20:34:56.000000 heaobject-1.5.1/src/heaobject/record.py
--rw-rw-rw-   0        0        0    24659 2024-04-09 20:34:56.000000 heaobject-1.5.1/src/heaobject/registry.py
--rw-rw-rw-   0        0        0    80257 2024-04-24 17:43:21.000000 heaobject-1.5.1/src/heaobject/root.py
--rw-rw-rw-   0        0        0      597 2024-04-09 20:34:56.000000 heaobject-1.5.1/src/heaobject/settings.py
--rw-rw-rw-   0        0        0       66 2024-03-26 22:41:59.000000 heaobject-1.5.1/src/heaobject/source.py
--rw-rw-rw-   0        0        0     1165 2023-12-16 22:23:08.000000 heaobject-1.5.1/src/heaobject/source2target.py
--rw-rw-rw-   0        0        0     4074 2024-04-09 20:34:56.000000 heaobject-1.5.1/src/heaobject/storage.py
--rw-rw-rw-   0        0        0    10289 2024-04-18 02:00:20.000000 heaobject-1.5.1/src/heaobject/trash.py
--rw-rw-rw-   0        0        0     1191 2024-04-24 22:21:12.000000 heaobject-1.5.1/src/heaobject/user.py
--rw-rw-rw-   0        0        0      498 2023-12-16 22:23:08.000000 heaobject-1.5.1/src/heaobject/util.py
--rw-rw-rw-   0        0        0     6618 2024-05-03 22:46:44.000000 heaobject-1.5.1/src/heaobject/volume.py
-drwxrwxrwx   0        0        0        0 2024-05-03 23:00:45.337164 heaobject-1.5.1/src/heaobject.egg-info/
--rw-rw-rw-   0        0        0     4832 2024-05-03 23:00:45.000000 heaobject-1.5.1/src/heaobject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      995 2024-05-03 23:00:45.000000 heaobject-1.5.1/src/heaobject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-03 23:00:45.000000 heaobject-1.5.1/src/heaobject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      144 2024-05-03 23:00:45.000000 heaobject-1.5.1/src/heaobject.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-03 23:00:45.000000 heaobject-1.5.1/src/heaobject.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 22:49:58.480852 heaobject-1.6.0/
+-rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:08.000000 heaobject-1.6.0/LICENSE
+-rw-rw-rw-   0        0        0     6085 2024-05-21 22:49:58.479271 heaobject-1.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4579 2024-05-21 22:47:32.000000 heaobject-1.6.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-21 22:49:58.480852 heaobject-1.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     2603 2024-05-21 22:49:15.000000 heaobject-1.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:49:58.410035 heaobject-1.6.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 22:49:58.467310 heaobject-1.6.0/src/heaobject/
+-rw-rw-rw-   0        0        0     1247 2023-12-16 22:23:08.000000 heaobject-1.6.0/src/heaobject/__init__.py
+-rw-rw-rw-   0        0        0    11351 2024-05-21 22:47:32.000000 heaobject-1.6.0/src/heaobject/account.py
+-rw-rw-rw-   0        0        0    15629 2024-04-09 20:34:56.000000 heaobject-1.6.0/src/heaobject/activity.py
+-rw-rw-rw-   0        0        0     4030 2023-12-16 22:23:08.000000 heaobject-1.6.0/src/heaobject/aws.py
+-rw-rw-rw-   0        0        0     6945 2023-12-16 22:23:08.000000 heaobject-1.6.0/src/heaobject/awss3key.py
+-rw-rw-rw-   0        0        0     7587 2024-04-09 20:34:56.000000 heaobject-1.6.0/src/heaobject/bucket.py
+-rw-rw-rw-   0        0        0     9988 2024-05-21 22:47:32.000000 heaobject-1.6.0/src/heaobject/data.py
+-rw-rw-rw-   0        0        0     2604 2023-12-16 22:23:08.000000 heaobject-1.6.0/src/heaobject/dataadapter.py
+-rw-rw-rw-   0        0        0      272 2022-03-11 01:28:08.000000 heaobject-1.6.0/src/heaobject/dataelement.py
+-rw-rw-rw-   0        0        0     1601 2022-03-11 01:28:08.000000 heaobject-1.6.0/src/heaobject/datamodel.py
+-rw-rw-rw-   0        0        0      430 2022-03-11 01:28:08.000000 heaobject-1.6.0/src/heaobject/datapattern.py
+-rw-rw-rw-   0        0        0      238 2023-12-16 22:23:08.000000 heaobject-1.6.0/src/heaobject/datatransform.py
+-rw-rw-rw-   0        0        0      353 2023-12-16 22:23:08.000000 heaobject-1.6.0/src/heaobject/error.py
+-rw-rw-rw-   0        0        0    22016 2024-04-09 20:34:56.000000 heaobject-1.6.0/src/heaobject/folder.py
+-rw-rw-rw-   0        0        0     4566 2024-05-21 22:47:32.000000 heaobject-1.6.0/src/heaobject/keychain.py
+-rw-rw-rw-   0        0        0     2859 2024-04-09 20:34:56.000000 heaobject-1.6.0/src/heaobject/mimetype.py
+-rw-rw-rw-   0        0        0    11029 2024-05-21 22:47:32.000000 heaobject-1.6.0/src/heaobject/organization.py
+-rw-rw-rw-   0        0        0    13108 2024-05-21 22:47:32.000000 heaobject-1.6.0/src/heaobject/person.py
+-rw-rw-rw-   0        0        0     5129 2024-04-09 20:34:56.000000 heaobject-1.6.0/src/heaobject/project.py
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:08.000000 heaobject-1.6.0/src/heaobject/py.typed
+-rw-rw-rw-   0        0        0      211 2024-04-09 20:34:56.000000 heaobject-1.6.0/src/heaobject/record.py
+-rw-rw-rw-   0        0        0    23400 2024-05-21 22:47:32.000000 heaobject-1.6.0/src/heaobject/registry.py
+-rw-rw-rw-   0        0        0    80257 2024-04-24 17:43:21.000000 heaobject-1.6.0/src/heaobject/root.py
+-rw-rw-rw-   0        0        0      597 2024-04-09 20:34:56.000000 heaobject-1.6.0/src/heaobject/settings.py
+-rw-rw-rw-   0        0        0       66 2024-03-26 22:41:59.000000 heaobject-1.6.0/src/heaobject/source.py
+-rw-rw-rw-   0        0        0     1165 2023-12-16 22:23:08.000000 heaobject-1.6.0/src/heaobject/source2target.py
+-rw-rw-rw-   0        0        0     4074 2024-04-09 20:34:56.000000 heaobject-1.6.0/src/heaobject/storage.py
+-rw-rw-rw-   0        0        0    10289 2024-04-18 02:00:20.000000 heaobject-1.6.0/src/heaobject/trash.py
+-rw-rw-rw-   0        0        0     1217 2024-05-21 22:47:32.000000 heaobject-1.6.0/src/heaobject/user.py
+-rw-rw-rw-   0        0        0      498 2023-12-16 22:23:08.000000 heaobject-1.6.0/src/heaobject/util.py
+-rw-rw-rw-   0        0        0     7290 2024-05-21 22:47:32.000000 heaobject-1.6.0/src/heaobject/volume.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:49:58.477736 heaobject-1.6.0/src/heaobject.egg-info/
+-rw-rw-rw-   0        0        0     6085 2024-05-21 22:49:58.000000 heaobject-1.6.0/src/heaobject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      995 2024-05-21 22:49:58.000000 heaobject-1.6.0/src/heaobject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 22:49:58.000000 heaobject-1.6.0/src/heaobject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      144 2024-05-21 22:49:58.000000 heaobject-1.6.0/src/heaobject.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-21 22:49:58.000000 heaobject-1.6.0/src/heaobject.egg-info/top_level.txt
```

### Comparing `heaobject-1.5.1/LICENSE` & `heaobject-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.1/PKG-INFO` & `heaobject-1.6.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.5.1
+Version: 1.6.0
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,35 @@
 Requires-Dist: mimetype-description~=0.1.0
 
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.6.0
+* Replaced heaobject.keychain.AWSCredentials role_arn attribute with a role attribute on heaobject.keychain.Credentials objects.
+* Added group_ids attribute to heaobject.person.Person.
+* New attributes in heaobject.account.Account: file_system_type, file_system_name.
+* New methods in heaobject.account.Account: get_role_to_assume(), and new_credentials().
+* Added full_name attribute to Person that is mirrors display_name.
+* Removed file_system_name parameter from queries of a registry Component's
+resources.
+* New heaobject.volume.Volume credential_type_name attribute.
+* Added role_ids attribute to heaobject.person.Group.
+* heaobject.user.is_system_user() now returns True for the system|credentialsmanager user.
+* Changed heaobject.organization.Organization.accounts to account_ids, which is
+a string, and removed the heaobject.account.AccountAssociation class.
+* Removed AWS-specific attributes and methods from heaobject.organization.Organization.
+* Docstring improvements.
+* Better default type_display_name for heaobject.account.AccountView objects.
+* Added group_type attribute to heaobject.person.Group.
+
+## Version 1.5.1
+* Ensure AWSS3FileObject's display_name attribute always has a non-None value.
+
 ## Version 1.5.0
 * Added attribute-level permissions.
 * Fixed bug in checking equality of AbstractAssociation objects.
 
 ## Version 1.4.0
 * Added "deleted" attribute to the trash module's TrashItem class.
 * Added Group class to the person module.
```

### Comparing `heaobject-1.5.1/README.md` & `heaobject-1.6.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,33 @@
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.6.0
+* Replaced heaobject.keychain.AWSCredentials role_arn attribute with a role attribute on heaobject.keychain.Credentials objects.
+* Added group_ids attribute to heaobject.person.Person.
+* New attributes in heaobject.account.Account: file_system_type, file_system_name.
+* New methods in heaobject.account.Account: get_role_to_assume(), and new_credentials().
+* Added full_name attribute to Person that is mirrors display_name.
+* Removed file_system_name parameter from queries of a registry Component's
+resources.
+* New heaobject.volume.Volume credential_type_name attribute.
+* Added role_ids attribute to heaobject.person.Group.
+* heaobject.user.is_system_user() now returns True for the system|credentialsmanager user.
+* Changed heaobject.organization.Organization.accounts to account_ids, which is
+a string, and removed the heaobject.account.AccountAssociation class.
+* Removed AWS-specific attributes and methods from heaobject.organization.Organization.
+* Docstring improvements.
+* Better default type_display_name for heaobject.account.AccountView objects.
+* Added group_type attribute to heaobject.person.Group.
+
+## Version 1.5.1
+* Ensure AWSS3FileObject's display_name attribute always has a non-None value.
+
 ## Version 1.5.0
 * Added attribute-level permissions.
 * Fixed bug in checking equality of AbstractAssociation objects.
 
 ## Version 1.4.0
 * Added "deleted" attribute to the trash module's TrashItem class.
 * Added Group class to the person module.
```

### Comparing `heaobject-1.5.1/setup.py` & `heaobject-1.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(name='heaobject',
-                 version='1.5.1',
+                 version='1.6.0',
                  description='Data and other classes that are passed into and out of HEA REST APIs.',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://risr.hci.utah.edu',
                  author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
                  author_email='Andrew.Post@hci.utah.edu',
                  python_requires='>=3.10',
```

### Comparing `heaobject-1.5.1/src/heaobject/__init__.py` & `heaobject-1.6.0/src/heaobject/__init__.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.1/src/heaobject/account.py` & `heaobject-1.6.0/src/heaobject/keychain.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,124 +1,132 @@
-from typing import Optional
-from .data import DataObject, SameMimeType
-from .root import AbstractAssociation
-from abc import ABC
-from email_validator import validate_email, EmailNotValidError  # Leave this here for other modules to use
-from functools import partial
+"""
+Classes supporting the management of user credentials and certificates.
+"""
+from datetime import datetime, timezone
+from typing import Optional, Union, TypeVar
+from heaobject import root
 
 
-class Account(DataObject, ABC):
+class Credentials(root.AbstractDesktopObject):
     """
-    Abstract base class for user accounts.
+        Stores a user's secrets, passwords, and keys, and makes them available to applications.
     """
-    pass
 
-
-class AWSAccount(Account, SameMimeType):
-    """
-    Represents an AWS account in the HEA desktop. Contains functions that allow access and setting of the value. Below are the attributes that can be accessed.
-
-    account_id (str)              : 1234567890
-    account_name (str)            : HCI - name
-    full_name (str)               : john smith
-    phone_number (str)            : 123-456-7890
-    alternate_contact_name (str)  : bob smith
-    alternate_email_address (str) : 123@hciutah.edu
-    alternate_phone_number (str)  : 123-456-7890
-    """
     def __init__(self) -> None:
         super().__init__()
-        self.__full_name: Optional[str] = None
-        self.__phone_number: Optional[str] = None
-        self.__alternate_contact_name: Optional[str] = None
-        self.__alternate_email_address: Optional[str] = None
-        self.__alternate_phone_number: Optional[str] = None
-        self.__email_address: Optional[str] = None
+        self.__account: str | None = None
+        self.__where:str | None = None
+        self.__password: str | None = None
+        self.__role: str | None = None
 
-    @classmethod
-    def get_mime_type(cls) -> str:
+    @property  # type: ignore
+    def account(self) -> Optional[str]:
         """
-        Returns the mime type for AWSAccount objects.
+        The username or account name.
+        """
+        return self.__account
+
+    @account.setter  # type: ignore
+    def account(self, account: Optional[str]) -> None:
+        self.__account = str(account) if account is not None else None
 
-        :return: application/x.awsaccount
+    @property  # type: ignore
+    def where(self) -> Optional[str]:
         """
-        return 'application/x.awsaccount'
+        The hostname, URL, service, or other location of the account.
+        """
+        return self.__where
 
-    @property
-    def mime_type(self) -> str:
-        """Read-only. The mime type for AWSAccount objects, application/x.awsaccount."""
-        return type(self).get_mime_type()
+    @where.setter  # type: ignore
+    def where(self, where: Optional[str]) -> None:
+        self.__where = str(where) if where is not None else None
 
+    @property  # type: ignore
+    def password(self) -> Optional[str]:
+        """
+        The account password or secret
+        """
+        return self.__password
 
-    @property
-    def full_name(self) -> Optional[str]:
-        """Returns the full name of person associated with this account"""
-        return self.__full_name
-
-    @full_name.setter
-    def full_name(self, full_name: Optional[str]) -> None:
-        """Sets the full name of person associated with this account"""
-        self.__full_name = str(full_name) if full_name is not None else None
+    @password.setter  # type: ignore
+    def password(self, password: Optional[str]) -> None:
+        self.__password = str(password) if password is not None else None
 
     @property
-    def phone_number(self) -> Optional[str]:
-        """Returns the phone number associated with the account"""
-        return self.__phone_number
-
-    @phone_number.setter
-    def phone_number(self, phone_number: Optional[str]) -> None:
-        """Sets the phone number associated with the account"""
-        self.__phone_number = str(phone_number) if phone_number is not None else None
+    def type_display_name(self) -> str:
+        return "Credentials"
 
     @property
-    def alternate_contact_name(self) -> Optional[str]:
-        """Returns the alternate contact full name of person associated with this account"""
-        return self.__alternate_contact_name
-
-    @alternate_contact_name.setter
-    def alternate_contact_name(self, alternate_contact_name: Optional[str]) -> None:
-        """Sets the alternate contact full name of person associated with this account"""
-        self.__alternate_contact_name = str(alternate_contact_name) if alternate_contact_name is not None else None
+    def role(self) -> str:
+        """A role to assume while logged in with these credentials."""
+        return self.__role
 
-    @property
-    def alternate_email_address(self) -> Optional[str]:
-        """Returns the alternate contact e-mail address associated with the account"""
-        return self.__alternate_email_address
-
-    @alternate_email_address.setter
-    def alternate_email_address(self, alternate_email_address: Optional[str]) -> None:
-        """Sets the alternate contact e-mail address associated with the account"""
-        self.__alternate_email_address = _validate_email(str(alternate_email_address)).email \
-            if alternate_email_address is not None else None
+    @role.setter
+    def role(self, role: str):
+        self.__role = str(role) if role is not None else None
 
-    @property
-    def alternate_phone_number(self) -> Optional[str]:
-        """Returns the alternate contact phone number associated with the account"""
-        return self.__alternate_phone_number
-
-    @alternate_phone_number.setter
-    def alternate_phone_number(self, alternate_phone_number: Optional[str]) -> None:
-        """Sets the alternate contact phone number associated with the account"""
-        self.__alternate_phone_number = str(alternate_phone_number) if alternate_phone_number is not None else None
 
-    @property
-    def email_address(self) -> Optional[str]:
-        return self.__email_address
+CredentialTypeVar = TypeVar('CredentialTypeVar', bound=Credentials)
 
-    @email_address.setter
-    def email_address(self, email_address: Optional[str]) -> None:
-        """Sets the email address associated with the account"""
-        self.__email_address = _validate_email(str(email_address)).email if email_address is not None else None
 
-    @property
-    def type_display_name(self) -> str:
-        return 'AWS Account'
+class AWSCredentials(Credentials):
+    def __init__(self) -> None:
+        super().__init__()
+        self.__session_token: Optional[str] = None
+        self.__expiration: Optional[str] = None
+        self.__temporary = False
+
 
+    @property  # type: ignore
+    def session_token(self) -> Optional[str]:
+        """
+        The session token.
+        """
+        return self.__session_token
+
+    @session_token.setter  # type: ignore
+    def session_token(self, session_token: Optional[str]):
+        self.__session_token = str(session_token) if session_token is not None else None
+
+    @property  # type: ignore
+    def expiration(self) -> Optional[str]:
+        """
+        The session's expiration time.
+        """
+        return self.__expiration
+
+    @expiration.setter  # type: ignore
+    def expiration(self, expiration: Optional[Union[str, datetime]]) -> None:
+        exp_formatted = expiration
+        if type(exp_formatted) is datetime:
+            exp_formatted = exp_formatted.strftime("%Y-%m-%dT%H:%M:%S%z")
+        self.__expiration = str(exp_formatted) if exp_formatted is not None else None
 
-class AccountAssociation(AbstractAssociation):
     @property
-    def allowed_actual_object_type_names(self) -> list[str]:
-        return [Account.get_type_name(), AWSAccount.get_type_name()]
+    def temporary(self) -> bool:
+        """Whether or not to use AWS' temporary credentials generation mechanism. The default value is False."""
+        return self.__temporary
 
+    @temporary.setter
+    def temporary(self, temporary: bool):
+        self.__temporary = bool(temporary)
 
+    def has_expired(self, exp_diff: int = 0, parse_pattern: Optional[str] = None):
+        """
+        This function assumes time will be provided in UTC per aws documentation
+        and that the expiration time is a datetime str.
+        :param exp_diff: the difference between expiration and current time in minutes (default to zero)
+        :param parse_pattern: is the pattern to parse for the expiration field (optional)
+        :return: a boolean whether the token has expired or not
+        :raise Value Error if expiration field cannot be parsed
+        """
+        parse_pattern = "%Y-%m-%dT%H:%M:%S%z" if not parse_pattern else parse_pattern
+        if not self.expiration:
+            #if not field not set allow credentials to generated to set it
+            return True
+        exp = datetime.strptime(self.expiration, parse_pattern)
+        diff = exp - datetime.now(timezone.utc)
+        return (diff.total_seconds() / 60) < exp_diff
 
-_validate_email = partial(validate_email, check_deliverability=False)
+    @property
+    def type_display_name(self) -> str:
+        return "AWS Credentials"
```

### Comparing `heaobject-1.5.1/src/heaobject/activity.py` & `heaobject-1.6.0/src/heaobject/activity.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.1/src/heaobject/aws.py` & `heaobject-1.6.0/src/heaobject/aws.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.1/src/heaobject/awss3key.py` & `heaobject-1.6.0/src/heaobject/awss3key.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.1/src/heaobject/bucket.py` & `heaobject-1.6.0/src/heaobject/bucket.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.1/src/heaobject/data.py` & `heaobject-1.6.0/src/heaobject/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,15 @@
             self.__key = key
 
     @property
     def display_name(self) -> str:
         """
         The object's display name. It's the last part of the object's key.
         It is computed from the key, and setting the display name updates the
-        key.
+        key. Passing a None value into this property does nothing.
         """
         key = self.key
         if key is not None and is_folder(key):
             key = key.strip('/')
         if key is not None:
             return key.rsplit('/', maxsplit=1)[-1]
         else:
```

### Comparing `heaobject-1.5.1/src/heaobject/dataadapter.py` & `heaobject-1.6.0/src/heaobject/dataadapter.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.1/src/heaobject/datamodel.py` & `heaobject-1.6.0/src/heaobject/datamodel.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.1/src/heaobject/folder.py` & `heaobject-1.6.0/src/heaobject/folder.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.1/src/heaobject/mimetype.py` & `heaobject-1.6.0/src/heaobject/mimetype.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.1/src/heaobject/person.py` & `heaobject-1.6.0/src/heaobject/person.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .root import AbstractDesktopObject, ShareImpl, Permission
 from typing import Optional
 from email_validator import validate_email, EmailNotValidError  # Leave this here for other modules to use
 from base64 import urlsafe_b64encode, urlsafe_b64decode
 from functools import partial
-
+from enum import Enum
 from .source import HEA
-from .user import NONE_USER, ALL_USERS, TEST_USER, SOURCE_USER, AWS_USER
+from .user import NONE_USER, ALL_USERS, TEST_USER, SOURCE_USER, AWS_USER, CREDENTIALS_MANAGER_USER
 
 
 class Person(AbstractDesktopObject):
     """
     Represents a Person
     """
 
@@ -21,14 +21,15 @@
         self.__first_name: Optional[str] = None
         self.__last_name: Optional[str] = None
         self.__title: Optional[str] = None
         self.__email: Optional[str] = None
         self.__phone_number: Optional[str] = None
         self.__display_name: str | None = None
         self.__overridden_display_name: str | None = None
+        self.__group_ids: list[str] = []
 
     @property
     def preferred_name(self) -> Optional[str]:
         """
         The Person's preferred name (Optional).
         """
         return self.__preferred_name
@@ -58,14 +59,18 @@
 
     @last_name.setter
     def last_name(self, last_name: Optional[str]) -> None:
         self.__last_name = str(last_name) if last_name is not None else None
         self.__update_display_name()
 
     @property
+    def full_name(self) -> str:
+        return self.display_name
+
+    @property
     def title(self) -> Optional[str]:
         """
           The Person's title (Optional).
         """
         return self.__title
 
     @title.setter
@@ -107,14 +112,33 @@
     def display_name(self, display_name: str) -> None:
         self.__overridden_display_name = display_name
 
     @property
     def type_display_name(self) -> str:
         return 'Person'
 
+    @property
+    def group_ids(self) -> list[str]:
+        return self.__group_ids.copy()
+
+    @group_ids.setter
+    def group_ids(self, group_ids: list[str]):
+        if group_ids is None:
+            self.__group_ids.clear()
+        elif not isinstance(group_ids, str):
+            self.__group_ids = [str(i) for i in group_ids]
+        else:
+            self.__group_ids = [str(group_ids)]
+
+    def add_group_id(self, group_id: str):
+        self.__group_ids.append(str(group_id))
+
+    def remove_group_id(self, group_id: str):
+        self.__group_ids.remove(str(group_id))
+
     def __update_display_name(self):
         fname = self.first_name if self.first_name else ""
         lname = self.last_name if self.last_name else ""
         if fname or lname:
             self.__display_name = f"{fname}{' ' if fname and lname else ''}{lname}"
         else:
             self.__display_name = None
@@ -181,24 +205,42 @@
     def display_name(self) -> str:
         return self.__display_name if self.__display_name is not None else super().display_name
 
     @display_name.setter
     def display_name(self, display_name: str):
         self.__display_name = str(display_name) if display_name is not None else None
 
+    @staticmethod
+    def id_to_role(id_: str) -> str:
+        """
+        Converts a Role id to a role.
+
+        :param id_: the role id.
+        :return: the role.
+        """
+        role = Role()
+        role.id = id_
+        return role.role
+
+class GroupType(Enum):
+    ADMIN = 10
+    ORGANIZATION = 20
+
 class Group(AbstractDesktopObject):
     """
     A user group, for authorization purposes. The id and name attributes are synchronized with the group attribute such
     that setting one automatically populates the others.
     """
     def __init__(self):
         super().__init__()
         self.__group: str | None = None
         self.__display_name: str | None = None
         self.__id: str | None = None
+        self.__role_ids: list[str] = []
+        self.__group_type = GroupType.ADMIN
 
     @property
     def id(self) -> str | None:
         """
         The group, base64-encoded using this module's encode_group() function. Setting this attribute automatically
         generates values for the name and group attributes.
         """
@@ -239,14 +281,44 @@
     def display_name(self) -> str:
         return self.__display_name if self.__display_name is not None else super().display_name
 
     @display_name.setter
     def display_name(self, display_name: str):
         self.__display_name = str(display_name) if display_name is not None else None
 
+    @property
+    def role_ids(self) -> list[str]:
+        return self.__role_ids.copy()
+
+    @role_ids.setter
+    def role_ids(self, role_ids: list[str]):
+        if role_ids is None:
+            self.__role_ids.clear()
+        elif not isinstance(role_ids, str):
+            self.__role_ids = [str(i) for i in role_ids]
+        else:
+            self.__role_ids = [str(role_ids)]
+
+    def add_role_id(self, role_id: str):
+        self.__role_ids.append(str(role_id))
+
+    def remove_role_id(self, role_id: str):
+        self.__role_ids.remove(str(role_id))
+
+    @property
+    def group_type(self) -> GroupType:
+        return self.__group_type
+
+    @group_type.setter
+    def group_type(self, group_type: GroupType):
+        if group_type is None:
+            self.__group_type = GroupType.ADMIN
+        else:
+            self.__group_type = group_type if isinstance(group_type, GroupType) else GroupType[group_type]
+
 
 def encode_role(role: str) -> str:
     """
     Encodes a role string using the Base 64 URL- and filesystem-safe alphabet, which replaces '+' with '-' and '/' with
     '_' in the base 64 alphabet as described in the IETF RFC 4648 specification section 5.
 
     :param role: the role string (required).
@@ -316,9 +388,10 @@
 _validate_email = partial(validate_email, check_deliverability=False)
 
 _system_user_display_names = {
     NONE_USER: 'None',
     ALL_USERS: 'All users',
     TEST_USER: 'Test user',
     SOURCE_USER: 'Source user',
-    AWS_USER: 'AWS account holder'
+    AWS_USER: 'AWS account holder',
+    CREDENTIALS_MANAGER_USER: 'Automatic credentials manager'
 }
```

### Comparing `heaobject-1.5.1/src/heaobject/project.py` & `heaobject-1.6.0/src/heaobject/project.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.1/src/heaobject/registry.py` & `heaobject-1.6.0/src/heaobject/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -329,101 +329,84 @@
         Removes a REST resource from the list of resources that are served by this component. Ignores None values.
         :param value: a Resource object.
         """
         if not isinstance(value, Resource):
             raise TypeError('value must be a Resource')
         self.__resources.remove(value)
 
-    def get_resource(self, type_name: str, file_system_name: Optional[str] = DEFAULT_FILE_SYSTEM) -> Resource | None:
+    def get_resource(self, type_name: str) -> Resource | None:
         """
         Returns the resource with the given type.
 
         :param type_name: a HEA object type or type name.
-        :param file_system_name: the unique name of a file system (or volume.DEFAULT_FILE_SYSTEM, or None, which
-        is the same as specifying volume.DEFAULT_FILE_SYSTEM)
         :return: a Resource, or None if this service does not serve resources of the given type.
         :raises ValueError: if type_name is not a valid HEA object type.
         """
         if not root.is_heaobject_type(type_name):
             raise ValueError('type_name not a type of HEAObject')
 
-        if file_system_name is None:
-            file_system_name_ = DEFAULT_FILE_SYSTEM
-        else:
-            file_system_name_ = str(file_system_name)
-
         for resource in self.__resources:
-            if type_name == resource.resource_type_name and file_system_name_ == resource.file_system_name:
+            if type_name == resource.resource_type_name:
                 return resource
         return None
 
-    def get_resource_url(self, type_name: str, file_system_name: Optional[str] = DEFAULT_FILE_SYSTEM,
+    def get_resource_url(self, type_name: str,
                          parameters: Optional[dict[str, Union[Sequence[Union[int, float, complex, str]], Mapping[str, Union[int, float, complex, str]], tuple[str, Union[int, float, complex, str]], int, float, complex, str]]] = None,
                          **kwargs: Union[Sequence[Union[int, float, complex, str]], Mapping[str, Union[int, float, complex, str]], tuple[str, Union[int, float, complex, str]], int, float, complex, str]) -> str | None:
         """
         Returns the base URL of resources of the given type. It constructs the
         URL by combining the base_url of the component with the base path
         provided in the Resource object corresponding to this type.
 
         :param type_name: a HEA object type or type name.
-        :param file_system_name: the unique name of a file system (or volume.DEFAULT_FILE_SYSTEM, or None, which
-        is the same as specifying volume.DEFAULT_FILE_SYSTEM)
         :param parameters: an optional dictionary of parameters for expanding the resource's base path.
         :param kwargs: alternative way of specifying parameters.
         :return: a URL string, or None if this service does not serve resources of the given type.
         :raises ValueError: if type_name is not a valid HEA object type.
         """
-        return self.__get_resource_url(self.base_url, type_name,
-                                       file_system_name, parameters, **kwargs)
+        return self.__get_resource_url(self.base_url, type_name, parameters, **kwargs)
 
-    def get_external_resource_url(self, type_name: str, file_system_name: Optional[str] = DEFAULT_FILE_SYSTEM,
+    def get_external_resource_url(self, type_name: str,
                          parameters: Optional[dict[str, Union[Sequence[Union[int, float, complex, str]], Mapping[str, Union[int, float, complex, str]], tuple[str, Union[int, float, complex, str]], int, float, complex, str]]] = None,
                          **kwargs: Union[Sequence[Union[int, float, complex, str]], Mapping[str, Union[int, float, complex, str]], tuple[str, Union[int, float, complex, str]], int, float, complex, str]) -> str | None:
         """
         Returns the external base URL of resources of the given type. It
         constructs the URL by combining the external_base_url of the component
         with the base path provided in the Resource object corresponding to
         this type.
 
         :param type_name: a HEA object type or type name.
-        :param file_system_name: the unique name of a file system (or
-        DEFAULT_FILE_SYSTEM, or None, which is the same as specifying
-        DEFAULT_FILE_SYSTEM)
         :param parameters: an optional dictionary of parameters for expanding
         the resource's base path.
         :param kwargs: alternative way of specifying parameters.
         :return: a URL string, or None if this service does not serve resources
         of the given type.
         :raises ValueError: if type_name is not a valid HEA object type.
         """
-        return self.__get_resource_url(self.external_base_url, type_name,
-                                       file_system_name, parameters, **kwargs)
+        return self.__get_resource_url(self.external_base_url, type_name, parameters, **kwargs)
 
     def __get_resource_url(self, base_url: str | None, type_name: str,
-                           file_system_name: Optional[str] = DEFAULT_FILE_SYSTEM,
                          parameters: Optional[dict[str, Union[Sequence[Union[int, float, complex, str]], Mapping[str, Union[int, float, complex, str]], tuple[str, Union[int, float, complex, str]], int, float, complex, str]]] = None,
                          **kwargs: Union[Sequence[Union[int, float, complex, str]], Mapping[str, Union[int, float, complex, str]], tuple[str, Union[int, float, complex, str]], int, float, complex, str]):
         """
         Constructs a REST resource URL from the given base URL and a
         base path from one of the component's Resource objects. The base path
         may contain URI template-style parameters.
 
         :param base_url: the base URL (required). If None, just the base path
         is used to construct a relative URL.
         :param type_name: the type name of the resource to use (required).
-        :param file_system_name: the file system name of the resource to use.
-        If None or omitted, DEFAULT_FILE_SYSTEM is used.
         :param parameters: If the base path has any URI template-style
         parameters, they will be substituted with the values in this mapping.
         :param kwargs: additional parameters may be specified as keyword
         arguments.
         :return a URL string, or None if no resource matched the type_name and
         file_system_name arguments.
         """
-        resource = self.get_resource(type_name, file_system_name)
+        resource = self.get_resource(type_name)
         parameters_ = dict(parameters or [])
         parameters_.update(kwargs)
         if resource is None:
             return None
         else:
             vars_ = uritemplate.variables(resource.base_path) if resource.base_path is not None else OrderedSet()
             if vars_ > parameters_.keys():
```

### Comparing `heaobject-1.5.1/src/heaobject/root.py` & `heaobject-1.6.0/src/heaobject/root.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.1/src/heaobject/settings.py` & `heaobject-1.6.0/src/heaobject/settings.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.1/src/heaobject/source2target.py` & `heaobject-1.6.0/src/heaobject/source2target.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.1/src/heaobject/storage.py` & `heaobject-1.6.0/src/heaobject/storage.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.1/src/heaobject/trash.py` & `heaobject-1.6.0/src/heaobject/trash.py`

 * *Files identical despite different names*

### Comparing `heaobject-1.5.1/src/heaobject/user.py` & `heaobject-1.6.0/src/heaobject/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 def is_system_user(id_: str) -> bool:
     """
     Returns whether the given ID is a system user or not.
 
     :param id_: The user ID to check.
     :return: True or False.
     """
-    return id_ in (NONE_USER, ALL_USERS, TEST_USER, SOURCE_USER, AWS_USER)
+    return id_ in (NONE_USER, ALL_USERS, TEST_USER, SOURCE_USER, AWS_USER, CREDENTIALS_MANAGER_USER)
```

### Comparing `heaobject-1.5.1/src/heaobject/volume.py` & `heaobject-1.6.0/src/heaobject/volume.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 microservice supports it, create a volume with the file_system_name set to DEFAULT_FILE_SYSTEM or None. Or use variants
 of the microservice's REST API calls that do not require passing in a volume id.
 
 """
 from abc import ABC
 from typing import Optional, TypeVar
 from . import root
-from .account import AccountAssociation
 from .data import DataObject, SameMimeType
+from .user import NONE_USER
+from .root import AbstractDesktopObject
 from copy import deepcopy
 
 
 class FileSystem(root.AbstractDesktopObject, ABC):
     """
     Represents a filesystem, which controls how data is stored and retrieved. In HEA, all filesystems are either
-    databases or network storage.
+    databases or other storage for REST resource persistence.
 
     File systems must have a name property that is unique per concrete FileSystem subclass. The name is typically a
     connection string, account id, or similar field.
     """
     def __new__(cls, *args, **kwargs):
         return root.make_abstract(FileSystem, cls, *args, **kwargs)
 
@@ -73,22 +74,36 @@
 class AWSFileSystem(FileSystem):
     """
     AWS-based file system. There can be at most one global AWS file system with name DEFAULT_FILE_SYSTEM, and users may
     have one volume for accessing their AWS account, with an association to a credentials object with the user's AWS
     key and secret.
     """
 
-    def __init__(self):
-        super().__init__()
-
     @property
     def type_display_name(self) -> str:
         return "AWS File System"
 
 
+class KeycloakFileSystem(FileSystem):
+    """
+    Keycloak file system. There can be at most one global Keycloak file system with name DEFAULT_FILE_SYSTEM.
+    """
+
+    @property
+    def type_display_name(self) -> str:
+        return "Keycloak File System"
+
+class MemoryFileSystem(FileSystem):
+    """
+    Represents in-memory desktop object storage.
+    """
+    @property
+    def type_display_name(self) -> str:
+        return "Memory File System"
+
 class Volume(DataObject, SameMimeType):
     """
     A single accessible storage area that stores a single filesystem. Some volumes may require providing credentials in
     order to access them.
     """
 
     @classmethod
@@ -97,15 +112,16 @@
 
     def __init__(self) -> None:
         super().__init__()
         self.__file_system_name = DEFAULT_FILE_SYSTEM
         self.__file_system_type = MongoDBFileSystem.get_type_name()
         self.__credential_id: Optional[str] = None
         self.__folder_id: Optional[str] = None
-        self.__account: AccountAssociation | None = None
+        self.__account_id: str | None = None
+        self.__credential_type_name: str | None = None
 
     @property
     def mime_type(self) -> str:
         return type(self).get_mime_type()
 
     @property  # type: ignore
     def folder_id(self) -> Optional[str]:
@@ -150,21 +166,27 @@
         return self.__credential_id
 
     @credential_id.setter  # type: ignore
     def credential_id(self, credentials_id: Optional[str]) -> None:
         self.__credential_id = str(credentials_id) if credentials_id is not None else None
 
     @property
-    def account(self) -> AccountAssociation | None:
-        return deepcopy(self.__account)
+    def credential_type_name(self) -> str | None:
+        return self.__credential_type_name
+
+    @credential_type_name.setter
+    def credential_type_name(self, credential_type_name: str | None):
+        self.__credential_type_name = str(credential_type_name) if credential_type_name is not None else None
+
+    @property
+    def account_id(self) -> str | None:
+        return self.__account_id
 
-    @account.setter
-    def account(self, account: AccountAssociation | None):
-        if account is not None and not isinstance(account, AccountAssociation):
-            raise TypeError('account must be a AccountAssociation')
-        self.__account = deepcopy(account) if account is not None else None
+    @account_id.setter
+    def account_id(self, account_id: str | None):
+        self.__account_id = str(account_id) if account_id is not None else None
 
     @property
     def type_display_name(self) -> str:
         return "Volume"
 
 DEFAULT_FILE_SYSTEM = 'DEFAULT_FILE_SYSTEM'
```

### Comparing `heaobject-1.5.1/src/heaobject.egg-info/PKG-INFO` & `heaobject-1.6.0/src/heaobject.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaobject
-Version: 1.5.1
+Version: 1.6.0
 Summary: Data and other classes that are passed into and out of HEA REST APIs.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,35 @@
 Requires-Dist: mimetype-description~=0.1.0
 
 # HEA Object Library
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Object Library contains data and other classes that are passed into and out of HEA REST APIs.
 
+## Version 1.6.0
+* Replaced heaobject.keychain.AWSCredentials role_arn attribute with a role attribute on heaobject.keychain.Credentials objects.
+* Added group_ids attribute to heaobject.person.Person.
+* New attributes in heaobject.account.Account: file_system_type, file_system_name.
+* New methods in heaobject.account.Account: get_role_to_assume(), and new_credentials().
+* Added full_name attribute to Person that is mirrors display_name.
+* Removed file_system_name parameter from queries of a registry Component's
+resources.
+* New heaobject.volume.Volume credential_type_name attribute.
+* Added role_ids attribute to heaobject.person.Group.
+* heaobject.user.is_system_user() now returns True for the system|credentialsmanager user.
+* Changed heaobject.organization.Organization.accounts to account_ids, which is
+a string, and removed the heaobject.account.AccountAssociation class.
+* Removed AWS-specific attributes and methods from heaobject.organization.Organization.
+* Docstring improvements.
+* Better default type_display_name for heaobject.account.AccountView objects.
+* Added group_type attribute to heaobject.person.Group.
+
+## Version 1.5.1
+* Ensure AWSS3FileObject's display_name attribute always has a non-None value.
+
 ## Version 1.5.0
 * Added attribute-level permissions.
 * Fixed bug in checking equality of AbstractAssociation objects.
 
 ## Version 1.4.0
 * Added "deleted" attribute to the trash module's TrashItem class.
 * Added Group class to the person module.
```

### Comparing `heaobject-1.5.1/src/heaobject.egg-info/SOURCES.txt` & `heaobject-1.6.0/src/heaobject.egg-info/SOURCES.txt`

 * *Files identical despite different names*

