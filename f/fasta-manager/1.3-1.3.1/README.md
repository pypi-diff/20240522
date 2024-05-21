# Comparing `tmp/fasta_manager-1.3.tar.gz` & `tmp/fasta_manager-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasta_manager-1.3.tar", last modified: Tue May 21 21:54:10 2024, max compression
+gzip compressed data, was "fasta_manager-1.3.1.tar", last modified: Tue May 21 22:11:19 2024, max compression
```

## Comparing `fasta_manager-1.3.tar` & `fasta_manager-1.3.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 21:54:10.357765 fasta_manager-1.3/
--rw-rw-rw-   0        0        0     1084 2024-05-21 20:37:12.000000 fasta_manager-1.3/LICENSE
--rw-rw-rw-   0        0        0     2359 2024-05-21 21:54:10.357264 fasta_manager-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1844 2024-05-21 21:39:18.000000 fasta_manager-1.3/README.md
--rw-rw-rw-   0        0        0      108 2024-05-21 21:46:37.000000 fasta_manager-1.3/pyproject.toml
--rw-rw-rw-   0        0        0      729 2024-05-21 21:54:10.358764 fasta_manager-1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-21 21:54:10.330264 fasta_manager-1.3/src/
-drwxrwxrwx   0        0        0        0 2024-05-21 21:54:10.356763 fasta_manager-1.3/src/fasta_manager.egg-info/
--rw-rw-rw-   0        0        0     2359 2024-05-21 21:54:10.000000 fasta_manager-1.3/src/fasta_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      761 2024-05-21 21:54:10.000000 fasta_manager-1.3/src/fasta_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 21:54:10.000000 fasta_manager-1.3/src/fasta_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-21 21:54:10.000000 fasta_manager-1.3/src/fasta_manager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-21 21:54:10.000000 fasta_manager-1.3/src/fasta_manager.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-21 21:54:10.346766 fasta_manager-1.3/src/packages/
--rw-rw-rw-   0        0        0        0 2024-05-21 20:37:12.000000 fasta_manager-1.3/src/packages/__init__.py
--rw-rw-rw-   0        0        0     4393 2024-05-21 21:36:14.000000 fasta_manager-1.3/src/packages/main.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:54:10.348263 fasta_manager-1.3/src/packages/plots/
--rw-rw-rw-   0        0        0        0 2024-05-21 20:37:12.000000 fasta_manager-1.3/src/packages/plots/__init__.py
--rw-rw-rw-   0        0        0     3048 2024-05-21 20:37:12.000000 fasta_manager-1.3/src/packages/plots/plot_generator.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:54:10.349763 fasta_manager-1.3/src/packages/sequences/
--rw-rw-rw-   0        0        0        0 2024-05-21 20:37:12.000000 fasta_manager-1.3/src/packages/sequences/__init__.py
--rw-rw-rw-   0        0        0      784 2024-05-21 21:34:56.000000 fasta_manager-1.3/src/packages/sequences/sequences.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:54:10.351263 fasta_manager-1.3/src/packages/stats/
--rw-rw-rw-   0        0        0        0 2024-05-21 20:37:12.000000 fasta_manager-1.3/src/packages/stats/__init__.py
--rw-rw-rw-   0        0        0     1744 2024-05-21 21:13:57.000000 fasta_manager-1.3/src/packages/stats/sequence_stats.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:54:10.354263 fasta_manager-1.3/src/packages/transformers/
--rw-rw-rw-   0        0        0        0 2024-05-21 20:37:12.000000 fasta_manager-1.3/src/packages/transformers/__init__.py
--rw-rw-rw-   0        0        0      356 2024-05-21 20:37:12.000000 fasta_manager-1.3/src/packages/transformers/abstract_transformer.py
--rw-rw-rw-   0        0        0     1626 2024-05-21 20:37:12.000000 fasta_manager-1.3/src/packages/transformers/duplicated_transformer.py
--rw-rw-rw-   0        0        0     1529 2024-05-21 21:35:49.000000 fasta_manager-1.3/src/packages/transformers/reverse_complement.py
-drwxrwxrwx   0        0        0        0 2024-05-21 21:54:10.355762 fasta_manager-1.3/src/packages/utils/
--rw-rw-rw-   0        0        0        0 2024-05-21 20:37:12.000000 fasta_manager-1.3/src/packages/utils/__init__.py
--rw-rw-rw-   0        0        0     2269 2024-05-21 21:36:04.000000 fasta_manager-1.3/src/packages/utils/seq_file_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:19.881958 fasta_manager-1.3.1/
+-rw-rw-rw-   0        0        0     1084 2024-05-21 20:37:12.000000 fasta_manager-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0     2361 2024-05-21 22:11:19.881458 fasta_manager-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1844 2024-05-21 21:39:18.000000 fasta_manager-1.3.1/README.md
+-rw-rw-rw-   0        0        0      108 2024-05-21 21:46:37.000000 fasta_manager-1.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0      731 2024-05-21 22:11:19.883458 fasta_manager-1.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:19.841728 fasta_manager-1.3.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:19.880958 fasta_manager-1.3.1/src/fasta_manager.egg-info/
+-rw-rw-rw-   0        0        0     2361 2024-05-21 22:11:19.000000 fasta_manager-1.3.1/src/fasta_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      761 2024-05-21 22:11:19.000000 fasta_manager-1.3.1/src/fasta_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 22:11:19.000000 fasta_manager-1.3.1/src/fasta_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-21 22:11:19.000000 fasta_manager-1.3.1/src/fasta_manager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-21 22:11:19.000000 fasta_manager-1.3.1/src/fasta_manager.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:19.869228 fasta_manager-1.3.1/src/packages/
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:37:12.000000 fasta_manager-1.3.1/src/packages/__init__.py
+-rw-rw-rw-   0        0        0     4298 2024-05-21 22:08:37.000000 fasta_manager-1.3.1/src/packages/main.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:19.871228 fasta_manager-1.3.1/src/packages/plots/
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:37:12.000000 fasta_manager-1.3.1/src/packages/plots/__init__.py
+-rw-rw-rw-   0        0        0     3048 2024-05-21 20:37:12.000000 fasta_manager-1.3.1/src/packages/plots/plot_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:19.872727 fasta_manager-1.3.1/src/packages/sequences/
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:37:12.000000 fasta_manager-1.3.1/src/packages/sequences/__init__.py
+-rw-rw-rw-   0        0        0      784 2024-05-21 21:34:56.000000 fasta_manager-1.3.1/src/packages/sequences/sequences.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:19.874947 fasta_manager-1.3.1/src/packages/stats/
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:37:12.000000 fasta_manager-1.3.1/src/packages/stats/__init__.py
+-rw-rw-rw-   0        0        0     1744 2024-05-21 21:13:57.000000 fasta_manager-1.3.1/src/packages/stats/sequence_stats.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:19.877957 fasta_manager-1.3.1/src/packages/transformers/
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:37:12.000000 fasta_manager-1.3.1/src/packages/transformers/__init__.py
+-rw-rw-rw-   0        0        0      356 2024-05-21 20:37:12.000000 fasta_manager-1.3.1/src/packages/transformers/abstract_transformer.py
+-rw-rw-rw-   0        0        0     1626 2024-05-21 20:37:12.000000 fasta_manager-1.3.1/src/packages/transformers/duplicated_transformer.py
+-rw-rw-rw-   0        0        0     1529 2024-05-21 21:35:49.000000 fasta_manager-1.3.1/src/packages/transformers/reverse_complement.py
+drwxrwxrwx   0        0        0        0 2024-05-21 22:11:19.879958 fasta_manager-1.3.1/src/packages/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:37:12.000000 fasta_manager-1.3.1/src/packages/utils/__init__.py
+-rw-rw-rw-   0        0        0     2269 2024-05-21 21:36:04.000000 fasta_manager-1.3.1/src/packages/utils/seq_file_manager.py
```

### Comparing `fasta_manager-1.3/LICENSE` & `fasta_manager-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fasta_manager-1.3/PKG-INFO` & `fasta_manager-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasta_manager
-Version: 1.3
+Version: 1.3.1
 Summary: Manage your fasta files
 Home-page: https://github.com/santipvz/FASTA-manager
 Author: santipvz
 Author-email: santivzqzz@gmail.com
 Project-URL: Bug Tracker, https://github.com/santipvz/FASTA-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fasta_manager-1.3/README.md` & `fasta_manager-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `fasta_manager-1.3/setup.cfg` & `fasta_manager-1.3.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2066 6173 7461 5f6d 616e 6167 6572   = fasta_manager
