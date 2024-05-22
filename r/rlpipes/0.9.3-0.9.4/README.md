# Comparing `tmp/rlpipes-0.9.3.tar.gz` & `tmp/rlpipes-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rlpipes-0.9.3.tar", last modified: Mon Aug  8 17:51:19 2022, max compression
+gzip compressed data, was "rlpipes-0.9.4.tar", last modified: Wed May 22 15:30:59 2024, max compression
```

## Comparing `rlpipes-0.9.3.tar` & `rlpipes-0.9.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 millerh1  (1000) millerh1  (1000)        0 2022-08-08 17:51:19.214641 rlpipes-0.9.3/
--rw-r--r--   0 millerh1  (1000) millerh1  (1000)     1090 2021-09-19 20:26:51.000000 rlpipes-0.9.3/LICENSE
--rw-rw-r--   0 millerh1  (1000) millerh1  (1000)       32 2021-09-03 03:16:45.000000 rlpipes-0.9.3/MANIFEST.in
--rw-r--r--   0 millerh1  (1000) millerh1  (1000)    11775 2022-08-08 17:51:19.214641 rlpipes-0.9.3/PKG-INFO
--rw-r--r--   0 millerh1  (1000) millerh1  (1000)    11230 2022-08-01 22:00:46.000000 rlpipes-0.9.3/README.md
-drwxr-xr-x   0 millerh1  (1000) millerh1  (1000)        0 2022-08-08 17:51:19.214641 rlpipes-0.9.3/rlpipes/
--rw-rw-r--   0 millerh1  (1000) millerh1  (1000)        0 2021-08-27 14:27:45.000000 rlpipes-0.9.3/rlpipes/__init__.py
--rw-r--r--   0 millerh1  (1000) millerh1  (1000)    20888 2022-08-01 19:38:47.000000 rlpipes-0.9.3/rlpipes/cli.py
--rw-r--r--   0 millerh1  (1000) millerh1  (1000)     3476 2022-08-01 19:38:47.000000 rlpipes-0.9.3/rlpipes/run_workflow.py
-drwxr-xr-x   0 millerh1  (1000) millerh1  (1000)        0 2022-08-08 17:51:19.214641 rlpipes-0.9.3/rlpipes/src/
-drwxr-xr-x   0 millerh1  (1000) millerh1  (1000)        0 2022-08-08 17:51:19.214641 rlpipes-0.9.3/rlpipes/src/data/
--rw-r--r--   0 millerh1  (1000) millerh1  (1000)    22287 2021-08-29 02:50:25.000000 rlpipes-0.9.3/rlpipes/src/data/.Rhistory
--rw-rw-r--   0 millerh1  (1000) millerh1  (1000)    21488 2021-08-30 01:52:19.000000 rlpipes-0.9.3/rlpipes/src/data/available_genomes.tsv.xz
--rw-rw-r--   0 millerh1  (1000) millerh1  (1000)    10532 2021-08-30 01:52:19.000000 rlpipes-0.9.3/rlpipes/src/data/eff_gen_size.tsv.xz
--rw-rw-r--   0 millerh1  (1000) millerh1  (1000)      470 2021-08-30 01:52:19.000000 rlpipes-0.9.3/rlpipes/src/data/wrangle_effgensize.R
-drwxr-xr-x   0 millerh1  (1000) millerh1  (1000)        0 2022-08-08 17:51:19.214641 rlpipes-0.9.3/rlpipes/src/envs/
--rw-r--r--   0 millerh1  (1000) millerh1  (1000)     1549 2022-08-01 22:56:36.000000 rlpipes-0.9.3/rlpipes/src/envs/awscli.yaml
--rw-rw-r--   0 millerh1  (1000) millerh1  (1000)      962 2022-08-01 22:56:38.000000 rlpipes-0.9.3/rlpipes/src/envs/bwa.yaml
--rw-rw-r--   0 millerh1  (1000) millerh1  (1000)      910 2022-08-01 22:56:39.000000 rlpipes-0.9.3/rlpipes/src/envs/bwamem2.yaml
--rw-rw-r--   0 millerh1  (1000) millerh1  (1000)     2774 2022-08-01 22:56:17.000000 rlpipes-0.9.3/rlpipes/src/envs/deeptools.yaml
--rw-rw-r--   0 millerh1  (1000) millerh1  (1000)      411 2022-08-01 22:56:18.000000 rlpipes-0.9.3/rlpipes/src/envs/fastp.yaml
--rw-rw-r--   0 millerh1  (1000) millerh1  (1000)     3644 2022-08-01 22:56:20.000000 rlpipes-0.9.3/rlpipes/src/envs/macs2.yaml
--rw-r--r--   0 millerh1  (1000) millerh1  (1000)     1017 2022-08-01 22:56:22.000000 rlpipes-0.9.3/rlpipes/src/envs/macs3.yaml
--rw-rw-r--   0 millerh1  (1000) millerh1  (1000)    12962 2022-08-01 22:56:25.000000 rlpipes-0.9.3/rlpipes/src/envs/rlseq.yaml
--rw-r--r--   0 millerh1  (1000) millerh1  (1000)     6866 2022-08-01 22:56:28.000000 rlpipes-0.9.3/rlpipes/src/envs/rsem.yaml
--rw-r--r--   0 millerh1  (1000) millerh1  (1000)      604 2022-08-01 22:56:30.000000 rlpipes-0.9.3/rlpipes/src/envs/salmon.yaml
--rw-rw-r--   0 millerh1  (1000) millerh1  (1000)      880 2022-08-01 22:56:32.000000 rlpipes-0.9.3/rlpipes/src/envs/samtools.yaml
--rw-rw-r--   0 millerh1  (1000) millerh1  (1000)     4227 2022-08-01 22:56:35.000000 rlpipes-0.9.3/rlpipes/src/envs/sratools.yaml
--rw-r--r--   0 millerh1  (1000) millerh1  (1000)    24664 2022-08-01 21:56:44.000000 rlpipes-0.9.3/rlpipes/src/rlpipes.smk
-drwxr-xr-x   0 millerh1  (1000) millerh1  (1000)        0 2022-08-08 17:51:19.214641 rlpipes-0.9.3/rlpipes/src/scripts/
--rw-r--r--   0 millerh1  (1000) millerh1  (1000)      942 2022-08-01 21:57:18.000000 rlpipes-0.9.3/rlpipes/src/scripts/RLSeq.R
-drwxr-xr-x   0 millerh1  (1000) millerh1  (1000)        0 2022-08-08 17:51:19.214641 rlpipes-0.9.3/rlpipes.egg-info/
--rw-rw-r--   0 millerh1  (1000) millerh1  (1000)    11775 2022-08-08 17:51:19.000000 rlpipes-0.9.3/rlpipes.egg-info/PKG-INFO
--rw-rw-r--   0 millerh1  (1000) millerh1  (1000)      838 2022-08-08 17:51:19.000000 rlpipes-0.9.3/rlpipes.egg-info/SOURCES.txt
--rw-rw-r--   0 millerh1  (1000) millerh1  (1000)        1 2022-08-08 17:51:19.000000 rlpipes-0.9.3/rlpipes.egg-info/dependency_links.txt
--rw-rw-r--   0 millerh1  (1000) millerh1  (1000)       44 2022-08-08 17:51:19.000000 rlpipes-0.9.3/rlpipes.egg-info/entry_points.txt
--rw-rw-r--   0 millerh1  (1000) millerh1  (1000)       50 2022-08-08 17:51:19.000000 rlpipes-0.9.3/rlpipes.egg-info/requires.txt
--rw-rw-r--   0 millerh1  (1000) millerh1  (1000)        8 2022-08-08 17:51:19.000000 rlpipes-0.9.3/rlpipes.egg-info/top_level.txt
--rw-rw-r--   0 millerh1  (1000) millerh1  (1000)      118 2022-08-08 17:51:19.214641 rlpipes-0.9.3/setup.cfg
--rw-r--r--   0 millerh1  (1000) millerh1  (1000)     1117 2022-08-08 17:41:24.000000 rlpipes-0.9.3/setup.py
+drwxr-xr-x   0 hmiller  (470203733) domain users (470200513)        0 2024-05-22 15:30:59.768840 rlpipes-0.9.4/
+-rw-r--r--   0 hmiller  (470203733) domain users (470200513)     1090 2024-05-21 20:30:14.000000 rlpipes-0.9.4/LICENSE
+-rw-r--r--   0 hmiller  (470203733) domain users (470200513)       32 2024-05-21 20:30:14.000000 rlpipes-0.9.4/MANIFEST.in
+-rw-r--r--   0 hmiller  (470203733) domain users (470200513)    11795 2024-05-22 15:30:59.762840 rlpipes-0.9.4/PKG-INFO
+-rw-r--r--   0 hmiller  (470203733) domain users (470200513)    11230 2024-05-21 20:30:14.000000 rlpipes-0.9.4/README.md
+drwxr-xr-x   0 hmiller  (470203733) domain users (470200513)        0 2024-05-22 15:30:59.648112 rlpipes-0.9.4/rlpipes/
+-rw-r--r--   0 hmiller  (470203733) domain users (470200513)        0 2024-05-21 20:30:14.000000 rlpipes-0.9.4/rlpipes/__init__.py
+-rw-r--r--   0 hmiller  (470203733) domain users (470200513)    20888 2024-05-21 20:30:14.000000 rlpipes-0.9.4/rlpipes/cli.py
+-rw-r--r--   0 hmiller  (470203733) domain users (470200513)     3476 2024-05-21 20:30:14.000000 rlpipes-0.9.4/rlpipes/run_workflow.py
+drwxr-xr-x   0 hmiller  (470203733) domain users (470200513)        0 2024-05-22 15:30:59.682391 rlpipes-0.9.4/rlpipes/src/
+drwxr-xr-x   0 hmiller  (470203733) domain users (470200513)        0 2024-05-22 15:30:59.698388 rlpipes-0.9.4/rlpipes/src/data/
+-rw-r--r--   0 hmiller  (470203733) domain users (470200513)    21488 2024-05-21 20:30:14.000000 rlpipes-0.9.4/rlpipes/src/data/available_genomes.tsv.xz
+-rw-r--r--   0 hmiller  (470203733) domain users (470200513)    10532 2024-05-21 20:30:14.000000 rlpipes-0.9.4/rlpipes/src/data/eff_gen_size.tsv.xz
+-rw-r--r--   0 hmiller  (470203733) domain users (470200513)      470 2024-05-21 20:30:14.000000 rlpipes-0.9.4/rlpipes/src/data/wrangle_effgensize.R
+drwxr-xr-x   0 hmiller  (470203733) domain users (470200513)        0 2024-05-22 15:30:59.760217 rlpipes-0.9.4/rlpipes/src/envs/
+-rw-------   0 hmiller  (470203733) domain users (470200513)      996 2024-05-21 20:44:20.000000 rlpipes-0.9.4/rlpipes/src/envs/awscli.yaml
+-rw-------   0 hmiller  (470203733) domain users (470200513)      671 2024-05-21 20:44:17.000000 rlpipes-0.9.4/rlpipes/src/envs/bwa.yaml
+-rw-------   0 hmiller  (470203733) domain users (470200513)      647 2024-05-21 20:44:17.000000 rlpipes-0.9.4/rlpipes/src/envs/bwamem2.yaml
+-rw-r--r--   0 hmiller  (470203733) domain users (470200513)      679 2024-05-21 20:43:29.000000 rlpipes-0.9.4/rlpipes/src/envs/clean.sh
+-rw-------   0 hmiller  (470203733) domain users (470200513)       78 2024-05-21 20:44:17.000000 rlpipes-0.9.4/rlpipes/src/envs/deeptools.yaml
+-rw-------   0 hmiller  (470203733) domain users (470200513)      324 2024-05-21 20:44:20.000000 rlpipes-0.9.4/rlpipes/src/envs/fastp.yaml
+-rw-------   0 hmiller  (470203733) domain users (470200513)     2390 2024-05-21 20:44:19.000000 rlpipes-0.9.4/rlpipes/src/envs/macs2.yaml
+-rw-------   0 hmiller  (470203733) domain users (470200513)      738 2024-05-21 20:44:17.000000 rlpipes-0.9.4/rlpipes/src/envs/macs3.yaml
+-rw-------   0 hmiller  (470203733) domain users (470200513)     8950 2024-05-21 20:44:19.000000 rlpipes-0.9.4/rlpipes/src/envs/rlseq.yaml
+-rw-------   0 hmiller  (470203733) domain users (470200513)     4752 2024-05-21 20:44:20.000000 rlpipes-0.9.4/rlpipes/src/envs/rsem.yaml
+-rw-------   0 hmiller  (470203733) domain users (470200513)      440 2024-05-21 20:44:17.000000 rlpipes-0.9.4/rlpipes/src/envs/salmon.yaml
+-rw-------   0 hmiller  (470203733) domain users (470200513)      628 2024-05-21 20:44:17.000000 rlpipes-0.9.4/rlpipes/src/envs/samtools.yaml
+-rw-------   0 hmiller  (470203733) domain users (470200513)     2982 2024-05-21 20:44:58.000000 rlpipes-0.9.4/rlpipes/src/envs/sratools.yaml
+-rw-r--r--   0 hmiller  (470203733) domain users (470200513)    24668 2024-05-22 14:54:38.000000 rlpipes-0.9.4/rlpipes/src/rlpipes.smk
+drwxr-xr-x   0 hmiller  (470203733) domain users (470200513)        0 2024-05-22 15:30:59.765390 rlpipes-0.9.4/rlpipes/src/scripts/
+-rw-r--r--   0 hmiller  (470203733) domain users (470200513)      942 2024-05-21 20:30:14.000000 rlpipes-0.9.4/rlpipes/src/scripts/RLSeq.R
+drwxr-xr-x   0 hmiller  (470203733) domain users (470200513)        0 2024-05-22 15:30:59.672420 rlpipes-0.9.4/rlpipes.egg-info/
+-rw-r--r--   0 hmiller  (470203733) domain users (470200513)    11795 2024-05-22 15:30:59.000000 rlpipes-0.9.4/rlpipes.egg-info/PKG-INFO
+-rw-r--r--   0 hmiller  (470203733) domain users (470200513)      837 2024-05-22 15:30:59.000000 rlpipes-0.9.4/rlpipes.egg-info/SOURCES.txt
+-rw-r--r--   0 hmiller  (470203733) domain users (470200513)        1 2024-05-22 15:30:59.000000 rlpipes-0.9.4/rlpipes.egg-info/dependency_links.txt
+-rw-r--r--   0 hmiller  (470203733) domain users (470200513)       45 2024-05-22 15:30:59.000000 rlpipes-0.9.4/rlpipes.egg-info/entry_points.txt
+-rw-r--r--   0 hmiller  (470203733) domain users (470200513)       50 2024-05-22 15:30:59.000000 rlpipes-0.9.4/rlpipes.egg-info/requires.txt
+-rw-r--r--   0 hmiller  (470203733) domain users (470200513)        8 2024-05-22 15:30:59.000000 rlpipes-0.9.4/rlpipes.egg-info/top_level.txt
+-rw-r--r--   0 hmiller  (470203733) domain users (470200513)      118 2024-05-22 15:30:59.763496 rlpipes-0.9.4/setup.cfg
+-rw-r--r--   0 hmiller  (470203733) domain users (470200513)     1117 2024-05-22 15:30:20.000000 rlpipes-0.9.4/setup.py
```

### Comparing `rlpipes-0.9.3/LICENSE` & `rlpipes-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rlpipes-0.9.3/PKG-INFO` & `rlpipes-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: rlpipes
-Version: 0.9.3
+Version: 0.9.4
 Summary: A standardized R-loop-mapping pipeline
 Home-page: https://github.com/Bishop-Laboratory/RLPipes
 Author: Henry Miller
 Author-email: millerh1@livemail.uthscsa.edu
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -32,15 +33,15 @@
 package can be used for more fine-grained downstream analysis.
 
 ## Install
 
 The preferred installation method is `mamba` or `conda` (slower):
 
 ```shell
-mamba create -n rlpipes -c bioconda -c conda-forge rlpipes
+mamba create -n rlpipes -c conda-forge -c bioconda rlpipes
 conda activate rlpipes
 ```
 
 ### Using `pip`
 
 RLPipes can also be installed with `pip`. However, system dependencies will 
 still need to be installed. To accomplish this, do the following:
