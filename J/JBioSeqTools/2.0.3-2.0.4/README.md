# Comparing `tmp/JBioSeqTools-2.0.3.tar.gz` & `tmp/JBioSeqTools-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "JBioSeqTools-2.0.3.tar", last modified: Tue Mar 19 11:57:50 2024, max compression
+gzip compressed data, was "JBioSeqTools-2.0.4.tar", last modified: Wed May 22 12:48:14 2024, max compression
```

## Comparing `JBioSeqTools-2.0.3.tar` & `JBioSeqTools-2.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 11:57:50.943987 JBioSeqTools-2.0.3/
-drwxrwxrwx   0        0        0        0 2024-03-19 11:57:50.887851 JBioSeqTools-2.0.3/JBioSeqTools.egg-info/
--rw-rw-rw-   0        0        0     1027 2024-03-19 11:57:49.000000 JBioSeqTools-2.0.3/JBioSeqTools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      733 2024-03-19 11:57:50.000000 JBioSeqTools-2.0.3/JBioSeqTools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 11:57:49.000000 JBioSeqTools-2.0.3/JBioSeqTools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      124 2024-03-19 11:57:49.000000 JBioSeqTools-2.0.3/JBioSeqTools.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-03-19 11:57:49.000000 JBioSeqTools-2.0.3/JBioSeqTools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 JBioSeqTools-2.0.3/LICENSE
--rw-rw-rw-   0        0        0       93 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1027 2024-03-19 11:57:50.942988 JBioSeqTools-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0   136379 2024-03-08 13:18:31.000000 JBioSeqTools-2.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-19 11:57:50.903288 JBioSeqTools-2.0.3/jbst/
--rw-rw-rw-   0        0        0     1489 2024-03-19 11:53:10.000000 JBioSeqTools-2.0.3/jbst/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 11:57:50.933931 JBioSeqTools-2.0.3/jbst/data/
--rw-rw-rw-   0        0        0    11970 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.3/jbst/data/backbone.xlsx
--rw-rw-rw-   0        0        0    18801 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.3/jbst/data/codons.xlsx
--rw-rw-rw-   0        0        0    24612 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.3/jbst/data/enzymes.xlsx
--rw-rw-rw-   0        0        0    10901 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.3/jbst/data/fluorescent_tag.xlsx
--rw-rw-rw-   0        0        0     9685 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.3/jbst/data/linkers.xlsx
--rw-rw-rw-   0        0        0    11897 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.3/jbst/data/polya.xlsx
--rw-rw-rw-   0        0        0    65342 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.3/jbst/data/promoters.xlsx
--rw-rw-rw-   0        0        0    11212 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.3/jbst/data/regulators.xlsx
--rw-rw-rw-   0        0        0   228812 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.3/jbst/data/restriction_enzymes.xlsx
--rw-rw-rw-   0        0        0     8571 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.3/jbst/data/rnai_scoring.xlsx
--rw-rw-rw-   0        0        0    11916 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.3/jbst/data/selectors.xlsx
--rw-rw-rw-   0        0        0    12038 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.3/jbst/data/sh_loops.xlsx
--rw-rw-rw-   0        0        0    10129 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.3/jbst/data/vector_capacity.xlsx
--rw-rw-rw-   0        0        0    16540 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.3/jbst/data/vectors.xlsx
--rw-rw-rw-   0        0        0    16460 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.3/jbst/install.py
--rw-rw-rw-   0        0        0   100908 2024-03-19 11:55:37.000000 JBioSeqTools-2.0.3/jbst/seq_tools.py
-drwxrwxrwx   0        0        0        0 2024-03-19 11:57:50.940976 JBioSeqTools-2.0.3/jbst/tests/
--rw-rw-rw-   0        0        0        2 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.3/jbst/tests/__init__.py
--rw-rw-rw-   0        0        0    10100 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.3/jbst/tests/fasta_vector_test.fasta
--rw-rw-rw-   0        0        0   770446 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.3/jbst/tests/jseq_tests.py
--rw-rw-rw-   0        0        0   126532 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.3/jbst/vector_build.py
--rw-rw-rw-   0        0        0       42 2024-03-19 11:57:50.943987 JBioSeqTools-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1584 2024-03-19 11:37:42.000000 JBioSeqTools-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:48:14.579867 JBioSeqTools-2.0.4/
+drwxrwxrwx   0        0        0        0 2024-05-22 12:48:14.544746 JBioSeqTools-2.0.4/JBioSeqTools.egg-info/
+-rw-rw-rw-   0        0        0     1027 2024-05-22 12:48:13.000000 JBioSeqTools-2.0.4/JBioSeqTools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      733 2024-05-22 12:48:14.000000 JBioSeqTools-2.0.4/JBioSeqTools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 12:48:13.000000 JBioSeqTools-2.0.4/JBioSeqTools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      137 2024-05-22 12:48:14.000000 JBioSeqTools-2.0.4/JBioSeqTools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-22 12:48:14.000000 JBioSeqTools-2.0.4/JBioSeqTools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1104 2022-01-09 13:54:52.000000 JBioSeqTools-2.0.4/LICENSE
+-rw-rw-rw-   0        0        0       93 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1027 2024-05-22 12:48:14.579867 JBioSeqTools-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0   136379 2024-03-08 13:18:31.000000 JBioSeqTools-2.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 12:48:14.550181 JBioSeqTools-2.0.4/jbst/
+-rw-rw-rw-   0        0        0     1489 2024-05-22 12:46:26.000000 JBioSeqTools-2.0.4/jbst/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:48:14.571658 JBioSeqTools-2.0.4/jbst/data/
+-rw-rw-rw-   0        0        0    11970 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/backbone.xlsx
+-rw-rw-rw-   0        0        0    18801 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/codons.xlsx
+-rw-rw-rw-   0        0        0    24612 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/enzymes.xlsx
+-rw-rw-rw-   0        0        0    10901 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/fluorescent_tag.xlsx
+-rw-rw-rw-   0        0        0     9685 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/linkers.xlsx
+-rw-rw-rw-   0        0        0    11897 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/polya.xlsx
+-rw-rw-rw-   0        0        0    65342 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/promoters.xlsx
+-rw-rw-rw-   0        0        0    11212 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/regulators.xlsx
+-rw-rw-rw-   0        0        0   228812 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/restriction_enzymes.xlsx
+-rw-rw-rw-   0        0        0     8571 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/rnai_scoring.xlsx
+-rw-rw-rw-   0        0        0    11916 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/selectors.xlsx
+-rw-rw-rw-   0        0        0    12038 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/data/sh_loops.xlsx
+-rw-rw-rw-   0        0        0    10119 2024-05-22 12:14:29.000000 JBioSeqTools-2.0.4/jbst/data/vector_capacity.xlsx
+-rw-rw-rw-   0        0        0    16543 2024-05-22 12:14:07.000000 JBioSeqTools-2.0.4/jbst/data/vectors.xlsx
+-rw-rw-rw-   0        0        0    15427 2024-05-22 12:45:35.000000 JBioSeqTools-2.0.4/jbst/install.py
+-rw-rw-rw-   0        0        0    99588 2024-05-22 10:14:39.000000 JBioSeqTools-2.0.4/jbst/seq_tools.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:48:14.576856 JBioSeqTools-2.0.4/jbst/tests/
+-rw-rw-rw-   0        0        0        2 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/tests/__init__.py
+-rw-rw-rw-   0        0        0    10100 2023-12-01 12:13:27.000000 JBioSeqTools-2.0.4/jbst/tests/fasta_vector_test.fasta
+-rw-rw-rw-   0        0        0   770959 2024-05-22 11:09:36.000000 JBioSeqTools-2.0.4/jbst/tests/jseq_tests.py
+-rw-rw-rw-   0        0        0   126569 2024-05-22 10:16:21.000000 JBioSeqTools-2.0.4/jbst/vector_build.py
+-rw-rw-rw-   0        0        0       42 2024-05-22 12:48:14.579867 JBioSeqTools-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1600 2024-05-22 12:46:08.000000 JBioSeqTools-2.0.4/setup.py
```

### Comparing `JBioSeqTools-2.0.3/JBioSeqTools.egg-info/PKG-INFO` & `JBioSeqTools-2.0.4/JBioSeqTools.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JBioSeqTools
-Version: 2.0.3
+Version: 2.0.4
 Summary: JBioSeqTools
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: sequence,optimization,vectors,AAV,GC,restriction enzyme
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JBioSeqTools-2.0.3/JBioSeqTools.egg-info/SOURCES.txt` & `JBioSeqTools-2.0.4/JBioSeqTools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.3/LICENSE` & `JBioSeqTools-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.3/PKG-INFO` & `JBioSeqTools-2.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: JBioSeqTools
-Version: 2.0.3
+Version: 2.0.4
 Summary: JBioSeqTools
 Author: Jakub Kubis
 Author-email: jbiosystem@gmail.com
 License: MIT
 Keywords: sequence,optimization,vectors,AAV,GC,restriction enzyme
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `JBioSeqTools-2.0.3/README.md` & `JBioSeqTools-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.3/jbst/__init__.py` & `JBioSeqTools-2.0.4/jbst/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
                                     __/ |                                   
                                    |___/                                   
 """
 
 print(pattern)
 
 print('')
-print('Welcome in JBioSeqTools v.2.0.3 library')
+print('Welcome in JBioSeqTools v.2.0.4 library')
 print('')
 print('Loading required packages...')
 
 
 
 
 import os
```

### Comparing `JBioSeqTools-2.0.3/jbst/data/backbone.xlsx` & `JBioSeqTools-2.0.4/jbst/data/backbone.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.3/jbst/data/codons.xlsx` & `JBioSeqTools-2.0.4/jbst/data/codons.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.3/jbst/data/enzymes.xlsx` & `JBioSeqTools-2.0.4/jbst/data/enzymes.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.3/jbst/data/fluorescent_tag.xlsx` & `JBioSeqTools-2.0.4/jbst/data/fluorescent_tag.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.3/jbst/data/linkers.xlsx` & `JBioSeqTools-2.0.4/jbst/data/linkers.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.3/jbst/data/polya.xlsx` & `JBioSeqTools-2.0.4/jbst/data/polya.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.3/jbst/data/promoters.xlsx` & `JBioSeqTools-2.0.4/jbst/data/promoters.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.3/jbst/data/regulators.xlsx` & `JBioSeqTools-2.0.4/jbst/data/regulators.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.3/jbst/data/restriction_enzymes.xlsx` & `JBioSeqTools-2.0.4/jbst/data/restriction_enzymes.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.3/jbst/data/rnai_scoring.xlsx` & `JBioSeqTools-2.0.4/jbst/data/rnai_scoring.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.3/jbst/data/selectors.xlsx` & `JBioSeqTools-2.0.4/jbst/data/selectors.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.3/jbst/data/sh_loops.xlsx` & `JBioSeqTools-2.0.4/jbst/data/sh_loops.xlsx`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.3/jbst/data/vector_capacity.xlsx` & `JBioSeqTools-2.0.4/jbst/data/vector_capacity.xlsx`

 * *Files 17% similar despite different names*

```diff
@@ -103,68 +103,68 @@
 00000660: d542 53ed ad86 b0b7 37a0 ea93 cf9b 7fd7  .BS.....7.......
 00000670: 96a6 e90d 3f88 394c ecd2 9915 c873 6267  ....?.9L.....sbg
 00000680: d9ae 7cc8 6c21 f5f9 1a55 5368 3969 b062  ..|.l!...USh9i.b
 00000690: 9e72 3a22 795f 646c c0f3 449b bf13 fd7c  .r:"y_dl..D....|
 000006a0: 2d4e 9cc8 5222 3412 f832 cf47 c725 a0f5  -N..R"4..2.G.%..
 000006b0: 7f5a b434 f1cb 9d79 c437 09c3 abc8 f0c9  .Z.4...y.7......
 000006c0: 828b 1fa8 de01 0000 ffff 0300 504b 0304  ............PK..
-000006d0: 1400 0600 0800 0000 2100 e553 dd52 f002  ........!..S.R..
-000006e0: 0000 ce06 0000 0f00 0000 786c 2f77 6f72  ..........xl/wor
-000006f0: 6b62 6f6f 6b2e 786d 6cac 55db 6ea3 3010  kbook.xml.U.n.0.
-00000700: 7d5f 69ff 01f9 9d82 09a1 092a ad42 48b5  }_i........*.BH.
-00000710: 95da dda8 dbcb 4ba4 ca05 2758 019b b54d  ......K...'X...M
-00000720: 92b6 eabf ef18 427a c94b b75d 94d8 8c07  ......Bz.K.]....
-00000730: 8ecf cc1c 0f47 279b b2b0 5654 2a26 7884  .....G'...VT*&x.
-00000740: f081 8b2c ca53 9131 be88 d0f5 d5a9 3d40  ...,.S.1......=@
-00000750: 96d2 8467 a410 9c46 e881 2a74 72fc fddb  ...g...F..*tr...
-00000760: d15a c8e5 bd10 4b0b 00b8 8a50 ae75 153a  .Z....K....P.u.:
-00000770: 8e4a 735a 1275 202a cac1 3317 b224 1a4c  .JsZ.u *..3..$.L
-00000780: b970 5425 29c9 544e a92e 0bc7 73dd c029  .pT%).TN....s..)
-00000790: 09e3 a845 08e5 4730 c47c ce52 9a88 b42e  ...E..G0.|.R....
-000007a0: 29d7 2d88 a405 d140 5fe5 ac52 1d5a 997e  ).-....@_..R.Z.~
-000007b0: 04ae 2472 5957 762a ca0a 20ee 59c1 f443  ..$rYWv*.. .Y..C
-000007c0: 038a ac32 0dcf 165c 4872 5f40 d81b dcb7  ...2...\Hr_@....
-000007d0: 3612 7e01 fcb1 0b83 d7ed 04ae bdad 4a96  6.~...........J.
-000007e0: 4aa1 c45c 1f00 b4d3 92de 8b1f bb0e c66f  J..\...........o
-000007f0: 52b0 d9cf c1c7 907c 47d2 1533 35dc b192  R......|G..35...
-00000800: c127 5905 3bac e005 0cbb 5f46 c320 ad46  .'Y.;....._F. .F
-00000810: 2b21 24ef 9368 fd1d 370f 1d1f cd59 416f  +!$..h..7....YAo
-00000820: 5ae9 5aa4 aa7e 92d2 54aa 4056 4194 9e64  Z.Z..~..T.@VA..d
-00000830: 4cd3 2c42 8760 8a35 7d59 80a8 645d c535  L.,B.`.5}Y..d].5
-00000840: 2bc0 eb05 43cf 47ce f14e ce53 0906 d47e  +...C.G..N.S...~
-00000850: 5468 2a39 d174 2cb8 06a9 6da9 7f55 560d  Th*9.t,...m..UV.
-00000860: f638 1720 62eb 92fe a999 a470 7640 4210  .8. b......pv@B.
-00000870: 0e8c 240d c9bd 9a12 9d5b b52c 2234 0e67  ..$......[.,"4.g
-00000880: d70a 229c 9554 92c5 ec17 a789 642b 3a9b  .."..T......d+:.
-00000890: d645 c5f4 6c14 5fdc c1a9 226b f198 11ce  .E..l._..."k....
-000008a0: e8ec 9526 c9fe 01f8 0755 92d4 24c5 8144  ...&.....U..$..D
-000008b0: b464 dbfb f749 01ce 32ec 9437 d5d2 82fb  .d...I..2..7....
-000008c0: b3e4 1cb2 ff9b aca0 1650 f16c 7b54 cf20  .........P.l{T. 
-000008d0: d9b8 77c7 5319 e2bb a724 ee8f 8678 806d  ..w.S....$...x.m
-000008e0: 2f1e 8c6c dfeb f9f6 2098 0c6c 7712 8fe2  /..l.... ..lw...
-000008f0: c304 0f5c 0f3f 4330 3208 5341 6a9d 6fcb  ...\.?C02.SAj.o.
-00000900: 6ca0 23e4 434d f75c 1764 d379 b01b d62c  l.#.CM.\.d.y...,
-00000910: 7ba1 f1e4 6e2f dbcc ef86 cef7 6c02 360d  {...n/......l.6.
-00000920: ed86 d1b5 7a11 8431 adcd 2de3 9958 47c8  ....z..1..-..XG.
-00000930: c62e 34c4 87b7 e6ba 71de b24c e7a0 a89e  ..4.....q..L....
-00000940: d707 89b5 6b3f 285b e4c0 187b be59 04e1  ....k?([...{.Y..
-00000950: 1b66 117a c328 6919 9dc2 659b e10d 23e7  .f.z.(i...e...#.
-00000960: 15a5 a675 02b5 66b6 7823 f711 3430 f588  ...u..f.x#..40..
-00000970: a149 9bbe da64 19f4 1d9a 4de4 5986 9b2a  .I...d....M.Y..*
-00000980: 76ef a5a4 48a7 d232 53f3 60e0 0d71 cf3c  v...H..2S.`..q.<
-00000990: 4137 fa5c e966 06dd 31e0 877d 7774 e80e  A7.\.f..1..}wt..
-000009a0: 7da8 48af 6ffb 83a1 670f fc9e 678f fdc4  }.H.o...g...g...
-000009b0: 9bf4 0f27 c924 ee9b 0299 de1f fe8f 0ed8  ...'.$..........
-000009c0: c83f ec3e 2a86 654e a4be 9224 5dc2 a7e8  .?.>*.eN...$]...
-000009d0: 92ce 63a2 4051 6d40 c017 04d9 b176 bab7  ..c.@Qm@.....v..
-000009e0: 8eff 0200 00ff ff03 0050 4b03 0414 0006  .........PK.....
-000009f0: 0008 0000 0021 0081 3e94 97f3 0000 00ba  .....!..>.......
-00000a00: 0200 001a 0008 0178 6c2f 5f72 656c 732f  .......xl/_rels/
-00000a10: 776f 726b 626f 6f6b 2e78 6d6c 2e72 656c  workbook.xml.rel
-00000a20: 7320 a204 0128 a000 0100 0000 0000 0000  s ...(..........
+000006d0: 1400 0600 0800 0000 2100 30df 7278 e802  ........!.0.rx..
+000006e0: 0000 c306 0000 0f00 0000 786c 2f77 6f72  ..........xl/wor
+000006f0: 6b62 6f6f 6b2e 786d 6cac 554d 6fa3 3010  kbook.xml.UMo.0.
+00000700: bdaf b4ff 01f9 4ec1 8490 0495 5469 4876  ......N.....TiHv
+00000710: 23b5 aba8 9f97 4895 034e f006 30b5 4d93  #.....H..N..0.M.
+00000720: 6ed5 ffbe 6308 49d3 5cba ed22 b019 0f3c  n...c.I.\.."...<
+00000730: bf99 790c a767 9b2c 359e a890 8ce7 01c2  ..y..g.,5.......
+00000740: 2736 3268 1ef1 98e5 cb00 ddde 8ccd 2e32  '62h...........2
+00000750: a422 794c 529e d300 3d53 89ce fadf bf9d  ."yLR...=S......
+00000760: aeb9 58cd 395f 1900 90cb 0025 4a15 be65  ..X.9_.....%J..e
+00000770: c928 a119 9127 bca0 3978 165c 6444 8129  .(...'..9x.\dD.)
+00000780: 9696 2c04 25b1 4c28 5559 6a39 b6ed 5919  ..,.%.L(UYj9..Y.
+00000790: 6139 aa11 7cf1 110c be58 b088 863c 2a33  a9..|....X...<*3
+000007a0: 9aab 1a44 d094 28a0 2f13 56c8 062d 8b3e  ...D..(./.V..-.>
+000007b0: 0297 11b1 2a0b 33e2 5901 1073 9632 f55c  ....*.3.Y..s.2.\
+000007c0: 8122 238b fcc9 32e7 82cc 5308 7b83 dbc6  ."#...2...S.{...
+000007d0: 46c0 e9c1 856d 189c 6627 701d 6d95 b148  F....m..f'p.m..H
+000007e0: 70c9 17ea 04a0 ad9a f451 fcd8 b630 3e48  p........Q...0>H
+000007f0: c1e6 3807 1f43 722d 419f 98ae e18e 95f0  ..8..Cr-A.......
+00000800: 3ec9 cadb 6179 7b30 6c7f 190d 83b4 2aad  >...ay{0l.....*.
+00000810: f890 bc4f a2b5 77dc 1cd4 3f5d b094 ded5  ...O..w...?]....
+00000820: d235 4851 fc22 99ae 548a 8c94 4835 8a99  .5HQ."..T...H5..
+00000830: a271 803a 60f2 35dd 2f40 54a2 2cce 4b96  .q.:`.5./@T.,.K.
+00000840: 82d7 e9b4 5b18 59fd 9d9c a702 0ca8 fd20  ....[.Y........ 
+00000850: 5554 e444 d121 cf15 486d 4bfd abb2 aab0  UT.D.!..HmK.....
+00000860: 8709 0711 1b57 f4b1 6482 c2b7 0312 8270  .....W..d......p
+00000870: 6024 914f e672 4a54 6294 220d d0d0 9fdd  `$.O.rJTb.".....
+00000880: 4a88 7096 5141 96b3 1f4c cdae e9e3 0de7  J.p.QA...L......
+00000890: e9ec f75c aa59 4c14 99bd 1122 3956 fd3f  ...\.YL...."9V.?
+000008a0: 4891 443a 1316 445f 33ac efdf 6702 880a  H.D:..D_3...g...
+000008b0: bf91 db54 0903 ee27 e105 a4fc 9a3c 4101  ...T...'.....<A.
+000008c0: a0cc f1f6 fb9c 4086 71eb 218f 848f 1f5e  ......@.q.!....^
+000008d0: dc71 673c 18b7 42b3 1bba 6dd3 ed0d 47e6  .qg<..B...m...G.
+000008e0: c00e 07a6 e775 7add 7068 7be3 8efd 0ac1  .....uz.ph{.....
+000008f0: 08cf 8f38 2955 b2ad ad86 0e90 0b85 3c72  ...8)U........<r
+00000900: 5d92 4de3 c1b6 5fb2 784f e3c5 de1e a69e  ].M..._.xO......
+00000910: df0d 8def 5507 acbb d81d a36b b957 8136  ....U......k.W.6
+00000920: 8dcd 3dcb 63be 0e90 896d e882 cf87 e6ba  ..=.c....m......
+00000930: 72de b358 2520 a396 d306 5dd5 6b3f 295b  r..X% ....].k?)[
+00000940: 26c0 183b ae5e 04b5 6b66 013a 6014 d68c  &..;.^..kf.:`...
+00000950: c670 987a 3860 64bd a154 f54b a056 cd46  .p.z8`d..T.K.V.F
+00000960: 5e69 7c00 5d4b fec1 d099 7533 adb2 0ca2  ^i|.]K....u3....
+00000970: f6f5 2662 1257 7ab6 9af7 2292 4653 61e8  ..&b.Wz...".FSa.
+00000980: a97a d073 7ab8 a5c3 a61b 7521 5535 83d8  .z.sz.....u!U5..
+00000990: 18f0 c3ae 3de8 d83d d7b4 472d 2850 b7e7  ....=..=..G-(P..
+000009a0: 985d b7e5 9843 3774 46ed ce28 1c9d b775  .]...C7tF..(...u
+000009b0: 8174 c3f7 ff47 dbab 34ef 377f 12cd 3221  .t...G..4.7...2!
+000009c0: 42dd 0812 ade0 ff73 4517 e744 82a2 ea80  B......sE..D....
+000009d0: 802f 08b2 616d 356f f5ff 0200 00ff ff03  ./..am5o........
+000009e0: 0050 4b03 0414 0006 0008 0000 0021 0081  .PK..........!..
+000009f0: 3e94 97f3 0000 00ba 0200 001a 0008 0178  >..............x
+00000a00: 6c2f 5f72 656c 732f 776f 726b 626f 6f6b  l/_rels/workbook
+00000a10: 2e78 6d6c 2e72 656c 7320 a204 0128 a000  .xml.rels ...(..
+00000a20: 0100 0000 0000 0000 0000 0000 0000 0000  ................
 00000a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -172,463 +172,462 @@
 00000ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b20: 0000 0000 0000 0000 00ac 524d 4bc4 3010  ..........RMK.0.
-00000b30: bd0b fe87 3077 9b76 1511 d974 2f22 ec55  ....0w.v...t/".U
-00000b40: eb0f 08c9 b429 db26 2133 7ef4 df1b 2aba  .....).&!3~...*.
-00000b50: 5d58 d64b 2f03 6f86 79ef cdc7 76f7 350e  ]X.K/.o.y...v.5.
-00000b60: e203 13f5 c12b a88a 1204 7a13 6cef 3b05  .....+....z.l.;.
-00000b70: 6fcd f3cd 0308 62ed ad1e 8247 0513 12ec  o.....b....G....
-00000b80: eaeb abed 0b0e 9a73 13b9 3e92 c82c 9e14  .......s..>..,..
-00000b90: 38e6 f828 2519 87a3 a622 44f4 b9d2 8634  8..(%...."D....4
-00000ba0: 6ace 3075 326a 73d0 1dca 4d59 decb b4e4  j.0u2js...MY....
-00000bb0: 80fa 8453 ecad 82b4 b7b7 209a 2966 e5ff  ...S...... .)f..
-00000bc0: b943 dbf6 069f 8279 1fd1 f319 0949 3c0d  .C.....y.....I<.
-00000bd0: 7900 d1e8 d421 2bf8 c145 f608 f2bc fc66  y....!+..E.....f
-00000be0: 4d79 ce6b c1a3 fa0c e51c ab4b 1eaa 353d  My.k.......K..5=
-00000bf0: 7c86 7420 87c8 471f 7f29 9273 e5a2 99bb  |.t ..G..).s....
-00000c00: 55ef e174 42fb ca29 bfdb f22c cbf4 ef66  U..tB..)...,...f
-00000c10: e4c9 c7d5 df00 0000 ffff 0300 504b 0304  ............PK..
-00000c20: 1400 0600 0800 0000 2100 7d60 1dbf e203  ........!.}`....
-00000c30: 0000 940c 0000 1800 0000 786c 2f77 6f72  ..........xl/wor
-00000c40: 6b73 6865 6574 732f 7368 6565 7431 2e78  ksheets/sheet1.x
-00000c50: 6d6c 9c92 c96e c230 1086 ef95 fa0e 96ef  ml...n.0........
-00000c60: c409 505a 2202 aa8a da72 a854 75bb 1b67  ..PZ"....r.Tu..g
-00000c70: 422c bca4 b6d9 54f5 dd3b 0965 91b8 20a2  B,....T..;.e.. .
-00000c80: c49e 78f9 fe19 fb1f 8cd6 5a91 2538 2fad  ..x.......Z.%8/.
-00000c90: c968 12c5 9480 1136 9766 96d1 cf8f c7d6  .h.....6.f......
-00000ca0: 1d25 3e70 9373 650d 6474 039e 8e86 d757  .%>p.se.dt.....W
-00000cb0: 8395 7573 5f02 0482 04e3 335a 8650 a58c  ..us_.....3Z.P..
-00000cc0: 7951 82e6 3eb2 1518 9c29 acd3 3ce0 af9b  yQ..>....)..<...
-00000cd0: 315f 39e0 79b3 492b d68e e31e d35c 1aba  1_9.y.I+.....\..
-00000ce0: 25a4 ee1c 862d 0a29 606c c542 8309 5b88  %....-.)`l.B..[.
-00000cf0: 03c5 03e6 ef4b 59f9 1d4d 8b73 709a bbf9  .....KY..M.sp...
-00000d00: a26a 09ab 2b44 4ca5 9261 d340 29d1 229d  .j..+DL..a.@).".
-00000d10: cc8c 757c aab0 ee75 d2e5 82ac 1dbe 6dfc  ..u|...u......m.
-00000d20: 3a3b 9966 fc44 494b e1ac b745 8890 ccb6  :;.f.DIK...E....
-00000d30: 399f 96df 677d c6c5 9e74 5aff 5998 a4cb  9...g}...tZ.Y...
-00000d40: 1c2c 657d 8107 54fb b294 929b 3dab 7d80  .,e}..T.....=.}.
-00000d50: 752e 84f5 f6b0 fab8 5cba 9079 467f e2ff  u.......\..yF...
-00000d60: a785 7d52 37f1 a1d9 cdfd d2e1 2097 78c3  ..}R7....... .x.
-00000d70: 7555 c441 91d1 fb24 7dba a56c 3868 fcf3  uU.A...$}..l8h..
-00000d80: 2561 e58f 6212 f8f4 1d14 8800 a891 5052  %a..b.........PR
-00000d90: db73 6aed bc5e 38c1 a118 89be 5950 13b9  .sj..^8.....YP..
-00000da0: 0872 090f a054 465f 6ed0 e1df 8d06 8628  .r...TF_n......(
-00000db0: c0f6 0ac7 f14e edb1 31f4 ab23 3914 7ca1  .....N..1..#9.|.
-00000dc0: c29b 5d3d 839c 9501 65bb 5117 0bad 9d92  ..]=....e.Q.....
-00000dd0: e69b 3178 8116 45e9 a883 d83f 0000 00ff  ..1x..E....?....
-00000de0: ff00 0000 ffff 9c96 ed6e 8230 1486 6f85  .........n.0..o.
-00000df0: f402 8416 f163 4192 01e2 7510 46e2 2fb7  .....cA...u.F./.
-00000e00: 8871 dbdd afd5 61ed fb1e dce2 3f83 cf29  .q....a.....?..)
-00000e10: edd3 735e cd87 7ddf 9fea f6d4 16f9 f1fd  ..s^..}.........
-00000e20: 333a 6e94 56d1 f0d1 1e06 fbe9 65a9 a2fd  3:n.V.......e...
-00000e30: 69a3 d2f5 6ca1 a22f 3d6f bb97 b7ef ba1f  i...l../=o......
-00000e40: bafe 601f 27b3 5415 79e7 8a5e 5dd5 a5d6  ..`.'.T.y..^]...
-00000e50: 3e1f ecd3 73a1 5779 7c2e f2b8 fb45 4a01  >...s.Wy|....EJ.
-00000e60: 5986 4825 208b 10a9 0524 0b91 ad80 ac43  Y.H% ....$.....C
-00000e70: a461 c4e8 10d9 3192 dc88 d8ba ba09 33a1  .a....1.......3.
-00000e80: b087 9a1c 1b6a 3273 d0c4 08ec ac12 1601  .....j2s........
-00000e90: 4923 e1ee 6195 247e e397 cbda f202 29f8  I#..a.$~......).
-00000ea0: 6102 b6b9 63c2 5f43 a027 e57e cacc 6cf5  a...c._C.'.~..l.
-00000eb0: 473f b92a 1005 d75c 3202 bd52 3101 0d57  G?.*...\2..R1..W
-00000ec0: 8f84 1395 b128 5e00 9aba 6142 1b68 2446  .....(^...aB.h$F
-00000ed0: 7c37 06a6 e64f 9972 5560 0a3c 948c a029  |7...O.rU`.<...)
-00000ee0: 26d0 d448 4c98 e205 d014 1364 8a91 0953  &..HL......d...S
-00000ef0: d953 a65c d546 d9c6 bd65 9481 5396 57c4  .S.\.F...e..S.W.
-00000f00: 8ebe 8f31 8828 8180 f9ac c7f7 3855 46e8  ...1.(......8UF.
-00000f10: 2a61 1f30 a10d 2324 8b37 3231 8036 ba31  *a.0..#$.721.6.1
-00000f20: d0ff 3180 ae0a da0a 42a2 6444 c339 2a01  ..1.....B.dD.9*.
-00000f30: 415b 2332 65eb fe7b 9d40 0834 c20b 70fe  A[#2e..{.@.4..p.
-00000f40: 04c4 9f24 1840 fb73 776f ea61 923b 16fc  ...$.@.swo.a.;..
-00000f50: c08b 4b46 30c9 8545 20c9 4762 22c9 7901  ..KF0..E .Gb".y.
-00000f60: 4c72 2630 c985 6d7a e4ea 27f6 7f13 7e00  Lr&0..mz..'...~.
-00000f70: 0000 ffff 0000 00ff ff34 8fcd 4ec3 400c  .........4..N.@.
-00000f80: 845f 65e5 07e8 4f08 54a9 b2bd d04b 0e48  ._e...O.T....K.H
-00000f90: 487d 82a5 71b2 1665 6d39 2e88 3c3d 0e6a  H}..q..em9..<=.j
-00000fa0: 6e9e b134 f34d 2b99 0b1a 5ddf 350c 5cac  n..4.M+...].5.\.
-00000fb0: eb23 5410 ec57 3042 e157 2edf a813 7181  .#T..W0B.W....q.
-00000fc0: eda9 9534 e25b d291 ca14 6e38 5884 dde6  ...4.[....n8X...
-00000fd0: 0041 69cc eb6d 2cff ee33 840f 36e3 af55  .Ai..m,..3..6..U
-00000fe0: 654c 3dea a29e c09b d856 f1c8 bda0 dd25  eL=......V.....%
-00000ff0: 4812 d40b cd5e de40 6025 2c96 cceb 2308  H....^.@`%,...#.
-00001000: ab69 2283 90dd 9f9d 35dd ce42 11ea aaa9  .i".....5..B....
-00001010: 9b97 43d5 78b0 c3fa 96c7 63e7 6847 f241  ..C.x.....c.hG.A
-00001020: daf5 fb85 7ffb c3fa 3965 443b fd01 0000  ........9eD;....
-00001030: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00001040: 2100 4d3f 802c 8406 0000 801a 0000 1300  !.M?.,..........
-00001050: 0000 786c 2f74 6865 6d65 2f74 6865 6d65  ..xl/theme/theme
-00001060: 312e 786d 6cec 59cf 6fdb 3614 be0f d8ff  1.xml.Y.o.6.....
-00001070: 20e8 ee5a b625 d90e ea14 b66c 276b 93b6   ..Z.%.....l'k..
-00001080: 68dc 0e3d d236 6db1 a144 43a4 931a 4581  h..=.6m..DC...E.
-00001090: 5d77 1930 a01b 7619 b0db 0ec3 8002 db69  ]w.0..v........i
-000010a0: 97fd 372d b6ee 8fd8 2325 5b64 4c37 fd91  ..7-....#%[dL7..
-000010b0: 02dd d018 0824 ea7b 8f1f df7b faf8 43d7  .....$.{...{..C.
-000010c0: 6f3c 4ea8 7386 334e 58da 716b d73c d7c1  o<N.s.3NX.qk.<..
-000010d0: e984 4d49 3aef b8f7 47c3 4acb 75b8 40e9  ..MI:...G.J.u.@.
-000010e0: 1451 96e2 8ebb c2dc bdb1 fff9 67d7 d19e  .Q..........g...
-000010f0: 8871 821d b04f f91e eab8 b110 8bbd 6a95  .q...O........j.
-00001100: 4fa0 19f1 6b6c 8153 7836 6359 8204 dc66  O...kl.Sx6cY...f
-00001110: f3ea 3443 e7e0 37a1 d5ba e785 d504 91d4  ..4C..7.........
-00001120: 7552 9480 db3b b319 9960 6724 5dba fb6b  uR...;...`g$]..k
-00001130: e703 0ab7 a9e0 b261 42b3 13e9 1a1b 160a  .......aB.......
-00001140: 3b3d ad49 045f f188 66ce 19a2 1d17 fa99  ;=.I._..f.......
-00001150: b2f3 117e 2c5c 8722 2ee0 41c7 f5d4 9f5b  ...~,\."..A....[
-00001160: ddbf 5e45 7b85 1115 3b6c 35bb a1fa 2bec  ..^E{...;l5...+.
-00001170: 0a83 e969 5df5 99cd c79b 4e7d 3ff0 c3ee  ...i].....N}?...
-00001180: c6bf 0250 b18d 1b34 07e1 20dc f853 0034  ...P...4.. ..S.4
-00001190: 99c0 4873 2eba cfa0 d7ee f583 02ab 81f2  ..Hs............
-000011a0: 4b8b ef7e b3df a819 78cd 7f63 8b73 3790  K..~....x..c.s7.
-000011b0: 3f03 af40 b97f 7f0b 3f1c 4610 4503 af40  ?..@....?.F.E..@
-000011c0: 393e b0c4 a459 8f7c 03af 4039 3edc c237  9>...Y.|..@9>..7
-000011d0: bd6e df6f 1a78 058a 2949 4fb7 d05e 1036  .n.o.x..)IO..^.6
-000011e0: a2f5 6837 9019 a387 5678 3bf0 87cd 7ae1  ..h7....Vx;...z.
-000011f0: bc44 4135 6caa 4b76 3163 a9d8 556b 097a  .DA5l.Kv1c..Uk.z
-00001200: c4b2 2100 2490 2241 5247 ac16 7886 2650  ..!.$."ARG..x.&P
-00001210: c511 a264 9c11 e788 cc63 28bc 054a 1987  ...d.....c(..J..
-00001220: 66af ee0d bd06 fc97 3f5f 5da9 88a0 3d8c  f.......?_]...=.
-00001230: 346b c90b 98f0 ad26 c9c7 e193 8c2c 44c7  4k.....&.....,D.
-00001240: bd09 5e5d 0df2 70e9 1c30 1193 49d1 ab72  ..^]..p..0..I..r
-00001250: 6258 1ca2 74ae 5bbc faf9 db7f 7efc caf9  bX..t.[.....~...
-00001260: fbb7 9f5e 3dfb 2eef f422 9eeb f897 bf7e  ...^=....".....~
-00001270: fdf2 8f3f 5fe7 1ec6 5a06 e1c5 f7cf 5ffe  ...?_...Z....._.
-00001280: fefc c50f dffc f5cb 338b f76e 86c6 3a7c  ........3..n..:|
-00001290: 4412 cc9d dbf8 dcb9 c712 189a 853f 1e67  D............?.g
-000012a0: 6f67 318a 1131 2c50 0cbe 2dae 0710 381d  og1..1,P..-...8.
-000012b0: 787b 85a8 0dd7 c366 081f 64a0 2f36 e0c1  x{.....f..d./6..
-000012c0: f291 c1f5 24ce 9682 587a be15 2706 f098  ....$...Xz..'...
-000012d0: 31da 6399 3500 b764 5f5a 8447 cb74 6eef  1.c.5..d_Z.G.tn.
-000012e0: 3c5b eab8 7b08 9dd9 fa8e 506a 2478 b05c  <[..{.....Pj$x.\
-000012f0: 80b0 129b cb28 c606 cdbb 14a5 02cd 718a  .....(........q.
-00001300: 8523 9fb1 538c 2da3 7b48 8811 d763 32c9  .#..S.-.{H...c2.
-00001310: 1867 33e1 3c24 4e0f 116b 4846 646c 1452  .g3.<$N..kHFdl.R
-00001320: 6974 4812 c8cb ca46 1052 6dc4 e6f8 81d3  itH....F.Rm.....
-00001330: 63d4 36ea 3e3e 3391 f05a 206a 213f c2d4  c.6.>>3..Z j!?..
-00001340: 08e3 015a 0a94 d85c 8e50 42f5 801f 2111  ...Z...\.PB...!.
-00001350: db48 9eac b289 8e1b 7001 999e 63ca 9cc1  .H......p...c...
-00001360: 1473 6eb3 b993 c178 b5a4 df02 6db1 a7fd  .sn....x....m...
-00001370: 98ae 1213 9909 726a f379 8418 d391 7d76  ......rj.y....}v
-00001380: 1ac5 2859 5839 9334 d6b1 5ff0 5328 51e4  ..(YX9.4.._.S(Q.
-00001390: dc65 c206 3f66 e61b 22ef 210f 28dd 99ee  .e..?f..".!.(...
-000013a0: 0704 1be9 be5c 08ee 83ac ea94 ca02 914f  .....\.........O
-000013b0: 9699 2597 0798 99ef e38a ce10 562a 03aa  ..%.........V*..
-000013c0: 6f88 7942 d24b 95fd 82a6 071f 5ad3 edea  o.yB.K......Z...
-000013d0: 7c05 6a6e 77fc 3e3a decd 88f5 6d3a bca0  |.jnw.>:....m:..
-000013e0: debb 70ff 41cd eea3 657a 17c3 6bb2 3d67  ..p.A...ez..k.=g
-000013f0: 7d92 ec4f 92ed feef 257b d7bb 7cf5 425d  }..O....%{..|.B]
-00001400: 6a33 c876 b93e 57ab f564 e762 7d46 283d  j3.v.>W..d.b}F(=
-00001410: 112b 8a8f b85a af73 9891 a643 6854 1b09  .+...Z.s...ChT..
-00001420: b59b dc6c de16 315c 165b 0303 37cf 90b2  ...l..1\.[..7...
-00001430: 7132 26be 2422 3e89 d102 16f5 35b5 f59c  q2&.$">.....5...
-00001440: f3c2 f59c 3b0b c661 adaf 9ad5 2618 5ff0  ....;..a....&._.
-00001450: ad76 0ccb e498 4df3 3d6a ad26 f7a3 b978  .v....M.=j.&...x
-00001460: 7024 ca76 2fd8 b4c3 fe42 e4e8 b059 eebb  p$.v/....B...Y..
-00001470: 36ee d54e 76ae f6c7 6b02 d2f6 6d48 689d  6..Nv...k...mHh.
-00001480: 9924 1a16 12cd 7523 64e1 7524 d4c8 ae84  .$....u#d.u$....
-00001490: 45db c2a2 25dd af53 b5ce e226 1440 6d93  E...%..S...&.@m.
-000014a0: 1558 3239 b0d0 eab8 819f effd 611b 8528  .X29........a..(
-000014b0: 9eca 3ce5 c700 ebec cae4 5c69 a677 0593  ..<.......\i.w..
-000014c0: ea15 00eb 8775 0594 996e 4bae 3b87 2747  .....u...nK.;.'G
-000014d0: 9797 da1b 64da 20a1 959b 4942 2bc3 184d  ....d. ...IB+..M
-000014e0: 7151 9dfa 61c9 55e6 ba5d a6d4 a027 43b1  qQ..a.U..]...'C.
-000014f0: 7e1b 4a1a cdd6 87c8 b514 910b da40 535d  ~.J..........@S]
-00001500: 2968 ea9c 77dc b011 c079 d804 2d3a ee0c  )h..w....y..-:..
-00001510: f6fa 7099 2ca0 76b8 5cea 223a 8703 b389  ..p.,.v.\.":....
-00001520: c8f2 17fe 5d94 6591 71d1 473c ce03 ae44  ....].e.q.G<...D
-00001530: 2757 8384 089c 3994 241d 570e 7f53 0d34  'W....9.$.W..S.4
-00001540: 551a a2b8 d5ea 2008 1f2d b936 c8ca c746  U..... ..-.6...F
-00001550: 0e92 6e26 19cf 6678 22f4 b46b 2d32 d2f9  ..n&..fx"..k-2..
-00001560: 2d28 7cae 15d6 a7ca fcdd c1d2 922d 21dd  -(|..........-!.
-00001570: 27f1 f4dc 19d3 6576 0f41 8905 cd9a 0ce0  '.....ev.A......
-00001580: 9470 38f2 a9e5 d19c 1238 c3dc 0859 597f  .p8......8...YY.
-00001590: 1726 a642 76f5 4344 5543 793b a28b 1815  .&.Bv.CDUCy;....
-000015a0: 338a 2ee6 395c 89e8 868e badb c440 bb2b  3...9\.......@.+
-000015b0: c60c 01dd 0ee1 782e 27d8 f79e 752f 9faa  ......x.'...u/..
-000015c0: 65e4 34d1 2ce7 4c43 55e4 ac69 17d3 0f37  e.4.,.LCU..i...7
-000015d0: c96b acca 49d4 6095 4bb7 da36 f052 ebda  .k..I.`.K..6.R..
-000015e0: 6bad 8342 b5ce 1297 ccba 6f30 2168 d4ca  k..B......o0!h..
-000015f0: ce0c 6a92 f1b6 0c4b cd2e 5a4d 6a57 b820  ..j....K..ZMjW. 
-00001600: d022 11ee 88db 668e b046 e25d 677e b0bb  ."....f..F.]g~..
-00001610: 58b5 7282 58af 2b55 e1ab 8f1d faf7 0836  X.r.X.+U.......6
-00001620: 7e04 e2d1 8793 df25 155c a512 be36 6408  ~......%.\...6d.
-00001630: 167d f9d9 712e 1bf0 8a3c 16c5 1a11 ae9c  .}..q....<......
-00001640: 6546 3aee 132f e8fa 513d 882a 5e2b 1854  eF:../..Q=.*^+.T
-00001650: fc86 ef55 5a41 b751 e906 41a3 3608 6a5e  ...UZA.Q..A.6.j^
-00001660: bf57 7f0a 138b 8893 5a90 7f68 19c2 1114  .W......Z..h....
-00001670: 5d15 9f5b 54fb d627 9764 7dca 766d c292  ]..[T..'.d}.vm..
-00001680: 2a53 9f54 aa8a b8fa e452 abef fee4 e210  *S.T.....R......
-00001690: 109d 2761 7dd8 6eb4 7b61 a5dd e80e 2b7e  ..'a}.n.{a....+~
-000016a0: bfd7 aab4 a3b0 57e9 8751 b33f ec47 41ab  ......W..Q.?.GA.
-000016b0: 3d7c ea3a 670a ec77 1b91 1f0e 5a95 b016  =|.:g..w....Z...
-000016c0: 4515 3ff4 24fd 56bb d2f4 ebf5 aedf ecb6  E.?.$.V.........
-000016d0: 067e f769 b18c 8191 e7f2 51c4 02c2 ab78  .~.i......Q....x
-000016e0: edff 0b00 00ff ff03 0050 4b03 0414 0006  .........PK.....
-000016f0: 0008 0000 0021 0045 9ea9 ab6d 0300 0095  .....!.E...m....
-00001700: 0900 000d 0000 0078 6c2f 7374 796c 6573  .......xl/styles
-00001710: 2e78 6d6c ac56 db8e db36 107d 2f90 7f20  .xml.V...6.}/.. 
-00001720: f8ae d5c5 966b 1b92 82f5 7a05 0448 8302  .....k....z..H..
-00001730: bb05 fa4a 4b94 4c84 1781 a237 7282 fe7b  ...JK.L....7r..{
-00001740: 8694 6469 9b4d 6bb8 f58b c8e1 cce1 990b  ..di.Mk.........
-00001750: 679c bcef 0447 2f54 b74c c914 8777 0146  g....G/T.L...w.F
-00001760: 5416 aa64 b24e f11f cfb9 b7c6 a835 4496  T..d.N.......5D.
-00001770: 842b 4953 7ca6 2d7e 9fbd fb25 69cd 99d3  .+IS|.-~...%i...
-00001780: a723 a506 0184 6c53 7c34 a6d9 fa7e 5b1c  .#....lS|4...~[.
-00001790: a920 ed9d 6aa8 8493 4a69 410c 6c75 edb7  . ..j...JiA.lu..
-000017a0: 8da6 a46c ad91 e07e 1404 2b5f 1026 718f  ...l...~..+_.&q.
-000017b0: b015 c535 2082 e8cf a7c6 2b94 6888 6107  ...5 .....+.h.a.
-000017c0: c699 393b 2c8c 44b1 fd50 4ba5 c981 03d5  ..9;,.D..PK.....
-000017d0: 2e5c 9202 75e1 4a47 a8d3 e325 4efa c33d  .\..u.JG...%N..=
-000017e0: 8215 5ab5 aa32 7780 ebab aa62 05fd 91ee  ..Z..2w....b....
-000017f0: c6df f8a4 9890 00f9 36a4 30f6 83e8 95ef  ........6.0.....
-00001800: 9dbe 1169 e96b fac2 6cfa 7096 544a 9a16  ...i.k..l.p.TJ..
-00001810: 15ea 244d 8a17 40d4 8660 fb59 aa2f 32b7  ..$M..@..`.Y./2.
-00001820: 4790 e141 2b4b daaf e885 7090 84d8 cf92  G..A+K....p.....
-00001830: 4271 a591 81d4 41e4 9c44 1241 7b8d 07c2  Bq....A..D.A{...
-00001840: d941 33ab 5611 c1f8 b917 4756 e0b2 3de8  .A3.V.....GV..=.
-00001850: 0906 b1b7 42df f2e8 d9cc ee09 ecd1 847a  ....B..........z
-00001860: af19 e16f 62be 69be 7e6d 7d2b 2787 dd02  ...ob.i.~m}+'...
-00001870: 37c6 f92c 52bd 204b a0a4 0cd5 3287 5334  7..,R. K....2.S4
-00001880: ac9f cf0d 8444 42f5 f7ae c1d1 bf6a d79a  .....DB......j..
-00001890: 9cc3 28be dea0 559c 9536 35f5 834b 84ae  ..(...U..65..K..
-000018a0: 0f29 ce87 9f85 390c 074c 96b4 a365 8a57  .)....9..L...e.W
-000018b0: 4b87 3e23 6ce3 eec8 b90f f878 50ba 8497  K.>#l......xP...
-000018c0: 3dd6 4304 f8bd 284b 38ad 0ca0 6a56 1fed  =.C...(K8...jV..
-000018d0: d7a8 c6de a18c 81ea cf92 9291 5a49 c26d  ............ZI.m
-000018e0: 2a47 8bb9 2574 0478 fc29 3647 78bc 63ed  *G..%t.x.)6Gx.c.
-000018f0: fc9d 99bd 62b8 e12a 7dc7 c551 b94a 1d28  ....b..*}..Q.J.(
-00001900: 8f8c afd2 ef9d 7bdb b7c1 4908 5941 397f  ......{...I.YA9.
-00001910: b2ce fd59 5de2 669f 4c57 2179 12b9 301f  ...Y].f.LW!y..0.
-00001920: 20f4 d023 6d81 8f4b 88f9 b0ec 63d4 6f6c   ..#m..K....c.ol
-00001930: ece6 683d f60c 7671 132c eaaa 0bfe cf48  ..h=..vq.,.....H
-00001940: 85c0 6f20 1561 3491 02f9 688d 48d3 f0b3  ..o .a4...h.H...
-00001950: ed09 f6b5 0f3b b099 763b 573c d3fe 9eb3  .....;..v;W<....
-00001960: 5a0a da1b 6409 b484 7e8b 8e4a b3af 0064  Z...d...~..J...d
-00001970: 7b49 01e7 145a 2d0c 14c3 8ab9 e48b 26cd  {I...Z-.......&.
-00001980: 33ed dc75 3634 5df5 f3a0 cef8 43a8 afe6  3..u64].....C...
-00001990: ffff 321e 49ba 2442 da66 b5f1 aa32 2e39  ..2.I.$B.f...2.9
-000019a0: 46b6 b5a5 f893 9d77 5c9e 67b1 3e9c 1837  F......w\.g.>..7
-000019b0: 4cbe 5117 805a 7653 a5b9 0e69 ecf4 7235  L.Q..ZvS...i..r5
-000019c0: 78b9 07a2 50d2 8a9c b879 be1c a678 5aff  x...P....y...xZ.
-000019d0: 464b 7612 90eb 41eb 77f6 a28c 8348 f1b4  FKv...A.w....H..
-000019e0: fe68 1f7b b8b2 6d03 12f1 b185 d709 5f74  .h.{..m......._t
-000019f0: d22c c5df 1e77 bf6e f68f 79e4 ad83 ddda  .,...w.n..y.....
-00001a00: 5b2e 68ec 6de2 ddde 8b97 0fbb fd3e df04  [.h.m........>..
-00001a10: 51f0 f0d7 6c86 fe87 09ea 463e 643f 5c6e  Q...l.....F>d?\n
-00001a20: 5b0e 7356 0fce 0ee4 9f26 598a 679b 9ebe  [.sV.....&Y.g...
-00001a30: 6b7a 407b ce7d 13ad 82fb 380c bc7c 1184  kz@{.}....8..|..
-00001a40: de72 45d6 de7a b588 bd3c 0ea3 fd6a b97b  .rE..z...<...j.{
-00001a50: 8cf3 78c6 3dbe 71d2 067e 18f6 33db 928f  ..x.=.q..~..3...
-00001a60: b786 09ca 991c 7335 6668 2e85 24c1 f61f  ......s5fh..$...
-00001a70: 9cf0 c74c f8d3 ffa9 ec3b 0000 00ff ff03  ...L.....;......
-00001a80: 0050 4b03 0414 0006 0008 0000 0021 00fb  .PK..........!..
-00001a90: 9141 a072 0100 006d 0300 0014 0000 0078  .A.r...m.......x
-00001aa0: 6c2f 7368 6172 6564 5374 7269 6e67 732e  l/sharedStrings.
-00001ab0: 786d 6c8c 534d 6b1b 3110 bd07 fa1f 840e  xml.SMk.1.......
-00001ac0: 3d04 ec5d 3b21 9876 774d 6908 0d24 39b8  =..];!.vwMi..$9.
-00001ad0: 6e20 9462 a6ab e95a 208d b69a 5927 eeaf  n .b...Z ...Y'..
-00001ae0: 8f8c 0f05 ad09 39ee fbd8 379a 2755 cb17  ......9...7.'U..
-00001af0: efd4 0e23 db40 b59e 4d4b ad90 da60 2c75  ...#.@..MK...`,u
-00001b00: b5fe b1be 992c b462 0132 e002 61ad f7c8  .....,.b.2..a...
-00001b10: 7ad9 7c38 ab98 4525 2f71 adb7 22fd a7a2  z.|8..E%/q.."...
-00001b20: e076 8b1e 781a 7aa4 c4fc 09d1 83a4 cfd8  .v..x.z.........
-00001b30: 15dc 4704 c35b 44f1 ae98 97e5 55e1 c192  ..G..[D.....U...
-00001b40: 566d 1848 6a7d 39d7 6a20 fb77 c0af 4760  Vm.Hj}9.j .w..G`
-00001b50: bed0 4dc5 b6a9 a4b9 f57e 2054 2be4 3e10  ..M......~ T+.>.
-00001b60: 6355 4853 1507 ea48 7f17 f8ed 46e8 eae1  cUHS...H....F...
-00001b70: 4b2e 5c94 93d9 4599 a34f c839 7417 9e73  K.\...E..O.9t..s
-00001b80: 681d 81d8 2289 0a51 1d13 cf73 0da7 9539  h..."..Q...s...9
-00001b90: 4ccb 4a5a 8346 394b 0851 5d8f 2799 2d26  L.JZ.F9K.Q].'.-&
-00001ba0: f3ab dcfe 8871 afde 8ace 0d26 0ce9 e0ef  .....q.....&....
-00001bb0: c97b 08b9 f79b edb6 3976 1f0c 4690 d12a  .{......9v..F..*
-00001bc0: 5be8 a1b5 b2cf f51d 52f0 2335 bea4 aaf9  [.......R.#5....
-00001bd0: 709b 72fd 0e5b 0971 23fb 7e64 62fb 0f7f  p.r..[.q#.~db...
-00001be0: 92ff 955b 3e3a f9ac 66a3 ce8e c91b 4b82  ...[>:..f.....K.
-00001bf0: 5d9a f844 56c4 14b5 b311 5cfe 4b30 69ec  ]..DV.....\.K0i.
-00001c00: 938c 4bf5 da93 0c33 c06e 5477 7b02 8cd8  ..K....3.nTw{...
-00001c10: 0d2e 95de 3b60 6fcd 7f4f 919e 4bf3 0a00  ....;`o..O..K...
-00001c20: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00001c30: 0021 003b 6d32 4bc1 0000 0042 0100 0023  .!.;m2K....B...#
-00001c40: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-00001c50: 2f5f 7265 6c73 2f73 6865 6574 312e 786d  /_rels/sheet1.xm
-00001c60: 6c2e 7265 6c73 848f c18a c230 1445 f703  l.rels.....0.E..
-00001c70: fe43 787b 93d6 850c 4353 3722 b855 e703  .Cx{....CS7".U..
-00001c80: 62fa da06 db97 90f7 14fd 7bb3 1c65 c0e5  b.........{..e..
-00001c90: e570 cfe5 369b fb3c a91b 660e 912c d4ba  .p..6..<..f..,..
-00001ca0: 0285 e463 1768 b0f0 7bda 2dbf 41b1 38ea  ...c.h..{.-.A.8.
-00001cb0: dc14 092d 3c90 61d3 2ebe 9a03 4e4e 4a89  ...-<.a.....NNJ.
-00001cc0: c790 5815 0bb1 8551 24fd 18c3 7ec4 d9b1  ..X....Q$...~...
-00001cd0: 8e09 a990 3ee6 d949 8979 30c9 f98b 1bd0  ....>..I.y0.....
-00001ce0: acaa 6a6d f25f 07b4 2f4e b5ef 2ce4 7d57  ..jm._../N..,.}W
-00001cf0: 833a 3d52 59fe ec8e 7d1f 3c6e a3bf ce48  .:=RY...}.<n...H
-00001d00: f2cf 8449 3990 603e a248 39c8 45ed f280  ...I9.`>.H9.E...
-00001d10: 6241 eb77 f69e 6b7d 0e04 a66d cccb f3f6  bA.w..k}...m....
-00001d20: 0900 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-00001d30: 0000 0021 0094 258c 3ea4 0100 00b0 0f00  ...!..%.>.......
-00001d40: 0027 0000 0078 6c2f 7072 696e 7465 7253  .'...xl/printerS
-00001d50: 6574 7469 6e67 732f 7072 696e 7465 7253  ettings/printerS
-00001d60: 6574 7469 6e67 7331 2e62 696e ec57 cf4b  ettings1.bin.W.K
-00001d70: 4241 10fe de53 414d a463 27f1 5681 8702  BA...SAM.c'.V...
-00001d80: 838e 99d2 2188 c03c 782c b043 d00f c92e  ....!..<x,.C....
-00001d90: 9da2 ff20 e8d6 b953 7f8f 9720 e822 d41f  ... ...S... ."..
-00001da0: d035 ec1b 7572 5bf7 3d2f 81f0 d891 793b  .5..ur[.=/....y;
-00001db0: bb33 3b3b f3cd 1cc6 3a4e 7089 2b72 192d  .3;;....:Np.+r.-
-00001dc0: 3451 c516 36f8 2ba3 8753 5ce3 8cdf 1e77  4Q..6.+..S\....w
-00001dd0: 6ba8 d3aa 8b5b ca9b 5887 5290 ce17 ded0  k....[..X.R.....
-00001de0: 2fa6 deef 5301 7278 5aaa 663b 0850 0abe  /...S.rxZ.f;.P..
-00001df0: 8721 5790 03d4 e8f7 ff49 bc87 a317 e495  .!W......I......
-00001e00: 59ea 1781 ddfd c641 be30 d63d e481 578a  Y......A.0.=..W.
-00001e10: c2bf f153 c836 81f4 0d50 a193 16f9 f810  ...S.6...P......
-00001e20: 1874 67f7 b69d d87e 39ec f55c fdd9 76ed  .tg....~9..\..v.
-00001e30: b01d aea0 41b4 6bd8 23ea 8ba4 23d6 ff82  ....A.k.#...#...
-00001e40: 753d 679d a5b2 49a0 e5d5 44a4 e193 f008  u=g...I...D.....
-00001e50: 7804 3c02 1e81 0521 20b3 456a c212 c278  x.<....! .Ej...x
-00001e60: 9e71 0513 8eec 7ca1 3c02 5304 729c 86a7  .q....|.<.S.r...
-00001e70: fd23 bd64 539a 0732 b74a 8f95 28c8 2ae4  .#.dS..2.J..(.*.
-00001e80: 9a65 e55c f43a efda 761d 1ec8 7b3a a38a  .e.\.:..v...{:..
-00001e90: dede 6b0c e3a9 3cfa 9d49 1878 5481 eb0e  ..k...<..I.xT...
-00001ea0: 6767 bd57 31ce 4d51 f4c3 e15f 25af cd90  gg.W1.MQ..._%...
-00001eb0: 2bbf a89c cd3c 6ddf 36a6 ea23 ca97 898d  +....<m.6..#....
-00001ec0: d8dc 596c be25 f207 01b7 d271 661e 177b  ..Yl.%.....qf..{
-00001ed0: 0454 b198 b830 9358 e651 c630 506c cc7e  .T...0.X.Q.0Pl.~
-00001ee0: b1ef 7f4e 7cba 708b c256 7a56 49fb 212e  ...N|.p..VzVI.!.
-00001ef0: aeb8 5e73 e126 fea5 97e7 f914 bd19 8bda  ..^s.&..........
-00001f00: d713 fc7f 36b3 fdfc f203 0000 ffff 0300  ....6...........
-00001f10: 504b 0304 1400 0600 0800 0000 2100 c520  PK..........!.. 
-00001f20: 73fd 5401 0000 6902 0000 1100 0801 646f  s.T...i.......do
-00001f30: 6350 726f 7073 2f63 6f72 652e 786d 6c20  cProps/core.xml 
-00001f40: a204 0128 a000 0100 0000 0000 0000 0000  ...(............
+00000b20: 00ac 524d 4bc4 3010 bd0b fe87 3077 9b76  ..RMK.0.....0w.v
+00000b30: 1511 d974 2f22 ec55 eb0f 08c9 b429 db26  ...t/".U.....).&
+00000b40: 2133 7ef4 df1b 2aba 5d58 d64b 2f03 6f86  !3~...*.]X.K/.o.
+00000b50: 79ef cdc7 76f7 350e e203 13f5 c12b a88a  y...v.5......+..
+00000b60: 1204 7a13 6cef 3b05 6fcd f3cd 0308 62ed  ..z.l.;.o.....b.
+00000b70: ad1e 8247 0513 12ec eaeb abed 0b0e 9a73  ...G...........s
+00000b80: 13b9 3e92 c82c 9e14 38e6 f828 2519 87a3  ..>..,..8..(%...
+00000b90: a622 44f4 b9d2 8634 6ace 3075 326a 73d0  ."D....4j.0u2js.
+00000ba0: 1dca 4d59 decb b4e4 80fa 8453 ecad 82b4  ..MY.......S....
+00000bb0: b7b7 209a 2966 e5ff b943 dbf6 069f 8279  .. .)f...C.....y
+00000bc0: 1fd1 f319 0949 3c0d 7900 d1e8 d421 2bf8  .....I<.y....!+.
+00000bd0: c145 f608 f2bc fc66 4d79 ce6b c1a3 fa0c  .E.....fMy.k....
+00000be0: e51c ab4b 1eaa 353d 7c86 7420 87c8 471f  ...K..5=|.t ..G.
+00000bf0: 7f29 9273 e5a2 99bb 55ef e174 42fb ca29  .).s....U..tB..)
+00000c00: bfdb f22c cbf4 ef66 e4c9 c7d5 df00 0000  ...,...f........
+00000c10: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
+00000c20: 2100 4bd1 61e8 e003 0000 940c 0000 1800  !.K.a...........
+00000c30: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
+00000c40: 7368 6565 7431 2e78 6d6c 9c92 c96e c230  sheet1.xml...n.0
+00000c50: 1086 ef95 fa0e 96ef c409 505a 2202 aa8a  ..........PZ"...
+00000c60: 68b9 55dd eec6 9910 0b2f a96d 3655 7df7  h.U....../.m6U}.
+00000c70: 4e42 5924 2e88 28b1 275e be7f c6fe 07a3  NBY$..(.'^......
+00000c80: 8d56 6405 ce4b 6b32 9a44 3125 6084 cda5  .Vd..Kk2.D1%`...
+00000c90: 9967 f4f3 63d2 7aa0 c407 6e72 aeac 818c  .g..c.z...nr....
+00000ca0: 6ec1 d3d1 f0f6 66b0 b66e e14b 8040 9060  n.....f..n.K.@.`
+00000cb0: 7c46 cb10 aa94 312f 4ad0 dc47 b602 8333  |F....1/J..G...3
+00000cc0: 8575 9a07 fc75 73e6 2b07 3c6f 3669 c5da  .u...us.+.<o6i..
+00000cd0: 71dc 639a 4b43 7784 d45d c2b0 4521 058c  q.c.KCw..]..E!..
+00000ce0: ad58 6a30 6107 71a0 78c0 fc7d 292b bfa7  .Xj0a.q.x..})+..
+00000cf0: 6971 094e 73b7 5856 2d61 7585 8899 5432  iq.Ns.XV-au...T2
+00000d00: 6c1b 2825 5aa4 d3b9 b18e cf14 d6bd 49ba  l.(%Z.........I.
+00000d10: 5c90 8dc3 b78d 5f67 2fd3 8c9f 2969 299c  \....._g/...)i).
+00000d20: f5b6 0811 92d9 2ee7 f3f2 fbac cfb8 3890  ..............8.
+00000d30: ceeb bf08 9374 9983 95ac 2ff0 886a 5f97  .....t..../..j_.
+00000d40: 5272 7760 b58f b0ce 95b0 de01 561f 974b  Rrw`........V..K
+00000d50: 9732 cfe8 4ffc ffb4 b04f ea26 3e36 fbb9  .2..O....O.&>6..
+00000d60: 5f3a 1ce4 126f b8ae 8a38 2832 fa98 a4cf  _:...o...8(2....
+00000d70: f794 0d07 8d7f be24 acfd 494c 029f bd83  .......$..IL....
+00000d80: 0211 0035 124a 6a7b ceac 5dd4 0ba7 3814  ...5.Jj{..]...8.
+00000d90: 23d1 370b 6a22 1741 aee0 0994 cae8 b88b  #.7.j".A........
+00000da0: 0eff 6e34 3044 0176 5038 8df7 6a93 c6d0  ..n40D.vP8..j...
+00000db0: af8e e450 f0a5 0a6f 76fd 0272 5e06 94ed  ...P...ov..r^...
+00000dc0: 46c8 6a1c 91e6 db31 7881 1645 e9a8 83d8  F.j....1x..E....
+00000dd0: 3f00 0000 ffff 0000 00ff ff9c 96ed 6e82  ?.............n.
+00000de0: 3014 866f 85f4 0280 16f1 2b48 3240 bc0e  0..o......+H2@..
+00000df0: c248 fca5 8b18 b7dd fd5a 5dad 7ddf e216  .H.......Z].}...
+00000e00: ff19 7c4e 699f 9ef3 6a31 ee87 e1dc 74e7  ..|Ni...j1....t.
+00000e10: ae2c 4ec7 cfe8 b411 5244 e347 7718 f5a7  .,N.....RD.Gw...
+00000e20: f542 44fb f346 64ab 782e a22f 39eb faf5  .BD..Fd.x../9...
+00000e30: fb77 338c fd70 d08f d338 1365 d19b a237  .w3..p...8.e...7
+00000e40: 5375 add5 cf47 fdf4 52ca 6591 5cca 22e9  Su...G..R.e.\.".
+00000e50: 7f91 2a80 2c7c a40e 2073 1f69 0248 ee23  ..*.,|.. s.i.H.#
+00000e60: db00 b2f2 9196 1125 7d64 c748 7a27 12ed  .......%}d.Hz'..
+00000e70: ea2e 4cf9 c29e 6a32 acaf 49cd 4013 23b0  ..L...j2..I.@.#.
+00000e80: b33a b008 48b2 84b9 8765 9aba 8d5f 2f6b  .:..H....e..._/k
+00000e90: cb0b 64e0 8709 d8e6 8e09 770d 9e9e 8cfb  ..d.......w.....
+00000ea0: 2957 f1f2 8f7e 3255 200a aeb9 6204 7aa5  )W...~2U ...b.z.
+00000eb0: 6602 1aae b184 1195 b328 5e00 9aba 6542  f........(^...eB
+00000ec0: 2a68 2446 5c37 7aa6 662f 9932 5560 0a3c  *h$F\7z.f/.2U`.<
+00000ed0: 548c a029 26d0 9425 8c29 a555 c1cc f102  T..)&..%.).U....
+00000ee0: 688a 0932 c5c8 84a9 fc25 53a6 6a23 74e3  h..2.....%S.j#t.
+00000ef0: de33 4ac1 29ab 1ba2 47df c518 4454 8080  .3J.)...G...DT..
+00000f00: f96c ec7b ac2a 7415 d807 202d 2324 8b37  .l.{.*t... -#$.7
+00000f10: 3231 803a ba31 d0ff 3180 a60a da0a 42a2  21.:.1..1.....B.
+00000f20: 6244 c239 ea00 82b6 2c32 65eb f17b 9942  bD.9....,2e..{.B
+00000f30: 08b4 8117 e0fc 0510 7712 6f00 f5cf dda3  ........w.o.....
+00000f40: a9a7 496e 58f0 032f ae18 c124 0f2c 0249  ..InX../...$.,.I
+00000f50: 6e89 8924 e705 30c9 99c0 240f 6cd3 2137  n..$..0...$.l.!7
+00000f60: 3f89 fb9b f003 0000 ffff 0000 00ff ff34  ?..............4
+00000f70: 8fcd 4ec3 400c 845f 65e5 07e8 4f08 54a9  ..N.@.._e...O.T.
+00000f80: b2bd d04b 0e48 487d 82a5 71b2 1665 6d39  ...K.HH}..q..em9
+00000f90: 2e88 3c3d 0e6a 6e9e b134 f34d 2b99 0b1a  ..<=.jn..4.M+...
+00000fa0: 5ddf 350c 5cac eb23 5410 ec57 3042 e157  ].5.\..#T..W0B.W
+00000fb0: 2edf a813 7181 eda9 9534 e25b d291 ca14  ....q....4.[....
+00000fc0: 6e38 5884 dde6 0041 69cc eb6d 2cff ee33  n8X....Ai..m,..3
+00000fd0: 840f 36e3 af55 654c 3dea a29e c09b d856  ..6..UeL=......V
+00000fe0: f1c8 bda0 dd25 4812 d40b cd5e de40 6025  .....%H....^.@`%
+00000ff0: 2c96 cceb 2308 ab69 2283 90dd 9f9d 35dd  ,...#..i".....5.
+00001000: ce42 11ea aaa9 9b97 43d5 78b0 c3fa 96c7  .B......C.x.....
+00001010: 63e7 6847 f241 daf5 fb85 7ffb c3fa 3965  c.hG.A........9e
+00001020: 443b fd01 0000 ffff 0300 504b 0304 1400  D;........PK....
+00001030: 0600 0800 0000 2100 4d3f 802c 8406 0000  ......!.M?.,....
+00001040: 801a 0000 1300 0000 786c 2f74 6865 6d65  ........xl/theme
+00001050: 2f74 6865 6d65 312e 786d 6cec 59cf 6fdb  /theme1.xml.Y.o.
+00001060: 3614 be0f d8ff 20e8 ee5a b625 d90e ea14  6..... ..Z.%....
+00001070: b66c 276b 93b6 68dc 0e3d d236 6db1 a144  .l'k..h..=.6m..D
+00001080: 43a4 931a 4581 5d77 1930 a01b 7619 b0db  C...E.]w.0..v...
+00001090: 0ec3 8002 db69 97fd 372d b6ee 8fd8 2325  .....i..7-....#%
+000010a0: 5b64 4c37 fd91 02dd d018 0824 ea7b 8f1f  [dL7.......$.{..
+000010b0: df7b faf8 43d7 6f3c 4ea8 7386 334e 58da  .{..C.o<N.s.3NX.
+000010c0: 716b d73c d7c1 e984 4d49 3aef b8f7 47c3  qk.<....MI:...G.
+000010d0: 4acb 75b8 40e9 1451 96e2 8ebb c2dc bdb1  J.u.@..Q........
+000010e0: fff9 67d7 d19e 8871 821d b04f f91e eab8  ..g....q...O....
+000010f0: b110 8bbd 6a95 4fa0 19f1 6b6c 8153 7836  ....j.O...kl.Sx6
+00001100: 6359 8204 dc66 f3ea 3443 e7e0 37a1 d5ba  cY...f..4C..7...
+00001110: e785 d504 91d4 7552 9480 db3b b319 9960  ......uR...;...`
+00001120: 6724 5dba fb6b e703 0ab7 a9e0 b261 42b3  g$]..k.......aB.
+00001130: 13e9 1a1b 160a 3b3d ad49 045f f188 66ce  ......;=.I._..f.
+00001140: 19a2 1d17 fa99 b2f3 117e 2c5c 8722 2ee0  .........~,\."..
+00001150: 41c7 f5d4 9f5b ddbf 5e45 7b85 1115 3b6c  A....[..^E{...;l
+00001160: 35bb a1fa 2bec 0a83 e969 5df5 99cd c79b  5...+....i].....
+00001170: 4e7d 3ff0 c3ee c6bf 0250 b18d 1b34 07e1  N}?......P...4..
+00001180: 20dc f853 0034 99c0 4873 2eba cfa0 d7ee   ..S.4..Hs......
+00001190: f583 02ab 81f2 4b8b ef7e b3df a819 78cd  ......K..~....x.
+000011a0: 7f63 8b73 3790 3f03 af40 b97f 7f0b 3f1c  .c.s7.?..@....?.
+000011b0: 4610 4503 af40 393e b0c4 a459 8f7c 03af  F.E..@9>...Y.|..
+000011c0: 4039 3edc c237 bd6e df6f 1a78 058a 2949  @9>..7.n.o.x..)I
+000011d0: 4fb7 d05e 1036 a2f5 6837 9019 a387 5678  O..^.6..h7....Vx
+000011e0: 3bf0 87cd 7ae1 bc44 4135 6caa 4b76 3163  ;...z..DA5l.Kv1c
+000011f0: a9d8 556b 097a c4b2 2100 2490 2241 5247  ..Uk.z..!.$."ARG
+00001200: ac16 7886 2650 c511 a264 9c11 e788 cc63  ..x.&P...d.....c
+00001210: 28bc 054a 1987 66af ee0d bd06 fc97 3f5f  (..J..f.......?_
+00001220: 5da9 88a0 3d8c 346b c90b 98f0 ad26 c9c7  ]...=.4k.....&..
+00001230: e193 8c2c 44c7 bd09 5e5d 0df2 70e9 1c30  ...,D...^]..p..0
+00001240: 1193 49d1 ab72 6258 1ca2 74ae 5bbc faf9  ..I..rbX..t.[...
+00001250: db7f 7efc caf9 fbb7 9f5e 3dfb 2eef f422  ..~......^=...."
+00001260: 9eeb f897 bf7e fdf2 8f3f 5fe7 1ec6 5a06  .....~...?_...Z.
+00001270: e1c5 f7cf 5ffe fefc c50f dffc f5cb 338b  ...._.........3.
+00001280: f76e 86c6 3a7c 4412 cc9d dbf8 dcb9 c712  .n..:|D.........
+00001290: 189a 853f 1e67 6f67 318a 1131 2c50 0cbe  ...?.gog1..1,P..
+000012a0: 2dae 0710 381d 787b 85a8 0dd7 c366 081f  -...8.x{.....f..
+000012b0: 64a0 2f36 e0c1 f291 c1f5 24ce 9682 587a  d./6......$...Xz
+000012c0: be15 2706 f098 31da 6399 3500 b764 5f5a  ..'...1.c.5..d_Z
+000012d0: 8447 cb74 6eef 3c5b eab8 7b08 9dd9 fa8e  .G.tn.<[..{.....
+000012e0: 506a 2478 b05c 80b0 129b cb28 c606 cdbb  Pj$x.\.....(....
+000012f0: 14a5 02cd 718a 8523 9fb1 538c 2da3 7b48  ....q..#..S.-.{H
+00001300: 8811 d763 32c9 1867 33e1 3c24 4e0f 116b  ...c2..g3.<$N..k
+00001310: 4846 646c 1452 6974 4812 c8cb ca46 1052  HFdl.RitH....F.R
+00001320: 6dc4 e6f8 81d3 63d4 36ea 3e3e 3391 f05a  m.....c.6.>>3..Z
+00001330: 206a 213f c2d4 08e3 015a 0a94 d85c 8e50   j!?.....Z...\.P
+00001340: 42f5 801f 2111 db48 9eac b289 8e1b 7001  B...!..H......p.
+00001350: 999e 63ca 9cc1 1473 6eb3 b993 c178 b5a4  ..c....sn....x..
+00001360: df02 6db1 a7fd 98ae 1213 9909 726a f379  ..m.........rj.y
+00001370: 8418 d391 7d76 1ac5 2859 5839 9334 d6b1  ....}v..(YX9.4..
+00001380: 5ff0 5328 51e4 dc65 c206 3f66 e61b 22ef  _.S(Q..e..?f..".
+00001390: 210f 28dd 99ee 0704 1be9 be5c 08ee 83ac  !.(........\....
+000013a0: ea94 ca02 914f 9699 2597 0798 99ef e38a  .....O..%.......
+000013b0: ce10 562a 03aa 6f88 7942 d24b 95fd 82a6  ..V*..o.yB.K....
+000013c0: 071f 5ad3 edea 7c05 6a6e 77fc 3e3a decd  ..Z...|.jnw.>:..
+000013d0: 88f5 6d3a bca0 debb 70ff 41cd eea3 657a  ..m:....p.A...ez
+000013e0: 17c3 6bb2 3d67 7d92 ec4f 92ed feef 257b  ..k.=g}..O....%{
+000013f0: d7bb 7cf5 425d 6a33 c876 b93e 57ab f564  ..|.B]j3.v.>W..d
+00001400: e762 7d46 283d 112b 8a8f b85a af73 9891  .b}F(=.+...Z.s..
+00001410: a643 6854 1b09 b59b dc6c de16 315c 165b  .ChT.....l..1\.[
+00001420: 0303 37cf 90b2 7132 26be 2422 3e89 d102  ..7...q2&.$">...
+00001430: 16f5 35b5 f59c f3c2 f59c 3b0b c661 adaf  ..5.......;..a..
+00001440: 9ad5 2618 5ff0 ad76 0ccb e498 4df3 3d6a  ..&._..v....M.=j
+00001450: ad26 f7a3 b978 7024 ca76 2fd8 b4c3 fe42  .&...xp$.v/....B
+00001460: e4e8 b059 eebb 36ee d54e 76ae f6c7 6b02  ...Y..6..Nv...k.
+00001470: d2f6 6d48 689d 9924 1a16 12cd 7523 64e1  ..mHh..$....u#d.
+00001480: 7524 d4c8 ae84 45db c2a2 25dd af53 b5ce  u$....E...%..S..
+00001490: e226 1440 6d93 1558 3239 b0d0 eab8 819f  .&.@m..X29......
+000014a0: effd 611b 8528 9eca 3ce5 c700 ebec cae4  ..a..(..<.......
+000014b0: 5c69 a677 0593 ea15 00eb 8775 0594 996e  \i.w.......u...n
+000014c0: 4bae 3b87 2747 9797 da1b 64da 20a1 959b  K.;.'G....d. ...
+000014d0: 4942 2bc3 184d 7151 9dfa 61c9 55e6 ba5d  IB+..MqQ..a.U..]
+000014e0: a6d4 a027 43b1 7e1b 4a1a cdd6 87c8 b514  ...'C.~.J.......
+000014f0: 910b da40 535d 2968 ea9c 77dc b011 c079  ...@S])h..w....y
+00001500: d804 2d3a ee0c f6fa 7099 2ca0 76b8 5cea  ..-:....p.,.v.\.
+00001510: 223a 8703 b389 c8f2 17fe 5d94 6591 71d1  ":........].e.q.
+00001520: 473c ce03 ae44 2757 8384 089c 3994 241d  G<...D'W....9.$.
+00001530: 570e 7f53 0d34 551a a2b8 d5ea 2008 1f2d  W..S.4U..... ..-
+00001540: b936 c8ca c746 0e92 6e26 19cf 6678 22f4  .6...F..n&..fx".
+00001550: b46b 2d32 d2f9 2d28 7cae 15d6 a7ca fcdd  .k-2..-(|.......
+00001560: c1d2 922d 21dd 27f1 f4dc 19d3 6576 0f41  ...-!.'.....ev.A
+00001570: 8905 cd9a 0ce0 9470 38f2 a9e5 d19c 1238  .......p8......8
+00001580: c3dc 0859 597f 1726 a642 76f5 4344 5543  ...YY..&.Bv.CDUC
+00001590: 793b a28b 1815 338a 2ee6 395c 89e8 868e  y;....3...9\....
+000015a0: badb c440 bb2b c60c 01dd 0ee1 782e 27d8  ...@.+......x.'.
+000015b0: f79e 752f 9faa 65e4 34d1 2ce7 4c43 55e4  ..u/..e.4.,.LCU.
+000015c0: ac69 17d3 0f37 c96b acca 49d4 6095 4bb7  .i...7.k..I.`.K.
+000015d0: da36 f052 ebda 6bad 8342 b5ce 1297 ccba  .6.R..k..B......
+000015e0: 6f30 2168 d4ca ce0c 6a92 f1b6 0c4b cd2e  o0!h....j....K..
+000015f0: 5a4d 6a57 b820 d022 11ee 88db 668e b046  ZMjW. ."....f..F
+00001600: e25d 677e b0bb 58b5 7282 58af 2b55 e1ab  .]g~..X.r.X.+U..
+00001610: 8f1d faf7 0836 7e04 e2d1 8793 df25 155c  .....6~......%.\
+00001620: a512 be36 6408 167d f9d9 712e 1bf0 8a3c  ...6d..}..q....<
+00001630: 16c5 1a11 ae9c 6546 3aee 132f e8fa 513d  ......eF:../..Q=
+00001640: 882a 5e2b 1854 fc86 ef55 5a41 b751 e906  .*^+.T...UZA.Q..
+00001650: 41a3 3608 6a5e bf57 7f0a 138b 8893 5a90  A.6.j^.W......Z.
+00001660: 7f68 19c2 1114 5d15 9f5b 54fb d627 9764  .h....]..[T..'.d
+00001670: 7dca 766d c292 2a53 9f54 aa8a b8fa e452  }.vm..*S.T.....R
+00001680: abef fee4 e210 109d 2761 7dd8 6eb4 7b61  ........'a}.n.{a
+00001690: a5dd e80e 2b7e bfd7 aab4 a3b0 57e9 8751  ....+~......W..Q
+000016a0: b33f ec47 41ab 3d7c ea3a 670a ec77 1b91  .?.GA.=|.:g..w..
+000016b0: 1f0e 5a95 b016 4515 3ff4 24fd 56bb d2f4  ..Z...E.?.$.V...
+000016c0: ebf5 aedf ecb6 067e f769 b18c 8191 e7f2  .......~.i......
+000016d0: 51c4 02c2 ab78 edff 0b00 00ff ff03 0050  Q....x.........P
+000016e0: 4b03 0414 0006 0008 0000 0021 0045 9ea9  K..........!.E..
+000016f0: ab6d 0300 0095 0900 000d 0000 0078 6c2f  .m...........xl/
+00001700: 7374 796c 6573 2e78 6d6c ac56 db8e db36  styles.xml.V...6
+00001710: 107d 2f90 7f20 f8ae d5c5 966b 1b92 82f5  .}/.. .....k....
+00001720: 7a05 0448 8302 bb05 fa4a 4b94 4c84 1781  z..H.....JK.L...
+00001730: a237 7282 fe7b 8694 6469 9b4d 6bb8 f58b  .7r..{..di.Mk...
+00001740: c8e1 cce1 990b 679c bcef 0447 2f54 b74c  ......g....G/T.L
+00001750: c914 8777 0146 5416 aa64 b24e f11f cfb9  ...w.FT..d.N....
+00001760: b7c6 a835 4496 842b 4953 7ca6 2d7e 9fbd  ...5D..+IS|.-~..
+00001770: fb25 69cd 99d3 a723 a506 0184 6c53 7c34  .%i....#....lS|4
+00001780: a6d9 fa7e 5b1c a920 ed9d 6aa8 8493 4a69  ...~[.. ..j...Ji
+00001790: 410c 6c75 edb7 8da6 a46c ad91 e07e 1404  A.lu.....l...~..
+000017a0: 2b5f 1026 718f b015 c535 2082 e8cf a7c6  +_.&q....5 .....
+000017b0: 2b94 6888 6107 c699 393b 2c8c 44b1 fd50  +.h.a...9;,.D..P
+000017c0: 4ba5 c981 03d5 2e5c 9202 75e1 4a47 a8d3  K......\..u.JG..
+000017d0: e325 4efa c33d 8215 5ab5 aa32 7780 ebab  .%N..=..Z..2w...
+000017e0: aa62 05fd 91ee c6df f8a4 9890 00f9 36a4  .b............6.
+000017f0: 30f6 83e8 95ef 9dbe 1169 e96b fac2 6cfa  0........i.k..l.
+00001800: 7096 544a 9a16 15ea 244d 8a17 40d4 8660  p.TJ....$M..@..`
+00001810: fb59 aa2f 32b7 4790 e141 2b4b daaf e885  .Y./2.G..A+K....
+00001820: 7090 84d8 cf92 4271 a591 81d4 41e4 9c44  p.....Bq....A..D
+00001830: 1241 7b8d 07c2 d941 33ab 5611 c1f8 b917  .A{....A3.V.....
+00001840: 4756 e0b2 3de8 0906 b1b7 42df f2e8 d9cc  GV..=.....B.....
+00001850: ee09 ecd1 847a af19 e16f 62be 69be 7e6d  .....z...ob.i.~m
+00001860: 7d2b 2787 dd02 37c6 f92c 52bd 204b a0a4  }+'...7..,R. K..
+00001870: 0cd5 3287 5334 ac9f cf0d 8444 42f5 f7ae  ..2.S4.....DB...
+00001880: c1d1 bf6a d79a 9cc3 28be dea0 559c 9536  ...j....(...U..6
+00001890: 35f5 834b 84ae 0f29 ce87 9f85 390c 074c  5..K...)....9..L
+000018a0: 96b4 a365 8a57 4b87 3e23 6ce3 eec8 b90f  ...e.WK.>#l.....
+000018b0: f878 50ba 8497 3dd6 4304 f8bd 284b 38ad  .xP...=.C...(K8.
+000018c0: 0ca0 6a56 1fed d7a8 c6de a18c 81ea cf92  ..jV............
+000018d0: 9291 5a49 c26d 2a47 8bb9 2574 0478 fc29  ..ZI.m*G..%t.x.)
+000018e0: 3647 78bc 63ed fc9d 99bd 62b8 e12a 7dc7  6Gx.c.....b..*}.
+000018f0: c551 b94a 1d28 8f8c afd2 ef9d 7bdb b7c1  .Q.J.(......{...
+00001900: 4908 5941 397f b2ce fd59 5de2 669f 4c57  I.YA9....Y].f.LW
+00001910: 2179 12b9 301f 20f4 d023 6d81 8f4b 88f9  !y..0. ..#m..K..
+00001920: b0ec 63d4 6f6c ece6 683d f60c 7671 132c  ..c.ol..h=..vq.,
+00001930: eaaa 0bfe cf48 85c0 6f20 1561 3491 02f9  .....H..o .a4...
+00001940: 688d 48d3 f0b3 ed09 f6b5 0f3b b099 763b  h.H........;..v;
+00001950: 573c d3fe 9eb3 5a0a da1b 6409 b484 7e8b  W<....Z...d...~.
+00001960: 8e4a b3af 0064 7b49 01e7 145a 2d0c 14c3  .J...d{I...Z-...
+00001970: 8ab9 e48b 26cd 33ed dc75 3634 5df5 f3a0  ....&.3..u64]...
+00001980: cef8 43a8 afe6 ffff 321e 49ba 2442 da66  ..C.....2.I.$B.f
+00001990: b5f1 aa32 2e39 46b6 b5a5 f893 9d77 5c9e  ...2.9F......w\.
+000019a0: 67b1 3e9c 1837 4cbe 5117 805a 7653 a5b9  g.>..7L.Q..ZvS..
+000019b0: 0e69 ecf4 7235 78b9 07a2 50d2 8a9c b879  .i..r5x...P....y
+000019c0: be1c a678 5aff 464b 7612 90eb 41eb 77f6  ...xZ.FKv...A.w.
+000019d0: a28c 8348 f1b4 fe68 1f7b b8b2 6d03 12f1  ...H...h.{..m...
+000019e0: b185 d709 5f74 d22c c5df 1e77 bf6e f68f  ...._t.,...w.n..
+000019f0: 79e4 ad83 ddda 5b2e 68ec 6de2 ddde 8b97  y.....[.h.m.....
+00001a00: 0fbb fd3e df04 51f0 f0d7 6c86 fe87 09ea  ...>..Q...l.....
+00001a10: 463e 643f 5c6e 5b0e 7356 0fce 0ee4 9f26  F>d?\n[.sV.....&
+00001a20: 598a 679b 9ebe 6b7a 407b ce7d 13ad 82fb  Y.g...kz@{.}....
+00001a30: 380c bc7c 1184 de72 45d6 de7a b588 bd3c  8..|...rE..z...<
+00001a40: 0ea3 fd6a b97b 8cf3 78c6 3dbe 71d2 067e  ...j.{..x.=.q..~
+00001a50: 18f6 33db 928f b786 09ca 991c 7335 6668  ..3.........s5fh
+00001a60: 2e85 24c1 f61f 9cf0 c74c f8d3 ffa9 ec3b  ..$......L.....;
+00001a70: 0000 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
+00001a80: 0000 0021 00fb 9141 a072 0100 006d 0300  ...!...A.r...m..
+00001a90: 0014 0000 0078 6c2f 7368 6172 6564 5374  .....xl/sharedSt
+00001aa0: 7269 6e67 732e 786d 6c8c 534d 6b1b 3110  rings.xml.SMk.1.
+00001ab0: bd07 fa1f 840e 3d04 ec5d 3b21 9876 774d  ......=..];!.vwM
+00001ac0: 6908 0d24 39b8 6e20 9462 a6ab e95a 208d  i..$9.n .b...Z .
+00001ad0: b69a 5927 eeaf 8f8c 0f05 ad09 39ee fbd8  ..Y'........9...
+00001ae0: 379a 2755 cb17 efd4 0e23 db40 b59e 4d4b  7.'U.....#.@..MK
+00001af0: ad90 da60 2c75 b5fe b1be 992c b462 0132  ...`,u.....,.b.2
+00001b00: e002 61ad f7c8 7ad9 7c38 ab98 4525 2f71  ..a...z.|8..E%/q
+00001b10: adb7 22fd a7a2 e076 8b1e 781a 7aa4 c4fc  .."....v..x.z...
+00001b20: 09d1 83a4 cfd8 15dc 4704 c35b 44f1 ae98  ........G..[D...
+00001b30: 97e5 55e1 c192 566d 1848 6a7d 39d7 6a20  ..U...Vm.Hj}9.j 
+00001b40: fb77 c0af 4760 bed0 4dc5 b6a9 a4b9 f57e  .w..G`..M......~
+00001b50: 2054 2be4 3e10 6355 4853 1507 ea48 7f17   T+.>.cUHS...H..
+00001b60: f8ed 46e8 eae1 4b2e 5c94 93d9 4599 a34f  ..F...K.\...E..O
+00001b70: c839 7417 9e73 681d 81d8 2289 0a51 1d13  .9t..sh..."..Q..
+00001b80: cf73 0da7 9539 4ccb 4a5a 8346 394b 0851  .s...9L.JZ.F9K.Q
+00001b90: 5d8f 2799 2d26 f3ab dcfe 8871 afde 8ace  ].'.-&.....q....
+00001ba0: 0d26 0ce9 e0ef c97b 08b9 f79b edb6 3976  .&.....{......9v
+00001bb0: 1f0c 4690 d12a 5be8 a1b5 b2cf f51d 52f0  ..F..*[.......R.
+00001bc0: 2335 bea4 aaf9 709b 72fd 0e5b 0971 23fb  #5....p.r..[.q#.
+00001bd0: 7e64 62fb 0f7f 92ff 955b 3e3a f9ac 66a3  ~db......[>:..f.
+00001be0: ce8e c91b 4b82 5d9a f844 56c4 14b5 b311  ....K.]..DV.....
+00001bf0: 5cfe 4b30 69ec 938c 4bf5 da93 0c33 c06e  \.K0i...K....3.n
+00001c00: 5477 7b02 8cd8 0d2e 95de 3b60 6fcd 7f4f  Tw{.......;`o..O
+00001c10: 919e 4bf3 0a00 00ff ff03 0050 4b03 0414  ..K........PK...
+00001c20: 0006 0008 0000 0021 003b 6d32 4bc1 0000  .......!.;m2K...
+00001c30: 0042 0100 0023 0000 0078 6c2f 776f 726b  .B...#...xl/work
+00001c40: 7368 6565 7473 2f5f 7265 6c73 2f73 6865  sheets/_rels/she
+00001c50: 6574 312e 786d 6c2e 7265 6c73 848f c18a  et1.xml.rels....
+00001c60: c230 1445 f703 fe43 787b 93d6 850c 4353  .0.E...Cx{....CS
+00001c70: 3722 b855 e703 62fa da06 db97 90f7 14fd  7".U..b.........
+00001c80: 7bb3 1c65 c0e5 e570 cfe5 369b fb3c a91b  {..e...p..6..<..
+00001c90: 660e 912c d4ba 0285 e463 1768 b0f0 7bda  f..,.....c.h..{.
+00001ca0: 2dbf 41b1 38ea dc14 092d 3c90 61d3 2ebe  -.A.8....-<.a...
+00001cb0: 9a03 4e4e 4a89 c790 5815 0bb1 8551 24fd  ..NNJ...X....Q$.
+00001cc0: 18c3 7ec4 d9b1 8e09 a990 3ee6 d949 8979  ..~.......>..I.y
+00001cd0: 30c9 f98b 1bd0 acaa 6a6d f25f 07b4 2f4e  0.......jm._../N
+00001ce0: b5ef 2ce4 7d57 833a 3d52 59fe ec8e 7d1f  ..,.}W.:=RY...}.
+00001cf0: 3c6e a3bf ce48 f2cf 8449 3990 603e a248  <n...H...I9.`>.H
+00001d00: 39c8 45ed f280 6241 eb77 f69e 6b7d 0e04  9.E...bA.w..k}..
+00001d10: a66d cccb f3f6 0900 00ff ff03 0050 4b03  .m...........PK.
+00001d20: 0414 0006 0008 0000 0021 0094 258c 3ea4  .........!..%.>.
+00001d30: 0100 00b0 0f00 0027 0000 0078 6c2f 7072  .......'...xl/pr
+00001d40: 696e 7465 7253 6574 7469 6e67 732f 7072  interSettings/pr
+00001d50: 696e 7465 7253 6574 7469 6e67 7331 2e62  interSettings1.b
+00001d60: 696e ec57 cf4b 4241 10fe de53 414d a463  in.W.KBA...SAM.c
+00001d70: 27f1 5681 8702 838e 99d2 2188 c03c 782c  '.V.......!..<x,
+00001d80: b043 d00f c92e 9da2 ff20 e8d6 b953 7f8f  .C....... ...S..
+00001d90: 9720 e822 d41f d035 ec1b 7572 5bf7 3d2f  . ."...5..ur[.=/
+00001da0: 81f0 d891 793b bb33 3b3b f3cd 1cc6 3a4e  ....y;.3;;....:N
+00001db0: 7089 2b72 192d 3451 c516 36f8 2ba3 8753  p.+r.-4Q..6.+..S
+00001dc0: 5ce3 8cdf 1e77 6ba8 d3aa 8b5b ca9b 5887  \....wk....[..X.
+00001dd0: 5290 ce17 ded0 2fa6 deef 5301 7278 5aaa  R...../...S.rxZ.
+00001de0: 663b 0850 0abe 8721 5790 03d4 e8f7 ff49  f;.P...!W......I
+00001df0: bc87 a317 e495 59ea 1781 ddfd c641 be30  ......Y......A.0
+00001e00: d63d e481 578a c2bf f153 c836 81f4 0d50  .=..W....S.6...P
+00001e10: a193 16f9 f810 1874 67f7 b69d d87e 39ec  .......tg....~9.
+00001e20: f55c fdd9 76ed b01d aea0 41b4 6bd8 23ea  .\..v.....A.k.#.
+00001e30: 8ba4 23d6 ff82 753d 679d a5b2 49a0 e5d5  ..#...u=g...I...
+00001e40: 44a4 e193 f008 7804 3c02 1e81 0521 20b3  D.....x.<....! .
+00001e50: 456a c212 c278 9e71 0513 8eec 7ca1 3c02  Ej...x.q....|.<.
+00001e60: 5304 729c 86a7 fd23 bd64 539a 0732 b74a  S.r....#.dS..2.J
+00001e70: 8f95 28c8 2ae4 9a65 e55c f43a efda 761d  ..(.*..e.\.:..v.
+00001e80: 1ec8 7b3a a38a dede 6b0c e3a9 3cfa 9d49  ..{:....k...<..I
+00001e90: 1878 5481 eb0e 6767 bd57 31ce 4d51 f4c3  .xT...gg.W1.MQ..
+00001ea0: e15f 25af cd90 2bbf a89c cd3c 6ddf 36a6  ._%...+....<m.6.
+00001eb0: ea23 ca97 898d d8dc 596c be25 f207 01b7  .#......Yl.%....
+00001ec0: d271 661e 177b 0454 b198 b830 9358 e651  .qf..{.T...0.X.Q
+00001ed0: c630 506c cc7e b1ef 7f4e 7cba 708b c256  .0Pl.~...N|.p..V
+00001ee0: 7a56 49fb 212e aeb8 5e73 e126 fea5 97e7  zVI.!...^s.&....
+00001ef0: f914 bd19 8bda d713 fc7f 36b3 fdfc f203  ..........6.....
+00001f00: 0000 ffff 0300 504b 0304 1400 0600 0800  ......PK........
+00001f10: 0000 2100 0e2b 64fe 5401 0000 6902 0000  ..!..+d.T...i...
+00001f20: 1100 0801 646f 6350 726f 7073 2f63 6f72  ....docProps/cor
+00001f30: 652e 786d 6c20 a204 0128 a000 0100 0000  e.xml ...(......
+00001f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002000: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002010: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002020: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002030: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002040: 0000 0000 0000 007c 92d1 4e83 3018 85ef  .......|..N.0...
-00002050: 4d7c 07d2 7b28 856d 990d b044 cd2e d425  M|..{(.m...D...%
-00002060: 2662 34de 75ed bf8d 0c0a 693b d99e c5e7  &b4.u.....i;....
-00002070: f1bd 2cb0 213a e365 7bce fff5 9c3f 8d66  ..,.!:.e{....?.f
-00002080: fb22 77de 41e9 ac94 3122 9e8f 1c90 bc14  ."w.A...1"......
-00002090: 995c c7e8 399d bb53 e468 c3a4 6079 2921  .\..9..S.h..`y)!
-000020a0: 4607 d068 965c 5e44 bca2 bc54 f0a8 ca0a  F..h.\^D...T....
-000020b0: 94c9 403b 9624 35e5 558c 36c6 5414 63cd  ..@;.$5.U.6.T.c.
-000020c0: 3750 30ed 5987 b4e2 aa54 0533 f6a8 d6b8  7P0.Y....T.3....
-000020d0: 627c cbd6 8003 df9f e002 0c13 cc30 dc00  b|...........0..
-000020e0: ddaa 27a2 2352 f01e 59ed 54de 0204 c790  ..'.#R..Y.T.....
-000020f0: 4301 d268 4c3c 82bf bd06 54a1 ff1c 6895  C..hL<....T...h.
-00002100: 81b3 c8cc a1b2 9d8e 7187 6cc1 3bb1 77ef  ........q.l.;.w.
-00002110: 75d6 1beb baf6 eab0 8d61 f313 fcba 7878  u........a....xx
-00002120: 6aab ba99 6c76 c501 2591 e094 2b60 a654  j...lv..%...+`.T
-00002130: c91d dbee 96ce fd6e 997d 7e44 7820 344b  .......n.}~Dx 4K
-00002140: cc99 360b bbef 5506 e2fa f0cb 7bae 5b6e  ..6...U.....{.[n
-00002150: 5ba3 8383 706c 30da d538 292f e1cd 6d3a  [...pl0..8)/..m:
-00002160: 4749 e093 b1eb 4f5c 7f9c 9229 2557 341c  GI....O\...)%W4.
-00002170: bd35 cfff 986f 8276 17c5 31c4 bfc4 2074  .5...o.v..1... t
-00002180: 0971 4998 9231 1d8d 2809 06c4 1320 89f0  .qI..1..(.... ..
-00002190: d9e7 48be 0000 00ff ff03 0050 4b03 0414  ..H........PK...
-000021a0: 0006 0008 0000 0021 00a0 0798 4084 0100  .......!....@...
-000021b0: 000f 0300 0010 0008 0164 6f63 5072 6f70  .........docProp
-000021c0: 732f 6170 702e 786d 6c20 a204 0128 a000  s/app.xml ...(..
-000021d0: 0100 0000 0000 0000 0000 0000 0000 0000  ................
+00002030: 0000 0000 0000 0000 0000 0000 007c 924d  .............|.M
+00002040: 4ec3 3014 84f7 48dc 21f2 3e71 9cfe 885a  N.0...H.!.>q...Z
+00002050: 492a 01ea 02a8 8444 1088 9d6b bfb6 5113  I*.....D...k..Q.
+00002060: c7b2 5dda 9e85 f370 2f9c a40d 8122 96f6  ..]....p/...."..
+00002070: ccfb 3cf3 e478 ba2f 0bef 1db4 c92b 9920  ..<..x./.....+. 
+00002080: 1284 c803 c92b 91cb 5582 9eb3 997f 853c  .....+..U......<
+00002090: 6399 14ac a824 24e8 0006 4dd3 cb8b 982b  c....$$...M....+
+000020a0: ca2b 0d8f ba52 a06d 0ec6 7324 6928 5709  .+...R.m..s$i(W.
+000020b0: 5a5b ab28 c686 afa1 6426 700e e9c4 65a5  Z[.(....d&p...e.
+000020c0: 4b66 dd51 afb0 627c c356 80a3 301c e312  Kf.Q..b|.V..0...
+000020d0: 2c13 cc32 5c03 7dd5 11d1 1129 7887 545b  ,..2\.}....)x.T[
+000020e0: 5d34 00c1 3114 5082 b406 9380 e06f af05  ]4..1.P......o..
+000020f0: 5d9a 3f07 1aa5 e72c 737b 50ae d331 6e9f  ].?....,s{P..1n.
+00002100: 2d78 2b76 eebd c93b e36e b70b 7683 2686  -x+v...;.n..v.&.
+00002110: cb4f f0eb fce1 a9a9 eae7 b2de 1507 94c6  .O..............
+00002120: 8253 ae81 d94a a777 6cb3 5d78 f7db 45fe  .S...J.wl.]x..E.
+00002130: f911 e39e 502f b160 c6ce ddbe 9739 88eb  ....P/.`.....9..
+00002140: c32f efb9 eeb8 4d8d 160e c273 c168 5be3  ./....M....s.h[.
+00002150: a4bc 0c6e 6eb3 194a a390 8cfc 70ec 87a3  ...nn..J....p...
+00002160: 8c5c 5132 a183 e15b fdfc 8ff9 3a68 7b51  .\Q2...[....:h{Q
+00002170: 1e43 fc4b 8c86 0ee7 4751 4622 4a86 349a  .C.K....GQF"J.4.
+00002180: f488 2740 1ae3 b3cf 917e 0100 00ff ff03  ..'@.....~......
+00002190: 0050 4b03 0414 0006 0008 0000 0021 00a0  .PK..........!..
+000021a0: 0798 4084 0100 000f 0300 0010 0008 0164  ..@............d
+000021b0: 6f63 5072 6f70 732f 6170 702e 786d 6c20  ocProps/app.xml 
+000021c0: a204 0128 a000 0100 0000 0000 0000 0000  ...(............
+000021d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000021e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000021f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002200: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002210: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002220: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002230: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002240: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002250: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002260: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002270: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002280: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002290: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000022a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000022b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-000022d0: 009c 9241 4fe3 3010 85ef 2bed 7f88 7ca7  ...AO.0...+...|.
-000022e0: 4e59 8456 9563 840a 88c3 aea8 d4c2 7d70  NY.V.c........}p
-000022f0: 26ad 8563 5bf6 346a f9f5 4c12 51d2 dd3d  &..c[.4j..L.Q..=
-00002300: ed6d 66de e8f9 f3b3 d5cd a175 4587 29db  .mf........uE.).
-00002310: e02b 319f 95a2 406f 426d fdb6 12cf 9b87  .+1...@oBm......
-00002320: 8b9f a2c8 04be 0617 3c56 e288 59dc e8ef  ........<V..Y...
-00002330: dfd4 2a85 8889 2ce6 822d 7cae c48e 282e  ..*...,..-|...(.
-00002340: a4cc 6687 2de4 19cb 9e95 26a4 1688 dbb4  ..f.-.....&.....
-00002350: 95a1 69ac c1bb 60f6 2d7a 9297 6579 2df1  ..i...`.-z..ey-.
-00002360: 40e8 6bac 2fe2 c950 8c8e 8b8e fed7 b40e  @.k./..P........
-00002370: a6e7 cb2f 9b63 6460 ad6e 6374 d600 f12d  .../.cd`.nct...-
-00002380: f56f 6b52 c8a1 a1e2 fe60 d029 3915 15d3  .okR.....`.)9...
-00002390: add1 ec93 a5a3 2e95 9cb6 6a6d c0e1 928d  ..........jm....
-000023a0: 7503 2ea3 925f 03f5 88d0 87b6 029b b256  u...._.........V
-000023b0: 1d2d 3a34 1452 91ed 3bc7 7629 8a57 c8d8  .-:4.R..;.v).W..
-000023c0: e354 a283 64c1 1363 f56b 6333 d42e 664a  .T..d..c.kc3..fJ
-000023d0: fa36 bded f33b bbb3 3a4e 8672 ba38 aded  .6...;..:N.r.8..
-000023e0: 959e 0f0b 5c9c 2ff6 0623 050b e77c 1b4b  ....\./..#...|.K
-000023f0: 0ef3 53b3 8244 ffc0 9d4f 7107 8611 760a  ..S..D...Oq...v.
-00002400: 381e 3a05 1c2e cc47 fd61 be0c 6d04 7f64  8.:....G.a..m..d
-00002410: e154 fdb2 fe2d 3fc7 4db8 03c2 cf30 cf87  .T...-?.M....0..
-00002420: 6abd 8384 35e7 7f0a fb34 508f 9c63 72bd  j...5....4P..cr.
-00002430: c972 077e 8bf5 e7ce df42 fff4 2fe3 ffd6  .r.~.....B../...
-00002440: f3eb 59f9 a3e4 579d cc94 fcfa c9fa 0300  ..Y...W.........
-00002450: 00ff ff03 0050 4b01 022d 0014 0006 0008  .....PK..-......
-00002460: 0000 0021 0041 3782 cf6e 0100 0004 0500  ...!.A7..n......
-00002470: 0013 0000 0000 0000 0000 0000 0000 0000  ................
-00002480: 0000 005b 436f 6e74 656e 745f 5479 7065  ...[Content_Type
-00002490: 735d 2e78 6d6c 504b 0102 2d00 1400 0600  s].xmlPK..-.....
-000024a0: 0800 0000 2100 b555 3023 f400 0000 4c02  ....!..U0#....L.
-000024b0: 0000 0b00 0000 0000 0000 0000 0000 0000  ................
-000024c0: a703 0000 5f72 656c 732f 2e72 656c 7350  ...._rels/.relsP
-000024d0: 4b01 022d 0014 0006 0008 0000 0021 00e5  K..-.........!..
-000024e0: 53dd 52f0 0200 00ce 0600 000f 0000 0000  S.R.............
-000024f0: 0000 0000 0000 0000 00cc 0600 0078 6c2f  .............xl/
-00002500: 776f 726b 626f 6f6b 2e78 6d6c 504b 0102  workbook.xmlPK..
-00002510: 2d00 1400 0600 0800 0000 2100 813e 9497  -.........!..>..
-00002520: f300 0000 ba02 0000 1a00 0000 0000 0000  ................
-00002530: 0000 0000 0000 e909 0000 786c 2f5f 7265  ..........xl/_re
-00002540: 6c73 2f77 6f72 6b62 6f6f 6b2e 786d 6c2e  ls/workbook.xml.
-00002550: 7265 6c73 504b 0102 2d00 1400 0600 0800  relsPK..-.......
-00002560: 0000 2100 7d60 1dbf e203 0000 940c 0000  ..!.}`..........
-00002570: 1800 0000 0000 0000 0000 0000 0000 1c0c  ................
-00002580: 0000 786c 2f77 6f72 6b73 6865 6574 732f  ..xl/worksheets/
-00002590: 7368 6565 7431 2e78 6d6c 504b 0102 2d00  sheet1.xmlPK..-.
-000025a0: 1400 0600 0800 0000 2100 4d3f 802c 8406  ........!.M?.,..
-000025b0: 0000 801a 0000 1300 0000 0000 0000 0000  ................
-000025c0: 0000 0000 3410 0000 786c 2f74 6865 6d65  ....4...xl/theme
-000025d0: 2f74 6865 6d65 312e 786d 6c50 4b01 022d  /theme1.xmlPK..-
-000025e0: 0014 0006 0008 0000 0021 0045 9ea9 ab6d  .........!.E...m
-000025f0: 0300 0095 0900 000d 0000 0000 0000 0000  ................
-00002600: 0000 0000 00e9 1600 0078 6c2f 7374 796c  .........xl/styl
-00002610: 6573 2e78 6d6c 504b 0102 2d00 1400 0600  es.xmlPK..-.....
-00002620: 0800 0000 2100 fb91 41a0 7201 0000 6d03  ....!...A.r...m.
-00002630: 0000 1400 0000 0000 0000 0000 0000 0000  ................
-00002640: 811a 0000 786c 2f73 6861 7265 6453 7472  ....xl/sharedStr
-00002650: 696e 6773 2e78 6d6c 504b 0102 2d00 1400  ings.xmlPK..-...
-00002660: 0600 0800 0000 2100 3b6d 324b c100 0000  ......!.;m2K....
-00002670: 4201 0000 2300 0000 0000 0000 0000 0000  B...#...........
-00002680: 0000 251c 0000 786c 2f77 6f72 6b73 6865  ..%...xl/workshe
-00002690: 6574 732f 5f72 656c 732f 7368 6565 7431  ets/_rels/sheet1
-000026a0: 2e78 6d6c 2e72 656c 7350 4b01 022d 0014  .xml.relsPK..-..
-000026b0: 0006 0008 0000 0021 0094 258c 3ea4 0100  .......!..%.>...
-000026c0: 00b0 0f00 0027 0000 0000 0000 0000 0000  .....'..........
-000026d0: 0000 0027 1d00 0078 6c2f 7072 696e 7465  ...'...xl/printe
-000026e0: 7253 6574 7469 6e67 732f 7072 696e 7465  rSettings/printe
-000026f0: 7253 6574 7469 6e67 7331 2e62 696e 504b  rSettings1.binPK
-00002700: 0102 2d00 1400 0600 0800 0000 2100 c520  ..-.........!.. 
-00002710: 73fd 5401 0000 6902 0000 1100 0000 0000  s.T...i.........
-00002720: 0000 0000 0000 0000 101f 0000 646f 6350  ............docP
-00002730: 726f 7073 2f63 6f72 652e 786d 6c50 4b01  rops/core.xmlPK.
-00002740: 022d 0014 0006 0008 0000 0021 00a0 0798  .-.........!....
-00002750: 4084 0100 000f 0300 0010 0000 0000 0000  @...............
-00002760: 0000 0000 0000 009b 2100 0064 6f63 5072  ........!..docPr
-00002770: 6f70 732f 6170 702e 786d 6c50 4b05 0600  ops/app.xmlPK...
-00002780: 0000 000c 000c 0026 0300 0055 2400 0000  .......&...U$...
-00002790: 00                                       .
+000022c0: 0000 0000 0000 009c 9241 4fe3 3010 85ef  .........AO.0...
+000022d0: 2bed 7f88 7ca7 4e59 8456 9563 840a 88c3  +...|.NY.V.c....
+000022e0: aea8 d4c2 7d70 26ad 8563 5bf6 346a f9f5  ....}p&..c[.4j..
+000022f0: 4c12 51d2 dd3d ed6d 66de e8f9 f3b3 d5cd  L.Q..=.mf.......
+00002300: a175 4587 29db e02b 319f 95a2 406f 426d  .uE.)..+1...@oBm
+00002310: fdb6 12cf 9b87 8b9f a2c8 04be 0617 3c56  ..............<V
+00002320: e288 59dc e8ef dfd4 2a85 8889 2ce6 822d  ..Y.....*...,..-
+00002330: 7cae c48e 282e a4cc 6687 2de4 19cb 9e95  |...(...f.-.....
+00002340: 26a4 1688 dbb4 95a1 69ac c1bb 60f6 2d7a  &.......i...`.-z
+00002350: 9297 6579 2df1 40e8 6bac 2fe2 c950 8c8e  ..ey-.@.k./..P..
+00002360: 8b8e fed7 b40e a6e7 cb2f 9b63 6460 ad6e  ........./.cd`.n
+00002370: 6374 d600 f12d f56f 6b52 c8a1 a1e2 fe60  ct...-.okR.....`
+00002380: d029 3915 15d3 add1 ec93 a5a3 2e95 9cb6  .)9.............
+00002390: 6a6d c0e1 928d 7503 2ea3 925f 03f5 88d0  jm....u...._....
+000023a0: 87b6 029b b256 1d2d 3a34 1452 91ed 3bc7  .....V.-:4.R..;.
+000023b0: 7629 8a57 c8d8 e354 a283 64c1 1363 f56b  v).W...T..d..c.k
+000023c0: 6333 d42e 664a fa36 bded f33b bbb3 3a4e  c3..fJ.6...;..:N
+000023d0: 8672 ba38 aded 959e 0f0b 5c9c 2ff6 0623  .r.8......\./..#
+000023e0: 050b e77c 1b4b 0ef3 53b3 8244 ffc0 9d4f  ...|.K..S..D...O
+000023f0: 7107 8611 760a 381e 3a05 1c2e cc47 fd61  q...v.8.:....G.a
+00002400: be0c 6d04 7f64 e154 fdb2 fe2d 3fc7 4db8  ..m..d.T...-?.M.
+00002410: 03c2 cf30 cf87 6abd 8384 35e7 7f0a fb34  ...0..j...5....4
+00002420: 508f 9c63 72bd c972 077e 8bf5 e7ce df42  P..cr..r.~.....B
+00002430: fff4 2fe3 ffd6 f3eb 59f9 a3e4 579d cc94  ../.....Y...W...
+00002440: fcfa c9fa 0300 00ff ff03 0050 4b01 022d  ...........PK..-
+00002450: 0014 0006 0008 0000 0021 0041 3782 cf6e  .........!.A7..n
+00002460: 0100 0004 0500 0013 0000 0000 0000 0000  ................
+00002470: 0000 0000 0000 0000 005b 436f 6e74 656e  .........[Conten
+00002480: 745f 5479 7065 735d 2e78 6d6c 504b 0102  t_Types].xmlPK..
+00002490: 2d00 1400 0600 0800 0000 2100 b555 3023  -.........!..U0#
+000024a0: f400 0000 4c02 0000 0b00 0000 0000 0000  ....L...........
+000024b0: 0000 0000 0000 a703 0000 5f72 656c 732f  .........._rels/
+000024c0: 2e72 656c 7350 4b01 022d 0014 0006 0008  .relsPK..-......
+000024d0: 0000 0021 0030 df72 78e8 0200 00c3 0600  ...!.0.rx.......
+000024e0: 000f 0000 0000 0000 0000 0000 0000 00cc  ................
+000024f0: 0600 0078 6c2f 776f 726b 626f 6f6b 2e78  ...xl/workbook.x
+00002500: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
+00002510: 2100 813e 9497 f300 0000 ba02 0000 1a00  !..>............
+00002520: 0000 0000 0000 0000 0000 0000 e109 0000  ................
+00002530: 786c 2f5f 7265 6c73 2f77 6f72 6b62 6f6f  xl/_rels/workboo
+00002540: 6b2e 786d 6c2e 7265 6c73 504b 0102 2d00  k.xml.relsPK..-.
+00002550: 1400 0600 0800 0000 2100 4bd1 61e8 e003  ........!.K.a...
+00002560: 0000 940c 0000 1800 0000 0000 0000 0000  ................
+00002570: 0000 0000 140c 0000 786c 2f77 6f72 6b73  ........xl/works
+00002580: 6865 6574 732f 7368 6565 7431 2e78 6d6c  heets/sheet1.xml
+00002590: 504b 0102 2d00 1400 0600 0800 0000 2100  PK..-.........!.
+000025a0: 4d3f 802c 8406 0000 801a 0000 1300 0000  M?.,............
+000025b0: 0000 0000 0000 0000 0000 2a10 0000 786c  ..........*...xl
+000025c0: 2f74 6865 6d65 2f74 6865 6d65 312e 786d  /theme/theme1.xm
+000025d0: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
+000025e0: 0045 9ea9 ab6d 0300 0095 0900 000d 0000  .E...m..........
+000025f0: 0000 0000 0000 0000 0000 00df 1600 0078  ...............x
+00002600: 6c2f 7374 796c 6573 2e78 6d6c 504b 0102  l/styles.xmlPK..
+00002610: 2d00 1400 0600 0800 0000 2100 fb91 41a0  -.........!...A.
+00002620: 7201 0000 6d03 0000 1400 0000 0000 0000  r...m...........
+00002630: 0000 0000 0000 771a 0000 786c 2f73 6861  ......w...xl/sha
+00002640: 7265 6453 7472 696e 6773 2e78 6d6c 504b  redStrings.xmlPK
+00002650: 0102 2d00 1400 0600 0800 0000 2100 3b6d  ..-.........!.;m
+00002660: 324b c100 0000 4201 0000 2300 0000 0000  2K....B...#.....
+00002670: 0000 0000 0000 0000 1b1c 0000 786c 2f77  ............xl/w
+00002680: 6f72 6b73 6865 6574 732f 5f72 656c 732f  orksheets/_rels/
+00002690: 7368 6565 7431 2e78 6d6c 2e72 656c 7350  sheet1.xml.relsP
+000026a0: 4b01 022d 0014 0006 0008 0000 0021 0094  K..-.........!..
+000026b0: 258c 3ea4 0100 00b0 0f00 0027 0000 0000  %.>........'....
+000026c0: 0000 0000 0000 0000 001d 1d00 0078 6c2f  .............xl/
+000026d0: 7072 696e 7465 7253 6574 7469 6e67 732f  printerSettings/
+000026e0: 7072 696e 7465 7253 6574 7469 6e67 7331  printerSettings1
+000026f0: 2e62 696e 504b 0102 2d00 1400 0600 0800  .binPK..-.......
+00002700: 0000 2100 0e2b 64fe 5401 0000 6902 0000  ..!..+d.T...i...
+00002710: 1100 0000 0000 0000 0000 0000 0000 061f  ................
+00002720: 0000 646f 6350 726f 7073 2f63 6f72 652e  ..docProps/core.
+00002730: 786d 6c50 4b01 022d 0014 0006 0008 0000  xmlPK..-........
+00002740: 0021 00a0 0798 4084 0100 000f 0300 0010  .!....@.........
+00002750: 0000 0000 0000 0000 0000 0000 0091 2100  ..............!.
+00002760: 0064 6f63 5072 6f70 732f 6170 702e 786d  .docProps/app.xm
+00002770: 6c50 4b05 0600 0000 000c 000c 0026 0300  lPK..........&..
+00002780: 004b 2400 0000 00                        .K$....
```

### Comparing `JBioSeqTools-2.0.3/jbst/data/vectors.xlsx` & `JBioSeqTools-2.0.4/jbst/data/vectors.xlsx`

 * *Files 16% similar despite different names*

```diff
@@ -103,67 +103,67 @@
 00000660: 86b0 b737 a0ea 93cf 9b7f d796 a6e9 0d3f  ...7...........?
 00000670: 8839 4cec d299 15c8 7362 67d9 ae7c c86c  .9L.....sbg..|.l
 00000680: 21f5 f91a 5553 6839 69b0 629e 723a 2279  !...USh9i.b.r:"y
 00000690: 5f64 6cc0 f344 9bbf 13fd 7c2d 4e9c c852  _dl..D....|-N..R
 000006a0: 2234 12f8 32cf 47c7 25a0 f57f 5ab4 34f1  "4..2.G.%...Z.4.
 000006b0: cb9d 79c4 3709 c3ab c8f0 c982 8b1f a8de  ..y.7...........
 000006c0: 0100 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-000006d0: 0000 0021 0063 a728 9adf 0200 0012 0700  ...!.c.(........
+000006d0: 0000 0021 006a 4a1c bfe1 0200 0012 0700  ...!.jJ.........
 000006e0: 000f 0000 0078 6c2f 776f 726b 626f 6f6b  .....xl/workbook
-000006f0: 2e78 6d6c a455 5b6f 9b30 147e 9fb4 ff60  .xml.U[o.0.~...`
-00000700: f99d 8209 9004 9554 4d13 b44a 6d55 ad59  .......TM..JmU.Y
-00000710: fb58 b960 12ab 8091 3109 59d5 ffbe 6308  .X.`....1.Y...c.
-00000720: a459 aa29 ea10 f872 cef1 e7ef 5c6c ce2f  .Y.)...r....\l./
-00000730: ea2c 456b 264b 2ef2 0093 330b 2396 4722  .,Ek&K....3.#.G"
-00000740: e6f9 32c0 bf16 a131 c2a8 5434 8f69 2a72  ..2....1..T4.i*r
-00000750: 16e0 2d2b f1c5 e4fb b7f3 8d90 af2f 42bc  ..-+........./B.
-00000760: 2200 c8cb 00af 942a 7cd3 2ca3 15cb 6879  "......*|.,...hy
-00000770: 260a 9683 2611 32a3 0aa6 7269 9685 6434  &...&.2...ri..d4
-00000780: 2e57 8ca9 2c35 6dcb f2cc 8cf2 1cb7 08be  .W..,5m.........
-00000790: 3c05 4324 098f d84c 4455 c672 d582 4896  <.C$...LDU.r..H.
-000007a0: 5205 f4cb 152f ca0e 2d8b 4e81 cba8 7cad  R..../..-.N...|.
-000007b0: 0a23 1259 0110 2f3c e56a db80 6294 45fe  .#.Y../<.j..b.E.
-000007c0: f532 1792 bea4 e076 4d5c 544b 783d f888  .2.....vM\TKx=..
-000007d0: 058d dded 04aa a3ad 321e 4951 8a44 9d01  ........2.IQ.D..
-000007e0: b4d9 923e f29f 5826 2107 21a8 8f63 701a  ...>..X&!.!..cp.
-000007f0: 9263 4ab6 e63a 873d 2be9 7d91 95d7 6379  .cJ..:.=+.}...cy
-00000800: 7b30 62fd 371a 81d2 6a6a c587 e07d 11cd  {0b.7...jj...}..
-00000810: edb9 d978 729e f094 3db6 a58b 6851 dcd1  ...xr...=...hQ..
-00000820: 4c67 2ac5 28a5 a59a c75c b138 c043 988a  Lg*.(....\.8.C..
-00000830: 0ddb 0b1c 8c64 554c 2b9e 82d6 f6c6 b683  .....dUL+.......
-00000840: cd49 5fce f712 01ac 62f2 5ef2 358d b670  .I_.....b.^.5..p
-00000850: 2630 8a59 42ab 542d a0b4 bb0d 416e 3bb6  &0.YB.T-....An;.
-00000860: ede9 b5b5 f4bb f0df 2b89 607c 3dbb 010a  ........+.`|=...
-00000870: 0f74 0d84 c0ed 7857 afd7 b023 193c e791  .t....xW...#.<..
-00000880: f4c9 f3db f4f2 6a3e 1e85 23c3 7107 96e1  ......j>..#.q...
-00000890: 0c89 658c 86b6 65b8 b633 75c9 90cc 1dc7  ..e...e..3u.....
-000008a0: 7e87 9849 cf8f 04ad d46a e7ab 860e b003  ~..I.....j......
-000008b0: 8e1d a96e 69dd 6988 e557 3cde d378 b376  ...ni.i..W<..x.v
-000008c0: 8fa1 fbbf 9a4e f7ae ddd1 a7fa 91b3 4db9  .....N........M.
-000008d0: 8f8a 9ea2 fa89 e7b1 d804 d820 16dc 0adb  ........... ....
-000008e0: c3e9 a651 3ef1 58ad 20ac 03db 85ea 6965  ...Q>.X. .....ie
-000008f0: 3f18 5fae 8031 044c 0b21 fb9a 5980 0f18  ?._..1.L.!..Y...
-00000900: cd5a 4621 3c86 6e0e 1899 1f28 35f7 0750  .ZF!<.n....(5..P
-00000910: 6b7a 9437 39bf 8453 5cfe 8644 35c2 26ca  kz.79..S\..D5.&.
-00000920: 9064 5f6f 22af 63a2 9d3a 3687 03dc 9bc3  .d_o".c..:6.....
-00000930: b837 b73f 371f 7c30 8771 6f3e d0e6 66c7  .7.?7.|0.qo>..f.
-00000940: 2aa2 6904 25a4 bb86 c698 58f6 585b b05a  *.i.%.....X.X[.Z
-00000950: dd94 aae9 5125 3978 3f75 4753 6b30 b60d  ....Q%9x?uGSk0..
-00000960: 2724 a1e1 90b1 654c a79e 63b8 b370 e00e  '$....eL..c..p..
-00000970: c9ec 6aee 863a fdfa 7af5 6b8d 987c f1d4  ..j..:..z.k..|..
-00000980: 8ccc 6635 a3aa 9270 7d43 c136 735f b7e1  ..f5...p}C.6s_..
-00000990: 4eda 0b93 56b0 8bec c1f5 e3ff 9c35 e5de  N...V........5..
-000009a0: aefe 97e1 03fc 3e52 76a2 71f8 78a2 e1d5  ......>Rv.q.x...
-000009b0: dded e2f6 44db 9bf9 e2f9 296c 72f3 a9b7  ....D.....)lr...
-000009c0: 2624 04f2 d6a5 c5ec 7e67 933f 0000 00ff  &$......~g.?....
-000009d0: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-000009e0: 00de 09fd 2802 0100 00d4 0300 001a 0008  ....(...........
-000009f0: 0178 6c2f 5f72 656c 732f 776f 726b 626f  .xl/_rels/workbo
-00000a00: 6f6b 2e78 6d6c 2e72 656c 7320 a204 0128  ok.xml.rels ...(
-00000a10: a000 0100 0000 0000 0000 0000 0000 0000  ................
+000006f0: 2e78 6d6c a455 5b6f 9b30 147e 9fb4 ff80  .xml.U[o.0.~....
+00000700: fc4e c1dc 92a0 2655 1841 abd4 56d5 9ab5  .N....&U.A..V...
+00000710: 8f95 0b26 b10a 1819 9390 55fd ef3b 8640  ...&......U..;.@
+00000720: 9a65 9aa2 0e81 2fe7 1c7f fece c5e6 f2aa  .e..../.........
+00000730: c933 6d43 45c5 7831 45f8 c244 1a2d 629e  .3mCE.x1E..D.-b.
+00000740: b062 3545 3f97 913e 465a 2549 9190 8c17  .b5E?..>FZ%I....
+00000750: 748a 76b4 4257 b3af 5f2e b75c bcbe 70fe  t.v.BW.._..\..p.
+00000760: aa01 4051 4dd1 5aca d237 8c2a 5ed3 9c54  ..@QM.Z..7.*^..T
+00000770: 17bc a405 6852 2e72 2261 2a56 4655 0a4a  ....hR.r"a*VFU.J
+00000780: 926a 4da9 cc33 c332 4dcf c809 2b50 87e0  .jM..3.2M...+P..
+00000790: 8b73 3078 9ab2 9886 3cae 735a c80e 44d0  .s0x....<.sZ..D.
+000007a0: 8c48 a05f ad59 59f5 6879 7c0e 5c4e c46b  .H._.YY.hy|.\N.k
+000007b0: 5dea 31cf 4b80 7861 1993 bb16 1469 79ec  ].1.K.xa.....iy.
+000007c0: 5faf 0a2e c84b 066e 37d8 d51a 01af 071f  _....K.n7.......
+000007d0: 36a1 b1fa 9d40 75b2 55ce 62c1 2b9e ca0b  6....@u.U.b.+...
+000007e0: 8036 3ad2 27fe 63d3 c0f8 2804 cd69 0cce  .6:.'.c...(..i..
+000007f0: 4372 0c41 374c e570 6025 bc4f b2f2 062c  Cr.A7L.p`%.O...,
+00000800: ef00 86cd ff46 c350 5a6d adf8 10bc 4fa2  .....F.PZm....O.
+00000810: b903 370b cd2e 5396 d1c7 ae74 3552 9677  ..7...S....t5R.w
+00000820: 2457 99ca 9096 914a 2e12 2669 3245 2398  $W.....J..&i2E#.
+00000830: f22d 3d08 1ca4 89ba 0c6a 9681 d61a b936  .-=......j.....6
+00000840: 46c6 6c28 e77b a101 aca4 e25e b00d 8977  F.l(.{.....^...w
+00000850: 7026 9096 d094 d499 5c42 69f7 1b82 dc72  p&......\Bi....r
+00000860: 2ccb 536b 1be1 f7e1 bf97 4283 f175 7803  ,.Sk......B..ux.
+00000870: 141e c806 0881 dbc9 be5e af61 476c 3f17  .........^.aGl?.
+00000880: b1f0 f1f3 5b10 98d1 241c cdf5 d1c2 5be8  ....[...$.....[.
+00000890: ce28 b2f5 f9c4 1ae9 8b49 e0cd 1761 88c7  .(.......I...a..
+000008a0: 81f5 0e31 139e 1f73 52cb f5de 5705 3d45  ...1...sR...W.=E
+000008b0: 0e38 76a2 ba25 4daf c1a6 5fb3 e440 e3cd  .8v..%M..._..@..
+000008c0: dc3f baea ff68 7add bb72 479d ea47 46b7  .?...hz..rG..GF.
+000008d0: d521 2a6a aa35 4fac 48f8 768a 746c c2ad  .!*j.5O.H.v.tl..
+000008e0: b03b 9e6e 5be5 134b e41a c26a 5b2e 544f  .;.n[..K...j[.TO
+000008f0: 27fb 4ed9 6a0d 8c21 604a 08d9 57cc a6e8  '.N.j..!`J..W...
+00000900: 8851 d831 8ae0 d155 73c4 c8f8 40a9 bd3f  .Q.1...Us...@..?
+00000910: 805a db6b 459b f339 9ce2 ea17 24aa 15b6  .Z.kE..9....$...
+00000920: 5186 24fb 6a13 719d b4f9 3d35 8703 3c98  Q.$.j.q...=5..<.
+00000930: c378 30b7 540c 4ecd ed0f e630 1ecc 6d65  .x0.T.N....0..me
+00000940: 6ef4 ac62 92c5 5042 aa6b 694c b069 4d94  n..b..PB.kiL.iM.
+00000950: 056d e44d 25db 5eab 0503 ef03 771c 98f6  .m.M%.^.....w...
+00000960: c4d2 9d08 47ba 8327 a61e 049e a3bb 6164  ....G..'......ad
+00000970: bb23 1c7e 5bb8 914a bfba 5efd 4621 a69f  .#.~[..J..^.F!..
+00000980: 3c35 63a3 5d4d 89ac 055c df50 b0ed dc57  <5c.]M...\.P...W
+00000990: 6db4 970e c2b4 13ec 237b 74fd f83f c2b6  m.......#{t..?..
+000009a0: dcbb d5ff 327c 80df 4746 cf34 8e1e cf34  ....2|..GF.4...4
+000009b0: fc76 77bb bc3d d3f6 66b1 7c7e 8ada dcfc  .vw..=..f.|~....
+000009c0: d55b 0312 0279 ebd3 62f4 bfb3 d96f 0000  .[...y..b....o..
+000009d0: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
+000009e0: 0021 00de 09fd 2802 0100 00d4 0300 001a  .!....(.........
+000009f0: 0008 0178 6c2f 5f72 656c 732f 776f 726b  ...xl/_rels/work
+00000a00: 626f 6f6b 2e78 6d6c 2e72 656c 7320 a204  book.xml.rels ..
+00000a10: 0128 a000 0100 0000 0000 0000 0000 0000  .(..............
 00000a20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000a80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -171,741 +171,741 @@
 00000aa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ab0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ac0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ad0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ae0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000b10: 0000 00bc 93cf 6ac3 300c c6ef 83bd 83d1  ......j.0.......
-00000b20: 7d71 926e 6594 3abd 8c41 af5b f700 2651  }q.ne.:..A.[..&Q
-00000b30: e2d0 c436 96f6 276f 3f93 43ba 40c9 2ea1  ...6..'o?.C.@...
-00000b40: 1783 24fc 7d3f d0a7 fde1 a7ef c417 066a  ..$.}?.........j
-00000b50: 9d55 9025 2908 b4a5 ab5a db28 f838 bd3e  .U.%)....Z.(.8.>
-00000b60: 3c83 20d6 b6d2 9db3 a860 4082 4371 7fb7  <. ......`@.Cq..
-00000b70: 7fc3 4e73 fc44 a6f5 24a2 8a25 0586 d9ef  ..Ns.D..$..%....
-00000b80: a4a4 d260 af29 711e 6d9c d42e f49a 6319  ...`.)q.m.....c.
-00000b90: 1ae9 7579 d60d ca3c 4db7 32fc d580 62a6  ..uy...<M.2...b.
-00000ba0: 298e 9582 70ac 3620 4e83 8fce ff6b bbba  )...p.6 N....k..
-00000bb0: 6e4b 7c71 e567 8f96 af58 c86f 17ce 6410  nK|q.g...X.o..d.
-00000bc0: 398a ead0 202b 985a 24c7 c926 89c4 20af  9... +.Z$..&.. .
-00000bd0: c3e4 3786 c997 60b2 1bc3 644b 30db 3561  ..7...`...dK0.5a
-00000be0: c8e8 80d5 3b87 9842 baac 6ad6 5e82 795a  ....;..B..j.^.yZ
-00000bf0: 1586 872e 867e 0a0c 8df5 92fd e39a f61c  .....~..........
-00000c00: 4f09 2fee 6329 c777 da87 9cdd 62f1 0b00  O./.c).w....b...
-00000c10: 00ff ff03 0050 4b03 0414 0006 0008 0000  .....PK.........
-00000c20: 0021 008f 560f 0d0c 0d00 0085 5e00 0018  .!..V.......^...
-00000c30: 0000 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-00000c40: 2f73 6865 6574 312e 786d 6c9c 93db 8adb  /sheet1.xml.....
-00000c50: 3010 86ef 0b7d 07a1 fb58 969d cd66 4d9c  0....}...X...fM.
-00000c60: a56c 085d 28a5 747b b856 e471 2c62 59ae  .l.](.t{.V.q,bY.
-00000c70: a41c b6a5 efde 9172 845c 34ac b175 f47c  .......r.\4..u.|
-00000c80: f38f 6634 79dc e996 6cc0 3a65 ba92 f224  ..f4y...l.:e...$
-00000c90: a504 3a69 2ad5 2d4b fafd db7c 30a6 c479  ..:i*.-K...|0..y
-00000ca0: d155 a235 1d94 f415 1c7d 9cbe 7f37 d91a  .U.5.....}...7..
-00000cb0: bb72 0d80 2748 e85c 491b effb 8231 271b  .r..'H.\I....1'.
-00000cc0: d0c2 25a6 870e 776a 63b5 f038 b54b e67a  ..%...wjc..8.K.z
-00000cd0: 0ba2 8a46 ba65 599a 8e98 16aa a37b 4261  ...F.eY......{Ba
-00000ce0: 6f61 98ba 5612 6646 ae35 747e 0fb1 d00a  oa..V.fF.5t~....
-00000cf0: 8ffa 5da3 7a77 a469 790b 4e0b bb5a f703  ..].zw.iy.N..Z..
-00000d00: 6974 8f88 856a 957f 8d50 4ab4 2c9e 979d  it...j...PJ.,...
-00000d10: b162 d162 dc3b 3e14 92ec 2cbe 197e f9d1  .b.b.;>...,..~..
-00000d20: 4d5c bff2 a495 b4c6 99da 2748 667b cdd7  M\........'Hf{..
-00000d30: e13f b007 26e4 8974 1dff 4d18 3e64 1636  .?..&..t..M.>d.6
-00000d40: 2a24 f08c cade 2689 df9d 58d9 1996 bf11  *$....&...X.....
-00000d50: 363a c1c2 71d9 62ad aa92 fe49 0fcf 007b  6:..q.b....I...{
-00000d60: 1e9a f4dc 1cf7 fed2 e9a4 5298 e110 15b1  ..........R.....
-00000d70: 5097 f403 2f66 3ce7 944d 27b1 827e 28d8  P.../f<..M'..~(.
-00000d80: ba8b 31f1 62f1 022d 480f e885 53e2 4dff  ..1.b..-H...S.M.
-00000d90: 096a ff04 6d1b ac39 16f2 6f63 f48b 1421  .j..m..9..oc...!
-00000da0: 9f9c df5d cc3f 872a c5df e26a a8ec 8531  ...].?.*...j...1
-00000db0: abe0 e119 5929 8a71 911c c408 e9d5 06f6  ....Y).q........
-00000dc0: d427 9e63 64ee 5714 1827 a88e 9de4 5d8e  .'.cd.W..'....].
-00000dd0: 8f52 e7f1 3e7c b1a4 825a ac5b ffd5 6c3f  .R..>|...Z.[..l?
-00000de0: 825a 361e 9d0f 9321 9e53 28b4 a27a 9d81  .Z6....!.S(..z..
-00000df0: 9358 e1e8 3ec9 43d0 d2b4 c8c0 9668 156e  .X..>.C......h.n
-00000e00: 2a16 a8d8 c57e ab2a df04 ed94 2cc0 f9b9  *....~.*....,...
-00000e10: 0a2c 4ae4 da79 a37f 1e36 0f88 bd31 e636  .,J..y...6...1.6
-00000e20: 1a63 7f30 cef2 643c 1edd f3f1 3d1e cb8d  .c.0..d<....=...
-00000e30: 140c 3d52 b03f 4a40 ad79 96e6 3cfb 2f85  ..=R.?J@.y..<./.
-00000e40: c578 fe01 0000 ffff 0000 00ff ffb4 9cdb  .x..............
-00000e50: 6e1c 4510 865f 25f2 0324 db73 1ee4 4422  n.E.._%..$.s..D"
-00000e60: f605 af11 198b 7041 8262 13e0 ed99 5ad0  ......pA.b....Z.
-00000e70: 6e7d 555d e594 44b8 02fe aad6 3fed 9efe  n}U]..D.....?...
-00000e80: fa30 5bb7 4f1f 1f1f 9fef 3f3c 7f78 77fb  .0[.O.....?<.xw.
-00000e90: e5f3 9faf bebc bd69 37af 9e7e fff0 e9e9  .......i7..~....
-00000ea0: f8b7 1fa6 9b57 7fb5 e9c3 c30f 3fff 7dff  .....W......?.}.
-00000eb0: f8f4 f0f8 e9f9 edcd e9f5 78f3 eef6 4142  ..........x...AB
-00000ec0: 7f3c 628f fff3 74fc f7d7 77cb 7cfb e6eb  .<b...t...w.|...
-00000ed0: bbdb 370f ff89 efb5 d8a8 dd69 ed44 ed5e  ..7........i.D.^
-00000ee0: 6bc3 457b 73d8 bb78 1ce8 f1e3 61a2 adaf  k.E{s..x....a...
-00000ef0: c71d ffdc bc7a f8e3 e9f9 f36f 3f3d fefa  .....z.....o?=..
-00000f00: cb39 e285 8739 1abd 3ecc 621e 06a2 7918  .9...9..>.b...y.
-00000f10: ad6d 9379 1a2d 8efd a719 bfc7 d31c 8dc6  .m.y.-..........
-00000f20: 4f03 d13c 8dd6 36f3 37bd d7e2 f549 f1b7  O..<..6.7....I..
-00000f30: 39c6 8c1e 3fff cfdf e668 347e 1a88 e669  9...?....h4~...i
-00000f40: b4b6 ade6 6fa3 c5eb 93e2 69e6 eff1 3447  ....o.....i...4G
-00000f50: a3f1 d340 344f a3b5 cd0c d17b 2d06 7f9b  ...@4O.....{-...
-00000f60: a5f0 6e1f b1b1 4988 c6a4 d66c 8f6b 6deb  ..n...I....l.km.
-00000f70: bf0d 6bc1 e311 1b7b 8468 3c6a 6d37 a342  ..k....{.h<jm7.B
-00000f80: 6b2d 9880 b682 c923 3636 09d1 98d4 da60  k-.....#66.....`
-00000f90: 66d0 7b88 81cb bde0 f288 8d5d 4234 2eb5  f.{........]B4..
-00000fa0: 36d8 b95c 8bed dad1 78c5 daa9 429c 2338  6..\....x...B.#8
-00000fb0: f629 4d5d 5563 1462 73d4 d1a9 2d98 a95b  .)M]Uc.bs...-..[
-00000fc0: 098e a0a3 058a 3415 5b05 3bed 9f1e a92d  ......4.[.;....-
-00000fd0: 78d5 9b61 64ce f194 7dd2 546c 558b cdf2  x..ad...}.TlU...
-00000fe0: 02a9 edda 071c 0006 80b9 d514 6c2d 231b  ............l-#.
-00000ff0: c466 a726 aac1 e4d4 0cdd 72ab 29b5 a4a9  .f.&......r.)...
-00001000: 4baf 0ed7 0177 5e59 dd41 7556 911a 0d00  K....w^Y.AuV....
-00001010: 83ae dc6a 8aa4 a655 6f55 ab76 3245 6a34  ...j...UoU.v2Ej4
-00001020: 9bb6 0a97 2438 9901 b4ea ad82 3fae 5bb5  ....$8......?.[.
-00001030: 1aac 075a 054f 129c 58d5 aab7 0ad5 bd57  ...Z.O..X......W
-00001040: 50a3 f7aa 42a9 9662 0aaa f7aa 73fd cc0a  P...B..b....s...
-00001050: 545d 3b9d 7340 8555 2d85 1554 ef15 4872  T];.s@.U-..T..Hr
-00001060: 532b 6816 4c02 4305 5812 9c6c 2bb4 eabc  S+h.L.C.X..l+...
-00001070: 22d7 cdad 5087 00ae 4385 5812 9c78 c5c6  "...P...C.X..x..
-00001080: cc4e 58c8 7593 2bd4 f1ca 5eee ea2a c81a  .NX.u.+...^..*..
-00001090: f2ed 9a56 7dbf e63b 366c d9ae 2384 5e2b  ...V}..;6l..#.^+
-000010a0: cc1a 5266 41f5 5e75 ee78 5de8 9d31 718f  ..RfA.^u.x]..1q.
-000010b0: dc35 da2d 57a0 35a4 d082 eabd eadc c94e  .5.-W.5........N
-000010c0: afc8 1d83 15d6 50a1 9604 27e3 55ab a3d9  ......P...'.U...
-000010d0: 97df 2177 b7d8 823a 062c 182a d892 e0c4  ..!w...:.,.*....
-000010e0: ab56 bd57 adee ae5f 911b b060 a870 4b82  .V.W..._...`.pK.
-000010f0: 13af 5af5 5eb5 eaac 2235 40c1 50c1 9604  ..Z.^..."5@.P...
-00001100: 2756 b5ea ad12 5b76 4780 a6c7 8805 156e  'V....[vG......n
-00001110: 0d29 b7a0 7ab3 3ad7 0d57 2d8e 010a c60a  .)..z.:..W-.....
-00001120: b624 38ee 57a8 ce2a d476 b28c 853c 052c  .$8.W..*.v...<.,
-00001130: 182b dc92 e0c4 ac56 bd59 50cd 9d77 6975  .+.....V.YP..wiu
-00001140: 0a58 3056 b825 c189 57b0 c7ce 59c8 6d27  .X0V.%..W...Y.m'
-00001150: 0b03 c853 0083 b102 2e09 4ecc 024d ceac  ...S......N..M..
-00001160: 56dd a210 2d4f d1c1 6805 5c63 0a2e a87e  V...-O..h.\c...~
-00001170: 10e8 dce6 062c d4a8 5f2b e01a 5370 41f5  .....,.._+..SpA.
-00001180: 5e71 0868 6758 e406 dc1a 2bdc 92e0 6408  ^q.hgX....+...d.
-00001190: a4dc 42ae 5bbf 429d 825d ec58 e196 0427  ..B.[.B..].X...'
-000011a0: 5e53 6e21 d7ad 5fa1 4e51 bf56 c035 a6e0  ^Sn!.._.NQ.V.5..
-000011b0: 82ea 8700 b0e6 a601 ad4e c17a 60ac 704b  .........N.z`.pK
-000011c0: 8293 7e05 7cdc 34a0 55b7 2644 cb53 c0d8  ..~.|.4.U.&D.S..
-000011d0: a902 2e09 8ebd 4275 fd0a 75bf baf9 77ad  ......Bu..u...w.
-000011e0: 0d75 0a20 3b55 b825 c189 d794 5bc8 9ded  .u. ;U.%....[...
-000011f0: da85 6ac0 ada9 c22d 094e bca6 dc42 ee6c  ..j....-.N...B.l
-00001200: c72b d500 0553 055b 129c 784d b185 dcd9  .+...S.[..xM....
-00001210: dee6 418d ce33 a70a b624 38f1 aa55 3f5e  ..A..3...$8..U?^
-00001220: 71bb e5bc e27a 2b98 b3a6 0ab6 2438 f19a  q....z+.....$8..
-00001230: eeb7 903b dbbb 2baa c1c6 60aa 704b 8213  ...;..+...`.pK..
-00001240: af38 ea33 6ffa 1d72 dd1d 285b 0ed6 af53  .8.3o..r..([...S
-00001250: 855b 129c 78d5 eaec bc66 fb2d 343c 4753  .[..x....f.-4<GS
-00001260: 5605 5b53 8a2d a8de aace b55b 18a4 4607  V.[S.-.....[..F.
-00001270: c553 855a 129c f4aa 56bd 55ad fa7b 63e4  .S.Z....V.U..{c.
-00001280: f6af 31e7 0ab4 2438 b60a d559 853a d80d  ..1...$8...Y.:..
-00001290: 0cd5 6031 3057 a025 c189 57ad 7aaf b8d7  ..`10W.%..W.z...
-000012a0: b2d0 62cb 01b4 e60a b424 38f1 aa55 ef15  ..b......$8..U..
-000012b0: 8784 eeb2 1d2d 077b 82b9 022d 094e bc6a  .....-.{...-.N.j
-000012c0: d57b c55e cbee 5fd8 7200 d8b9 022d 094e  .{.^.._.r....-.N
-000012d0: bc02 3c76 c242 aedb 1450 8dc6 6b05 5a73  ..<v.B...P..k.Zs
-000012e0: 0a2d a8be 5fb1 d7b2 8045 6ed4 ad15 66cd  .-.._....En...f.
-000012f0: 29b3 a07a ab3a d7ed 5fd8 72b0 d79a 2bcc  )..z.:.._.r...+.
-00001300: 92e0 cb10 d8ed ed36 5477 4e0c d5ee 6021  .......6TwN...`!
-00001310: 2ec1 5260 ae30 4b82 13ab b89e b2d7 1ac8  ..R`.0K.........
-00001320: 6d27 23df 435e 82fd cb5c a196 0427 6671  m'#.C^...\...'fq
-00001330: 3fe5 cc66 6784 6878 09d6 024b 855a 121c  ?..fg.hx...K.Z..
-00001340: 5b85 ea86 0055 4b2d a8d1 6260 a950 4b82  [....UK-..b`.PK.
-00001350: 13af e9d5 1672 dd62 006a b0ca 5e2a d092  .....r.b.j..^*..
-00001360: e0c4 6a7a b385 5c77 e806 7508 26d7 a502  ..jz..\w..u.&...
-00001370: 2d09 4ebc 6ad5 0f81 145a 6879 0d56 d94b  -.N.j....Zhy.V.K
-00001380: 055a 129c 78d5 aaf7 9aee b4d0 f21a 2c5c  .Z..x.........,\
-00001390: 960a b424 38f1 9a7e 8f81 5c07 58a8 d18d  ...$8..~..\.X...
-000013a0: e152 a196 0427 5eb5 eafb 35a5 165a 5e03  .R...'^...5..Z^.
-000013b0: c22e 156a 4970 e235 3d21 64ae ddbf 408d  ...jIp.5=!d...@.
-000013c0: 6e0c 970a b624 38f1 9a5e 6d31 d77d 8589  n....$8..^m1.}..
-000013d0: dc68 1ea8 506b 49a9 05d5 9d62 4075 5671  .h..PkI....b@uVq
-000013e0: b818 ac06 d60a b524 38ee 56a8 ce2a d476  .......$8.V..*.v
-000013f0: b21b 1826 47df b756 b0b5 a6d8 82ea cd22  ...&G..V......."
-00001400: d77e e48a c3c5 6035 b056 b025 c149 bfa6  .~....`5.V.%.I..
-00001410: 0784 c8f5 3786 90a3 1bc3 b5c2 2d09 4ecc  ....7.......-.N.
-00001420: a627 84c8 751b 6ea8 d18d e15a e196 0427  .'..u.n....Z...'
-00001430: 5ed3 1342 e4fa 1b43 c8d1 8de1 5a01 9704  ^..B...C....Z...
-00001440: 2766 d323 42e4 bac5 0bd4 2580 ec5a 0197  'f.#B.....%..Z..
-00001450: 0427 5ed3 ab2d e4ba 1b43 a8d1 1e66 ad80  .'^..-...C...f..
-00001460: 4b82 13af 29b8 90eb f730 90a3 3dcc 5a21  K...)....0..=.Z!
-00001470: 9704 2766 5372 21d7 ad5e a046 9b98 b542  ..'fSr!..^.F...B
-00001480: 2e09 4ebc a677 5bc8 757b 6ea8 6bb0 e7de  ..N..w[.u{n.k...
-00001490: 2ae8 92e0 d82b 5447 03aa f60e 06ea 1aec  *....+TG........
-000014a0: 62b6 0ab9 2438 f19a de6d 21d7 dd19 425d  b...$8...m!...B]
-000014b0: 83d5 cb56 4197 0427 5e53 7431 d7de 1942  ...VA..'^St1...B
-000014c0: 8dee 0cb7 0ab9 2438 f19a 920b b9ee ce90  ......$8........
-000014d0: 6a30 c16e 1572 4970 e235 2517 72dd 9d21  j0.n.rIp.5%.r..!
-000014e0: d560 67b0 55c0 25c1 89d7 145c c875 7786  .`g.U.%....\.uw.
-000014f0: 50a3 3bc3 ad02 2e09 4ebc a6e0 42ae fbb5  P.;.....N...B...
-00001500: 22d4 399a 072a e0da 5270 41f5 7316 6ebe  ".9..*..RpA.s.n.
-00001510: ec11 3c72 e760 6bb0 55b8 25c1 49bf e2ea  ..<r.`k.U.%.I...
-00001520: cbfe 564b 8bee ca10 0d47 24a8 506b 4ba9  ..VK.....G$.PkK.
-00001530: 05d5 74db 1d44 bbdd a218 f4e9 5e61 9604  ..t..D......^a..
-00001540: c77d 0ad5 3a65 aad9 c030 3372 5a21 d69e  .}..:e...03rZ!..
-00001550: 120b aa73 ca7b 2d7b 4acc dc60 5fb8 5788  ...s.{-{J..`_.W.
-00001560: 25c1 49af e272 cafe 5e0f 0788 f6e4 150d  %.I..r..^.......
-00001570: 470b acbd 022c 094e ace2 d6cb 5ac5 09a1  G....,.N....Z...
-00001580: fb6d a156 a3f5 d55e e195 0427 5671 e965  .m.V...^...'Vq.e
-00001590: ad6a d1ed 07d0 7074 f0ba 5770 25c1 8955  .j....pt..Wp%..U
-000015a0: dc79 59ab 5a74 2b6c 34bc 4663 b542 ab3d  .yY.Zt+l4.Fc.B.=
-000015b0: a515 54f7 5ee9 54f7 8367 a4ae c119 c65e  ..T.^.T..g.....^
-000015c0: 8195 0427 bd8a cf34 6caf 6ad1 ed05 d0f0  ...'...4l.j.....
-000015d0: 169c 66ef 1556 4970 6235 6315 52dd 4f4a  ..f..VIpb5c.R.OJ
-000015e0: a046 cb95 bd02 2b09 4eac 6ad5 0d00 2dba  .F....+.N.j...-.
-000015f0: d50a 1a8e 7eb2 7baa d0ea 38d3 cbbc 52b6  ....~.{...8...R.
-00001600: 66a9 ba7d 0be5 2d58 601f a75f a59f 43a7  f..}..-X`.._..C.
-00001610: d03a 3776 e97a 7767 4cd9 ad5a 282f c1a8  .:7v.zwgL..Z(/..
-00001620: 3d4e 954a 8653 729d 1bcb 0ceb 6cbb 7861  =N.J.Sr.....l.xa
-00001630: f216 7c94 711c 8094 fca6 f83a 3796 f945  ..|.q......:7..E
-00001640: b659 c230 393a 266a a70a c2ce d1f1 cb46  .Y.09:&j.......F
-00001650: b933 2080 3177 ddcd f4e8 aca8 9d2a 243b  .3 .1w.......*$;
-00001660: 4767 8e35 ae3a 8e71 17e6 7e27 2b56 2e8d  Gg.5.:.q..~'+V..
-00001670: 6fe1 1c51 e159 3ba5 40a3 dc31 8c2b 2f5f  o..Q.Y;.@..1.+/_
-00001680: 8640 cbd1 aaa6 9d2a 543b 4767 3d8c 6d96  .@.....*T;Gg=.m.
-00001690: fd5e 87d9 6e69 4339 5adb b453 856d e7e8  .^..niC9Z..S.m..
-000016a0: ccb0 a65b a787 b5ec 4b12 8895 4be3 d141  ...[....K...K..A
-000016b0: 723b 5508 778e ce0c 6b8c 750c 8372 769f  r;U.w...k.u..rv.
-000016c0: cbc6 9768 5aab 95d1 4031 0cf7 f94e 83ec  ...hZ...@1...N..
-000016d0: 0db3 9486 9b87 5986 23ac a551 021d 8a5e  ......Y.#..Q...^
-000016e0: 740c 6b0e 760c e3bc d19e 7e36 56d4 088e  t.k.v.....~6V...
-000016f0: 145b ada4 064a 5f74 0c6b 9275 0c6b d92d  .[...J_t.k.u.k.-
-00001700: 7cce 562e e32d ece0 12e8 50ff a2e3 5793  |.V..-....P...W.
-00001710: ace3 57cb 7ee9 c3ba 1c51 c58a 5a75 0d94  ..W.~....Q..Zu..
-00001720: c8d8 ccb4 f5be 413e de21 5b0d 86e9 7e0c  ......A>.![...~.
-00001730: 6b12 46c5 20a4 bac5 b717 4b43 2d8c 8e61  k.F. .....KC-..a
-00001740: eccb 3a86 a9db af11 1b9b 8f8a edd4 6a6d  ..:...........jm
-00001750: a0d8 46c7 3259 e6fb 98ba a333 9adf a305  ..F.2Y.....3....
-00001760: 66ad e606 8a6e 742c 639f d6e9 65ad fb51  f....nt,c...e..Q
-00001770: 810d 62b4 8497 6a19 8561 81a3 433f 8e41  ..b...j..a..C?.A
-00001780: b38e 61ea 8e1e 28dd b187 f428 e10e 2536  ..a...(....(..%6
-00001790: 3a7d ac79 d67b f5a8 fb5e c686 319a de4a  :}.y.{...^..1..J
-000017a0: 6538 1aaa 6578 cb2c b5e1 7bd9 e8f6 9e87  e8..ex.,..{.....
-000017b0: cdef 614d a612 f250 34a3 6399 878e eee5  ..aM...P4.c.....
-000017c0: 43ba abcb 4335 9ae0 a4ca c6b7 8f64 d4e4  C...C5.......d..
-000017d0: e818 d64c eb0c 0ba6 bbf9 0d72 f495 5d93  ...L.......r..].
-000017e0: 8a18 05c7 1a5b 1dc7 3c80 f45d ac75 f729  .....[..<..].u.)
-000017f0: c8d9 cb85 d2d1 b776 4dea 6214 1ce3 4b44  .......vM.b...KD
-00001800: 375b a0c8 46af 8fb9 c1b3 3b52 a447 5fdc  7[..F.....;R.G_.
-00001810: b552 918e 7374 b236 46a9 8d9e e317 b087  .R..st.6F.......
-00001820: fc2d c25e a956 4743 b10e bf16 82dc b38c  .-.^.VGC........
-00001830: 3d9c eb63 6c1f 2386 940a 7634 54ec e818  =..cl.#...v4T...
-00001840: 7e01 7a48 3f36 b0ce 32b0 1731 a454 b8a3  ~.zH?6..2..1.T..
-00001850: a1bc 46c7 f20b d863 ba33 8c6c f52d 118b  ..F....c.3.l.-..
-00001860: 4e49 c98d c2ab 979e 6336 d4ef e88d 8af4  NI......c6......
-00001870: 2c93 e9e1 f456 2ae2 d150 6ac3 f7b1 29d4  ,....V*..Pj...).
-00001880: e1a6 37e8 7e7a 831c 4e6f a54a 1e0d a53c  ..7.~z..No.J...<
-00001890: 3a8e 5f60 1ed2 7d25 32c8 6e7a 7b73 2d86  :._`..}%2.nz{s-.
-000018a0: fc0f 0000 00ff ff00 0000 ffff 448f 410e  ............D.A.
-000018b0: 8240 0c45 af32 e901 0463 8c1b 60a3 1b17  .@.E.2...c..`...
-000018c0: 2626 9c60 84c2 34e2 b429 5523 a777 2012  &&.`..4..)U#.w .
-000018d0: 777d bfcd ffbf 8504 8e68 d45c d575 1ced  w}.......h.\.u..
-000018e0: dc96 b005 671f c112 221f 39be 5047 e208  ....g...".9.PG..
-000018f0: 5955 88ef f1e2 b5a7 38ba 013b 2b21 df1c  YU......8..;+!..
-00001900: c029 f561 9d8d 6551 f7e0 6e6c c68f 9502  .).a..eQ..nl....
-00001910: fa16 75a6 1da4 24b6 157e be35 da53 9c78  ..u...$..~.5.S.x
-00001920: 41ad 694a e139 3856 c268 de52 7c09 c26a  A.iJ.98V.h.R|..j
-00001930: eac9 c085 a44f a9ab 1f4e 42cb 61ea 985e  .....O...NB.a..^
-00001940: f873 c342 38ce abe4 9ebd 59ef 6340 b4ea  .s.B8.....Y.c@..
-00001950: 0b00 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
-00001960: 0000 0021 0063 fdce 8f11 0200 00f3 0300  ...!.c..........
-00001970: 0018 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
-00001980: 7473 2f73 6865 6574 322e 786d 6c9c 925b  ts/sheet2.xml..[
-00001990: 6bc2 3014 c7df 07fb 0e21 ef36 6d75 324b  k.0......!.6mu2K
-000019a0: ab0c 44e6 db18 dbde 637a da06 9ba4 24f1  ..D.....cz....$.
-000019b0: c6d8 77df 49dd 54f0 450c b95f 7ee7 9c9c  ..w.I.T.E.._~...
-000019c0: 7f3e dbab 966c c13a 6974 4193 28a6 04b4  .>...l.:itA.(...
-000019d0: 30a5 d475 413f 3f16 8367 4a9c e7ba e4ad  0..uA??..gJ.....
-000019e0: d150 d003 383a 9b3e 3ee4 3b63 d7ae 01f0  .P..8:.>>.;c....
-000019f0: 0409 da15 b4f1 becb 1873 a201 c55d 643a  .........s...]d:
-00001a00: d078 5219 abb8 c7a5 ad99 eb2c f0b2 7fa4  .xR........,....
-00001a10: 5a96 c6f1 9829 2e35 3d12 327b 0bc3 5495  Z....).5=.2{..T.
-00001a20: 1430 3762 a340 fb23 c442 cb3d faef 1ad9  .07b.@.#.B.=....
-00001a30: b97f 9a12 b7e0 14b7 eb4d 3710 4675 8858  .........M7.Fu.X
-00001a40: c956 fa43 0fa5 4489 6c59 6b63 f9aa c5b8  .V.C..D.lYkc....
-00001a50: f7c9 880b b2b7 5853 6cc3 7f33 fdfe 9525  ......XSl..3...%
-00001a60: 2585 35ce 543e 4232 3bfa 7c1d fe84 4d18  %.5.T>B2;.|...M.
-00001a70: 1727 d275 fc37 6192 11b3 b095 2181 6754  .'.u.7a.....!.gT
-00001a80: 7a9f 4bc9 d389 959e 61c3 3b61 e313 2c7c  z.K.....a.;a..,|
-00001a90: 97cd 36b2 2ce8 77fc 5706 3826 a18b 0771  ..6.,.w.W.8&...q
-00001aa0: 12ba 8bf2 43a7 7929 31c3 212a 62a1 2ae8  ....C.y)1.!*b.*.
-00001ab0: 4b42 d934 efc5 f325 61e7 2ee6 2468 7165  KB.4...%a...$hqe
-00001ac0: cc3a 1c2c d146 1cae b2ab bb8b 5e8b 6f96  .:.,.F......^.o.
-00001ad0: 9450 f14d ebdf cdee 1564 dd78 14fe 281a  .P.M.....d.x..(.
-00001ae0: a18f 21c9 5979 9883 13a8 2e04 4543 44fd  ..!.Yy......ECD.
-00001af0: 0200 00ff ff00 0000 ffff b229 ce48 4d2d  ...........).HM-
-00001b00: 7149 2c49 d4b7 0300 0000 ffff 0000 00ff  qI,I............
-00001b10: ff44 8c41 0ac2 400c 45af 1272 002b 88b8  .D.A..@.E..r.+..
-00001b20: 69bb 72eb aa27 186b 3a13 ac4d 48a3 424f  i.r..'.k:..MH.BO
-00001b30: ef4c 6170 f7df 7f9f df6a 8874 0b16 7959  .Lap.....j.t..yY
-00001b40: 61a6 c93b 3c1e 2e08 c631 d5ec a27b 7b46  a..;<....1...{{F
-00001b50: b88b bbbc 2a25 0a0f b242 2784 49c4 2b34  ....*%...B'.I.+4
-00001b60: 7d5b 7e07 f2b7 8206 251b 78a3 3c44 1063  }[~.....%.x.<D.c
-00001b70: 5a3c 38cb d2a1 8ab9 0576 8494 fb4d b298  Z<8......v...M..
-00001b80: afca fbf0 43e6 3cfe 7914 655a 8bca efcd  ....C.<.y.eZ....
-00001b90: 57ec b926 22ef 7f00 0000 ffff 0300 504b  W..&".........PK
-00001ba0: 0304 1400 0600 0800 0000 2100 9c73 ee78  ..........!..s.x
-00001bb0: 1402 0000 f303 0000 1800 0000 786c 2f77  ............xl/w
-00001bc0: 6f72 6b73 6865 6574 732f 7368 6565 7433  orksheets/sheet3
-00001bd0: 2e78 6d6c 9c92 df6b c230 10c7 df07 fb1f  .xml...k.0......
-00001be0: 42de 6d5a ed64 9656 1988 ccb7 31b6 bdc7  B.mZ.d.V....1...
-00001bf0: f46a 834d 5292 f88b b1ff 7d97 3a75 d017  .j.MR.....}.:u..
-00001c00: b1a4 f975 c9e7 ee72 df7c 7650 0dd9 8175  ...u...r.|vP...u
-00001c10: d2e8 8226 514c 0968 614a a9d7 05fd fc58  ...&QL.haJ.....X
-00001c20: 0c9e 2971 9eeb 9237 4643 418f e0e8 6cfa  ..)q...7FCA...l.
-00001c30: f890 ef8d ddb8 1ac0 1324 6857 d0da fb36  .........$hW...6
-00001c40: 63cc 891a 1477 9169 41a3 a532 5671 8f4b  c....w.iA..2Vq.K
-00001c50: bb66 aeb5 c0cb ee92 6ad8 308e c74c 71a9  .f......j.0..Lq.
-00001c60: e989 90d9 5b18 a6aa a480 b911 5b05 da9f  ....[.......[...
-00001c70: 2016 1aee 317e 57cb d69d 694a dc82 53dc   ...1~W...iJ..S.
-00001c80: 6eb6 ed40 18d5 2262 251b e98f 1d94 1225  n..@.."b%......%
-00001c90: b2e5 5a1b cb57 0de6 7d48 522e c8c1 621b  ..Z..W..}HR...b.
-00001ca0: e23f 3abb e9f6 7b9e 9414 d638 53f9 08c9  .?:...{....8S...
-00001cb0: ec14 733f fd09 9b30 2e2e a47e fe37 6192  ..s?...0...~.7a.
-00001cc0: 9459 d8c9 50c0 2b6a 785f 48c9 d385 35bc  .Y..P.+jx_H...5.
-00001cd0: c246 77c2 c617 5878 2e9b 6d65 59d0 eff8  .Fw...Xx..meY...
-00001ce0: ef1b e098 842e 1ec4 a885 6e76 b6fd d069  ..........nv...i
-00001cf0: 5e4a ac70 c88a 58a8 0afa 9250 36cd 3bf1  ^J.p..X....P6.;.
-00001d00: 7c49 d8bb 7f73 12b4 b832 6613 0c4b f411  |I...s...2f..K..
-00001d10: 87a3 ac77 76d1 69f1 cd92 122a be6d fcbb  ...wv.i....*.m..
-00001d20: d9bf 825c d71e 859f 4629 c618 8a9c 95c7  ...\....F)......
-00001d30: 3938 81ea 4250 3442 d42f 0000 00ff ff00  98..BP4B./......
-00001d40: 0000 ffff b229 ce48 4d2d 7149 2c49 d4b7  .....).HM-qI,I..
-00001d50: 0300 0000 ffff 0000 00ff ff44 8c41 0ac2  ...........D.A..
-00001d60: 400c 45af 1272 002b 88b8 69bb 72eb aa27  @.E..r.+..i.r..'
-00001d70: 186b 3a13 ac4d 48a3 424f ef4c 6170 f7df  .k:..MH.BO.Lap..
-00001d80: 7f9f df6a 8874 0b16 7959 61a6 c93b 3c1e  ...j.t..yYa..;<.
-00001d90: 2e08 c631 d5ec a27b 7b46 b88b bbbc 2a25  ...1...{{F....*%
-00001da0: 0a0f b242 2784 49c4 2b34 7d5b 7e07 f2b7  ...B'.I.+4}[~...
-00001db0: 8206 251b 78a3 3c44 1063 5a3c 38cb d2a1  ..%.x.<D.cZ<8...
-00001dc0: 8ab9 0576 8494 fb4d b298 afca fbf0 43e6  ...v...M......C.
-00001dd0: 3cfe 7914 655a 8bca efcd 57ec b926 22ef  <.y.eZ....W..&".
-00001de0: 7f00 0000 ffff 0300 504b 0304 1400 0600  ........PK......
-00001df0: 0800 0000 2100 f8a6 e9a8 8a06 0000 ec1b  ....!...........
-00001e00: 0000 1300 0000 786c 2f74 6865 6d65 2f74  ......xl/theme/t
-00001e10: 6865 6d65 312e 786d 6cec 594f 6f13 4714  heme1.xml.YOo.G.
-00001e20: bf57 ea77 18ed 1d62 3bb6 1347 3828 766c  .W.w...b;..G8(vl
-00001e30: d242 204a 0c15 c7f1 7abc 3b78 7667 3533  .B J....z.;xvg53
-00001e40: 4ef0 0dc1 b152 a50a 5af5 52a9 b71e aab6  N....R..Z.R.....
-00001e50: 4820 f542 bf4c d352 b554 e22b f4cd ccda  H .B.L.R.T.+....
-00001e60: de89 2710 43a4 9616 1f12 7bf6 f7fe ccfb  ..'.C.....{.....
-00001e70: 37ef cd5e ba7c 3761 e890 0849 79da 0cca  7..^.|7a...Iy...
-00001e80: 174b 0122 69c8 0734 8d9a c1cd 5ef7 c27a  .K."i..4....^..z
-00001e90: 80a4 c2e9 0033 9e92 6630 2132 b8bc f9e1  .....3..f0!2....
-00001ea0: 0797 f086 8a49 4210 d0a7 7203 3783 58a9  .....IB...r.7.X.
-00001eb0: 6c63 6545 86b0 8ce5 459e 9114 9e0d b948  lceE....E......H
-00001ec0: b082 9f22 5a19 087c 047c 13b6 5229 95ea  ..."Z..|.|..R)..
-00001ed0: 2b09 a669 8052 9c00 db1b c321 0d09 ea19  +..i.R.....!....
-00001ee0: 96f0 740d 5d40 9552 b914 6c4e 0575 1848  ..t.]@.R..lN.u.H
-00001ef0: 4b95 d40b 2113 075a 0cc9 a9f7 f088 1285  K...!..Z........
-00001f00: 7226 9afc 977b 0f67 e483 5159 13c9 896c  r&...{.g..QY...l
-00001f10: 3381 0e31 6b06 a0c6 801f f5c8 5d15 2086  3..1k.......]. .
-00001f20: a582 07cd a064 3ec1 cae6 a515 bc91 1331  .....d>........1
-00001f30: 750a 6d81 ae6b 3e39 5d4e 3018 558c 4c11  u.m..k>9]N0.U.L.
-00001f40: f567 42cb dd6a 636d 7bc6 df00 985a c475  .gB..jcm{....Z.u
-00001f50: 3a9d 76a7 3ce3 6700 380c 61f3 5697 22cf  :.v.<.g.8.a.V.".
-00001f60: 6a77 bddc 9af2 2c80 ecd7 45de ed52 ad54  jw....,...E..R.T
-00001f70: 75f1 05fe ab0b 3a37 5aad 56ad 91eb 6299  u.....:7Z.V...b.
-00001f80: 1a90 fd5a 5dc0 af97 ead5 ad8a 8337 208b  ...Z]........7 .
-00001f90: af2d e0ab adad 76bb eee0 0dc8 e2eb 0bf8  .-....v.........
-00001fa0: ee5a a35e 75f1 0614 339a 8e16 d0da a1dd  .Z.^u...3.......
-00001fb0: 6ece 7d06 1972 b6e3 85af 037c bd94 c3e7  n.}..r.....|....
-00001fc0: 2888 8659 c069 1143 9eaa 25c2 2fc1 77b8  (..Y.i.C..%./.w.
-00001fd0: e802 8da6 6558 d114 a949 4686 3884 b86f  ....eX...IF.8..o
-00001fe0: e3a4 2f28 d632 f106 c185 2776 2994 0b4b  ../(.2....'v)..K
-00001ff0: 5a3c 92a1 a099 6a06 1f67 1872 68ce efe5  Z<....j..g.rh...
-00002000: b3ef 5f3e 7b82 5e3e 7b7c 7cff e9f1 fd9f  .._>{.^>{||.....
-00002010: 8e1f 3c38 beff a3e5 e510 eee0 342a 12be  ..<8........4*..
-00002020: f8f6 f3bf bebe 87fe 7cf2 cd8b 475f f8f1  ........|...G_..
-00002030: b288 ffed 874f 7ffd f9a1 1f08 4935 d7e8  .....O......I5..
-00002040: f997 8f7f 7ffa f8f9 579f fdf1 dd23 0f7c  ........W....#.|
-00002050: 4be0 7e11 dea3 0991 e83a 3942 fb3c 81bd  K.~......:9B.<..
-00002060: 19c3 b89a 93be 588e a217 63ea 50e0 1878  ......X...c.P..x
-00002070: 7b58 7754 ec00 af4f 30f3 e15a c435 de2d  {XwT...O0..Z.5.-
-00002080: 01f5 c407 bc32 bee3 e87a 108b b1a2 1ec9  .....2...z......
-00002090: 57e3 c401 ee72 ce5a 5c78 0d70 55cb 2a58  W....r.Z\x.pU.*X
-000020a0: b837 4e23 bf70 312e e2f6 313e f4c9 6ee3  .7N#.p1...1>..n.
-000020b0: d471 6d67 9c41 6d9d 06a5 63fb 764c 1c35  .qmg.Am...c.vL.5
-000020c0: f718 4e15 8e48 0ad5 573f e323 423c bbbb  ..N..H..W?.#B<..
-000020d0: 4da9 63d7 5d1a 0a2e f950 a1db 14b5 30f5  M.c.]....P....0.
-000020e0: 9aa4 47fb 4e20 cd89 7668 027e 99f8 f60c  ..G.N ..vh.~....
-000020f0: ae76 6cb3 7b0b b538 f3ed 7a9b 1cba 4848  .vl.{..8..z...HH
-00002100: 08cc 3cca f708 73cc 7805 8f15 4e7c 2c7b  ..<...s.x...N|,{
-00002110: 3861 4583 5fc3 2af6 2979 3011 6111 d791  8aE._.*.)y0.a...
-00002120: 0a3c 1d11 c651 6740 a4f4 d1dc 10b0 df82  .<...Qg@........
-00002130: d3af 6228 615e b7ef b249 e222 85a2 231f  ..b(a^...I."..#.
-00002140: cf6b 98f3 2272 9b8f da31 4e32 afce 348d  .k.."r...1N2..4.
-00002150: 8bd8 8fe4 0842 14a3 3dae 7cf0 5dee 6688  .....B..=.|.].f.
-00002160: fe0d 7ec0 e9a9 eebe 0527 f872 697d 9346  ..~......'.ri}.F
-00002170: 8e4a f300 d14f c6c2 e3cb 2b84 bbf9 3861  .J...O....+...8a
-00002180: 434c 4c95 812a ef54 ea84 a6af 2adb 8c42  CLL..*.T....*..B
-00002190: dd7e 5fb6 a7e7 d816 1c62 bee4 d939 51ac  .~_......b...9Q.
-000021a0: 4fc3 bd83 257a 1b8f d33d 0259 b178 44bd  O...%z...=.Y.xD.
-000021b0: afd0 ef2b 74f0 9faf d0a7 e5f2 f9d7 e579  ...+t..........y
-000021c0: 2986 2a3d 6fbf 4d33 9e2c d38b 0f29 6307  ).*=o.M3.,...)c.
-000021d0: 6ac2 c835 69da 7109 67d2 a00b 8b66 7430  j..5i.q.g....ft0
-000021e0: 23e5 6c5c cb62 f89a 0f03 0e2e 12d8 d020  #.l\.b......... 
-000021f0: c1d5 2754 c507 31ce a095 2f9b 5935 9239  ..'T..1.../.Y5.9
-00002200: eb48 a28c 4b98 2acd b299 8ac9 09de 66b6  .H..K.*.......f.
-00002210: a5d0 cd9b 99b4 a6a7 155b 4c24 56bb 7c60  .........[L$V.|`
-00002220: 9757 8b53 e98c 8d99 5123 330c 4f05 ad6a  .W.S....Q#3.O..j
-00002230: 0667 15b6 baf6 76c2 ca56 ab53 cde6 6ead  .g....v..V.S..n.
-00002240: 6c54 3375 d2d9 da6c cbe0 d6c5 adc1 e2cc  lT3u...l........
-00002250: 9ad0 ec20 6891 c0ca 7518 efb5 ee30 0261  ... h...u....0.a
-00002260: 4606 daee 7662 9fba 458b 3e57 17c9 180f  F...vb..E.>W....
-00002270: 48ee 23bd ef45 1f95 8d93 a6b1 320d 238f  H.#..E......2.#.
-00002280: 8ff4 84f9 1a1f 15a4 3534 dbb7 9076 1627  ........54...v.'
-00002290: 15c5 554f 1137 f5de db78 693a 56cf bda4  ..UO.7...xi:V...
-000022a0: 53f9 443a b2b4 989c 2c45 47cd a051 abd4  S.D:....,EG..Q..
-000022b0: 0214 e2ac 190c 617a 86af 4906 5e97 babf  ......az..I.^...
-000022c0: c42c 824b ab50 091b f6af 4d66 13ae 736f  .,.K.P....Mf..so
-000022d0: 36fc 6159 863b 126b f785 0d3b 7520 1352  6.aY.;.k...;u .R
-000022e0: 6d63 19db d030 8ff2 1060 a999 f58d fe95  mc...0...`......
-000022f0: 1a98 f5bc 3660 23fd 0db4 585d 8760 f8c7  ....6`#...X].`..
-00002300: b400 3bba ae25 c321 0955 d1d9 8515 7315  ..;..%.!.U....s.
-00002310: 6200 7929 e563 45c4 413c 3842 7d36 16fb  b.y).cE.A<8B}6..
-00002320: 18dc af43 15f6 33a0 122e 414c 45d0 3fe0  ...C..3...ALE.?.
-00002330: 124f 5bdb 3c72 8b73 9e74 c5ab 3383 b3eb  .O[.<r.s.t..3...
-00002340: 9865 31ce cbad 4ed1 6926 5bb8 c9e3 990e  .e1...N.i&[.....
-00002350: e697 d5d6 a807 7bf3 ea6e 36b7 fc56 4cca  ......{..n6..VL.
-00002360: 9fd3 568a 61fc 3fdb 8a3e 4fe0 5662 75a0  ..V.a.?..>O.Vbu.
-00002370: 3d10 c215 b3c0 48e7 6b33 e042 c51c aa50  =.....H.k3.B...P
-00002380: 16d3 b02b e02e cdd4 0e88 16b8 0886 c710  ...+............
-00002390: 5470 d16d fe0b 72a8 ffdb 9cb3 3c4c 5ac3  Tp.m..r.....<LZ.
-000023a0: 70a9 f669 8404 85f3 48c5 8290 3d28 4b26  p..i....H...=(K&
-000023b0: fa5e c3ac 9c9f 5d96 25cb 1999 882a a82b  .^....].%....*.+
-000023c0: 33ab 769f 1c12 d6d3 35b0 aecf f600 c510  3.v.....5.......
-000023d0: eaa6 9ae4 65c0 e04e c69f fb3b cfa0 7ea4  ....e..N...;..~.
-000023e0: 9b9c 7f6b e763 9379 d9f6 4077 07b6 c5b2  ...k.c.y..@w....
-000023f0: f467 ec45 aa85 a25f 380a 1ade b3cf f454  .g.E..._8......T
-00002400: b372 f08a 837d c9a3 d656 ac85 1d57 6a67  .r...}...V...Wjg
-00002410: 3e6a 33b8 5b42 fa0f 9c7f 5484 8c98 30d6  >j3.[B....T...0.
-00002420: 076a 8fef 436d 45f0 96c3 b657 08a2 fa82  .j..CmE....W....
-00002430: 6d3c 902e 90b6 3cf6 a171 b28b 3698 342b  m<....<..q..6.4+
-00002440: dbb0 e4dd edb9 b751 70f1 9d77 ba33 b990  .......Qp..w.3..
-00002450: a56f d2e9 2e69 ec59 73e6 8a73 72f1 d5dd  .o...i.Ys..sr...
-00002460: e772 c6ce 2dec d8ba d8e9 7a4c 0d49 7b32  .r..-.....zL.I{2
-00002470: 4575 7b34 9d6d 8c63 cceb b6e2 5b30 debf  Eu{4.m.c....[0..
-00002480: 038e de86 3709 63a6 a47d 8370 176e 1261  ....7.c..}.p.n.a
-00002490: cab0 af27 20f9 ad73 0de9 e6df 0000 00ff  ...' ..s........
-000024a0: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
-000024b0: 001e 63f5 13bc 0200 00d1 0600 000d 0000  ..c.............
-000024c0: 0078 6c2f 7374 796c 6573 2e78 6d6c b455  .xl/styles.xml.U
-000024d0: 5b6b db30 147e 1fec 3f08 bdbb b29d 384b  [k.0.~..?.....8K
-000024e0: 82ed b234 3514 ba31 6807 7b55 6c39 11d5  ...45..1h.{Ul9..
-000024f0: 2548 4ae6 6cec bff7 c876 1287 8e6d b4ec  %HJ.l....v...m..
-00002500: 253e 3a3a face 77ae 49af 1b29 d09e 19cb  %>::..w.I..)....
-00002510: b5ca 7074 1562 c454 a92b aed6 19fe fa58  ..pt.b.T.+.....X
-00002520: 0453 8cac a3aa a242 2b96 e103 b3f8 3a7f  .S.....B+.....:.
-00002530: ff2e b5ee 20d8 c386 3187 0042 d90c 6f9c  .... ...1..B..o.
-00002540: dbce 09b1 e586 496a aff4 9629 b8a9 b591  ......Ij...)....
-00002550: d4c1 d1ac 89dd 1a46 2beb 1f49 41e2 309c  .......F+..IA.0.
-00002560: 1049 b9c2 1dc2 5c96 ff02 22a9 79da 6d83  .I....\...".y.m.
-00002570: 52cb 2d75 7cc5 0577 8716 0b23 59ce efd6  R.-u|..w...#Y...
-00002580: 4a1b ba12 40b5 89c6 b444 4d34 3131 6acc  J...@....DM411j.
-00002590: d149 ab7d e147 f2d2 68ab 6b77 05b8 44d7  .I.}.G..h.kw..D.
-000025a0: 352f d94b ba33 3223 b43c 2301 f2eb 90a2  5/.K.32#.<#.....
-000025b0: 8484 f145 ec8d 7925 d298 18b6 e7be 7c38  ...E..y%......|8
-000025c0: 4f6b ad9c 45a5 de29 97e1 1888 fa14 cc9f  Ok..E..)........
-000025d0: 94fe ae0a 7f05 15ee adf2 d4fe 407b 2a40  ............@{*@
-000025e0: 1361 92a7 a516 da20 07a5 83cc b51a 4525  .a..... ......E%
-000025f0: eb2c 6ea8 e02b c3bd 594d 2517 874e 1db7  .,n..+..YM%..N..
-00002600: ef36 d458 e881 162a 1e4d bdae ed80 fead  .6.X...*.M......
-00002610: e450 0faf 249e 5bc7 f0ec bb35 ff3f 8e5a  .P..$.[....5.?.Z
-00002620: 7f16 1c72 2106 29e9 1479 0abd e398 5105  ...r!.)..y....Q.
-00002630: dca2 5e7e 3c6c 2176 056d def1 85ab bf5a  ..^~<l!v.m.....Z
-00002640: af0d 3d44 7132 7840 5a87 79ba d2a6 82b1  ..=Dq2x@Z.y.....
-00002650: 3a16 c3e7 bd53 e5a9 60b5 838c 18be def8  :....S..`.......
-00002660: afd3 5bf8 5d69 e7a0 f5f2 b4e2 74ad 1515  ..[.]i......t...
-00002670: 3e67 c717 bd00 e194 4c88 073f 7adf ea0b  >g......L..?z...
-00002680: eca6 466a 270b e9ee aa0c c310 fb6c 1f45  ..Fj'........l.E
-00002690: 08a4 173b bcee e0f1 8768 1df6 9b61 5153  ...;.....h...aQS
-000026a0: 5fe2 03e2 80f6 05e9 937b e47b 20c3 9ffd  _........{.{ ...
-000026b0: ae10 ea00 8ddb 83a0 d58e 0bc7 d56f 2803  .............o(.
-000026c0: 6ad5 9c93 10fa 1a38 3ff9 6d7a 4e7e 2017  j......8?.mzN~ .
-000026d0: 15ab e94e b8c7 d365 86cf f227 56f1 9d9c  ...N...e...'V...
-000026e0: 9dac bef0 bd76 2d44 86cf f2bd af55 34f1  .....v-D.....U4.
-000026f0: 3e58 e3ee 2d74 327c d1ce f00c ffbc 5d7c  >X..-t2|......]|
-00002700: 982d 6f8b 3898 868b 6930 1eb1 2498 258b  .-o.8...i0..$.%.
-00002710: 6590 8c6f 16cb 6531 0be3 f0e6 d760 ffbc  e..o..e1.....`..
-00002720: 61fb b4eb 324f 61ae e756 c08e 327d b07d  a...2Oa..V..2}.}
-00002730: 880f 675d 8607 878e 7edb a540 7bc8 7d16  ..g]....~..@{.}.
-00002740: 4fc2 8f49 1406 c528 8c82 f184 4e83 e964  O..I...(....N..d
-00002750: 9404 4512 c5cb c978 719b 14c9 807b f2ca  ..E....xq....{..
-00002760: 2d15 9228 eaf6 9d27 9fcc 1d97 4c70 75ac  -..(...'....Lpu.
-00002770: d5b1 4243 2d14 098e 7f08 821c 2b41 ceff  ..BC-.......+A..
-00002780: 45f9 3300 0000 ffff 0300 504b 0304 1400  E.3.......PK....
-00002790: 0600 0800 0000 2100 45c8 2668 7f10 0000  ......!.E.&h....
-000027a0: 4e39 0000 1400 0000 786c 2f73 6861 7265  N9......xl/share
-000027b0: 6453 7472 696e 6773 2e78 6d6c ec9b 5d6f  dStrings.xml..]o
-000027c0: 5bc7 1545 df0b f43f 087c 6f64 d971 9a06  [..E...?.|od.q..
-000027d0: b202 9668 85a0 7d30 6ca6 7974 599a b189  ...h..}0l.ytY...
-000027e0: 48a4 4ad2 469c 5fdf b3d6 9e2b a59c 2bc4  H.J.F._....+..+.
-000027f0: 79a8 e114 9625 999c 7bef cc99 f3b1 f73e  y....%..{......>
-00002800: 23e9 fceb 1faf af4e deae 76fb f576 f364  #......N..v..v.d
-00002810: 72f6 d983 c9c9 6ab3 dcbe 5c6f 5e3d 997c  r.....j...\o^=.|
-00002820: 3bff eb1f be9c 9cec 0f8b cdcb c5d5 76b3  ;.............v.
-00002830: 7a32 79b7 da4f bebe f8fd efce f7fb c349  z2y..O.........I
-00002840: 3dbb d93f 99bc 3e1c 6ebe 3a3d dd2f 5faf  =..?..>.n.:=./_.
-00002850: ae17 fbcf b637 ab4d 5df9 7ebb bb5e 1cea  .....7.M].~..^..
-00002860: edee d5e9 fe66 b75a bcdc bf5e ad0e d757  .....f.Z...^...W
-00002870: a70f 1f3c f8e2 f47a b1de 4c4e 96db 379b  ...<...z..LN..7.
-00002880: c393 c9e3 879f 4f4e de6c d6ff 7eb3 9a65  ......ON.l..~..e
-00002890: e4ec ec6c 7271 be5f 5f9c 1f2e 96db eb9b  ...lrq.__.......
-000028a0: 5a7c 7338 3f3d 5c9c 9f32 980b 6f57 cbc3  Z|s8?=\..2..oW..
-000028b0: 76f7 e2f0 ee66 757c 69bf aab9 36cb 6e7c  v....fu|i...6.n|
-000028c0: 3ebf 9c5e 4ee7 b3d9 3c1f b3f9 e5ac fecd  >..^N...<.......
-000028d0: a735 562f f9ac afe9 74ca 171f b359 7dd6  .5V/....t....Y}.
-000028e0: 282f eac6 cb79 7dd6 2d7c d538 534d 6bc2  (/...y}.-|.8SMk.
-000028f0: 76c3 7456 b3f0 5197 6a98 696b 4ae6 e461  v.tV..Q.j.ikJ..a
-00002900: eff3 3f67 ab25 b95a d7f8 9cd6 ccf5 ad1e  ..?g.%.Z........
-00002910: e465 7dd5 4b17 e7d9 7ad2 a9bd 437b 3088  .e}.K...z...C{0.
-00002920: e76b c19a 5ebb d982 f369 aacb baa1 5a97  .k..^....i....Z.
-00002930: 3765 6acd 53b7 d73a b522 b3b0 95da 423d  7ej.S..:."....B=
-00002940: cf0a dec1 d2d9 17f6 d7dc d934 f7d6 dc65  ...........4...e
-00002950: 45bd f039 e629 03eb 5f19 ca37 a762 1926  E..9.).._..7.b.&
-00002960: 2a43 b8e6 bb78 bc0d e1eb b8cb e15a a4d6  *C...x.......Z..
-00002970: a83b f551 f31a 11ca ea35 915e c49f 3893  .;.Q.....5.^..8.
-00002980: 0030 c236 58a8 5e0e 4ead a56a 5c3b 3087  .0.6X.^.N..j\;0.
-00002990: 0fa2 5793 1331 a25b 3bc3 b5fa 287b c777  ..W..1.[;...({.w
-000029a0: 5889 ffca 0b1a c6d4 5363 88a1 e443 59dc  X.......Sc...CY.
-000029b0: 2664 79b6 5b13 39fb 71d2 b564 6a31 e151  &dy.[.9.q..dj1.Q
-000029c0: 026c 2871 123e 6463 eda5 9bc0 6126 a37b  .l(q.>dc....a&.{
-000029d0: f20a f610 3276 3b7c 1908 b68a 0144 b326  ....2v;|.....D.&
-000029e0: aadb 2a05 58c2 ed92 74f3 638b b2bf ae38  ..*.X...t.c....8
-000029f0: f6d3 e93f 8e07 ff55 25fa c3d9 f1a8 9949  ...?...U%......I
-00002a00: 31e0 3ffc 686c c8d0 cbd1 091e 8e8e 7e3e  1.?.hl........~>
-00002a10: 3afa b8f3 1f09 ea32 adfa 0cf6 c8ae 70c0  :......2......p.
-00002a20: e56c ccfd 8440 7724 f204 d0f0 5393 563d  .l...@w$....S.V=
-00002a30: 2961 addf 5d31 8d1d ae8b d402 b54a 1191  )a..]1.......J..
-00002a40: 2edc 4fc4 529d 2989 ca24 f396 7756 4383  ..O.R.)..$..wVC.
-00002a50: 85dc cb25 f229 a861 5e05 3b88 73f2 dd9a  ...%.).a^.;.s...
-00002a60: c5a3 e6bd 00c0 4513 c1ec a122 bc4a c28b  ......E....".J..
-00002a70: 2700 0365 4ab2 9685 1480 3589 69c2 05f7  '..eJ.....5.i...
-00002a80: 2775 c910 07ad 1621 a2ac 2165 0434 f21c  'u.....!..!e.4..
-00002a90: 2f63 3489 0cc0 0475 9810 e764 bfc6 1aef  /c4....u...d....
-00002aa0: 0968 8ef1 2886 9985 96ad e805 7a9a 96c1  .h..(.......z...
-00002ab0: 3f2d a1f8 ac12 5c19 88d1 74c2 a0e1 6583  ?-....\...t...e.
-00002ac0: 58a9 3162 1368 da70 9517 2c4d a969 626c  X.1b.h.p..,M.ibl
-00002ad0: 0f74 e489 86d0 6c5e bf97 0d79 cdad 3cc6  .t....l^...y..<.
-00002ae0: 3023 6580 5798 07c8 c202 033b 603e 352a  0#e.W......;`>5*
-00002af0: 9a27 e206 37b0 4671 e2ba d45b 5ee9 82c1  .'..7.Fq...[^...
-00002b00: 45d9 8a88 4a64 a871 1c68 5881 2716 0738  E...Jd.q.hX.'..8
-00002b10: 930f a660 4329 ee13 8aad 6a5d 4cca 9469  ...`C)....j]L..i
-00002b20: 8403 e04c 3601 70be 3338 c237 b81f 14ca  ...L6.p.38.7....
-00002b30: be80 4842 e0c3 c2bc efd8 bc19 97ac 3647  ..HB..........6G
-00002b40: d97e 5c2b 8061 01f9 0d96 9248 e605 3e4b  .~\+.a.....H..>K
-00002b50: cc4d 3478 c6a2 00f5 0052 93b7 5e67 77b8  .M4x.....R..^gw.
-00002b60: 99ea 2082 c225 f79a 1024 0b1f cc0e 6a8d  .. ..%...$....j.
-00002b70: 62c0 1723 454c 7828 3fc1 c0d4 0177 204b  b..#ELx(?....w K
-00002b80: 129d 84c0 be96 cb58 e7bb 3624 2583 88ac  .......X..6$%...
-00002b90: 7ec7 f471 0b91 3714 e688 a563 9660 9e6e  ~..q..7....c.`.n
-00002ba0: a186 82d9 417d dd02 ebba 11c9 9efd 58b1  ....A}........X.
-00002bb0: a3fb f9e3 f168 3828 8822 7d19 0022 6899  .....h8(."}.."h.
-00002bc0: 88e5 ac4d 9610 d4bc 0492 8867 83b3 7248  ...M.......g..rH
-00002bd0: 87ec 6435 2193 f388 0966 c94e 952e a3b6  ..d5!....f.N....
-00002be0: 3d7a 7133 0ecf 75a1 037e 762e 9bb2 5760  =zq3..u..~v...W`
-00002bf0: 9048 021a ae7b 3cff 6ef5 eacd d562 3702  .H...{<.n....b7.
-00002c00: e8ef c91b 8f3a bfdd b37e 30cb 42b3 cae0  .....:...~0.B...
-00002c10: c86e d99e 1ba0 7844 9a6c a99c 4aa0 2ded  .n....xD.l..J.-.
-00002c20: d908 9530 6fc8 cfc2 0b94 98eb bfe0 ea04  ...0o...........
-00002c30: d9ef 8275 4303 6178 5004 5108 945e 504e  ...uC.axP.Q..^PN
-00002c40: ac67 5ef0 43d2 b7d2 44fb 60a7 624c 999a  .g^.C...D.`.bL..
-00002c50: cca1 0e05 1883 4e58 0283 569b fb13 5ecc  ......NX..V...^.
-00002c60: 3bb5 14c1 4c35 2a8f d809 d359 9f94 34a8  ;...L5*....Y..4.
-00002c70: ae8f ea45 2702 2c0b 35a9 bb01 2b94 4c98  ...E'.,.5...+.L.
-00002c80: 2a5e 3911 ca29 e080 eb82 6bee 276e 8b5c  *^9..)....k.'n.\
-00002c90: 0364 5854 f1ea ae28 bc4c 48c5 8aa2 c29c  .dXT...(.LH.....
-00002ca0: 5345 aec9 6cae 3940 2b98 a5fc a548 5237  SE..l.9@+....HR7
-00002cb0: 02bb b4e1 3c11 bd92 2755 df7c 2918 374d  ....<...'U.|).7M
-00002cc0: 290d 1800 2a5c 691c 35dd 405b c92b 448a  )...*\i.5.@[.+D.
-00002cd0: c01a 292d 5365 eab6 844c 5ec7 8ce8 7d08  ..)-Se...L^...}.
-00002ce0: d4a2 516c 66ef 8a57 b844 9d19 8a95 1f0d  ..Qlf..W.D......
-00002cf0: 8b2a 4d99 1a1f 2913 2c6c 145f 7057 ad41  .*M...).,l._pW.A
-00002d00: 888c 3a09 23be b2cb 0087 a9ad 5c90 6fc9  ..:.#.......\.o.
-00002d10: 8148 e4a0 7a34 7052 ce48 2b44 c13d f5a7  .H..z4pR.H+D.=..
-00002d20: 1c60 5ca4 f7b8 4ba4 0da7 41e2 6c25 b206  .`\...K...A.l%..
-00002d30: a314 564d 1d80 10e4 8fca 291d 4e13 4e41  ..VM......).N.NA
-00002d40: ceb0 80c4 3b0e 4d5f f6e5 1f55 1422 6a84  ....;.M_...U."j.
-00002d50: 9e1d 8bf8 2ded a52a bc2d aecb 6469 8c30  ....-..*.-..di.0
-00002d60: 474a 942a 4244 e41d bbb8 d3cb b843 7e33  GJ.*BD.......C~3
-00002d70: 0303 f228 015c a2d2 0131 a462 16f5 3304  ...(.\...1.b..3.
-00002d80: 1279 d172 3933 524e 2a29 f57e c41d c945  .y.r93RN*).~...E
-00002d90: 6d59 60a3 9af5 aada daf5 dbf5 6e71 d513  mY`.........nq..
-00002da0: 8792 530a d7b5 1060 b038 e9a5 b06a 5983  ..S....`.8...jY.
-00002db0: 8031 962a 57d5 4c94 4f1a a4d4 b9c1 632a  .1.*W.L.O.....c*
-00002dc0: c54e 8495 e4cc 264d 24f2 33b5 8770 5056  .N....&M$.3..pPV
-00002dd0: 0a1e f80d 7fa8 c810 3528 3b65 20d2 a451  ........5(;e ..Q
-00002de0: 2603 6cd4 ffc9 5e55 185e 81ac 511a b015  &.l...^U.^..Q...
-00002df0: 8847 e58a 021d ee66 05f6 a9a6 5106 48b7  .G.....f....Q.H.
-00002e00: 200d 8361 bbff 42f3 a65e 2827 ac0e 05aa   ..a..B..^('....
-00002e10: 41e4 2fc1 c1ae a9ae 2a2a b0c5 b256 6f91  A./.....**...Vo.
-00002e20: babe d5bd 430d 6b3e 8813 2d22 2f07 d5b8  ....C.k>..-"/...
-00002e30: d94c 21eb d850 97d1 0d79 1471 3623 f600  .L!..P...y.q6#..
-00002e40: d4c0 20e4 524a 14b7 0e61 26a1 9301 2981  .. .RJ...a&...).
-00002e50: 3893 823c 628e da3a f200 f400 23f9 0a8f  8..<b..:....#...
-00002e60: 7460 cd5e 1588 0165 2b41 4359 0d00 615a  t`.^...e+ACY..aZ
-00002e70: f657 ffba a4c3 c5d0 50d0 2742 394e 6555  .W......P.'B9NeU
-00002e80: 864d 0b11 8ca4 8b2b d404 51a1 b610 b937  .M.....+..Q....7
-00002e90: a563 c129 0e23 d994 7282 5af6 140f 35bb  .c.).#..r.Z...5.
-00002ea0: c80d 30d8 5c86 e382 6da0 9465 68d9 9b92  ..0.\...m..eh...
-00002eb0: 1647 2be7 2486 7285 117b 1840 3902 5cbd  .G+.$.r..{.@9.\.
-00002ec0: 36c0 6114 64aa 3932 95b5 e446 a36d bf11  6.a.d.92...F.m..
-00002ed0: cc57 f44a 33c9 65d1 911a d27d e616 56f1  .W.J3.e....}..V.
-00002ee0: 1648 9179 8927 6e0f d50a 1e0d 33a9 20f1  .H.y.'n.....3. .
-00002ef0: 1107 3509 d12c c47c 2392 75a8 64f2 00a7  ..5..,.|#.u.d...
-00002f00: c6e3 6a59 0ad2 a269 045a 4b86 bf45 3af6  ..jY...i.ZK..E:.
-00002f10: 0cae b5cd 209e 62a8 ba2d bb0f 5748 cc03  .... .b..-..WH..
-00002f20: 2c6b ef20 ebba 6448 7a0a eeb8 93d4 1081  ,k. ..dHz.......
-00002f30: 1c67 3b44 df96 ca4c 306e 6953 d324 f95d  .g;D...L0niS.$.]
-00002f40: ed98 acc8 9ed8 560a 1cb7 8147 ed53 b735  ......V....G.S.5
-00002f50: 298c 0bd2 fc99 f362 9d5a c372 e52d 58ab  )......b.Z.r.-X.
-00002f60: 44b3 1c94 e6ce 8330 6ad5 3224 d050 b24d  D......0j.2$.P.M
-00002f70: 320c 6c24 aaa1 37fa 6313 0595 3b8e 2e32  2.l$..7.c...;..2
-00002f80: 44c4 15a2 91e9 9a7c 0c8e 1828 bb1f 1237  D......|...(...7
-00002f90: 5148 ac02 65c1 4f1e a47e 305c f920 8a7a  QH..e.O..~0\. .z
-00002fa0: 7702 6e79 855a 2c33 6e34 cf40 33fa 1295  w.ny.Z,3n4.@3...
-00002fb0: 06fe b3b4 2c94 0625 66a1 190a 1324 29e5  ....,..%f....$).
-00002fc0: ab2c 497e a641 8b6b 30a5 5d91 c279 0201  .,I~.A.k0.]..y..
-00002fd0: 49b1 5272 5e1d 122e f378 837d 9e6a 4928  I.Rr^....x.}.jI(
-00002fe0: 01a5 a10e 1142 1a94 af23 b222 bd12 63af  .....B...#."..c.
-00002ff0: 85a0 4c9b 7083 394a 5eab ae1b d2c2 bda4  ..L.p.9J^.......
-00003000: 6f5a 2fc1 8e97 1404 5904 84ea c556 d1be  oZ/.....Y....V..
-00003010: 4d9d 04d3 92df 7c27 1340 132b 43af 0805  M.....|'.@.+C...
-00003020: c15a d95a d4e9 4888 3d50 c4d1 03c1 b2e4  .Z.Z..H.=P......
-00003030: 02db 25e9 b207 ae13 4f6b 2e0e 6c48 222c  ..%.....Ok..lH",
-00003040: a467 f2b4 26a8 2928 341f 0721 308f 9558  .g..&.)(4..!0..X
-00003050: 7144 01b1 92ce 57ed 9af4 c44d b461 ed7a  qD....W....M.a.z
-00003060: f36b da26 524f 4b7a da15 c0a3 52f4 58c7  .k.&ROKz....R.X.
-00003070: 6964 2cbc d03d eab1 e19f baee 14ad d008  id,..=..........
-00003080: 159f 910b 388b b882 0a83 3811 b3c9 a132  ....8.....8....2
-00003090: 0dfc b2aa c6fc dfb5 7866 6f40 422f 0e49  ........xfo@B/.I
-000030a0: 6369 0493 2308 0228 b84d 9a90 b57f d3f2  ci..#..(.M......
-000030b0: 2207 b50f 3a97 270f c928 f035 0e55 c5c9  "...:.'..(.5.U..
-000030c0: 7004 800a 17bc 92db 2ae4 302a bc61 f9dc  p.......*.0*.a..
-000030d0: 7374 70d6 9f0f 08cf d4a3 bd9b d0e8 6bca  stp...........k.
-000030e0: ae1f f4b0 835b 09d6 d044 c21a 0aed 324c  .....[...D....2L
-000030f0: e0d0 480c a5c0 2cf7 f6dd ee19 25c7 ed21  ..H...,.....%..!
-00003100: 0660 9e1a 88e5 de97 3924 53b5 2629 68f6  .`......9$S.&)h.
-00003110: c9a5 1a65 f1a8 95d5 ebad 4b41 95a6 1d83  ...e......KA....
-00003120: bec0 338b 376f 48d7 a673 6c41 ed95 3d1e  ..3.7oH..slA..=.
-00003130: 318f 9542 712b 54e8 f6cd 77d6 c356 941a  1..Bq+T...w..V..
-00003140: 1b8c fccb 86d4 7411 dbcc d900 cf8a 0e8b  ......t.........
-00003150: 2afe 7c94 8271 23b1 5fb1 c294 127e f421  *.|..q#._....~.!
-00003160: 6a50 092b c3df 765e 546c fa35 c9c3 c6c6  jP.+..v^Tl.5....
-00003170: 6624 6ad0 3049 2976 bd52 7b33 a6f6 8f0c  f$j.0I)v.R{3....
-00003180: a51a 3d9a b007 6490 6714 d16a 5f01 45fa  ..=...d.g..j_.E.
-00003190: e50a 4e8b 4410 72c3 ed7a 12ce 3182 62ba  ..N.D.r..z..1.b.
-000031a0: b234 92b8 3da1 9024 7171 946a 4409 47ba  .4..=..$qq.jD.G.
-000031b0: 8470 72e6 8101 8e41 8018 2675 0e46 8a30  .pr....A..&u.F.0
-000031c0: 797c 6894 2000 1213 be50 4110 666c 8072  y|h. ....PA.fl.r
-000031d0: e8cd 10f0 ee9b 195b 8534 ea1f 7a24 5bb8  .......[.4..z$[.
-000031e0: 2811 54a8 1fc9 c13c 710b e414 9702 3ff0  (.T....<q.....?.
-000031f0: 155c 0f99 db97 9883 b2a5 eee0 2ec2 0689  .\..............
-00003200: 2822 0862 48cf 8e49 5235 a165 103b 26c9  (".bH..IR5.e.;&.
-00003210: 82ea c07e 44a4 cd68 a462 f635 b07c 5a1d  ...~D..h.b.5.|Z.
-00003220: b34e b510 c943 4d8d 1fc3 9e75 0783 3c26  .N...CM....u..<&
-00003230: 85b6 c204 4c5b 228b abec 49ad 1b56 63f9  ....L["...I..Vc.
-00003240: 21d7 c8fa f493 b015 b70d fc95 da95 dcc1  !...............
-00003250: 7b33 2a04 9e30 45b3 5bfb 9601 b247 4d42  {3*..0E.[....GMB
-00003260: 1093 a046 58a6 3057 70a8 2b93 5011 4182  ...FX.0Wp.+.P.A.
-00003270: 8444 2c0e a5d7 34fd bc82 3b6d 2ca8 71c9  .D,...4...;m,.q.
-00003280: 9c1a e5b3 bdd1 87c2 807d 36bb 42e2 84cf  .........}6.B...
-00003290: 2431 f5be 8f23 286c 4794 9e24 9494 4420  $1...#(lG..$..D 
-000032a0: d50d 560f 7e52 ac02 7ffa 0d3f 780f 65c1  ..V.~R.....?x.e.
-000032b0: 35df c5e3 6d08 5f37 a88b 2cb4 723d 5f13  5...m._7..,.r=_.
-000032c0: 6031 a45d 3073 5047 490b c086 2146 3448  `1.]0sPGI...!F4H
-000032d0: f5e9 ddc2 0e08 e4cc 51ca 4941 0a4b 3567  ........Q.IA.K5g
-000032e0: 5cd4 340c b89f 5677 9670 c85b fba3 ac88  \.4...Vw.p.[....
-000032f0: 2fc5 4336 7aea e7be 0938 337a 5030 1d3f  /.C6z....83zP0.?
-00003300: f339 ebcf 7cd3 b692 56e4 9a9d 7b03 10b0  .9..|...V...{...
-00003310: 0738 346b 02aa c34b 4137 d9e1 4d20 4350  .84k...KA7..M CP
-00003320: d8a2 6617 0913 d845 4126 2d4c f0db 4a4e  ..f....EA&-L..JN
-00003330: eee2 0523 791b 1d77 6a42 d36b 846b 6cc1  ...#y..wjB.k.kl.
-00003340: e363 a320 2829 d153 10fa 523d c22e 0254  .c. ().S..R=...T
-00003350: 4458 6a26 fbd2 a708 0391 b516 0212 57a8  DXj&..........W.
-00003360: 327a dca3 75cd 1b30 6490 2232 3a8c d5ba  2z..u..0d."2:...
-00003370: 3e32 88dc 22b9 d229 8444 f11a 836e 9c1c  >2.."..).D...n..
-00003380: be53 fd99 dbf4 0d32 b51c 058f cc52 759a  .S.....2.....Ru.
-00003390: 00c3 9454 47c8 c6bb 8336 70a6 c812 7cb5  ...TG....6p...|.
-000033a0: 5749 6a61 34c6 1c8b 94fd 72e4 27cf 12b6  WIja4.....r.'...
-000033b0: 8081 8f43 5ad6 b572 e517 046f ca5f fe49  ...CZ..r...o._.I
-000033c0: 79e3 7209 2d00 a960 1081 2839 d1c4 aa80  y.r.-..`..(9....
-000033d0: c9dc 562a 5694 f2a5 49f6 b348 136d e398  ..V*V...I..H.m..
-000033e0: 8293 735c d47e cc6e 4ede 53e1 dca3 e23b  ..s\.~.nN.S....;
-000033f0: f59a 660e 831b aefe 8f4d ee7f 3023 b603  ..f......M..0#..
-00003400: 5666 3ce0 6e5f 6423 f051 4ba1 2015 4524  Vf<.n_d#.QK. .E$
-00003410: e051 3a8a 1882 09ad dba6 58e8 69b4 1d06  .Q:.......X.i...
-00003420: 8784 616e 4634 92c5 c2be 0a23 650f b588  ..anF4.....#e...
-00003430: 9de4 7ff2 83ba 32f5 adb0 8855 8198 c75a  ......2....U...Z
-00003440: e678 9861 b953 d121 66db 44bb 700d 025d  .x.a.S.!f.D.p..]
-00003450: 227b 6fcb c35a 94e9 949b 7280 aa3d 6420  "{o..Z....r..=d 
-00003460: 0092 7af5 2225 2683 2987 f440 0433 40ad  ..z."%&.)..@.3@.
-00003470: d191 fc96 b330 c1a4 7654 0825 b9e1 e352  .....0..vT.%...R
-00003480: 1d22 3c7e fe04 f532 f5c7 07f5 2ae4 34e6  ."<~...2....*.4.
-00003490: 9e84 00e7 5483 1f16 cf31 a87c ff66 b33c  ....T....1.|.f.<
-000034a0: d4ef 111e 8faf 7eac 5fff dbf3 1b86 5dcf  ......~._.....].
-000034b0: da9f 5e23 0abb db72 3cf1 9e74 00fc 4b7c  ..^#...r<..t..K|
-000034c0: 7e0f 1580 68e0 b53a 4f7e 489f 273b 2a35  ~...h..:O~H.';*5
-000034d0: 4479 1514 c425 3e5b 77a2 0c3a d43a 4332  Dy...%>[w..:.:C2
-000034e0: 51b4 76cd 760a e6af 2752 0cdb 7b33 95e7  Q.v.v...'R..{3..
-000034f0: 474a ca9f bd54 df23 cf32 73d3 06ea 9aaa  GJ...T.#.2s.....
-00003500: d7ee 209f 4d58 e080 8b88 643f 2421 c93b  .. .MX....d?$!.;
-00003510: 6946 c263 8a5f 2a1d 40a8 9492 c7e5 388c  iF.c._*.@.....8.
-00003520: 6b3f a902 1fa2 13c4 0740 2ee7 28c2 97dc  k?.......@..(...
-00003530: 2b6b 367d ece3 dcc2 f277 7a37 c250 140a  +k6}.....wz7.P..
-00003540: f8e2 6865 a4a2 5502 f682 3daf 6d1d 28d8  ..he..U...=.m.(.
-00003550: 04aa f86b f395 a1d6 61da ab29 ecf8 268a  ...k....a..)..&.
-00003560: 0b7d d808 7af2 5830 7908 2216 a96f 3cd6  .}..z.X0y."..o<.
-00003570: a00d 27ee b57f a732 5541 73e4 754e 9c08  ..'....2UAs.uN..
-00003580: 3f81 b5e0 9cce 373c 8e8f 6846 f59f fa2e  ?.....7<..hF....
-00003590: 6d16 8e84 3882 e711 999e 3ac4 c9c8 1fae  m...8.....:.....
-000035a0: a1b1 ecb1 3d92 70be 3471 2694 9d53 d886  ....=.p.4q&..S..
-000035b0: 67ed 3388 835e 4b32 d8f9 dbda 670f d16d  g.3..^K2....g..m
-000035c0: 4ab1 bbce 0abe 8b3d 5286 ca3b 4d98 8292  J......=R..;M...
-000035d0: 5a55 a9b9 8b74 aa6c 8b6c ee7f 4685 67e4  ZU...t.l.l..F.g.
-000035e0: 4d28 4529 9d8d d814 ab8c 2277 d3a6 6089  M(E)......"w..`.
-000035f0: 8194 2075 161d d1d0 801a 8996 d6ce 069d  .. u............
-00003600: 95b1 6d05 32be f5ce b51a 7bf5 1d76 d5d2  ..m.2.....{..v..
-00003610: 1403 c732 789c 5796 f960 c6c8 8fa8 5a79  ...2x.W..`....Zy
-00003620: a77d 4476 b3ba f37a 36df 4a33 836e fe4e  .}Dv...z6.J3.n.N
-00003630: ea52 4eb8 4d21 6dc3 4f99 3007 31e3 7fd0  .RN.M!m.O.0.1...
-00003640: 2de0 61d3 1661 6e31 21c7 ed34 657e ed4e  -.a..an1!..4e~.N
-00003650: 8d65 7d96 e54a 3afe 566f 9951 f56d 162a  .e}..J:.Vo.Q.m.*
-00003660: b76c a7e6 fdaf 9cc4 31d1 2622 4404 7d16  .l......1.&"D.}.
-00003670: 7dff 735e 2618 f97d 1603 a7fe 1509 5540  }.s^&..}......U@
-00003680: 2904 4bd3 a899 9be6 8218 a56f 1ade f73f  ).K........o...?
-00003690: 28a4 a119 1f0d 6974 d7ee 8e37 d230 126c  (.....it...7.0.l
-000036a0: 5b3a 85f4 07d0 c223 67c8 821b 7d93 dd4a  [:.....#g...}..J
-000036b0: 2412 410a 3bd8 4b29 a06c 4a3c 8723 53d2  $.A.;.K).lJ<.#S.
-000036c0: 8aa2 bbe8 ba38 7920 91eb 31ab 3189 236c  .....8y ..1.1.#l
-000036d0: 0d9d 731a 5672 db0a b66b 6cca dbc6 5074  ..s.Vr...kl...Pt
-000036e0: 975e 831d 2286 0db4 a92a 9a0b ea12 c0af  .^.."....*......
-000036f0: 94be 0a40 7047 2441 e446 5c0a e302 8a12  ...@pG$A.F\.....
-00003700: 59e5 1b2a 04dc 14cc 6e11 3ce7 36f2 06ec  Y..*....n.<.6...
-00003710: fd78 0f13 0910 7066 0913 376a d65e cde8  .x....pf..7j.^..
-00003720: 28f5 55d4 c1cf e6f5 d433 3c28 73c8 3502  (.U......3<(s.5.
-00003730: 541e 273b 3dc7 b277 0c5f e24a 01d1 5c10  T.';=..w._.J..\.
-00003740: 623d f7f9 2087 8969 f1d5 ff9f da1a c93c  b=.. ..i.......<
-00003750: f405 5281 e136 801c 4079 28f2 610f 5355  ..R..6..@y(.a.SU
-00003760: 839f da1a 51e5 633b c142 8380 d1d8 c557  ....Q.c;.B.....W
-00003770: df8c 84fd 0304 77c7 50f7 7423 e81b 3155  ......w.P.t#..1U
-00003780: 1d06 b04b dab5 c6f1 0337 dfce 5e6c 77eb  ...K.....7..^lw.
-00003790: e3e1 c7ff fc66 feec 78f0 d1d8 e0df b63f  .....f..x......?
-000037a0: 2d7e 7871 df9f 345d ef36 8bae 7780 6994  -~xq..4].6..w.i.
-000037b0: bd9e d161 6ac7 c751 88f7 7eef a61c f103  ...aj..Q..~.....
-000037c0: 9d4e c7aa f24b ef5c ba9d 5e98 e844 f8ed  .N...K.\..^..D..
-000037d0: ffa1 63ab 408c 44f9 ef63 511e 197c f6bc  ..c.@.D..cQ..|..
-000037e0: fb9b 9ca7 cfbf 3976 e4b3 677f 391e 5a3e  ......9v..g.9.Z>
-000037f0: 7dda 378f abdd f57a b3a8 3f8f ebe2 d8fd  }.7....z..?.....
-00003800: 8afa d3ed d5bb ae41 78be b8e9 d6fe f37e  .......Ax......~
-00003810: fd5d 3738 dd2f bbb1 c36e b1d9 2f77 eb9b  .]78./...n../w..
-00003820: b1e3 0078 3927 ad4a 26aa e8b7 9f00 a7f5  ...x9'.J&.......
-00003830: f790 17ff 0100 00ff ff03 0050 4b03 0414  ...........PK...
-00003840: 0006 0008 0000 0021 00eb 239e 3242 0100  .......!..#.2B..
-00003850: 0051 0200 0011 0008 0164 6f63 5072 6f70  .Q.......docProp
-00003860: 732f 636f 7265 2e78 6d6c 20a2 0401 28a0  s/core.xml ...(.
-00003870: 0001 0000 0000 0000 0000 0000 0000 0000  ................
+00000b10: 0000 0000 00bc 93cf 6ac3 300c c6ef 83bd  ........j.0.....
+00000b20: 83d1 7d71 926e 6594 3abd 8c41 af5b f700  ..}q.ne.:..A.[..
+00000b30: 2651 e2d0 c436 96f6 276f 3f93 43ba 40c9  &Q...6..'o?.C.@.
+00000b40: 2ea1 1783 24fc 7d3f d0a7 fde1 a7ef c417  ....$.}?........
+00000b50: 066a 9d55 9025 2908 b4a5 ab5a db28 f838  .j.U.%)....Z.(.8
+00000b60: bd3e 3c83 20d6 b6d2 9db3 a860 4082 4371  .><. ......`@.Cq
+00000b70: 7fb7 7fc3 4e73 fc44 a6f5 24a2 8a25 0586  ....Ns.D..$..%..
+00000b80: d9ef a4a4 d260 af29 711e 6d9c d42e f49a  .....`.)q.m.....
+00000b90: 6319 1ae9 7579 d60d ca3c 4db7 32fc d580  c...uy...<M.2...
+00000ba0: 62a6 298e 9582 70ac 3620 4e83 8fce ff6b  b.)...p.6 N....k
+00000bb0: bbba 6e4b 7c71 e567 8f96 af58 c86f 17ce  ..nK|q.g...X.o..
+00000bc0: 6410 398a ead0 202b 985a 24c7 c926 89c4  d.9... +.Z$..&..
+00000bd0: 20af c3e4 3786 c997 60b2 1bc3 644b 30db   ...7...`...dK0.
+00000be0: 3561 c8e8 80d5 3b87 9842 baac 6ad6 5e82  5a....;..B..j.^.
+00000bf0: 795a 1586 872e 867e 0a0c 8df5 92fd e39a  yZ.....~........
+00000c00: f61c 4f09 2fee 6329 c777 da87 9cdd 62f1  ..O./.c).w....b.
+00000c10: 0b00 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
+00000c20: 0000 0021 004f 1743 310f 0d00 0083 5e00  ...!.O.C1.....^.
+00000c30: 0018 0000 0078 6c2f 776f 726b 7368 6565  .....xl/workshee
+00000c40: 7473 2f73 6865 6574 312e 786d 6c9c 93db  ts/sheet1.xml...
+00000c50: 8adb 3010 86ef 0b7d 07a1 fb58 969d cd66  ..0....}...X...f
+00000c60: 4d9c a534 842e 9452 ba3d 5c2b f238 16b1  M..4...R.=\+.8..
+00000c70: 2c57 520e dbb2 efde 9172 845c 34ac b175  ,WR......r.\4..u
+00000c80: f47c f38f 6634 79dc e996 6cc0 3a65 ba92  .|..f4y...l.:e..
+00000c90: f224 a504 3a69 2ad5 2d4b fae3 fb7c 30a6  .$..:i*.-K...|0.
+00000ca0: c479 d155 a235 1d94 f405 1c7d 9cbe 7f37  .y.U.5.....}...7
+00000cb0: d91a bb72 0d80 2748 e85c 491b effb 8231  ...r..'H.\I....1
+00000cc0: 271b d0c2 25a6 870e 776a 63b5 f038 b54b  '...%...wjc..8.K
+00000cd0: e67a 0ba2 8a46 ba65 599a 8e98 16aa a37b  .z...F.eY......{
+00000ce0: 4261 6f61 98ba 5612 6646 ae35 747e 0fb1  Baoa..V.fF.5t~..
+00000cf0: d00a 8ffa 5da3 7a77 a469 790b 4e0b bb5a  ....].zw.iy.N..Z
+00000d00: f703 6974 8f88 856a 957f 8950 4ab4 2c9e  ..it...j...PJ.,.
+00000d10: 969d b162 d162 dc3b 3e14 92ec 2cbe 197e  ...b.b.;>...,..~
+00000d20: f9d1 4d5c bff2 a495 b4c6 99da 2748 667b  ..M\........'Hf{
+00000d30: cdd7 e13f b007 26e4 8974 1dff 4d18 3e64  ...?..&..t..M.>d
+00000d40: 1636 2a24 f08c cade 2689 df9d 58d9 1996  .6*$....&...X...
+00000d50: bf11 363a c1c2 71d9 62ad aa92 fe4d 0fcf  ..6:..q.b....M..
+00000d60: 007b 1e9a f4dc 1cf7 5ee9 7452 29cc 7088  .{......^.tR).p.
+00000d70: 8a58 a84b fa81 1733 9e73 caa6 9358 413f  .X.K...3.s...XA?
+00000d80: 156c ddc5 9878 b178 8616 a407 f4c2 29f1  .l...x.x......).
+00000d90: a6ff 0cb5 ff08 6d8b d663 ace3 3fc6 e867  ......m..c..?..g
+00000da0: 2942 3a39 bfbb 987f 0945 8a7f c5d5 50d8  )B:9.....E....P.
+00000db0: 0b63 56c1 c113 a252 d4e2 2238 6811 d2ab  .cV....R.."8h...
+00000dc0: 0dec a1b3 d110 2fc7 ef28 2f8c 511a 3b69  ....../..(/.Q.;i
+00000dd0: bb1c 1f75 cee3 65f8 6a49 05b5 58b7 fe9b  ...u..e.jI..X...
+00000de0: d97e 02b5 6c3c ba1e 2608 8bd5 5454 2f33  .~..l<..&...TT/3
+00000df0: 7012 cb1b 9d27 79c0 4ad3 2203 5ba2 55b8  p....'y.J.".[.U.
+00000e00: a658 9d62 17fb adaa 7c13 9453 b200 e7e7  .X.b....|..S....
+00000e10: 2ab0 2891 6be7 8dfe 75d8 3c20 f6c6 98d8  *.(.k...u.< ....
+00000e20: 688c fdc1 38cb 93f1 7874 cfc7 f778 2837  h...8...xt...x(7
+00000e30: 5230 a391 82fd 5102 6acd b334 e7d9 7f29  R0....Q.j..4...)
+00000e40: 2cc6 f30f 0000 ffff 0000 00ff ffb4 9cdb  ,...............
+00000e50: 8e1c 450c 865f 25da 0748 a6fa dcd1 2612  ..E.._%..H....&.
+00000e60: d9bd e035 a265 45b8 2041 d910 e0ed 694f  ...5.eE. A....iO
+00000e70: d08c 3fbb ec8d 25c2 15f0 dba5 bf6b abeb  ..?...%......k..
+00000e80: ab43 8f6f 9f3e 3c3e 7eb9 7fff e5fd dbdb  .C.o.><>~.......
+00000e90: cf9f fe7a f1f9 cd4d bb79 f1f4 c7fb 8f4f  ...z...M.y.....O
+00000ea0: c7bf bd9e 6e5e fcdd a6f7 0faf 7ff9 e7fe  ....n^..........
+00000eb0: f1e9 e1f1 e397 3737 a797 e3cd dbdb 0709  ......77........
+00000ec0: fde9 883d fecf d3f1 df5f df2e f3ed abaf  ...=....._......
+00000ed0: 6f6f 5f3d fc27 bed3 62a3 76a7 b513 b57b  oo_=.'..b.v....{
+00000ee0: ad0d 17ed d561 efe2 71a0 c70f 8789 b6be  .....a..q.......
+00000ef0: 1c77 fc73 f3e2 e1cf a72f 9f7e fff9 f1b7  .w.s...../.~....
+00000f00: 5fcf 11cf 3ccc d1e8 f561 16f3 3010 cdc3  _...<....a..0...
+00000f10: 686d 9bcc d368 71ec 3fcd f823 9ee6 6834  hm...hq.?..#..h4
+00000f20: 7e1a 88e6 69b4 b699 bfe9 bd16 af4f 8abf  ~...i........O..
+00000f30: cd31 66f4 f8f9 7ffe 3647 a3f1 d340 344f  .1f.....6G...@4O
+00000f40: a3b5 6d35 7f1b 2d5e 9f14 4f33 ff88 a739  ..m5..-^..O3...9
+00000f50: 1a8d 9f06 a279 1aad 6d66 88de 6b71 ddfb  .....y..mf..kq..
+00000f60: 436d 29bc dc47 6cec 12a2 71a9 35db e55a  Cm)..Gl...q.5..Z
+00000f70: dbfa 1ed7 82c7 2336 f608 d178 d4da b5af  ......#6...x....
+00000f80: ceb3 dabd d65a 3003 6d05 9347 6c6c 12a2  .....Z0.m..Gll..
+00000f90: 31a9 b5c1 4ca1 f710 0397 7bc1 e511 1bbb  1...L.....{.....
+00000fa0: 8468 5c6a 6db0 93b9 165b 3028 dba9 829c  .h\jm....[0(....
+00000fb0: 2338 f629 4d5d 5563 1462 73d8 d1a9 2d98  #8.)M]Uc.bs...-.
+00000fc0: aa5b 898e c0a3 258a 3415 5b05 3ced 9f1e  .[....%.4.[.<...
+00000fd0: a92d 9887 9b81 640e f214 7ed2 546c 558b  .-....d...~.TlU.
+00000fe0: cd02 03a9 edda 0798 649b 2160 6e35 259b  ........d.!`n5%.
+00000ff0: 3415 5bd5 62b3 5313 525b 3039 3583 b7dc  4.[.b.S.R[095...
+00001000: 6a8a 2d69 ea62 75b8 0eb8 f324 7407 d559  j.-i.bu....$t..Y
+00001010: 456a 3400 0cbb 72ab 2993 9a56 bd55 adda  Ej4...r.)..V.U..
+00001020: c914 a9d1 6cda 2a5c 92e0 6406 d0aa b70a  ....l.*\..d.....
+00001030: feb8 6ed5 6ab0 2068 153c 4970 6255 abde  ..n.j. h.<IpbU..
+00001040: 2a54 f75e 418d deab 0aa5 5a8a 29a8 deab  *T.^A.....Z.)...
+00001050: cef5 332b 5075 ed74 ce01 1556 b514 5650  ..3+Pu.t...V..VP
+00001060: bd57 20c9 4dad a059 3009 0c15 6049 70b2  .W .M..Y0...`Ip.
+00001070: afd0 aaf3 8a5c 37b7 421d 02b8 0e15 6249  .....\7.B.....bI
+00001080: 70e2 153b 333b 6121 d74d ae50 c72b 7bb9  p..;3;a!.M.P.+{.
+00001090: adab 206b c8f7 6b5a f5fd 9a6f d9b0 67bb  .. k..kZ...o..g.
+000010a0: 8e10 7aad 306b 4899 05d5 7bd5 b9e3 75a1  ..z.0kH...{...u.
+000010b0: f76d ad8a dc35 da2e 57a0 35a4 d082 eabd  .m...5..W.5.....
+000010c0: eadc c94e afc8 1d83 15d6 50a1 9604 27e3  ...N......P...'.
+000010d0: 55ab a3d9 98df 2177 b7d8 823a 062c 182a  U.....!w...:.,.*
+000010e0: d892 e0c4 ab56 bd57 adee ae5f 911b b060  .....V.W..._...`
+000010f0: a870 4b82 13af 5af5 5eb5 eaac 2235 40c1  .pK...Z.^..."5@.
+00001100: 50c1 9604 2756 b5ea ad12 5b76 4780 a6c7  P...'V....[vG...
+00001110: 8805 156e 0d29 b7a0 7ab3 3ad7 0d57 2d8e  ...n.)..z.:..W-.
+00001120: 010a c60a b624 38ee 57a8 ce2a d476 b28c  .....$8.W..*.v..
+00001130: 853c 052c 182b dc92 e0c4 ac56 bd59 50cd  .<.,.+.....V.YP.
+00001140: 1d78 6975 0a58 3056 b825 c189 57b0 c7ce  .xiu.X0V.%..W...
+00001150: 59c8 6d27 0b03 c853 0083 b102 2e09 4ecc  Y.m'...S......N.
+00001160: 024d ce2c 765b f6e5 42cb 5374 325a 01d7  .M.,v[..B.St2Z..
+00001170: 9882 0baa 1f04 3ab7 b901 0b35 ead7 0ab8  ......:....5....
+00001180: c614 5c50 bd57 9c02 da19 16b9 01b7 c60a  ..\P.W..........
+00001190: b724 3819 0229 b790 ebd6 af50 a760 173b  .$8..).....P.`.;
+000011a0: 56b8 25c1 89d7 945b c875 eb57 a853 d4af  V.%....[.u.W.S..
+000011b0: 1570 8d29 b8a0 fa21 00ac b969 40ab 53b0  .p.)...!...i@.S.
+000011c0: 1e18 2bdc 92e0 a45f 011f 370d 68d5 ad09  ..+...._..7.h...
+000011d0: d1f2 1430 76aa 804b 8263 af50 5dbf 42dd  ...0v..K.c.P].B.
+000011e0: af6e bead b5a1 4e01 64a7 0ab7 2438 f19a  .n....N.d...$8..
+000011f0: 720b b9b3 9d5e a906 dc9a 2adc 92e0 c46b  r....^....*....k
+00001200: ca2d e4ce 76bc 520d 5030 55b0 25c1 89d7  .-..v.R.P0U.%...
+00001210: 145b c89d ed75 1ed4 e83c 73aa 604b 8213  .[...u...<s.`K..
+00001220: af5a f5e3 15d7 5bce 2bee b782 396b aa60  .Z....[.+...9k.`
+00001230: 4b82 13af e97e 0bb9 b3bd bca2 1a6c 0ca6  K....~.......l..
+00001240: 0ab7 2438 f18a a33e f3a6 df21 d75d 82b2  ..$8...>...!.]..
+00001250: e560 fd3a 55b8 25c1 8957 adce ce6b b6df  .`.:U.%..W...k..
+00001260: 42c3 7334 6555 b035 a5d8 82ea adea 5cbb  B.s4eU.5......\.
+00001270: 8541 6a74 503c 55a8 25c1 49af 6ad5 5bd5  .AjtP<U.%.I.j.[.
+00001280: aabf 3846 6eff 1a73 ae40 4b82 63ab 509d  ..8Fn..s.@K.c.P.
+00001290: 55a8 83dd c050 0d16 0373 055a 129c 78d5  U....P...s.Z..x.
+000012a0: aaf7 8a7b 2d0b 2db6 1c40 6bae 404b 8213  ...{-.-..@k.@K..
+000012b0: af5a f55e 7148 e86e dbd1 72b0 2798 2bd0  .Z.^qH.n..r.'.+.
+000012c0: 92e0 c4ab 56bd 57ec b5ec fe85 2d07 809d  ....V.W.....-...
+000012d0: 2bd0 92e0 c42b c063 272c e4ba 4d01 d568  +....+.c',..M..h
+000012e0: bc56 a035 a7d0 82ea fb15 7b2d 0b58 e446  .V.5......{-.X.F
+000012f0: dd5a 61d6 9c32 0baa b7aa 73dd fe85 2d07  .Za..2....s...-.
+00001300: 7bad b9c2 2c09 be0c 81dd de6e 4375 e7c4  {...,......nCu..
+00001310: 50ed 0e16 e212 2c05 e60a b324 38b1 8aeb  P.....,....$8...
+00001320: 297b ad81 dc76 32f2 3de4 25d8 bfcc 156a  ){...v2.=.%....j
+00001330: 4970 6216 f753 ce6c 7646 8886 97e8 03a1  Ipb..S.lvF......
+00001340: 0ab5 164d 2d37 04a0 ba21 40d5 520b 6ab4  ...M-7...!@.R.j.
+00001350: 1858 2ad4 92e0 b85b a17a af3a d72d 0690  .X*....[.z.:.-..
+00001360: 1bac b297 0ab4 2438 b19a de6c 21d7 ddc4  ......$8...l!...
+00001370: 421d 82c9 75a9 404b 8213 af5a f5dd 9a42  B...u.@K...Z...B
+00001380: 0b2d afc1 2a7b a940 4b82 13af 5af5 5ed3  .-..*{.@K...Z.^.
+00001390: 9d16 5a5e 8385 cb52 8196 0427 5ed3 ef31  ..Z^...R...'^..1
+000013a0: 90eb 000b 35ba 315c 2ad4 92e0 c4ab 567d  ....5.1\*.....V}
+000013b0: bfa6 d442 cb6b 40d8 a542 2d09 4ebc a627  ...B.k@..B-.N..'
+000013c0: 84cc b5fb 17a8 d18d e152 c196 0427 5ed3  .........R...'^.
+000013d0: ab2d e6ba af30 911b cd03 156a 2d29 b5a0  .-...0.....j-)..
+000013e0: ba53 0ca8 ce2a 0e17 83d5 c05a a196 04c7  .S...*.....Z....
+000013f0: dd0a d559 85da 4e76 03c3 e4e8 fbd6 0ab6  ...Y..Nv........
+00001400: d614 5b50 bd59 e49a 6f9f 991a ac06 d60a  ..[P.Y..o.......
+00001410: b624 38e9 d7f4 8010 b9fe c610 7274 63b8  .$8.........rtc.
+00001420: 56b8 25c1 89d9 f484 10b9 6ec3 0d35 ba31  V.%.......n..5.1
+00001430: 5c2b dc92 e0c4 6b7a 4288 5c7f 6308 39ba  \+....kzB.\.c.9.
+00001440: 315c 2be0 92e0 c46c 7a44 885c b778 81ba  1\+....lzD.\.x..
+00001450: 0490 5d2b e092 e0c4 6b7a b585 5c77 6308  ..]+....kz..\wc.
+00001460: 35da c3ac 1570 4970 e235 0517 72fd 1e06  5....pIp.5..r...
+00001470: 72b4 8759 2be4 92e0 c46c 4a2e e4ba d50b  r..Y+....lJ.....
+00001480: d468 13b3 56c8 25c1 89d7 f46e 0bb9 6ecf  .h..V.%....n..n.
+00001490: 0d75 0df6 dc5b 055d 121c 7b85 ea68 40d5  .u...[.]..{..h@.
+000014a0: dec1 405d 835d cc56 2197 0427 5ed3 bb2d  ..@].].V!..'^..-
+000014b0: e4ba 3b43 a86b b07a d92a e892 e0c4 6b8a  ..;C.k.z.*....k.
+000014c0: 2ee6 da3b 43a8 d19d e156 2197 0427 5e53  ...;C....V!..'^S
+000014d0: 7221 d7dd 1952 0d26 d8ad 422e 094e bca6  r!...R.&..B..N..
+000014e0: e442 aebb 33a4 1aec 0cb6 0ab8 2438 f19a  .B..3.......$8..
+000014f0: 820b b9ee ce10 6a74 67b8 55c0 25c1 89d7  ......jtg.U.%...
+00001500: 145c c875 3f57 843a 47f3 4005 5c5b 0a2e  .\.u?W.:G.@.\[..
+00001510: a87e cec2 cd97 3d82 47ee 1c6c 0db6 0ab7  .~....=.G..l....
+00001520: 2438 e957 5c7d d9df 6a69 d15d 19a2 e188  $8.W\}..ji.]....
+00001530: 0415 6a6d 29b5 a09a 6ebb 8368 b75b 1483  ..jm)...n..h.[..
+00001540: 3edd 2bcc 92e0 b84f a15a a74c 351b 1866  >.+....O.Z.L5..f
+00001550: 464e 2bc4 da53 6241 754e 79af 654f 8999  FN+..SbAuNy.eO..
+00001560: 1bec 0bf7 0ab1 2438 e955 5c4e d9df ebe1  ......$8.U\N....
+00001570: 00d1 9ebc a2e1 6881 b557 8025 c189 55dc  ......h..W.%..U.
+00001580: 7a59 ab38 2174 bf2d d46a b4be da2b bc92  zY.8!t.-.j...+..
+00001590: e0c4 2a2e bdac 552d bafd 001a 8e0e 5ef7  ..*...U-......^.
+000015a0: 0aae 2438 b18a 3b2f 6b55 8b6e 858d 86d7  ..$8..;/kU.n....
+000015b0: 68ac 5668 b5a7 b482 eade 2b9d ea7e f18c  h.Vh......+..~..
+000015c0: d4e8 27cf 7b05 5612 9cf4 2a3e d3b0 bdaa  ..'.{.V...*>....
+000015d0: 45b7 1740 c35b 709a bd57 5825 c189 d58c  E..@.[p..WX%....
+000015e0: 5548 753f 2981 1a2d 57f6 0aac 2438 b1aa  UHu?)..-W...$8..
+000015f0: 5537 00b4 e856 2b68 38fa c9ee a942 abe3  U7...V+h8....B..
+00001600: 4c2f f34a d99a a5ea f62d 94b7 6081 7d9c  L/.J.....-..`.}.
+00001610: 7e95 7e0e 9d42 ebdc d8a5 ebdd 9d31 65b7  ~.~..B.......1e.
+00001620: 6aa1 bc04 a3f6 3855 2a19 4ec9 756e 2c33  j.....8U*.N.un,3
+00001630: acb3 ede2 85c9 5bf0 51c6 7100 52f2 9be2  ......[.Q.q.R...
+00001640: ebdc 58e6 17d9 6609 c3e4 e898 a89d 2a08  ..X...f.......*.
+00001650: 3b47 c72f 1be5 ce80 00c6 dc75 37d3 a3b3  ;G./.......u7...
+00001660: a276 aa90 ec1c 9d39 d6b8 ea38 c65d 98fb  .v.....9...8.]..
+00001670: 9dac 58b9 34be 8573 4485 67ed 9402 8d72  ..X.4..sD.g....r
+00001680: c730 aebc 7c19 022d 47ab 9a76 aa50 ed1c  .0..|..-G..v.P..
+00001690: 9df5 30b6 59f6 7b1d 66bb a50d e568 6dd3  ..0.Y.{.f....hm.
+000016a0: 4e15 b69d a333 c39a 6e9d 1ed6 b22f 4920  N....3..n..../I 
+000016b0: 562e 8d47 07c9 ed54 21dc 393a 33ac 31d6  V..G...T!.9:3.1.
+000016c0: 310c cad9 7d2e 1b5f a269 ad56 4603 c530  1...}.._.i.VF..0
+000016d0: dcb7 1b0d b237 cc52 1a6e 1e66 198e b096  .....7.R.n.f....
+000016e0: 4609 7428 7ad1 31ac 39d8 318c f346 7bfa  F.t(z.1.9.1..F{.
+000016f0: d958 5123 3852 6cb5 921a 287d d131 ac49  .XQ#8Rl...(}.1.I
+00001700: d631 ac65 b7f0 395b b98c b7b0 834b a043  .1.e..9[.....K.C
+00001710: fd8b 8e5f 4db2 8e5f 2dfb a50f eb72 4415  ..._M.._-....rD.
+00001720: 2b6a d535 5022 6333 d3d6 bb06 f978 876c  +j.5P"c3.....x.l
+00001730: 3518 a6fb 31ac 4918 1583 90ea 16df 5f2d  5...1.I......._-
+00001740: 0db5 303a 86b1 2feb 18a6 6ebf 466c 6c3e  ..0:../...n.Fll>
+00001750: 2ab6 53ab b581 621b 1dcb 6499 ef63 ea8e  *.S...b...d..c..
+00001760: ce68 7e8f 1698 b59a 1b28 bad1 b18c 7d5a  .h~......(....}Z
+00001770: a797 b5ee 4705 3688 d112 5eaa 6514 8605  ....G.6...^.e...
+00001780: 8e0e fd38 06cd 3a86 a93b 7aa0 74c7 1ed2  ...8..:..;z.t...
+00001790: a384 3b94 d8e8 f4b1 e659 efd5 a3ee 7b19  ..;......Y....{.
+000017a0: 1bc6 687a 2b95 e168 a896 e12d b3d4 86ef  ..hz+..h...-....
+000017b0: 65a3 db7b 1e36 bf87 3599 4ac8 43d1 8c8e  e..{.6..5.J.C...
+000017c0: 651e 3aba 970f e9ae 2e0f d568 8293 2a1b  e.:........h..*.
+000017d0: df3f 9251 93a3 6358 33ad 332c 98ee e637  .?.Q..cX3.3,...7
+000017e0: c8d1 5776 4d2a 6214 1c6b 6c75 1cf3 00d2  ..WvM*b..klu....
+000017f0: 77b1 d6dd a720 672f 174a 47df da35 a98b  w.... g/.JG..5..
+00001800: 5170 8c2f 11dd 6c81 221b bd3e e606 cfee  Qp./..l."..>....
+00001810: 4891 1e7d 71d7 4a45 3ace d1c9 da18 a536  H..}q.JE:......6
+00001820: 7a8e 9fc1 1ef2 b708 7ba5 5a1d 0dc5 3afc  z.......{.Z...:.
+00001830: 5a08 72cf 32f6 70ae 8fb1 7d8c 1852 2ad8  Z.r.2.p...}..R*.
+00001840: d150 b1a3 63f8 19e8 21fd d8c0 3acb c05e  .P..c...!...:..^
+00001850: c490 52e1 8e86 f21a 1dcb cf60 8fe9 ce30  ..R........`...0
+00001860: b2d5 b744 2c3a 2525 370a af5e 7a8e d950  ...D,:%%7..^z..P
+00001870: bfa3 372a d2b3 4ca6 87d3 5ba9 8847 43a9  ..7*..L...[..GC.
+00001880: 0ddf c7a6 5087 9bde a0fb e90d 7238 bd95  ....P.......r8..
+00001890: 2a79 3494 f2e8 387e 8679 48f7 95c8 20bb  *y4...8~.yH... .
+000018a0: e9ed d5b5 1af2 bf00 0000 ffff 0000 00ff  ................
+000018b0: ff44 8f41 0e82 400c 45af 32e9 0104 638c  .D.A..@.E.2...c.
+000018c0: 1b60 a31b 1726 269c 6084 c234 e2b4 2955  .`...&&.`..4..)U
+000018d0: 23a7 7720 1277 7dbf cdff bf85 048e 68d4  #.w .w}.......h.
+000018e0: 5cd5 751c eddc 96b0 0567 1fc1 1222 1f39  \.u......g...".9
+000018f0: be50 47e2 0859 5588 eff1 e2b5 a738 ba01  .PG..YU......8..
+00001900: 3b2b 21df 1cc0 29f5 619d 8d65 51f7 e06e  ;+!...).a..eQ..n
+00001910: 6cc6 8f95 02fa 1675 a61d a424 b615 7ebe  l......u...$..~.
+00001920: 35da 539c 7841 ad69 4ae1 3938 56c2 68de  5.S.xA.iJ.98V.h.
+00001930: 527c 09c2 6aea c9c0 85a4 4fa9 ab1f 4e42  R|..j.....O...NB
+00001940: cb61 ea98 5ef8 73c3 4238 ceab e49e bd59  .a..^.s.B8.....Y
+00001950: ef63 40b4 ea0b 0000 ffff 0300 504b 0304  .c@.........PK..
+00001960: 1400 0600 0800 0000 2100 63fd ce8f 1102  ........!.c.....
+00001970: 0000 f303 0000 1800 0000 786c 2f77 6f72  ..........xl/wor
+00001980: 6b73 6865 6574 732f 7368 6565 7432 2e78  ksheets/sheet2.x
+00001990: 6d6c 9c92 5b6b c230 14c7 df07 fb0e 21ef  ml..[k.0......!.
+000019a0: 366d 7532 4bab 0c44 e6db 18db de63 7ada  6mu2K..D.....cz.
+000019b0: 069b a424 f1c6 d877 df49 dd54 f045 0cb9  ...$...w.I.T.E..
+000019c0: 5f7e e79c 9c7f 3edb ab96 6cc1 3a69 7441  _~....>...l.:itA
+000019d0: 9328 a604 b430 a5d4 7541 3f3f 1683 674a  .(...0..uA??..gJ
+000019e0: 9ce7 bae4 add1 50d0 0338 3a9b 3e3e e43b  ......P..8:.>>.;
+000019f0: 63d7 ae01 f004 09da 15b4 f1be cb18 73a2  c.............s.
+00001a00: 01c5 5d64 3ad0 7852 19ab b8c7 a5ad 99eb  ..]d:.xR........
+00001a10: 2cf0 b27f a45a 96c6 f198 292e 353d 1232  ,....Z....).5=.2
+00001a20: 7b0b c354 9514 3037 62a3 40fb 23c4 42cb  {..T..07b.@.#.B.
+00001a30: 3dfa ef1a d9b9 7f9a 12b7 e014 b7eb 4d37  =.............M7
+00001a40: 1046 7588 58c9 56fa 430f a544 896c 596b  .Fu.X.V.C..D.lYk
+00001a50: 63f9 aac5 b8f7 c988 0bb2 b758 536c c37f  c..........XSl..
+00001a60: 33fd fe95 2525 8535 ce54 3e42 323b fa7c  3...%%.5.T>B2;.|
+00001a70: 1dfe 844d 1817 27d2 75fc 3761 9211 b3b0  ...M..'.u.7a....
+00001a80: 9521 8167 547a 9f4b c9d3 8995 9e61 c33b  .!.gTz.K.....a.;
+00001a90: 61e3 132c 7c97 cd36 b22c e877 fc57 0638  a..,|..6.,.w.W.8
+00001aa0: 26a1 8b07 7112 ba8b f243 a779 2931 c321  &...q....C.y)1.!
+00001ab0: 2a62 a12a e84b 42d9 34ef c5f3 2561 e72e  *b.*.KB.4...%a..
+00001ac0: e624 6871 65cc 3a1c 2cd1 461c aeb2 abbb  .$hqe.:.,.F.....
+00001ad0: 8b5e 8b6f 9694 50f1 4deb dfcd ee15 64dd  .^.o..P.M.....d.
+00001ae0: 7814 fe28 1aa1 8f21 c959 7998 8313 a82e  x..(...!.Yy.....
+00001af0: 0445 4344 fd02 0000 ffff 0000 00ff ffb2  .ECD............
+00001b00: 29ce 484d 2d71 492c 49d4 b703 0000 00ff  ).HM-qI,I.......
+00001b10: ff00 0000 ffff 448c 410a c240 0c45 af12  ......D.A..@.E..
+00001b20: 7200 2b88 b869 bb72 ebaa 2718 6b3a 13ac  r.+..i.r..'.k:..
+00001b30: 4d48 a342 4fef 4c61 70f7 df7f 9fdf 6a88  MH.BO.Lap.....j.
+00001b40: 740b 1679 5961 a6c9 3b3c 1e2e 08c6 31d5  t..yYa..;<....1.
+00001b50: eca2 7b7b 46b8 8bbb bc2a 250a 0fb2 4227  ..{{F....*%...B'
+00001b60: 8449 c42b 347d 5b7e 07f2 b782 0625 1b78  .I.+4}[~.....%.x
+00001b70: a33c 4410 635a 3c38 cbd2 a18a b905 7684  .<D.cZ<8......v.
+00001b80: 94fb 4db2 98af cafb f043 e63c fe79 1465  ..M......C.<.y.e
+00001b90: 5a8b caef cd57 ecb9 2622 ef7f 0000 00ff  Z....W..&"......
+00001ba0: ff03 0050 4b03 0414 0006 0008 0000 0021  ...PK..........!
+00001bb0: 009c 73ee 7814 0200 00f3 0300 0018 0000  ..s.x...........
+00001bc0: 0078 6c2f 776f 726b 7368 6565 7473 2f73  .xl/worksheets/s
+00001bd0: 6865 6574 332e 786d 6c9c 92df 6bc2 3010  heet3.xml...k.0.
+00001be0: c7df 07fb 1f42 de6d 5aed 6496 5619 88cc  .....B.mZ.d.V...
+00001bf0: b731 b6bd c7f4 6a83 4d52 92f8 8bb1 ff7d  .1....j.MR.....}
+00001c00: 973a 75d0 17b1 a4f9 75c9 e7ee 72df 7c76  .:u.....u...r.|v
+00001c10: 500d d981 75d2 e882 2651 4c09 6861 4aa9  P...u...&QL.haJ.
+00001c20: d705 fdfc 580c 9e29 719e eb92 3746 4341  ....X..)q...7FCA
+00001c30: 8fe0 e86c faf8 90ef 8ddd b81a c013 2468  ...l..........$h
+00001c40: 57d0 dafb 3663 cc89 1a14 7791 6941 a3a5  W...6c....w.iA..
+00001c50: 3256 718f 4bbb 66ae b5c0 cbee 926a d830  2Vq.K.f......j.0
+00001c60: 8ec7 4c71 a9e9 8990 d95b 18a6 aaa4 80b9  ..Lq.....[......
+00001c70: 115b 05da 9f20 161a ee31 7e57 cbd6 9d69  .[... ...1~W...i
+00001c80: 4adc 8253 dc6e b6ed 4018 d522 6225 1be9  J..S.n..@.."b%..
+00001c90: 8f1d 9412 25b2 e55a 1bcb 570d e67d 4852  ....%..Z..W..}HR
+00001ca0: 2ec8 c162 1be2 3f3a bbe9 f67b 9e94 14d6  ...b..?:...{....
+00001cb0: 3853 f908 c9ec 1473 3ffd 099b 302e 2ea4  8S.....s?...0...
+00001cc0: 7efe 3761 9294 59d8 c950 c02b 6a78 5f48  ~.7a..Y..P.+jx_H
+00001cd0: c9d3 8535 bcc2 4677 c2c6 1758 782e 9b6d  ...5..Fw...Xx..m
+00001ce0: 6559 d0ef f8ef 1be0 9884 2e1e c4a8 856e  eY.............n
+00001cf0: 76b6 fdd0 695e 4aac 70c8 8a58 a80a fa92  v...i^J.p..X....
+00001d00: 5036 cd3b f17c 49d8 bb7f 7312 b4b8 3266  P6.;.|I...s...2f
+00001d10: 130c 4bf4 1187 a3ac 7776 d169 f1cd 9212  ..K.....wv.i....
+00001d20: 2abe 6dfc bbd9 bf82 5cd7 1e85 9f46 29c6  *.m.....\....F).
+00001d30: 188a 9c95 c739 3881 ea42 5034 42d4 2f00  .....98..BP4B./.
+00001d40: 0000 ffff 0000 00ff ffb2 29ce 484d 2d71  ..........).HM-q
+00001d50: 492c 49d4 b703 0000 00ff ff00 0000 ffff  I,I.............
+00001d60: 448c 410a c240 0c45 af12 7200 2b88 b869  D.A..@.E..r.+..i
+00001d70: bb72 ebaa 2718 6b3a 13ac 4d48 a342 4fef  .r..'.k:..MH.BO.
+00001d80: 4c61 70f7 df7f 9fdf 6a88 740b 1679 5961  Lap.....j.t..yYa
+00001d90: a6c9 3b3c 1e2e 08c6 31d5 eca2 7b7b 46b8  ..;<....1...{{F.
+00001da0: 8bbb bc2a 250a 0fb2 4227 8449 c42b 347d  ...*%...B'.I.+4}
+00001db0: 5b7e 07f2 b782 0625 1b78 a33c 4410 635a  [~.....%.x.<D.cZ
+00001dc0: 3c38 cbd2 a18a b905 7684 94fb 4db2 98af  <8......v...M...
+00001dd0: cafb f043 e63c fe79 1465 5a8b caef cd57  ...C.<.y.eZ....W
+00001de0: ecb9 2622 ef7f 0000 00ff ff03 0050 4b03  ..&".........PK.
+00001df0: 0414 0006 0008 0000 0021 00f8 a6e9 a88a  .........!......
+00001e00: 0600 00ec 1b00 0013 0000 0078 6c2f 7468  ...........xl/th
+00001e10: 656d 652f 7468 656d 6531 2e78 6d6c ec59  eme/theme1.xml.Y
+00001e20: 4f6f 1347 14bf 57ea 7718 ed1d 623b b613  Oo.G..W.w...b;..
+00001e30: 4738 2876 6cd2 4220 4a0c 15c7 f17a bc3b  G8(vl.B J....z.;
+00001e40: 7876 6735 334e f00d c1b1 52a5 0a5a f552  xvg53N....R..Z.R
+00001e50: a9b7 1eaa b648 20f5 42bf 4cd3 52b5 54e2  .....H .B.L.R.T.
+00001e60: 2bf4 cdcc dade 8927 1043 a496 161f 127b  +......'.C.....{
+00001e70: f6f7 fecc fb37 efcd 5eba 7c37 61e8 9008  .....7..^.|7a...
+00001e80: 4979 da0c ca17 4b01 2269 c807 348d 9ac1  Iy....K."i..4...
+00001e90: cd5e f7c2 7a80 a4c2 e900 339e 9266 3021  .^..z.....3..f0!
+00001ea0: 32b8 bcf9 e107 97f0 868a 4942 10d0 a772  2.........IB...r
+00001eb0: 0337 8358 a96c 6365 4586 b08c e545 9e91  .7.X.lceE....E..
+00001ec0: 149e 0db9 48b0 829f 225a 1908 7c04 7c13  ....H..."Z..|.|.
+00001ed0: b652 2995 ea2b 09a6 6980 529c 00db 1bc3  .R)..+..i.R.....
+00001ee0: 210d 09ea 1996 f074 0d5d 4095 52b9 146c  !......t.]@.R..l
+00001ef0: 4e05 7518 484b 95d4 0b21 1307 5a0c c9a9  N.u.HK...!..Z...
+00001f00: f7f0 8812 8572 269a fc97 7b0f 67e4 8351  .....r&...{.g..Q
+00001f10: 5913 c989 6c33 810e 316b 06a0 c680 1ff5  Y...l3..1k......
+00001f20: c85d 1520 86a5 8207 cda0 643e c1ca e6a5  .]. ......d>....
+00001f30: 15bc 9113 3175 0a6d 81ae 6b3e 395d 4e30  ....1u.m..k>9]N0
+00001f40: 1855 8c4c 11f5 6742 cbdd 6a63 6d7b c6df  .U.L..gB..jcm{..
+00001f50: 0098 5ac4 753a 9d76 a73c e367 0038 0c61  ..Z.u:.v.<.g.8.a
+00001f60: f356 9722 cf6a 77bd dc9a f22c 80ec d745  .V.".jw....,...E
+00001f70: deed 52ad 5475 f105 feab 0b3a 375a ad56  ..R.Tu.....:7Z.V
+00001f80: ad91 eb62 991a 90fd 5a5d c0af 97ea d5ad  ...b....Z]......
+00001f90: 8a83 3720 8baf 2de0 abad ad76 bbee e00d  ..7 ..-....v....
+00001fa0: c8e2 eb0b f8ee 5aa3 5e75 f106 1433 9a8e  ......Z.^u...3..
+00001fb0: 16d0 daa1 dd6e ce7d 0619 72b6 e385 af03  .....n.}..r.....
+00001fc0: 7cbd 94c3 e728 8886 59c0 6911 439e aa25  |....(..Y.i.C..%
+00001fd0: c22f c177 b8e8 028d a665 58d1 14a9 4946  ./.w.....eX...IF
+00001fe0: 8638 84b8 6fe3 a42f 28d6 32f1 06c1 8527  .8..o../(.2....'
+00001ff0: 7629 940b 4b5a 3c92 a1a0 996a 061f 6718  v)..KZ<....j..g.
+00002000: 7268 ceef e5b3 ef5f 3e7b 825e 3e7b 7c7c  rh....._>{.^>{||
+00002010: ffe9 f1fd 9f8e 1f3c 38be ffa3 e5e5 10ee  .......<8.......
+00002020: e034 2a12 bef8 f6f3 bfbe be87 fe7c f2cd  .4*..........|..
+00002030: 8b47 5ff8 f1b2 88ff ed87 4f7f fdf9 a11f  .G_.......O.....
+00002040: 0849 35d7 e8f9 978f 7f7f faf8 f957 9ffd  .I5..........W..
+00002050: f1dd 230f 7c4b e07e 11de a309 91e8 3a39  ..#.|K.~......:9
+00002060: 42fb 3c81 bd19 c3b8 9a93 be58 8ea2 1763  B.<........X...c
+00002070: ea50 e018 787b 5877 54ec 00af 4f30 f3e1  .P..x{XwT...O0..
+00002080: 5ac4 35de 2d01 f5c4 07bc 32be e3e8 7a10  Z.5.-.....2...z.
+00002090: 8bb1 a21e c957 e3c4 01ee 72ce 5a5c 780d  .....W....r.Z\x.
+000020a0: 7055 cb2a 58b8 374e 23bf 7031 2ee2 f631  pU.*X.7N#.p1...1
+000020b0: 3ef4 c96e e3d4 716d 679c 416d 9d06 a563  >..n..qmg.Am...c
+000020c0: fb76 4c1c 35f7 184e 158e 480a d557 3fe3  .vL.5..N..H..W?.
+000020d0: 2342 3cbb bb4d a963 d75d 1a0a 2ef9 50a1  #B<..M.c.]....P.
+000020e0: db14 b530 f59a a447 fb4e 20cd 8976 6802  ...0...G.N ..vh.
+000020f0: 7e99 f8f6 0cae 766c b37b 0bb5 38f3 ed7a  ~.....vl.{..8..z
+00002100: 9b1c ba48 4808 cc3c caf7 0873 cc78 058f  ...HH..<...s.x..
+00002110: 154e 7c2c 7b38 6145 835f c32a f629 7930  .N|,{8aE._.*.)y0
+00002120: 1161 11d7 910a 3c1d 11c6 5167 40a4 f4d1  .a....<...Qg@...
+00002130: dc10 b0df 82d3 af62 2861 5eb7 efb2 49e2  .......b(a^...I.
+00002140: 2285 a223 1fcf 6b98 f322 729b 8fda 314e  "..#..k.."r...1N
+00002150: 32af ce34 8d8b d88f e408 4214 a33d ae7c  2..4......B..=.|
+00002160: f05d ee66 88fe 0d7e c0e9 a9ee be05 27f8  .].f...~......'.
+00002170: 7269 7d93 468e 4af3 00d1 4fc6 c2e3 cb2b  ri}.F.J...O....+
+00002180: 84bb f938 6143 4c4c 9581 2aef 54ea 84a6  ...8aCLL..*.T...
+00002190: af2a db8c 42dd 7e5f b6a7 e7d8 161c 62be  .*..B.~_......b.
+000021a0: e4d9 3951 ac4f c3bd 8325 7a1b 8fd3 3d02  ..9Q.O...%z...=.
+000021b0: 59b1 7844 bdaf d0ef 2b74 f09f afd0 a7e5  Y.xD....+t......
+000021c0: f2f9 d7e5 7929 862a 3d6f bf4d 339e 2cd3  ....y).*=o.M3.,.
+000021d0: 8b0f 2963 076a c2c8 3569 da71 0967 d2a0  ..)c.j..5i.q.g..
+000021e0: 0b8b 6674 3023 e56c 5ccb 62f8 9a0f 030e  ..ft0#.l\.b.....
+000021f0: 2e12 d8d0 20c1 d527 54c5 0731 cea0 952f  .... ..'T..1.../
+00002200: 9b59 3592 39eb 48a2 8c4b 982a cdb2 998a  .Y5.9.H..K.*....
+00002210: c909 de66 b6a5 d0cd 9b99 b4a6 a715 5b4c  ...f..........[L
+00002220: 2456 bb7c 6097 578b 53e9 8c8d 9951 2333  $V.|`.W.S....Q#3
+00002230: 0c4f 05ad 6a06 6715 b6ba f676 c2ca 56ab  .O..j.g....v..V.
+00002240: 53cd e66e ad6c 5433 75d2 d9da 6ccb e0d6  S..n.lT3u...l...
+00002250: c5ad c1e2 cc9a d0ec 2068 91c0 ca75 18ef  ........ h...u..
+00002260: b5ee 3002 6146 06da ee76 629f ba45 8b3e  ..0.aF...vb..E.>
+00002270: 5717 c918 0f48 ee23 bdef 451f 958d 93a6  W....H.#..E.....
+00002280: b132 0d23 8f8f f484 f91a 1f15 a435 34db  .2.#.........54.
+00002290: b790 7616 2715 c555 4f11 37f5 dedb 7869  ..v.'..UO.7...xi
+000022a0: 3a56 cfbd a453 f944 3ab2 b498 9c2c 4547  :V...S.D:....,EG
+000022b0: cda0 51ab d402 14e2 ac19 0c61 7a86 af49  ..Q........az..I
+000022c0: 065e 97ba bfc4 2c82 4bab 5009 1bf6 af4d  .^....,.K.P....M
+000022d0: 6613 ae73 6f36 fc61 5986 3b12 6bf7 850d  f..so6.aY.;.k...
+000022e0: 3b75 2013 526d 6319 dbd0 308f f210 60a9  ;u .Rmc...0...`.
+000022f0: 99f5 8dfe 951a 98f5 bc36 6023 fd0d b458  .........6`#...X
+00002300: 5d87 60f8 c7b4 003b baae 25c3 2109 55d1  ].`....;..%.!.U.
+00002310: d985 1573 1562 0079 29e5 6345 c441 3c38  ...s.b.y).cE.A<8
+00002320: 427d 3616 fb18 dcaf 4315 f633 a012 2e41  B}6.....C..3...A
+00002330: 4c45 d03f e012 4f5b db3c 728b 739e 74c5  LE.?..O[.<r.s.t.
+00002340: ab33 83b3 eb98 6531 cecb ad4e d169 265b  .3....e1...N.i&[
+00002350: b8c9 e399 0ee6 97d5 d6a8 077b f3ea 6e36  ...........{..n6
+00002360: b7fc 564c ca9f d356 8a61 fc3f db8a 3e4f  ..VL...V.a.?..>O
+00002370: e056 6275 a03d 10c2 15b3 c048 e76b 33e0  .Vbu.=.....H.k3.
+00002380: 42c5 1caa 5016 d3b0 2be0 2ecd d40e 8816  B...P...+.......
+00002390: b808 86c7 1054 70d1 6dfe 0b72 a8ff db9c  .....Tp.m..r....
+000023a0: b33c 4c5a c370 a9f6 6984 0485 f348 c582  .<LZ.p..i....H..
+000023b0: 903d 284b 26fa 5ec3 ac9c 9f5d 9625 cb19  .=(K&.^....].%..
+000023c0: 9988 2aa8 2b33 ab76 9f1c 12d6 d335 b0ae  ..*.+3.v.....5..
+000023d0: cff6 00c5 10ea a69a e465 c0e0 4ec6 9ffb  .........e..N...
+000023e0: 3bcf a07e a49b 9c7f 6be7 6393 79d9 f640  ;..~....k.c.y..@
+000023f0: 7707 b6c5 b2f4 67ec 45aa 85a2 5f38 0a1a  w.....g.E..._8..
+00002400: deb3 cff4 54b3 72f0 8a83 7dc9 a3d6 56ac  ....T.r...}...V.
+00002410: 851d 576a 673e 6a33 b85b 42fa 0f9c 7f54  ..Wjg>j3.[B....T
+00002420: 848c 9830 d607 6a8f ef43 6d45 f096 c3b6  ...0..j..CmE....
+00002430: 5708 a2fa 826d 3c90 2e90 b63c f6a1 71b2  W....m<....<..q.
+00002440: 8b36 9834 2bdb b0e4 dded b9b7 5170 f19d  .6.4+.......Qp..
+00002450: 77ba 33b9 90a5 6fd2 e92e 69ec 5973 e68a  w.3...o...i.Ys..
+00002460: 7372 f1d5 dde7 72c6 ce2d ecd8 bad8 e97a  sr....r..-.....z
+00002470: 4c0d 497b 3245 757b 349d 6d8c 63cc ebb6  L.I{2Eu{4.m.c...
+00002480: e25b 30de bf03 8ede 8637 0963 a6a4 7d83  .[0......7.c..}.
+00002490: 7017 6e12 61ca b0af 2720 f9ad 730d e9e6  p.n.a...' ..s...
+000024a0: df00 0000 ffff 0300 504b 0304 1400 0600  ........PK......
+000024b0: 0800 0000 2100 1e63 f513 bc02 0000 d106  ....!..c........
+000024c0: 0000 0d00 0000 786c 2f73 7479 6c65 732e  ......xl/styles.
+000024d0: 786d 6cb4 555b 6bdb 3014 7e1f ec3f 08bd  xml.U[k.0.~..?..
+000024e0: bbb2 9d38 4b82 edb2 3435 14ba 3168 077b  ...8K...45..1h.{
+000024f0: 556c 3911 d525 484a e66c ecbf f7c8 7612  Ul9..%HJ.l....v.
+00002500: 878e 6db4 ec25 3e3a 3afa ce77 ae49 af1b  ..m..%>::..w.I..
+00002510: 29d0 9e19 cbb5 ca70 7415 62c4 54a9 2bae  )......pt.b.T.+.
+00002520: d619 fefa 5804 538c aca3 aaa2 422b 96e1  ....X.S.....B+..
+00002530: 03b3 f83a 7fff 2eb5 ee20 d8c3 8631 8700  ...:..... ...1..
+00002540: 42d9 0c6f 9cdb ce09 b1e5 8649 6aaf f496  B..o.......Ij...
+00002550: 29b8 a9b5 91d4 c1d1 ac89 dd1a 462b eb1f  )...........F+..
+00002560: 4941 e230 9c10 49b9 c21d c25c 96ff 0222  IA.0..I....\..."
+00002570: a979 da6d 8352 cb2d 757c c505 7787 160b  .y.m.R.-u|..w...
+00002580: 2359 ceef d64a 1bba 1240 b589 c6b4 444d  #Y...J...@....DM
+00002590: 3431 316a ccd1 49ab 7de1 47f2 d268 ab6b  411j..I.}.G..h.k
+000025a0: 7705 b844 d735 2fd9 4bba 3332 23b4 3c23  w..D.5/.K.32#.<#
+000025b0: 01f2 eb90 a284 84f1 45ec 8d79 25d2 9818  ........E..y%...
+000025c0: b6e7 be7c 384f 6bad 9c45 a5de 2997 e118  ...|8Ok..E..)...
+000025d0: 88fa 14cc 9f94 feae 0a7f 0515 eead f2d4  ................
+000025e0: fe40 7b2a 4013 6192 a7a5 16da 2007 a583  .@{*@.a..... ...
+000025f0: ccb5 1a45 25eb 2c6e a8e0 2bc3 bd59 4d25  ...E%.,n..+..YM%
+00002600: 1787 4e1d b7ef 36d4 58e8 8116 2a1e 4dbd  ..N...6.X...*.M.
+00002610: aeed 80fe ade4 500f af24 9e5b c7f0 ecbb  ......P..$.[....
+00002620: 35ff 3f8e 5a7f 161c 7221 0629 e914 790a  5.?.Z...r!.)..y.
+00002630: bde3 9851 05dc a25e 7e3c 6c21 7605 6dde  ...Q...^~<l!v.m.
+00002640: f185 abbf 5aaf 0d3d 4471 3278 405a 8779  ....Z..=Dq2x@Z.y
+00002650: bad2 a682 b13a 16c3 e7bd 53e5 a960 b583  .....:....S..`..
+00002660: 8c18 bede f8af d35b f85d 69e7 a0f5 f2b4  .......[.]i.....
+00002670: e274 ad15 153e 67c7 17bd 00e1 944c 8807  .t...>g......L..
+00002680: 3f7a dfea 0bec a646 6a27 0be9 eeaa 0cc3  ?z.....Fj'......
+00002690: 10fb 6c1f 4508 a417 3bbc eee0 f187 681d  ..l.E...;.....h.
+000026a0: f69b 6151 535f e203 e280 f605 e993 7be4  ..aQS_........{.
+000026b0: 7b20 c39f fdae 10ea 008d db83 a0d5 8e0b  { ..............
+000026c0: c7d5 6f28 036a d59c 9310 fa1a 383f f96d  ..o(.j......8?.m
+000026d0: 7a4e 7e20 1715 abe9 4eb8 c7d3 6586 cff2  zN~ ....N...e...
+000026e0: 2756 f19d 9c9d acbe f0bd 762d 4486 cff2  'V........v-D...
+000026f0: bdaf 5534 f13e 58e3 ee2d 7432 7cd1 cef0  ..U4.>X..-t2|...
+00002700: 0cff bc5d 7c98 2d6f 8b38 9886 8b69 301e  ...]|.-o.8...i0.
+00002710: b124 9825 8b65 908c 6f16 cb65 310b e3f0  .$.%.e..o..e1...
+00002720: e6d7 60ff bc61 fbb4 eb32 4f61 aee7 56c0  ..`..a...2Oa..V.
+00002730: 8e32 7db0 7d88 0f67 5d86 0787 8e7e dba5  .2}.}..g]....~..
+00002740: 407b c87d 164f c28f 4914 06c5 288c 82f1  @{.}.O..I...(...
+00002750: 844e 83e9 6494 0445 12c5 cbc9 7871 9b14  .N..d..E....xq..
+00002760: c980 7bf2 ca2d 1592 28ea f69d 279f cc1d  ..{..-..(...'...
+00002770: 974c 7075 acd5 b142 432d 1409 8e7f 0882  .Lpu...BC-......
+00002780: 1c2b 41ce ff45 f933 0000 00ff ff03 0050  .+A..E.3.......P
+00002790: 4b03 0414 0006 0008 0000 0021 0045 c826  K..........!.E.&
+000027a0: 687f 1000 004e 3900 0014 0000 0078 6c2f  h....N9......xl/
+000027b0: 7368 6172 6564 5374 7269 6e67 732e 786d  sharedStrings.xm
+000027c0: 6cec 9b5d 6f5b c715 45df 0bf4 3f08 7c6f  l..]o[..E...?.|o
+000027d0: 64d9 719a 06b2 0296 6885 a07d 306c a679  d.q.....h..}0l.y
+000027e0: 7459 9ab1 8948 a44a d246 9c5f dfb3 d69e  tY...H.J.F._....
+000027f0: 2ba5 9c2b c479 a8e1 1496 2599 9c7b efcc  +..+.y....%..{..
+00002800: 99f3 b1f7 3e23 e9fc eb1f afaf 4ede ae76  ....>#......N..v
+00002810: fbf5 76f3 6472 f6d9 83c9 c96a b3dc be5c  ..v.dr.....j...\
+00002820: 6f5e 3d99 7c3b ffeb 1fbe 9c9c ec0f 8bcd  o^=.|;..........
+00002830: cbc5 d576 b37a 3279 b7da 4fbe bef8 fdef  ...v.z2y..O.....
+00002840: cef7 fbc3 493d bbd9 3f99 bc3e 1c6e be3a  ....I=..?..>.n.:
+00002850: 3ddd 2f5f afae 17fb cfb6 37ab 4d5d f97e  =./_......7.M].~
+00002860: bbbb 5e1c eaed eed5 e9fe 66b7 5abc dcbf  ..^.......f.Z...
+00002870: 5ead 0ed7 57a7 0f1f 3cf8 e2f4 7ab1 de4c  ^...W...<...z..L
+00002880: 4e96 db37 9bc3 93c9 e387 9f4f 4ede 6cd6  N..7.......ON.l.
+00002890: ff7e b39a 65e4 ecec 6c72 71be 5f5f 9c1f  .~..e...lrq.__..
+000028a0: 2e96 dbeb 9b5a 7c73 383f 3d5c 9c9f 3298  .....Z|s8?=\..2.
+000028b0: 0b6f 57cb c376 f7e2 f0ee 6675 7c69 bfaa  .oW..v....fu|i..
+000028c0: b936 cb6e 7c3e bf9c 5e4e e7b3 d93c 1fb3  .6.n|>..^N...<..
+000028d0: f9e5 acfe cda7 3556 2ff9 acaf e974 ca17  ......5V/....t..
+000028e0: 1fb3 597d d628 2fea c6cb 797d d62d 7cd5  ..Y}.(/...y}.-|.
+000028f0: 3853 4d6b c276 c374 56b3 f051 976a 9869  8SMk.v.tV..Q.j.i
+00002900: 6b4a e6e4 61ef f33f 67ab 25b9 5ad7 f89c  kJ..a..?g.%.Z...
+00002910: d6cc f5ad 1ee4 657d d54b 17e7 d97a d2a9  ......e}.K...z..
+00002920: bd43 7b30 88e7 6bc1 9a5e bbd9 82f3 69aa  .C{0..k..^....i.
+00002930: cbba a15a 9737 656a cd53 b7d7 3ab5 22b3  ...Z.7ej.S..:.".
+00002940: b095 da42 3dcf 0ade c1d2 d917 f6d7 dcd9  ...B=...........
+00002950: 34f7 d6dc 6545 bdf0 39e6 2903 eb5f 19ca  4...eE..9.).._..
+00002960: 37a7 6219 262a 43b8 e6bb 78bc 0de1 ebb8  7.b.&*C...x.....
+00002970: cbe1 5aa4 d6a8 3bf5 51f3 1a11 caea 3591  ..Z...;.Q.....5.
+00002980: 5ec4 9f38 9300 30c2 3658 a85e 0e4e ada5  ^..8..0.6X.^.N..
+00002990: 6a5c 3b30 870f a257 9313 31a2 5b3b c3b5  j\;0...W..1.[;..
+000029a0: fa28 7bc7 7758 89ff ca0b 1ac6 d453 6388  .({.wX.......Sc.
+000029b0: a1e4 4359 dc26 6479 b65b 1339 fb71 d2b5  ..CY.&dy.[.9.q..
+000029c0: 646a 31e1 5102 6c28 7112 3e64 63ed a59b  dj1.Q.l(q.>dc...
+000029d0: c061 26a3 7bf2 0af6 1032 763b 7c19 08b6  .a&.{....2v;|...
+000029e0: 8a01 44b3 26aa db2a 0558 c2ed 9274 f363  ..D.&..*.X...t.c
+000029f0: 8bb2 bfae 38f6 d3e9 3f8e 07ff 5525 fac3  ....8...?...U%..
+00002a00: d9f1 a899 4931 e03f fc68 6cc8 d0cb d109  ....I1.?.hl.....
+00002a10: 1e8e 8e7e 3e3a fab8 f31f 09ea 32ad fa0c  ...~>:......2...
+00002a20: f6c8 ae70 c0e5 6ccc fd84 4077 24f2 04d0  ...p..l...@w$...
+00002a30: f053 9356 3d29 61ad df5d 318d 1dae 8bd4  .S.V=)a..]1.....
+00002a40: 02b5 4a11 912e dc4f c452 9d29 89ca 24f3  ..J....O.R.)..$.
+00002a50: 9677 5643 8385 dccb 25f2 29a8 615e 053b  .wVC....%.).a^.;
+00002a60: 8873 f2dd 9ac5 a3e6 bd00 c045 13c1 eca1  .s.........E....
+00002a70: 22bc 4ac2 8b27 0003 654a b296 8514 8035  ".J..'..eJ.....5
+00002a80: 8969 c205 f727 75c9 1007 ad16 21a2 ac21  .i...'u.....!..!
+00002a90: 6504 34f2 1c2f 6334 890c c004 7598 10e7  e.4../c4....u...
+00002aa0: 64bf c61a ef09 688e f128 8699 8596 ade8  d.....h..(......
+00002ab0: 057a 9a96 c13f 2da1 f8ac 125c 1988 d174  .z...?-....\...t
+00002ac0: c2a0 e165 8358 a931 6213 68da 7095 172c  ...e.X.1b.h.p..,
+00002ad0: 4da9 6962 6c0f 74e4 8986 d06c 5ebf 970d  M.ibl.t....l^...
+00002ae0: 79cd ad3c c630 2365 8057 9807 c8c2 0203  y..<.0#e.W......
+00002af0: 3b60 3e35 2a9a 27e2 0637 b046 71e2 bad4  ;`>5*.'..7.Fq...
+00002b00: 5b5e e982 c145 d98a 884a 64a8 711c 6858  [^...E...Jd.q.hX
+00002b10: 8127 1607 3893 0fa6 6043 29ee 138a ad6a  .'..8...`C)....j
+00002b20: 5d4c ca94 6984 03e0 4c36 0170 be33 38c2  ]L..i...L6.p.38.
+00002b30: 37b8 1f14 cabe 8048 42e0 c3c2 bcef d8bc  7......HB.......
+00002b40: 1997 ac36 47d9 7e5c 2b80 6101 f90d 9692  ...6G.~\+.a.....
+00002b50: 48e6 053e 4bcc 4d34 78c6 a200 f500 5293  H..>K.M4x.....R.
+00002b60: b75e 6777 b899 ea20 82c2 25f7 9a10 240b  .^gw... ..%...$.
+00002b70: 1fcc 0e6a 8d62 c017 2345 4c78 283f c1c0  ...j.b..#ELx(?..
+00002b80: d401 7720 4b12 9d84 c0be 96cb 58e7 bb36  ..w K.......X..6
+00002b90: 2425 8388 ac7e c7f4 710b 9137 14e6 88a5  $%...~..q..7....
+00002ba0: 6396 609e 6ea1 8682 d941 7ddd 02eb ba11  c.`.n....A}.....
+00002bb0: c99e fd58 b1a3 fbf9 e3f1 6838 2888 227d  ...X......h8(."}
+00002bc0: 1900 2268 9988 e5ac 4d96 10d4 bc04 9288  .."h....M.......
+00002bd0: 6783 b372 4887 ec64 3521 93f3 8809 66c9  g..rH..d5!....f.
+00002be0: 4e95 2ea3 b63d 7a71 330e cf75 a103 7e76  N....=zq3..u..~v
+00002bf0: 2e9b b257 6090 4802 1aae 7b3c ff6e f5ea  ...W`.H...{<.n..
+00002c00: cdd5 6237 02e8 efc9 1b8f 3abf ddb3 7e30  ..b7......:...~0
+00002c10: cb42 b3ca e0c8 6ed9 9e1b a078 449a 6ca9  .B....n....xD.l.
+00002c20: 9c4a a02d edd9 0895 306f c8cf c20b 9498  .J.-....0o......
+00002c30: ebbf e0ea 04d9 ef82 7543 0361 7850 0451  ........uC.axP.Q
+00002c40: 0894 5e50 4eac 675e f043 d2b7 d244 fb60  ..^PN.g^.C...D.`
+00002c50: a762 4c99 9acc a10e 0518 834e 5802 8356  .bL........NX..V
+00002c60: 9bfb 135e cc3b b514 c14c 352a 8fd8 09d3  ...^.;...L5*....
+00002c70: 599f 9434 a8ae 8fea 4527 022c 0b35 a9bb  Y..4....E'.,.5..
+00002c80: 012b 944c 982a 5e39 11ca 29e0 80eb 826b  .+.L.*^9..)....k
+00002c90: ee27 6e8b 5c03 6458 54f1 eaae 28bc 4c48  .'n.\.dXT...(.LH
+00002ca0: c58a a2c2 9c53 45ae c96c ae39 402b 98a5  .....SE..l.9@+..
+00002cb0: fca5 4852 3702 bbb4 e13c 11bd 9227 55df  ..HR7....<...'U.
+00002cc0: 7c29 1837 4d29 0d18 002a 5c69 1c35 dd40  |).7M)...*\i.5.@
+00002cd0: 5bc9 2b44 8ac0 1a29 2d53 65ea b684 4c5e  [.+D...)-Se...L^
+00002ce0: c78c e87d 08d4 a251 6c66 ef8a 57b8 449d  ...}...Qlf..W.D.
+00002cf0: 198a 951f 0d8b 2a4d 991a 1f29 132c 6c14  ......*M...).,l.
+00002d00: 5f70 57ad 4188 8c3a 0923 beb2 cb00 87a9  _pW.A..:.#......
+00002d10: ad5c 906f c981 48e4 a07a 3470 52ce 482b  .\.o..H..z4pR.H+
+00002d20: 44c1 3df5 a71c 605c a4f7 b84b a40d a741  D.=...`\...K...A
+00002d30: e26c 25b2 06a3 1456 4d1d 8010 e48f ca29  .l%....VM......)
+00002d40: 1d4e 134e 41ce b080 c43b 0e4d 5ff6 e51f  .N.NA....;.M_...
+00002d50: 5514 226a 849e 1d8b f82d eda5 2abc 2dae  U."j.....-..*.-.
+00002d60: cb64 698c 3047 4a94 2a42 44e4 1dbb b8d3  .di.0GJ.*BD.....
+00002d70: cbb8 437e 3303 03f2 2801 5ca2 d201 31a4  ..C~3...(.\...1.
+00002d80: 6216 f533 0412 79d1 7239 3352 4e2a 29f5  b..3..y.r93RN*).
+00002d90: 7ec4 1dc9 456d 5960 a39a f5aa dada f5db  ~...EmY`........
+00002da0: f56e 71d5 1387 9253 0ad7 b510 60b0 38e9  .nq....S....`.8.
+00002db0: a5b0 6a59 8380 3196 2a57 d54c 944f 1aa4  ..jY..1.*W.L.O..
+00002dc0: d4b9 c163 2ac5 4e84 95e4 cc26 4d24 f233  ...c*.N....&M$.3
+00002dd0: b587 7050 560a 1ef8 0d7f a8c8 1035 283b  ..pPV........5(;
+00002de0: 6520 d2a4 5126 036c d4ff c95e 5518 5e81  e ..Q&.l...^U.^.
+00002df0: ac51 1ab0 1588 47e5 8a02 1dee 6605 f6a9  .Q....G.....f...
+00002e00: a651 0648 b720 0d83 61bb ff42 f3a6 5e28  .Q.H. ..a..B..^(
+00002e10: 27ac 0e05 aa41 e42f c1c1 aea9 ae2a 2ab0  '....A./.....**.
+00002e20: c5b2 566f 91ba bed5 bd43 0d6b 3e88 132d  ..Vo.....C.k>..-
+00002e30: 222f 07d5 b8d9 4c21 ebd8 5097 d10d 7914  "/....L!..P...y.
+00002e40: 7136 23f6 00d4 c020 e452 4a14 b70e 6126  q6#.... .RJ...a&
+00002e50: a193 0129 8138 9382 3c62 8eda 3af2 00f4  ...).8..<b..:...
+00002e60: 0023 f90a 8f74 60cd 5e15 8801 652b 4143  .#...t`.^...e+AC
+00002e70: 590d 0061 5af6 57ff baa4 c3c5 d050 d027  Y..aZ.W......P.'
+00002e80: 4239 4e65 5586 4d0b 118c a48b 2bd4 0451  B9NeU.M.....+..Q
+00002e90: a1b6 10b9 37a5 63c1 290e 23d9 9472 825a  ....7.c.).#..r.Z
+00002ea0: f614 0f35 bbc8 0d30 d85c 86e3 826d a094  ...5...0.\...m..
+00002eb0: 6568 d99b 9216 472b e724 8672 8511 7b18  eh....G+.$.r..{.
+00002ec0: 4039 025c bd36 c061 1464 aa39 3295 b5e4  @9.\.6.a.d.92...
+00002ed0: 46a3 6dbf 11cc 57f4 4a33 c965 d191 1ad2  F.m...W.J3.e....
+00002ee0: 7de6 1656 f116 4891 7989 276e 0fd5 0a1e  }..V..H.y.'n....
+00002ef0: 0d33 a920 f111 0735 09d1 2cc4 7c23 9275  .3. ...5..,.|#.u
+00002f00: a864 f200 a7c6 e36a 590a d2a2 6904 5a4b  .d.....jY...i.ZK
+00002f10: 86bf 453a f60c aeb5 cd20 9e62 a8ba 2dbb  ..E:..... .b..-.
+00002f20: 0f57 48cc 032c 6bef 20eb ba64 487a 0aee  .WH..,k. ..dHz..
+00002f30: b893 d410 811c 673b 44df 96ca 4c30 6e69  ......g;D...L0ni
+00002f40: 53d3 24f9 5ded 98ac c89e d856 0a1c b781  S.$.]......V....
+00002f50: 47ed 53b7 3529 8c0b d2fc 99f3 629d 5ac3  G.S.5)......b.Z.
+00002f60: 72e5 2d58 ab44 b31c 94e6 ce83 306a d532  r.-X.D......0j.2
+00002f70: 24d0 50b2 4d32 0c6c 24aa a137 fa63 1305  $.P.M2.l$..7.c..
+00002f80: 953b 8e2e 3244 c415 a291 e99a 7c0c 8e18  .;..2D......|...
+00002f90: 28bb 1f12 3751 48ac 0265 c14f 1ea4 7e30  (...7QH..e.O..~0
+00002fa0: 5cf9 208a 7a77 026e 7985 5a2c 336e 34cf  \. .zw.ny.Z,3n4.
+00002fb0: 4033 fa12 9506 feb3 b42c 9406 2566 a119  @3.......,..%f..
+00002fc0: 0a13 2429 e5ab 2c49 7ea6 418b 6b30 a55d  ..$)..,I~.A.k0.]
+00002fd0: 91c2 7902 0149 b152 725e 1d12 2ef3 7883  ..y..I.Rr^....x.
+00002fe0: 7d9e 6a49 2801 a5a1 0e11 421a 94af 23b2  }.jI(.....B...#.
+00002ff0: 22bd 1263 af85 a04c 9b70 8339 4a5e abae  "..c...L.p.9J^..
+00003000: 1bd2 c2bd a46f 5a2f c18e 9714 0459 0484  .....oZ/.....Y..
+00003010: eac5 56d1 be4d 9d04 d392 df7c 2713 4013  ..V..M.....|'.@.
+00003020: 2b43 af08 05c1 5ad9 5ad4 e948 883d 50c4  +C....Z.Z..H.=P.
+00003030: d103 c1b2 e402 db25 e9b2 07ae 134f 6b2e  .......%.....Ok.
+00003040: 0e6c 4822 2ca4 67f2 b426 a829 2834 1f07  .lH",.g..&.)(4..
+00003050: 2130 8f95 5871 4401 b192 ce57 ed9a f4c4  !0..XqD....W....
+00003060: 4db4 61ed 7af3 6bda 2652 4f4b 7ada 15c0  M.a.z.k.&ROKz...
+00003070: a352 f458 c769 642c bcd0 3dea b1e1 9fba  .R.X.id,..=.....
+00003080: ee14 add0 0815 9f91 0b38 8bb8 820a 8338  .........8.....8
+00003090: 11b3 c9a1 320d fcb2 aac6 fcdf b578 666f  ....2........xfo
+000030a0: 4042 2f0e 4963 6904 9323 0802 28b8 4d9a  @B/.Ici..#..(.M.
+000030b0: 90b5 7fd3 f222 07b5 0f3a 9727 0fc9 28f0  ....."...:.'..(.
+000030c0: 350e 55c5 c970 0480 0a17 bc92 db2a e430  5.U..p.......*.0
+000030d0: 2abc 61f9 dc73 7470 d69f 0f08 cfd4 a3bd  *.a..stp........
+000030e0: 9bd0 e86b caae 1ff4 b083 5b09 d6d0 44c2  ...k......[...D.
+000030f0: 1a0a ed32 4ce0 d048 0ca5 c02c f7f6 ddee  ...2L..H...,....
+00003100: 1925 c7ed 2106 609e 1a88 e5de 9739 2453  .%..!.`......9$S
+00003110: b526 2968 f6c9 a51a 65f1 a895 d5eb ad4b  .&)h....e......K
+00003120: 4195 a61d 83be c033 8b37 6f48 d7a6 736c  A......3.7oH..sl
+00003130: 41ed 953d 1e31 8f95 4271 2b54 e8f6 cd77  A..=.1..Bq+T...w
+00003140: d6c3 5694 1a1b 8cfc cb86 d474 11db ccd9  ..V........t....
+00003150: 00cf 8a0e 8b2a fe7c 9482 7123 b15f b1c2  .....*.|..q#._..
+00003160: 9412 7ef4 216a 5009 2bc3 df76 5e54 6cfa  ..~.!jP.+..v^Tl.
+00003170: 35c9 c3c6 c666 246a d030 4929 76bd 527b  5....f$j.0I)v.R{
+00003180: 33a6 f68f 0ca5 1a3d 9ab0 0764 9067 14d1  3......=...d.g..
+00003190: 6a5f 0145 fae5 0a4e 8b44 1072 c3ed 7a12  j_.E...N.D.r..z.
+000031a0: ce31 8262 bab2 3492 b83d a190 2471 7194  .1.b..4..=..$qq.
+000031b0: 6a44 0947 ba84 7072 e681 018e 4180 1826  jD.G..pr....A..&
+000031c0: 750e 468a 3079 7c68 9420 0012 13be 5041  u.F.0y|h. ....PA
+000031d0: 1066 6c80 72e8 cd10 f0ee 9b19 5b85 34ea  .fl.r.......[.4.
+000031e0: 1f7a 245b b828 1154 a81f c9c1 3c71 0be4  .z$[.(.T....<q..
+000031f0: 1497 023f f015 5c0f 99db 9798 83b2 a5ee  ...?..\.........
+00003200: e02e c206 8928 2208 6248 cf8e 4952 35a1  .....(".bH..IR5.
+00003210: 6510 3b26 c982 eac0 7e44 a4cd 68a4 62f6  e.;&....~D..h.b.
+00003220: 35b0 7c5a 1db3 4eb5 10c9 434d 8d1f c39e  5.|Z..N...CM....
+00003230: 7507 833c 2685 b6c2 044c 5b22 8bab ec49  u..<&....L["...I
+00003240: ad1b 5663 f921 d7c8 faf4 93b0 15b7 0dfc  ..Vc.!..........
+00003250: 95da 95dc c17b 332a 049e 3045 b35b fb96  .....{3*..0E.[..
+00003260: 01b2 474d 4210 93a0 4658 a630 5770 a82b  ..GMB...FX.0Wp.+
+00003270: 9350 1141 8284 442c 0ea5 d734 fdbc 823b  .P.A..D,...4...;
+00003280: 6d2c a871 c99c 1ae5 b3bd d187 c280 7d36  m,.q..........}6
+00003290: bb42 e284 cf24 31f5 be8f 2328 6c47 949e  .B...$1...#(lG..
+000032a0: 2494 9444 20d5 0d56 0f7e 52ac 027f fa0d  $..D ..V.~R.....
+000032b0: 3f78 0f65 c135 dfc5 e36d 085f 37a8 8b2c  ?x.e.5...m._7..,
+000032c0: b472 3d5f 1360 31a4 5d30 7350 4749 0bc0  .r=_.`1.]0sPGI..
+000032d0: 8621 4634 48f5 e9dd c20e 08e4 cc51 ca49  .!F4H........Q.I
+000032e0: 410a 4b35 675c d434 0cb8 9f56 7796 70c8  A.K5g\.4...Vw.p.
+000032f0: 5bfb a3ac 882f c543 367a eae7 be09 3833  [..../.C6z....83
+00003300: 7a50 301d 3ff3 39eb cf7c d3b6 9256 e49a  zP0.?.9..|...V..
+00003310: 9d7b 0310 b007 3834 6b02 aac3 4b41 37d9  .{....84k...KA7.
+00003320: e14d 2043 50d8 a266 1709 13d8 4541 262d  .M CP..f....EA&-
+00003330: 4cf0 db4a 4eee e205 2379 1b1d 776a 42d3  L..JN...#y..wjB.
+00003340: 6b84 6b6c c1e3 63a3 2028 29d1 5310 fa52  k.kl..c. ().S..R
+00003350: 3dc2 2e02 5444 586a 26fb d2a7 0803 91b5  =...TDXj&.......
+00003360: 1602 1257 a832 7adc a375 cd1b 3064 9022  ...W.2z..u..0d."
+00003370: 323a 8cd5 ba3e 3288 dc22 b9d2 2984 44f1  2:...>2.."..).D.
+00003380: 1a83 6e9c 1cbe 53fd 99db f40d 32b5 1c05  ..n...S.....2...
+00003390: 8fcc 5275 9a00 c394 5447 c8c6 bb83 3670  ..Ru....TG....6p
+000033a0: a6c8 127c b557 496a 6134 c61c 8b94 fd72  ...|.WIja4.....r
+000033b0: e427 cf12 b680 818f 435a d6b5 72e5 1704  .'......CZ..r...
+000033c0: 6fca 5ffe 4979 e372 092d 00a9 6010 8128  o._.Iy.r.-..`..(
+000033d0: 39d1 c4aa 80c9 dc56 2a56 94f2 a549 f6b3  9......V*V...I..
+000033e0: 4813 6de3 9882 9373 5cd4 7ecc 6e4e de53  H.m....s\.~.nN.S
+000033f0: e1dc a3e2 3bf5 9a66 0e83 1bae fe8f 4dee  ....;..f......M.
+00003400: 7f30 23b6 0356 663c e06e 5f64 23f0 514b  .0#..Vf<.n_d#.QK
+00003410: a120 1545 24e0 513a 8a18 8209 addb a658  . .E$.Q:.......X
+00003420: e869 b41d 0687 8461 6e46 3492 c5c2 be0a  .i.....anF4.....
+00003430: 2365 0fb5 889d e47f f283 ba32 f5ad b088  #e.........2....
+00003440: 5581 98c7 5ae6 7898 61b9 53d1 2166 db44  U...Z.x.a.S.!f.D
+00003450: bb70 0d02 5d22 7b6f cbc3 5a94 e994 9b72  .p..]"{o..Z....r
+00003460: 80aa 3d64 2000 927a f522 2526 8329 87f4  ..=d ..z."%&.)..
+00003470: 4004 3340 add1 91fc 96b3 30c1 a476 5408  @.3@......0..vT.
+00003480: 25b9 e1e3 521d 223c 7efe 04f5 32f5 c707  %...R."<~...2...
+00003490: f52a e434 e69e 8400 e754 831f 16cf 31a8  .*.4.....T....1.
+000034a0: 7cff 66b3 3cd4 ef11 1e8f af7e ac5f ffdb  |.f.<......~._..
+000034b0: f31b 865d cfda 9f5e 230a bbdb 723c f19e  ...]...^#...r<..
+000034c0: 7400 fc4b 7c7e 0f15 8068 e0b5 3a4f 7e48  t..K|~...h..:O~H
+000034d0: 9f27 3b2a 3544 7915 14c4 253e 5b77 a20c  .';*5Dy...%>[w..
+000034e0: 3ad4 3a43 3251 b476 cd76 0ae6 af27 520c  :.:C2Q.v.v...'R.
+000034f0: db7b 3395 e747 4aca 9fbd 54df 23cf 3273  .{3..GJ...T.#.2s
+00003500: d306 ea9a aad7 ee20 9f4d 58e0 808b 8864  ....... .MX....d
+00003510: 3f24 21c9 3b69 46c2 638a 5f2a 1d40 a894  ?$!.;iF.c._*.@..
+00003520: 92c7 e538 8c6b 3fa9 021f a213 c407 402e  ...8.k?.......@.
+00003530: e728 c297 dc2b 6b36 7dec e3dc c2f2 777a  .(...+k6}.....wz
+00003540: 37c2 5014 0af8 e268 65a4 a255 02f6 823d  7.P....he..U...=
+00003550: af6d 1d28 d804 aaf8 6bf3 95a1 d661 daab  .m.(....k....a..
+00003560: 29ec f826 8a0b 7dd8 087a f258 3079 0822  )..&..}..z.X0y."
+00003570: 16a9 6f3c d6a0 0d27 eeb5 7fa7 3255 4173  ..o<...'....2UAs
+00003580: e475 4e9c 083f 81b5 e09c ce37 3c8e 8f68  .uN..?.....7<..h
+00003590: 46f5 9ffa 2e6d 168e 8438 82e7 1199 9e3a  F....m...8.....:
+000035a0: c4c9 c81f aea1 b1ec b13d 9270 be34 7126  .........=.p.4q&
+000035b0: 949d 53d8 8667 ed33 8883 5e4b 32d8 f9db  ..S..g.3..^K2...
+000035c0: da67 0fd1 6d4a b1bb ce0a be8b 3d52 86ca  .g..mJ......=R..
+000035d0: 3b4d 9882 925a 55a9 b98b 74aa 6c8b 6cee  ;M...ZU...t.l.l.
+000035e0: 7f46 8567 e44d 2845 299d 8dd8 14ab 8c22  .F.g.M(E)......"
+000035f0: 77d3 a660 8981 9420 7516 1dd1 d080 1a89  w..`... u.......
+00003600: 96d6 ce06 9d95 b16d 0532 bef5 ceb5 1a7b  .......m.2.....{
+00003610: f51d 76d5 d214 03c7 3278 9c57 96f9 60c6  ..v.....2x.W..`.
+00003620: c88f a85a 79a7 7d44 76b3 baf3 7a36 df4a  ...Zy.}Dv...z6.J
+00003630: 3383 6efe 4eea 524e b84d 216d c34f 9930  3.n.N.RN.M!m.O.0
+00003640: 0731 e37f d02d e061 d316 616e 3121 c7ed  .1...-.a..an1!..
+00003650: 3465 7eed 4e8d 657d 96e5 4a3a fe56 6f99  4e~.N.e}..J:.Vo.
+00003660: 51f5 6d16 2ab7 6ca7 e6fd af9c c431 d126  Q.m.*.l......1.&
+00003670: 2244 047d 167d ff73 5e26 18f9 7d16 03a7  "D.}.}.s^&..}...
+00003680: fe15 0955 4029 044b d3a8 999b e682 18a5  ...U@).K........
+00003690: 6f1a def7 3f28 a4a1 191f 0d69 74d7 ee8e  o...?(.....it...
+000036a0: 37d2 3012 6c5b 3a85 f407 d0c2 2367 c882  7.0.l[:.....#g..
+000036b0: 1b7d 93dd 4a24 1241 0a3b d84b 29a0 6c4a  .}..J$.A.;.K).lJ
+000036c0: 3c87 2353 d28a a2bb e8ba 3879 2091 eb31  <.#S......8y ..1
+000036d0: ab31 8923 6c0d 9d73 1a56 72db 0ab6 6b6c  .1.#l..s.Vr...kl
+000036e0: cadb c650 7497 5e83 1d22 860d b4a9 2a9a  ...Pt.^.."....*.
+000036f0: 0bea 12c0 af94 be0a 4070 4724 41e4 465c  ........@pG$A.F\
+00003700: 0ae3 028a 1259 e51b 2a04 dc14 cc6e 113c  .....Y..*....n.<
+00003710: e736 f206 ecfd 780f 1309 1070 6609 1337  .6....x....pf..7
+00003720: 6ad6 5ecd e828 f555 d4c1 cfe6 f5d4 333c  j.^..(.U......3<
+00003730: 2873 c835 0254 1e27 3b3d c7b2 770c 5fe2  (s.5.T.';=..w._.
+00003740: 4a01 d15c 1062 3df7 f920 8789 69f1 d5ff  J..\.b=.. ..i...
+00003750: 9fda 1ac9 3cf4 0552 81e1 3680 1c40 7928  ....<..R..6..@y(
+00003760: f261 0f53 5583 9fda 1a51 e563 3bc1 4283  .a.SU....Q.c;.B.
+00003770: 80d1 d8c5 57df 8c84 fd03 0477 c750 f774  ....W......w.P.t
+00003780: 23e8 1b31 551d 06b0 4bda b5c6 f103 37df  #..1U...K.....7.
+00003790: ce5e 6c77 ebe3 e1c7 fffc 66fe ec78 f0d1  .^lw......f..x..
+000037a0: d8e0 dfb6 3f2d 7e78 71df 9f34 5def 368b  ....?-~xq..4].6.
+000037b0: ae77 8069 94bd 9ed1 616a c7c7 5188 f77e  .w.i....aj..Q..~
+000037c0: efa6 1cf1 039d 4ec7 aaf2 4bef 5cba 9d5e  ......N...K.\..^
+000037d0: 98e8 44f8 edff a163 ab40 8c44 f9ef 6351  ..D....c.@.D..cQ
+000037e0: 1e19 7cf6 bcfb 9b9c a7cf bf39 76e4 b367  ..|........9v..g
+000037f0: 7f39 1e5a 3e7d da37 8fab ddf5 7ab3 a83f  .9.Z>}.7....z..?
+00003800: 8feb e2d8 fd8a fad3 edd5 bbae 4178 beb8  ............Ax..
+00003810: e9d6 fef3 7efd 5d37 38dd 2fbb b1c3 6eb1  ....~.]78./...n.
+00003820: d92f 77eb 9bb1 e300 7839 27ad 4a26 aae8  ./w.....x9'.J&..
+00003830: b79f 00a7 f5f7 9017 ff01 0000 ffff 0300  ................
+00003840: 504b 0304 1400 0600 0800 0000 2100 1170  PK..........!..p
+00003850: bcd6 4001 0000 5102 0000 1100 0801 646f  ..@...Q.......do
+00003860: 6350 726f 7073 2f63 6f72 652e 786d 6c20  cProps/core.xml 
+00003870: a204 0128 a000 0100 0000 0000 0000 0000  ...(............
 00003880: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003890: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000038a0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000038b0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000038c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000038d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000038e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -913,38 +913,38 @@
 00003900: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003910: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003920: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003930: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003940: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003950: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003960: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003970: 0000 7c92 5f4b c330 14c5 df05 bf43 c97b  ..|._K.0.....C.{
-00003980: 9ba6 71fe 096d 072a 7b72 2058 517c 0bc9  ..q..m.*{r XQ|..
-00003990: dd56 6cd2 9044 bb7d 7bd3 76ab 1d88 8ff7  .Vl..D.}{.v.....
-000039a0: 9e93 df3d f792 7cb9 574d f40d d6d5 ad2e  ...=..|.WM......
-000039b0: 1049 5214 8116 adac f5b6 40af d52a be45  .IR.......@..*.E
-000039c0: 91f3 5c4b deb4 1a0a 7400 8796 e5e5 452e  ..\K....t.....E.
-000039d0: 0c13 ad85 67db 1ab0 be06 1705 9276 4c98  ....g........vL.
-000039e0: 02ed bc37 0c63 2776 a0b8 4b82 4307 71d3  ...7.c'v..K.C.q.
-000039f0: 5ac5 7d28 ed16 1b2e 3ef9 1670 96a6 d758  Z.}(....>..p...X
-00003a00: 81e7 927b 8e7b 606c 2622 3a22 a598 90e6  ...{.{`l&":"....
-00003a10: cb36 0340 0a0c 0d28 d0de 6192 10fc ebf5  .6.@...(..a.....
-00003a20: 6095 fbf3 c1a0 cc9c aaf6 0713 763a c69d  `...........v:..
-00003a30: b3a5 18c5 c9bd 77f5 64ec ba2e e9e8 1023  ......w.d......#
-00003a40: e427 f87d fdf4 32ac 1ad7 babf 9500 54e6  .'.}..2.......T.
-00003a50: 5230 6181 fbd6 9639 9e17 e170 0d77 7e1d  R0a....9...p.w~.
-00003a60: 6ebc a941 de1f 82fe 474f 8a21 ee08 0119  n..A....GO.!....
-00003a70: 8500 6c8c 7b52 dee8 c363 b542 657f c338  ..l.{R...c.Be..8
-00003a80: bd8b b3ac 2294 d11b b620 1ffd c8b3 f77d  ....".... .....}
-00003a90: a0b1 a18e 83ff 2566 3426 694c 4995 5176  ......%f4&iLI.Qv
-00003aa0: b560 7431 239e 0063 eef3 4f50 fe00 0000  .`t1#..c..OP....
-00003ab0: ffff 0300 504b 0304 1400 0600 0800 0000  ....PK..........
-00003ac0: 2100 5c4c 3a5b 9001 0000 4703 0000 1000  !.\L:[....G.....
-00003ad0: 0801 646f 6350 726f 7073 2f61 7070 2e78  ..docProps/app.x
-00003ae0: 6d6c 20a2 0401 28a0 0001 0000 0000 0000  ml ...(.........
+00003970: 0000 0000 0000 007c 925f 4bc3 3014 c5df  .......|._K.0...
+00003980: 05bf 43c9 7b9b a6dd 9c86 b603 953d 3910  ..C.{........=9.
+00003990: 9c28 be85 e46e 2b36 7f48 a2dd bebd 69bb  .(...n+6.H....i.
+000039a0: d50e c4c7 7bcf c9ef 9e7b 49b1 3cc8 26fa  ....{....{I.<.&.
+000039b0: 06eb 6aad 4a44 9214 45a0 b816 b5da 95e8  ..j.JD..E.......
+000039c0: 75b3 8a6f 51e4 3c53 8235 5a41 898e e0d0  u..oQ.<S.5ZA....
+000039d0: b2ba be2a b8a1 5c5b 78b6 da80 f535 b828  ...*..\[x....5.(
+000039e0: 9094 a3dc 9468 efbd a118 3bbe 07c9 5c12  .....h....;...\.
+000039f0: 1c2a 885b 6d25 f3a1 b43b 6c18 ff64 3bc0  .*.[m%...;l..d;.
+00003a00: 599a de60 099e 09e6 19ee 80b1 1989 e884  Y..`............
+00003a10: 147c 449a 2fdb f400 c131 3420 4179 8749  .|D./....14 Ay.I
+00003a20: 42f0 afd7 8395 eecf 07bd 3271 cada 1f4d  B.........2q...M
+00003a30: d8e9 1477 ca16 7c10 47f7 c1d5 a3b1 6ddb  ...w..|.G.....m.
+00003a40: a4cd fb18 213f c1ef eba7 977e d5b8 56dd  ....!?.....~..V.
+00003a50: ad38 a0aa 109c 720b cc6b 5b15 785a 84c3  .8....r..k[.xZ..
+00003a60: 35cc f975 b8f1 b606 717f 0cfa 1f3d c1fb  5..u....q....=..
+00003a70: b803 0444 1402 d021 ee59 79cb 1f1e 372b  ...D...!.Yy...7+
+00003a80: 5475 378c d3bb 38cb 3624 a7f9 82ce c947  Tu7...8.6$.....G
+00003a90: 37f2 e27d 1768 68c8 d3e0 7f89 d92c 4ee7  7..}.hh......,N.
+00003aa0: 3d31 a364 46d3 c584 7806 0cb9 2f3f 41f5  =1.dF...x.../?A.
+00003ab0: 0300 00ff ff03 0050 4b03 0414 0006 0008  .......PK.......
+00003ac0: 0000 0021 005c 4c3a 5b90 0100 0047 0300  ...!.\L:[....G..
+00003ad0: 0010 0008 0164 6f63 5072 6f70 732f 6170  .....docProps/ap
+00003ae0: 702e 786d 6c20 a204 0128 a000 0100 0000  p.xml ...(......
 00003af0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003b00: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003b10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003b20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003b30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003b40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003b50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -952,83 +952,83 @@
 00003b70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003b80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003b90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003ba0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003bb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003bc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003bd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00003be0: 0000 0000 0000 0000 0000 9c93 c16e db30  .............n.0
-00003bf0: 0c86 ef03 f60e 86ee 8d9c 6428 8640 5651  ..........d(.@VQ
-00003c00: a41b 7ad8 d000 497b d764 3a11 2a4b 82c4  ..z...I{.d:.*K..
-00003c10: 1849 9fbe b48d baca 36f4 d01b c99f f8f1  .I......6.......
-00003c20: 9194 c4cd a9b5 4507 3119 ef2a 369f 95ac  ......E.1..*6...
-00003c30: 00a7 7d6d dcbe 628f bb9f 57df 5991 50b9  ..}m..b...W.Y.P.
-00003c40: 5a59 efa0 6267 48ec 467e fd22 36d1 0788  ZY..bgH.F~."6...
-00003c50: 6820 1564 e152 c50e 8861 c579 d207 6855  h .d.R...a.y..hU
-00003c60: 9a91 ec48 697c 6c15 521a f7dc 378d d170  ...Hi|l.R...7..p
-00003c70: e7f5 b105 877c 5196 d71c 4e08 ae86 fa2a  .....|Q...N....*
-00003c80: 4c86 6c74 5c75 f859 d3da eb9e 2f3d edce  L.lt\u.Y..../=..
-00003c90: 8180 a5b8 0dc1 1aad 90a6 94bf 8d8e 3ef9  ..............>.
-00003ca0: 068b 1f27 0d56 f05c 1444 b705 7d8c 06cf  ...'.V.\.D..}...
-00003cb0: b214 3c4f c556 2b0b 6b32 968d b209 047f  ..<O.V+.k2......
-00003cc0: 2f88 7b50 fdd2 36ca c424 4587 ab0e 34fa  /.{P..6..$E...4.
-00003cd0: 5824 f342 6b5b b0e2 8f4a d0e3 54ac 53d1  X$.Bk[...J..T.S.
-00003ce0: 2887 84d5 b78d c910 db90 30ca dbf8 7c4c  (.........0...|L
-00003cf0: 2fe4 4eea 5819 c2bc 318f cd37 b91c 1a28  /.N.X...1..7...(
-00003d00: b86c ec0d 460a 122e f976 062d a487 66a3  .l..F....v.-..f.
-00003d10: 22fe 0777 99e3 0e0c 236c 0e38 cf01 27d4  "..w....#l.8..'.
-00003d20: 117e f181 36c2 e683 0d8b 22c4 bfa0 d6be  .~..6.....".....
-00003d30: 0dca 9d49 98a2 5fc6 3da7 c7b0 f377 0ae1  ...I.._.=....w..
-00003d40: ed08 9745 b13d a808 35dd 6d3a d254 10f7  ...E.=..5.m:.T..
-00003d50: b4ff 687b 93f5 41b9 3dd4 6f3d ff0a fd93  ..h{..A.=.o=....
-00003d60: 791a ff85 9c5f cfca 6549 af21 ab09 fefe  y...._..eI.!....
-00003d70: 03e4 2b00 0000 ffff 0300 504b 0102 2d00  ..+.......PK..-.
-00003d80: 1400 0600 0800 0000 2100 7c6c 9816 6901  ........!.|l..i.
-00003d90: 0000 a005 0000 1300 0000 0000 0000 0000  ................
-00003da0: 0000 0000 0000 0000 5b43 6f6e 7465 6e74  ........[Content
-00003db0: 5f54 7970 6573 5d2e 786d 6c50 4b01 022d  _Types].xmlPK..-
-00003dc0: 0014 0006 0008 0000 0021 00b5 5530 23f4  .........!..U0#.
-00003dd0: 0000 004c 0200 000b 0000 0000 0000 0000  ...L............
-00003de0: 0000 0000 00a2 0300 005f 7265 6c73 2f2e  ........._rels/.
-00003df0: 7265 6c73 504b 0102 2d00 1400 0600 0800  relsPK..-.......
-00003e00: 0000 2100 63a7 289a df02 0000 1207 0000  ..!.c.(.........
-00003e10: 0f00 0000 0000 0000 0000 0000 0000 c706  ................
-00003e20: 0000 786c 2f77 6f72 6b62 6f6f 6b2e 786d  ..xl/workbook.xm
-00003e30: 6c50 4b01 022d 0014 0006 0008 0000 0021  lPK..-.........!
-00003e40: 00de 09fd 2802 0100 00d4 0300 001a 0000  ....(...........
-00003e50: 0000 0000 0000 0000 0000 00d3 0900 0078  ...............x
-00003e60: 6c2f 5f72 656c 732f 776f 726b 626f 6f6b  l/_rels/workbook
-00003e70: 2e78 6d6c 2e72 656c 7350 4b01 022d 0014  .xml.relsPK..-..
-00003e80: 0006 0008 0000 0021 008f 560f 0d0c 0d00  .......!..V.....
-00003e90: 0085 5e00 0018 0000 0000 0000 0000 0000  ..^.............
-00003ea0: 0000 0015 0c00 0078 6c2f 776f 726b 7368  .......xl/worksh
-00003eb0: 6565 7473 2f73 6865 6574 312e 786d 6c50  eets/sheet1.xmlP
-00003ec0: 4b01 022d 0014 0006 0008 0000 0021 0063  K..-.........!.c
-00003ed0: fdce 8f11 0200 00f3 0300 0018 0000 0000  ................
-00003ee0: 0000 0000 0000 0000 0057 1900 0078 6c2f  .........W...xl/
-00003ef0: 776f 726b 7368 6565 7473 2f73 6865 6574  worksheets/sheet
-00003f00: 322e 786d 6c50 4b01 022d 0014 0006 0008  2.xmlPK..-......
-00003f10: 0000 0021 009c 73ee 7814 0200 00f3 0300  ...!..s.x.......
-00003f20: 0018 0000 0000 0000 0000 0000 0000 009e  ................
-00003f30: 1b00 0078 6c2f 776f 726b 7368 6565 7473  ...xl/worksheets
-00003f40: 2f73 6865 6574 332e 786d 6c50 4b01 022d  /sheet3.xmlPK..-
-00003f50: 0014 0006 0008 0000 0021 00f8 a6e9 a88a  .........!......
-00003f60: 0600 00ec 1b00 0013 0000 0000 0000 0000  ................
-00003f70: 0000 0000 00e8 1d00 0078 6c2f 7468 656d  .........xl/them
-00003f80: 652f 7468 656d 6531 2e78 6d6c 504b 0102  e/theme1.xmlPK..
-00003f90: 2d00 1400 0600 0800 0000 2100 1e63 f513  -.........!..c..
-00003fa0: bc02 0000 d106 0000 0d00 0000 0000 0000  ................
-00003fb0: 0000 0000 0000 a324 0000 786c 2f73 7479  .......$..xl/sty
-00003fc0: 6c65 732e 786d 6c50 4b01 022d 0014 0006  les.xmlPK..-....
-00003fd0: 0008 0000 0021 0045 c826 687f 1000 004e  .....!.E.&h....N
-00003fe0: 3900 0014 0000 0000 0000 0000 0000 0000  9...............
-00003ff0: 008a 2700 0078 6c2f 7368 6172 6564 5374  ..'..xl/sharedSt
-00004000: 7269 6e67 732e 786d 6c50 4b01 022d 0014  rings.xmlPK..-..
-00004010: 0006 0008 0000 0021 00eb 239e 3242 0100  .......!..#.2B..
-00004020: 0051 0200 0011 0000 0000 0000 0000 0000  .Q..............
-00004030: 0000 003b 3800 0064 6f63 5072 6f70 732f  ...;8..docProps/
-00004040: 636f 7265 2e78 6d6c 504b 0102 2d00 1400  core.xmlPK..-...
-00004050: 0600 0800 0000 2100 5c4c 3a5b 9001 0000  ......!.\L:[....
-00004060: 4703 0000 1000 0000 0000 0000 0000 0000  G...............
-00004070: 0000 b43a 0000 646f 6350 726f 7073 2f61  ...:..docProps/a
-00004080: 7070 2e78 6d6c 504b 0506 0000 0000 0c00  pp.xmlPK........
-00004090: 0c00 0c03 0000 7a3d 0000 0000            ......z=....
+00003be0: 0000 0000 0000 0000 0000 0000 009c 93c1  ................
+00003bf0: 6edb 300c 86ef 03f6 0e86 ee8d 9c64 2886  n.0..........d(.
+00003c00: 4056 51a4 1b7a d8d0 0049 7bd7 643a 112a  @VQ..z...I{.d:.*
+00003c10: 4b82 c418 499f beb4 8dba ca36 f4d0 1bc9  K...I......6....
+00003c20: 9ff8 f191 94c4 cda9 b545 0731 19ef 2a36  .........E.1..*6
+00003c30: 9f95 ac00 a77d 6ddc be62 8fbb 9f57 df59  .....}m..b...W.Y
+00003c40: 9150 b95a 59ef a062 6748 ec46 7efd 2236  .P.ZY..bgH.F~."6
+00003c50: d107 8868 2015 64e1 52c5 0e88 61c5 79d2  ...h .d.R...a.y.
+00003c60: 0768 559a 91ec 4869 7c6c 1552 1af7 dc37  .hU...Hi|l.R...7
+00003c70: 8dd1 70e7 f5b1 0587 7c51 96d7 1c4e 08ae  ..p.....|Q...N..
+00003c80: 86fa 2a4c 866c 745c 75f8 59d3 daeb 9e2f  ..*L.lt\u.Y..../
+00003c90: 3ded ce81 80a5 b80d c11a ad90 a694 bf8d  =...............
+00003ca0: 8e3e f906 8b1f 270d 56f0 5c14 44b7 057d  .>....'.V.\.D..}
+00003cb0: 8c06 cfb2 143c 4fc5 562b 0b6b 3296 8db2  .....<O.V+.k2...
+00003cc0: 0904 7f2f 887b 50fd d236 cac4 2445 87ab  .../.{P..6..$E..
+00003cd0: 0e34 fa58 24f3 426b 5bb0 e28f 4ad0 e354  .4.X$.Bk[...J..T
+00003ce0: ac53 d128 8784 d5b7 8dc9 10db 9030 cadb  .S.(.........0..
+00003cf0: f87c 4c2f e44e ea58 19c2 bc31 8fcd 37b9  .|L/.N.X...1..7.
+00003d00: 1c1a 28b8 6cec 0d46 0a12 2ef9 7606 2da4  ..(.l..F....v.-.
+00003d10: 8766 a322 fe07 7799 e30e 0c23 6c0e 38cf  .f."..w....#l.8.
+00003d20: 0127 d411 7ef1 8136 c2e6 830d 8b22 c4bf  .'..~..6....."..
+00003d30: a0d6 be0d ca9d 4998 a25f c63d a7c7 b0f3  ......I.._.=....
+00003d40: 770a e1ed 0897 45b1 3da8 0835 dd6d 3ad2  w.....E.=..5.m:.
+00003d50: 5410 f7b4 ff68 7b93 f541 b93d d46f 3dff  T....h{..A.=.o=.
+00003d60: 0afd 9379 1aff 859c 5fcf ca65 49af 21ab  ...y...._..eI.!.
+00003d70: 09fe fe03 e42b 0000 00ff ff03 0050 4b01  .....+.......PK.
+00003d80: 022d 0014 0006 0008 0000 0021 007c 6c98  .-.........!.|l.
+00003d90: 1669 0100 00a0 0500 0013 0000 0000 0000  .i..............
+00003da0: 0000 0000 0000 0000 0000 005b 436f 6e74  ...........[Cont
+00003db0: 656e 745f 5479 7065 735d 2e78 6d6c 504b  ent_Types].xmlPK
+00003dc0: 0102 2d00 1400 0600 0800 0000 2100 b555  ..-.........!..U
+00003dd0: 3023 f400 0000 4c02 0000 0b00 0000 0000  0#....L.........
+00003de0: 0000 0000 0000 0000 a203 0000 5f72 656c  ............_rel
+00003df0: 732f 2e72 656c 7350 4b01 022d 0014 0006  s/.relsPK..-....
+00003e00: 0008 0000 0021 006a 4a1c bfe1 0200 0012  .....!.jJ.......
+00003e10: 0700 000f 0000 0000 0000 0000 0000 0000  ................
+00003e20: 00c7 0600 0078 6c2f 776f 726b 626f 6f6b  .....xl/workbook
+00003e30: 2e78 6d6c 504b 0102 2d00 1400 0600 0800  .xmlPK..-.......
+00003e40: 0000 2100 de09 fd28 0201 0000 d403 0000  ..!....(........
+00003e50: 1a00 0000 0000 0000 0000 0000 0000 d509  ................
+00003e60: 0000 786c 2f5f 7265 6c73 2f77 6f72 6b62  ..xl/_rels/workb
+00003e70: 6f6f 6b2e 786d 6c2e 7265 6c73 504b 0102  ook.xml.relsPK..
+00003e80: 2d00 1400 0600 0800 0000 2100 4f17 4331  -.........!.O.C1
+00003e90: 0f0d 0000 835e 0000 1800 0000 0000 0000  .....^..........
+00003ea0: 0000 0000 0000 170c 0000 786c 2f77 6f72  ..........xl/wor
+00003eb0: 6b73 6865 6574 732f 7368 6565 7431 2e78  ksheets/sheet1.x
+00003ec0: 6d6c 504b 0102 2d00 1400 0600 0800 0000  mlPK..-.........
+00003ed0: 2100 63fd ce8f 1102 0000 f303 0000 1800  !.c.............
+00003ee0: 0000 0000 0000 0000 0000 0000 5c19 0000  ............\...
+00003ef0: 786c 2f77 6f72 6b73 6865 6574 732f 7368  xl/worksheets/sh
+00003f00: 6565 7432 2e78 6d6c 504b 0102 2d00 1400  eet2.xmlPK..-...
+00003f10: 0600 0800 0000 2100 9c73 ee78 1402 0000  ......!..s.x....
+00003f20: f303 0000 1800 0000 0000 0000 0000 0000  ................
+00003f30: 0000 a31b 0000 786c 2f77 6f72 6b73 6865  ......xl/workshe
+00003f40: 6574 732f 7368 6565 7433 2e78 6d6c 504b  ets/sheet3.xmlPK
+00003f50: 0102 2d00 1400 0600 0800 0000 2100 f8a6  ..-.........!...
+00003f60: e9a8 8a06 0000 ec1b 0000 1300 0000 0000  ................
+00003f70: 0000 0000 0000 0000 ed1d 0000 786c 2f74  ............xl/t
+00003f80: 6865 6d65 2f74 6865 6d65 312e 786d 6c50  heme/theme1.xmlP
+00003f90: 4b01 022d 0014 0006 0008 0000 0021 001e  K..-.........!..
+00003fa0: 63f5 13bc 0200 00d1 0600 000d 0000 0000  c...............
+00003fb0: 0000 0000 0000 0000 00a8 2400 0078 6c2f  ..........$..xl/
+00003fc0: 7374 796c 6573 2e78 6d6c 504b 0102 2d00  styles.xmlPK..-.
+00003fd0: 1400 0600 0800 0000 2100 45c8 2668 7f10  ........!.E.&h..
+00003fe0: 0000 4e39 0000 1400 0000 0000 0000 0000  ..N9............
+00003ff0: 0000 0000 8f27 0000 786c 2f73 6861 7265  .....'..xl/share
+00004000: 6453 7472 696e 6773 2e78 6d6c 504b 0102  dStrings.xmlPK..
+00004010: 2d00 1400 0600 0800 0000 2100 1170 bcd6  -.........!..p..
+00004020: 4001 0000 5102 0000 1100 0000 0000 0000  @...Q...........
+00004030: 0000 0000 0000 4038 0000 646f 6350 726f  ......@8..docPro
+00004040: 7073 2f63 6f72 652e 786d 6c50 4b01 022d  ps/core.xmlPK..-
+00004050: 0014 0006 0008 0000 0021 005c 4c3a 5b90  .........!.\L:[.
+00004060: 0100 0047 0300 0010 0000 0000 0000 0000  ...G............
+00004070: 0000 0000 00b7 3a00 0064 6f63 5072 6f70  ......:..docProp
+00004080: 732f 6170 702e 786d 6c50 4b05 0600 0000  s/app.xmlPK.....
+00004090: 000c 000c 000c 0300 007d 3d00 0000 00    .........}=....
```

### Comparing `JBioSeqTools-2.0.3/jbst/install.py` & `JBioSeqTools-2.0.4/jbst/install.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 import platform
 import os
 from ftplib import FTP
 pd.options.mode.chained_assignment = None
 import warnings
 import json
 import subprocess
+import gdown
+
 
 warnings.filterwarnings("ignore")
 
 
  #       _  ____   _         _____              _                      __ _____  __  
  #      | ||  _ \ (_)       / ____|            | |                    / /|  __ \ \ \ 
  #      | || |_) | _   ___ | (___   _   _  ___ | |_  ___  _ __ ___   | | | |__) | | |
@@ -46,42 +48,45 @@
         os.makedirs(os.path.join(source, 'tmp'))
         
         
 
 def download_and_prepare_UTRs(source = None, min_size = 50):
     
  
-    
-    import urllib
     import gzip
     import shutil
     
     if source == None:
         source = os.getcwd()
         
-    url = 'http://srv00.recas.ba.infn.it/webshare/utrdb/Homo_sapiens.GRCh38.107.utrs.gz'
+
 
     local_filename = 'Homo_sapiens.GRCh38.107.utrs.gz'
     
     local_filename = os.path.join(source, local_filename)
     
+    
+    url = 'https://drive.google.com/uc?id=1lMKGwNvHjAPE16xjSjSeb8NlH78hnREO'
+    
     # Download 
-    urllib.request.urlretrieve(url, local_filename)
+    gdown.download(url, local_filename, quiet=False)
+
     
     # Unzip 
     
     file_path = 'Homo_sapiens.GRCh38.107.utrs'
     
     file_path = os.path.join(source, file_path)
     
     with gzip.open(local_filename, 'rb') as f_in:
         with open(file_path, 'wb') as f_out:
             shutil.copyfileobj(f_in, f_out)
     
 
+
     
     def read_fasta(file_path):
      headers = []
      sequences = []
  
      with open(file_path, 'r') as fasta_file:
          current_header = None
@@ -296,16 +301,16 @@
     
 
 
 
 
 def install_muscle(source = None):
 
-    windows = 'https://drive5.com/muscle/downloads3.8.31/muscle3.8.31_i86win32.exe'
-    linux = 'https://drive5.com/muscle/muscle_src_3.8.1551.tar.gz'
+    windows = 'https://drive.google.com/uc?id=1u-wqA2e2cqSLjY1JzpYqNUYmAX6zp8fl'
+    linux = 'https://drive.google.com/uc?id=1ZHP_bB7iTRZ8-73TsDrNLxIcQoPrvTLF'
     
     
     system = platform.system()
     
     if source == None:
         source = os.getcwd()
         
@@ -316,41 +321,31 @@
         print("\nWindows operating system")
         muscle_executable = os.path.join(source, 'muscle/windows/muscle3.8.31_i86win32.exe')
         
         if not os.path.exists(os.path.join(source, 'muscle/windows')):
             os.makedirs(os.path.join(source, 'muscle/windows'))
 
         
-        # Download the file
-        response = requests.get(windows)
-        if response.status_code == 200:
-            with open(muscle_executable, 'wb') as f:
-                f.write(response.content)
-        else:
-            print(f"\nFailed to download the file. HTTP status code: {response.status_code}")
-            exit(1)
+        # Download 
+        gdown.download(windows, muscle_executable, quiet=False)
+        
         
 
 
     elif system == "Linux":
         print("\nLinux operating system")
         muscle_executable = os.path.join(source, 'muscle/linux/muscle_src_3.8.1551.tar.gz')
                 
         if not os.path.exists(os.path.join(source, 'muscle/linux')):
             os.makedirs(os.path.join(source, 'muscle/linux'))
 
         
-        # Download the file
-        response = requests.get(linux)
-        if response.status_code == 200:
-            with open(muscle_executable, 'wb') as f:
-                f.write(response.content)
-        else:
-            print(f"\nFailed to download the file. HTTP status code: {response.status_code}")
-            exit(1)
+        # Download 
+        gdown.download(linux, muscle_executable, quiet=False)
+        
             
         with tarfile.open(muscle_executable, 'r:gz') as tar:
             tar.extractall(path=os.path.join(source, 'muscle/linux/'))
             
 
         # Clean up: remove the downloaded archive file
         os.remove(muscle_executable)
@@ -361,16 +356,17 @@
     
         subprocess.run(command_list, cwd=make_path)
 
  
 
 def install_blast(source = None):
     
-    windows = 'https://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/2.14.1/ncbi-blast-2.14.1+-x64-win64.tar.gz'
-    linux = 'https://ftp.ncbi.nlm.nih.gov/blast/executables/blast+/2.14.1/ncbi-blast-2.14.1+-x64-linux.tar.gz'
+    
+    windows = 'https://drive.google.com/uc?id=1yRw1kWE6UBARHvWJG4oycMT_4fnahvFt'
+    linux = 'https://drive.google.com/uc?id=1EaBPPWuElsrm89-dusAomm0Gq6Php4f6'
     
     
     system = platform.system()
     
     if source == None:
         source = os.getcwd()
         
@@ -382,46 +378,34 @@
         blast = os.path.join(source, 'blast/windows/ncbi-blast-2.14.1+-x64-win64.tar.gz')
         
         if not os.path.exists(os.path.join(source, 'blast/windows')):
             os.makedirs(os.path.join(source, 'blast/windows'))
 
         
         # Download the file
-        response = requests.get(windows)
-        if response.status_code == 200:
-            with open(blast, 'wb') as f:
-                f.write(response.content)
-        else:
-            print(f"\nFailed to download the file. HTTP status code: {response.status_code}")
-            exit(1)
+        gdown.download(windows, blast, quiet=False)
+
             
         with tarfile.open(blast, 'r:gz') as tar:
             tar.extractall(path=os.path.join(source, 'blast/windows/'))
             
 
         # Clean up: remove the downloaded archive file
         os.remove(blast)
 
     elif system == "Linux":
         print("\nLinux operating system")
         blast = os.path.join(source, 'blast/linux/ncbi-blast-2.14.1+-x64-linux.tar.gz')
         
         if not os.path.exists(os.path.join(source, 'blast/linux')):
             os.makedirs(os.path.join(source, 'blast/linux'))
-
         
         # Download the file
-        response = requests.get(linux)
-        if response.status_code == 200:
-            with open(blast, 'wb') as f:
-                f.write(response.content)
-        else:
-            print(f"\nFailed to download the file. HTTP status code: {response.status_code}")
-            exit(1)
-            
+        gdown.download(linux, blast, quiet=False)
+          
         with tarfile.open(blast, 'r:gz') as tar:
             tar.extractall(path=os.path.join(source, 'blast/linux/'))
             
 
         # Clean up: remove the downloaded archive file
         os.remove(blast)
```

### Comparing `JBioSeqTools-2.0.3/jbst/seq_tools.py` & `JBioSeqTools-2.0.4/jbst/seq_tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,17 @@
 import random
 import string
 from collections import Counter
 import xml.etree.ElementTree as ET
 import warnings
 import json
 import time
+import random
 
+random.seed(42)
 
  #       _  ____   _         _____              _                      __ _____  __  
  #      | ||  _ \ (_)       / ____|            | |                    / /|  __ \ \ \ 
  #      | || |_) | _   ___ | (___   _   _  ___ | |_  ___  _ __ ___   | | | |__) | | |
  #  _   | ||  _ < | | / _ \ \___ \ | | | |/ __|| __|/ _ \| '_ ` _ \  | | |  _  /  | |
  # | |__| || |_) || || (_) |____) || |_| |\__ \| |_|  __/| | | | | | | | | | \ \  | |
  #  \____/ |____/ |_| \___/|_____/  \__, ||___/ \__|\___||_| |_| |_|  \_\|_|  \_\/_/
@@ -2078,35 +2080,34 @@
     Returns:
         DataFrame: Data frame containing the restriction places and position of its occurrence in the provided genetic sequence
         DataFrame: Data frame containing the parsed information about restriction places and their indexes to mapping to the first DataFrame
 
     """
     
     try:
-        
+   
         restriction = metadata['restriction']
         
         enzyme_restriction = {'name':[], 'restriction_place':[], 'restriction_sequence':[], 'start':[], 'stop':[]}
         
+        #repaired :D
+        bmp = list(sequence.upper())
         for r in tqdm(restriction.index):
-            check = True
             if restriction['sequence'][r] in sequence.upper():
-                while(check == True):
-                    bmp = list(sequence.upper())
-                    for n in range(0,len(restriction['sequence'][r])):
-                        for j in range(n,len(bmp)-len(restriction['sequence'][r])):
-                           lower = j
-                           upper = j + len(restriction['sequence'][r])
-                           if upper < len(bmp) and ''.join(bmp[lower:upper]) == restriction['sequence'][r]:
-                                enzyme_restriction['name'].append(restriction['name'][r])
-                                enzyme_restriction['restriction_sequence'].append(restriction['sequence'][r])
-                                enzyme_restriction['restriction_place'].append(restriction['restriction_place'][r])
-                                enzyme_restriction['start'].append(lower)
-                                enzyme_restriction['stop'].append(upper)
-                                check = False
+                for n in range(0,len(restriction['sequence'][r])):
+                    for j in range(n,len(bmp), len(restriction['sequence'][r])):
+                       lower = j                       
+                       upper = j + len(restriction['sequence'][r])
+                       if upper < len(bmp) and ''.join(bmp[lower:upper]) == restriction['sequence'][r]:
+                            enzyme_restriction['name'].append(restriction['name'][r])
+                            enzyme_restriction['restriction_sequence'].append(restriction['sequence'][r])
+                            enzyme_restriction['restriction_place'].append(restriction['restriction_place'][r])
+                            enzyme_restriction['start'].append(lower)
+                            enzyme_restriction['stop'].append(upper)
+                            
     
                                    
         enzyme_restriction = pd.DataFrame.from_dict(enzyme_restriction)
         enzyme_restriction = enzyme_restriction.drop_duplicates()
         enzyme_restriction = enzyme_restriction.reset_index(drop=True)
         
         if len(enzyme_restriction['name']) > 0:
@@ -2258,36 +2259,18 @@
             print('\nRestriction places for:')
             for i in not_repaired:
                 print('\n'+ str(i))
                 
             print('\nwere unable to optimize:')
             print('\nRest of chosen restriction places in the sequence has repaired...')
     
-    
-        enzyme_restriction = {'name':[], 'restriction_place':[], 'restriction_sequence':[], 'sequence':[], 'start':[], 'stop':[]}
-        
+            
         print('\nChecking the new restriction places...')
-        for r in tqdm(restriction.index):
-            check = True
-            if restriction['sequence'][r] in final_sequence:
-                while(check == True):
-                    bmp = list(final_sequence.upper())
-                    for n in range(0,len(restriction['sequence'][r])):
-                        for j in range(n,len(bmp)-len(restriction['sequence'][r])):
-                           lower = j
-                           upper = j + len(restriction['sequence'][r])
-                           if upper < len(bmp) and ''.join(bmp[lower:upper]) == restriction['sequence'][r]:
-                                enzyme_restriction['name'].append(restriction['name'][r])
-                                enzyme_restriction['restriction_sequence'].append(restriction['sequence'][r])
-                                enzyme_restriction['restriction_place'].append(restriction['restriction_place'][r])
-                                enzyme_restriction['sequence'].append(final_sequence)
-                                enzyme_restriction['start'].append(lower)
-                                enzyme_restriction['stop'].append(upper)
-                                check = False
-    
+        
+        enzyme_restriction = check_restriction(final_sequence, metadata)
                                    
         enzyme_restriction = pd.DataFrame.from_dict(enzyme_restriction)
         enzyme_restriction = enzyme_restriction.drop_duplicates()
         enzyme_restriction = enzyme_restriction.reset_index(drop=True)
         enzyme_restriction = enzyme_restriction[~enzyme_restriction['name'].isin(restriction_df['name'])]
         
         if len(enzyme_restriction['name']) > 0:
```

### Comparing `JBioSeqTools-2.0.3/jbst/tests/fasta_vector_test.fasta` & `JBioSeqTools-2.0.4/jbst/tests/fasta_vector_test.fasta`

 * *Files identical despite different names*

### Comparing `JBioSeqTools-2.0.3/jbst/tests/jseq_tests.py` & `JBioSeqTools-2.0.4/jbst/tests/jseq_tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,26 +21,37 @@
 metadata = load_metadata() 
 
 
 def test_vectors(tests_dictonaries, tests_dictonaries_names, non, metadata, show_plot = True):
     passed = []
     errored = []
     
+    fail = False
     for l, i in enumerate(tests_dictonaries):
+        if fail:
+            break
         for n, di in enumerate(tqdm(tests_dictonaries[l])):
             try:
                 project = vector_create_on_dict(metadata, di, show_plot = show_plot)
                 if project == None and tests_dictonaries_names[l][n] not in non:
                     errored.append(tests_dictonaries_names[l][n])
+                    print(f'\n\nTest id:{str(tests_dictonaries_names[l][n])} not passed!')
+                    print('Further testing interrupted!\nCheck if all dependencies was installed properly during first run!\nCheck the internet connection!\nIf all should be ok, contact us!')
+                    fail = True
+                    break
+                
                 else:
                     passed.append(tests_dictonaries_names[l][n])
                 
             except:
                 errored.append(tests_dictonaries_names[l][n])
                 
+    if len(errored) == 0: 
+        print('All tests passed successfully!')
+                
     return passed, errored
 
 
 input_dict_expression_1 = {
 'project_name':'test',
 'vector_type':'ssAAV',
 'vector_function':'expression',
@@ -4943,15 +4954,15 @@
                            'input_dict_transcript_rnai_4', 'input_dict_transcript_rnai_5', 'input_dict_transcript_rnai_6',
                            'input_dict_transcript_rnai_7', 'input_dict_transcript_rnai_8', 'input_dict_transcript_rnai_9',
                            'input_dict_mrna_1', 'input_dict_mrna_2','input_dict_mrna_3', 'input_dict_mrna_4', 'input_dict_mrna_5',
                            'input_dict_mrna_6']
 
 
 
-tests_dictonaries = [test_expression_list, test_rnai_list, test_transcription_list]
+tests_dictonaries = [test_rnai_list, test_transcription_list, test_expression_list]
 
 tests_dictonaries_names = [test_expression_list_names, test_rnai_list_names, test_transcription_list_names]
 
 non = ['input_dict_expression_333', 'input_dict_rnai_7', 'input_dict_expression_4444444', 'input_dict_expression_44444441', 
        'input_dict_rnai_12', 'input_dict_rnai_777','input_dict_rnai_888', 'input_dict_rnai_1212',
        'input_dict_rnai_77777', 'input_dict_rnai_88888', 'input_dict_rnai_121212','input_dict_transcript_rnai_6']
```

### Comparing `JBioSeqTools-2.0.3/jbst/vector_build.py` & `JBioSeqTools-2.0.4/jbst/vector_build.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 import random
 import string
 import seaborn as sns
 pd.options.mode.chained_assignment = None
 import warnings
 
 warnings.filterwarnings("ignore")
+import random
+
+random.seed(42)
 
 
  #       _  ____   _         _____              _                      __ _____  __  
  #      | ||  _ \ (_)       / ____|            | |                    / /|  __ \ \ \ 
  #      | || |_) | _   ___ | (___   _   _  ___ | |_  ___  _ __ ___   | | | |__) | | |
  #  _   | ||  _ < | | / _ \ \___ \ | | | |/ __|| __|/ _ \| '_ ` _ \  | | |  _  /  | |
  # | |__| || |_) || || (_) |____) || |_| |\__ \| |_|  __/| | | | | | | | | | \ \  | |
@@ -26,30 +29,32 @@
  #                                  |___/                                                                                  
 
 
 def get_package_directory():
     return pkg_resources.resource_filename(__name__, '')
 
 
+
 _cwd = str(get_package_directory())
 
 
+
+
 from jbst.seq_tools import *
 
 
 def random_name(length=30):
     # Define a string of characters to choose from
     characters = string.ascii_letters + string.digits
 
     # Generate a random name by selecting random characters
     name = ''.join(random.choice(characters) for _ in range(length))
     return name
 
 
-  
 
 def determine_rnai_top1_seq(RNAi_data, loop_seq, gc_max = 55, gc_min = 35, end_3 = 'TT', rnai_type = 'sh'):
     
     RNAi_data = RNAi_data[(RNAi_data['GC%'] > gc_min) & (RNAi_data['GC%'] < gc_max)]
     RNAi_data = RNAi_data.reset_index(drop = True)
     
     if len(RNAi_data) > 0:
@@ -351,15 +356,15 @@
             print('id : ' + str(i))
             print('name : ' + restriction_df['name'][i])
 
     
         enzyme_list = []
         check = True
         enzyme_n = 1
-        while (check == True):
+        while(check == True):
             print('\nProvide enzyme id, if no restriction sites are relevant to your experiment or you have already provided all enzyme ids, write "x"')
             enzyme = input('\n Enter enzyme '+ str(enzyme_n) + ' id: ')
             if len(enzyme) != 0 and not enzyme.isalpha() and int(enzyme) in restriction_df.index:
                 enzyme_n += 1
                 enzyme_list = enzyme_list + restriction_df['index'][int(enzyme)]
             elif len(enzyme) != 0 and enzyme.upper() == 'X':
                 check = False
@@ -1700,15 +1705,15 @@
                                 en = list(tmp['index'][tmp['name'].isin(user_defined_enzymes)])
                                 list_tmp = [item for sublist in en for item in sublist]
                                 list_of_list.append(list_tmp)
                             else:
                                 list_of_list.append([])
                 
                         project = add_chosen_restriction(project, list_of_list)
-                        project = repair_restriction_vector(project, metadata, input_dict['species'])
+                        # project = repair_restriction_vector(project, metadata, input_dict['species'])
                         
                     
                 project = vector_string(project, metadata['backbone'], input_dict['vector_type'], input_dict['vector_function'], promoter_dec)
                 project = eval_vector(project, metadata['vectors'], input_dict['vector_type'], input_dict['vector_function'])
             
                 project, pl = vector_plot_project(project, metadata, show_plot = show_plot),
```

### Comparing `JBioSeqTools-2.0.3/setup.py` & `JBioSeqTools-2.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
-VERSION = '2.0.3' 
+VERSION = '2.0.4' 
 DESCRIPTION = 'JBioSeqTools'
 LONG_DESCRIPTION = 'JBioSeqTools is the Python library for biological sequence optimization (GC % content & codon frequency), restriction places removal, DNA/RNA structure prediction, and RNAi selection. It also allows the building of many plasmid vectors with the possibility of choosing sequences such as transcript, promoter, enhancer, molecular fluorescent tag, etc. Finally, the user obtains a ready-for-order construct with a whole sequence and visualization. Package description  on https://github.com/jkubis96/JBioSeqTools'
 
 # Setting up
 setup(
         name="JBioSeqTools", 
         version=VERSION,
         author="Jakub Kubis",
         author_email="jbiosystem@gmail.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=['jbst'],
         include_package_data=True,
-        install_requires=['pandas', 'tqdm', 'matplotlib', 'numpy', 'requests', 'openpyxl', 'pymsaviz==0.4.2', 'ViennaRNA==2.6.4', 'biopython==1.81', 'networkx==3.1', 'seaborn', 'scipy'],       
+        install_requires=['pandas', 'tqdm', 'matplotlib', 'numpy', 'requests', 'openpyxl', 'pymsaviz==0.4.2', 'ViennaRNA==2.6.4', 'biopython==1.81', 'networkx==3.1', 'seaborn', 'scipy', 'gdown==5.2.0'],       
         keywords=['sequence', 'optimization', 'vectors', 'AAV', 'GC', 'restriction enzyme'],
         license = 'MIT',
         classifiers = [
             "Development Status :: 3 - Alpha",
             "Programming Language :: Python :: 3",
             "Operating System :: MacOS :: MacOS X",
             "Operating System :: Microsoft :: Windows",
```

