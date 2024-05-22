# Comparing `tmp/composition_vectorizer-0.1.2.1.tar.gz` & `tmp/composition_vectorizer-0.1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composition_vectorizer-0.1.2.1.tar", last modified: Thu Mar 21 03:09:02 2024, max compression
+gzip compressed data, was "composition_vectorizer-0.1.2.2.tar", last modified: Wed May 22 19:45:08 2024, max compression
```

## Comparing `composition_vectorizer-0.1.2.1.tar` & `composition_vectorizer-0.1.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 aqd5773  (3463194) aqd5773  (3463194)        0 2024-03-21 03:09:02.232988 composition_vectorizer-0.1.2.1/
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)     1072 2024-03-20 20:34:16.000000 composition_vectorizer-0.1.2.1/LICENSE
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)       42 2024-03-21 01:19:05.000000 composition_vectorizer-0.1.2.1/MANIFEST.in
--rw-r--r--   0 aqd5773  (3463194) aqd5773  (3463194)      984 2024-03-21 03:09:02.232988 composition_vectorizer-0.1.2.1/PKG-INFO
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)      146 2024-03-20 20:34:16.000000 composition_vectorizer-0.1.2.1/README.md
-drwxrwxr-x   0 aqd5773  (3463194) aqd5773  (3463194)        0 2024-03-21 03:09:02.228988 composition_vectorizer-0.1.2.1/composition_vectorizer/
-drwxrwxr-x   0 aqd5773  (3463194) aqd5773  (3463194)        0 2024-03-21 03:09:02.232988 composition_vectorizer-0.1.2.1/composition_vectorizer/Files_from_GTDL_paper/
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)     5977 2024-03-20 20:45:51.000000 composition_vectorizer-0.1.2.1/composition_vectorizer/Files_from_GTDL_paper/Z_row_column.txt
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)    47553 2024-03-20 20:45:51.000000 composition_vectorizer-0.1.2.1/composition_vectorizer/Files_from_GTDL_paper/element_property.txt
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)    27486 2024-03-20 20:45:51.000000 composition_vectorizer-0.1.2.1/composition_vectorizer/Files_from_GTDL_paper/gao_data.txt
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)   543992 2024-03-20 20:45:51.000000 composition_vectorizer-0.1.2.1/composition_vectorizer/Files_from_GTDL_paper/gfa_dataset.txt
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)      138 2024-03-21 00:03:49.000000 composition_vectorizer-0.1.2.1/composition_vectorizer/__init__.py
-drwxrwxr-x   0 aqd5773  (3463194) aqd5773  (3463194)        0 2024-03-21 03:09:02.232988 composition_vectorizer-0.1.2.1/composition_vectorizer/__pycache__/
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)      327 2024-03-21 00:31:45.000000 composition_vectorizer-0.1.2.1/composition_vectorizer/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)     1779 2024-03-20 22:27:21.000000 composition_vectorizer-0.1.2.1/composition_vectorizer/__pycache__/d1.cpython-310.pyc
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)     1486 2024-03-21 03:07:13.000000 composition_vectorizer-0.1.2.1/composition_vectorizer/__pycache__/featurizers.cpython-310.pyc
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)      648 2024-03-21 03:07:13.000000 composition_vectorizer-0.1.2.1/composition_vectorizer/__pycache__/utilities.cpython-310.pyc
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)      190 2024-03-21 03:07:09.000000 composition_vectorizer-0.1.2.1/composition_vectorizer/__pycache__/version.cpython-310.pyc
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)     1285 2024-03-21 03:06:03.000000 composition_vectorizer-0.1.2.1/composition_vectorizer/featurizers.py
-drwxrwxr-x   0 aqd5773  (3463194) aqd5773  (3463194)        0 2024-03-21 03:09:02.232988 composition_vectorizer-0.1.2.1/composition_vectorizer/orderings/
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)     1731 2024-03-20 21:31:43.000000 composition_vectorizer-0.1.2.1/composition_vectorizer/orderings/1d_orderings.pkl
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)      431 2024-03-21 01:20:25.000000 composition_vectorizer-0.1.2.1/composition_vectorizer/utilities.py
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)       23 2024-03-21 03:08:56.000000 composition_vectorizer-0.1.2.1/composition_vectorizer/version.py
-drwxrwxr-x   0 aqd5773  (3463194) aqd5773  (3463194)        0 2024-03-21 03:09:02.232988 composition_vectorizer-0.1.2.1/composition_vectorizer.egg-info/
--rw-r--r--   0 aqd5773  (3463194) aqd5773  (3463194)      984 2024-03-21 03:09:02.000000 composition_vectorizer-0.1.2.1/composition_vectorizer.egg-info/PKG-INFO
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)     1004 2024-03-21 03:09:02.000000 composition_vectorizer-0.1.2.1/composition_vectorizer.egg-info/SOURCES.txt
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)        1 2024-03-21 03:09:02.000000 composition_vectorizer-0.1.2.1/composition_vectorizer.egg-info/dependency_links.txt
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)       34 2024-03-21 03:09:02.000000 composition_vectorizer-0.1.2.1/composition_vectorizer.egg-info/requires.txt
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)       23 2024-03-21 03:09:02.000000 composition_vectorizer-0.1.2.1/composition_vectorizer.egg-info/top_level.txt
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)       38 2024-03-21 03:09:02.232988 composition_vectorizer-0.1.2.1/setup.cfg
--rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)     1688 2024-03-21 00:48:59.000000 composition_vectorizer-0.1.2.1/setup.py
+drwxrwxr-x   0 aqd5773  (3463194) aqd5773  (3463194)        0 2024-05-22 19:45:08.115698 composition_vectorizer-0.1.2.2/
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)     1072 2024-03-20 20:34:16.000000 composition_vectorizer-0.1.2.2/LICENSE
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)       42 2024-03-21 01:19:05.000000 composition_vectorizer-0.1.2.2/MANIFEST.in
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)      920 2024-05-22 19:45:08.115698 composition_vectorizer-0.1.2.2/PKG-INFO
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)      146 2024-03-20 20:34:16.000000 composition_vectorizer-0.1.2.2/README.md
+drwxrwxr-x   0 aqd5773  (3463194) aqd5773  (3463194)        0 2024-05-22 19:45:08.111698 composition_vectorizer-0.1.2.2/composition_vectorizer/
+drwxrwxr-x   0 aqd5773  (3463194) aqd5773  (3463194)        0 2024-05-22 19:45:08.115698 composition_vectorizer-0.1.2.2/composition_vectorizer/Files_from_GTDL_paper/
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)     5977 2024-03-20 20:45:51.000000 composition_vectorizer-0.1.2.2/composition_vectorizer/Files_from_GTDL_paper/Z_row_column.txt
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)    47553 2024-03-20 20:45:51.000000 composition_vectorizer-0.1.2.2/composition_vectorizer/Files_from_GTDL_paper/element_property.txt
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)    27486 2024-03-20 20:45:51.000000 composition_vectorizer-0.1.2.2/composition_vectorizer/Files_from_GTDL_paper/gao_data.txt
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)   543992 2024-03-20 20:45:51.000000 composition_vectorizer-0.1.2.2/composition_vectorizer/Files_from_GTDL_paper/gfa_dataset.txt
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)      138 2024-03-21 00:03:49.000000 composition_vectorizer-0.1.2.2/composition_vectorizer/__init__.py
+drwxrwxr-x   0 aqd5773  (3463194) aqd5773  (3463194)        0 2024-05-22 19:45:08.115698 composition_vectorizer-0.1.2.2/composition_vectorizer/__pycache__/
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)      327 2024-03-21 00:31:45.000000 composition_vectorizer-0.1.2.2/composition_vectorizer/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)     1779 2024-03-20 22:27:21.000000 composition_vectorizer-0.1.2.2/composition_vectorizer/__pycache__/d1.cpython-310.pyc
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)     1539 2024-05-22 19:32:59.000000 composition_vectorizer-0.1.2.2/composition_vectorizer/__pycache__/featurizers.cpython-310.pyc
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)      648 2024-03-21 03:07:13.000000 composition_vectorizer-0.1.2.2/composition_vectorizer/__pycache__/utilities.cpython-310.pyc
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)      192 2024-05-22 19:24:26.000000 composition_vectorizer-0.1.2.2/composition_vectorizer/__pycache__/version.cpython-310.pyc
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)     1609 2024-05-22 19:37:05.000000 composition_vectorizer-0.1.2.2/composition_vectorizer/featurizers.py
+drwxrwxr-x   0 aqd5773  (3463194) aqd5773  (3463194)        0 2024-05-22 19:45:08.115698 composition_vectorizer-0.1.2.2/composition_vectorizer/orderings/
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)     1731 2024-03-20 21:31:43.000000 composition_vectorizer-0.1.2.2/composition_vectorizer/orderings/1d_orderings.pkl
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)      431 2024-03-21 01:20:25.000000 composition_vectorizer-0.1.2.2/composition_vectorizer/utilities.py
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)       23 2024-05-22 19:38:23.000000 composition_vectorizer-0.1.2.2/composition_vectorizer/version.py
+drwxrwxr-x   0 aqd5773  (3463194) aqd5773  (3463194)        0 2024-05-22 19:45:08.111698 composition_vectorizer-0.1.2.2/composition_vectorizer.egg-info/
+-rw-r--r--   0 aqd5773  (3463194) aqd5773  (3463194)      920 2024-05-22 19:45:08.000000 composition_vectorizer-0.1.2.2/composition_vectorizer.egg-info/PKG-INFO
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)     1004 2024-05-22 19:45:08.000000 composition_vectorizer-0.1.2.2/composition_vectorizer.egg-info/SOURCES.txt
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)        1 2024-05-22 19:45:08.000000 composition_vectorizer-0.1.2.2/composition_vectorizer.egg-info/dependency_links.txt
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)       34 2024-05-22 19:45:08.000000 composition_vectorizer-0.1.2.2/composition_vectorizer.egg-info/requires.txt
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)       23 2024-05-22 19:45:08.000000 composition_vectorizer-0.1.2.2/composition_vectorizer.egg-info/top_level.txt
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)       38 2024-05-22 19:45:08.115698 composition_vectorizer-0.1.2.2/setup.cfg
+-rw-rw-r--   0 aqd5773  (3463194) aqd5773  (3463194)     1688 2024-03-21 00:48:59.000000 composition_vectorizer-0.1.2.2/setup.py
```

### Comparing `composition_vectorizer-0.1.2.1/LICENSE` & `composition_vectorizer-0.1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `composition_vectorizer-0.1.2.1/PKG-INFO` & `composition_vectorizer-0.1.2.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composition_vectorizer
-Version: 0.1.2.1
+Version: 0.1.2.2
 Summary: Converts string composition to numpy arrays
 Home-page: https://github.com/dovahkiin0022/composition_vectorizer.git
 Author: Arindam Debnath
 Author-email: debnath@psu.edu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
@@ -13,12 +13,10 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pymatgen>=2024.2.20
-Requires-Dist: numpy>=1.25.0
 
 # composition_vectorizer
 This package contains functions to convert chemical compositions (in string) to vector arrays for machine learning tasks
```

