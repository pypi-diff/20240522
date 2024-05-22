# Comparing `tmp/edm_arch-1.0.41.tar.gz` & `tmp/edm_arch-1.0.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\mcpherro\Local\Source\Python3\edmpy\dist\.tmp-cj341jsy\edm_arch-1.0.41.tar", last modified: Tue May 21 12:46:36 2024, max compression
+gzip compressed data, was "C:\Users\mcpherro\Local\Source\Python3\edmpy\dist\.tmp-olnn701_\edm_arch-1.0.42.tar", last modified: Wed May 22 13:47:14 2024, max compression
```

## Comparing `edm_arch-1.0.41.tar` & `edm_arch-1.0.42.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 12:46:36.267487 edm_arch-1.0.41/
--rw-rw-rw-   0        0        0     1096 2022-06-07 20:35:30.000000 edm_arch-1.0.41/LICENSE
--rw-rw-rw-   0        0        0    22209 2024-05-21 12:46:36.267487 edm_arch-1.0.41/PKG-INFO
--rw-rw-rw-   0        0        0    20836 2024-05-21 12:46:17.000000 edm_arch-1.0.41/README.md
--rw-rw-rw-   0        0        0      523 2023-05-11 08:29:35.000000 edm_arch-1.0.41/pyproject.toml
--rw-rw-rw-   0        0        0     1277 2024-05-21 12:46:36.270488 edm_arch-1.0.41/setup.cfg
--rw-rw-rw-   0        0        0       73 2022-06-16 14:04:21.000000 edm_arch-1.0.41/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:46:36.210750 edm_arch-1.0.41/src/
-drwxrwxrwx   0        0        0        0 2024-05-21 12:46:36.263487 edm_arch-1.0.41/src/edm_arch.egg-info/
--rw-rw-rw-   0        0        0    22209 2024-05-21 12:46:36.000000 edm_arch-1.0.41/src/edm_arch.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      653 2024-05-21 12:46:36.000000 edm_arch-1.0.41/src/edm_arch.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 12:46:36.000000 edm_arch-1.0.41/src/edm_arch.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-06-22 11:44:30.000000 edm_arch-1.0.41/src/edm_arch.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      182 2024-05-21 12:46:36.000000 edm_arch-1.0.41/src/edm_arch.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-21 12:46:36.000000 edm_arch-1.0.41/src/edm_arch.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-21 12:46:36.251485 edm_arch-1.0.41/src/edmpy/
--rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm_arch-1.0.41/src/edmpy/__init__.py
--rw-rw-rw-   0        0        0       79 2022-06-21 13:54:13.000000 edm_arch-1.0.41/src/edmpy/__main__.py
--rw-rw-rw-   0        0        0    28555 2023-12-06 09:35:46.000000 edm_arch-1.0.41/src/edmpy/cfg.py
--rw-rw-rw-   0        0        0     2125 2023-12-04 13:37:08.000000 edm_arch-1.0.41/src/edmpy/constants.py
--rw-rw-rw-   0        0        0     5450 2023-12-06 09:37:10.000000 edm_arch-1.0.41/src/edmpy/db.py
--rw-rw-rw-   0        0        0    13431 2023-12-05 09:27:43.000000 edm_arch-1.0.41/src/edmpy/edm.kv
--rw-rw-rw-   0        0        0   126055 2024-05-21 12:42:03.000000 edm_arch-1.0.41/src/edmpy/edm.py
--rw-rw-rw-   0        0        0     5653 2024-04-18 08:18:35.000000 edm_arch-1.0.41/src/edmpy/geo.py
--rw-rw-rw-   0        0        0     2495 2023-12-06 09:36:13.000000 edm_arch-1.0.41/src/edmpy/ini.py
-drwxrwxrwx   0        0        0        0 2024-05-21 12:46:36.261486 edm_arch-1.0.41/src/edmpy/lib/
--rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm_arch-1.0.41/src/edmpy/lib/__init__.py
--rw-rw-rw-   0        0        0     4204 2023-12-04 14:38:01.000000 edm_arch-1.0.41/src/edmpy/lib/blockdata.py
--rw-rw-rw-   0        0        0     4333 2023-12-06 09:31:45.000000 edm_arch-1.0.41/src/edmpy/lib/colorscheme.py
--rw-rw-rw-   0        0        0     3994 2023-12-04 14:40:09.000000 edm_arch-1.0.41/src/edmpy/lib/dbs.py
--rw-rw-rw-   0        0        0   195805 2024-05-21 12:29:02.000000 edm_arch-1.0.41/src/edmpy/lib/e5_widgets.py
--rw-rw-rw-   0        0        0     1812 2023-12-04 14:41:01.000000 edm_arch-1.0.41/src/edmpy/lib/misc.py
--rw-rw-rw-   0        0        0        0 2022-06-07 20:43:53.000000 edm_arch-1.0.41/src/edmpy/py.typed
--rw-rw-rw-   0        0        0      531 2024-04-16 00:42:15.000000 edm_arch-1.0.41/src/edmpy/test_edm.py
--rw-rw-rw-   0        0        0    46620 2024-04-18 08:16:59.000000 edm_arch-1.0.41/src/edmpy/totalstation.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:14.537700 edm_arch-1.0.42/
+-rw-rw-rw-   0        0        0     1096 2022-06-07 20:35:30.000000 edm_arch-1.0.42/LICENSE
+-rw-rw-rw-   0        0        0    23114 2024-05-22 13:47:14.536700 edm_arch-1.0.42/PKG-INFO
+-rw-rw-rw-   0        0        0    21741 2024-05-22 13:45:45.000000 edm_arch-1.0.42/README.md
+-rw-rw-rw-   0        0        0      523 2023-05-11 08:29:35.000000 edm_arch-1.0.42/pyproject.toml
+-rw-rw-rw-   0        0        0     1277 2024-05-22 13:47:14.538700 edm_arch-1.0.42/setup.cfg
+-rw-rw-rw-   0        0        0       73 2022-06-16 14:04:21.000000 edm_arch-1.0.42/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:14.498896 edm_arch-1.0.42/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:14.535672 edm_arch-1.0.42/src/edm_arch.egg-info/
+-rw-rw-rw-   0        0        0    23114 2024-05-22 13:47:14.000000 edm_arch-1.0.42/src/edm_arch.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      653 2024-05-22 13:47:14.000000 edm_arch-1.0.42/src/edm_arch.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 13:47:14.000000 edm_arch-1.0.42/src/edm_arch.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-06-22 11:44:30.000000 edm_arch-1.0.42/src/edm_arch.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      182 2024-05-22 13:47:14.000000 edm_arch-1.0.42/src/edm_arch.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-22 13:47:14.000000 edm_arch-1.0.42/src/edm_arch.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:14.528516 edm_arch-1.0.42/src/edmpy/
+-rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm_arch-1.0.42/src/edmpy/__init__.py
+-rw-rw-rw-   0        0        0       79 2022-06-21 13:54:13.000000 edm_arch-1.0.42/src/edmpy/__main__.py
+-rw-rw-rw-   0        0        0    28555 2023-12-06 09:35:46.000000 edm_arch-1.0.42/src/edmpy/cfg.py
+-rw-rw-rw-   0        0        0     2125 2023-12-04 13:37:08.000000 edm_arch-1.0.42/src/edmpy/constants.py
+-rw-rw-rw-   0        0        0     5450 2023-12-06 09:37:10.000000 edm_arch-1.0.42/src/edmpy/db.py
+-rw-rw-rw-   0        0        0    13431 2023-12-05 09:27:43.000000 edm_arch-1.0.42/src/edmpy/edm.kv
+-rw-rw-rw-   0        0        0   126256 2024-05-22 13:13:38.000000 edm_arch-1.0.42/src/edmpy/edm.py
+-rw-rw-rw-   0        0        0     5653 2024-04-18 08:18:35.000000 edm_arch-1.0.42/src/edmpy/geo.py
+-rw-rw-rw-   0        0        0     2495 2023-12-06 09:36:13.000000 edm_arch-1.0.42/src/edmpy/ini.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:47:14.534671 edm_arch-1.0.42/src/edmpy/lib/
+-rw-rw-rw-   0        0        0        0 2021-08-16 15:52:39.000000 edm_arch-1.0.42/src/edmpy/lib/__init__.py
+-rw-rw-rw-   0        0        0     4204 2023-12-04 14:38:01.000000 edm_arch-1.0.42/src/edmpy/lib/blockdata.py
+-rw-rw-rw-   0        0        0     4333 2023-12-06 09:31:45.000000 edm_arch-1.0.42/src/edmpy/lib/colorscheme.py
+-rw-rw-rw-   0        0        0     3994 2023-12-04 14:40:09.000000 edm_arch-1.0.42/src/edmpy/lib/dbs.py
+-rw-rw-rw-   0        0        0   195835 2024-05-22 13:06:32.000000 edm_arch-1.0.42/src/edmpy/lib/e5_widgets.py
+-rw-rw-rw-   0        0        0     1812 2023-12-04 14:41:01.000000 edm_arch-1.0.42/src/edmpy/lib/misc.py
+-rw-rw-rw-   0        0        0        0 2022-06-07 20:43:53.000000 edm_arch-1.0.42/src/edmpy/py.typed
+-rw-rw-rw-   0        0        0      531 2024-04-16 00:42:15.000000 edm_arch-1.0.42/src/edmpy/test_edm.py
+-rw-rw-rw-   0        0        0    46620 2024-04-18 08:16:59.000000 edm_arch-1.0.42/src/edmpy/totalstation.py
```

### Comparing `edm_arch-1.0.41/LICENSE` & `edm_arch-1.0.42/LICENSE`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.41/PKG-INFO` & `edm_arch-1.0.42/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edm-arch
-Version: 1.0.41
+Version: 1.0.42
 Summary: Total stations for archaeologists
 Home-page: https://github.com/surf3s/EDM
 Author: Shannon P. McPherron
 Author-email: mcpherron@eva.mpg.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/surf3s/EDM/issues
 Platform: unix
@@ -135,14 +135,22 @@
 
 Short answer, I don't know.  I have simulated having 1000 points in the database and it is still reasonably fast and responsive on my laptop.  As you add more points, you can expect certain parts of the program to slow (e.g. opening the data grid to view all points).  I never intended my programs to be the main database a person uses.  I always envisioned doing some data entry with these programs (E5 and EDM) before moving the data into a real database.  However, I know lots of people who keep their entire dataset in these programs.  I think that is okay, but remember to always keep backups.
 
 #### Why can't I plot the points with this program?
 
 I am working on this.  Once this program is working smoothly, I will add plot functionality.
 
+##### Virus Warning
+
+Recently (May, 2024) I was helping someone put the program on a Windows 10 tablet.  However, the virus protection software (Microsoft) said the Windows exe version was a virus and immediately removed it.  It took a lot of time to find a work around.  Eventually we made exe programs a virus exception.  This is not a great solution.  I can assure you that edm.exe does not contain a virus.  I also personally downloaded the same version and scanned it with my virus detection software.  Nothing.  I will try to find a computer where I can replicate this and see what part of my program is giving this problem.  If you experience this as well, let me know.
+
+##### Changes for Version 1.0.42 (May, 2024)
+1.  Fixed bug where default values on speed buttons did not trigger linked fields
+2.  Fixed bug where changing value of a field in edit screen did not trigger linked fields
+
 ##### Changes for Version 1.0.41 (May, 2024)
 1.  Fixed crash when spamming Add button in menu in datagrid
 
 ##### Changes for Version 1.0.40 (Decemeber, 2023)
 1.  GeoMax added by Tim Schueler
 2.  Multiple bugs traps in datagrid
 3.  Brought changes in E5 over and debugged more
```

