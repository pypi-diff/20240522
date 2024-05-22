# Comparing `tmp/contact_email_address_local-0.0.8.tar.gz` & `tmp/contact_email_address_local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_email_address_local-0.0.8.tar", last modified: Tue May  7 23:38:38 2024, max compression
+gzip compressed data, was "contact_email_address_local-0.0.9.tar", last modified: Sun May 12 18:50:19 2024, max compression
```

## Comparing `contact_email_address_local-0.0.8.tar` & `contact_email_address_local-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:38.672177 contact_email_address_local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-07 23:38:38.672177 contact_email_address_local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-07 23:38:18.000000 contact_email_address_local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:38.668177 contact_email_address_local-0.0.8/contact_email_address_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:38.672177 contact_email_address_local-0.0.8/contact_email_address_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:18.000000 contact_email_address_local-0.0.8/contact_email_address_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-07 23:38:18.000000 contact_email_address_local-0.0.8/contact_email_address_local/src/contact_email_addresses_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5386 2024-05-07 23:38:18.000000 contact_email_address_local-0.0.8/contact_email_address_local/src/contact_email_addresses_local.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 23:38:38.672177 contact_email_address_local-0.0.8/contact_email_address_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-07 23:38:38.000000 contact_email_address_local-0.0.8/contact_email_address_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-07 23:38:38.000000 contact_email_address_local-0.0.8/contact_email_address_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 23:38:38.000000 contact_email_address_local-0.0.8/contact_email_address_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-07 23:38:38.000000 contact_email_address_local-0.0.8/contact_email_address_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-07 23:38:38.000000 contact_email_address_local-0.0.8/contact_email_address_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-07 23:38:18.000000 contact_email_address_local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 23:38:38.672177 contact_email_address_local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-07 23:38:18.000000 contact_email_address_local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 18:50:19.500664 contact_email_address_local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-12 18:50:19.500664 contact_email_address_local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-12 18:49:54.000000 contact_email_address_local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 18:50:19.500664 contact_email_address_local-0.0.9/contact_email_address_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 18:50:19.500664 contact_email_address_local-0.0.9/contact_email_address_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 18:49:54.000000 contact_email_address_local-0.0.9/contact_email_address_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-12 18:49:54.000000 contact_email_address_local-0.0.9/contact_email_address_local/src/contact_email_addresses_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5680 2024-05-12 18:49:54.000000 contact_email_address_local-0.0.9/contact_email_address_local/src/contact_email_addresses_local.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 18:50:19.500664 contact_email_address_local-0.0.9/contact_email_address_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-05-12 18:50:19.000000 contact_email_address_local-0.0.9/contact_email_address_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-12 18:50:19.000000 contact_email_address_local-0.0.9/contact_email_address_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 18:50:19.000000 contact_email_address_local-0.0.9/contact_email_address_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-12 18:50:19.000000 contact_email_address_local-0.0.9/contact_email_address_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-12 18:50:19.000000 contact_email_address_local-0.0.9/contact_email_address_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-12 18:49:54.000000 contact_email_address_local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 18:50:19.504664 contact_email_address_local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-12 18:49:54.000000 contact_email_address_local-0.0.9/setup.py
```

### Comparing `contact_email_address_local-0.0.8/PKG-INFO` & `contact_email_address_local-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-email-address-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles contact-email-address-local Python
 Home-page: https://github.com/circles-zone/contact-email-address-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact_email_address_local-0.0.8/contact_email_address_local/src/contact_email_addresses_constants.py` & `contact_email_address_local-0.0.9/contact_email_address_local/src/contact_email_addresses_constants.py`

 * *Files identical despite different names*

### Comparing `contact_email_address_local-0.0.8/contact_email_address_local/src/contact_email_addresses_local.py` & `contact_email_address_local-0.0.9/contact_email_address_local/src/contact_email_addresses_local.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,20 +20,21 @@
 
 class ContactEmailAdressesLocal(GenericMapping):
     def __init__(self, default_schema_name: str = DEFAULT_SCHEMA_NAME, default_entity_name1: str = DEFAULT_ENTITY_NAME1,
                  default_entity_name2: str = DEFAULT_ENTITY_NAME2, default_id_column_name: str = DEFAULT_ID_COLUMN_NAME,
                  default_table_name: str = DEFAULT_TABLE_NAME, default_view_table_name: str = DEFAULT_VIEW_TABLE_NAME,
                  lang_code: LangCode = None, is_test_data: bool = False) -> None:
 