### Comparing `composition_vectorizer-0.1.2.1/composition_vectorizer/Files_from_GTDL_paper/Z_row_column.txt` & `composition_vectorizer-0.1.2.2/composition_vectorizer/Files_from_GTDL_paper/Z_row_column.txt`

 * *Files identical despite different names*

### Comparing `composition_vectorizer-0.1.2.1/composition_vectorizer/Files_from_GTDL_paper/element_property.txt` & `composition_vectorizer-0.1.2.2/composition_vectorizer/Files_from_GTDL_paper/element_property.txt`

 * *Files identical despite different names*

### Comparing `composition_vectorizer-0.1.2.1/composition_vectorizer/Files_from_GTDL_paper/gao_data.txt` & `composition_vectorizer-0.1.2.2/composition_vectorizer/Files_from_GTDL_paper/gao_data.txt`

 * *Files identical despite different names*

### Comparing `composition_vectorizer-0.1.2.1/composition_vectorizer/Files_from_GTDL_paper/gfa_dataset.txt` & `composition_vectorizer-0.1.2.2/composition_vectorizer/Files_from_GTDL_paper/gfa_dataset.txt`

 * *Files identical despite different names*

### Comparing `composition_vectorizer-0.1.2.1/composition_vectorizer/__pycache__/d1.cpython-310.pyc` & `composition_vectorizer-0.1.2.2/composition_vectorizer/__pycache__/d1.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `composition_vectorizer-0.1.2.1/composition_vectorizer/__pycache__/featurizers.cpython-310.pyc` & `composition_vectorizer-0.1.2.2/composition_vectorizer/__pycache__/featurizers.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Mar 21 03:06:03 2024 UTC, .py size: 1285 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 1ba4 fb65 0505 0000  o..........e....
+00000000: 6f0d 0d0a 0000 0000 2d48 4e66 c405 0000  o.......-HNf....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0073 9600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6400 6403 6c05  d.l.m.Z...d.d.l.
 00000050: 6d06 5a06 0100 6504 6404 6405 8302 8f22  m.Z...e.d.d...."
 00000060: 5a04 6507 6504 6406 8302 8f0d 5a08 6502  Z.e.e.d.....Z.e.
 00000070: a009 6508 a101 5a0a 5700 6401 0400 0400  ..e...Z.W.d.....