@@ -333,7 +334,9 @@
   --noreport             If set, RLSeq reports will not be generated.
   --debug                Run pipeline on subsampled number of reads (for
                          testing).
   --tsv                  Obtain config from config.tsv file instead of
                          config.json.
   --help                 Show this message and exit.
 ```
+
+
```

### Comparing `rlpipes-0.9.3/README.md` & `rlpipes-0.9.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 package can be used for more fine-grained downstream analysis.
 
 ## Install
 
 The preferred installation method is `mamba` or `conda` (slower):
 
 ```shell
-mamba create -n rlpipes -c bioconda -c conda-forge rlpipes
+mamba create -n rlpipes -c conda-forge -c bioconda rlpipes
 conda activate rlpipes
 ```
 
 ### Using `pip`
 
 RLPipes can also be installed with `pip`. However, system dependencies will 
 still need to be installed. To accomplish this, do the following:
```

### Comparing `rlpipes-0.9.3/rlpipes/cli.py` & `rlpipes-0.9.4/rlpipes/cli.py`

 * *Files identical despite different names*

### Comparing `rlpipes-0.9.3/rlpipes/run_workflow.py` & `rlpipes-0.9.4/rlpipes/run_workflow.py`

 * *Files identical despite different names*

### Comparing `rlpipes-0.9.3/rlpipes/src/data/available_genomes.tsv.xz` & `rlpipes-0.9.4/rlpipes/src/data/available_genomes.tsv.xz`

 * *Files identical despite different names*

### Comparing `rlpipes-0.9.3/rlpipes/src/data/eff_gen_size.tsv.xz` & `rlpipes-0.9.4/rlpipes/src/data/eff_gen_size.tsv.xz`

 * *Files identical despite different names*

### Comparing `rlpipes-0.9.3/rlpipes/src/envs/bwa.yaml` & `rlpipes-0.9.4/rlpipes/src/envs/samtools.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,36 @@
-# # Original
+# # Original version
 # channels:
 #   - bioconda
 #   - conda-forge
 # dependencies:
-#   - bwa
 #   - samtools
 
-# Pinned
+# Pinned verion
 channels:
-  - bioconda
   - conda-forge
+  - bioconda
   - defaults
 dependencies:
-  - _libgcc_mutex=0.1=conda_forge
-  - _openmp_mutex=4.5=2_gnu
-  - bwa=0.7.17=h7132678_9
-  - bzip2=1.0.8=h7f98852_4
-  - c-ares=1.18.1=h7f98852_0
-  - ca-certificates=2022.6.15=ha878542_0
-  - htslib=1.15.1=h9753748_0
-  - keyutils=1.6.1=h166bdaf_0
-  - krb5=1.19.3=h3790be6_0
-  - libcurl=7.83.1=h7bff187_0
-  - libdeflate=1.10=h7f98852_0
-  - libedit=3.1.20191231=he28a2e2_2
-  - libev=4.33=h516909a_1
-  - libgcc-ng=12.1.0=h8d9b700_16
-  - libgomp=12.1.0=h8d9b700_16
-  - libnghttp2=1.47.0=h727a467_0
-  - libnsl=2.0.0=h7f98852_0
-  - libssh2=1.10.0=ha56f1ee_2
-  - libstdcxx-ng=12.1.0=ha89aaad_16
-  - libzlib=1.2.12=h166bdaf_2
-  - ncurses=6.3=h27087fc_1
-  - openssl=1.1.1q=h166bdaf_0
-  - perl=5.32.1=2_h7f98852_perl5
-  - samtools=1.15.1=h1170115_0
-  - xz=5.2.5=h516909a_1
-  - zlib=1.2.12=h166bdaf_2
+  - _libgcc_mutex=0.1
+  - _openmp_mutex=4.5
+  - bzip2=1.0.8
+  - c-ares=1.18.1
+  - ca-certificates=2022.6.15
+  - htslib=1.15.1
+  - keyutils=1.6.1
+  - krb5=1.19.3
+  - libcurl=7.83.1
+  - libdeflate=1.10
+  - libedit=3.1.20191231
+  - libev=4.33
+  - libgcc-ng=12.1.0
+  - libgomp=12.1.0
+  - libnghttp2=1.47.0
+  - libssh2=1.10.0
+  - libstdcxx-ng=12.1.0
+  - libzlib=1.2.12
+  - ncurses=6.3
+  - openssl=1.1.1q
+  - samtools=1.15.1
+  - xz=5.2.5
+  - zlib=1.2.12
```

### Comparing `rlpipes-0.9.3/rlpipes/src/envs/macs3.yaml` & `rlpipes-0.9.4/rlpipes/src/envs/awscli.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,44 +1,57 @@
 # # Original
 # channels:
-#   - bioconda
 #   - conda-forge
 # dependencies:
-#   - python >= 3.8
-#   - pip
-#   - pip:
-#     - macs3
+#   - awscli
 
 # Pinned
 channels:
   - conda-forge
   - defaults
 dependencies:
-  - _libgcc_mutex=0.1=conda_forge
-  - _openmp_mutex=4.5=2_gnu
-  - bzip2=1.0.8=h7f98852_4
-  - ca-certificates=2022.6.15=ha878542_0
-  - ld_impl_linux-64=2.36.1=hea4e1c9_2
-  - libffi=3.4.2=h7f98852_5
-  - libgcc-ng=12.1.0=h8d9b700_16
-  - libgomp=12.1.0=h8d9b700_16
-  - libnsl=2.0.0=h7f98852_0
-  - libuuid=2.32.1=h7f98852_1000
-  - libzlib=1.2.12=h166bdaf_2
-  - ncurses=6.3=h27087fc_1
-  - openssl=3.0.5=h166bdaf_0
-  - pip=22.2.1=pyhd8ed1ab_0
-  - python=3.10.5=ha86cf86_0_cpython
-  - python_abi=3.10=2_cp310
-  - readline=8.1.2=h0f457ee_0
-  - setuptools=63.3.0=py310hff52083_0
-  - sqlite=3.39.2=h4ff8645_0
-  - tk=8.6.12=h27826a3_0
-  - tzdata=2022a=h191b570_0
-  - wheel=0.37.1=pyhd8ed1ab_0
-  - xz=5.2.5=h516909a_1
-  - zlib=1.2.12=h166bdaf_2
+  - _libgcc_mutex=0.1
+  - _openmp_mutex=4.5
+  - awscli=1.25.34
+  - botocore=1.27.34
+  - brotlipy=0.7.0
+  - bzip2=1.0.8
+  - ca-certificates=2022.6.15
+  - certifi=2022.6.15
+  - cffi=1.15.1
+  - colorama=0.4.4
+  - cryptography=37.0.4
+  - docutils=0.15.2
+  - idna=3.3
+  - jmespath=1.0.1
+  - ld_impl_linux-64=2.36.1
+  - libffi=3.4.2
+  - libgcc-ng=12.1.0
+  - libgomp=12.1.0
+  - libnsl=2.0.0
+  - libuuid=2.32.1
+  - libzlib=1.2.12
+  - ncurses=6.3
+  - openssl=1.1.1q
+  - pip=22.2.1
+  - pyasn1=0.4.8
+  - pycparser=2.21
+  - pyopenssl=22.0.0
+  - pysocks=1.7.1
+  - python=3.10.5
+  - python-dateutil=2.8.2
+  - python_abi=3.10
+  - pyyaml=5.4.1
+  - readline=8.1.2
+  - rsa=4.7.2
+  - s3transfer=0.6.0
+  - six=1.16.0
+  - sqlite=3.39.2
+  - tk=8.6.12
+  - tzdata=2022a
+  - urllib3=1.26.11
+  - wheel=0.37.1
+  - xz=5.2.5
+  - yaml=0.2.5
+  - zlib=1.2.12
   - pip:
-    - cykhash==2.0.0
-    - cython==0.29.32
-    - macs3==3.0.0a7
-    - numpy==1.23.1
+    - setuptools==57.4.0
```

### Comparing `rlpipes-0.9.3/rlpipes/src/rlpipes.smk` & `rlpipes-0.9.4/rlpipes/src/rlpipes.smk`

 * *Files 0% similar despite different names*

```diff
@@ -357,15 +357,15 @@
     """
 
 rule download_gtf:
     output:
         genome_home_dir + "/{genome}/{genome}.ensGene.gtf"
     log: genome_home_dir + "/logs/download_gtf/{genome}__download_gtf.log"
     shell: """
-        wget -O {output}.gz ftp://hgdownload.soe.ucsc.edu/goldenPath/{wildcards.genome}/bigZips/genes/{wildcards.genome}.ensGene.gtf.gz
+        wget -O {output}.gz https://hgdownload.cse.ucsc.edu/goldenpath/{wildcards.genome}/bigZips/genes/{wildcards.genome}.ensGene.gtf.gz
         gunzip {output}.gz &> {log}
     """
 
 rule rlseq:
     input: unpack(get_report_inputs)
     output:
         html="{outdir}/rlseq_report/{sample}_{genome}.html",
@@ -507,15 +507,15 @@
     output:
         genome_home_dir + "/{genome}/{genome}.fa"
     params:
           prefix=genome_home_dir + "/{genome}/bwa_index/{genome}",
     log: outdir + "/logs/download_fasta/{genome}__download_fasta.log"
     shell: """
         (mkdir -p {params.prefix}
-        wget -O {output}.gz ftp://hgdownload.soe.ucsc.edu/goldenPath/{wildcards.genome}/bigZips/{wildcards.genome}.fa.gz
+        wget -O {output}.gz https://hgdownload.cse.ucsc.edu/goldenpath/{wildcards.genome}/bigZips/{wildcards.genome}.fa.gz
         gunzip {output}.gz && echo "Indexing BAM at {params.prefix} ... This may take some time ...") &> {log}
     """
 
 
 # TODO: Pipe this part
 rule fastp:
     input: check_type_fq
```

### Comparing `rlpipes-0.9.3/rlpipes/src/scripts/RLSeq.R` & `rlpipes-0.9.4/rlpipes/src/scripts/RLSeq.R`

 * *Files identical despite different names*

### Comparing `rlpipes-0.9.3/rlpipes.egg-info/PKG-INFO` & `rlpipes-0.9.4/rlpipes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: rlpipes
-Version: 0.9.3
+Version: 0.9.4
 Summary: A standardized R-loop-mapping pipeline
 Home-page: https://github.com/Bishop-Laboratory/RLPipes
 Author: Henry Miller
 Author-email: millerh1@livemail.uthscsa.edu
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -32,15 +33,15 @@
 package can be used for more fine-grained downstream analysis.
 
 ## Install
 
 The preferred installation method is `mamba` or `conda` (slower):
 
 ```shell
-mamba create -n rlpipes -c bioconda -c conda-forge rlpipes
+mamba create -n rlpipes -c conda-forge -c bioconda rlpipes
 conda activate rlpipes
 ```
 
 ### Using `pip`
 
 RLPipes can also be installed with `pip`. However, system dependencies will 
 still need to be installed. To accomplish this, do the following:
@@ -333,7 +334,9 @@
   --noreport             If set, RLSeq reports will not be generated.
   --debug                Run pipeline on subsampled number of reads (for
                          testing).
   --tsv                  Obtain config from config.tsv file instead of
                          config.json.
   --help                 Show this message and exit.
 ```
+
+
```

### Comparing `rlpipes-0.9.3/rlpipes.egg-info/SOURCES.txt` & `rlpipes-0.9.4/rlpipes.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -9,21 +9,21 @@
 rlpipes.egg-info/PKG-INFO
 rlpipes.egg-info/SOURCES.txt
 rlpipes.egg-info/dependency_links.txt
 rlpipes.egg-info/entry_points.txt
 rlpipes.egg-info/requires.txt
 rlpipes.egg-info/top_level.txt
 rlpipes/src/rlpipes.smk
-rlpipes/src/data/.Rhistory
 rlpipes/src/data/available_genomes.tsv.xz
 rlpipes/src/data/eff_gen_size.tsv.xz
 rlpipes/src/data/wrangle_effgensize.R
 rlpipes/src/envs/awscli.yaml
 rlpipes/src/envs/bwa.yaml
 rlpipes/src/envs/bwamem2.yaml
+rlpipes/src/envs/clean.sh
 rlpipes/src/envs/deeptools.yaml
 rlpipes/src/envs/fastp.yaml
 rlpipes/src/envs/macs2.yaml
 rlpipes/src/envs/macs3.yaml
 rlpipes/src/envs/rlseq.yaml
 rlpipes/src/envs/rsem.yaml
 rlpipes/src/envs/salmon.yaml
```

### Comparing `rlpipes-0.9.3/setup.py` & `rlpipes-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name='rlpipes',
-    version='0.9.3',
+    version='0.9.4',
     description="A standardized R-loop-mapping pipeline",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/Bishop-Laboratory/RLPipes",
     author="Henry Miller",
     author_email="millerh1@livemail.uthscsa.edu",
     license="MIT",
```

