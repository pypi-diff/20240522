# Comparing `tmp/contact_person_profile_csv_imp_local-0.0.8.tar.gz` & `tmp/contact_person_profile_csv_imp_local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_person_profile_csv_imp_local-0.0.8.tar", last modified: Tue May 14 20:50:52 2024, max compression
+gzip compressed data, was "contact_person_profile_csv_imp_local-0.0.9.tar", last modified: Sat May 18 08:12:33 2024, max compression
```

## Comparing `contact_person_profile_csv_imp_local-0.0.8.tar` & `contact_person_profile_csv_imp_local-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:50:52.304778 contact_person_profile_csv_imp_local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-14 20:50:52.304778 contact_person_profile_csv_imp_local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-14 20:50:12.000000 contact_person_profile_csv_imp_local-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:50:52.300778 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:50:52.304778 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)    50693 2024-05-14 20:50:12.000000 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local/src/CSVToContactPersonProfile.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:50:12.000000 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-05-14 20:50:12.000000 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:50:52.304778 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-14 20:50:52.000000 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-14 20:50:52.000000 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:50:52.000000 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-14 20:50:52.000000 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-14 20:50:52.000000 contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-14 20:50:12.000000 contact_person_profile_csv_imp_local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:50:52.304778 contact_person_profile_csv_imp_local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-14 20:50:12.000000 contact_person_profile_csv_imp_local-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 08:12:33.232741 contact_person_profile_csv_imp_local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-18 08:12:33.232741 contact_person_profile_csv_imp_local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1592 2024-05-18 08:11:53.000000 contact_person_profile_csv_imp_local-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 08:12:33.228741 contact_person_profile_csv_imp_local-0.0.9/contact_person_profile_csv_imp_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 08:12:33.232741 contact_person_profile_csv_imp_local-0.0.9/contact_person_profile_csv_imp_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)    50170 2024-05-18 08:11:53.000000 contact_person_profile_csv_imp_local-0.0.9/contact_person_profile_csv_imp_local/src/CSVToContactPersonProfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 08:11:53.000000 contact_person_profile_csv_imp_local-0.0.9/contact_person_profile_csv_imp_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-18 08:11:53.000000 contact_person_profile_csv_imp_local-0.0.9/contact_person_profile_csv_imp_local/src/contact_person_profile_csv_imp_local_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10655 2024-05-18 08:11:53.000000 contact_person_profile_csv_imp_local-0.0.9/contact_person_profile_csv_imp_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 08:12:33.232741 contact_person_profile_csv_imp_local-0.0.9/contact_person_profile_csv_imp_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-18 08:12:33.000000 contact_person_profile_csv_imp_local-0.0.9/contact_person_profile_csv_imp_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-18 08:12:33.000000 contact_person_profile_csv_imp_local-0.0.9/contact_person_profile_csv_imp_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 08:12:33.000000 contact_person_profile_csv_imp_local-0.0.9/contact_person_profile_csv_imp_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-18 08:12:33.000000 contact_person_profile_csv_imp_local-0.0.9/contact_person_profile_csv_imp_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-18 08:12:33.000000 contact_person_profile_csv_imp_local-0.0.9/contact_person_profile_csv_imp_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-18 08:11:53.000000 contact_person_profile_csv_imp_local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 08:12:33.232741 contact_person_profile_csv_imp_local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-18 08:11:53.000000 contact_person_profile_csv_imp_local-0.0.9/setup.py
```

### Comparing `contact_person_profile_csv_imp_local-0.0.8/PKG-INFO` & `contact_person_profile_csv_imp_local-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-person-profile-csv-imp-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles CSVToContactPersonProfile-local Local/Remote Python
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `contact_person_profile_csv_imp_local-0.0.8/README.md` & `contact_person_profile_csv_imp_local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local/src/CSVToContactPersonProfile.py` & `contact_person_profile_csv_imp_local-0.0.9/contact_person_profile_csv_imp_local/src/CSVToContactPersonProfile.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import csv
 import os
 import pycountry
 from phonenumbers import NumberParseException
 
+from .contact_person_profile_csv_imp_local_constants import CSVToContactPersonProfileConstants
+
 from contact_local.contact_local import ContactsLocal
 from database_mysql_local.generic_crud import GenericCRUD
-from logger_local.LoggerComponentEnum import LoggerComponentEnum
 from logger_local.LoggerLocal import Logger
 # from text_block_local.text_block import TextBlocks
 from user_context_remote.user_context import UserContext
 
 from contact_email_address_local.contact_email_addresses_local import ContactEmailAdressesLocal
 from contact_group_local.contact_group import ContactGroups
 from contact_local.contact_local import ContactsLocal
@@ -30,25 +31,16 @@
 from organizations_local.organizations_local import OrganizationsLocal
 from python_sdk_remote.utilities import our_get_env
 from url_remote import action_name_enum, component_name_enum, entity_name_enum
 from url_remote.url_circlez import OurUrl
 from user_context_remote.user_context import UserContext
 from user_external_local.user_externals_local import UserExternalsLocal
 
-CSV_LOCAL_PYTHON_COMPONENT_ID = 198
-CSV_LOCAL_PYTHON_COMPONENT_NAME = 'contact-person-profile-csv-imp-local-python-package'
-
-obj = {
-    'component_id': CSV_LOCAL_PYTHON_COMPONENT_ID,
-    'component_name': CSV_LOCAL_PYTHON_COMPONENT_NAME,
-    'component_category': LoggerComponentEnum.ComponentCategory.Code.value,
-    'developer_email': 'sahar.g.m@circ.zone'
-}
 
-logger = Logger.create_logger(object=obj)
+logger = Logger.create_logger(object=CSVToContactPersonProfileConstants.CSV_LOCAL_PYTHON_PACKAGE_CODE_LOGGER_OBJECT)
 user_context = UserContext()
 
 CLASS_NAME = "CSVToContactPersonProfile"
 CONTACT_PERSON_PROFILE_CSV_SYSTEM_ID = 1
 DEFAULT_LOCATION_ID = LocationLocalConstants.UNKNOWN_LOCATION_ID
 DEFAULT_PROFILE_ID = 0
 
@@ -106,17 +98,17 @@
 #     location_id, normalized_building_address_name = GroupsLocal.add_update_group_and_link_to_contact( location_id, is_street=true) # When checking if exists, ignore the upper-case lower-case, return the value with is_main == true
 
 # TODO def process_website
 
 
 class CSVToContactPersonProfile(GenericCRUD):
     def __init__(self, is_test_data: bool = False) -> None:
-        super().__init__(default_schema_name="field", default_id_column_name="field_id",
-                         default_table_name="field_table", default_view_table_name="field_view",
-                         is_test_data=is_test_data)
+        GenericCRUD.__init__(self, default_schema_name="field", default_id_column_name="field_id",
+                             default_table_name="field_table", default_view_table_name="field_view",
+                             is_test_data=is_test_data)
         self.contact_entity_type_id = GenericCRUD(default_schema_name="entity_type").select_one_value_by_id(
             view_table_name="entity_type_ml_en_view",
             select_clause_value="entity_type_id",
             id_column_name="entity_type_name",
             id_column_value="Contact"
         )
 
@@ -600,47 +592,38 @@
                 contact_id=contact_id, groups=groups)
         logger.end(object={"groups_linked": groups_linked})
         return groups_linked
 
     def __insert_link_contact_persons(self, contact_dict: dict, contact_id: int) -> int:
         logger.start(object={"contact_dict": contact_dict, "contact_id": contact_id})
         contact_persons = ContactPersonsLocal()
-        contact_person_id = contact_persons.insert_contact_and_link_to_existing_or_new_person(
+        contact_person_results_dict = contact_persons.insert_contact_and_link_to_existing_or_new_person(
             contact_dict=contact_dict,
             contact_email_address=contact_dict["email1"],
             contact_id=contact_id
         )
+        contact_person_id = contact_person_results_dict.get("contact_person_id")
         logger.end(object={"contact_person_id": contact_person_id})
         return contact_person_id
 
-    def __insert_link_contact_email_addresses(self, contact_dict, contact_id):
+    def __insert_link_contact_email_addresses(self, contact_dict, contact_id) -> list[int]:
         logger.start(object={"contact_dict": contact_dict, "contact_id": contact_id})
-        email1 = contact_dict.get("email1")
-        email2 = contact_dict.get("email2")
-        email3 = contact_dict.get("email3")
+        contacts_local = ContactsLocal()
+        email_addresses = contacts_local.get_contact_email_addresses_from_contact_dict(contact_dict=contact_dict)
         contact_email_addresses = ContactEmailAdressesLocal(is_test_data=self.is_test_data)
-        if email1:
-            contact_email_addresses.insert_contact_and_link_to_email_address(
-                contact_dict=contact_dict,
-                contact_email_address=email1,
-                contact_id=contact_id
-            )
-        if email2:
-            contact_email_addresses.insert_contact_and_link_to_email_address(
-                contact_dict=contact_dict,
-                contact_email_address=email2,
-                contact_id=contact_id
-            )
-        if email3:
-            contact_email_addresses.insert_contact_and_link_to_email_address(
+        contact_email_address_ids = []
+        for email_address in email_addresses:
+            contact_email_address_id = contact_email_addresses.insert_contact_and_link_to_email_address(
                 contact_dict=contact_dict,
-                contact_email_address=email3,
+                contact_email_address=email_address,
                 contact_id=contact_id
             )
-        logger.end()
+            contact_email_address_ids.append(contact_email_address_id)
+        logger.end(object={"contact_email_address_ids": contact_email_address_ids})
+        return contact_email_address_ids
 
     def __insert_link_contact_notes_and_text_blocks(
             self, contact_dict: dict, contact_id: int, profile_id: int) -> int or None:
         try:
             logger.start(object={"contact_dict": contact_dict, "contact_id": contact_id})
             if not contact_dict.get("notes"):
                 logger.end(log_message="contact_dict['notes'] is None")
@@ -655,39 +638,29 @@
             logger.end(object={"contact_note_id": contact_note_id})
             return contact_note_id
         except Exception as exception:
             logger.exception(log_message="Error while inserting to contact_notes and text_blocks",
                              object={"exception": exception})
             return None
 
-    def __insert_link_contact_phones(self, contact_dict: dict, contact_id: int):
+    def __insert_link_contact_phones(self, contact_dict: dict, contact_id: int) -> list[int]:
         logger.start(object={"contact_dict": contact_dict, "contact_id": contact_id})
-        phone1 = contact_dict.get("phone1")
-        phone2 = contact_dict.get("phone2")
-        phone3 = contact_dict.get("phone3")
-        contact_phones = ContactPhoneLocal()
-        if phone1:
-            contact_phones.insert_contact_and_link_to_existing_or_new_phone(
-                contact_dict=contact_dict,
-                phone_number=phone1,
-                contact_id=contact_id
-            )
-        if phone2:
-            contact_phones.insert_contact_and_link_to_existing_or_new_phone(
-                contact_dict=contact_dict,
-                phone_number=phone2,
-                contact_id=contact_id
-            )
-        if phone3:
-            contact_phones.insert_contact_and_link_to_existing_or_new_phone(
+        contacts_local = ContactsLocal()
+        contact_phone = ContactPhoneLocal()
+        phone_numbers = contacts_local.get_contact_phone_numbers_from_contact_dict(contact_dict=contact_dict)
+        contact_phone_ids = []
+        for phone_number in phone_numbers:
+            contact_phone_id = contact_phone.insert_contact_and_link_to_existing_or_new_phone(
                 contact_dict=contact_dict,
-                phone_number=phone3,
+                phone_number=phone_number,
                 contact_id=contact_id
             )
-        logger.end()
+            contact_phone_ids.append(contact_phone_id)
+        logger.end(object={"contact_phone_ids": contact_phone_ids})
+        return contact_phone_ids
 
     def __insert_link_contact_user_external(self, contact_dict: dict, contact_id: int) -> int:
         logger.start(object={"contact_dict": contact_dict, "contact_id": contact_id})
         contact_user_external = ContactUserExternalLocal()
         contact_user_external_id = contact_user_external.insert_contact_and_link_to_existing_or_new_user_external(
             contact_dict=contact_dict,
             contact_email_address=contact_dict["email1"],
```

### Comparing `contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local/src/utils.py` & `contact_person_profile_csv_imp_local-0.0.9/contact_person_profile_csv_imp_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `contact_person_profile_csv_imp_local-0.0.8/contact_person_profile_csv_imp_local.egg-info/PKG-INFO` & `contact_person_profile_csv_imp_local-0.0.9/contact_person_profile_csv_imp_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-person-profile-csv-imp-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles CSVToContactPersonProfile-local Local/Remote Python
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `contact_person_profile_csv_imp_local-0.0.8/pyproject.toml` & `contact_person_profile_csv_imp_local-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `contact_person_profile_csv_imp_local-0.0.8/setup.py` & `contact_person_profile_csv_imp_local-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = 'contact-person-profile-csv-imp-local'
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,
-    version='0.0.8',  # https://pypi.org/project/contact-person-profile-csv-imp-local/
+    version='0.0.9',  # https://pypi.org/project/contact-person-profile-csv-imp-local/
     author="Circles",
     author_email="info@circles.ai",
     description="PyPI Package for Circles CSVToContactPersonProfile-local Local/Remote Python",
     long_description="This is a package for sharing common XXX function used in different repositories",
     long_description_content_type="text/markdown",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
```