@@ -12,82 +12,86 @@
 000000b0: 5900 0100 6700 6601 6407 6408 8401 5a0b  Y...g.f.d.d...Z.
 000000c0: 6401 5300 2909 e900 0000 004e 2901 da04  d.S.)......N)...
 000000d0: 7061 7468 2901 da0d 7079 6d61 7467 656e  path)...pymatgen
 000000e0: 5f63 6f6d 707a 2063 6f6d 706f 7369 7469  _compz compositi
 000000f0: 6f6e 5f76 6563 746f 7269 7a65 722e 6f72  on_vectorizer.or
 00000100: 6465 7269 6e67 737a 1031 645f 6f72 6465  deringsz.1d_orde
 00000110: 7269 6e67 732e 706b 6cda 0272 6263 0300  rings.pkl..rbc..
-00000120: 0000 0000 0000 0000 0000 0b00 0000 0700  ................
-00000130: 0000 0300 0000 730a 0100 0088 0064 0176  ......s......d.v
+00000120: 0000 0000 0000 0000 0000 0a00 0000 0700  ................
+00000130: 0000 0300 0000 7324 0100 0088 0064 0176  ......s$.....d.v
 00000140: 0172 0874 0064 0283 0182 0174 017c 0083  .r.t.d.....t.|..