-00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 330d  ..version = 1.3.
-00000030: 0a61 7574 686f 7220 3d20 7361 6e74 6970  .author = santip
-00000040: 767a 0d0a 6175 7468 6f72 5f65 6d61 696c  vz..author_email
-00000050: 203d 2073 616e 7469 767a 717a 7a40 676d   = santivzqzz@gm
-00000060: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
-00000070: 7469 6f6e 203d 204d 616e 6167 6520 796f  tion = Manage yo
-00000080: 7572 2066 6173 7461 2066 696c 6573 0d0a  ur fasta files..
-00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
-000000a0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
-000000b0: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
-000000c0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
-000000d0: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
-000000e0: 6e0d 0a75 726c 203d 2068 7474 7073 3a2f  n..url = https:/
-000000f0: 2f67 6974 6875 622e 636f 6d2f 7361 6e74  /github.com/sant
-00000100: 6970 767a 2f46 4153 5441 2d6d 616e 6167  ipvz/FASTA-manag
-00000110: 6572 0d0a 7072 6f6a 6563 745f 7572 6c73  er..project_urls
-00000120: 203d 200d 0a09 4275 6720 5472 6163 6b65   = ...Bug Tracke
-00000130: 7220 3d20 6874 7470 733a 2f2f 6769 7468  r = https://gith
-00000140: 7562 2e63 6f6d 2f73 616e 7469 7076 7a2f  ub.com/santipvz/
-00000150: 4641 5354 412d 6d61 6e61 6765 722f 6973  FASTA-manager/is
-00000160: 7375 6573 0d0a 636c 6173 7369 6669 6572  sues..classifier
-00000170: 7320 3d20 0d0a 0950 726f 6772 616d 6d69  s = ...Programmi
-00000180: 6e67 204c 616e 6775 6167 6520 3a3a 2050  ng Language :: P
-00000190: 7974 686f 6e20 3a3a 2033 0d0a 094c 6963  ython :: 3...Lic
-000001a0: 656e 7365 203a 3a20 4f53 4920 4170 7072  ense :: OSI Appr
-000001b0: 6f76 6564 203a 3a20 4d49 5420 4c69 6365  oved :: MIT Lice
-000001c0: 6e73 650d 0a09 4f70 6572 6174 696e 6720  nse...Operating 
-000001d0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-000001e0: 6570 656e 6465 6e74 0d0a 0d0a 5b6f 7074  ependent....[opt
-000001f0: 696f 6e73 5d0d 0a70 6163 6b61 6765 5f64  ions]..package_d
-00000200: 6972 203d 200d 0a09 3d20 7372 630d 0a70  ir = ...= src..p
-00000210: 6163 6b61 6765 7320 3d20 6669 6e64 3a0d  ackages = find:.
-00000220: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
-00000230: 203d 203e 3d33 2e36 0d0a 0d0a 5b6f 7074   = >=3.6....[opt
-00000240: 696f 6e73 2e70 6163 6b61 6765 732e 6669  ions.packages.fi
-00000250: 6e64 5d0d 0a77 6865 7265 203d 2073 7263  nd]..where = src
-00000260: 0d0a 0d0a 5b6f 7074 696f 6e73 2e65 6e74  ....[options.ent
-00000270: 7279 5f70 6f69 6e74 735d 0d0a 636f 6e73  ry_points]..cons
-00000280: 6f6c 655f 7363 7269 7074 7320 3d20 0d0a  ole_scripts = ..
-00000290: 0966 6173 7461 203d 2070 6163 6b61 6765  .fasta = package
-000002a0: 732e 6d61 696e 3a6d 6169 6e0d 0a0d 0a5b  s.main:main....[
-000002b0: 6567 675f 696e 666f 5d0d 0a74 6167 5f62  egg_info]..tag_b
-000002c0: 7569 6c64 203d 200d 0a74 6167 5f64 6174  uild = ..tag_dat
-000002d0: 6520 3d20 300d 0a0d 0a                   e = 0....
+00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 332e  ..version = 1.3.
+00000030: 310d 0a61 7574 686f 7220 3d20 7361 6e74  1..author = sant
+00000040: 6970 767a 0d0a 6175 7468 6f72 5f65 6d61  ipvz..author_ema
+00000050: 696c 203d 2073 616e 7469 767a 717a 7a40  il = santivzqzz@
+00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
+00000070: 6970 7469 6f6e 203d 204d 616e 6167 6520  iption = Manage 
+00000080: 796f 7572 2066 6173 7461 2066 696c 6573  your fasta files
+00000090: 0d0a 6c6f 6e67 5f64 6573 6372 6970 7469  ..long_descripti
+000000a0: 6f6e 203d 2066 696c 653a 2052 4541 444d  on = file: READM
+000000b0: 452e 6d64 0d0a 6c6f 6e67 5f64 6573 6372  E.md..long_descr
+000000c0: 6970 7469 6f6e 5f63 6f6e 7465 6e74 5f74  iption_content_t
+000000d0: 7970 6520 3d20 7465 7874 2f6d 6172 6b64  ype = text/markd
+000000e0: 6f77 6e0d 0a75 726c 203d 2068 7474 7073  own..url = https
+000000f0: 3a2f 2f67 6974 6875 622e 636f 6d2f 7361  ://github.com/sa
+00000100: 6e74 6970 767a 2f46 4153 5441 2d6d 616e  ntipvz/FASTA-man
+00000110: 6167 6572 0d0a 7072 6f6a 6563 745f 7572  ager..project_ur
+00000120: 6c73 203d 200d 0a09 4275 6720 5472 6163  ls = ...Bug Trac
+00000130: 6b65 7220 3d20 6874 7470 733a 2f2f 6769  ker = https://gi
+00000140: 7468 7562 2e63 6f6d 2f73 616e 7469 7076  thub.com/santipv
+00000150: 7a2f 4641 5354 412d 6d61 6e61 6765 722f  z/FASTA-manager/
+00000160: 6973 7375 6573 0d0a 636c 6173 7369 6669  issues..classifi
+00000170: 6572 7320 3d20 0d0a 0950 726f 6772 616d  ers = ...Program
+00000180: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000190: 2050 7974 686f 6e20 3a3a 2033 0d0a 094c   Python :: 3...L
+000001a0: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+000001b0: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+000001c0: 6365 6e73 650d 0a09 4f70 6572 6174 696e  cense...Operatin
+000001d0: 6720 5379 7374 656d 203a 3a20 4f53 2049  g System :: OS I
+000001e0: 6e64 6570 656e 6465 6e74 0d0a 0d0a 5b6f  ndependent....[o
+000001f0: 7074 696f 6e73 5d0d 0a70 6163 6b61 6765  ptions]..package
+00000200: 5f64 6972 203d 200d 0a09 3d20 7372 630d  _dir = ...= src.
+00000210: 0a70 6163 6b61 6765 7320 3d20 6669 6e64  .packages = find
+00000220: 3a0d 0a70 7974 686f 6e5f 7265 7175 6972  :..python_requir
+00000230: 6573 203d 203e 3d33 2e36 0d0a 0d0a 5b6f  es = >=3.6....[o
+00000240: 7074 696f 6e73 2e70 6163 6b61 6765 732e  ptions.packages.
+00000250: 6669 6e64 5d0d 0a77 6865 7265 203d 2073  find]..where = s
+00000260: 7263 0d0a 0d0a 5b6f 7074 696f 6e73 2e65  rc....[options.e
+00000270: 6e74 7279 5f70 6f69 6e74 735d 0d0a 636f  ntry_points]..co
+00000280: 6e73 6f6c 655f 7363 7269 7074 7320 3d20  nsole_scripts = 
+00000290: 0d0a 0966 6173 7461 203d 2070 6163 6b61  ...fasta = packa
+000002a0: 6765 732e 6d61 696e 3a6d 6169 6e0d 0a0d  ges.main:main...
+000002b0: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+000002c0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+000002d0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