### Comparing `edm_arch-1.0.41/README.md` & `edm_arch-1.0.42/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -95,14 +95,22 @@
 
 Short answer, I don't know.  I have simulated having 1000 points in the database and it is still reasonably fast and responsive on my laptop.  As you add more points, you can expect certain parts of the program to slow (e.g. opening the data grid to view all points).  I never intended my programs to be the main database a person uses.  I always envisioned doing some data entry with these programs (E5 and EDM) before moving the data into a real database.  However, I know lots of people who keep their entire dataset in these programs.  I think that is okay, but remember to always keep backups.
 
 #### Why can't I plot the points with this program?
 
 I am working on this.  Once this program is working smoothly, I will add plot functionality.
 
+##### Virus Warning
+
+Recently (May, 2024) I was helping someone put the program on a Windows 10 tablet.  However, the virus protection software (Microsoft) said the Windows exe version was a virus and immediately removed it.  It took a lot of time to find a work around.  Eventually we made exe programs a virus exception.  This is not a great solution.  I can assure you that edm.exe does not contain a virus.  I also personally downloaded the same version and scanned it with my virus detection software.  Nothing.  I will try to find a computer where I can replicate this and see what part of my program is giving this problem.  If you experience this as well, let me know.
+
+##### Changes for Version 1.0.42 (May, 2024)
+1.  Fixed bug where default values on speed buttons did not trigger linked fields
+2.  Fixed bug where changing value of a field in edit screen did not trigger linked fields
+
 ##### Changes for Version 1.0.41 (May, 2024)
 1.  Fixed crash when spamming Add button in menu in datagrid
 
 ##### Changes for Version 1.0.40 (Decemeber, 2023)
 1.  GeoMax added by Tim Schueler
 2.  Multiple bugs traps in datagrid
 3.  Brought changes in E5 over and debugged more