-00000150: 017d 0074 027c 0283 0164 036b 0272 3367  .}.t.|...d.k.r3g
-00000160: 007d 037c 0044 005d 0c7d 047c 0374 037c  .}.|.D.].}.|.t.|
-00000170: 04a0 04a1 00a0 05a1 0083 0137 007d 0371  ...........7.}.q
-00000180: 1674 06a0 0774 0874 097c 0383 0187 0066  .t...t.t.|.....f
-00000190: 0164 0464 0584 0864 068d 02a1 017d 056e  .d.d...d.....}.n
-000001a0: 0d74 06a0 0774 087c 0287 0066 0164 0764  .t...t.|...f.d.d
-000001b0: 0584 0864 068d 02a1 017d 0574 06a0 0a74  ...d.....}.t...t
-000001c0: 027c 0083 0174 027c 0583 0167 02a1 017d  .|...t.|...g...}
-000001d0: 0674 0b7c 0083 0144 005d 1c5c 027d 077d  .t.|...D.].\.}.}
-000001e0: 047c 04a0 04a1 00a0 0ca1 0044 005d 115c  .|.........D.].\
-000001f0: 027d 087d 0974 06a0 0d7c 057c 086b 02a1  .}.}.t...|.|.k..
-00000200: 017d 0a7c 097c 067c 077c 0a66 023c 0071  .}.|.|.|.|.f.<.q
-00000210: 5971 4f7c 0674 066a 0e7c 0664 0864 098d  YqO|.t.j.|.d.d..
-00000220: 02a0 0f64 0a64 08a1 021b 007d 0674 066a  ...d.d.....}.t.j
-00000230: 077c 0674 066a 1064 0b8d 027d 067c 067c  .|.t.j.d...}.|.|
-00000240: 0566 0253 0029 0c4e 2904 da08 616c 7068  .f.S.).N)...alph
-00000250: 6162 6574 5a08 7065 7269 6f64 6963 5a08  abetZ.periodicZ.
-00000260: 7065 7474 6966 6f72 7a0a 6d2d 7065 7474  pettiforz.m-pett
-00000270: 6966 6f72 7a44 6f72 6465 7220 6d75 7374  iforzDorder must
-00000280: 2062 6520 6f6e 6520 6f66 205b 2761 6c70   be one of ['alp
-00000290: 6861 6265 7427 2c27 7065 7269 6f64 6963  habet','periodic
-000002a0: 272c 2770 6574 7469 666f 7227 2c27 6d2d  ','pettifor','m-
-000002b0: 7065 7474 6966 6f72 275d 7201 0000 0063  pettifor']r....c
-000002c0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000002d0: 0300 0000 1300 0000 f30e 0000 0074 0088  .............t..
-000002e0: 0019 00a0 017c 00a1 0153 00a9 014e a902  .....|...S...N..
-000002f0: da0b 6f72 6465 7273 5f64 6963 74da 0569  ..orders_dict..i
-00000300: 6e64 6578 a901 da01 78a9 01da 056f 7264  ndex....x....ord
-00000310: 6572 a900 fa50 2f6e 6f65 7468 6572 2f73  er...P/noether/s
-00000320: 302f 6171 6435 3737 332f 636f 6d70 6f73  0/aqd5773/compos
-00000330: 6974 696f 6e5f 7665 6374 6f72 697a 6572  ition_vectorizer
-00000340: 2f63 6f6d 706f 7369 7469 6f6e 5f76 6563  /composition_vec
-00000350: 746f 7269 7a65 722f 6665 6174 7572 697a  torizer/featuriz
-00000360: 6572 732e 7079 da08 3c6c 616d 6264 613e  ers.py..<lambda>
-00000370: 1400 0000 f302 0000 000e 007a 1f66 6561  ...........z.fea
-00000380: 7475 7269 7a65 725f 3164 2e3c 6c6f 6361  turizer_1d.<loca
-00000390: 6c73 3e2e 3c6c 616d 6264 613e 2901 da03  ls>.<lambda>)...
-000003a0: 6b65 7963 0100 0000 0000 0000 0000 0000  keyc............
-000003b0: 0100 0000 0300 0000 1300 0000 7206 0000  ............r...
-000003c0: 0072 0700 0000 7208 0000 0072 0b00 0000  .r....r....r....
-000003d0: 720d 0000 0072 0f00 0000 7210 0000 0072  r....r....r....r
-000003e0: 1100 0000 1600 0000 7212 0000 00e9 0100  ........r.......
-000003f0: 0000 2901 5a04 6178 6973 e9ff ffff ff29  ..).Z.axis.....)
-00000400: 01da 0564 7479 7065 2911 da0a 5661 6c75  ...dtype)...Valu
-00000410: 6545 7272 6f72 7203 0000 00da 036c 656e  eErrorr......len
-00000420: da04 6c69 7374 5a0f 6765 745f 656c 5f61  ..listZ.get_el_a
-00000430: 6d74 5f64 6963 74da 046b 6579 73da 026e  mt_dict..keys..n
-00000440: 70da 0561 7272 6179 da06 736f 7274 6564  p..array..sorted
-00000450: da03 7365 74da 057a 6572 6f73 da09 656e  ..set..zeros..en
-00000460: 756d 6572 6174 65da 0569 7465 6d73 da08  umerate..items..
-00000470: 6172 6777 6865 7265 da03 7375 6dda 0772  argwhere..sum..r
-00000480: 6573 6861 7065 5a07 666c 6f61 7433 3229  eshapeZ.float32)
-00000490: 0bda 0563 6f6d 7073 720e 0000 005a 0765  ...compsr....Z.e
-000004a0: 6c5f 6c69 7374 5a08 616c 6c5f 656c 6573  l_listZ.all_eles
-000004b0: da01 635a 0465 6c65 735a 0861 6c6c 5f76  ..cZ.elesZ.all_v
-000004c0: 6563 73da 0169 da01 6bda 0176 da01 6a72  ecs..i..k..v..jr
-000004d0: 0f00 0000 720d 0000 0072 1000 0000 da0d  ....r....r......
-000004e0: 6665 6174 7572 697a 6572 5f31 640b 0000  featurizer_1d...
-000004f0: 0073 2400 0000 0801 0801 0802 0c01 0401  .s$.............
-00000500: 0801 1601 2001 1a02 1602 1001 1401 0e01  .... ...........
-00000510: 0e01 02fe 1a04 1001 0802 722b 0000 0029  ..........r+...)
-00000520: 0cda 056e 756d 7079 721b 0000 00da 0670  ...numpyr......p
-00000530: 6963 6b6c 65da 1369 6d70 6f72 746c 6962  ickle..importlib
-00000540: 2e72 6573 6f75 7263 6573 7202 0000 005a  .resourcesr....Z
-00000550: 2063 6f6d 706f 7369 7469 6f6e 5f76 6563   composition_vec
-00000560: 746f 7269 7a65 722e 7574 696c 6974 6965  torizer.utilitie
-00000570: 7372 0300 0000 da04 6f70 656e da03 6669  sr......open..fi
-00000580: 64da 046c 6f61 6472 0900 0000 722b 0000  d..loadr....r+..
-00000590: 0072 0f00 0000 720f 0000 0072 0f00 0000  .r....r....r....
-000005a0: 7210 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-000005b0: 0000 0073 1600 0000 0800 0801 0c01 0c01  ...s............
-000005c0: 0c02 0c01 0c01 1cff 0280 1cff 1005       ..............
+00000150: 017d 0088 0064 0376 0072 3974 027c 0283  .}...d.v.r9t.|..
+00000160: 0164 046b 0272 2b7c 0044 005d 0c7d 037c  .d.k.r+|.D.].}.|
+00000170: 0274 037c 03a0 04a1 00a0 05a1 0083 0137  .t.|...........7
+00000180: 007d 0271 1874 0374 067c 0283 0183 017d  .}.q.t.t.|.....}
+00000190: 0274 07a0 0874 097c 0287 0066 0164 0564  .t...t.|...f.d.d
+000001a0: 0684 0864 078d 02a1 017d 046e 1488 0064  ...d.....}.n...d
+000001b0: 086b 0272 4974 027c 0283 0164 046b 0372  .k.rIt.|...d.k.r
+000001c0: 4974 07a0 087c 02a1 017d 046e 0474 0064  It...|...}.n.t.d
+000001d0: 0983 0182 0174 07a0 0a74 027c 0083 0174  .....t...t.|...t
+000001e0: 027c 0483 0167 02a1 017d 0574 0b7c 0083  .|...g...}.t.|..
+000001f0: 0144 005d 1c5c 027d 067d 037c 03a0 04a1  .D.].\.}.}.|....
+00000200: 00a0 0ca1 0044 005d 115c 027d 077d 0874  .....D.].\.}.}.t
+00000210: 07a0 0d7c 047c 076b 02a1 017d 097c 087c  ...|.|.k...}.|.|
+00000220: 057c 067c 0966 023c 0071 6671 5c7c 0574  .|.|.f.<.qfq\|.t
+00000230: 076a 0e7c 0564 0a64 0b8d 02a0 0f64 0c64  .j.|.d.d.....d.d
+00000240: 0aa1 021b 007d 0574 076a 087c 0574 076a  .....}.t.j.|.t.j
+00000250: 1064 0d8d 027d 057c 057c 0466 0253 0029  .d...}.|.|.f.S.)
+00000260: 0e4e 2905 da08 616c 7068 6162 6574 da08  .N)...alphabet..
+00000270: 7065 7269 6f64 6963 da08 7065 7474 6966  periodic..pettif
+00000280: 6f72 fa0a 6d2d 7065 7474 6966 6f72 da04  or..m-pettifor..
+00000290: 7573 6572 7a4b 6f72 6465 7220 6d75 7374  userzKorder must
+000002a0: 2062 6520 6f6e 6520 6f66 205b 2761 6c70   be one of ['alp
+000002b0: 6861 6265 7427 2c27 7065 7269 6f64 6963  habet','periodic
+000002c0: 272c 2770 6574 7469 666f 7227 2c27 6d2d  ','pettifor','m-
+000002d0: 7065 7474 6966 6f72 272c 2775 7365 7227  pettifor','user'
+000002e0: 5d29 0472 0500 0000 7206 0000 0072 0700  ]).r....r....r..
+000002f0: 0000 7208 0000 0072 0100 0000 6301 0000  ..r....r....c...
+00000300: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00000310: 0013 0000 0073 0e00 0000 7400 8800 1900  .....s....t.....
+00000320: a001 7c00 a101 5300 2901 4e29 02da 0b6f  ..|...S.).N)...o
+00000330: 7264 6572 735f 6469 6374 da05 696e 6465  rders_dict..inde
+00000340: 7829 01da 0178 a901 da05 6f72 6465 72a9  x)...x....order.
+00000350: 00fa 502f 6e6f 6574 6865 722f 7330 2f61  ..P/noether/s0/a
+00000360: 7164 3537 3733 2f63 6f6d 706f 7369 7469  qd5773/compositi
+00000370: 6f6e 5f76 6563 746f 7269 7a65 722f 636f  on_vectorizer/co
+00000380: 6d70 6f73 6974 696f 6e5f 7665 6374 6f72  mposition_vector
+00000390: 697a 6572 2f66 6561 7475 7269 7a65 7273  izer/featurizers
+000003a0: 2e70 79da 083c 6c61 6d62 6461 3e15 0000  .py..<lambda>...
+000003b0: 0073 0200 0000 0e00 7a1f 6665 6174 7572  .s......z.featur
+000003c0: 697a 6572 5f31 642e 3c6c 6f63 616c 733e  izer_1d.<locals>
+000003d0: 2e3c 6c61 6d62 6461 3e29 01da 036b 6579  .<lambda>)...key
+000003e0: 7209 0000 007a 3f75 7365 7220 6465 6669  r....z?user defi
+000003f0: 6e65 6420 6f72 6465 7220 6e65 6564 7320  ned order needs 
+00000400: 746f 2062 6520 666f 6c6c 6f77 6564 2062  to be followed b
+00000410: 7920 7468 6520 6c69 7374 206f 6620 656c  y the list of el
+00000420: 656d 656e 7473 e901 0000 0029 015a 0461  ements.....).Z.a
+00000430: 7869 73e9 ffff ffff 2901 da05 6474 7970  xis.....)...dtyp
+00000440: 6529 11da 0a56 616c 7565 4572 726f 7272  e)...ValueErrorr
+00000450: 0300 0000 da03 6c65 6eda 046c 6973 745a  ......len..listZ
+00000460: 0f67 6574 5f65 6c5f 616d 745f 6469 6374  .get_el_amt_dict
+00000470: da04 6b65 7973 da03 7365 74da 026e 70da  ..keys..set..np.
+00000480: 0561 7272 6179 da06 736f 7274 6564 da05  .array..sorted..
+00000490: 7a65 726f 73da 0965 6e75 6d65 7261 7465  zeros..enumerate
+000004a0: da05 6974 656d 73da 0861 7267 7768 6572  ..items..argwher
+000004b0: 65da 0373 756d da07 7265 7368 6170 655a  e..sum..reshapeZ
+000004c0: 0766 6c6f 6174 3332 290a da05 636f 6d70  .float32)...comp
+000004d0: 7372 0e00 0000 5a07 656c 5f6c 6973 74da  sr....Z.el_list.
+000004e0: 0163 5a04 656c 6573 5a08 616c 6c5f 7665  .cZ.elesZ.all_ve
+000004f0: 6373 da01 69da 016b da01 76da 016a 720f  cs..i..k..v..jr.
+00000500: 0000 0072 0d00 0000 7210 0000 00da 0d66  ...r....r......f
+00000510: 6561 7475 7269 7a65 725f 3164 0b00 0000  eaturizer_1d....
+00000520: 732a 0000 0008 0108 0108 0208 010c 0108  s*..............
+00000530: 0116 010c 011c 0114 010c 0108 0216 0210  ................
+00000540: 0114 010e 010e 0102 fe1a 0410 0108 0272  ...............r
+00000550: 2a00 0000 290c da05 6e75 6d70 7972 1b00  *...)...numpyr..
+00000560: 0000 da06 7069 636b 6c65 da13 696d 706f  ....pickle..impo
+00000570: 7274 6c69 622e 7265 736f 7572 6365 7372  rtlib.resourcesr
+00000580: 0200 0000 5a20 636f 6d70 6f73 6974 696f  ....Z compositio
+00000590: 6e5f 7665 6374 6f72 697a 6572 2e75 7469  n_vectorizer.uti
+000005a0: 6c69 7469 6573 7203 0000 00da 046f 7065  litiesr......ope
+000005b0: 6eda 0366 6964 da04 6c6f 6164 720a 0000  n..fid..loadr...
+000005c0: 0072 2a00 0000 720f 0000 0072 0f00 0000  .r*...r....r....
+000005d0: 720f 0000 0072 1000 0000 da08 3c6d 6f64  r....r......<mod
+000005e0: 756c 653e 0100 0000 7316 0000 0008 0008  ule>....s.......
+000005f0: 010c 010c 010c 020c 010c 011c ff02 801c  ................
+00000600: ff10 05                                  ...
```

### Comparing `composition_vectorizer-0.1.2.1/composition_vectorizer/__pycache__/utilities.cpython-310.pyc` & `composition_vectorizer-0.1.2.2/composition_vectorizer/__pycache__/utilities.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `composition_vectorizer-0.1.2.1/composition_vectorizer/featurizers.py` & `composition_vectorizer-0.1.2.2/composition_vectorizer/featurizers.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,29 +5,37 @@
 
 with path('composition_vectorizer.orderings', '1d_orderings.pkl') as path:
     with open(path, 'rb') as fid:
         orders_dict = pickle.load(fid)
 
 
 def featurizer_1d(comps, order, el_list = []):
-        if order not in ['alphabet','periodic','pettifor','m-pettifor']:
-           raise ValueError("order must be one of ['alphabet','periodic','pettifor','m-pettifor']")
+        if order not in ['alphabet','periodic','pettifor','m-pettifor','user']:
+           raise ValueError("order must be one of ['alphabet','periodic','pettifor','m-pettifor','user']")
         
         comps = pymatgen_comp(comps)
-        if len(el_list) == 0:
-            all_eles = []
-            for c in comps:
-                all_eles += list(c.get_el_amt_dict().keys())
-            eles = np.array(sorted(set(all_eles),key = lambda x : orders_dict[order].index(x)))
-        else:
+        if order in ['alphabet','periodic','pettifor','m-pettifor']:
+            if len(el_list) == 0:
+                for c in comps:
+                    el_list += list(c.get_el_amt_dict().keys())
+                el_list = list(set(el_list))
             eles = np.array(sorted(el_list,key = lambda x : orders_dict[order].index(x)))
-            
+        elif order == 'user' and len(el_list)!=0:
+            eles = np.array(el_list)
+        else:
+            raise ValueError('user defined order needs to be followed by the list of elements')
+
         all_vecs = np.zeros([len(comps), len(eles)])
         for i, c in enumerate(comps):
             for k, v in c.get_el_amt_dict().items(): 
                 j = np.argwhere(eles == k)
                 all_vecs[i, j] = v
 
         all_vecs = all_vecs / np.sum(all_vecs, axis=1).reshape(-1, 1)
         all_vecs = np.array(all_vecs, dtype=np.float32)
 
-        return (all_vecs,eles)
+        return (all_vecs,eles)
+
+def decode_comp(val_list,order):
+    return [''.join([f'{order[i]}{x[i]}' for i in range(len(order)) if x[i]!=0])for x in val_list]
+
+
```

