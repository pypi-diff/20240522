# Comparing `tmp/adtoolbox-0.5.8.tar.gz` & `tmp/adtoolbox-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adtoolbox-0.5.8.tar", max compression
+gzip compressed data, was "adtoolbox-0.5.9.tar", max compression
```

## Comparing `adtoolbox-0.5.8.tar` & `adtoolbox-0.5.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      988 2024-05-09 04:21:15.185160 adtoolbox-0.5.8/README.md
--rw-r--r--   0        0        0    10244 2024-05-08 17:37:32.568953 adtoolbox-0.5.8/adtoolbox/.DS_Store
--rw-r--r--   0        0        0     1441 2024-05-08 19:34:33.066301 adtoolbox-0.5.8/adtoolbox/__init__.py
--rw-r--r--   0        0        0      105 2024-05-08 17:23:25.597504 adtoolbox-0.5.8/adtoolbox/__main__.py
--rw-r--r--   0        0        0   128039 2024-05-08 17:48:13.221816 adtoolbox-0.5.8/adtoolbox/adm.py
--rw-r--r--   0        0        0     2205 2022-08-16 19:59:36.800896 adtoolbox-0.5.8/adtoolbox/bio_struct.py
--rwxr-xr-x   0        0        0    29971 2024-05-08 22:45:44.491151 adtoolbox-0.5.8/adtoolbox/cli.py
--rw-r--r--   0        0        0    16660 2024-05-20 16:45:36.910045 adtoolbox-0.5.8/adtoolbox/configs.py
--rw-r--r--   0        0        0   110142 2024-05-21 19:48:16.265314 adtoolbox-0.5.8/adtoolbox/core.py
--rw-r--r--   0        0        0    22543 2023-08-02 19:32:18.486966 adtoolbox-0.5.8/adtoolbox/metagenomics_report.py
--rw-r--r--   0        0        0    22395 2024-05-03 15:32:20.794835 adtoolbox-0.5.8/adtoolbox/optimize.py
--rw-r--r--   0        0        0     1416 2024-02-02 20:59:40.864054 adtoolbox-0.5.8/adtoolbox/pipeline.py
--rw-r--r--   0        0        0     6148 2024-05-08 17:42:50.899853 adtoolbox-0.5.8/adtoolbox/pkg_data/.DS_Store
--rw-r--r--   0        0        0    68830 2024-04-30 20:16:40.698305 adtoolbox-0.5.8/adtoolbox/pkg_data/Modified_ADM_Map.json
--rw-r--r--   0        0        0    12494 2024-04-30 20:13:51.051065 adtoolbox-0.5.8/adtoolbox/pkg_data/Modified_ADM_Model.json
--rw-r--r--   0        0        0     7558 2022-08-16 19:59:36.805098 adtoolbox-0.5.8/adtoolbox/pkg_data/README.md
--rw-r--r--   0        0        0      864 2024-05-15 19:39:10.537774 adtoolbox-0.5.8/adtoolbox/pkg_data/qiime_template_paired.txt
--rw-r--r--   0        0        0      920 2024-05-15 19:45:02.263654 adtoolbox-0.5.8/adtoolbox/pkg_data/qiime_template_single.txt
--rw-r--r--   0        0        0      235 2023-01-24 22:36:35.570064 adtoolbox-0.5.8/adtoolbox/pkg_data/slurm_template.txt
--rw-r--r--   0        0        0     2851 2023-12-18 19:46:22.537162 adtoolbox-0.5.8/adtoolbox/stats.py
--rw-r--r--   0        0        0    10949 2024-01-31 20:24:29.307481 adtoolbox-0.5.8/adtoolbox/tables.py
--rw-r--r--   0        0        0    15972 2024-05-20 19:34:44.781887 adtoolbox-0.5.8/adtoolbox/utils.py
--rw-r--r--   0        0        0      768 2024-05-21 20:34:26.806580 adtoolbox-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     4448 2024-05-21 20:34:36.616119 adtoolbox-0.5.8/setup.py
--rw-r--r--   0        0        0     2003 2024-05-21 20:34:36.616315 adtoolbox-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0      988 2024-05-09 04:21:15.185160 adtoolbox-0.5.9/README.md
+-rw-r--r--   0        0        0    10244 2024-05-08 17:37:32.568953 adtoolbox-0.5.9/adtoolbox/.DS_Store
+-rw-r--r--   0        0        0     1441 2024-05-08 19:34:33.066301 adtoolbox-0.5.9/adtoolbox/__init__.py
+-rw-r--r--   0        0        0      105 2024-05-08 17:23:25.597504 adtoolbox-0.5.9/adtoolbox/__main__.py
+-rw-r--r--   0        0        0   128039 2024-05-08 17:48:13.221816 adtoolbox-0.5.9/adtoolbox/adm.py
+-rw-r--r--   0        0        0     2205 2022-08-16 19:59:36.800896 adtoolbox-0.5.9/adtoolbox/bio_struct.py
+-rwxr-xr-x   0        0        0    29971 2024-05-08 22:45:44.491151 adtoolbox-0.5.9/adtoolbox/cli.py
+-rw-r--r--   0        0        0    16660 2024-05-20 16:45:36.910045 adtoolbox-0.5.9/adtoolbox/configs.py
+-rw-r--r--   0        0        0   110891 2024-05-21 21:28:52.224485 adtoolbox-0.5.9/adtoolbox/core.py
+-rw-r--r--   0        0        0    22543 2023-08-02 19:32:18.486966 adtoolbox-0.5.9/adtoolbox/metagenomics_report.py
+-rw-r--r--   0        0        0    22395 2024-05-03 15:32:20.794835 adtoolbox-0.5.9/adtoolbox/optimize.py
+-rw-r--r--   0        0        0     1416 2024-02-02 20:59:40.864054 adtoolbox-0.5.9/adtoolbox/pipeline.py
+-rw-r--r--   0        0        0     6148 2024-05-08 17:42:50.899853 adtoolbox-0.5.9/adtoolbox/pkg_data/.DS_Store
+-rw-r--r--   0        0        0    68830 2024-04-30 20:16:40.698305 adtoolbox-0.5.9/adtoolbox/pkg_data/Modified_ADM_Map.json
+-rw-r--r--   0        0        0    12494 2024-04-30 20:13:51.051065 adtoolbox-0.5.9/adtoolbox/pkg_data/Modified_ADM_Model.json
+-rw-r--r--   0        0        0     7558 2022-08-16 19:59:36.805098 adtoolbox-0.5.9/adtoolbox/pkg_data/README.md
+-rw-r--r--   0        0        0      864 2024-05-15 19:39:10.537774 adtoolbox-0.5.9/adtoolbox/pkg_data/qiime_template_paired.txt
+-rw-r--r--   0        0        0      920 2024-05-15 19:45:02.263654 adtoolbox-0.5.9/adtoolbox/pkg_data/qiime_template_single.txt
+-rw-r--r--   0        0        0      235 2023-01-24 22:36:35.570064 adtoolbox-0.5.9/adtoolbox/pkg_data/slurm_template.txt
+-rw-r--r--   0        0        0     2851 2023-12-18 19:46:22.537162 adtoolbox-0.5.9/adtoolbox/stats.py
+-rw-r--r--   0        0        0    10949 2024-01-31 20:24:29.307481 adtoolbox-0.5.9/adtoolbox/tables.py
+-rw-r--r--   0        0        0    15972 2024-05-20 19:34:44.781887 adtoolbox-0.5.9/adtoolbox/utils.py
+-rw-r--r--   0        0        0      768 2024-05-21 21:30:20.637120 adtoolbox-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     4448 2024-05-21 21:30:27.844064 adtoolbox-0.5.9/setup.py
+-rw-r--r--   0        0        0     2003 2024-05-21 21:30:27.844271 adtoolbox-0.5.9/PKG-INFO
```

### Comparing `adtoolbox-0.5.8/README.md` & `adtoolbox-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.8/adtoolbox/.DS_Store` & `adtoolbox-0.5.9/adtoolbox/.DS_Store`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.8/adtoolbox/__init__.py` & `adtoolbox-0.5.9/adtoolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.8/adtoolbox/adm.py` & `adtoolbox-0.5.9/adtoolbox/adm.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.8/adtoolbox/bio_struct.py` & `adtoolbox-0.5.9/adtoolbox/bio_struct.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.8/adtoolbox/cli.py` & `adtoolbox-0.5.9/adtoolbox/cli.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.8/adtoolbox/configs.py` & `adtoolbox-0.5.9/adtoolbox/configs.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.8/adtoolbox/core.py` & `adtoolbox-0.5.9/adtoolbox/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -2026,14 +2026,24 @@
             prefetch_script+=f"docker run -v {target_dir}:{target_dir} {self.config.adtoolbox_docker} prefetch {accession} -O {target_dir}\n"
             acc_folder=pathlib.Path(target_dir)/accession
             fasterq_dump_script=""
             sra_file=acc_folder/(accession+".sra")
             fasterq_dump_script+=f"docker run -v {target_dir}:{target_dir} {self.config.adtoolbox_docker} fasterq-dump {sra_file} -O {acc_folder} --split-files\n"
             fasterq_dump_script+=f"docker run -v {target_dir}:{target_dir} {self.config.adtoolbox_docker} rm {sra_file}"
             prefetch_script+=fasterq_dump_script
+        
+        elif container=="singularity":
+            prefetch_script=f"""#!/bin/bash\n"""
+            prefetch_script+=f"singularity exec -B {target_dir}:{target_dir} {self.config.adtoolbox_singularity} prefetch {accession} -O {target_dir}\n"
+            acc_folder=pathlib.Path(target_dir)/accession
+            fasterq_dump_script=""
+            sra_file=acc_folder/(accession+".sra")
+            fasterq_dump_script+=f"singularity exec -B {target_dir}:{target_dir} {self.config.adtoolbox_singularity} fasterq-dump {sra_file} -O {acc_folder} --split-files\n"
+            fasterq_dump_script+=f"singularity exec -B {target_dir}:{target_dir} {self.config.adtoolbox_singularity} rm {sra_file}"
+            prefetch_script+=fasterq_dump_script
        
         sample_metadata=utils.get_sample_metadata_from_accession(accession)      
             
         
         return prefetch_script,sample_metadata
```