```

### Comparing `edm_arch-1.0.41/pyproject.toml` & `edm_arch-1.0.42/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.41/setup.cfg` & `edm_arch-1.0.42/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 646d 2d61 7263 680d 0a64 6573   = edm-arch..des
 00000020: 6372 6970 7469 6f6e 203d 2054 6f74 616c  cription = Total
 00000030: 2073 7461 7469 6f6e 7320 666f 7220 6172   stations for ar
 00000040: 6368 6165 6f6c 6f67 6973 7473 0d0a 7665  chaeologists..ve
-00000050: 7273 696f 6e20 3d20 312e 302e 3431 0d0a  rsion = 1.0.41..
+00000050: 7273 696f 6e20 3d20 312e 302e 3432 0d0a  rsion = 1.0.42..
 00000060: 6175 7468 6f72 203d 2053 6861 6e6e 6f6e  author = Shannon
 00000070: 2050 2e20 4d63 5068 6572 726f 6e0d 0a61   P. McPherron..a
 00000080: 7574 686f 725f 656d 6169 6c20 3d20 6d63  uthor_email = mc
 00000090: 7068 6572 726f 6e40 6576 612e 6d70 672e  pherron@eva.mpg.
 000000a0: 6465 0d0a 6c6f 6e67 5f64 6573 6372 6970  de..long_descrip
 000000b0: 7469 6f6e 203d 2066 696c 653a 2052 4541  tion = file: REA
 000000c0: 444d 452e 6d64 0d0a 6c6f 6e67 5f64 6573  DME.md..long_des
