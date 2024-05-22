# Comparing `tmp/tahrir_api-1.1.1.tar.gz` & `tmp/tahrir_api-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahrir_api-1.1.1.tar", max compression
+gzip compressed data, was "tahrir_api-1.1.2.tar", max compression
```

## Comparing `tahrir_api-1.1.1.tar` & `tahrir_api-1.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    35147 2024-05-19 06:52:35.625696 tahrir_api-1.1.1/LICENSE
--rw-r--r--   0        0        0     2510 2024-05-19 06:52:35.625696 tahrir_api-1.1.1/README.rst
--rw-r--r--   0        0        0      273 2024-05-19 06:52:35.625696 tahrir_api-1.1.1/examples/awardbadge.py
--rw-r--r--   0        0        0      519 2024-05-19 06:52:35.625696 tahrir_api-1.1.1/examples/fossboxbadge.py
--rw-r--r--   0        0        0     2266 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/__init__.py
--rw-r--r--   0        0        0    31012 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/dbapi.py
--rw-r--r--   0        0        0      154 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/migrations/README
--rw-r--r--   0        0        0      946 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/migrations/alembic.ini
--rw-r--r--   0        0        0     2121 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/migrations/env.py
--rw-r--r--   0        0        0      532 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/migrations/script.py.mako
--rw-r--r--   0        0        0      432 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/migrations/versions/139ec7ed17b7_add_a_rank_column_to.py
--rw-r--r--   0        0        0      445 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/migrations/versions/16943d9088cf_fix_foreign_key_mism.py
--rw-r--r--   0        0        0      609 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/migrations/versions/24282792d72a_add_created_by_field.py
--rw-r--r--   0        0        0      490 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/migrations/versions/2879ed5a6297_issued_for.py
--rw-r--r--   0        0        0      707 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/migrations/versions/39583332f4ea_add_profile_fields_t.py
--rw-r--r--   0        0        0     1037 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/migrations/versions/3c7fd5b4e2c2_add_two_new_columns_.py
--rw-r--r--   0        0        0      466 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/migrations/versions/3d3fb9e59e7b_add_person_avatar.py
--rw-r--r--   0        0        0      618 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/migrations/versions/4099fa344171_add_last_login.py
--rw-r--r--   0        0        0      507 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/migrations/versions/420c02357a1b_add_created_on_field.py
--rw-r--r--   0        0        0      510 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/migrations/versions/508367dcbbb5_add_an_stl_column_fo.py
--rw-r--r--   0        0        0      500 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/migrations/versions/5791a2b9fb6a_add_tags_field_to_ba.py
--rw-r--r--   0        0        0      735 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/migrations/versions/ce541796a7_add_authz_table.py
--rw-r--r--   0        0        0     2429 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/migrations/versions/e7040e76728_create_new_tables_for_quest.py
--rw-r--r--   0        0        0      526 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/migrations/versions/fa1d309e8c3_add_created_on_field.py
--rw-r--r--   0        0        0     9769 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/model.py
--rw-r--r--   0        0        0        0 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/scripts/__init__.py
--rw-r--r--   0        0        0     1711 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/scripts/populate_avatars.py
--rw-r--r--   0        0        0     2705 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/scripts/populateseries.py
--rw-r--r--   0        0        0      383 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/scripts/syncdb.py
--rw-r--r--   0        0        0     1443 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/scripts/utils.py
--rw-r--r--   0        0        0      838 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tahrir_api/utils.py
--rw-r--r--   0        0        0        0 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0      408 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tests/conftest.py
--rw-r--r--   0        0        0     5578 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tests/test_dbapi.py
--rw-r--r--   0        0        0     4909 2024-05-19 06:52:35.629696 tahrir_api-1.1.1/tests/test_ranking.py
--rw-r--r--   0        0        0     3937 1970-01-01 00:00:00.000000 tahrir_api-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35147 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2510 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/README.rst
+-rw-r--r--   0        0        0      273 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/examples/awardbadge.py
+-rw-r--r--   0        0        0      519 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/examples/fossboxbadge.py
+-rw-r--r--   0        0        0     2266 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/tahrir_api/__init__.py
+-rw-r--r--   0        0        0    31058 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/tahrir_api/dbapi.py
+-rw-r--r--   0        0        0      154 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/tahrir_api/migrations/README
+-rw-r--r--   0        0        0      946 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/tahrir_api/migrations/alembic.ini
+-rw-r--r--   0        0        0     2121 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/tahrir_api/migrations/env.py
+-rw-r--r--   0        0        0      532 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/tahrir_api/migrations/script.py.mako
+-rw-r--r--   0        0        0      432 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/tahrir_api/migrations/versions/139ec7ed17b7_add_a_rank_column_to.py
+-rw-r--r--   0        0        0      445 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/tahrir_api/migrations/versions/16943d9088cf_fix_foreign_key_mism.py
+-rw-r--r--   0        0        0      609 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/tahrir_api/migrations/versions/24282792d72a_add_created_by_field.py
+-rw-r--r--   0        0        0      490 2024-05-22 20:24:03.898796 tahrir_api-1.1.2/tahrir_api/migrations/versions/2879ed5a6297_issued_for.py
+-rw-r--r--   0        0        0      707 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/migrations/versions/39583332f4ea_add_profile_fields_t.py
+-rw-r--r--   0        0        0     1037 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/migrations/versions/3c7fd5b4e2c2_add_two_new_columns_.py
+-rw-r--r--   0        0        0      466 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/migrations/versions/3d3fb9e59e7b_add_person_avatar.py
+-rw-r--r--   0        0        0      618 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/migrations/versions/4099fa344171_add_last_login.py
+-rw-r--r--   0        0        0      507 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/migrations/versions/420c02357a1b_add_created_on_field.py
+-rw-r--r--   0        0        0      510 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/migrations/versions/508367dcbbb5_add_an_stl_column_fo.py
+-rw-r--r--   0        0        0      500 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/migrations/versions/5791a2b9fb6a_add_tags_field_to_ba.py
+-rw-r--r--   0        0        0      735 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/migrations/versions/ce541796a7_add_authz_table.py
+-rw-r--r--   0        0        0     2429 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/migrations/versions/e7040e76728_create_new_tables_for_quest.py
+-rw-r--r--   0        0        0      526 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/migrations/versions/fa1d309e8c3_add_created_on_field.py
+-rw-r--r--   0        0        0     9769 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/model.py
+-rw-r--r--   0        0        0        0 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/scripts/__init__.py
+-rw-r--r--   0        0        0     1711 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/scripts/populate_avatars.py
+-rw-r--r--   0        0        0     2705 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/scripts/populateseries.py
+-rw-r--r--   0        0        0      383 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/scripts/syncdb.py
+-rw-r--r--   0        0        0     1443 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/scripts/utils.py
+-rw-r--r--   0        0        0      838 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tahrir_api/utils.py
+-rw-r--r--   0        0        0        0 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      408 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     6156 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tests/test_dbapi.py
+-rw-r--r--   0        0        0     4909 2024-05-22 20:24:03.902796 tahrir_api-1.1.2/tests/test_ranking.py
+-rw-r--r--   0        0        0     3937 1970-01-01 00:00:00.000000 tahrir_api-1.1.2/PKG-INFO
```

### Comparing `tahrir_api-1.1.1/LICENSE` & `tahrir_api-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.1/README.rst` & `tahrir_api-1.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.1/examples/fossboxbadge.py` & `tahrir_api-1.1.2/examples/fossboxbadge.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.1/pyproject.toml` & `tahrir_api-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tahrir-api"
-version = "1.1.1"
+version = "1.1.2"
 description = "An API for interacting with the Tahrir database"
 
 license = "GPLv3+"
 
 authors = [
   "Ross Delinger <rdelinge@redhat.com>",
   "Fedora Infrastructure <admin@fedoraproject.org>",
```

### Comparing `tahrir_api-1.1.1/tahrir_api/dbapi.py` & `tahrir_api-1.1.2/tahrir_api/dbapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -644,18 +644,17 @@
         """
 
         if not self.badge_exists(badge_id):
             raise ValueError(f"No such badge {badge_id!r}")
 
         created_on = created_on or datetime.now(timezone.utc)
         expires_on = expires_on or (created_on + timedelta(hours=1))
-        if self.person_exists(email=created_by_email):
-            created_by = self.get_person(created_by_email).id
-        else:
-            created_by = self.session.query(Person).first().id
+        if not created_by_email or not self.person_exists(email=created_by_email):
+            raise ValueError(f"No user with email {created_by_email!r}. Ask them to login first.")
+        created_by = self.get_person(created_by_email).id
 
         invitation = Invitation(
             created_on=created_on,
             expires_on=expires_on,
             badge_id=badge_id,
             created_by=created_by,
         )
```

### Comparing `tahrir_api-1.1.1/tahrir_api/migrations/alembic.ini` & `tahrir_api-1.1.2/tahrir_api/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.1/tahrir_api/migrations/env.py` & `tahrir_api-1.1.2/tahrir_api/migrations/env.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.1/tahrir_api/migrations/script.py.mako` & `tahrir_api-1.1.2/tahrir_api/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.1/tahrir_api/migrations/versions/24282792d72a_add_created_by_field.py` & `tahrir_api-1.1.2/tahrir_api/migrations/versions/24282792d72a_add_created_by_field.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.1/tahrir_api/migrations/versions/39583332f4ea_add_profile_fields_t.py` & `tahrir_api-1.1.2/tahrir_api/migrations/versions/39583332f4ea_add_profile_fields_t.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.1/tahrir_api/migrations/versions/3c7fd5b4e2c2_add_two_new_columns_.py` & `tahrir_api-1.1.2/tahrir_api/migrations/versions/3c7fd5b4e2c2_add_two_new_columns_.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.1/tahrir_api/migrations/versions/4099fa344171_add_last_login.py` & `tahrir_api-1.1.2/tahrir_api/migrations/versions/4099fa344171_add_last_login.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.1/tahrir_api/migrations/versions/ce541796a7_add_authz_table.py` & `tahrir_api-1.1.2/tahrir_api/migrations/versions/ce541796a7_add_authz_table.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.1/tahrir_api/migrations/versions/e7040e76728_create_new_tables_for_quest.py` & `tahrir_api-1.1.2/tahrir_api/migrations/versions/e7040e76728_create_new_tables_for_quest.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.1/tahrir_api/migrations/versions/fa1d309e8c3_add_created_on_field.py` & `tahrir_api-1.1.2/tahrir_api/migrations/versions/fa1d309e8c3_add_created_on_field.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.1/tahrir_api/model.py` & `tahrir_api-1.1.2/tahrir_api/model.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.1/tahrir_api/scripts/populate_avatars.py` & `tahrir_api-1.1.2/tahrir_api/scripts/populate_avatars.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.1/tahrir_api/scripts/populateseries.py` & `tahrir_api-1.1.2/tahrir_api/scripts/populateseries.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.1/tahrir_api/scripts/utils.py` & `tahrir_api-1.1.2/tahrir_api/scripts/utils.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.1/tahrir_api/utils.py` & `tahrir_api-1.1.2/tahrir_api/utils.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.1/tests/test_dbapi.py` & `tahrir_api-1.1.2/tests/test_dbapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import pytest
+
+
 def test_add_badges(api):
     issuer_id = api.add_issuer("TestOrigin", "TestName", "TestOrg", "TestContact")
     api.add_badge(
         "TestBadge",
         "TestImage",
         "A test badge for doing unit tests",
         "TestCriteria",
@@ -72,17 +75,33 @@
     badge_id = api.add_badge(
         "TestBadge",
         "TestImage",
         "A test badge for doing unit tests",
         "TestCriteria",
         issuer_id,
     )
-    _id = api.add_invitation(badge_id)
+    _id = api.add_invitation(badge_id, created_by_email="test@tester.com")
 
     assert api.invitation_exists(_id)
+    invitation = api.get_invitation(_id)
+    assert api.get_person(id=invitation.created_by).email == "test@tester.com"
+
+
+def test_add_invitation_no_created_by(api):
+    issuer_id = api.add_issuer("TestOrigin", "TestName", "TestOrg", "TestContact")
+    api.add_person("test@tester.com")
+    badge_id = api.add_badge(
+        "TestBadge",
+        "TestImage",
+        "A test badge for doing unit tests",
+        "TestCriteria",
+        issuer_id,
+    )
+    with pytest.raises(ValueError):
+        api.add_invitation(badge_id)
 
 
 def test_last_login(api, callback_calls):
     email = "test@tester.com"
     person_id = api.add_person(email)
     person = api.get_person(person_id)
     assert not person.last_login
```

### Comparing `tahrir_api-1.1.1/tests/test_ranking.py` & `tahrir_api-1.1.2/tests/test_ranking.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.1.1/PKG-INFO` & `tahrir_api-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahrir-api
-Version: 1.1.1
+Version: 1.1.2
 Summary: An API for interacting with the Tahrir database
 Home-page: https://github.com/fedora-infra/tahrir-api
 License: GPLv3+
 Author: Ross Delinger
 Author-email: rdelinge@redhat.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Framework :: Pyramid
```

