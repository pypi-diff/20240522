# Comparing `tmp/zermelo_api_vogk-0.3.9.tar.gz` & `tmp/zermelo_api_vogk-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zermelo_api_vogk-0.3.9.tar", last modified: Tue Jan 16 14:50:00 2024, max compression
+gzip compressed data, was "zermelo_api_vogk-1.0.4.tar", last modified: Wed May 22 15:32:27 2024, max compression
```

## Comparing `zermelo_api_vogk-0.3.9.tar` & `zermelo_api_vogk-1.0.4.tar`

### file list

```diff
@@ -1,31 +1,33 @@
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-01-16 14:50:00.127700 zermelo_api_vogk-0.3.9/
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1068 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.9/LICENSE
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3333 2024-01-16 14:50:00.127700 zermelo_api_vogk-0.3.9/PKG-INFO
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     2784 2024-01-16 14:49:59.000000 zermelo_api_vogk-0.3.9/README.md
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-01-16 14:50:00.115700 zermelo_api_vogk-0.3.9/app/
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-01-16 14:50:00.115700 zermelo_api_vogk-0.3.9/app/zermelo_api/
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      442 2024-01-16 10:27:33.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/__init__.py
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-01-16 14:50:00.123700 zermelo_api_vogk-0.3.9/app/zermelo_api/src/
--rw-rw-r--   0 klaas     (1000) klaas     (1000)        0 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/__init__.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3019 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/appointments.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3465 2024-01-16 10:51:53.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/branches.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1437 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/config.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      644 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/credentials.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      941 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/groepen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1216 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/leerjaren.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     8415 2024-01-16 14:49:59.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/lesgroepen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1192 2024-01-09 09:30:53.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/logger.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      841 2024-01-16 10:27:33.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/lokalen.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      446 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/time_utils.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3696 2024-01-09 08:31:30.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/users.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     1941 2024-01-16 11:13:00.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/vakken.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     2159 2024-01-16 11:13:00.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/vaklokdoc.py
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     4256 2024-01-16 10:27:33.000000 zermelo_api_vogk-0.3.9/app/zermelo_api/src/zermelo_api.py
-drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-01-16 14:50:00.127700 zermelo_api_vogk-0.3.9/app/zermelo_api_vogk.egg-info/
--rw-rw-r--   0 klaas     (1000) klaas     (1000)     3333 2024-01-16 14:49:59.000000 zermelo_api_vogk-0.3.9/app/zermelo_api_vogk.egg-info/PKG-INFO
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      758 2024-01-16 14:49:59.000000 zermelo_api_vogk-0.3.9/app/zermelo_api_vogk.egg-info/SOURCES.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)        1 2024-01-16 14:49:59.000000 zermelo_api_vogk-0.3.9/app/zermelo_api_vogk.egg-info/dependency_links.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)       16 2024-01-16 14:49:59.000000 zermelo_api_vogk-0.3.9/app/zermelo_api_vogk.egg-info/requires.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)       12 2024-01-16 14:49:59.000000 zermelo_api_vogk-0.3.9/app/zermelo_api_vogk.egg-info/top_level.txt
--rw-rw-r--   0 klaas     (1000) klaas     (1000)       38 2024-01-16 14:50:00.127700 zermelo_api_vogk-0.3.9/setup.cfg
--rw-rw-r--   0 klaas     (1000) klaas     (1000)      875 2024-01-16 14:49:59.000000 zermelo_api_vogk-0.3.9/setup.py
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-22 15:32:27.789367 zermelo_api_vogk-1.0.4/
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1068 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.4/LICENSE
+-rw-r--r--   0 klaas     (1000) klaas     (1000)     3969 2024-05-22 15:32:27.785366 zermelo_api_vogk-1.0.4/PKG-INFO
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3397 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.4/README.md
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-22 15:32:27.769366 zermelo_api_vogk-1.0.4/app/
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-22 15:32:27.773366 zermelo_api_vogk-1.0.4/app/zermelo_api/
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      563 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/__init__.py
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-22 15:32:27.781366 zermelo_api_vogk-1.0.4/app/zermelo_api/src/
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)        0 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/__init__.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3138 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/appointments.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3771 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/branches.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1437 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/config.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      618 2024-05-17 10:07:35.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/credentials.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1556 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/groepen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      674 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/io_json.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1136 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/leerjaren.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     6089 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/lesgroepen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      812 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/lokalen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      446 2024-01-09 08:31:30.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/time_utils.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3786 2024-05-22 15:29:42.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/users.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1806 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/vakdoclok.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     2291 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/vakken.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     5831 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/vaklessen.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     3612 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/zermelo_api.py
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)     1523 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.4/app/zermelo_api/src/zermelo_collection.py
+drwxrwxr-x   0 klaas     (1000) klaas     (1000)        0 2024-05-22 15:32:27.785366 zermelo_api_vogk-1.0.4/app/zermelo_api_vogk.egg-info/
+-rw-r--r--   0 klaas     (1000) klaas     (1000)     3969 2024-05-22 15:32:27.000000 zermelo_api_vogk-1.0.4/app/zermelo_api_vogk.egg-info/PKG-INFO
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      834 2024-05-22 15:32:27.000000 zermelo_api_vogk-1.0.4/app/zermelo_api_vogk.egg-info/SOURCES.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)        1 2024-05-22 15:32:27.000000 zermelo_api_vogk-1.0.4/app/zermelo_api_vogk.egg-info/dependency_links.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)       15 2024-05-22 15:32:27.000000 zermelo_api_vogk-1.0.4/app/zermelo_api_vogk.egg-info/requires.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)       12 2024-05-22 15:32:27.000000 zermelo_api_vogk-1.0.4/app/zermelo_api_vogk.egg-info/top_level.txt
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)       38 2024-05-22 15:32:27.789367 zermelo_api_vogk-1.0.4/setup.cfg
+-rw-rw-r--   0 klaas     (1000) klaas     (1000)      874 2024-05-22 15:29:43.000000 zermelo_api_vogk-1.0.4/setup.py
```

### Comparing `zermelo_api_vogk-0.3.9/LICENSE` & `zermelo_api_vogk-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-0.3.9/PKG-INFO` & `zermelo_api_vogk-1.0.4/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,35 @@
-Metadata-Version: 2.1
-Name: zermelo_api_vogk
-Version: 0.3.9
-Summary: A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
-Home-page: https://github.com/KlaasVogel/zermelo_api_vogk
-Author: Klaas Vogel
-Author-email: zermelo_api@klaasvogel.nl
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE
-
 ## zermelo_api_vogk
 A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 
