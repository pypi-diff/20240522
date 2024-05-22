# Comparing `tmp/aleksis_app_kolego-0.1.0.dev0.tar.gz` & `tmp/aleksis_app_kolego-0.1.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_kolego-0.1.0.dev0.tar", max compression
+gzip compressed data, was "aleksis_app_kolego-0.1.0.dev1.tar", max compression
```

## Comparing `aleksis_app_kolego-0.1.0.dev0.tar` & `aleksis_app_kolego-0.1.0.dev1.tar`

### file list

```diff
@@ -1,31 +1,33 @@
--rw-r--r--   0        0        0      438 2023-05-27 11:23:59.633988 aleksis_app_kolego-0.1.0.dev0/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2023-05-27 11:23:59.645988 aleksis_app_kolego-0.1.0.dev0/LICENCE.rst
--rw-r--r--   0        0        0     1079 2023-05-27 11:23:59.653988 aleksis_app_kolego-0.1.0.dev0/README.rst
--rw-r--r--   0        0        0      152 2023-05-27 11:23:59.661988 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/__init__.py
--rw-r--r--   0        0        0      395 2023-10-18 17:01:15.467338 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/apps.py
--rw-r--r--   0        0        0     1388 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/frontend/components/AbsenceReasons.vue
--rw-r--r--   0        0        0     3989 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/frontend/components/Absences.vue
--rw-r--r--   0        0        0      380 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/frontend/components/Empty.vue
--rw-r--r--   0        0        0      738 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/frontend/components/absenceReasons.graphql
--rw-r--r--   0        0        0     1069 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/frontend/components/absences.graphql
--rw-r--r--   0        0        0       14 2023-05-27 11:23:59.669988 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/frontend/components/appName.graphql
--rw-r--r--   0        0        0      139 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/frontend/components/helper.graphql
--rw-r--r--   0        0        0       57 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/frontend/components/persons.graphql
--rw-r--r--   0        0        0      965 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/frontend/index.js
--rw-r--r--   0        0        0      468 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/frontend/messages/de.json
--rw-r--r--   0        0        0      435 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/frontend/messages/en.json
--rw-r--r--   0        0        0        0 2023-05-27 11:23:59.661988 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/locale/.keepdir
--rw-r--r--   0        0        0      400 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/managers.py
--rw-r--r--   0        0        0     3394 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/migrations/0001_initial.py
--rw-r--r--   0        0        0     1049 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/migrations/0002_drop_site.py
--rw-r--r--   0        0        0     1925 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/migrations/0003_refactor_absence.py
--rw-r--r--   0        0        0        0 2023-05-27 11:23:59.665988 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/migrations/__init__.py
--rw-r--r--   0        0        0       58 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/models/__init__.py
--rw-r--r--   0        0        0     2734 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/models/absence.py
--rw-r--r--   0        0        0     1940 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/rules.py
--rw-r--r--   0        0        0     1077 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/schema/__init__.py
--rw-r--r--   0        0        0     3935 2024-04-03 18:50:00.973813 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/schema/absence.py
--rw-r--r--   0        0        0        0 2023-05-27 11:23:59.661988 aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/static/.keepdir
--rw-r--r--   0        0        0     2446 2024-04-18 13:12:41.678603 aleksis_app_kolego-0.1.0.dev0/pyproject.toml
--rw-r--r--   0        0        0     2180 2023-12-29 17:36:22.268540 aleksis_app_kolego-0.1.0.dev0/tox.ini
--rw-r--r--   0        0        0     2051 1970-01-01 00:00:00.000000 aleksis_app_kolego-0.1.0.dev0/PKG-INFO
+-rw-r--r--   0        0        0      438 2023-05-27 11:23:59.633988 aleksis_app_kolego-0.1.0.dev1/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2023-05-27 11:23:59.645988 aleksis_app_kolego-0.1.0.dev1/LICENCE.rst
+-rw-r--r--   0        0        0     1079 2023-05-27 11:23:59.653988 aleksis_app_kolego-0.1.0.dev1/README.rst
+-rw-r--r--   0        0        0      152 2023-05-27 11:23:59.661988 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/__init__.py
+-rw-r--r--   0        0        0      395 2023-10-18 17:01:15.467338 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/apps.py
+-rw-r--r--   0        0        0     1211 2024-05-22 10:49:15.249655 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/frontend/components/AbsenceReasonChip.vue
+-rw-r--r--   0        0        0     2499 2024-05-22 10:49:15.249655 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/frontend/components/AbsenceReasonGroupSelect.vue
+-rw-r--r--   0        0        0     3381 2024-05-16 18:16:34.235665 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/frontend/components/AbsenceReasons.vue
+-rw-r--r--   0        0        0     4046 2024-05-16 18:16:34.235665 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/frontend/components/Absences.vue
+-rw-r--r--   0        0        0      380 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/frontend/components/Empty.vue
+-rw-r--r--   0        0        0      815 2024-05-16 18:16:34.235665 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/frontend/components/absenceReasons.graphql
+-rw-r--r--   0        0        0     1158 2024-05-16 18:16:34.235665 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/frontend/components/absences.graphql
+-rw-r--r--   0        0        0       14 2023-05-27 11:23:59.669988 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/frontend/components/appName.graphql
+-rw-r--r--   0        0        0      162 2024-05-16 18:16:34.235665 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/frontend/components/helper.graphql
+-rw-r--r--   0        0        0       57 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/frontend/components/persons.graphql
+-rw-r--r--   0        0        0      965 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/frontend/index.js
+-rw-r--r--   0        0        0      497 2024-05-16 18:16:34.235665 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/frontend/messages/de.json
+-rw-r--r--   0        0        0      604 2024-05-16 18:16:34.235665 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/frontend/messages/en.json
+-rw-r--r--   0        0        0        0 2023-05-27 11:23:59.661988 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/locale/.keepdir
+-rw-r--r--   0        0        0      400 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/managers.py
+-rw-r--r--   0        0        0     3394 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1049 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/migrations/0002_drop_site.py
+-rw-r--r--   0        0        0     1925 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/migrations/0003_refactor_absence.py
+-rw-r--r--   0        0        0        0 2023-05-27 11:23:59.665988 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/migrations/__init__.py
+-rw-r--r--   0        0        0       58 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/models/__init__.py
+-rw-r--r--   0        0        0     2734 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/models/absence.py
+-rw-r--r--   0        0        0     2095 2024-05-16 17:59:51.477424 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/rules.py
+-rw-r--r--   0        0        0     1077 2024-04-03 18:50:00.969813 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/schema/__init__.py
+-rw-r--r--   0        0        0     3814 2024-05-22 10:49:15.249655 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/schema/absence.py
+-rw-r--r--   0        0        0        0 2023-05-27 11:23:59.661988 aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/static/.keepdir
+-rw-r--r--   0        0        0     2446 2024-05-22 10:51:23.170527 aleksis_app_kolego-0.1.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0     2180 2023-12-29 17:36:22.268540 aleksis_app_kolego-0.1.0.dev1/tox.ini
+-rw-r--r--   0        0        0     2051 1970-01-01 00:00:00.000000 aleksis_app_kolego-0.1.0.dev1/PKG-INFO
```

### Comparing `aleksis_app_kolego-0.1.0.dev0/LICENCE.rst` & `aleksis_app_kolego-0.1.0.dev1/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_kolego-0.1.0.dev0/README.rst` & `aleksis_app_kolego-0.1.0.dev1/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/frontend/components/Absences.vue` & `aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/frontend/components/Absences.vue`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 <script setup>
+import AbsenceReasonChip from "./AbsenceReasonChip.vue";
 import InlineCRUDList from "aleksis.core/components/generic/InlineCRUDList.vue";
 import DateTimeField from "aleksis.core/components/generic/forms/DateTimeField.vue";
 </script>
 
 <template>
   <v-container>
     <inline-c-r-u-d-list
@@ -63,16 +64,15 @@
             required
             :rules="required"
           />
         </div>
       </template>
 
       <template #reason="{ item }">
-        <v-chip>{{ item.reason.shortName }}</v-chip
-        >&nbsp;
+        <absence-reason-chip :absence-reason="item.reason" short />
       </template>
       <!-- eslint-disable-next-line vue/valid-v-slot -->
       <template #reason.field="{ attrs, on }">
         <div aria-required="true">
           <v-autocomplete
             :items="absenceReasons"
             item-text="shortName"
```