### Comparing `fasta_manager-1.3/src/fasta_manager.egg-info/PKG-INFO` & `fasta_manager-1.3.1/src/fasta_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fasta_manager
-Version: 1.3
+Version: 1.3.1
 Summary: Manage your fasta files
 Home-page: https://github.com/santipvz/FASTA-manager
 Author: santipvz
 Author-email: santivzqzz@gmail.com
 Project-URL: Bug Tracker, https://github.com/santipvz/FASTA-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fasta_manager-1.3/src/fasta_manager.egg-info/SOURCES.txt` & `fasta_manager-1.3.1/src/fasta_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fasta_manager-1.3/src/packages/main.py` & `fasta_manager-1.3.1/src/packages/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,19 +52,19 @@
     # Get the FASTA files in the current directory
     current_directory = os.getcwd()
     fasta_files = [file for file in os.listdir(current_directory) if file.endswith('.fasta')]
 
     # Verify that there are FASTA files in the current directory
     if not any([args.casefile, args.dremove, args.drename, args.reverse,
                 args.complement, args.rc, args.stats, args.plots]):
-        print('No transformation specified')
+        print('No transformation specified, use fasta -h for help.')
         return
 
     if not fasta_files:
-        print('No FASTA files found in the current directory')
+        print('No FASTA files found in the current directory.')
         return
 
     stats_directory = os.path.join(current_directory, 'result_stats')
 
     
     for filename in fasta_files:
         seq_file_manager = SeqFileManager(input_filename=filename)