### Comparing `adtoolbox-0.5.8/adtoolbox/metagenomics_report.py` & `adtoolbox-0.5.9/adtoolbox/metagenomics_report.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.8/adtoolbox/optimize.py` & `adtoolbox-0.5.9/adtoolbox/optimize.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.8/adtoolbox/pipeline.py` & `adtoolbox-0.5.9/adtoolbox/pipeline.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.8/adtoolbox/pkg_data/.DS_Store` & `adtoolbox-0.5.9/adtoolbox/pkg_data/.DS_Store`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.8/adtoolbox/pkg_data/Modified_ADM_Map.json` & `adtoolbox-0.5.9/adtoolbox/pkg_data/Modified_ADM_Map.json`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.8/adtoolbox/pkg_data/Modified_ADM_Model.json` & `adtoolbox-0.5.9/adtoolbox/pkg_data/Modified_ADM_Model.json`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.8/adtoolbox/pkg_data/README.md` & `adtoolbox-0.5.9/adtoolbox/pkg_data/README.md`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.8/adtoolbox/pkg_data/qiime_template_paired.txt` & `adtoolbox-0.5.9/adtoolbox/pkg_data/qiime_template_paired.txt`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.8/adtoolbox/pkg_data/qiime_template_single.txt` & `adtoolbox-0.5.9/adtoolbox/pkg_data/qiime_template_single.txt`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.8/adtoolbox/stats.py` & `adtoolbox-0.5.9/adtoolbox/stats.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.8/adtoolbox/tables.py` & `adtoolbox-0.5.9/adtoolbox/tables.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.8/adtoolbox/utils.py` & `adtoolbox-0.5.9/adtoolbox/utils.py`

 * *Files identical despite different names*