### Comparing `aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/frontend/components/absenceReasons.graphql` & `aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/frontend/components/absenceReasons.graphql`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 query absenceReasons($orderBy: [String], $filters: JSONString) {
   items: absenceReasons(orderBy: $orderBy, filters: $filters) {
     id
     shortName
     name
+    colour
+    default
     canEdit
     canDelete
   }
 }
 
 mutation createAbsenceReasons($input: [BatchCreateAbsenceReasonInput]!) {
   createAbsenceReasons(input: $input) {
     items: absenceReasons {
       id
       shortName
       name
+      colour
+      default
       canEdit
       canDelete
     }
   }
 }
 
 mutation deleteAbsenceReasons($ids: [ID]!) {
@@ -28,12 +32,14 @@
 
 mutation updateAbsenceReasons($input: [BatchPatchAbsenceReasonInput]!) {
   updateAbsenceReasons(input: $input) {
     items: absenceReasons {
       id
       shortName
       name
+      colour
+      default
       canEdit
       canDelete
     }
   }
 }
```

### Comparing `aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/frontend/components/absences.graphql` & `aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/frontend/components/absences.graphql`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,16 @@
       id
       fullName
     }
     reason {
       id
       shortName
       name
+      colour
+      default
     }
     comment
     datetimeStart
     datetimeEnd
     canEdit
     canDelete
   }
@@ -26,14 +28,16 @@
         id
         fullName
       }
       reason {
         id
         shortName
         name
+        colour
+        default
       }
       comment
       datetimeStart
       datetimeEnd
       canEdit
       canDelete
     }
@@ -54,14 +58,16 @@
         id
         fullName
       }
       reason {
         id
         shortName
         name
+        colour
+        default
       }
       comment
       datetimeStart
       datetimeEnd
       canEdit
       canDelete
     }
```

### Comparing `aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/frontend/index.js` & `aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/frontend/index.js`

 * *Files identical despite different names*

### Comparing `aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/migrations/0001_initial.py` & `aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/migrations/0002_drop_site.py` & `aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/migrations/0002_drop_site.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/migrations/0003_refactor_absence.py` & `aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/migrations/0003_refactor_absence.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/models/absence.py` & `aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/models/absence.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/rules.py` & `aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/rules.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,7 +45,10 @@
 )
 rules.add_perm("kolego.edit_absencereason_rule", edit_absencereason_predicate)
 
 delete_absencereason_predicate = has_person & (
     has_global_perm("kolego.delete_absencereason") | has_object_perm("kolego.delete_absencereason")
 )
 rules.add_perm("kolego.delete_absencereason_rule", delete_absencereason_predicate)