@@ -89,18 +89,12 @@
 
 
         # Process the sequences if any transformation was specified
         if any([args.casefile, args.dremove, args.drename, args.reverse, args.complement, args.rc]):
             output_directory = os.path.join(current_directory, 'result_formatted')
             seq_file_manager.write_fasta(sequences, output_directory)
 
+        # Print success message
+        print('Operation completed successfully!')
+
 if __name__ == '__main__':
     main()
-
-    list_of_sequences = [Sequence('seq1', 'atgc'), Sequence('seq2', 'atgc')]
-
-    a = Sequence('seq1', 'atgccc').upper()
-
-    print(a)
-
-    for seq in list_of_sequences:
-        print(seq.upper())
```

### Comparing `fasta_manager-1.3/src/packages/plots/plot_generator.py` & `fasta_manager-1.3.1/src/packages/plots/plot_generator.py`

 * *Files identical despite different names*

### Comparing `fasta_manager-1.3/src/packages/sequences/sequences.py` & `fasta_manager-1.3.1/src/packages/sequences/sequences.py`

 * *Files identical despite different names*

### Comparing `fasta_manager-1.3/src/packages/stats/sequence_stats.py` & `fasta_manager-1.3.1/src/packages/stats/sequence_stats.py`

 * *Files identical despite different names*

### Comparing `fasta_manager-1.3/src/packages/transformers/duplicated_transformer.py` & `fasta_manager-1.3.1/src/packages/transformers/duplicated_transformer.py`

 * *Files identical despite different names*

### Comparing `fasta_manager-1.3/src/packages/transformers/reverse_complement.py` & `fasta_manager-1.3.1/src/packages/transformers/reverse_complement.py`

 * *Files identical despite different names*

### Comparing `fasta_manager-1.3/src/packages/utils/seq_file_manager.py` & `fasta_manager-1.3.1/src/packages/utils/seq_file_manager.py`

 * *Files identical despite different names*