-        super().__init__(default_schema_name=default_schema_name, default_entity_name1=default_entity_name1,
-                         default_entity_name2=default_entity_name2, default_id_column_name=default_id_column_name,
-                         default_table_name=default_table_name, default_view_table_name=default_view_table_name,
-                         is_test_data=is_test_data)
+        GenericMapping.__init__(
+            self,
+            default_schema_name=default_schema_name, default_entity_name1=default_entity_name1,
+            default_entity_name2=default_entity_name2, default_id_column_name=default_id_column_name,
+            default_table_name=default_table_name, default_view_table_name=default_view_table_name,
+            is_test_data=is_test_data)
         self.email_address_local = EmailAddressesLocal()
-        self.lang_code = lang_code or user_context.get_effective_profile_preferred_lang_code()
 
     def insert_contact_and_link_to_email_address(self, contact_dict: dict, contact_email_address: str,
                                                  contact_id: int) -> int or None:
         """
         Insert contact and link to existing or new email address
         :param contact_dict: contact_dict
         :param contact_email_address: contact_email_address
@@ -42,44 +43,51 @@
         """
         logger.start(object={"contact_dict": contact_dict, "contact_email_address": contact_email_address,
                              "contact_id": contact_id})
         if not contact_email_address:
             # TODO: we can try to look if there's an email address in the database by phone number
             # when contact-phones-local is done
             return None
+        lang_code = LangCode.detect_lang_code_str_restricted(
+            text=contact_email_address,
+            allowed_lang_codes=[LangCode.ENGLISH, LangCode.HEBREW],
+            default_lang_code=LangCode.ENGLISH
+        )
         email_address_id = self.email_address_local.get_email_address_id_by_email_address(
             email_address=contact_email_address)
         if not email_address_id:
             # Create a new  email address and add it to email_address_table and email_address_ml_table
             logger.info(log_message="email_address_id is None, creating a new email address and adding it to"
                                     " email_address_table and email_address_ml_table")
             first_name = contact_dict.get("first_name")
             last_name = contact_dict.get("last_name")
             name = f"{first_name} {last_name}"
             email_address_id = self.email_address_local.insert(email_address=contact_email_address,
-                                                               lang_code=self.lang_code,
+                                                               lang_code=lang_code,
                                                                name=name, is_test_data=self.is_test_data)
             if not email_address_id:
                 logger.error(log_message="email_address_id is None")
                 return None
             # Link contact to email address
             logger.info(log_message="Linking contact to email address")
             contact_email_address_id = self.insert_mapping(entity_name1=self.default_entity_name1,
                                                            entity_name2=self.default_entity_name2,
-                                                           entity_id1=contact_id, entity_id2=email_address_id)
+                                                           entity_id1=contact_id, entity_id2=email_address_id,
+                                                           ignore_duplicate=True)
         else:
             # check if there is link to existing email address
             logger.info(log_message="Linking contact to existing email address")
             mapping_tuple = self.select_multi_mapping_tuple_by_id(entity_name1=self.default_entity_name1,
                                                                   entity_name2=self.default_entity_name2,
                                                                   entity_id1=contact_id, entity_id2=email_address_id)
             if not mapping_tuple:
                 # Link contact to existing email address
                 logger.info(log_message="Linking contact to existing email address")
                 contact_email_address_id = self.insert_mapping(entity_name1=self.default_entity_name1,
                                                                entity_name2=self.default_entity_name2,
-                                                               entity_id1=contact_id, entity_id2=email_address_id)
+                                                               entity_id1=contact_id, entity_id2=email_address_id,
+                                                               ignore_duplicate=True)
             else:
                 logger.info(log_message="contact is already linked to email address")
                 contact_email_address_id = mapping_tuple[0]
         logger.end(object={"contact_email_address_id": contact_email_address_id})
         return contact_email_address_id
```

### Comparing `contact_email_address_local-0.0.8/contact_email_address_local.egg-info/PKG-INFO` & `contact_email_address_local-0.0.9/contact_email_address_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-email-address-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles contact-email-address-local Python
 Home-page: https://github.com/circles-zone/contact-email-address-local-python-package
 Author: Circles
 Author-email: info@circlez.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `contact_email_address_local-0.0.8/setup.py` & `contact_email_address_local-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "contact-email-address-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',  # https://pypi.org/project/contact-email-address-local/
+    version='0.0.9',  # https://pypi.org/project/contact-email-address-local/
     author="Circles",
     author_email="info@circlez.ai",
     description="PyPI Package for Circles contact-email-address-local Python",
     long_description="PyPI Package for Circles contact-email-address-local Python",
     long_description_content_type='text/markdown',
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
```