### Comparing `composition_vectorizer-0.1.2.1/composition_vectorizer/orderings/1d_orderings.pkl` & `composition_vectorizer-0.1.2.2/composition_vectorizer/orderings/1d_orderings.pkl`

 * *Files identical despite different names*

### Comparing `composition_vectorizer-0.1.2.1/composition_vectorizer.egg-info/PKG-INFO` & `composition_vectorizer-0.1.2.2/composition_vectorizer.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: composition_vectorizer
-Version: 0.1.2.1
+Name: composition-vectorizer
+Version: 0.1.2.2
 Summary: Converts string composition to numpy arrays
 Home-page: https://github.com/dovahkiin0022/composition_vectorizer.git
 Author: Arindam Debnath
 Author-email: debnath@psu.edu
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
@@ -13,12 +13,10 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pymatgen>=2024.2.20
-Requires-Dist: numpy>=1.25.0
 
 # composition_vectorizer
 This package contains functions to convert chemical compositions (in string) to vector arrays for machine learning tasks
```

### Comparing `composition_vectorizer-0.1.2.1/composition_vectorizer.egg-info/SOURCES.txt` & `composition_vectorizer-0.1.2.2/composition_vectorizer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `composition_vectorizer-0.1.2.1/setup.py` & `composition_vectorizer-0.1.2.2/setup.py`

 * *Files identical despite different names*