```

### Comparing `edm_arch-1.0.41/src/edm_arch.egg-info/PKG-INFO` & `edm_arch-1.0.42/src/edm_arch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edm-arch
-Version: 1.0.41
+Version: 1.0.42
 Summary: Total stations for archaeologists
 Home-page: https://github.com/surf3s/EDM
 Author: Shannon P. McPherron
 Author-email: mcpherron@eva.mpg.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/surf3s/EDM/issues
 Platform: unix
@@ -135,14 +135,22 @@
 
 Short answer, I don't know.  I have simulated having 1000 points in the database and it is still reasonably fast and responsive on my laptop.  As you add more points, you can expect certain parts of the program to slow (e.g. opening the data grid to view all points).  I never intended my programs to be the main database a person uses.  I always envisioned doing some data entry with these programs (E5 and EDM) before moving the data into a real database.  However, I know lots of people who keep their entire dataset in these programs.  I think that is okay, but remember to always keep backups.
 
 #### Why can't I plot the points with this program?
 
 I am working on this.  Once this program is working smoothly, I will add plot functionality.
 
+##### Virus Warning
+
+Recently (May, 2024) I was helping someone put the program on a Windows 10 tablet.  However, the virus protection software (Microsoft) said the Windows exe version was a virus and immediately removed it.  It took a lot of time to find a work around.  Eventually we made exe programs a virus exception.  This is not a great solution.  I can assure you that edm.exe does not contain a virus.  I also personally downloaded the same version and scanned it with my virus detection software.  Nothing.  I will try to find a computer where I can replicate this and see what part of my program is giving this problem.  If you experience this as well, let me know.
+
+##### Changes for Version 1.0.42 (May, 2024)
+1.  Fixed bug where default values on speed buttons did not trigger linked fields
+2.  Fixed bug where changing value of a field in edit screen did not trigger linked fields
+
 ##### Changes for Version 1.0.41 (May, 2024)
 1.  Fixed crash when spamming Add button in menu in datagrid
 
 ##### Changes for Version 1.0.40 (Decemeber, 2023)
 1.  GeoMax added by Tim Schueler
 2.  Multiple bugs traps in datagrid
 3.  Brought changes in E5 over and debugged more
```

### Comparing `edm_arch-1.0.41/src/edm_arch.egg-info/SOURCES.txt` & `edm_arch-1.0.42/src/edm_arch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.41/src/edmpy/cfg.py` & `edm_arch-1.0.42/src/edmpy/cfg.py`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.41/src/edmpy/constants.py` & `edm_arch-1.0.42/src/edmpy/constants.py`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.41/src/edmpy/db.py` & `edm_arch-1.0.42/src/edmpy/db.py`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.41/src/edmpy/edm.kv` & `edm_arch-1.0.42/src/edmpy/edm.kv`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.41/src/edmpy/edm.py` & `edm_arch-1.0.42/src/edmpy/edm.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,14 +87,18 @@
   Fixed datum menu in setups (to not have add new)
   Added message when trying to do setups without having added datums
   fixed a logic bug with units when also unit is set to carry
 
 Changes for Version 1.0.41
   fixed crash when Add button is pressed multiple times
 