+# V1.0.4
+ - async loading lesgroepen done
+ - async loading appointments done
+
+# V1.0.2
+ - replacement of request for working with asyncio
+ - first rough test if asyncio is working
+ - TODO: refactor leerlingen (sort should be done later)
+ - loading branches seems done.
+ - Next check Lesgroepen en vakdocloks
+
+# V0.3.18
+ - better logging
+ - removed trace
+
+# V0.3.15
+ - changed vakdoclok from subjects to choosableindepartments
+
+# V0.3.10 - V0.3.14
+ - added VakDocLoks to __init__
+ - change of vakdocloks to raw data only
+ - bugfix filename vakdocloks
+ - testing choosablle_etc in vakdocloks
+ - wrong copy of code
+
 # V0.3.9
  - change lesgroepnaam
 
 # V0.3.5 -> V0.3.8
  - added lokalen, removed debug from zermelo_api
  - added vakdocloks
  - bugfix: added lokalen to dataclass of branch
```

### Comparing `zermelo_api_vogk-0.3.9/app/zermelo_api/src/appointments.py` & `zermelo_api_vogk-1.0.4/app/zermelo_api/src/appointments.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from .zermelo_api import zermelo, from_zermelo_dict
+from .zermelo_collection import from_zermelo_dict, ZermeloAPI
 from dataclasses import dataclass, InitVar, field
-from logger import makeLogger, DEBUG
-
-logger = makeLogger("APPS")
+import logging
 
+logger = logging.getLogger(__name__)
 
 @dataclass
 class Appointment:
     id: int
     appointmentInstance: int = 0
     start: int = 0
     end: int = 0
@@ -66,27 +65,31 @@
     #     query = f"appointments/{id}"
     #     status, data = zermelo.getData(query, from_id=True)
     #     if status != 200:
     #         raise Exception(data)
     #     return from_zermelo_dict(cls, data[0])
 
 
-def get_appointments(query: str) -> list[Appointment]:
+async def get_appointments(zermelo: ZermeloAPI, query: str) -> list[Appointment]:
     status, data = zermelo.getData(query)
     if status != 200:
         raise Exception(data)
     return [from_zermelo_dict(Appointment, row) for row in data]
 
 
-def get_user_appointments(user: int | str, **kwargs) -> list[Appointment]:
+async def get_user_appointments(
+    zermelo: ZermeloAPI, user: int | str, **kwargs
+) -> list[Appointment]:
     query = f"appointments/?user={user}"
     for key, val in kwargs.items():
         query += f"&{key}={val}"
     logger.debug(query)
-    return get_appointments(query)
+    return await get_appointments(zermelo, query)
 
 
-def get_department_updates(id: int, **kwargs) -> list[Appointment]:
+async def get_department_updates(
+    zermelo: ZermeloAPI, id: int, **kwargs
+) -> list[Appointment]:
     query = f"appointments/?containsStudentsFromGroupInDepartment={id}"
     for key, val in kwargs.items():
         query += f"&{key}={val}"
-    return get_appointments(query)
+    return await get_appointments(zermelo, query)
```

### Comparing `zermelo_api_vogk-0.3.9/app/zermelo_api/src/branches.py` & `zermelo_api_vogk-1.0.4/app/zermelo_api/src/branches.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,100 +1,107 @@
-from .logger import makeLogger
-from .zermelo_api import ZermeloCollection, zermelo, from_zermelo_dict
+from .zermelo_collection import ZermeloCollection, ZermeloAPI, from_zermelo_dict
 from .time_utils import get_date, get_year, datetime
-from .users import Leerling, Leerlingen, Personeel, Medewerker
-from .leerjaren import Leerjaren, Leerjaar
-from .groepen import Groep, Groepen
-from .lesgroepen import Lesgroepen, Lesgroep
-from .vakken import Vakken, Vak
-from .lokalen import Lokalen, Lokaal
-from .vaklokdoc import get_vakdocloks, VakDocLoks
-from dataclasses import dataclass, InitVar, field
-
-# branch is roughly translated to 'afdeling' in Dutch
-# for readability kept as branch, might be changed in the future
+from .users import Leerlingen, Personeel
+from .leerjaren import Leerjaren
+from .groepen import Groepen
+from .lesgroepen import Lesgroepen
+from .vakken import Vakken
+from .lokalen import Lokalen
 
-logger = makeLogger("BRANCH")
+# from .vakdoclok import get_vakdocloks, VakDocLoks
+from dataclasses import dataclass, InitVar, field
+import asyncio
+import logging
 