+
+view_menu_predicate = has_person & (view_absences_predicate | view_absencereasons_predicate)
+rules.add_perm("kolego.view_menu_rule", view_menu_predicate)
```

### Comparing `aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/schema/__init__.py` & `aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_kolego-0.1.0.dev0/aleksis/apps/kolego/schema/absence.py` & `aleksis_app_kolego-0.1.0.dev1/aleksis/apps/kolego/schema/absence.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,30 @@
 from datetime import timezone
 
 from django.conf import settings
 
 from graphene_django.types import DjangoObjectType
-from graphene_django_cud.mutations import (
-    DjangoBatchCreateMutation,
-    DjangoBatchDeleteMutation,
-    DjangoBatchPatchMutation,
-)
 from guardian.shortcuts import get_objects_for_user
 from zoneinfo import ZoneInfo
 
 from aleksis.core.schema.base import (
+    BaseBatchCreateMutation,
+    BaseBatchDeleteMutation,
+    BaseBatchPatchMutation,
     DjangoFilterMixin,
-    PermissionBatchPatchMixin,
     PermissionsTypeMixin,
 )
 
 from ..models import Absence, AbsenceReason
 
 
 class AbsenceReasonType(PermissionsTypeMixin, DjangoFilterMixin, DjangoObjectType):
     class Meta:
         model = AbsenceReason
-        fields = ("id", "short_name", "name")
+        fields = ("id", "short_name", "name", "colour", "default")
         filter_fields = {
             "short_name": ["icontains", "exact"],
             "name": ["icontains", "exact"],
         }
 
     @classmethod
     def get_queryset(cls, queryset, info):
@@ -44,20 +41,20 @@
         }
 
     @classmethod
     def get_queryset(cls, queryset, info):
         return get_objects_for_user(info.context.user, "kolego.view_absence", queryset)
 
 
-class AbsenceBatchCreateMutation(DjangoBatchCreateMutation):
+class AbsenceBatchCreateMutation(BaseBatchCreateMutation):
     class Meta:
         model = Absence
         fields = ("person", "reason", "comment", "datetime_start", "datetime_end")
         optional_fields = ("comment", "reason")
-        permissions = ("kolego.add_absence",)  # FIXME
+        permissions = ("kolego.create_absence_rule",)
 
     @classmethod
     def handle_datetime_start(cls, value, name, info) -> int:
         value = value.replace(tzinfo=timezone.utc)
         return value
 
     @classmethod
@@ -68,25 +65,25 @@
     @classmethod
     def before_save(cls, root, info, input, obj):  # noqa: A002
         for absence in obj:
             absence.timezone = ZoneInfo(settings.TIME_ZONE)  # FIXME Use TZ provided by client
         return obj
 
 