+Changes for Version 1.0.42
+  Fixed bug where default values on speed buttons did not trigger linked fields
+  Fixed bug where changing value of a field in edit screen did not trigger linked fields
+
 Bugs/To Do
   have to click twice on unit to get it to switch units
   add units to menu as you go along
   need to move load_dialog out of kv and into code and error trap bad paths
   could make menus work better with keyboard (at least with tab)
   Do unitchecking after doing an offset shot on suffix 0 points
   Good way to get random hash IDs
@@ -183,15 +187,15 @@
 """
 try:
     import win32timezone
     win32timezone.TimeZoneInfo.local()
 except ModuleNotFoundError:
     pass
 
-VERSION = '1.0.41'
+VERSION = '1.0.42'
 PRODUCTION_DATE = 'May, 2024'
 __DEFAULT_FIELDS__ = ['X', 'Y', 'Z', 'SLOPED', 'VANGLE', 'HANGLE', 'STATIONX', 'STATIONY', 'STATIONZ', 'DATUMX', 'DATUMY', 'DATUMZ', 'LOCALX', 'LOCALY', 'LOCALZ', 'DATE', 'PRISM', 'ID']
 __BUTTONS__ = 13
 __LASTCOMPORT__ = 16
 MAX_SCREEN_WIDTH = 400
 __program__ = 'EDM'
 
@@ -978,16 +982,16 @@
 
     def add_point_record(self):
         new_record = {}
         new_record = self.fill_default_fields(new_record)
         if self.station.shot_type != 'continue':
             new_record = self.find_unit_and_fill_fields(new_record)
             new_record = self.fill_carry_fields(new_record)
-            new_record = self.fill_link_fields(new_record)
             new_record = self.fill_button_defaults(new_record)
+            new_record = self.fill_link_fields(new_record)
             new_record = self.do_increments(new_record)
             new_record['SUFFIX'] = 0
         else:
             new_record = self.fill_empty_with_last(new_record)
             new_record['SUFFIX'] = int(self.get_last_value('SUFFIX')) + 1
 
         self.data.db.table(self.data.table).insert(new_record)
```

### Comparing `edm_arch-1.0.41/src/edmpy/geo.py` & `edm_arch-1.0.42/src/edmpy/geo.py`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.41/src/edmpy/ini.py` & `edm_arch-1.0.42/src/edmpy/ini.py`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.41/src/edmpy/lib/blockdata.py` & `edm_arch-1.0.42/src/edmpy/lib/blockdata.py`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.41/src/edmpy/lib/colorscheme.py` & `edm_arch-1.0.42/src/edmpy/lib/colorscheme.py`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.41/src/edmpy/lib/dbs.py` & `edm_arch-1.0.42/src/edmpy/lib/dbs.py`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.41/src/edmpy/lib/e5_widgets.py` & `edm_arch-1.0.42/src/edmpy/lib/e5_widgets.py`

 * *Files 0% similar despite different names*

```diff
@@ -1953,15 +1953,15 @@
         elif not instance.focus and not self.loading:
             self.refresh_linked_fields(instance.id, instance.text)
 
     def menu_selection(self, instance):
         self.popup.dismiss()
         if self.popup_field_widget:
             self.popup_field_widget.text = instance.text if not instance.id == 'add_button' else self.popup_textbox.text
-            self.refresh_linked_fields(instance.id, instance.text)
+            self.refresh_linked_fields(self.popup_field_widget.id, self.popup_field_widget.text)
             if instance.id == 'add_button' and self.popup_field_widget.text.strip() != '':
                 field = self.e5_cfg.get(self.popup_field_widget.id)
                 if self.popup_field_widget.text not in field.menu:
                     field.menu.append(self.popup_field_widget.text)
                     self.e5_cfg.update_value(field.name, 'MENU', ','.join(field.menu))
                     self.e5_cfg.save()
         self.popup_field_widget = None
```

### Comparing `edm_arch-1.0.41/src/edmpy/lib/misc.py` & `edm_arch-1.0.42/src/edmpy/lib/misc.py`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.41/src/edmpy/test_edm.py` & `edm_arch-1.0.42/src/edmpy/test_edm.py`

 * *Files identical despite different names*

### Comparing `edm_arch-1.0.41/src/edmpy/totalstation.py` & `edm_arch-1.0.42/src/edmpy/totalstation.py`

 * *Files identical despite different names*