+logger = logging.getLogger(__name__)
+# logger.setLevel(logging.DEBUG)
 
 @dataclass
 class SchoolInSchoolYear:
     id: int
-    # school: int
-    # year: int
-    # archived: bool
-    # name: str
-    # projectName: str
-    # schoolName: str
-    # schoolHrmsCode: str
+    school: int
+    year: int
+    archived: bool
+    name: str
+    projectName: str
+    schoolName: str
+    schoolHrmsCode: str
 
 
 @dataclass
 class Branch:
+    zermelo: InitVar
     id: int
     schoolInSchoolYear: int
     branch: str
     name: str
     schoolYear: int
     date: datetime = datetime.now()
-    leerlingen: list[Leerling] = field(default_factory=list)
-    personeel: list[Medewerker] = field(default_factory=list)
-    leerjaren: list[Leerjaar] = field(default_factory=list)
+    leerlingen: Leerlingen = field(default_factory=list)
+    personeel: Personeel = field(default_factory=list)
+    leerjaren: Leerjaren = field(default_factory=list)
     vakken: Vakken = field(default_factory=list)
     groepen: Groepen = field(default_factory=list)
     lokalen: Lokalen = field(default_factory=list)
 
-    def __post_init__(self):
+    def __post_init__(self, zermelo: ZermeloAPI):
         logger.info(f"*** loading branch: {self.name} ***")
-        self.leerlingen = Leerlingen(self.schoolInSchoolYear)
-        self.personeel = Personeel(self.schoolInSchoolYear)
-        self.leerjaren = Leerjaren(self.schoolInSchoolYear)
-        self.groepen = Groepen(self.schoolInSchoolYear)
-        self.vakken = Vakken(self.schoolInSchoolYear)
-        self.lokalen = Lokalen(self.schoolInSchoolYear)
+        self.leerlingen = Leerlingen(zermelo, self.schoolInSchoolYear)
+        self.personeel = Personeel(zermelo, self.schoolInSchoolYear)
+        self.leerjaren = Leerjaren(zermelo, self.schoolInSchoolYear)
+        self.groepen = Groepen(zermelo, self.schoolInSchoolYear)
+        self.vakken = Vakken(zermelo, self.schoolInSchoolYear)
+        self.lokalen = Lokalen(zermelo, self.schoolInSchoolYear)
+
+    async def _init(self):
+        attrs = ["leerlingen", "personeel", "leerjaren", "groepen", "vakken", "lokalen"]
+        await asyncio.gather(*[getattr(self, name)._init() for name in attrs])
 
-    def find_lesgroepen(self) -> Lesgroepen | bool:
+    async def find_lesgroepen(self) -> Lesgroepen | bool:
         if self.leerlingen and self.personeel:
-            return Lesgroepen(
+            return await Lesgroepen.create(
                 self.leerjaren,
                 self.vakken,
                 self.groepen,
                 self.leerlingen,
                 self.personeel,
             )
         return False
 
-    def get_vak_doc_loks(self, start: int, eind: int) -> VakDocLoks:
-        return get_vakdocloks(
-            self.id,
-            self.vakken,
-            self.personeel,
-            self.lokalen,
-            start,
-            eind,
-        )
+    # def get_vak_doc_loks(self, start: int, eind: int) -> VakDocLoks:
+    #     return get_vakdocloks(self.id, start, eind)
 
 
 @dataclass
-class Branches(ZermeloCollection, list[Branch]):
-    datestring: InitVar = ""
+class Branches(ZermeloCollection[Branch]):
 
-    def __post_init__(self, datestring):
+    def __post_init__(self):
+        super().__post_init__()
+        self.type = Branch
+
+    async def _init(self, datestring):
         logger.debug("init branches")
         date = get_date(datestring)
         year = get_year(datestring)
         logger.debug(year)
         query = f"schoolsinschoolyears/?year={year}&archived=False"
-        data = zermelo.load_query(query)
+        data = await self.get_collection(query)
+        tasks = []
+
         for schoolrow in data:
             school = from_zermelo_dict(SchoolInSchoolYear, schoolrow)
             query = f"branchesofschools/?schoolInSchoolYear={school.id}"
-            self.load_collection(query, Branch)
-        for branch in self:
-            branch.date = date
+            tasks.append(
+                asyncio.create_task(
+                    self.load_collection(query, zermelo=self.zermelo, date=date)
+                )
+            )
+        await asyncio.gather(*tasks)
+        await asyncio.gather(*[branch._init() for branch in self])
+        logger.info(self)
 
     def __str__(self):
         return "Branches(" + ", ".join([br.name for br in self]) + ")"
 
     def get(self, name: str) -> Branch:
         logger.info(f"loading branch: {name} ")
         for branch in self:
```

### Comparing `zermelo_api_vogk-0.3.9/app/zermelo_api/src/config.py` & `zermelo_api_vogk-1.0.4/app/zermelo_api/src/config.py`

 * *Files identical despite different names*

### Comparing `zermelo_api_vogk-0.3.9/app/zermelo_api/src/leerjaren.py` & `zermelo_api_vogk-1.0.4/app/zermelo_api/src/leerjaren.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from .zermelo_api import ZermeloCollection
-from .logger import makeLogger
+from .zermelo_collection import ZermeloCollection
 from dataclasses import dataclass, InitVar
+import logging
 
-# Leerjaar is a rough dutch translation of department in Zermelo
-
-logger = makeLogger("Leerjaren")
+logger = logging.getLogger(__name__)
 
 
 def getLeerjaarNaam(string):
     names = {"LG1": "klas 1", "LG2": "klas 2", "LG3": "klas 3"}
     for name, result in names.items():
         if name in string:
             return result
@@ -36,13 +34,13 @@
     name: str = ""
 
     def __post_init__(self):
         self.name = getLeerjaarNaam(self.code.upper())
 
 
 @dataclass
-class Leerjaren(ZermeloCollection, list[Leerjaar]):
-    schoolinschoolyear: InitVar
+class Leerjaren(ZermeloCollection[Leerjaar]):
+    schoolinschoolyear: InitVar[int] = 0
 
     def __post_init__(self, schoolinschoolyear: int):
-        query = f"departmentsofbranches?schoolInSchoolYear={schoolinschoolyear}"
-        self.load_collection(query, Leerjaar)
+        self.query = f"departmentsofbranches?schoolInSchoolYear={schoolinschoolyear}"
+        self.type = Leerjaar
```

### Comparing `zermelo_api_vogk-0.3.9/app/zermelo_api/src/lesgroepen.py` & `zermelo_api_vogk-1.0.4/app/zermelo_api/src/lesgroepen.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,160 +1,29 @@
 from dataclasses import dataclass, field, InitVar
 from .vakken import Vakken, Vak
+from .vaklessen import get_groep_data, LesData
 from .groepen import Groepen, Groep
 from .users import Leerlingen, Leerling, Personeel, Medewerker
 from .leerjaren import Leerjaren, Leerjaar
-from .time_utils import get_date, delta_week
-from .logger import makeLogger, DEBUG
-from .zermelo_api import zermelo, from_zermelo_dict
+from .zermelo_collection import from_zermelo_dict
+import asyncio
+import logging
 
-# from typing import Tuple
-
-logger = makeLogger("LESGROEP")
+logger = logging.getLogger(__name__)
+# logger.setLevel(logging.DEBUG)
 
 
 def createLesgroepNaam(vak: Vak, groep: Groep) -> str:
     leerjaar, groepnaam = groep.extendedName.split(".")
     jaarnaam = leerjaar[2:].upper()
     if vak.subjectCode in groepnaam:
         return f"{jaarnaam}{groepnaam}"
     else:
         return f"{jaarnaam}{vak.subjectCode}{groepnaam[-1]}"
 
-
-def find_groepen(vak: Vak, groepen: Groepen) -> list[Groep]:
-    result = []
-    logger.debug(f"finding groep for vak: {vak.subjectCode}")
-    for groep in groepen.get_department_groups(vak.departmentOfBranch):
-        if groep in result:
-            continue
-        if vak.qualifiedCode and vak.qualifiedCode in groep.extendedName:
-            logger.debug(
-                f"found {groep.name} with {vak.qualifiedCode} in {groep.extendedName}"
-            )
-            result.append(groep)
-    return result
-
-
-def clean_docs(docs: list[str]) -> list[str]:
-    checklist = list(set(docs))
-    if "lgverv" in checklist:
-        checklist.remove("lgverv")
-    max = 0
-    if len(checklist) > 1:
-        logger.warning(f"multiple docs: {checklist}")
-        for doc in checklist:
-            doc_count = docs.count(doc)
-            if doc_count > max:
-                result = doc
-                max = doc_count
-        logger.warning(f"result: {result} ({max})")
-        return [result]
-    return checklist
-
-
-@dataclass
-class Les:
-    id: int
-    appointmentInstance: int
-    teachers: list[str]
-    students: list[str]
-    subjects: list[str]
-    groups: list[str]
-    groupsInDepartments: list[int]
-    choosableInDepartmentCodes: list[str]
-    valid: bool
-    cancelled: bool
-
-    def filter(self, name: str) -> bool:
-        if self.cancelled:
-            return False
-        if not self.valid:
-            return False
-        if len(self.students) > 40:
-            logger.debug("groep te groot")
-            return False
-        if not any([name.split(".")[-1] in group for group in self.groups]):
-            logger.debug(f"{name} not in {self}")
-            return False
-        return True
-
-
-def get_vak_data(
-    id: int, code: str, groupName: str, start, eind
-) -> tuple[list[int], list[str], list[str]]:
-    query = f"appointments/?containsStudentsFromGroupInDepartment={id}&subjects={code}&type=lesson&start={start}&end={eind}&fields=appointmentInstance,id,teachers,students,subjects,groups,groupsInDepartments,choosableInDepartmentCodes,valid,cancelled"
-    vakdata = zermelo.load_query(query)
-    grp_bck = []
-    ll_bck = []
-    doc_bck = []
-    leerlingen = []
-    docenten = []
-    grp_namen = []
-    lessen = [Les(**row) for row in reversed(vakdata) if row]
-    for les in [les for les in lessen if les.filter(groupName)]:
-        if len(les.groups) > 1:
-            if not grp_namen and not grp_bck or len(les.groups) < len(grp_bck):
-                logger.debug("meerdere groepen")
-                grp_bck = les.choosableInDepartmentCodes
-                ll_bck = list(set([llnr for llnr in les.students]))
-                doc_bck = list(set([doc for doc in les.teachers]))
-            continue
-        if les.students and les.teachers:
-            [leerlingen.append(llnr) for llnr in les.students if llnr not in leerlingen]
-            [docenten.append(doc) for doc in les.teachers]
-            [
-                grp_namen.append(grp)
-                for grp in les.choosableInDepartmentCodes
-                if grp not in grp_namen
-            ]
-    if not grp_namen and grp_bck:
-        logger.debug(f"result groepen: {grp_bck}")
-        grp_namen = grp_bck
-    if not docenten and doc_bck:
-        logger.debug(f"result docenten: {doc_bck}")
-        docenten = doc_bck
-    if not leerlingen and ll_bck:
-        logger.debug(f"result leerlingen: {ll_bck}")
-        leerlingen = ll_bck
-    docenten = clean_docs(docenten)
-    leerlingen = [int(llnr) for llnr in leerlingen]
-    return (leerlingen, docenten, grp_namen)
-
-
-def find_deelnemers(
-    vak: Vak, groep: Groep
-) -> tuple[list[int], list[str], list[str]] | bool:
-    date = get_date()
-    try:
-        logger.debug(groep)
-        for x in [0, -1, -2, 1, 2, 3]:
-            dweek = x * 4
-            starttijd = int(delta_week(date, dweek).timestamp())
-            eindtijd = int(delta_week(date, dweek + 4).timestamp())
-            data = get_vak_data(
-                groep.id, vak.subjectCode, groep.extendedName, starttijd, eindtijd
-            )
-            leerlingen, docenten, groep_namen = data
-            if len(leerlingen) and len(docenten):
-                logger.debug(f"found for {groep}")
-                namen = [
-                    groepnaam
-                    for groepnaam in groep_namen
-                    if vak.departmentOfBranchCode in groepnaam
-                ]
-                return (leerlingen, docenten, namen)
-        if not len(leerlingen) or not len(docenten):
-            logger.debug(f"geen deelnemers gevonden voor {groep}\n {vak}")
-            return False
-    except Exception:
-        logger.trace()
-        return False
-
-
 def get_info(
     llnrs: list[int],
     doc_codes: list[str],
     names: list[str],
     ll: Leerlingen,
     docs: Personeel,
 ) -> tuple[list[Leerling], list[Medewerker], list[str]]:
@@ -175,64 +44,130 @@
 
     def __post_init__(self):
         self.naam = createLesgroepNaam(self.vak, self.groep)
         for leerling in self.leerlingen:
             leerling.leerjaren.add(self.leerjaar.id)
 
 
-@dataclass
 class Lesgroepen(list[Lesgroep]):
-    leerjaren: InitVar
-    vakken: InitVar
-    groepen: InitVar
-    leerlingen: InitVar
-    personeel: InitVar
 
-    def __post_init__(
-        self,
+    @classmethod
+    async def create(
+        cls,
         leerjaren: Leerjaren,
         vakken: Vakken,
         groepen: Groepen,
         leerlingen: Leerlingen,
         personeel: Personeel,
     ):
+        self = cls()
         for leerjaar in leerjaren:
-            for vak in vakken.get_leerjaar_vakken(leerjaar.id):
-                if vak.subjectType in ["education", "profile"] or vak.scheduleCode in [
-                    "lo",
-                    "sport",
-                ]:
-                    # skip educatio / profile / lo
-                    continue
+            tasks1 = []
+            logger.info(f"finding lesgroepen for {leerjaar.code}")
+            for vak in vakken.get_leerjaar_vakken(leerjaar.id, skip=True):
                 logger.debug(vak)
-                found = False
-                for groep in find_groepen(vak, groepen):
-                    groepinfo = find_deelnemers(vak, groep)
-                    if groepinfo:
-                        data = get_info(*groepinfo, leerlingen, personeel)
-                        self.append(Lesgroep(vak, groep, leerjaar, *data))
-                        found = True
-                if found:
-                    continue
-                logger.debug(f"trying maingroups for {vak.subjectName}")
-                for groep in groepen.get_department_groups(
-                    vak.departmentOfBranch, True
-                ):
-                    logger.debug(f"trying: {groep}")
-                    groepinfo = find_deelnemers(vak, groep)
-                    if groepinfo:
-                        data = get_info(*groepinfo, leerlingen, personeel)
-                        self.append(Lesgroep(vak, groep, leerjaar, *data))
-                        found = True
-                if not found:
+                vakgroepen = groepen.get_vakgroepen(vak)
+                tasks1.append(
+                    asyncio.create_task(
+                        find_lesgroepen(
+                            leerjaar, vak, vakgroepen, leerlingen, personeel
+                        )
+                    )
+                )
+            results: list[tuple[Vak, list[Lesgroep]]] = await asyncio.gather(*tasks1)
+            tasks2 = []
+            for vak, lesgroepen in results:
+                self.extend(lesgroepen)
+                if not len(lesgroepen):
+                    logger.warning(vak)
+                    maingroepen = groepen.get_department_groups(leerjaar.id, True)
+                    tasks2.append(
+                        asyncio.create_task(
+                            find_lesgroepen(
+                                leerjaar, vak, maingroepen, leerlingen, personeel
+                            )
+                        )
+                    )
+            if not len(tasks2):
+                logger.debug("alle groepen gevonden.")
+                continue
+            results: list[tuple[Vak, list[Lesgroep]]] = await asyncio.gather(*tasks2)
+            for vak, lesgroepen in results:
+                self.extend(lesgroepen)
+                if not len(lesgroepen):
                     logger.warning(f"geen groepen gevonden voor {vak}")
         self.clean_leerlingen()
-        logger.info(f"found {len(self)} lesgroepen")
+        return self
 
     def clean_leerlingen(self):
         for lesgroep in self:
             for leerling in lesgroep.leerlingen.copy():
                 if leerling.leerjaren.get_id() != lesgroep.leerjaar.id:
                     logger.warning(
                         f"removing leerling ({leerling.fullName}) from {lesgroep.naam}"
                     )
                     lesgroep.leerlingen.remove(leerling)
+
+
+async def find_lesgroepen(
+    lj: Leerjaar,
+    vak: Vak,
+    grpn: list[Groep],
+    lln: Leerlingen,
+    docs: Personeel,
+) -> tuple[Vak, list[Lesgroep]]:
+    datalist = await asyncio.gather(
+        *[get_groep_data(lln.zermelo, vak, groep) for groep in grpn]
+    )
+    lesgroepen: list[Lesgroep] = []
+    for groep, lesdata in datalist:
+        if lesdata:
+            groepdata = get_info(*lesdata, lln, docs)
+            lesgroepen.append(Lesgroep(vak, groep, lj, *groepdata))
+    return (vak, lesgroepen)
+
+    # if not len(datalist):
+    #     datalist = await asyncio.gather(*[get_vakgroep_data(groepen.zermelo, vak, groep) for groep in groepen])
+
+
+# async def load_lesgroepen(leerjaar: Leerjaar, vak: Vak, groepen, ) -> Lesgroep:
+#     vakdata = await
+#     if vakdata:
+#         data =
+#         return
+
+#                 data = get_vak_data(
+
+#                 )
+#                  = data
+
+#             if not len(leerlingen) or not len(docenten):
+#                 logger.debug(f"geen deelnemers gevonden voor {groep}\n {vak}")
+#                 return False
+#         except Exception as e:
+#             logger.error(e)
+#             return False
+
+
+### uit lesgroepen:
+# groepinfo = await find_deelnemers(vak, groep)
+#                     if groepinfo:
+#                         data = get_info(*groepinfo, leerlingen, personeel)
+#                         self.append(Lesgroep(vak, groep, leerjaar, *data))
+#                         found = True
+#                 if found:
+#                     continue
+#                 logger.debug(f"trying maingroups for {vak.subjectName}")
+#                 for groep in groepen.get_department_groups(
+#                     vak.departmentOfBranch, True
+#                 ):
+#                     logger.debug(f"trying: {groep}")
+#                     groepinfo = find_deelnemers(vak, groep)
+#                     if groepinfo:
+#                         data = get_info(*groepinfo, leerlingen, personeel)
+#                         self.append(Lesgroep(vak, groep, leerjaar, *data))
+#                         found = True
+#                 if not found:
+#                     logger.warning(f"geen groepen gevonden voor {vak}")
+#         self.clean_leerlingen()
+#         logger.info(f"found {len(self)} lesgroepen")
+#         return self
```

### Comparing `zermelo_api_vogk-0.3.9/app/zermelo_api/src/users.py` & `zermelo_api_vogk-1.0.4/app/zermelo_api/src/users.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from .zermelo_api import ZermeloCollection, zermelo, from_zermelo_dict
-from .logger import makeLogger
+from .zermelo_collection import ZermeloCollection, from_zermelo_dict
 from dataclasses import dataclass, InitVar, field
+import logging
 
-logger = makeLogger("USERS")
+logger = logging.getLogger(__name__)
 
 
 @dataclass
 class User:
     code: str
     roles: list[str]
     firstName: str
@@ -81,20 +81,24 @@
 @dataclass
 class Leerling(User):
     volgnr: int = 0
     leerjaren: LeerjaarCounters = field(default_factory=LeerjaarCounters)
 
 
 @dataclass
-class Leerlingen(ZermeloCollection, Users, list[Leerling]):
-    schoolinschoolyear: InitVar
+class Leerlingen(Users, ZermeloCollection[Leerling]):
+    schoolinschoolyear: InitVar[int] = 0
 
-    def __init__(self, schoolinschoolyear: int):
-        query = f"users?schoolInSchoolYear={schoolinschoolyear}&isStudent=true"
-        data = zermelo.load_query(query)
+    def __post_init__(self, schoolinschoolyear: int):
+        super().__post_init__()
+        self.query = f"users?schoolInSchoolYear={schoolinschoolyear}&isStudent=true"
+        self.type = Leerling
+
+    async def _init(self):
+        data = await self.get_collection()
         if data:
             self.load_leerlingen(data)
 
     def load_leerlingen(self, data: list[dict]):
         logger.info("loading Leerlingen")
         data.sort(key=lambda x: (x["lastName"], x["firstName"]))
         for idx, row in enumerate(data):
@@ -116,20 +120,20 @@
 @dataclass
 class Medewerker(User):
     def __repr__(self):
         return self.fullName + f"({self.code})"
 
 
 @dataclass
-class Personeel(ZermeloCollection, Users, list[Medewerker]):
-    schoolinschoolyear: InitVar
+class Personeel(Users, ZermeloCollection[Medewerker]):
+    schoolinschoolyear: InitVar[int] = 0
 
-    def __init__(self, schoolinschoolyear: int):
-        query = f"users?schoolInSchoolYear={schoolinschoolyear}&isEmployee=true"
-        self.load_collection(query, Medewerker)
+    def __post_init__(self, schoolinschoolyear: int):
+        self.query = f"users?schoolInSchoolYear={schoolinschoolyear}&isEmployee=true"
+        self.type = Medewerker
 
     def __repr__(self):
         return f"{self}{self.print_list()}"
 
     def __str__(self):
         return f"Personeel({len(self)})"
```

### Comparing `zermelo_api_vogk-0.3.9/app/zermelo_api/src/vakken.py` & `zermelo_api_vogk-1.0.4/app/zermelo_api/src/vakken.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-from .zermelo_api import ZermeloCollection, zermelo
-from .logger import makeLogger, DEBUG
+from .zermelo_collection import ZermeloCollection
 from dataclasses import dataclass, InitVar, field
+import logging
 
-logger = makeLogger("VAKKEN")
+logger = logging.getLogger(__name__)
 
 
 @dataclass
 class Vak:
     id: int
     subject: int
     departmentOfBranch: int
@@ -37,28 +37,43 @@
             name = " ".join(nameparts)
             logger.debug(f"new name: {name}")
             return name.strip()
         return self.subjectName.strip()
 
 
 @dataclass
-class Vakken(ZermeloCollection, list[Vak]):
-    schoolinschoolyear: InitVar
+class Vakken(ZermeloCollection[Vak]):
+    schoolinschoolyear: InitVar[int] = 0
 
     def __post_init__(self, schoolinschoolyear: int):
-        query = f"choosableindepartments?schoolInSchoolYear={schoolinschoolyear}"
-        self.load_collection(query, Vak)
+        self.query = f"choosableindepartments?schoolInSchoolYear={schoolinschoolyear}"
+        self.type = Vak
 
     def get(self, vaknaam: str) -> Vak:
         for vak in self:
             if vak.subjectCode == vaknaam:
                 return vak
 
     def get_subject(self, subject: str) -> tuple[int, str]:
         """returns (code, naam)"""
         for vak in self:
             if vak.subjectCode == subject:
                 return (vak.subject, vak.getName())
         return (0, "Onbekend")
 
-    def get_leerjaar_vakken(self, leerjaar_id: int) -> list[Vak]:
-        return [vak for vak in self if vak.departmentOfBranch == leerjaar_id]
+    def get_leerjaar_vakken(self, leerjaar_id: int, skip: bool = False) -> list[Vak]:
+        return [
+            vak
+            for vak in self
+            if vak.departmentOfBranch == leerjaar_id
+            and not (
+                skip
+                and (
+                    vak.subjectType in ["education", "profile"]
+                    or vak.scheduleCode
+                    in [
+                        "lo",
+                        "sport",
+                    ]
+                )
+            )
+        ]
```

### Comparing `zermelo_api_vogk-0.3.9/app/zermelo_api/src/zermelo_api.py` & `zermelo_api_vogk-1.0.4/app/zermelo_api/src/zermelo_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,134 +1,107 @@
+from __future__ import annotations
 from .credentials import Credentials
-from .logger import makeLogger, DEBUG, INFO
+from .io_json import get_json, post_request
 import json
-import requests
-import inspect
+import logging
 
-logger = makeLogger("ZermeloAPI")
+logger = logging.getLogger(__name__)
 
-ZERMELO_NAME = "carmelhengelo"
+
+async def loadAPI(name: str) -> ZermeloAPI:
+    zermelo = ZermeloAPI(name)
+    if not await zermelo.checkCreds():
+        with open("creds.ini") as f:
+            token = f.read()
+            await zermelo.add_token(token)
+    return zermelo
 
 
 class ZermeloAPI:
-    def __init__(self, school=ZERMELO_NAME):
+    def __init__(self, school: str):
         self.credentials = Credentials()
         self.zerurl = f"https://{school}.zportal.nl/api/v3/"
 
     def login(self, code: str) -> bool:
         token = self.get_access_token(code)
         return self.add_token(token)
 
-    def get_access_token(self, code: str) -> str:
+    async def get_access_token(self, code: str) -> str:
         token = ""
         url = self.zerurl + "oauth/token"
-        # headers = {"Content-Type": "application/json"}
-        zerrequest = requests.post(
-            url, data={"grant_type": "authorization_code", "code": code}
-        )
+        data = {"grant_type": "authorization_code", "code": code}
+        response = await post_request(url, data)
+        logger.debug(response)
+        exit()
+
         if zerrequest.status_code == 200:
             data = json.loads(zerrequest.text)
             if "access_token" in data:
                 token = data["access_token"]
         return token
 
     def add_token(self, token: str) -> bool:
         if not token:
             return False
         self.credentials.settoken(token)
         return self.checkCreds()
 
-    def checkCreds(self):
-        result = False
+    async def checkCreds(self):
         try:
-            self.getName()
+            await self.getName()
             result = True
         except Exception as e:
-            logger.trace()
             logger.error(e)
+            result = False
         finally:
             return result
 
-    def getName(self):
+    async def getName(self):
         if not self.credentials.token:
             raise Exception("No Token loaded!")
-        status, data = self.getData("users/~me", True)
+        status, data = await self.getData("users/~me", True)
         if status != 200 or not len(data):
             raise Exception("could not load user data with token")
         logger.debug(f"get name: {data[0]}")
         row = data[0]
         if not row["prefix"]:
             return " ".join([row["firstName"], row["lastName"]])
         else:
             return " ".join([row["firstName"], row["prefix"], row["lastName"]])
 
-    def getData(self, task, from_id=False) -> tuple[int, list[dict] | str]:
-        result = (500, [])
+    async def getData(self, task, from_id=False) -> tuple[int, list[dict] | str]:
+        result = (500, "unknown error")
+        request = (
+            self.zerurl + task + f"?access_token={self.credentials.token}"
+            if from_id
+            else self.zerurl + task + f"&access_token={self.credentials.token}"
+        )
+        logger.debug(request)
         try:
-            request = (
-                self.zerurl + task + f"?access_token={self.credentials.token}"
-                if from_id
-                else self.zerurl + task + f"&access_token={self.credentials.token}"
-            )
-            logger.debug(request)
-            json_response = requests.get(request).json()
+            data1 = await get_json(request)
+            json_response = json.loads(data1.decode("utf-8"))
             if json_response:
                 json_status = json_response["response"]["status"]
                 if json_status == 200:
                     result = (200, json_response["response"]["data"])
                     logger.debug("    **** JSON OK ****")
                 else:
-                    logger.debug(
-                        f"oeps, geen juiste response: {task} - {json_response['response']}"
-                    )
-                    result = (json_status, json_response["response"])
+                    logger.debug(f"oeps, geen juiste response: {task}")
+                    result = (json_status, json_response["response"]["message"])
             else:
                 logger.error("JSON - response is leeg")
         except Exception as e:
-            logger.trace()
+            logger.error(e)
         finally:
             return result
 
-    def load_query(self, query: str) -> list[dict]:
+    async def load_query(self, query: str) -> list[dict]:
         try:
-            status, data = self.getData(query)
+            status, data = await self.getData(query)
             if status != 200:
-                raise Exception(f"Error loading data {status}")
+                raise Exception(f"Error loading data {status}, {data}")
             if not data:
                 logger.debug("no data")
         except Exception as e:
             logger.debug(e)
             data = []
         return data
-
-
-zermelo = ZermeloAPI()
-
-if not zermelo.checkCreds():
-    with open("creds.ini") as f:
-        token = f.read()
-        zermelo.add_token(token)
-
-
-def from_zermelo_dict(cls, data: dict, *args, **kwargs):
-    [
-        logger.debug(f"{k} ({v}) not defined in {cls}")
-        for k, v in data.items()
-        if k not in inspect.signature(cls).parameters
-    ]
-    return cls(
-        *args,
-        **{k: v for k, v in data.items() if k in inspect.signature(cls).parameters},
-        **kwargs,
-    )
-
-
-class ZermeloCollection:
-    def load_collection(self: list, query: str, type: object) -> None:
-        data = zermelo.load_query(query)
-        for row in data:
-            self.append(from_zermelo_dict(type, row))
-
-    def test(self: list, query: str):
-        data = zermelo.load_query(query)
-        for row in data:
-            logger.info(f"test: {row}")
```

### Comparing `zermelo_api_vogk-0.3.9/app/zermelo_api_vogk.egg-info/PKG-INFO` & `zermelo_api_vogk-1.0.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,52 @@
 Metadata-Version: 2.1
-Name: zermelo-api-vogk
-Version: 0.3.9
+Name: zermelo_api_vogk
+Version: 1.0.4
 Summary: A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 Home-page: https://github.com/KlaasVogel/zermelo_api_vogk
 Author: Klaas Vogel
 Author-email: zermelo_api@klaasvogel.nl
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
+Requires-Python: >=3.12
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
+Requires-Dist: aiohttp
+Provides-Extra: dev
 
 ## zermelo_api_vogk
 A small module to create a Zermelo accesstoken and put some data from Zermelo in dataclasses
 
+# V1.0.4
+ - async loading lesgroepen done
+ - async loading appointments done
+
+# V1.0.2
+ - replacement of request for working with asyncio
+ - first rough test if asyncio is working
+ - TODO: refactor leerlingen (sort should be done later)
+ - loading branches seems done.
+ - Next check Lesgroepen en vakdocloks
+
+# V0.3.18
+ - better logging
+ - removed trace
+
+# V0.3.15
+ - changed vakdoclok from subjects to choosableindepartments
+
+# V0.3.10 - V0.3.14
+ - added VakDocLoks to __init__
+ - change of vakdocloks to raw data only
+ - bugfix filename vakdocloks
+ - testing choosablle_etc in vakdocloks
+ - wrong copy of code
+
 # V0.3.9
  - change lesgroepnaam
 
 # V0.3.5 -> V0.3.8
  - added lokalen, removed debug from zermelo_api
  - added vakdocloks
  - bugfix: added lokalen to dataclass of branch
```

### Comparing `zermelo_api_vogk-0.3.9/app/zermelo_api_vogk.egg-info/SOURCES.txt` & `zermelo_api_vogk-1.0.4/app/zermelo_api_vogk.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 app/zermelo_api/__init__.py
 app/zermelo_api/src/__init__.py
 app/zermelo_api/src/appointments.py
 app/zermelo_api/src/branches.py
 app/zermelo_api/src/config.py
 app/zermelo_api/src/credentials.py
 app/zermelo_api/src/groepen.py
+app/zermelo_api/src/io_json.py
 app/zermelo_api/src/leerjaren.py
 app/zermelo_api/src/lesgroepen.py
-app/zermelo_api/src/logger.py
 app/zermelo_api/src/lokalen.py
 app/zermelo_api/src/time_utils.py
 app/zermelo_api/src/users.py
+app/zermelo_api/src/vakdoclok.py
 app/zermelo_api/src/vakken.py
-app/zermelo_api/src/vaklokdoc.py
+app/zermelo_api/src/vaklessen.py
 app/zermelo_api/src/zermelo_api.py
+app/zermelo_api/src/zermelo_collection.py
 app/zermelo_api_vogk.egg-info/PKG-INFO
 app/zermelo_api_vogk.egg-info/SOURCES.txt
 app/zermelo_api_vogk.egg-info/dependency_links.txt
 app/zermelo_api_vogk.egg-info/requires.txt
 app/zermelo_api_vogk.egg-info/top_level.txt
```