-class AbsenceBatchDeleteMutation(DjangoBatchDeleteMutation):
+class AbsenceBatchDeleteMutation(BaseBatchDeleteMutation):
     class Meta:
         model = Absence
-        permission_required = "kolego.delete_absence"  # FIXME
+        permissions = ("kolego.delete_absence_rule",)
 
 
-class AbsenceBatchPatchMutation(PermissionBatchPatchMixin, DjangoBatchPatchMutation):
+class AbsenceBatchPatchMutation(BaseBatchPatchMutation):
     class Meta:
         model = Absence
         fields = ("id", "person", "reason", "comment", "datetime_start", "datetime_end")
-        permissions = ("kolego.change_absence",)  # FIXME
+        permissions = ("kolego.edit_absence_rule",)
 
     @classmethod
     def handle_datetime_start(cls, value, name, info) -> int:
         value = value.replace(tzinfo=timezone.utc)
         return value
 
     @classmethod
@@ -97,26 +94,26 @@
     @classmethod
     def before_save(cls, root, info, input, obj):  # noqa: A002
         for absence in obj:
             absence.timezone = ZoneInfo(settings.TIME_ZONE)  # FIXME Use TZ provided by client
         return obj
 
 
-class AbsenceReasonBatchCreateMutation(DjangoBatchCreateMutation):
+class AbsenceReasonBatchCreateMutation(BaseBatchCreateMutation):
     class Meta:
         model = AbsenceReason
-        fields = ("short_name", "name")
+        fields = ("short_name", "name", "colour", "default")
         optional_fields = ("name",)
-        permissions = ("kolego.create_absencereason",)  # FIXME
+        permissions = ("kolego.create_absencereason_rule",)
 
 
-class AbsenceReasonBatchDeleteMutation(DjangoBatchDeleteMutation):
+class AbsenceReasonBatchDeleteMutation(BaseBatchDeleteMutation):
     class Meta:
         model = AbsenceReason
-        permission_required = "kolego.delete_absencereason"  # FIXME
+        permissions = ("kolego.delete_absencereason_rule",)
 
 
-class AbsenceReasonBatchPatchMutation(PermissionBatchPatchMixin, DjangoBatchPatchMutation):
+class AbsenceReasonBatchPatchMutation(BaseBatchPatchMutation):
     class Meta:
         model = AbsenceReason
-        fields = ("id", "short_name", "name")
-        permissions = ("kolego.change_absencereason",)  # FIXME
+        fields = ("id", "short_name", "name", "colour", "default")
+        permissions = ("kolego.edit_absencereason_rule",)
```

### Comparing `aleksis_app_kolego-0.1.0.dev0/pyproject.toml` & `aleksis_app_kolego-0.1.0.dev1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Kolego"
-version = "0.1.0.dev0"
+version = "0.1.0.dev1"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
@@ -31,15 +31,15 @@
 [[tool.poetry.source]]
 name = "gitlab"
 url = "https://edugit.org/api/v4/projects/461/packages/pypi/simple"
 priority = "supplemental"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-aleksis-core = "^4.0.0.dev2"
+aleksis-core = "^4.0.0.dev9"
 
 [tool.poetry.plugins."aleksis.app"]
 kolego = "aleksis.apps.kolego.apps:DefaultConfig"
 
 
 [tool.poetry.group.dev.dependencies]
 django-stubs = "^4.2"
```

### Comparing `aleksis_app_kolego-0.1.0.dev0/tox.ini` & `aleksis_app_kolego-0.1.0.dev1/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_app_kolego-0.1.0.dev0/PKG-INFO` & `aleksis_app_kolego-0.1.0.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AlekSIS-App-Kolego
-Version: 0.1.0.dev0
+Version: 0.1.0.dev1
 Summary: AlekSIS (School Information System) — App Kolego (Staff Management)
 Home-page: https://aleksis.org
 License: EUPL-1.2-or-later
 Author: Jonathan Weth
 Author-email: dev@jonathanweth.de
 Maintainer: Jonathan Weth
 Maintainer-email: dev@jonathanweth.de
@@ -13,15 +13,15 @@
 Classifier: Intended Audience :: Education
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Education
-Requires-Dist: aleksis-core (>=4.0.0.dev2,<5.0.0)
+Requires-Dist: aleksis-core (>=4.0.0.dev9,<5.0.0)
 Project-URL: Documentation, https://aleksis.org/official/AlekSIS/docs/html/
 Project-URL: Repository, https://edugit.org/AlekSIS/onboarding//AlekSIS-App-Kolego
 Description-Content-Type: text/x-rst
 
 AlekSIS (School Information System) — App Kolego (Staff Management)
 ==================================================================================================
```