### Comparing `adtoolbox-0.5.8/pyproject.toml` & `adtoolbox-0.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "adtoolbox"
-version = "0.5.8"
+version = "0.5.9"
 description = "A tool for modeling and optimization of anaerobic digestion process."
 authors = ["ParsaGhadermazi <54489047+ParsaGhadermazi@users.noreply.github.com>"]
 readme= "README.md"
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 bs4 = "^0.0.1"
 dash = "^2.4.1"
```

### Comparing `adtoolbox-0.5.8/setup.py` & `adtoolbox-0.5.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
  'sympy>=1.10.1,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['ADToolbox = adtoolbox.__main__:main']}
 
 setup_kwargs = {
     'name': 'adtoolbox',
-    'version': '0.5.8',
+    'version': '0.5.9',
     'description': 'A tool for modeling and optimization of anaerobic digestion process.',
     'long_description': '# Toolbox Overview\nParsa Ghadermazi \nparsa96@colostate.edu\n\nAD Toolbox is developed in Chan Lab at Colorado State University. The main goal of this toolbox is to provide the tools that are useful for modeling and optimization of anaerobic digestion process.\n\nInterested in trying ADToolbox? Run the notebooks on Binder or Colab:\n\n[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/chan-csu/ADToolbox/HEAD)\n<a target="_blank" href="https://colab.research.google.com/github/chan-csu/ADToolbox/blob/main/README.md">\n  <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>\n</a>\n[![PyPI version](https://badge.fury.io/py/adtoolbox.svg)](https://badge.fury.io/py/adtoolbox)\n\n***NOTE***:Binder implementations don\'t offer escher map functionalities yet.\n\nADToolbox comes with a detailed documentation website. You can access this website using the link below:\n\n** [Full Documentation Here](https://chan-csu.github.io/ADToolbox/) **\n\n\n',
     'author': 'ParsaGhadermazi',
     'author_email': '54489047+ParsaGhadermazi@users.noreply.github.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `adtoolbox-0.5.8/PKG-INFO` & `adtoolbox-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adtoolbox
-Version: 0.5.8
+Version: 0.5.9
 Summary: A tool for modeling and optimization of anaerobic digestion process.
 Author: ParsaGhadermazi
 Author-email: 54489047+ParsaGhadermazi@users.noreply.github.com
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```

