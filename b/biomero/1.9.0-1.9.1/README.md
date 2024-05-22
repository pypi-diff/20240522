# Comparing `tmp/biomero-1.9.0.tar.gz` & `tmp/biomero-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/biomero/biomero/dist/.tmp-2z7ckeqa/biomero-1.9.0.tar", last modified: Mon May 13 13:20:09 2024, max compression
+gzip compressed data, was "/home/runner/work/biomero/biomero/dist/.tmp-fo89atde/biomero-1.9.1.tar", last modified: Wed May 22 14:24:48 2024, max compression
```

## Comparing `biomero-1.9.0.tar` & `biomero-1.9.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-13 13:20:03.000000 biomero-1.9.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-13 13:20:03.000000 biomero-1.9.0/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-13 13:20:03.000000 biomero-1.9.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-13 13:20:03.000000 biomero-1.9.0/.github/workflows/sphinx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-13 13:20:03.000000 biomero-1.9.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-13 13:20:03.000000 biomero-1.9.0/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-13 13:20:03.000000 biomero-1.9.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 13:20:03.000000 biomero-1.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    53104 2024-05-13 13:20:09.000000 biomero-1.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    39089 2024-05-13 13:20:03.000000 biomero-1.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/biomero/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-13 13:20:03.000000 biomero-1.9.0/biomero/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-13 13:20:03.000000 biomero-1.9.0/biomero/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    82826 2024-05-13 13:20:03.000000 biomero-1.9.0/biomero/slurm_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/biomero.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    53104 2024-05-13 13:20:09.000000 biomero-1.9.0/biomero.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-05-13 13:20:09.000000 biomero-1.9.0/biomero.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 13:20:09.000000 biomero-1.9.0/biomero.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-13 13:20:09.000000 biomero-1.9.0/biomero.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-13 13:20:09.000000 biomero-1.9.0/biomero.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-13 13:20:03.000000 biomero-1.9.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-13 13:20:03.000000 biomero-1.9.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-13 13:20:03.000000 biomero-1.9.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-13 13:20:03.000000 biomero-1.9.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-13 13:20:03.000000 biomero-1.9.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-13 13:20:03.000000 biomero-1.9.0/docs/omero_slurm_client.rst
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-13 13:20:03.000000 biomero-1.9.0/docs/readme_link.md
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-13 13:20:03.000000 biomero-1.9.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-13 13:20:03.000000 biomero-1.9.0/docs/tutorial_link.md
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-13 13:20:03.000000 biomero-1.9.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/convert_job_array.sh
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/convert_zarr_to_tiff.def
--rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/convert_zarr_to_tiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/example.config
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/job_template.sh
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/pull_images.sh
--rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/slurm-config.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/resources/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/resources/tutorials/images/
--rw-r--r--   0 runner    (1001) docker     (127)   315936 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/images/Cells.tif
--rw-r--r--   0 runner    (1001) docker     (127)   315102 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/images/cellexpansion.png
--rw-r--r--   0 runner    (1001) docker     (127)    83900 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/images/gc_allow_ssh.PNG
--rw-r--r--   0 runner    (1001) docker     (127)   200759 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/images/nuclei_labels.png
--rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/images/webclient_init_env.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    19235 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/images/webclient_init_env_done.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    31403 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/images/webclient_run_cellpose.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    50504 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/images/webclient_run_workflow.PNG
--rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/tutorial_Azure_slurm.md
--rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/tutorial_GoogleCloud_slurm.md
--rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/tutorial_cellexpansion.md
--rw-r--r--   0 runner    (1001) docker     (127)    23085 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/tutorial_cellprofiler.md
--rw-r--r--   0 runner    (1001) docker     (127)    27254 2024-05-13 13:20:03.000000 biomero-1.9.0/resources/tutorials/tutorial_local_slurm.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 13:20:09.000000 biomero-1.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:03.000000 biomero-1.9.0/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:09.000000 biomero-1.9.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 13:20:03.000000 biomero-1.9.0/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45395 2024-05-13 13:20:03.000000 biomero-1.9.0/tests/unit/test_slurm_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:24:48.000000 biomero-1.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 14:24:42.000000 biomero-1.9.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:24:48.000000 biomero-1.9.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:24:48.000000 biomero-1.9.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-22 14:24:42.000000 biomero-1.9.1/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-22 14:24:42.000000 biomero-1.9.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-05-22 14:24:42.000000 biomero-1.9.1/.github/workflows/sphinx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-22 14:24:42.000000 biomero-1.9.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-22 14:24:42.000000 biomero-1.9.1/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 14:24:42.000000 biomero-1.9.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 14:24:42.000000 biomero-1.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    53104 2024-05-22 14:24:48.000000 biomero-1.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    39089 2024-05-22 14:24:42.000000 biomero-1.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:24:48.000000 biomero-1.9.1/biomero/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-22 14:24:42.000000 biomero-1.9.1/biomero/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4250 2024-05-22 14:24:42.000000 biomero-1.9.1/biomero/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    82830 2024-05-22 14:24:42.000000 biomero-1.9.1/biomero/slurm_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:24:48.000000 biomero-1.9.1/biomero.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    53104 2024-05-22 14:24:48.000000 biomero-1.9.1/biomero.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-22 14:24:48.000000 biomero-1.9.1/biomero.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:24:48.000000 biomero-1.9.1/biomero.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-22 14:24:48.000000 biomero-1.9.1/biomero.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 14:24:48.000000 biomero-1.9.1/biomero.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:24:48.000000 biomero-1.9.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-22 14:24:42.000000 biomero-1.9.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-22 14:24:42.000000 biomero-1.9.1/docs/biomero.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-05-22 14:24:42.000000 biomero-1.9.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-22 14:24:42.000000 biomero-1.9.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-22 14:24:42.000000 biomero-1.9.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-22 14:24:42.000000 biomero-1.9.1/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 14:24:42.000000 biomero-1.9.1/docs/readme_link.md
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-22 14:24:42.000000 biomero-1.9.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-22 14:24:42.000000 biomero-1.9.1/docs/tutorial_link.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-22 14:24:42.000000 biomero-1.9.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:24:48.000000 biomero-1.9.1/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:24:42.000000 biomero-1.9.1/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-22 14:24:42.000000 biomero-1.9.1/resources/convert_job_array.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-22 14:24:42.000000 biomero-1.9.1/resources/convert_zarr_to_tiff.def
+-rw-r--r--   0 runner    (1001) docker     (127)     3341 2024-05-22 14:24:42.000000 biomero-1.9.1/resources/convert_zarr_to_tiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-22 14:24:42.000000 biomero-1.9.1/resources/example.config
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-05-22 14:24:42.000000 biomero-1.9.1/resources/job_template.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-22 14:24:42.000000 biomero-1.9.1/resources/pull_images.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     5693 2024-05-22 14:24:42.000000 biomero-1.9.1/resources/slurm-config.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:24:48.000000 biomero-1.9.1/resources/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:24:48.000000 biomero-1.9.1/resources/tutorials/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   315936 2024-05-22 14:24:42.000000 biomero-1.9.1/resources/tutorials/images/Cells.tif
+-rw-r--r--   0 runner    (1001) docker     (127)   315102 2024-05-22 14:24:42.000000 biomero-1.9.1/resources/tutorials/images/cellexpansion.png
+-rw-r--r--   0 runner    (1001) docker     (127)    83900 2024-05-22 14:24:42.000000 biomero-1.9.1/resources/tutorials/images/gc_allow_ssh.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)   200759 2024-05-22 14:24:42.000000 biomero-1.9.1/resources/tutorials/images/nuclei_labels.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12795 2024-05-22 14:24:42.000000 biomero-1.9.1/resources/tutorials/images/webclient_init_env.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    19235 2024-05-22 14:24:42.000000 biomero-1.9.1/resources/tutorials/images/webclient_init_env_done.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    31403 2024-05-22 14:24:42.000000 biomero-1.9.1/resources/tutorials/images/webclient_run_cellpose.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    50504 2024-05-22 14:24:42.000000 biomero-1.9.1/resources/tutorials/images/webclient_run_workflow.PNG
+-rw-r--r--   0 runner    (1001) docker     (127)    21942 2024-05-22 14:24:42.000000 biomero-1.9.1/resources/tutorials/tutorial_Azure_slurm.md
+-rw-r--r--   0 runner    (1001) docker     (127)    14671 2024-05-22 14:24:42.000000 biomero-1.9.1/resources/tutorials/tutorial_GoogleCloud_slurm.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-22 14:24:42.000000 biomero-1.9.1/resources/tutorials/tutorial_cellexpansion.md
+-rw-r--r--   0 runner    (1001) docker     (127)    23085 2024-05-22 14:24:42.000000 biomero-1.9.1/resources/tutorials/tutorial_cellprofiler.md
+-rw-r--r--   0 runner    (1001) docker     (127)    27254 2024-05-22 14:24:42.000000 biomero-1.9.1/resources/tutorials/tutorial_local_slurm.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 14:24:48.000000 biomero-1.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:24:48.000000 biomero-1.9.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:24:48.000000 biomero-1.9.1/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:24:42.000000 biomero-1.9.1/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:24:48.000000 biomero-1.9.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:24:42.000000 biomero-1.9.1/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45395 2024-05-22 14:24:42.000000 biomero-1.9.1/tests/unit/test_slurm_client.py
```

### Comparing `biomero-1.9.0/.github/workflows/python-package.yml` & `biomero-1.9.1/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/.github/workflows/python-publish.yml` & `biomero-1.9.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/.github/workflows/sphinx.yml` & `biomero-1.9.1/.github/workflows/sphinx.yml`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/.gitignore` & `biomero-1.9.1/.gitignore`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/CITATION.cff` & `biomero-1.9.1/CITATION.cff`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/LICENSE` & `biomero-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/PKG-INFO` & `biomero-1.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biomero
-Version: 1.9.0
+Version: 1.9.1
 Summary: A python library for easy connecting between OMERO (jobs) and a Slurm cluster
 Author: Core Facility - Cellular Imaging
 Author-email: Torec Luik <t.t.luik@amsterdamumc.nl>, cellularimaging@amsterdamumc.nl
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `biomero-1.9.0/README.md` & `biomero-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/biomero/constants.py` & `biomero-1.9.1/biomero/constants.py`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/biomero/slurm_client.py` & `biomero-1.9.1/biomero/slurm_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1146,4032 +1146,4032 @@
 00004790: 7273 0a20 2020 2020 2020 2077 6974 6820  rs.        with 
 000047a0: 7365 6c66 2e63 6428 7365 6c66 2e73 6c75  self.cd(self.slu
 000047b0: 726d 5f69 6d61 6765 735f 7061 7468 293a  rm_images_path):
 000047c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
 000047d0: 7365 6c66 2e73 6c75 726d 5f6d 6f64 656c  self.slurm_model
 000047e0: 5f70 6174 6873 3a0a 2020 2020 2020 2020  _paths:.        
 000047f0: 2020 2020 2020 2020 6d6f 6465 6c70 6174          modelpat
-00004800: 6873 203d 2022 2022 2e6a 6f69 6e28 7365  hs = " ".join(se
-00004810: 6c66 2e73 6c75 726d 5f6d 6f64 656c 5f70  lf.slurm_model_p
-00004820: 6174 6873 2e76 616c 7565 7328 2929 0a20  aths.values()). 
-00004830: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00004840: 206d 6b64 6972 2063 656c 6c70 726f 6669   mkdir cellprofi
-00004850: 6c65 7220 696d 6167 656a 202e 2e2e 0a20  ler imagej .... 
-00004860: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00004870: 203d 2073 656c 662e 7275 6e5f 636f 6d6d   = self.run_comm
-00004880: 616e 6473 285b 6622 6d6b 6469 7220 2d70  ands([f"mkdir -p
-00004890: 205c 227b 6d6f 6465 6c70 6174 6873 7d5c   \"{modelpaths}\
-000048a0: 2222 5d29 0a20 2020 2020 2020 2020 2020  ""]).           
-000048b0: 2020 2020 2069 6620 6e6f 7420 722e 6f6b       if not r.ok
-000048c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000048d0: 2020 2020 2020 7261 6973 6520 5353 4845        raise SSHE
-000048e0: 7863 6570 7469 6f6e 2872 290a 0a20 2020  xception(r)..   
-000048f0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00004900: 2e73 6c75 726d 5f6d 6f64 656c 5f69 6d61  .slurm_model_ima
-00004910: 6765 733a 0a20 2020 2020 2020 2020 2020  ges:.           
-00004920: 2020 2020 2070 756c 6c5f 636f 6d6d 616e       pull_comman
-00004930: 6473 203d 205b 5d0a 2020 2020 2020 2020  ds = [].        
-00004940: 2020 2020 2020 2020 666f 7220 7766 2c20          for wf, 
-00004950: 696d 6167 6520 696e 2073 656c 662e 736c  image in self.sl
-00004960: 7572 6d5f 6d6f 6465 6c5f 696d 6167 6573  urm_model_images
-00004970: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-00004980: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00004990: 706f 203d 2073 656c 662e 736c 7572 6d5f  po = self.slurm_
-000049a0: 6d6f 6465 6c5f 7265 706f 735b 7766 5d0a  model_repos[wf].
-000049b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000049c0: 2020 2020 7061 7468 203d 2073 656c 662e      path = self.
-000049d0: 736c 7572 6d5f 6d6f 6465 6c5f 7061 7468  slurm_model_path
-000049e0: 735b 7766 5d0a 2020 2020 2020 2020 2020  s[wf].          
-000049f0: 2020 2020 2020 2020 2020 5f2c 2076 6572            _, ver
-00004a00: 7369 6f6e 203d 2073 656c 662e 6578 7472  sion = self.extr
-00004a10: 6163 745f 7061 7274 735f 6672 6f6d 5f75  act_parts_from_u
-00004a20: 726c 2872 6570 6f29 0a20 2020 2020 2020  rl(repo).       
-00004a30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00004a40: 7665 7273 696f 6e20 3d3d 2022 6d61 7374  version == "mast
-00004a50: 6572 223a 0a20 2020 2020 2020 2020 2020  er":.           
-00004a60: 2020 2020 2020 2020 2020 2020 2076 6572               ver
-00004a70: 7369 6f6e 203d 2022 6c61 7465 7374 220a  sion = "latest".
-00004a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004a90: 2020 2020 7075 6c6c 5f74 656d 706c 6174      pull_templat
-00004aa0: 6520 3d20 2265 6368 6f20 2773 7461 7274  e = "echo 'start
-00004ab0: 696e 6720 2470 6174 6820 2476 6572 7369  ing $path $versi
-00004ac0: 6f6e 2720 3e3e 2073 696e 672e 6c6f 675c  on' >> sing.log\
-00004ad0: 6e6e 6f68 7570 2073 6820 2d63 205c 2273  nnohup sh -c \"s
-00004ae0: 696e 6775 6c61 7269 7479 2070 756c 6c20  ingularity pull 
-00004af0: 2d2d 6469 7361 626c 652d 6361 6368 6520  --disable-cache 
-00004b00: 2d2d 6469 7220 2470 6174 6820 646f 636b  --dir $path dock
-00004b10: 6572 3a2f 2f24 696d 6167 653a 2476 6572  er://$image:$ver
-00004b20: 7369 6f6e 3b20 6563 686f 2027 6669 6e69  sion; echo 'fini
-00004b30: 7368 6564 2024 7061 7468 2024 7665 7273  shed $path $vers
-00004b40: 696f 6e27 5c22 203e 3e20 7369 6e67 2e6c  ion'\" >> sing.l
-00004b50: 6f67 2032 3e26 3120 2620 6469 736f 776e  og 2>&1 & disown
-00004b60: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00004b70: 2020 2020 2020 7420 3d20 5465 6d70 6c61        t = Templa
-00004b80: 7465 2870 756c 6c5f 7465 6d70 6c61 7465  te(pull_template
-00004b90: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00004ba0: 2020 2020 2020 7375 6273 7469 7475 7465        substitute
-00004bb0: 7320 3d20 7b7d 0a20 2020 2020 2020 2020  s = {}.         
-00004bc0: 2020 2020 2020 2020 2020 2073 7562 7374             subst
-00004bd0: 6974 7574 6573 5b27 7061 7468 275d 203d  itutes['path'] =
-00004be0: 2070 6174 680a 2020 2020 2020 2020 2020   path.          
-00004bf0: 2020 2020 2020 2020 2020 7375 6273 7469            substi
-00004c00: 7475 7465 735b 2769 6d61 6765 275d 203d  tutes['image'] =
-00004c10: 2069 6d61 6765 0a20 2020 2020 2020 2020   image.         
-00004c20: 2020 2020 2020 2020 2020 2073 7562 7374             subst
-00004c30: 6974 7574 6573 5b27 7665 7273 696f 6e27  itutes['version'
-00004c40: 5d20 3d20 7665 7273 696f 6e0a 2020 2020  ] = version.    
+00004800: 6873 203d 2022 5c22 205c 2222 2e6a 6f69  hs = "\" \"".joi
+00004810: 6e28 7365 6c66 2e73 6c75 726d 5f6d 6f64  n(self.slurm_mod
+00004820: 656c 5f70 6174 6873 2e76 616c 7565 7328  el_paths.values(
+00004830: 2929 0a20 2020 2020 2020 2020 2020 2020  )).             
+00004840: 2020 2023 206d 6b64 6972 2063 656c 6c70     # mkdir cellp
+00004850: 726f 6669 6c65 7220 696d 6167 656a 202e  rofiler imagej .
+00004860: 2e2e 0a20 2020 2020 2020 2020 2020 2020  ...             
+00004870: 2020 2072 203d 2073 656c 662e 7275 6e5f     r = self.run_
+00004880: 636f 6d6d 616e 6473 285b 6622 6d6b 6469  commands([f"mkdi
+00004890: 7220 2d70 205c 227b 6d6f 6465 6c70 6174  r -p \"{modelpat
+000048a0: 6873 7d5c 2222 5d29 0a20 2020 2020 2020  hs}\""]).       
+000048b0: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+000048c0: 722e 6f6b 3a0a 2020 2020 2020 2020 2020  r.ok:.          
+000048d0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
+000048e0: 5353 4845 7863 6570 7469 6f6e 2872 290a  SSHException(r).
+000048f0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00004900: 7365 6c66 2e73 6c75 726d 5f6d 6f64 656c  self.slurm_model
+00004910: 5f69 6d61 6765 733a 0a20 2020 2020 2020  _images:.       
+00004920: 2020 2020 2020 2020 2070 756c 6c5f 636f           pull_co
+00004930: 6d6d 616e 6473 203d 205b 5d0a 2020 2020  mmands = [].    
+00004940: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00004950: 7766 2c20 696d 6167 6520 696e 2073 656c  wf, image in sel
+00004960: 662e 736c 7572 6d5f 6d6f 6465 6c5f 696d  f.slurm_model_im
+00004970: 6167 6573 2e69 7465 6d73 2829 3a0a 2020  ages.items():.  
+00004980: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004990: 2020 7265 706f 203d 2073 656c 662e 736c    repo = self.sl
+000049a0: 7572 6d5f 6d6f 6465 6c5f 7265 706f 735b  urm_model_repos[
+000049b0: 7766 5d0a 2020 2020 2020 2020 2020 2020  wf].            
+000049c0: 2020 2020 2020 2020 7061 7468 203d 2073          path = s
+000049d0: 656c 662e 736c 7572 6d5f 6d6f 6465 6c5f  elf.slurm_model_
+000049e0: 7061 7468 735b 7766 5d0a 2020 2020 2020  paths[wf].      
+000049f0: 2020 2020 2020 2020 2020 2020 2020 5f2c                _,
+00004a00: 2076 6572 7369 6f6e 203d 2073 656c 662e   version = self.
+00004a10: 6578 7472 6163 745f 7061 7274 735f 6672  extract_parts_fr
+00004a20: 6f6d 5f75 726c 2872 6570 6f29 0a20 2020  om_url(repo).   
+00004a30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a40: 2069 6620 7665 7273 696f 6e20 3d3d 2022   if version == "
+00004a50: 6d61 7374 6572 223a 0a20 2020 2020 2020  master":.       
+00004a60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004a70: 2076 6572 7369 6f6e 203d 2022 6c61 7465   version = "late
+00004a80: 7374 220a 2020 2020 2020 2020 2020 2020  st".            
+00004a90: 2020 2020 2020 2020 7075 6c6c 5f74 656d          pull_tem
+00004aa0: 706c 6174 6520 3d20 2265 6368 6f20 2773  plate = "echo 's
+00004ab0: 7461 7274 696e 6720 2470 6174 6820 2476  tarting $path $v
+00004ac0: 6572 7369 6f6e 2720 3e3e 2073 696e 672e  ersion' >> sing.
+00004ad0: 6c6f 675c 6e6e 6f68 7570 2073 6820 2d63  log\nnohup sh -c
+00004ae0: 205c 2273 696e 6775 6c61 7269 7479 2070   \"singularity p
+00004af0: 756c 6c20 2d2d 6469 7361 626c 652d 6361  ull --disable-ca
+00004b00: 6368 6520 2d2d 6469 7220 2470 6174 6820  che --dir $path 
+00004b10: 646f 636b 6572 3a2f 2f24 696d 6167 653a  docker://$image:
+00004b20: 2476 6572 7369 6f6e 3b20 6563 686f 2027  $version; echo '
+00004b30: 6669 6e69 7368 6564 2024 7061 7468 2024  finished $path $
+00004b40: 7665 7273 696f 6e27 5c22 203e 3e20 7369  version'\" >> si
+00004b50: 6e67 2e6c 6f67 2032 3e26 3120 2620 6469  ng.log 2>&1 & di
+00004b60: 736f 776e 220a 2020 2020 2020 2020 2020  sown".          
+00004b70: 2020 2020 2020 2020 2020 7420 3d20 5465            t = Te
+00004b80: 6d70 6c61 7465 2870 756c 6c5f 7465 6d70  mplate(pull_temp
+00004b90: 6c61 7465 290a 2020 2020 2020 2020 2020  late).          
+00004ba0: 2020 2020 2020 2020 2020 7375 6273 7469            substi
+00004bb0: 7475 7465 7320 3d20 7b7d 0a20 2020 2020  tutes = {}.     
+00004bc0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004bd0: 7562 7374 6974 7574 6573 5b27 7061 7468  ubstitutes['path
+00004be0: 275d 203d 2070 6174 680a 2020 2020 2020  '] = path.      
+00004bf0: 2020 2020 2020 2020 2020 2020 2020 7375                su
+00004c00: 6273 7469 7475 7465 735b 2769 6d61 6765  bstitutes['image
+00004c10: 275d 203d 2069 6d61 6765 0a20 2020 2020  '] = image.     
+00004c20: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004c30: 7562 7374 6974 7574 6573 5b27 7665 7273  ubstitutes['vers
+00004c40: 696f 6e27 5d20 3d20 7665 7273 696f 6e0a  ion'] = version.
 00004c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c60: 636d 6420 3d20 742e 7361 6665 5f73 7562  cmd = t.safe_sub
-00004c70: 7374 6974 7574 6528 7375 6273 7469 7475  stitute(substitu
-00004c80: 7465 7329 0a20 2020 2020 2020 2020 2020  tes).           
-00004c90: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00004ca0: 6465 6275 6728 6622 7375 6273 7469 7475  debug(f"substitu
-00004cb0: 7465 643a 207b 636d 647d 2229 0a20 2020  ted: {cmd}").   
-00004cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004cd0: 2070 756c 6c5f 636f 6d6d 616e 6473 2e61   pull_commands.a
-00004ce0: 7070 656e 6428 636d 6429 0a20 2020 2020  ppend(cmd).     
-00004cf0: 2020 2020 2020 2020 2020 2073 6372 6970             scrip
-00004d00: 745f 6e61 6d65 203d 2022 7075 6c6c 5f69  t_name = "pull_i
-00004d10: 6d61 6765 732e 7368 220a 2020 2020 2020  mages.sh".      
-00004d20: 2020 2020 2020 2020 2020 7465 6d70 6c61            templa
-00004d30: 7465 5f73 6372 6970 7420 3d20 6669 6c65  te_script = file
-00004d40: 7328 2272 6573 6f75 7263 6573 2229 2e6a  s("resources").j
-00004d50: 6f69 6e70 6174 6828 7363 7269 7074 5f6e  oinpath(script_n
-00004d60: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-00004d70: 2020 2020 2077 6974 6820 7465 6d70 6c61       with templa
-00004d80: 7465 5f73 6372 6970 742e 6f70 656e 2827  te_script.open('
-00004d90: 7227 2920 6173 2066 3a0a 2020 2020 2020  r') as f:.      
-00004da0: 2020 2020 2020 2020 2020 2020 2020 7372                sr
-00004db0: 6320 3d20 5465 6d70 6c61 7465 2866 2e72  c = Template(f.r
-00004dc0: 6561 6428 2929 0a20 2020 2020 2020 2020  ead()).         
-00004dd0: 2020 2020 2020 2020 2020 2073 7562 7374             subst
-00004de0: 6974 7574 6520 3d20 7b27 7075 6c6c 636f  itute = {'pullco
-00004df0: 6d6d 616e 6473 273a 2022 5c6e 222e 6a6f  mmands': "\n".jo
-00004e00: 696e 2870 756c 6c5f 636f 6d6d 616e 6473  in(pull_commands
-00004e10: 297d 0a20 2020 2020 2020 2020 2020 2020  )}.             
-00004e20: 2020 2020 2020 206a 6f62 5f73 6372 6970         job_scrip
-00004e30: 7420 3d20 7372 632e 7361 6665 5f73 7562  t = src.safe_sub
-00004e40: 7374 6974 7574 6528 7375 6273 7469 7475  stitute(substitu
-00004e50: 7465 290a 2020 2020 2020 2020 2020 2020  te).            
-00004e60: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
-00004e70: 2866 2273 7562 7374 6974 7574 6564 3a5c  (f"substituted:\
-00004e80: 6e20 7b6a 6f62 5f73 6372 6970 747d 2229  n {job_script}")
-00004e90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004ea0: 2023 2063 6f70 7920 746f 2072 656d 6f74   # copy to remot
-00004eb0: 6520 6669 6c65 0a20 2020 2020 2020 2020  e file.         
-00004ec0: 2020 2020 2020 2066 756c 6c5f 7061 7468         full_path
-00004ed0: 203d 2073 656c 662e 736c 7572 6d5f 696d   = self.slurm_im
-00004ee0: 6167 6573 5f70 6174 682b 222f 222b 7363  ages_path+"/"+sc
-00004ef0: 7269 7074 5f6e 616d 650a 2020 2020 2020  ript_name.      
-00004f00: 2020 2020 2020 2020 2020 5f20 3d20 7365            _ = se
-00004f10: 6c66 2e70 7574 286c 6f63 616c 3d69 6f2e  lf.put(local=io.
-00004f20: 5374 7269 6e67 494f 286a 6f62 5f73 6372  StringIO(job_scr
-00004f30: 6970 7429 2c0a 2020 2020 2020 2020 2020  ipt),.          
+00004c60: 2020 2020 636d 6420 3d20 742e 7361 6665      cmd = t.safe
+00004c70: 5f73 7562 7374 6974 7574 6528 7375 6273  _substitute(subs
+00004c80: 7469 7475 7465 7329 0a20 2020 2020 2020  titutes).       
+00004c90: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00004ca0: 6765 722e 6465 6275 6728 6622 7375 6273  ger.debug(f"subs
+00004cb0: 7469 7475 7465 643a 207b 636d 647d 2229  tituted: {cmd}")
+00004cc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00004cd0: 2020 2020 2070 756c 6c5f 636f 6d6d 616e       pull_comman
+00004ce0: 6473 2e61 7070 656e 6428 636d 6429 0a20  ds.append(cmd). 
+00004cf0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004d00: 6372 6970 745f 6e61 6d65 203d 2022 7075  cript_name = "pu
+00004d10: 6c6c 5f69 6d61 6765 732e 7368 220a 2020  ll_images.sh".  
+00004d20: 2020 2020 2020 2020 2020 2020 2020 7465                te
+00004d30: 6d70 6c61 7465 5f73 6372 6970 7420 3d20  mplate_script = 
+00004d40: 6669 6c65 7328 2272 6573 6f75 7263 6573  files("resources
+00004d50: 2229 2e6a 6f69 6e70 6174 6828 7363 7269  ").joinpath(scri
+00004d60: 7074 5f6e 616d 6529 0a20 2020 2020 2020  pt_name).       
+00004d70: 2020 2020 2020 2020 2077 6974 6820 7465           with te
+00004d80: 6d70 6c61 7465 5f73 6372 6970 742e 6f70  mplate_script.op
+00004d90: 656e 2827 7227 2920 6173 2066 3a0a 2020  en('r') as f:.  
+00004da0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004db0: 2020 7372 6320 3d20 5465 6d70 6c61 7465    src = Template
+00004dc0: 2866 2e72 6561 6428 2929 0a20 2020 2020  (f.read()).     
+00004dd0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00004de0: 7562 7374 6974 7574 6520 3d20 7b27 7075  ubstitute = {'pu
+00004df0: 6c6c 636f 6d6d 616e 6473 273a 2022 5c6e  llcommands': "\n
+00004e00: 222e 6a6f 696e 2870 756c 6c5f 636f 6d6d  ".join(pull_comm
+00004e10: 616e 6473 297d 0a20 2020 2020 2020 2020  ands)}.         
+00004e20: 2020 2020 2020 2020 2020 206a 6f62 5f73             job_s
+00004e30: 6372 6970 7420 3d20 7372 632e 7361 6665  cript = src.safe
+00004e40: 5f73 7562 7374 6974 7574 6528 7375 6273  _substitute(subs
+00004e50: 7469 7475 7465 290a 2020 2020 2020 2020  titute).        
+00004e60: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
+00004e70: 6562 7567 2866 2273 7562 7374 6974 7574  ebug(f"substitut
+00004e80: 6564 3a5c 6e20 7b6a 6f62 5f73 6372 6970  ed:\n {job_scrip
+00004e90: 747d 2229 0a20 2020 2020 2020 2020 2020  t}").           
+00004ea0: 2020 2020 2023 2063 6f70 7920 746f 2072       # copy to r
+00004eb0: 656d 6f74 6520 6669 6c65 0a20 2020 2020  emote file.     
+00004ec0: 2020 2020 2020 2020 2020 2066 756c 6c5f             full_
+00004ed0: 7061 7468 203d 2073 656c 662e 736c 7572  path = self.slur
+00004ee0: 6d5f 696d 6167 6573 5f70 6174 682b 222f  m_images_path+"/
+00004ef0: 222b 7363 7269 7074 5f6e 616d 650a 2020  "+script_name.  
+00004f00: 2020 2020 2020 2020 2020 2020 2020 5f20                _ 
+00004f10: 3d20 7365 6c66 2e70 7574 286c 6f63 616c  = self.put(local
+00004f20: 3d69 6f2e 5374 7269 6e67 494f 286a 6f62  =io.StringIO(job
+00004f30: 5f73 6372 6970 7429 2c0a 2020 2020 2020  _script),.      
 00004f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f50: 2020 2072 656d 6f74 653d 6675 6c6c 5f70     remote=full_p
-00004f60: 6174 6829 0a20 2020 2020 2020 2020 2020  ath).           
-00004f70: 2020 2020 2063 6d64 203d 2066 2274 696d       cmd = f"tim
-00004f80: 6520 7368 207b 7363 7269 7074 5f6e 616d  e sh {script_nam
-00004f90: 657d 220a 2020 2020 2020 2020 2020 2020  e}".            
-00004fa0: 2020 2020 7220 3d20 7365 6c66 2e72 756e      r = self.run
-00004fb0: 5f63 6f6d 6d61 6e64 7328 5b63 6d64 5d29  _commands([cmd])
-00004fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004fd0: 2069 6620 6e6f 7420 722e 6f6b 3a0a 2020   if not r.ok:.  
-00004fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004ff0: 2020 7261 6973 6520 5353 4845 7863 6570    raise SSHExcep
-00005000: 7469 6f6e 2872 290a 2020 2020 2020 2020  tion(r).        
-00005010: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
-00005020: 6e66 6f28 722e 7374 646f 7574 290a 2020  nfo(r.stdout).  
-00005030: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
-00005040: 6767 6572 2e69 6e66 6f28 2249 6e69 7469  gger.info("Initi
-00005050: 6174 6564 2064 6f77 6e6c 6f61 6469 6e67  ated downloading
-00005060: 2061 6e64 2062 7569 6c64 696e 6722 202b   and building" +
-00005070: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005080: 2020 2020 2020 2020 2020 2020 2022 2063               " c
-00005090: 6f6e 7461 696e 6572 2069 6d61 6765 7320  ontainer images 
-000050a0: 6f6e 2053 6c75 726d 2e22 202b 0a20 2020  on Slurm." +.   
-000050b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000050c0: 2020 2020 2020 2020 2022 2054 6869 7320           " This 
-000050d0: 7769 6c6c 2070 726f 6261 626c 7920 7461  will probably ta
-000050e0: 6b65 2061 2077 6869 6c65 2069 6e20 7468  ke a while in th
-000050f0: 6520 6261 636b 6772 6f75 6e64 2e22 202b  e background." +
-00005100: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-00005110: 2020 2020 2020 2020 2020 2020 2020 2220                " 
-00005120: 4368 6563 6b20 2773 696e 672e 6c6f 6727  Check 'sing.log'
-00005130: 206f 6e20 536c 7572 6d20 666f 7220 7072   on Slurm for pr
-00005140: 6f67 7265 7373 2e22 290a 2020 2020 2020  ogress.").      
-00005150: 2020 2020 2020 2020 2020 2320 2320 636c            # # cl
-00005160: 6561 6e75 7020 6769 616e 7420 7369 6e67  eanup giant sing
-00005170: 756c 6172 6974 7920 6361 6368 6521 0a20  ularity cache!. 
-00005180: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00005190: 2075 7369 6e67 202d 2d64 6973 6162 6c65   using --disable
-000051a0: 2d63 6163 6865 2062 6563 6175 7365 2077  -cache because w
-000051b0: 6520 7275 6e20 696e 2074 6865 2062 6163  e run in the bac
-000051c0: 6b67 726f 756e 640a 2020 2020 2020 2020  kground.        
-000051d0: 2020 2020 2020 2020 2320 636d 6420 3d20          # cmd = 
-000051e0: 2273 696e 6775 6c61 7269 7479 2063 6163  "singularity cac
-000051f0: 6865 2063 6c65 616e 202d 6622 0a20 2020  he clean -f".   
-00005200: 2020 2020 2020 2020 2020 2020 2023 2072               # r
-00005210: 203d 2073 656c 662e 7275 6e5f 636f 6d6d   = self.run_comm
-00005220: 616e 6473 285b 636d 645d 290a 0a20 2020  ands([cmd])..   
-00005230: 2064 6566 2073 6574 7570 5f63 6f6e 7665   def setup_conve
-00005240: 7274 6572 7328 7365 6c66 293a 0a20 2020  rters(self):.   
-00005250: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00005260: 2053 6574 7320 7570 2063 6f6e 7665 7274   Sets up convert
-00005270: 6572 7320 666f 7220 536c 7572 6d20 6f70  ers for Slurm op
-00005280: 6572 6174 696f 6e73 2e0a 0a20 2020 2020  erations...     
-00005290: 2020 2054 6869 7320 6675 6e63 7469 6f6e     This function
-000052a0: 2063 7265 6174 6573 206e 6563 6573 7361   creates necessa
-000052b0: 7279 2064 6972 6563 746f 7269 6573 2066  ry directories f
-000052c0: 6f72 2063 6f6e 7665 7274 6572 7320 616e  or converters an
-000052d0: 6420 636f 7069 6573 0a20 2020 2020 2020  d copies.       
-000052e0: 2063 6f6e 7665 7274 6572 2073 6372 6970   converter scrip
-000052f0: 7473 2061 6e64 2064 6566 696e 6974 696f  ts and definitio
-00005300: 6e73 2074 6f20 7468 6520 6170 7072 6f70  ns to the approp
-00005310: 7269 6174 6520 6c6f 6361 7469 6f6e 732e  riate locations.
-00005320: 2049 7420 616c 736f 0a20 2020 2020 2020   It also.       
-00005330: 2062 7569 6c64 7320 5369 6e67 756c 6172   builds Singular
-00005340: 6974 7920 636f 6e74 6169 6e65 7273 2066  ity containers f
-00005350: 726f 6d20 7468 6520 7072 6f76 6964 6564  rom the provided
-00005360: 2064 6566 696e 6974 696f 6e73 2e0a 0a20   definitions... 
-00005370: 2020 2020 2020 2052 6169 7365 733a 0a20         Raises:. 
-00005380: 2020 2020 2020 2020 2020 2053 5348 4578             SSHEx
-00005390: 6365 7074 696f 6e3a 2049 6620 7468 6572  ception: If ther
-000053a0: 6520 6973 2061 6e20 6973 7375 6520 6578  e is an issue ex
-000053b0: 6563 7574 696e 6720 636f 6d6d 616e 6473  ecuting commands
-000053c0: 206f 7220 636f 7079 696e 6720 6669 6c65   or copying file
-000053d0: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
-000053e0: 2020 2020 2020 2063 6f6e 7665 7274 5f63         convert_c
-000053f0: 6d64 7320 3d20 5b5d 0a20 2020 2020 2020  mds = [].       
-00005400: 2069 6620 7365 6c66 2e73 6c75 726d 5f63   if self.slurm_c
-00005410: 6f6e 7665 7274 6572 735f 7061 7468 3a0a  onverters_path:.
-00005420: 2020 2020 2020 2020 2020 2020 636f 6e76              conv
-00005430: 6572 745f 636d 6473 2e61 7070 656e 6428  ert_cmds.append(
-00005440: 6622 6d6b 6469 7220 2d70 205c 227b 7365  f"mkdir -p \"{se
-00005450: 6c66 2e73 6c75 726d 5f63 6f6e 7665 7274  lf.slurm_convert
-00005460: 6572 735f 7061 7468 7d5c 2222 290a 2020  ers_path}\"").  
-00005470: 2020 2020 2020 7220 3d20 7365 6c66 2e72        r = self.r
-00005480: 756e 5f63 6f6d 6d61 6e64 7328 636f 6e76  un_commands(conv
-00005490: 6572 745f 636d 6473 290a 2020 2020 2020  ert_cmds).      
-000054a0: 2020 2320 636f 7079 2067 656e 6572 6963    # copy generic
-000054b0: 206a 6f62 2061 7272 6179 2073 6372 6970   job array scrip
-000054c0: 7420 6f76 6572 2074 6f20 736c 7572 6d0a  t over to slurm.
-000054d0: 2020 2020 2020 2020 636f 6e76 6572 745f          convert_
-000054e0: 6a6f 625f 6c6f 6361 6c20 3d20 6669 6c65  job_local = file
-000054f0: 7328 2272 6573 6f75 7263 6573 2229 2e6a  s("resources").j
-00005500: 6f69 6e70 6174 6828 0a20 2020 2020 2020  oinpath(.       
-00005510: 2020 2020 2022 636f 6e76 6572 745f 6a6f       "convert_jo
-00005520: 625f 6172 7261 792e 7368 2229 0a20 2020  b_array.sh").   
-00005530: 2020 2020 205f 203d 2073 656c 662e 7075       _ = self.pu
-00005540: 7428 6c6f 6361 6c3d 636f 6e76 6572 745f  t(local=convert_
-00005550: 6a6f 625f 6c6f 6361 6c2c 0a20 2020 2020  job_local,.     
+00004f50: 2020 2020 2020 2072 656d 6f74 653d 6675         remote=fu
+00004f60: 6c6c 5f70 6174 6829 0a20 2020 2020 2020  ll_path).       
+00004f70: 2020 2020 2020 2020 2063 6d64 203d 2066           cmd = f
+00004f80: 2274 696d 6520 7368 207b 7363 7269 7074  "time sh {script
+00004f90: 5f6e 616d 657d 220a 2020 2020 2020 2020  _name}".        
+00004fa0: 2020 2020 2020 2020 7220 3d20 7365 6c66          r = self
+00004fb0: 2e72 756e 5f63 6f6d 6d61 6e64 7328 5b63  .run_commands([c
+00004fc0: 6d64 5d29 0a20 2020 2020 2020 2020 2020  md]).           
+00004fd0: 2020 2020 2069 6620 6e6f 7420 722e 6f6b       if not r.ok
+00004fe0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004ff0: 2020 2020 2020 7261 6973 6520 5353 4845        raise SSHE
+00005000: 7863 6570 7469 6f6e 2872 290a 2020 2020  xception(r).    
+00005010: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+00005020: 6572 2e69 6e66 6f28 722e 7374 646f 7574  er.info(r.stdout
+00005030: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00005040: 2020 6c6f 6767 6572 2e69 6e66 6f28 2249    logger.info("I
+00005050: 6e69 7469 6174 6564 2064 6f77 6e6c 6f61  nitiated downloa
+00005060: 6469 6e67 2061 6e64 2062 7569 6c64 696e  ding and buildin
+00005070: 6722 202b 0a20 2020 2020 2020 2020 2020  g" +.           
+00005080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005090: 2022 2063 6f6e 7461 696e 6572 2069 6d61   " container ima
+000050a0: 6765 7320 6f6e 2053 6c75 726d 2e22 202b  ges on Slurm." +
+000050b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000050c0: 2020 2020 2020 2020 2020 2020 2022 2054               " T
+000050d0: 6869 7320 7769 6c6c 2070 726f 6261 626c  his will probabl
+000050e0: 7920 7461 6b65 2061 2077 6869 6c65 2069  y take a while i
+000050f0: 6e20 7468 6520 6261 636b 6772 6f75 6e64  n the background
+00005100: 2e22 202b 200a 2020 2020 2020 2020 2020  ." + .          
+00005110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005120: 2020 2220 4368 6563 6b20 2773 696e 672e    " Check 'sing.
+00005130: 6c6f 6727 206f 6e20 536c 7572 6d20 666f  log' on Slurm fo
+00005140: 7220 7072 6f67 7265 7373 2e22 290a 2020  r progress.").  
+00005150: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00005160: 2320 636c 6561 6e75 7020 6769 616e 7420  # cleanup giant 
+00005170: 7369 6e67 756c 6172 6974 7920 6361 6368  singularity cach
+00005180: 6521 0a20 2020 2020 2020 2020 2020 2020  e!.             
+00005190: 2020 2023 2075 7369 6e67 202d 2d64 6973     # using --dis
+000051a0: 6162 6c65 2d63 6163 6865 2062 6563 6175  able-cache becau
+000051b0: 7365 2077 6520 7275 6e20 696e 2074 6865  se we run in the
+000051c0: 2062 6163 6b67 726f 756e 640a 2020 2020   background.    
+000051d0: 2020 2020 2020 2020 2020 2020 2320 636d              # cm
+000051e0: 6420 3d20 2273 696e 6775 6c61 7269 7479  d = "singularity
+000051f0: 2063 6163 6865 2063 6c65 616e 202d 6622   cache clean -f"
+00005200: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005210: 2023 2072 203d 2073 656c 662e 7275 6e5f   # r = self.run_
+00005220: 636f 6d6d 616e 6473 285b 636d 645d 290a  commands([cmd]).
+00005230: 0a20 2020 2064 6566 2073 6574 7570 5f63  .    def setup_c
+00005240: 6f6e 7665 7274 6572 7328 7365 6c66 293a  onverters(self):
+00005250: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00005260: 2020 2020 2053 6574 7320 7570 2063 6f6e       Sets up con
+00005270: 7665 7274 6572 7320 666f 7220 536c 7572  verters for Slur
+00005280: 6d20 6f70 6572 6174 696f 6e73 2e0a 0a20  m operations... 
+00005290: 2020 2020 2020 2054 6869 7320 6675 6e63         This func
+000052a0: 7469 6f6e 2063 7265 6174 6573 206e 6563  tion creates nec
+000052b0: 6573 7361 7279 2064 6972 6563 746f 7269  essary directori
+000052c0: 6573 2066 6f72 2063 6f6e 7665 7274 6572  es for converter
+000052d0: 7320 616e 6420 636f 7069 6573 0a20 2020  s and copies.   
+000052e0: 2020 2020 2063 6f6e 7665 7274 6572 2073       converter s
+000052f0: 6372 6970 7473 2061 6e64 2064 6566 696e  cripts and defin
+00005300: 6974 696f 6e73 2074 6f20 7468 6520 6170  itions to the ap
+00005310: 7072 6f70 7269 6174 6520 6c6f 6361 7469  propriate locati
+00005320: 6f6e 732e 2049 7420 616c 736f 0a20 2020  ons. It also.   
+00005330: 2020 2020 2062 7569 6c64 7320 5369 6e67       builds Sing
+00005340: 756c 6172 6974 7920 636f 6e74 6169 6e65  ularity containe
+00005350: 7273 2066 726f 6d20 7468 6520 7072 6f76  rs from the prov
+00005360: 6964 6564 2064 6566 696e 6974 696f 6e73  ided definitions
+00005370: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
+00005380: 733a 0a20 2020 2020 2020 2020 2020 2053  s:.            S
+00005390: 5348 4578 6365 7074 696f 6e3a 2049 6620  SHException: If 
+000053a0: 7468 6572 6520 6973 2061 6e20 6973 7375  there is an issu
+000053b0: 6520 6578 6563 7574 696e 6720 636f 6d6d  e executing comm
+000053c0: 616e 6473 206f 7220 636f 7079 696e 6720  ands or copying 
+000053d0: 6669 6c65 732e 0a20 2020 2020 2020 2022  files..        "
+000053e0: 2222 0a20 2020 2020 2020 2063 6f6e 7665  "".        conve
+000053f0: 7274 5f63 6d64 7320 3d20 5b5d 0a20 2020  rt_cmds = [].   
+00005400: 2020 2020 2069 6620 7365 6c66 2e73 6c75       if self.slu
+00005410: 726d 5f63 6f6e 7665 7274 6572 735f 7061  rm_converters_pa
+00005420: 7468 3a0a 2020 2020 2020 2020 2020 2020  th:.            
+00005430: 636f 6e76 6572 745f 636d 6473 2e61 7070  convert_cmds.app
+00005440: 656e 6428 6622 6d6b 6469 7220 2d70 205c  end(f"mkdir -p \
+00005450: 227b 7365 6c66 2e73 6c75 726d 5f63 6f6e  "{self.slurm_con
+00005460: 7665 7274 6572 735f 7061 7468 7d5c 2222  verters_path}\""
+00005470: 290a 2020 2020 2020 2020 7220 3d20 7365  ).        r = se
+00005480: 6c66 2e72 756e 5f63 6f6d 6d61 6e64 7328  lf.run_commands(
+00005490: 636f 6e76 6572 745f 636d 6473 290a 2020  convert_cmds).  
+000054a0: 2020 2020 2020 2320 636f 7079 2067 656e        # copy gen
+000054b0: 6572 6963 206a 6f62 2061 7272 6179 2073  eric job array s
+000054c0: 6372 6970 7420 6f76 6572 2074 6f20 736c  cript over to sl
+000054d0: 7572 6d0a 2020 2020 2020 2020 636f 6e76  urm.        conv
+000054e0: 6572 745f 6a6f 625f 6c6f 6361 6c20 3d20  ert_job_local = 
+000054f0: 6669 6c65 7328 2272 6573 6f75 7263 6573  files("resources
+00005500: 2229 2e6a 6f69 6e70 6174 6828 0a20 2020  ").joinpath(.   
+00005510: 2020 2020 2020 2020 2022 636f 6e76 6572           "conver
+00005520: 745f 6a6f 625f 6172 7261 792e 7368 2229  t_job_array.sh")
+00005530: 0a20 2020 2020 2020 205f 203d 2073 656c  .        _ = sel
+00005540: 662e 7075 7428 6c6f 6361 6c3d 636f 6e76  f.put(local=conv
+00005550: 6572 745f 6a6f 625f 6c6f 6361 6c2c 0a20  ert_job_local,. 
 00005560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005570: 7265 6d6f 7465 3d73 656c 662e 736c 7572  remote=self.slur
-00005580: 6d5f 7363 7269 7074 5f70 6174 6829 0a20  m_script_path). 
-00005590: 2020 2020 2020 2023 2063 7572 7265 6e74         # current
-000055a0: 6c79 206b 6e6f 776e 2063 6f6e 7665 7274  ly known convert
-000055b0: 6572 730a 2020 2020 2020 2020 2320 3361  ers.        # 3a
-000055c0: 2e20 5a41 5252 2074 6f20 5449 4646 0a20  . ZARR to TIFF. 
-000055d0: 2020 2020 2020 2023 2054 4f44 4f20 6578         # TODO ex
-000055e0: 7472 6163 7420 7468 6573 6520 7661 6c75  tract these valu
-000055f0: 6573 2074 6f20 652e 672e 2063 6f6e 6669  es to e.g. confi
-00005600: 6720 6966 2077 6520 6861 7665 206d 6f72  g if we have mor
-00005610: 650a 2020 2020 2020 2020 636f 6e76 6572  e.        conver
-00005620: 745f 6e61 6d65 203d 2022 636f 6e76 6572  t_name = "conver
-00005630: 745f 7a61 7272 5f74 6f5f 7469 6666 220a  t_zarr_to_tiff".
-00005640: 2020 2020 2020 2020 636f 6e76 6572 745f          convert_
-00005650: 7079 203d 2066 227b 636f 6e76 6572 745f  py = f"{convert_
-00005660: 6e61 6d65 7d2e 7079 220a 2020 2020 2020  name}.py".      
-00005670: 2020 636f 6e76 6572 745f 7363 7269 7074    convert_script
-00005680: 5f6c 6f63 616c 203d 2066 696c 6573 2822  _local = files("
-00005690: 7265 736f 7572 6365 7322 292e 6a6f 696e  resources").join
-000056a0: 7061 7468 280a 2020 2020 2020 2020 2020  path(.          
-000056b0: 2020 636f 6e76 6572 745f 7079 290a 2020    convert_py).  
-000056c0: 2020 2020 2020 636f 6e76 6572 745f 6465        convert_de
-000056d0: 6620 3d20 6622 7b63 6f6e 7665 7274 5f6e  f = f"{convert_n
-000056e0: 616d 657d 2e64 6566 220a 2020 2020 2020  ame}.def".      
-000056f0: 2020 636f 6e76 6572 745f 6465 665f 6c6f    convert_def_lo
-00005700: 6361 6c20 3d20 6669 6c65 7328 2272 6573  cal = files("res
-00005710: 6f75 7263 6573 2229 2e6a 6f69 6e70 6174  ources").joinpat
-00005720: 6828 0a20 2020 2020 2020 2020 2020 2063  h(.            c
-00005730: 6f6e 7665 7274 5f64 6566 290a 2020 2020  onvert_def).    
-00005740: 2020 2020 5f20 3d20 7365 6c66 2e70 7574      _ = self.put
-00005750: 286c 6f63 616c 3d63 6f6e 7665 7274 5f73  (local=convert_s
-00005760: 6372 6970 745f 6c6f 6361 6c2c 0a20 2020  cript_local,.   
-00005770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005780: 2020 7265 6d6f 7465 3d73 656c 662e 736c    remote=self.sl
-00005790: 7572 6d5f 636f 6e76 6572 7465 7273 5f70  urm_converters_p
-000057a0: 6174 6829 0a20 2020 2020 2020 205f 203d  ath).        _ =
-000057b0: 2073 656c 662e 7075 7428 6c6f 6361 6c3d   self.put(local=
-000057c0: 636f 6e76 6572 745f 6465 665f 6c6f 6361  convert_def_loca
-000057d0: 6c2c 0a20 2020 2020 2020 2020 2020 2020  l,.             
-000057e0: 2020 2020 2020 2020 7265 6d6f 7465 3d73          remote=s
-000057f0: 656c 662e 736c 7572 6d5f 636f 6e76 6572  elf.slurm_conver
-00005800: 7465 7273 5f70 6174 6829 0a20 2020 2020  ters_path).     
-00005810: 2020 2023 2042 7569 6c64 2073 696e 6775     # Build singu
-00005820: 6c61 7269 7479 2063 6f6e 7461 696e 6572  larity container
-00005830: 2066 726f 6d20 6465 6669 6e69 7469 6f6e   from definition
-00005840: 0a20 2020 2020 2020 2077 6974 6820 7365  .        with se
-00005850: 6c66 2e63 6428 7365 6c66 2e73 6c75 726d  lf.cd(self.slurm
-00005860: 5f63 6f6e 7665 7274 6572 735f 7061 7468  _converters_path
-00005870: 293a 0a20 2020 2020 2020 2020 2020 2063  ):.            c
-00005880: 6f6e 7665 7274 5f63 6d64 7320 3d20 5b5d  onvert_cmds = []
-00005890: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000058a0: 7365 6c66 2e73 6c75 726d 5f69 6d61 6765  self.slurm_image
-000058b0: 735f 7061 7468 3a0a 2020 2020 2020 2020  s_path:.        
-000058c0: 2020 2020 2020 2020 2320 544f 444f 2043          # TODO C
-000058d0: 6861 6e67 6520 7468 6520 746d 7020 6469  hange the tmp di
-000058e0: 723f 0a20 2020 2020 2020 2020 2020 2020  r?.             
-000058f0: 2020 2023 2065 7870 6f72 7420 5349 4e47     # export SING
-00005900: 554c 4152 4954 595f 544d 5044 4952 3d7e  ULARITY_TMPDIR=~
-00005910: 2f6d 792d 7363 7261 7463 682f 746d 703b  /my-scratch/tmp;
-00005920: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005930: 2023 206f 6e6c 7920 6966 2066 696c 6520   # only if file 
-00005940: 646f 6573 206e 6f74 2065 7869 7374 2079  does not exist y
-00005950: 6574 0a20 2020 2020 2020 2020 2020 2020  et.             
-00005960: 2020 2023 2063 6f6e 7665 7274 5f63 6d64     # convert_cmd
-00005970: 732e 6170 7065 6e64 2866 225b 2021 202d  s.append(f"[ ! -
-00005980: 6620 7b63 6f6e 7665 7274 5f6e 616d 657d  f {convert_name}
-00005990: 2e73 6966 205d 2229 0a20 2020 2020 2020  .sif ]").       
-000059a0: 2020 2020 2020 2020 2023 2045 4449 5420           # EDIT 
-000059b0: 2d2d 204e 4f2c 2074 6865 6e20 7765 2063  -- NO, then we c
-000059c0: 616e 2774 2075 7064 6174 6521 2046 6f72  an't update! For
-000059d0: 6365 2072 6562 7569 6c64 210a 2020 2020  ce rebuild!.    
-000059e0: 2020 2020 2020 2020 2020 2020 2320 646f              # do
-000059f0: 776e 6c6f 6164 202f 6275 696c 6420 6e65  wnload /build ne
-00005a00: 7720 636f 6e74 6169 6e65 720a 2020 2020  w container.    
-00005a10: 2020 2020 2020 2020 2020 2020 636f 6e76              conv
-00005a20: 6572 745f 636d 6473 2e61 7070 656e 6428  ert_cmds.append(
-00005a30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005a40: 2020 2020 2066 2273 696e 6775 6c61 7269       f"singulari
-00005a50: 7479 2062 7569 6c64 202d 4620 5c22 7b63  ty build -F \"{c
-00005a60: 6f6e 7665 7274 5f6e 616d 657d 2e73 6966  onvert_name}.sif
-00005a70: 5c22 207b 636f 6e76 6572 745f 6465 667d  \" {convert_def}
-00005a80: 203e 3e20 7369 6e67 2e6c 6f67 2032 3e26   >> sing.log 2>&
-00005a90: 3120 3b20 6563 686f 2027 6669 6e69 7368  1 ; echo 'finish
-00005aa0: 6564 207b 636f 6e76 6572 745f 6e61 6d65  ed {convert_name
-00005ab0: 7d2e 7369 6627 2026 2229 0a20 2020 2020  }.sif' &").     
-00005ac0: 2020 2020 2020 205f 203d 2073 656c 662e         _ = self.
-00005ad0: 7275 6e5f 636f 6d6d 616e 6473 2863 6f6e  run_commands(con
-00005ae0: 7665 7274 5f63 6d64 7329 0a0a 2020 2020  vert_cmds)..    
-00005af0: 6465 6620 7365 7475 705f 6a6f 625f 7363  def setup_job_sc
-00005b00: 7269 7074 7328 7365 6c66 293a 0a20 2020  ripts(self):.   
-00005b10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00005b20: 2053 6574 7320 7570 206a 6f62 2073 6372   Sets up job scr
-00005b30: 6970 7473 2066 6f72 2053 6c75 726d 206f  ipts for Slurm o
-00005b40: 7065 7261 7469 6f6e 732e 0a0a 2020 2020  perations...    
-00005b50: 2020 2020 5468 6973 2066 756e 6374 696f      This functio
-00005b60: 6e20 6569 7468 6572 2063 6c6f 6e65 7320  n either clones 
-00005b70: 6120 4769 7420 7265 706f 7369 746f 7279  a Git repository
-00005b80: 2063 6f6e 7461 696e 696e 6720 6a6f 6220   containing job 
-00005b90: 7363 7269 7074 730a 2020 2020 2020 2020  scripts.        
-00005ba0: 696e 746f 2074 6865 2073 7065 6369 6669  into the specifi
-00005bb0: 6564 2073 6372 6970 7420 7061 7468 206f  ed script path o
-00005bc0: 7220 6765 6e65 7261 7465 7320 7363 7269  r generates scri
-00005bd0: 7074 7320 6c6f 6361 6c6c 7920 6966 206e  pts locally if n
-00005be0: 6f20 7265 706f 7369 746f 7279 0a20 2020  o repository.   
-00005bf0: 2020 2020 2069 7320 7072 6f76 6964 6564       is provided
-00005c00: 2e0a 0a20 2020 2020 2020 2052 6169 7365  ...        Raise
-00005c10: 733a 0a20 2020 2020 2020 2020 2020 2053  s:.            S
-00005c20: 5348 4578 6365 7074 696f 6e3a 2049 6620  SHException: If 
-00005c30: 7468 6572 6520 6973 2061 6e20 6973 7375  there is an issu
-00005c40: 6520 6578 6563 7574 696e 6720 4769 7420  e executing Git 
-00005c50: 636f 6d6d 616e 6473 206f 7220 6765 6e65  commands or gene
-00005c60: 7261 7469 6e67 2073 6372 6970 7473 2e0a  rating scripts..
-00005c70: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00005c80: 2020 2020 6966 2073 656c 662e 736c 7572      if self.slur
-00005c90: 6d5f 7363 7269 7074 5f72 6570 6f20 616e  m_script_repo an
-00005ca0: 6420 7365 6c66 2e73 6c75 726d 5f73 6372  d self.slurm_scr
-00005cb0: 6970 745f 7061 7468 3a0a 2020 2020 2020  ipt_path:.      
-00005cc0: 2020 2020 2020 2320 6769 7420 636c 6f6e        # git clon
-00005cd0: 6520 696e 746f 2073 6372 6970 7420 7061  e into script pa
-00005ce0: 7468 0a20 2020 2020 2020 2020 2020 2065  th.            e
-00005cf0: 6e76 203d 207b 0a20 2020 2020 2020 2020  nv = {.         
-00005d00: 2020 2020 2020 2022 5245 504f 5352 4322         "REPOSRC"
-00005d10: 3a20 6622 5c22 7b73 656c 662e 736c 7572  : f"\"{self.slur
-00005d20: 6d5f 7363 7269 7074 5f72 6570 6f7d 5c22  m_script_repo}\"
-00005d30: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00005d40: 2020 2022 4c4f 4341 4c52 4550 4f22 3a20     "LOCALREPO": 
-00005d50: 6622 5c22 7b73 656c 662e 736c 7572 6d5f  f"\"{self.slurm_
-00005d60: 7363 7269 7074 5f70 6174 687d 5c22 220a  script_path}\"".
-00005d70: 2020 2020 2020 2020 2020 2020 7d0a 2020              }.  
-00005d80: 2020 2020 2020 2020 2020 2320 436c 6561            # Clea
-00005d90: 6e75 7020 7468 6520 6578 6973 7469 6e67  nup the existing
-00005da0: 2066 6f6c 6465 7220 6669 7273 740a 2020   folder first.  
-00005db0: 2020 2020 2020 2020 2020 636c 6561 6e75            cleanu
-00005dc0: 705f 6669 7273 7420 3d20 2772 6d20 2d72  p_first = 'rm -r
-00005dd0: 6620 2224 4c4f 4341 4c52 4550 4f22 270a  f "$LOCALREPO"'.
-00005de0: 2020 2020 2020 2020 2020 2020 636d 6420              cmd 
-00005df0: 3d20 2767 6974 2063 6c6f 6e65 2022 2452  = 'git clone "$R
-00005e00: 4550 4f53 5243 2220 2224 4c4f 4341 4c52  EPOSRC" "$LOCALR
-00005e10: 4550 4f22 2032 3e20 2f64 6576 2f6e 756c  EPO" 2> /dev/nul
-00005e20: 6c27 0a20 2020 2020 2020 2020 2020 2072  l'.            r
-00005e30: 203d 2073 656c 662e 7275 6e5f 636f 6d6d   = self.run_comm
-00005e40: 616e 6473 285b 636c 6561 6e75 705f 6669  ands([cleanup_fi
-00005e50: 7273 742c 2063 6d64 5d2c 2065 6e76 290a  rst, cmd], env).
-00005e60: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-00005e70: 6f74 2072 2e6f 6b3a 0a20 2020 2020 2020  ot r.ok:.       
-00005e80: 2020 2020 2020 2020 2072 6169 7365 2053           raise S
-00005e90: 5348 4578 6365 7074 696f 6e28 7229 0a20  SHException(r). 
-00005ea0: 2020 2020 2020 2065 6c69 6620 7365 6c66         elif self
-00005eb0: 2e73 6c75 726d 5f73 6372 6970 745f 7061  .slurm_script_pa
-00005ec0: 7468 3a0a 2020 2020 2020 2020 2020 2020  th:.            
-00005ed0: 2320 6765 6e65 7261 7465 2073 6372 6970  # generate scrip
-00005ee0: 7473 0a20 2020 2020 2020 2020 2020 2073  ts.            s
-00005ef0: 656c 662e 7570 6461 7465 5f73 6c75 726d  elf.update_slurm
-00005f00: 5f73 6372 6970 7473 2867 656e 6572 6174  _scripts(generat
-00005f10: 655f 6a6f 6273 3d54 7275 6529 0a0a 2020  e_jobs=True)..  
-00005f20: 2020 6465 6620 7365 7475 705f 6469 7265    def setup_dire
-00005f30: 6374 6f72 6965 7328 7365 6c66 293a 0a20  ctories(self):. 
-00005f40: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00005f50: 2020 2043 7265 6174 6573 206e 6563 6573     Creates neces
-00005f60: 7361 7279 2064 6972 6563 746f 7269 6573  sary directories
-00005f70: 2066 6f72 2053 6c75 726d 206f 7065 7261   for Slurm opera
-00005f80: 7469 6f6e 732e 0a0a 2020 2020 2020 2020  tions...        
-00005f90: 5468 6973 2066 756e 6374 696f 6e20 6372  This function cr
-00005fa0: 6561 7465 7320 6469 7265 6374 6f72 6965  eates directorie
-00005fb0: 7320 666f 7220 6461 7461 2073 746f 7261  s for data stora
-00005fc0: 6765 2c20 7363 7269 7074 732c 2061 6e64  ge, scripts, and
-00005fd0: 2077 6f72 6b66 6c6f 7773 0a20 2020 2020   workflows.     
-00005fe0: 2020 2061 7320 7370 6563 6966 6965 6420     as specified 
-00005ff0: 696e 2074 6865 2053 6c75 726d 436c 6965  in the SlurmClie
-00006000: 6e74 206f 626a 6563 742e 0a0a 2020 2020  nt object...    
-00006010: 2020 2020 5261 6973 6573 3a0a 2020 2020      Raises:.    
-00006020: 2020 2020 2020 2020 5353 4845 7863 6570          SSHExcep
-00006030: 7469 6f6e 3a20 4966 2074 6865 7265 2069  tion: If there i
-00006040: 7320 616e 2069 7373 7565 2065 7865 6375  s an issue execu
-00006050: 7469 6e67 2064 6972 6563 746f 7279 2063  ting directory c
-00006060: 7265 6174 696f 6e20 636f 6d6d 616e 6473  reation commands
-00006070: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00006080: 2020 2020 2020 6469 725f 636d 6473 203d        dir_cmds =
-00006090: 205b 5d0a 2020 2020 2020 2020 2320 612e   [].        # a.
-000060a0: 2064 6174 610a 2020 2020 2020 2020 6966   data.        if
-000060b0: 2073 656c 662e 736c 7572 6d5f 6461 7461   self.slurm_data
-000060c0: 5f70 6174 683a 0a20 2020 2020 2020 2020  _path:.         
-000060d0: 2020 2064 6972 5f63 6d64 732e 6170 7065     dir_cmds.appe
-000060e0: 6e64 2866 226d 6b64 6972 202d 7020 5c22  nd(f"mkdir -p \"
-000060f0: 7b73 656c 662e 736c 7572 6d5f 6461 7461  {self.slurm_data
-00006100: 5f70 6174 687d 5c22 2229 0a20 2020 2020  _path}\"").     
-00006110: 2020 2020 2020 2023 2062 2e20 7363 7269         # b. scri
-00006120: 7074 730a 2020 2020 2020 2020 6966 2073  pts.        if s
-00006130: 656c 662e 736c 7572 6d5f 7363 7269 7074  elf.slurm_script
-00006140: 5f70 6174 683a 0a20 2020 2020 2020 2020  _path:.         
-00006150: 2020 2064 6972 5f63 6d64 732e 6170 7065     dir_cmds.appe
-00006160: 6e64 2866 226d 6b64 6972 202d 7020 5c22  nd(f"mkdir -p \"
-00006170: 7b73 656c 662e 736c 7572 6d5f 7363 7269  {self.slurm_scri
-00006180: 7074 5f70 6174 687d 5c22 2229 0a20 2020  pt_path}\"").   
-00006190: 2020 2020 2020 2020 2023 2063 2e20 776f           # c. wo
-000061a0: 726b 666c 6f77 730a 2020 2020 2020 2020  rkflows.        
-000061b0: 6966 2073 656c 662e 736c 7572 6d5f 696d  if self.slurm_im
-000061c0: 6167 6573 5f70 6174 683a 0a20 2020 2020  ages_path:.     
-000061d0: 2020 2020 2020 2064 6972 5f63 6d64 732e         dir_cmds.
-000061e0: 6170 7065 6e64 2866 226d 6b64 6972 202d  append(f"mkdir -
-000061f0: 7020 5c22 7b73 656c 662e 736c 7572 6d5f  p \"{self.slurm_
-00006200: 696d 6167 6573 5f70 6174 687d 5c22 2229  images_path}\"")
-00006210: 0a20 2020 2020 2020 2072 203d 2073 656c  .        r = sel
-00006220: 662e 7275 6e5f 636f 6d6d 616e 6473 2864  f.run_commands(d
-00006230: 6972 5f63 6d64 7329 0a20 2020 2020 2020  ir_cmds).       
-00006240: 2069 6620 6e6f 7420 722e 6f6b 3a0a 2020   if not r.ok:.  
-00006250: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00006260: 5353 4845 7863 6570 7469 6f6e 2872 290a  SSHException(r).
-00006270: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00006280: 640a 2020 2020 6465 6620 6672 6f6d 5f63  d.    def from_c
-00006290: 6f6e 6669 6728 636c 732c 2063 6f6e 6669  onfig(cls, confi
-000062a0: 6766 696c 653a 2073 7472 203d 2027 272c  gfile: str = '',
-000062b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000062c0: 2020 2020 2069 6e69 745f 736c 7572 6d3a       init_slurm:
-000062d0: 2062 6f6f 6c20 3d20 4661 6c73 6529 202d   bool = False) -
-000062e0: 3e20 2753 6c75 726d 436c 6965 6e74 273a  > 'SlurmClient':
-000062f0: 0a20 2020 2020 2020 2022 2222 4372 6561  .        """Crea
-00006300: 7465 7320 6120 6e65 7720 536c 7572 6d43  tes a new SlurmC
-00006310: 6c69 656e 7420 6f62 6a65 6374 2075 7369  lient object usi
-00006320: 6e67 2074 6865 2070 6172 616d 6574 6572  ng the parameter
-00006330: 7320 7265 6164 2066 726f 6d20 610a 2020  s read from a.  
-00006340: 2020 2020 2020 636f 6e66 6967 7572 6174        configurat
-00006350: 696f 6e20 6669 6c65 2028 2e69 6e69 292e  ion file (.ini).
-00006360: 0a0a 2020 2020 2020 2020 4465 6661 756c  ..        Defaul
-00006370: 7473 2070 6174 6873 2074 6f20 6c6f 6f6b  ts paths to look
-00006380: 2066 6f72 2063 6f6e 6669 6720 6669 6c65   for config file
-00006390: 7320 6172 653a 0a20 2020 2020 2020 2020  s are:.         
-000063a0: 2020 202d 202f 6574 632f 736c 7572 6d2d     - /etc/slurm-
-000063b0: 636f 6e66 6967 2e69 6e69 0a20 2020 2020  config.ini.     
-000063c0: 2020 2020 2020 202d 207e 2f73 6c75 726d         - ~/slurm
-000063d0: 2d63 6f6e 6669 672e 696e 690a 0a20 2020  -config.ini..   
-000063e0: 2020 2020 204e 6f74 6520 7468 6174 2074       Note that t
-000063f0: 6869 7320 6973 206f 6e6c 7920 666f 7220  his is only for 
-00006400: 7468 6520 534c 5552 4d20 7370 6563 6966  the SLURM specif
-00006410: 6963 2076 616c 7565 7320 7468 6174 2077  ic values that w
-00006420: 6520 6164 6465 642e 0a20 2020 2020 2020  e added..       
-00006430: 204d 6f73 7420 636f 6e66 6967 7572 6174   Most configurat
-00006440: 696f 6e20 7661 6c75 6573 2061 7265 2073  ion values are s
-00006450: 6574 2076 6961 2063 6f6e 6669 6775 7261  et via configura
-00006460: 7469 6f6e 206d 6563 6861 6e69 736d 7320  tion mechanisms 
-00006470: 6672 6f6d 0a20 2020 2020 2020 2046 6162  from.        Fab
-00006480: 7269 6320 6c69 6272 6172 792c 0a20 2020  ric library,.   
-00006490: 2020 2020 206c 696b 6520 5353 4820 7365       like SSH se
-000064a0: 7474 696e 6773 2062 6569 6e67 206c 6f61  ttings being loa
-000064b0: 6465 6420 6672 6f6d 2053 5348 2063 6f6e  ded from SSH con
-000064c0: 6669 672c 202f 6574 632f 6661 6272 6963  fig, /etc/fabric
-000064d0: 2e79 6d6c 206f 720a 2020 2020 2020 2020  .yml or.        
-000064e0: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
-000064f0: 6162 6c65 732e 0a20 2020 2020 2020 2053  ables..        S
-00006500: 6565 2046 6162 7269 6327 7320 646f 6375  ee Fabric's docu
-00006510: 6d65 6e74 6174 696f 6e20 666f 7220 6d6f  mentation for mo
-00006520: 7265 2069 6e66 6f20 6f6e 2063 6f6e 6669  re info on confi
-00006530: 6775 7261 7469 6f6e 2069 6620 6e65 6564  guration if need
-00006540: 6564 2e0a 0a20 2020 2020 2020 2041 7267  ed...        Arg
-00006550: 733a 0a20 2020 2020 2020 2020 2020 2063  s:.            c
-00006560: 6f6e 6669 6766 696c 6520 2873 7472 293a  onfigfile (str):
-00006570: 2054 6865 2070 6174 6820 746f 2079 6f75   The path to you
-00006580: 7220 636f 6e66 6967 7572 6174 696f 6e20  r configuration 
-00006590: 6669 6c65 2e20 4f70 7469 6f6e 616c 2e0a  file. Optional..
-000065a0: 2020 2020 2020 2020 2020 2020 696e 6974              init
-000065b0: 5f73 6c75 726d 2028 626f 6f6c 293a 2049  _slurm (bool): I
-000065c0: 6e69 7469 6174 6520 2f20 7661 6c69 6461  nitiate / valida
-000065d0: 7465 2073 6c75 726d 2073 6574 7570 2e20  te slurm setup. 
-000065e0: 4f70 7469 6f6e 616c 0a20 2020 2020 2020  Optional.       
-000065f0: 2020 2020 2020 2020 204d 6967 6874 2074           Might t
-00006600: 616b 6520 736f 6d65 2074 696d 6520 7468  ake some time th
-00006610: 6520 6669 7273 7420 7469 6d65 2077 6974  e first time wit
-00006620: 6820 646f 776e 6c6f 6164 696e 6720 6574  h downloading et
-00006630: 632e 0a0a 2020 2020 2020 2020 5265 7475  c...        Retu
-00006640: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00006650: 2053 6c75 726d 436c 6965 6e74 3a20 4120   SlurmClient: A 
-00006660: 6e65 7720 536c 7572 6d43 6c69 656e 7420  new SlurmClient 
-00006670: 6f62 6a65 6374 2e0a 2020 2020 2020 2020  object..        
-00006680: 2222 220a 2020 2020 2020 2020 2320 4c6f  """.        # Lo
-00006690: 6164 2074 6865 2063 6f6e 6669 6775 7261  ad the configura
-000066a0: 7469 6f6e 2066 696c 650a 2020 2020 2020  tion file.      
-000066b0: 2020 636f 6e66 6967 7320 3d20 636f 6e66    configs = conf
-000066c0: 6967 7061 7273 6572 2e43 6f6e 6669 6750  igparser.ConfigP
-000066d0: 6172 7365 7228 616c 6c6f 775f 6e6f 5f76  arser(allow_no_v
-000066e0: 616c 7565 3d54 7275 6529 0a20 2020 2020  alue=True).     
-000066f0: 2020 2023 204c 6f61 6473 2066 726f 6d20     # Loads from 
-00006700: 6465 6661 756c 7420 6c6f 6361 7469 6f6e  default location
-00006710: 7320 616e 6420 6769 7665 6e20 6c6f 6361  s and given loca
-00006720: 7469 6f6e 2c20 6d69 7373 696e 6720 6669  tion, missing fi
-00006730: 6c65 7320 6172 6520 6f6b 0a20 2020 2020  les are ok.     
-00006740: 2020 2063 6f6e 6669 6773 2e72 6561 6428     configs.read(
-00006750: 5b63 6c73 2e5f 4445 4641 554c 545f 434f  [cls._DEFAULT_CO
-00006760: 4e46 4947 5f50 4154 485f 312c 0a20 2020  NFIG_PATH_1,.   
-00006770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006780: 2020 636c 732e 5f44 4546 4155 4c54 5f43    cls._DEFAULT_C
-00006790: 4f4e 4649 475f 5041 5448 5f32 2c0a 2020  ONFIG_PATH_2,.  
-000067a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000067b0: 2020 2063 6f6e 6669 6766 696c 655d 290a     configfile]).
-000067c0: 2020 2020 2020 2020 2320 5265 6164 2074          # Read t
-000067d0: 6865 2072 6571 7569 7265 6420 7061 7261  he required para
-000067e0: 6d65 7465 7273 2066 726f 6d20 7468 6520  meters from the 
-000067f0: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
-00006800: 6c65 2c0a 2020 2020 2020 2020 2320 6661  le,.        # fa
-00006810: 6c6c 6261 636b 2074 6f20 6465 6661 756c  llback to defaul
-00006820: 7473 0a20 2020 2020 2020 2068 6f73 7420  ts.        host 
-00006830: 3d20 636f 6e66 6967 732e 6765 7428 2253  = configs.get("S
-00006840: 5348 222c 2022 686f 7374 222c 2066 616c  SH", "host", fal
-00006850: 6c62 6163 6b3d 636c 732e 5f44 4546 4155  lback=cls._DEFAU
-00006860: 4c54 5f48 4f53 5429 0a20 2020 2020 2020  LT_HOST).       
-00006870: 2069 6e6c 696e 655f 7373 685f 656e 7620   inline_ssh_env 
-00006880: 3d20 636f 6e66 6967 732e 6765 7462 6f6f  = configs.getboo
-00006890: 6c65 616e 280a 2020 2020 2020 2020 2020  lean(.          
-000068a0: 2020 2253 5348 222c 2022 696e 6c69 6e65    "SSH", "inline
-000068b0: 5f73 7368 5f65 6e76 222c 2066 616c 6c62  _ssh_env", fallb
-000068c0: 6163 6b3d 636c 732e 5f44 4546 4155 4c54  ack=cls._DEFAULT
-000068d0: 5f49 4e4c 494e 455f 5353 485f 454e 5629  _INLINE_SSH_ENV)
-000068e0: 0a20 2020 2020 2020 2073 6c75 726d 5f64  .        slurm_d
-000068f0: 6174 615f 7061 7468 203d 2063 6f6e 6669  ata_path = confi
-00006900: 6773 2e67 6574 280a 2020 2020 2020 2020  gs.get(.        
-00006910: 2020 2020 2253 4c55 524d 222c 2022 736c      "SLURM", "sl
-00006920: 7572 6d5f 6461 7461 5f70 6174 6822 2c20  urm_data_path", 
-00006930: 6661 6c6c 6261 636b 3d63 6c73 2e5f 4445  fallback=cls._DE
-00006940: 4641 554c 545f 534c 5552 4d5f 4441 5441  FAULT_SLURM_DATA
-00006950: 5f50 4154 4829 0a20 2020 2020 2020 2073  _PATH).        s
-00006960: 6c75 726d 5f69 6d61 6765 735f 7061 7468  lurm_images_path
-00006970: 203d 2063 6f6e 6669 6773 2e67 6574 280a   = configs.get(.
-00006980: 2020 2020 2020 2020 2020 2020 2253 4c55              "SLU
-00006990: 524d 222c 2022 736c 7572 6d5f 696d 6167  RM", "slurm_imag
-000069a0: 6573 5f70 6174 6822 2c0a 2020 2020 2020  es_path",.      
-000069b0: 2020 2020 2020 6661 6c6c 6261 636b 3d63        fallback=c
-000069c0: 6c73 2e5f 4445 4641 554c 545f 534c 5552  ls._DEFAULT_SLUR
-000069d0: 4d5f 494d 4147 4553 5f50 4154 4829 0a20  M_IMAGES_PATH). 
-000069e0: 2020 2020 2020 2073 6c75 726d 5f63 6f6e         slurm_con
-000069f0: 7665 7274 6572 735f 7061 7468 203d 2063  verters_path = c
-00006a00: 6f6e 6669 6773 2e67 6574 280a 2020 2020  onfigs.get(.    
-00006a10: 2020 2020 2020 2020 2253 4c55 524d 222c          "SLURM",
-00006a20: 2022 736c 7572 6d5f 636f 6e76 6572 7465   "slurm_converte
-00006a30: 7273 5f70 6174 6822 2c0a 2020 2020 2020  rs_path",.      
-00006a40: 2020 2020 2020 6661 6c6c 6261 636b 3d63        fallback=c
-00006a50: 6c73 2e5f 4445 4641 554c 545f 534c 5552  ls._DEFAULT_SLUR
-00006a60: 4d5f 434f 4e56 4552 5445 5253 5f50 4154  M_CONVERTERS_PAT
-00006a70: 4829 0a0a 2020 2020 2020 2020 2320 5370  H)..        # Sp
-00006a80: 6c69 7420 7468 6520 4d4f 4445 4c53 2069  lit the MODELS i
-00006a90: 6e74 6f20 7061 7468 732c 2072 6570 6f73  nto paths, repos
-00006aa0: 2061 6e64 2069 6d61 6765 730a 2020 2020   and images.    
-00006ab0: 2020 2020 6d6f 6465 6c73 5f64 6963 7420      models_dict 
-00006ac0: 3d20 6469 6374 2863 6f6e 6669 6773 2e69  = dict(configs.i
-00006ad0: 7465 6d73 2822 4d4f 4445 4c53 2229 290a  tems("MODELS")).
-00006ae0: 2020 2020 2020 2020 736c 7572 6d5f 6d6f          slurm_mo
-00006af0: 6465 6c5f 7061 7468 7320 3d20 7b7d 0a20  del_paths = {}. 
-00006b00: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
-00006b10: 656c 5f72 6570 6f73 203d 207b 7d0a 2020  el_repos = {}.  
-00006b20: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
-00006b30: 6c5f 6a6f 6273 203d 207b 7d0a 2020 2020  l_jobs = {}.    
-00006b40: 2020 2020 736c 7572 6d5f 6d6f 6465 6c5f      slurm_model_
-00006b50: 6a6f 6273 5f70 6172 616d 7320 3d20 7b7d  jobs_params = {}
-00006b60: 0a20 2020 2020 2020 2066 6f72 206b 2c20  .        for k, 
-00006b70: 7620 696e 206d 6f64 656c 735f 6469 6374  v in models_dict
-00006b80: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-00006b90: 2020 2020 2020 7375 6666 6978 5f72 6570        suffix_rep
-00006ba0: 6f20 3d20 275f 7265 706f 270a 2020 2020  o = '_repo'.    
-00006bb0: 2020 2020 2020 2020 7375 6666 6978 5f6a          suffix_j
-00006bc0: 6f62 203d 2027 5f6a 6f62 270a 2020 2020  ob = '_job'.    
-00006bd0: 2020 2020 2020 2020 6a6f 625f 7061 7261          job_para
-00006be0: 6d5f 7061 7474 6572 6e20 3d20 2228 2e2b  m_pattern = "(.+
-00006bf0: 295f 6a6f 625f 282e 2b29 220a 2020 2020  )_job_(.+)".    
-00006c00: 2020 2020 2020 2020 6a6f 625f 7061 7261          job_para
-00006c10: 6d5f 6d61 7463 6820 3d20 7265 2e6d 6174  m_match = re.mat
-00006c20: 6368 286a 6f62 5f70 6172 616d 5f70 6174  ch(job_param_pat
-00006c30: 7465 726e 2c20 6b29 0a20 2020 2020 2020  tern, k).       
-00006c40: 2020 2020 2069 6620 6b2e 656e 6473 7769       if k.endswi
-00006c50: 7468 2873 7566 6669 785f 7265 706f 293a  th(suffix_repo):
-00006c60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006c70: 2073 6c75 726d 5f6d 6f64 656c 5f72 6570   slurm_model_rep
-00006c80: 6f73 5b6b 5b3a 2d6c 656e 2873 7566 6669  os[k[:-len(suffi
-00006c90: 785f 7265 706f 295d 5d20 3d20 760a 2020  x_repo)]] = v.  
-00006ca0: 2020 2020 2020 2020 2020 656c 6966 206b            elif k
-00006cb0: 2e65 6e64 7377 6974 6828 7375 6666 6978  .endswith(suffix
-00006cc0: 5f6a 6f62 293a 0a20 2020 2020 2020 2020  _job):.         
-00006cd0: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
-00006ce0: 656c 5f6a 6f62 735b 6b5b 3a2d 6c65 6e28  el_jobs[k[:-len(
-00006cf0: 7375 6666 6978 5f6a 6f62 295d 5d20 3d20  suffix_job)]] = 
-00006d00: 760a 2020 2020 2020 2020 2020 2020 2020  v.              
-00006d10: 2020 736c 7572 6d5f 6d6f 6465 6c5f 6a6f    slurm_model_jo
-00006d20: 6273 5f70 6172 616d 735b 6b5b 3a2d 6c65  bs_params[k[:-le
-00006d30: 6e28 7375 6666 6978 5f6a 6f62 295d 5d20  n(suffix_job)]] 
-00006d40: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
-00006d50: 2065 6c69 6620 6a6f 625f 7061 7261 6d5f   elif job_param_
-00006d60: 6d61 7463 683a 0a20 2020 2020 2020 2020  match:.         
-00006d70: 2020 2020 2020 2070 7269 6e74 2866 224d         print(f"M
-00006d80: 6174 6368 3a20 7b73 6c75 726d 5f6d 6f64  atch: {slurm_mod
-00006d90: 656c 5f6a 6f62 735f 7061 7261 6d73 7d22  el_jobs_params}"
-00006da0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00006db0: 2020 736c 7572 6d5f 6d6f 6465 6c5f 6a6f    slurm_model_jo
-00006dc0: 6273 5f70 6172 616d 735b 6a6f 625f 7061  bs_params[job_pa
-00006dd0: 7261 6d5f 6d61 7463 682e 6772 6f75 7028  ram_match.group(
-00006de0: 3129 5d2e 6170 7065 6e64 280a 2020 2020  1)].append(.    
+00005570: 2020 2020 7265 6d6f 7465 3d73 656c 662e      remote=self.
+00005580: 736c 7572 6d5f 7363 7269 7074 5f70 6174  slurm_script_pat
+00005590: 6829 0a20 2020 2020 2020 2023 2063 7572  h).        # cur
+000055a0: 7265 6e74 6c79 206b 6e6f 776e 2063 6f6e  rently known con
+000055b0: 7665 7274 6572 730a 2020 2020 2020 2020  verters.        
+000055c0: 2320 3361 2e20 5a41 5252 2074 6f20 5449  # 3a. ZARR to TI
+000055d0: 4646 0a20 2020 2020 2020 2023 2054 4f44  FF.        # TOD
+000055e0: 4f20 6578 7472 6163 7420 7468 6573 6520  O extract these 
+000055f0: 7661 6c75 6573 2074 6f20 652e 672e 2063  values to e.g. c
+00005600: 6f6e 6669 6720 6966 2077 6520 6861 7665  onfig if we have
+00005610: 206d 6f72 650a 2020 2020 2020 2020 636f   more.        co
+00005620: 6e76 6572 745f 6e61 6d65 203d 2022 636f  nvert_name = "co
+00005630: 6e76 6572 745f 7a61 7272 5f74 6f5f 7469  nvert_zarr_to_ti
+00005640: 6666 220a 2020 2020 2020 2020 636f 6e76  ff".        conv
+00005650: 6572 745f 7079 203d 2066 227b 636f 6e76  ert_py = f"{conv
+00005660: 6572 745f 6e61 6d65 7d2e 7079 220a 2020  ert_name}.py".  
+00005670: 2020 2020 2020 636f 6e76 6572 745f 7363        convert_sc
+00005680: 7269 7074 5f6c 6f63 616c 203d 2066 696c  ript_local = fil
+00005690: 6573 2822 7265 736f 7572 6365 7322 292e  es("resources").
+000056a0: 6a6f 696e 7061 7468 280a 2020 2020 2020  joinpath(.      
+000056b0: 2020 2020 2020 636f 6e76 6572 745f 7079        convert_py
+000056c0: 290a 2020 2020 2020 2020 636f 6e76 6572  ).        conver
+000056d0: 745f 6465 6620 3d20 6622 7b63 6f6e 7665  t_def = f"{conve
+000056e0: 7274 5f6e 616d 657d 2e64 6566 220a 2020  rt_name}.def".  
+000056f0: 2020 2020 2020 636f 6e76 6572 745f 6465        convert_de
+00005700: 665f 6c6f 6361 6c20 3d20 6669 6c65 7328  f_local = files(
+00005710: 2272 6573 6f75 7263 6573 2229 2e6a 6f69  "resources").joi
+00005720: 6e70 6174 6828 0a20 2020 2020 2020 2020  npath(.         
+00005730: 2020 2063 6f6e 7665 7274 5f64 6566 290a     convert_def).
+00005740: 2020 2020 2020 2020 5f20 3d20 7365 6c66          _ = self
+00005750: 2e70 7574 286c 6f63 616c 3d63 6f6e 7665  .put(local=conve
+00005760: 7274 5f73 6372 6970 745f 6c6f 6361 6c2c  rt_script_local,
+00005770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005780: 2020 2020 2020 7265 6d6f 7465 3d73 656c        remote=sel
+00005790: 662e 736c 7572 6d5f 636f 6e76 6572 7465  f.slurm_converte
+000057a0: 7273 5f70 6174 6829 0a20 2020 2020 2020  rs_path).       
+000057b0: 205f 203d 2073 656c 662e 7075 7428 6c6f   _ = self.put(lo
+000057c0: 6361 6c3d 636f 6e76 6572 745f 6465 665f  cal=convert_def_
+000057d0: 6c6f 6361 6c2c 0a20 2020 2020 2020 2020  local,.         
+000057e0: 2020 2020 2020 2020 2020 2020 7265 6d6f              remo
+000057f0: 7465 3d73 656c 662e 736c 7572 6d5f 636f  te=self.slurm_co
+00005800: 6e76 6572 7465 7273 5f70 6174 6829 0a20  nverters_path). 
+00005810: 2020 2020 2020 2023 2042 7569 6c64 2073         # Build s
+00005820: 696e 6775 6c61 7269 7479 2063 6f6e 7461  ingularity conta
+00005830: 696e 6572 2066 726f 6d20 6465 6669 6e69  iner from defini
+00005840: 7469 6f6e 0a20 2020 2020 2020 2077 6974  tion.        wit
+00005850: 6820 7365 6c66 2e63 6428 7365 6c66 2e73  h self.cd(self.s
+00005860: 6c75 726d 5f63 6f6e 7665 7274 6572 735f  lurm_converters_
+00005870: 7061 7468 293a 0a20 2020 2020 2020 2020  path):.         
+00005880: 2020 2063 6f6e 7665 7274 5f63 6d64 7320     convert_cmds 
+00005890: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
+000058a0: 2069 6620 7365 6c66 2e73 6c75 726d 5f69   if self.slurm_i
+000058b0: 6d61 6765 735f 7061 7468 3a0a 2020 2020  mages_path:.    
+000058c0: 2020 2020 2020 2020 2020 2020 2320 544f              # TO
+000058d0: 444f 2043 6861 6e67 6520 7468 6520 746d  DO Change the tm
+000058e0: 7020 6469 723f 0a20 2020 2020 2020 2020  p dir?.         
+000058f0: 2020 2020 2020 2023 2065 7870 6f72 7420         # export 
+00005900: 5349 4e47 554c 4152 4954 595f 544d 5044  SINGULARITY_TMPD
+00005910: 4952 3d7e 2f6d 792d 7363 7261 7463 682f  IR=~/my-scratch/
+00005920: 746d 703b 0a20 2020 2020 2020 2020 2020  tmp;.           
+00005930: 2020 2020 2023 206f 6e6c 7920 6966 2066       # only if f
+00005940: 696c 6520 646f 6573 206e 6f74 2065 7869  ile does not exi
+00005950: 7374 2079 6574 0a20 2020 2020 2020 2020  st yet.         
+00005960: 2020 2020 2020 2023 2063 6f6e 7665 7274         # convert
+00005970: 5f63 6d64 732e 6170 7065 6e64 2866 225b  _cmds.append(f"[
+00005980: 2021 202d 6620 7b63 6f6e 7665 7274 5f6e   ! -f {convert_n
+00005990: 616d 657d 2e73 6966 205d 2229 0a20 2020  ame}.sif ]").   
+000059a0: 2020 2020 2020 2020 2020 2020 2023 2045               # E
+000059b0: 4449 5420 2d2d 204e 4f2c 2074 6865 6e20  DIT -- NO, then 
+000059c0: 7765 2063 616e 2774 2075 7064 6174 6521  we can't update!
+000059d0: 2046 6f72 6365 2072 6562 7569 6c64 210a   Force rebuild!.
+000059e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000059f0: 2320 646f 776e 6c6f 6164 202f 6275 696c  # download /buil
+00005a00: 6420 6e65 7720 636f 6e74 6169 6e65 720a  d new container.
+00005a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a20: 636f 6e76 6572 745f 636d 6473 2e61 7070  convert_cmds.app
+00005a30: 656e 6428 0a20 2020 2020 2020 2020 2020  end(.           
+00005a40: 2020 2020 2020 2020 2066 2273 696e 6775           f"singu
+00005a50: 6c61 7269 7479 2062 7569 6c64 202d 4620  larity build -F 
+00005a60: 5c22 7b63 6f6e 7665 7274 5f6e 616d 657d  \"{convert_name}
+00005a70: 2e73 6966 5c22 207b 636f 6e76 6572 745f  .sif\" {convert_
+00005a80: 6465 667d 203e 3e20 7369 6e67 2e6c 6f67  def} >> sing.log
+00005a90: 2032 3e26 3120 3b20 6563 686f 2027 6669   2>&1 ; echo 'fi
+00005aa0: 6e69 7368 6564 207b 636f 6e76 6572 745f  nished {convert_
+00005ab0: 6e61 6d65 7d2e 7369 6627 2026 2229 0a20  name}.sif' &"). 
+00005ac0: 2020 2020 2020 2020 2020 205f 203d 2073             _ = s
+00005ad0: 656c 662e 7275 6e5f 636f 6d6d 616e 6473  elf.run_commands
+00005ae0: 2863 6f6e 7665 7274 5f63 6d64 7329 0a0a  (convert_cmds)..
+00005af0: 2020 2020 6465 6620 7365 7475 705f 6a6f      def setup_jo
+00005b00: 625f 7363 7269 7074 7328 7365 6c66 293a  b_scripts(self):
+00005b10: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00005b20: 2020 2020 2053 6574 7320 7570 206a 6f62       Sets up job
+00005b30: 2073 6372 6970 7473 2066 6f72 2053 6c75   scripts for Slu
+00005b40: 726d 206f 7065 7261 7469 6f6e 732e 0a0a  rm operations...
+00005b50: 2020 2020 2020 2020 5468 6973 2066 756e          This fun
+00005b60: 6374 696f 6e20 6569 7468 6572 2063 6c6f  ction either clo
+00005b70: 6e65 7320 6120 4769 7420 7265 706f 7369  nes a Git reposi
+00005b80: 746f 7279 2063 6f6e 7461 696e 696e 6720  tory containing 
+00005b90: 6a6f 6220 7363 7269 7074 730a 2020 2020  job scripts.    
+00005ba0: 2020 2020 696e 746f 2074 6865 2073 7065      into the spe
+00005bb0: 6369 6669 6564 2073 6372 6970 7420 7061  cified script pa
+00005bc0: 7468 206f 7220 6765 6e65 7261 7465 7320  th or generates 
+00005bd0: 7363 7269 7074 7320 6c6f 6361 6c6c 7920  scripts locally 
+00005be0: 6966 206e 6f20 7265 706f 7369 746f 7279  if no repository
+00005bf0: 0a20 2020 2020 2020 2069 7320 7072 6f76  .        is prov
+00005c00: 6964 6564 2e0a 0a20 2020 2020 2020 2052  ided...        R
+00005c10: 6169 7365 733a 0a20 2020 2020 2020 2020  aises:.         
+00005c20: 2020 2053 5348 4578 6365 7074 696f 6e3a     SSHException:
+00005c30: 2049 6620 7468 6572 6520 6973 2061 6e20   If there is an 
+00005c40: 6973 7375 6520 6578 6563 7574 696e 6720  issue executing 
+00005c50: 4769 7420 636f 6d6d 616e 6473 206f 7220  Git commands or 
+00005c60: 6765 6e65 7261 7469 6e67 2073 6372 6970  generating scrip
+00005c70: 7473 2e0a 2020 2020 2020 2020 2222 220a  ts..        """.
+00005c80: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+00005c90: 736c 7572 6d5f 7363 7269 7074 5f72 6570  slurm_script_rep
+00005ca0: 6f20 616e 6420 7365 6c66 2e73 6c75 726d  o and self.slurm
+00005cb0: 5f73 6372 6970 745f 7061 7468 3a0a 2020  _script_path:.  
+00005cc0: 2020 2020 2020 2020 2020 2320 6769 7420            # git 
+00005cd0: 636c 6f6e 6520 696e 746f 2073 6372 6970  clone into scrip
+00005ce0: 7420 7061 7468 0a20 2020 2020 2020 2020  t path.         
+00005cf0: 2020 2065 6e76 203d 207b 0a20 2020 2020     env = {.     
+00005d00: 2020 2020 2020 2020 2020 2022 5245 504f             "REPO
+00005d10: 5352 4322 3a20 6622 5c22 7b73 656c 662e  SRC": f"\"{self.
+00005d20: 736c 7572 6d5f 7363 7269 7074 5f72 6570  slurm_script_rep
+00005d30: 6f7d 5c22 222c 0a20 2020 2020 2020 2020  o}\"",.         
+00005d40: 2020 2020 2020 2022 4c4f 4341 4c52 4550         "LOCALREP
+00005d50: 4f22 3a20 6622 5c22 7b73 656c 662e 736c  O": f"\"{self.sl
+00005d60: 7572 6d5f 7363 7269 7074 5f70 6174 687d  urm_script_path}
+00005d70: 5c22 220a 2020 2020 2020 2020 2020 2020  \"".            
+00005d80: 7d0a 2020 2020 2020 2020 2020 2020 2320  }.            # 
+00005d90: 436c 6561 6e75 7020 7468 6520 6578 6973  Cleanup the exis
+00005da0: 7469 6e67 2066 6f6c 6465 7220 6669 7273  ting folder firs
+00005db0: 740a 2020 2020 2020 2020 2020 2020 636c  t.            cl
+00005dc0: 6561 6e75 705f 6669 7273 7420 3d20 2772  eanup_first = 'r
+00005dd0: 6d20 2d72 6620 2224 4c4f 4341 4c52 4550  m -rf "$LOCALREP
+00005de0: 4f22 270a 2020 2020 2020 2020 2020 2020  O"'.            
+00005df0: 636d 6420 3d20 2767 6974 2063 6c6f 6e65  cmd = 'git clone
+00005e00: 2022 2452 4550 4f53 5243 2220 2224 4c4f   "$REPOSRC" "$LO
+00005e10: 4341 4c52 4550 4f22 2032 3e20 2f64 6576  CALREPO" 2> /dev
+00005e20: 2f6e 756c 6c27 0a20 2020 2020 2020 2020  /null'.         
+00005e30: 2020 2072 203d 2073 656c 662e 7275 6e5f     r = self.run_
+00005e40: 636f 6d6d 616e 6473 285b 636c 6561 6e75  commands([cleanu
+00005e50: 705f 6669 7273 742c 2063 6d64 5d2c 2065  p_first, cmd], e
+00005e60: 6e76 290a 2020 2020 2020 2020 2020 2020  nv).            
+00005e70: 6966 206e 6f74 2072 2e6f 6b3a 0a20 2020  if not r.ok:.   
+00005e80: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00005e90: 7365 2053 5348 4578 6365 7074 696f 6e28  se SSHException(
+00005ea0: 7229 0a20 2020 2020 2020 2065 6c69 6620  r).        elif 
+00005eb0: 7365 6c66 2e73 6c75 726d 5f73 6372 6970  self.slurm_scrip
+00005ec0: 745f 7061 7468 3a0a 2020 2020 2020 2020  t_path:.        
+00005ed0: 2020 2020 2320 6765 6e65 7261 7465 2073      # generate s
+00005ee0: 6372 6970 7473 0a20 2020 2020 2020 2020  cripts.         
+00005ef0: 2020 2073 656c 662e 7570 6461 7465 5f73     self.update_s
+00005f00: 6c75 726d 5f73 6372 6970 7473 2867 656e  lurm_scripts(gen
+00005f10: 6572 6174 655f 6a6f 6273 3d54 7275 6529  erate_jobs=True)
+00005f20: 0a0a 2020 2020 6465 6620 7365 7475 705f  ..    def setup_
+00005f30: 6469 7265 6374 6f72 6965 7328 7365 6c66  directories(self
+00005f40: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00005f50: 2020 2020 2020 2043 7265 6174 6573 206e         Creates n
+00005f60: 6563 6573 7361 7279 2064 6972 6563 746f  ecessary directo
+00005f70: 7269 6573 2066 6f72 2053 6c75 726d 206f  ries for Slurm o
+00005f80: 7065 7261 7469 6f6e 732e 0a0a 2020 2020  perations...    
+00005f90: 2020 2020 5468 6973 2066 756e 6374 696f      This functio
+00005fa0: 6e20 6372 6561 7465 7320 6469 7265 6374  n creates direct
+00005fb0: 6f72 6965 7320 666f 7220 6461 7461 2073  ories for data s
+00005fc0: 746f 7261 6765 2c20 7363 7269 7074 732c  torage, scripts,
+00005fd0: 2061 6e64 2077 6f72 6b66 6c6f 7773 0a20   and workflows. 
+00005fe0: 2020 2020 2020 2061 7320 7370 6563 6966         as specif
+00005ff0: 6965 6420 696e 2074 6865 2053 6c75 726d  ied in the Slurm
+00006000: 436c 6965 6e74 206f 626a 6563 742e 0a0a  Client object...
+00006010: 2020 2020 2020 2020 5261 6973 6573 3a0a          Raises:.
+00006020: 2020 2020 2020 2020 2020 2020 5353 4845              SSHE
+00006030: 7863 6570 7469 6f6e 3a20 4966 2074 6865  xception: If the
+00006040: 7265 2069 7320 616e 2069 7373 7565 2065  re is an issue e
+00006050: 7865 6375 7469 6e67 2064 6972 6563 746f  xecuting directo
+00006060: 7279 2063 7265 6174 696f 6e20 636f 6d6d  ry creation comm
+00006070: 616e 6473 2e0a 2020 2020 2020 2020 2222  ands..        ""
+00006080: 220a 2020 2020 2020 2020 6469 725f 636d  ".        dir_cm
+00006090: 6473 203d 205b 5d0a 2020 2020 2020 2020  ds = [].        
+000060a0: 2320 612e 2064 6174 610a 2020 2020 2020  # a. data.      
+000060b0: 2020 6966 2073 656c 662e 736c 7572 6d5f    if self.slurm_
+000060c0: 6461 7461 5f70 6174 683a 0a20 2020 2020  data_path:.     
+000060d0: 2020 2020 2020 2064 6972 5f63 6d64 732e         dir_cmds.
+000060e0: 6170 7065 6e64 2866 226d 6b64 6972 202d  append(f"mkdir -
+000060f0: 7020 5c22 7b73 656c 662e 736c 7572 6d5f  p \"{self.slurm_
+00006100: 6461 7461 5f70 6174 687d 5c22 2229 0a20  data_path}\""). 
+00006110: 2020 2020 2020 2020 2020 2023 2062 2e20             # b. 
+00006120: 7363 7269 7074 730a 2020 2020 2020 2020  scripts.        
+00006130: 6966 2073 656c 662e 736c 7572 6d5f 7363  if self.slurm_sc
+00006140: 7269 7074 5f70 6174 683a 0a20 2020 2020  ript_path:.     
+00006150: 2020 2020 2020 2064 6972 5f63 6d64 732e         dir_cmds.
+00006160: 6170 7065 6e64 2866 226d 6b64 6972 202d  append(f"mkdir -
+00006170: 7020 5c22 7b73 656c 662e 736c 7572 6d5f  p \"{self.slurm_
+00006180: 7363 7269 7074 5f70 6174 687d 5c22 2229  script_path}\"")
+00006190: 0a20 2020 2020 2020 2020 2020 2023 2063  .            # c
+000061a0: 2e20 776f 726b 666c 6f77 730a 2020 2020  . workflows.    
+000061b0: 2020 2020 6966 2073 656c 662e 736c 7572      if self.slur
+000061c0: 6d5f 696d 6167 6573 5f70 6174 683a 0a20  m_images_path:. 
+000061d0: 2020 2020 2020 2020 2020 2064 6972 5f63             dir_c
+000061e0: 6d64 732e 6170 7065 6e64 2866 226d 6b64  mds.append(f"mkd
+000061f0: 6972 202d 7020 5c22 7b73 656c 662e 736c  ir -p \"{self.sl
+00006200: 7572 6d5f 696d 6167 6573 5f70 6174 687d  urm_images_path}
+00006210: 5c22 2229 0a20 2020 2020 2020 2072 203d  \"").        r =
+00006220: 2073 656c 662e 7275 6e5f 636f 6d6d 616e   self.run_comman
+00006230: 6473 2864 6972 5f63 6d64 7329 0a20 2020  ds(dir_cmds).   
+00006240: 2020 2020 2069 6620 6e6f 7420 722e 6f6b       if not r.ok
+00006250: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+00006260: 6973 6520 5353 4845 7863 6570 7469 6f6e  ise SSHException
+00006270: 2872 290a 0a20 2020 2040 636c 6173 736d  (r)..    @classm
+00006280: 6574 686f 640a 2020 2020 6465 6620 6672  ethod.    def fr
+00006290: 6f6d 5f63 6f6e 6669 6728 636c 732c 2063  om_config(cls, c
+000062a0: 6f6e 6669 6766 696c 653a 2073 7472 203d  onfigfile: str =
+000062b0: 2027 272c 0a20 2020 2020 2020 2020 2020   '',.           
+000062c0: 2020 2020 2020 2020 2069 6e69 745f 736c           init_sl
+000062d0: 7572 6d3a 2062 6f6f 6c20 3d20 4661 6c73  urm: bool = Fals
+000062e0: 6529 202d 3e20 2753 6c75 726d 436c 6965  e) -> 'SlurmClie
+000062f0: 6e74 273a 0a20 2020 2020 2020 2022 2222  nt':.        """
+00006300: 4372 6561 7465 7320 6120 6e65 7720 536c  Creates a new Sl
+00006310: 7572 6d43 6c69 656e 7420 6f62 6a65 6374  urmClient object
+00006320: 2075 7369 6e67 2074 6865 2070 6172 616d   using the param
+00006330: 6574 6572 7320 7265 6164 2066 726f 6d20  eters read from 
+00006340: 610a 2020 2020 2020 2020 636f 6e66 6967  a.        config
+00006350: 7572 6174 696f 6e20 6669 6c65 2028 2e69  uration file (.i
+00006360: 6e69 292e 0a0a 2020 2020 2020 2020 4465  ni)...        De
+00006370: 6661 756c 7473 2070 6174 6873 2074 6f20  faults paths to 
+00006380: 6c6f 6f6b 2066 6f72 2063 6f6e 6669 6720  look for config 
+00006390: 6669 6c65 7320 6172 653a 0a20 2020 2020  files are:.     
+000063a0: 2020 2020 2020 202d 202f 6574 632f 736c         - /etc/sl
+000063b0: 7572 6d2d 636f 6e66 6967 2e69 6e69 0a20  urm-config.ini. 
+000063c0: 2020 2020 2020 2020 2020 202d 207e 2f73             - ~/s
+000063d0: 6c75 726d 2d63 6f6e 6669 672e 696e 690a  lurm-config.ini.
+000063e0: 0a20 2020 2020 2020 204e 6f74 6520 7468  .        Note th
+000063f0: 6174 2074 6869 7320 6973 206f 6e6c 7920  at this is only 
+00006400: 666f 7220 7468 6520 534c 5552 4d20 7370  for the SLURM sp
+00006410: 6563 6966 6963 2076 616c 7565 7320 7468  ecific values th
+00006420: 6174 2077 6520 6164 6465 642e 0a20 2020  at we added..   
+00006430: 2020 2020 204d 6f73 7420 636f 6e66 6967       Most config
+00006440: 7572 6174 696f 6e20 7661 6c75 6573 2061  uration values a
+00006450: 7265 2073 6574 2076 6961 2063 6f6e 6669  re set via confi
+00006460: 6775 7261 7469 6f6e 206d 6563 6861 6e69  guration mechani
+00006470: 736d 7320 6672 6f6d 0a20 2020 2020 2020  sms from.       
+00006480: 2046 6162 7269 6320 6c69 6272 6172 792c   Fabric library,
+00006490: 0a20 2020 2020 2020 206c 696b 6520 5353  .        like SS
+000064a0: 4820 7365 7474 696e 6773 2062 6569 6e67  H settings being
+000064b0: 206c 6f61 6465 6420 6672 6f6d 2053 5348   loaded from SSH
+000064c0: 2063 6f6e 6669 672c 202f 6574 632f 6661   config, /etc/fa
+000064d0: 6272 6963 2e79 6d6c 206f 720a 2020 2020  bric.yml or.    
+000064e0: 2020 2020 656e 7669 726f 6e6d 656e 7420      environment 
+000064f0: 7661 7269 6162 6c65 732e 0a20 2020 2020  variables..     
+00006500: 2020 2053 6565 2046 6162 7269 6327 7320     See Fabric's 
+00006510: 646f 6375 6d65 6e74 6174 696f 6e20 666f  documentation fo
+00006520: 7220 6d6f 7265 2069 6e66 6f20 6f6e 2063  r more info on c
+00006530: 6f6e 6669 6775 7261 7469 6f6e 2069 6620  onfiguration if 
+00006540: 6e65 6564 6564 2e0a 0a20 2020 2020 2020  needed...       
+00006550: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00006560: 2020 2063 6f6e 6669 6766 696c 6520 2873     configfile (s
+00006570: 7472 293a 2054 6865 2070 6174 6820 746f  tr): The path to
+00006580: 2079 6f75 7220 636f 6e66 6967 7572 6174   your configurat
+00006590: 696f 6e20 6669 6c65 2e20 4f70 7469 6f6e  ion file. Option
+000065a0: 616c 2e0a 2020 2020 2020 2020 2020 2020  al..            
+000065b0: 696e 6974 5f73 6c75 726d 2028 626f 6f6c  init_slurm (bool
+000065c0: 293a 2049 6e69 7469 6174 6520 2f20 7661  ): Initiate / va
+000065d0: 6c69 6461 7465 2073 6c75 726d 2073 6574  lidate slurm set
+000065e0: 7570 2e20 4f70 7469 6f6e 616c 0a20 2020  up. Optional.   
+000065f0: 2020 2020 2020 2020 2020 2020 204d 6967               Mig
+00006600: 6874 2074 616b 6520 736f 6d65 2074 696d  ht take some tim
+00006610: 6520 7468 6520 6669 7273 7420 7469 6d65  e the first time
+00006620: 2077 6974 6820 646f 776e 6c6f 6164 696e   with downloadin
+00006630: 6720 6574 632e 0a0a 2020 2020 2020 2020  g etc...        
+00006640: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00006650: 2020 2020 2053 6c75 726d 436c 6965 6e74       SlurmClient
+00006660: 3a20 4120 6e65 7720 536c 7572 6d43 6c69  : A new SlurmCli
+00006670: 656e 7420 6f62 6a65 6374 2e0a 2020 2020  ent object..    
+00006680: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00006690: 2320 4c6f 6164 2074 6865 2063 6f6e 6669  # Load the confi
+000066a0: 6775 7261 7469 6f6e 2066 696c 650a 2020  guration file.  
+000066b0: 2020 2020 2020 636f 6e66 6967 7320 3d20        configs = 
+000066c0: 636f 6e66 6967 7061 7273 6572 2e43 6f6e  configparser.Con
+000066d0: 6669 6750 6172 7365 7228 616c 6c6f 775f  figParser(allow_
+000066e0: 6e6f 5f76 616c 7565 3d54 7275 6529 0a20  no_value=True). 
+000066f0: 2020 2020 2020 2023 204c 6f61 6473 2066         # Loads f
+00006700: 726f 6d20 6465 6661 756c 7420 6c6f 6361  rom default loca
+00006710: 7469 6f6e 7320 616e 6420 6769 7665 6e20  tions and given 
+00006720: 6c6f 6361 7469 6f6e 2c20 6d69 7373 696e  location, missin
+00006730: 6720 6669 6c65 7320 6172 6520 6f6b 0a20  g files are ok. 
+00006740: 2020 2020 2020 2063 6f6e 6669 6773 2e72         configs.r
+00006750: 6561 6428 5b63 6c73 2e5f 4445 4641 554c  ead([cls._DEFAUL
+00006760: 545f 434f 4e46 4947 5f50 4154 485f 312c  T_CONFIG_PATH_1,
+00006770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006780: 2020 2020 2020 636c 732e 5f44 4546 4155        cls._DEFAU
+00006790: 4c54 5f43 4f4e 4649 475f 5041 5448 5f32  LT_CONFIG_PATH_2
+000067a0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000067b0: 2020 2020 2020 2063 6f6e 6669 6766 696c         configfil
+000067c0: 655d 290a 2020 2020 2020 2020 2320 5265  e]).        # Re
+000067d0: 6164 2074 6865 2072 6571 7569 7265 6420  ad the required 
+000067e0: 7061 7261 6d65 7465 7273 2066 726f 6d20  parameters from 
+000067f0: 7468 6520 636f 6e66 6967 7572 6174 696f  the configuratio
+00006800: 6e20 6669 6c65 2c0a 2020 2020 2020 2020  n file,.        
+00006810: 2320 6661 6c6c 6261 636b 2074 6f20 6465  # fallback to de
+00006820: 6661 756c 7473 0a20 2020 2020 2020 2068  faults.        h
+00006830: 6f73 7420 3d20 636f 6e66 6967 732e 6765  ost = configs.ge
+00006840: 7428 2253 5348 222c 2022 686f 7374 222c  t("SSH", "host",
+00006850: 2066 616c 6c62 6163 6b3d 636c 732e 5f44   fallback=cls._D
+00006860: 4546 4155 4c54 5f48 4f53 5429 0a20 2020  EFAULT_HOST).   
+00006870: 2020 2020 2069 6e6c 696e 655f 7373 685f       inline_ssh_
+00006880: 656e 7620 3d20 636f 6e66 6967 732e 6765  env = configs.ge
+00006890: 7462 6f6f 6c65 616e 280a 2020 2020 2020  tboolean(.      
+000068a0: 2020 2020 2020 2253 5348 222c 2022 696e        "SSH", "in
+000068b0: 6c69 6e65 5f73 7368 5f65 6e76 222c 2066  line_ssh_env", f
+000068c0: 616c 6c62 6163 6b3d 636c 732e 5f44 4546  allback=cls._DEF
+000068d0: 4155 4c54 5f49 4e4c 494e 455f 5353 485f  AULT_INLINE_SSH_
+000068e0: 454e 5629 0a20 2020 2020 2020 2073 6c75  ENV).        slu
+000068f0: 726d 5f64 6174 615f 7061 7468 203d 2063  rm_data_path = c
+00006900: 6f6e 6669 6773 2e67 6574 280a 2020 2020  onfigs.get(.    
+00006910: 2020 2020 2020 2020 2253 4c55 524d 222c          "SLURM",
+00006920: 2022 736c 7572 6d5f 6461 7461 5f70 6174   "slurm_data_pat
+00006930: 6822 2c20 6661 6c6c 6261 636b 3d63 6c73  h", fallback=cls
+00006940: 2e5f 4445 4641 554c 545f 534c 5552 4d5f  ._DEFAULT_SLURM_
+00006950: 4441 5441 5f50 4154 4829 0a20 2020 2020  DATA_PATH).     
+00006960: 2020 2073 6c75 726d 5f69 6d61 6765 735f     slurm_images_
+00006970: 7061 7468 203d 2063 6f6e 6669 6773 2e67  path = configs.g
+00006980: 6574 280a 2020 2020 2020 2020 2020 2020  et(.            
+00006990: 2253 4c55 524d 222c 2022 736c 7572 6d5f  "SLURM", "slurm_
+000069a0: 696d 6167 6573 5f70 6174 6822 2c0a 2020  images_path",.  
+000069b0: 2020 2020 2020 2020 2020 6661 6c6c 6261            fallba
+000069c0: 636b 3d63 6c73 2e5f 4445 4641 554c 545f  ck=cls._DEFAULT_
+000069d0: 534c 5552 4d5f 494d 4147 4553 5f50 4154  SLURM_IMAGES_PAT
+000069e0: 4829 0a20 2020 2020 2020 2073 6c75 726d  H).        slurm
+000069f0: 5f63 6f6e 7665 7274 6572 735f 7061 7468  _converters_path
+00006a00: 203d 2063 6f6e 6669 6773 2e67 6574 280a   = configs.get(.
+00006a10: 2020 2020 2020 2020 2020 2020 2253 4c55              "SLU
+00006a20: 524d 222c 2022 736c 7572 6d5f 636f 6e76  RM", "slurm_conv
+00006a30: 6572 7465 7273 5f70 6174 6822 2c0a 2020  erters_path",.  
+00006a40: 2020 2020 2020 2020 2020 6661 6c6c 6261            fallba
+00006a50: 636b 3d63 6c73 2e5f 4445 4641 554c 545f  ck=cls._DEFAULT_
+00006a60: 534c 5552 4d5f 434f 4e56 4552 5445 5253  SLURM_CONVERTERS
+00006a70: 5f50 4154 4829 0a0a 2020 2020 2020 2020  _PATH)..        
+00006a80: 2320 5370 6c69 7420 7468 6520 4d4f 4445  # Split the MODE
+00006a90: 4c53 2069 6e74 6f20 7061 7468 732c 2072  LS into paths, r
+00006aa0: 6570 6f73 2061 6e64 2069 6d61 6765 730a  epos and images.
+00006ab0: 2020 2020 2020 2020 6d6f 6465 6c73 5f64          models_d
+00006ac0: 6963 7420 3d20 6469 6374 2863 6f6e 6669  ict = dict(confi
+00006ad0: 6773 2e69 7465 6d73 2822 4d4f 4445 4c53  gs.items("MODELS
+00006ae0: 2229 290a 2020 2020 2020 2020 736c 7572  ")).        slur
+00006af0: 6d5f 6d6f 6465 6c5f 7061 7468 7320 3d20  m_model_paths = 
+00006b00: 7b7d 0a20 2020 2020 2020 2073 6c75 726d  {}.        slurm
+00006b10: 5f6d 6f64 656c 5f72 6570 6f73 203d 207b  _model_repos = {
+00006b20: 7d0a 2020 2020 2020 2020 736c 7572 6d5f  }.        slurm_
+00006b30: 6d6f 6465 6c5f 6a6f 6273 203d 207b 7d0a  model_jobs = {}.
+00006b40: 2020 2020 2020 2020 736c 7572 6d5f 6d6f          slurm_mo
+00006b50: 6465 6c5f 6a6f 6273 5f70 6172 616d 7320  del_jobs_params 
+00006b60: 3d20 7b7d 0a20 2020 2020 2020 2066 6f72  = {}.        for
+00006b70: 206b 2c20 7620 696e 206d 6f64 656c 735f   k, v in models_
+00006b80: 6469 6374 2e69 7465 6d73 2829 3a0a 2020  dict.items():.  
+00006b90: 2020 2020 2020 2020 2020 7375 6666 6978            suffix
+00006ba0: 5f72 6570 6f20 3d20 275f 7265 706f 270a  _repo = '_repo'.
+00006bb0: 2020 2020 2020 2020 2020 2020 7375 6666              suff
+00006bc0: 6978 5f6a 6f62 203d 2027 5f6a 6f62 270a  ix_job = '_job'.
+00006bd0: 2020 2020 2020 2020 2020 2020 6a6f 625f              job_
+00006be0: 7061 7261 6d5f 7061 7474 6572 6e20 3d20  param_pattern = 
+00006bf0: 2228 2e2b 295f 6a6f 625f 282e 2b29 220a  "(.+)_job_(.+)".
+00006c00: 2020 2020 2020 2020 2020 2020 6a6f 625f              job_
+00006c10: 7061 7261 6d5f 6d61 7463 6820 3d20 7265  param_match = re
+00006c20: 2e6d 6174 6368 286a 6f62 5f70 6172 616d  .match(job_param
+00006c30: 5f70 6174 7465 726e 2c20 6b29 0a20 2020  _pattern, k).   
+00006c40: 2020 2020 2020 2020 2069 6620 6b2e 656e           if k.en
+00006c50: 6473 7769 7468 2873 7566 6669 785f 7265  dswith(suffix_re
+00006c60: 706f 293a 0a20 2020 2020 2020 2020 2020  po):.           
+00006c70: 2020 2020 2073 6c75 726d 5f6d 6f64 656c       slurm_model
+00006c80: 5f72 6570 6f73 5b6b 5b3a 2d6c 656e 2873  _repos[k[:-len(s
+00006c90: 7566 6669 785f 7265 706f 295d 5d20 3d20  uffix_repo)]] = 
+00006ca0: 760a 2020 2020 2020 2020 2020 2020 656c  v.            el
+00006cb0: 6966 206b 2e65 6e64 7377 6974 6828 7375  if k.endswith(su
+00006cc0: 6666 6978 5f6a 6f62 293a 0a20 2020 2020  ffix_job):.     
+00006cd0: 2020 2020 2020 2020 2020 2073 6c75 726d             slurm
+00006ce0: 5f6d 6f64 656c 5f6a 6f62 735b 6b5b 3a2d  _model_jobs[k[:-
+00006cf0: 6c65 6e28 7375 6666 6978 5f6a 6f62 295d  len(suffix_job)]
+00006d00: 5d20 3d20 760a 2020 2020 2020 2020 2020  ] = v.          
+00006d10: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
+00006d20: 6c5f 6a6f 6273 5f70 6172 616d 735b 6b5b  l_jobs_params[k[
+00006d30: 3a2d 6c65 6e28 7375 6666 6978 5f6a 6f62  :-len(suffix_job
+00006d40: 295d 5d20 3d20 5b5d 0a20 2020 2020 2020  )]] = [].       
+00006d50: 2020 2020 2065 6c69 6620 6a6f 625f 7061       elif job_pa
+00006d60: 7261 6d5f 6d61 7463 683a 0a20 2020 2020  ram_match:.     
+00006d70: 2020 2020 2020 2020 2020 2070 7269 6e74             print
+00006d80: 2866 224d 6174 6368 3a20 7b73 6c75 726d  (f"Match: {slurm
+00006d90: 5f6d 6f64 656c 5f6a 6f62 735f 7061 7261  _model_jobs_para
+00006da0: 6d73 7d22 290a 2020 2020 2020 2020 2020  ms}").          
+00006db0: 2020 2020 2020 736c 7572 6d5f 6d6f 6465        slurm_mode
+00006dc0: 6c5f 6a6f 6273 5f70 6172 616d 735b 6a6f  l_jobs_params[jo
+00006dd0: 625f 7061 7261 6d5f 6d61 7463 682e 6772  b_param_match.gr
+00006de0: 6f75 7028 3129 5d2e 6170 7065 6e64 280a  oup(1)].append(.
 00006df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006e00: 6622 202d 2d7b 6a6f 625f 7061 7261 6d5f  f" --{job_param_
-00006e10: 6d61 7463 682e 6772 6f75 7028 3229 7d3d  match.group(2)}=
-00006e20: 7b76 7d22 290a 2020 2020 2020 2020 2020  {v}").          
-00006e30: 2020 2020 2020 7072 696e 7428 6622 4164        print(f"Ad
-00006e40: 6465 643a 207b 736c 7572 6d5f 6d6f 6465  ded: {slurm_mode
-00006e50: 6c5f 6a6f 6273 5f70 6172 616d 737d 2229  l_jobs_params}")
-00006e60: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-00006e70: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00006e80: 2020 2073 6c75 726d 5f6d 6f64 656c 5f70     slurm_model_p
-00006e90: 6174 6873 5b6b 5d20 3d20 760a 0a20 2020  aths[k] = v..   
-00006ea0: 2020 2020 2073 6c75 726d 5f73 6372 6970       slurm_scrip
-00006eb0: 745f 7061 7468 203d 2063 6f6e 6669 6773  t_path = configs
-00006ec0: 2e67 6574 280a 2020 2020 2020 2020 2020  .get(.          
-00006ed0: 2020 2253 4c55 524d 222c 2022 736c 7572    "SLURM", "slur
-00006ee0: 6d5f 7363 7269 7074 5f70 6174 6822 2c0a  m_script_path",.
-00006ef0: 2020 2020 2020 2020 2020 2020 6661 6c6c              fall
-00006f00: 6261 636b 3d63 6c73 2e5f 4445 4641 554c  back=cls._DEFAUL
-00006f10: 545f 534c 5552 4d5f 4749 545f 5343 5249  T_SLURM_GIT_SCRI
-00006f20: 5054 5f50 4154 4829 0a20 2020 2020 2020  PT_PATH).       
-00006f30: 2073 6c75 726d 5f73 6372 6970 745f 7265   slurm_script_re
-00006f40: 706f 203d 2063 6f6e 6669 6773 2e67 6574  po = configs.get
-00006f50: 280a 2020 2020 2020 2020 2020 2020 2253  (.            "S
-00006f60: 4c55 524d 222c 2022 736c 7572 6d5f 7363  LURM", "slurm_sc
-00006f70: 7269 7074 5f72 6570 6f22 2c0a 2020 2020  ript_repo",.    
-00006f80: 2020 2020 2020 2020 6661 6c6c 6261 636b          fallback
-00006f90: 3d4e 6f6e 650a 2020 2020 2020 2020 290a  =None.        ).
-00006fa0: 2020 2020 2020 2020 2320 4372 6561 7465          # Create
-00006fb0: 2074 6865 2053 6c75 726d 436c 6965 6e74   the SlurmClient
-00006fc0: 206f 626a 6563 7420 7769 7468 2074 6865   object with the
-00006fd0: 2070 6172 616d 6574 6572 7320 7265 6164   parameters read
-00006fe0: 2066 726f 6d0a 2020 2020 2020 2020 2320   from.        # 
-00006ff0: 7468 6520 636f 6e66 6967 2066 696c 650a  the config file.
-00007000: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00007010: 6c73 2868 6f73 743d 686f 7374 2c0a 2020  ls(host=host,.  
-00007020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007030: 2069 6e6c 696e 655f 7373 685f 656e 763d   inline_ssh_env=
-00007040: 696e 6c69 6e65 5f73 7368 5f65 6e76 2c0a  inline_ssh_env,.
-00007050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007060: 2020 2073 6c75 726d 5f64 6174 615f 7061     slurm_data_pa
-00007070: 7468 3d73 6c75 726d 5f64 6174 615f 7061  th=slurm_data_pa
-00007080: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
-00007090: 2020 2020 2020 2073 6c75 726d 5f69 6d61         slurm_ima
-000070a0: 6765 735f 7061 7468 3d73 6c75 726d 5f69  ges_path=slurm_i
-000070b0: 6d61 6765 735f 7061 7468 2c0a 2020 2020  mages_path,.    
-000070c0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000070d0: 6c75 726d 5f63 6f6e 7665 7274 6572 735f  lurm_converters_
-000070e0: 7061 7468 3d73 6c75 726d 5f63 6f6e 7665  path=slurm_conve
-000070f0: 7274 6572 735f 7061 7468 2c0a 2020 2020  rters_path,.    
-00007100: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00007110: 6c75 726d 5f6d 6f64 656c 5f70 6174 6873  lurm_model_paths
-00007120: 3d73 6c75 726d 5f6d 6f64 656c 5f70 6174  =slurm_model_pat
-00007130: 6873 2c0a 2020 2020 2020 2020 2020 2020  hs,.            
-00007140: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
-00007150: 656c 5f72 6570 6f73 3d73 6c75 726d 5f6d  el_repos=slurm_m
-00007160: 6f64 656c 5f72 6570 6f73 2c0a 2020 2020  odel_repos,.    
-00007170: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00007180: 6c75 726d 5f6d 6f64 656c 5f69 6d61 6765  lurm_model_image
-00007190: 733d 4e6f 6e65 2c0a 2020 2020 2020 2020  s=None,.        
-000071a0: 2020 2020 2020 2020 2020 2073 6c75 726d             slurm
-000071b0: 5f6d 6f64 656c 5f6a 6f62 733d 736c 7572  _model_jobs=slur
-000071c0: 6d5f 6d6f 6465 6c5f 6a6f 6273 2c0a 2020  m_model_jobs,.  
-000071d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000071e0: 2073 6c75 726d 5f6d 6f64 656c 5f6a 6f62   slurm_model_job
-000071f0: 735f 7061 7261 6d73 3d73 6c75 726d 5f6d  s_params=slurm_m
-00007200: 6f64 656c 5f6a 6f62 735f 7061 7261 6d73  odel_jobs_params
-00007210: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007220: 2020 2020 2073 6c75 726d 5f73 6372 6970       slurm_scrip
-00007230: 745f 7061 7468 3d73 6c75 726d 5f73 6372  t_path=slurm_scr
-00007240: 6970 745f 7061 7468 2c0a 2020 2020 2020  ipt_path,.      
-00007250: 2020 2020 2020 2020 2020 2020 2073 6c75               slu
-00007260: 726d 5f73 6372 6970 745f 7265 706f 3d73  rm_script_repo=s
-00007270: 6c75 726d 5f73 6372 6970 745f 7265 706f  lurm_script_repo
-00007280: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00007290: 2020 2020 2069 6e69 745f 736c 7572 6d3d       init_slurm=
-000072a0: 696e 6974 5f73 6c75 726d 290a 0a20 2020  init_slurm)..   
-000072b0: 2064 6566 2063 6c65 616e 7570 5f74 6d70   def cleanup_tmp
-000072c0: 5f66 696c 6573 2873 656c 662c 0a20 2020  _files(self,.   
-000072d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000072e0: 2020 2020 2020 2073 6c75 726d 5f6a 6f62         slurm_job
-000072f0: 5f69 643a 2073 7472 2c0a 2020 2020 2020  _id: str,.      
+00006e00: 2020 2020 6622 202d 2d7b 6a6f 625f 7061      f" --{job_pa
+00006e10: 7261 6d5f 6d61 7463 682e 6772 6f75 7028  ram_match.group(
+00006e20: 3229 7d3d 7b76 7d22 290a 2020 2020 2020  2)}={v}").      
+00006e30: 2020 2020 2020 2020 2020 7072 696e 7428            print(
+00006e40: 6622 4164 6465 643a 207b 736c 7572 6d5f  f"Added: {slurm_
+00006e50: 6d6f 6465 6c5f 6a6f 6273 5f70 6172 616d  model_jobs_param
+00006e60: 737d 2229 0a20 2020 2020 2020 2020 2020  s}").           
+00006e70: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00006e80: 2020 2020 2020 2073 6c75 726d 5f6d 6f64         slurm_mod
+00006e90: 656c 5f70 6174 6873 5b6b 5d20 3d20 760a  el_paths[k] = v.
+00006ea0: 0a20 2020 2020 2020 2073 6c75 726d 5f73  .        slurm_s
+00006eb0: 6372 6970 745f 7061 7468 203d 2063 6f6e  cript_path = con
+00006ec0: 6669 6773 2e67 6574 280a 2020 2020 2020  figs.get(.      
+00006ed0: 2020 2020 2020 2253 4c55 524d 222c 2022        "SLURM", "
+00006ee0: 736c 7572 6d5f 7363 7269 7074 5f70 6174  slurm_script_pat
+00006ef0: 6822 2c0a 2020 2020 2020 2020 2020 2020  h",.            
+00006f00: 6661 6c6c 6261 636b 3d63 6c73 2e5f 4445  fallback=cls._DE
+00006f10: 4641 554c 545f 534c 5552 4d5f 4749 545f  FAULT_SLURM_GIT_
+00006f20: 5343 5249 5054 5f50 4154 4829 0a20 2020  SCRIPT_PATH).   
+00006f30: 2020 2020 2073 6c75 726d 5f73 6372 6970       slurm_scrip
+00006f40: 745f 7265 706f 203d 2063 6f6e 6669 6773  t_repo = configs
+00006f50: 2e67 6574 280a 2020 2020 2020 2020 2020  .get(.          
+00006f60: 2020 2253 4c55 524d 222c 2022 736c 7572    "SLURM", "slur
+00006f70: 6d5f 7363 7269 7074 5f72 6570 6f22 2c0a  m_script_repo",.
+00006f80: 2020 2020 2020 2020 2020 2020 6661 6c6c              fall
+00006f90: 6261 636b 3d4e 6f6e 650a 2020 2020 2020  back=None.      
+00006fa0: 2020 290a 2020 2020 2020 2020 2320 4372    ).        # Cr
+00006fb0: 6561 7465 2074 6865 2053 6c75 726d 436c  eate the SlurmCl
+00006fc0: 6965 6e74 206f 626a 6563 7420 7769 7468  ient object with
+00006fd0: 2074 6865 2070 6172 616d 6574 6572 7320   the parameters 
+00006fe0: 7265 6164 2066 726f 6d0a 2020 2020 2020  read from.      
+00006ff0: 2020 2320 7468 6520 636f 6e66 6967 2066    # the config f
+00007000: 696c 650a 2020 2020 2020 2020 7265 7475  ile.        retu
+00007010: 726e 2063 6c73 2868 6f73 743d 686f 7374  rn cls(host=host
+00007020: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00007030: 2020 2020 2069 6e6c 696e 655f 7373 685f       inline_ssh_
+00007040: 656e 763d 696e 6c69 6e65 5f73 7368 5f65  env=inline_ssh_e
+00007050: 6e76 2c0a 2020 2020 2020 2020 2020 2020  nv,.            
+00007060: 2020 2020 2020 2073 6c75 726d 5f64 6174         slurm_dat
+00007070: 615f 7061 7468 3d73 6c75 726d 5f64 6174  a_path=slurm_dat
+00007080: 615f 7061 7468 2c0a 2020 2020 2020 2020  a_path,.        
+00007090: 2020 2020 2020 2020 2020 2073 6c75 726d             slurm
+000070a0: 5f69 6d61 6765 735f 7061 7468 3d73 6c75  _images_path=slu
+000070b0: 726d 5f69 6d61 6765 735f 7061 7468 2c0a  rm_images_path,.
+000070c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000070d0: 2020 2073 6c75 726d 5f63 6f6e 7665 7274     slurm_convert
+000070e0: 6572 735f 7061 7468 3d73 6c75 726d 5f63  ers_path=slurm_c
+000070f0: 6f6e 7665 7274 6572 735f 7061 7468 2c0a  onverters_path,.
+00007100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007110: 2020 2073 6c75 726d 5f6d 6f64 656c 5f70     slurm_model_p
+00007120: 6174 6873 3d73 6c75 726d 5f6d 6f64 656c  aths=slurm_model
+00007130: 5f70 6174 6873 2c0a 2020 2020 2020 2020  _paths,.        
+00007140: 2020 2020 2020 2020 2020 2073 6c75 726d             slurm
+00007150: 5f6d 6f64 656c 5f72 6570 6f73 3d73 6c75  _model_repos=slu
+00007160: 726d 5f6d 6f64 656c 5f72 6570 6f73 2c0a  rm_model_repos,.
+00007170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007180: 2020 2073 6c75 726d 5f6d 6f64 656c 5f69     slurm_model_i
+00007190: 6d61 6765 733d 4e6f 6e65 2c0a 2020 2020  mages=None,.    
+000071a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000071b0: 6c75 726d 5f6d 6f64 656c 5f6a 6f62 733d  lurm_model_jobs=
+000071c0: 736c 7572 6d5f 6d6f 6465 6c5f 6a6f 6273  slurm_model_jobs
+000071d0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000071e0: 2020 2020 2073 6c75 726d 5f6d 6f64 656c       slurm_model
+000071f0: 5f6a 6f62 735f 7061 7261 6d73 3d73 6c75  _jobs_params=slu
+00007200: 726d 5f6d 6f64 656c 5f6a 6f62 735f 7061  rm_model_jobs_pa
+00007210: 7261 6d73 2c0a 2020 2020 2020 2020 2020  rams,.          
+00007220: 2020 2020 2020 2020 2073 6c75 726d 5f73           slurm_s
+00007230: 6372 6970 745f 7061 7468 3d73 6c75 726d  cript_path=slurm
+00007240: 5f73 6372 6970 745f 7061 7468 2c0a 2020  _script_path,.  
+00007250: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00007260: 2073 6c75 726d 5f73 6372 6970 745f 7265   slurm_script_re
+00007270: 706f 3d73 6c75 726d 5f73 6372 6970 745f  po=slurm_script_
+00007280: 7265 706f 2c0a 2020 2020 2020 2020 2020  repo,.          
+00007290: 2020 2020 2020 2020 2069 6e69 745f 736c           init_sl
+000072a0: 7572 6d3d 696e 6974 5f73 6c75 726d 290a  urm=init_slurm).
+000072b0: 0a20 2020 2064 6566 2063 6c65 616e 7570  .    def cleanup
+000072c0: 5f74 6d70 5f66 696c 6573 2873 656c 662c  _tmp_files(self,
+000072d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000072e0: 2020 2020 2020 2020 2020 2073 6c75 726d             slurm
+000072f0: 5f6a 6f62 5f69 643a 2073 7472 2c0a 2020  _job_id: str,.  
 00007300: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007310: 2020 2020 6669 6c65 6e61 6d65 3a20 7374      filename: st
-00007320: 7220 3d20 4e6f 6e65 2c0a 2020 2020 2020  r = None,.      
+00007310: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
+00007320: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
 00007330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007340: 2020 2020 6461 7461 5f6c 6f63 6174 696f      data_locatio
-00007350: 6e3a 2073 7472 203d 204e 6f6e 652c 0a20  n: str = None,. 
-00007360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007370: 2020 2020 2020 2020 206c 6f67 6669 6c65           logfile
-00007380: 3a20 7374 7220 3d20 4e6f 6e65 2c0a 2020  : str = None,.  
-00007390: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000073a0: 2020 2020 2020 2020 2920 2d3e 2052 6573          ) -> Res
-000073b0: 756c 743a 0a20 2020 2020 2020 2022 2222  ult:.        """
-000073c0: 0a20 2020 2020 2020 2043 6c65 616e 7570  .        Cleanup
-000073d0: 207a 6970 2061 6e64 2075 6e7a 6970 7065   zip and unzippe
-000073e0: 6420 6669 6c65 732f 666f 6c64 6572 7320  d files/folders 
-000073f0: 6173 736f 6369 6174 6564 2077 6974 6820  associated with 
-00007400: 6120 536c 7572 6d20 6a6f 622e 0a0a 2020  a Slurm job...  
-00007410: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00007420: 2020 2020 2020 2020 736c 7572 6d5f 6a6f          slurm_jo
-00007430: 625f 6964 2028 7374 7229 3a20 5468 6520  b_id (str): The 
-00007440: 6a6f 6220 4944 206f 6620 7468 6520 536c  job ID of the Sl
-00007450: 7572 6d20 7363 7269 7074 2e0a 2020 2020  urm script..    
-00007460: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
-00007470: 2028 7374 7229 3a20 5468 6520 7a69 7020   (str): The zip 
-00007480: 6669 6c65 6e61 6d65 206f 6e20 536c 7572  filename on Slur
-00007490: 6d2e 0a20 2020 2020 2020 2020 2020 2064  m..            d
-000074a0: 6174 615f 6c6f 6361 7469 6f6e 2028 7374  ata_location (st
-000074b0: 722c 206f 7074 696f 6e61 6c29 3a20 5468  r, optional): Th
-000074c0: 6520 6c6f 6361 7469 6f6e 206f 6620 6461  e location of da
-000074d0: 7461 2066 696c 6573 206f 6e20 536c 7572  ta files on Slur
-000074e0: 6d2e 0a20 2020 2020 2020 2020 2020 2020  m..             
-000074f0: 2020 2049 6620 6e6f 7420 7072 6f76 6964     If not provid
-00007500: 6564 2c20 6974 2077 696c 6c20 6265 2065  ed, it will be e
-00007510: 7874 7261 6374 6564 2066 726f 6d20 7468  xtracted from th
-00007520: 6520 6c6f 6720 6669 6c65 2e0a 2020 2020  e log file..    
-00007530: 2020 2020 2020 2020 6c6f 6766 696c 6520          logfile 
-00007540: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
-00007550: 2054 6865 206c 6f67 2066 696c 6520 6f66   The log file of
-00007560: 2074 6865 2053 6c75 726d 206a 6f62 2e20   the Slurm job. 
-00007570: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00007580: 2049 6620 6e6f 7420 7072 6f76 6964 6564   If not provided
-00007590: 2c20 6120 6465 6661 756c 7420 6c6f 6720  , a default log 
-000075a0: 6669 6c65 2077 696c 6c20 6265 2075 7365  file will be use
-000075b0: 642e 0a0a 2020 2020 2020 2020 5265 7475  d...        Retu
-000075c0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-000075d0: 2052 6573 756c 743a 2054 6865 2072 6573   Result: The res
-000075e0: 756c 7420 6f66 2074 6865 2063 6c65 616e  ult of the clean
-000075f0: 7570 206f 7065 7261 7469 6f6e 2e0a 0a20  up operation... 
-00007600: 2020 2020 2020 204e 6f74 653a 0a20 2020         Note:.   
-00007610: 2020 2020 2020 2020 2054 6865 2063 6c65           The cle
-00007620: 616e 7570 2070 726f 6365 7373 2069 6e76  anup process inv
-00007630: 6f6c 7665 7320 7265 6d6f 7669 6e67 2074  olves removing t
-00007640: 6865 2073 7065 6369 6669 6564 207a 6970  he specified zip
-00007650: 2066 696c 652c 200a 2020 2020 2020 2020   file, .        
-00007660: 2020 2020 7468 6520 6c6f 6720 6669 6c65      the log file
-00007670: 2c20 616e 6420 6173 736f 6369 6174 6564  , and associated
-00007680: 2064 6174 6120 6669 6c65 7320 616e 6420   data files and 
-00007690: 666f 6c64 6572 732e 0a0a 2020 2020 2020  folders...      
-000076a0: 2020 4578 616d 706c 653a 0a20 2020 2020    Example:.     
-000076b0: 2020 2020 2020 2023 2043 6c65 616e 7570         # Cleanup
-000076c0: 2074 656d 706f 7261 7279 2066 696c 6573   temporary files
-000076d0: 2066 6f72 2061 2053 6c75 726d 206a 6f62   for a Slurm job
-000076e0: 0a20 2020 2020 2020 2020 2020 2063 6c69  .            cli
-000076f0: 656e 742e 636c 6561 6e75 705f 746d 705f  ent.cleanup_tmp_
-00007700: 6669 6c65 7328 2231 3233 3435 222c 2022  files("12345", "
-00007710: 6f75 7470 7574 2e7a 6970 2229 0a20 2020  output.zip").   
-00007720: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00007730: 2063 6d64 7320 3d20 5b5d 0a20 2020 2020   cmds = [].     
-00007740: 2020 2023 207a 6970 0a20 2020 2020 2020     # zip.       
-00007750: 2069 6620 6669 6c65 6e61 6d65 3a0a 2020   if filename:.  
-00007760: 2020 2020 2020 2020 2020 726d 7a69 7020            rmzip 
-00007770: 3d20 6622 726d 205c 227b 6669 6c65 6e61  = f"rm \"{filena
-00007780: 6d65 7d5c 222e 2a22 0a20 2020 2020 2020  me}\".*".       
-00007790: 2020 2020 2063 6d64 732e 6170 7065 6e64       cmds.append
-000077a0: 2872 6d7a 6970 290a 2020 2020 2020 2020  (rmzip).        
-000077b0: 2320 6c6f 670a 2020 2020 2020 2020 6966  # log.        if
-000077c0: 206c 6f67 6669 6c65 2069 7320 4e6f 6e65   logfile is None
-000077d0: 3a0a 2020 2020 2020 2020 2020 2020 6c6f  :.            lo
-000077e0: 6766 696c 6520 3d20 7365 6c66 2e5f 4c4f  gfile = self._LO
-000077f0: 4746 494c 450a 2020 2020 2020 2020 2020  GFILE.          
-00007800: 2020 6c6f 6766 696c 6520 3d20 6c6f 6766    logfile = logf
-00007810: 696c 652e 666f 726d 6174 2873 6c75 726d  ile.format(slurm
-00007820: 5f6a 6f62 5f69 643d 736c 7572 6d5f 6a6f  _job_id=slurm_jo
-00007830: 625f 6964 290a 2020 2020 2020 2020 726d  b_id).        rm
-00007840: 6c6f 6720 3d20 6622 726d 205c 227b 6c6f  log = f"rm \"{lo
-00007850: 6766 696c 657d 5c22 220a 2020 2020 2020  gfile}\"".      
-00007860: 2020 636d 6473 2e61 7070 656e 6428 726d    cmds.append(rm
-00007870: 6c6f 6729 0a20 2020 2020 2020 2023 2063  log).        # c
-00007880: 6f6e 7665 7274 6572 206c 6f67 730a 2020  onverter logs.  
-00007890: 2020 2020 2020 636c 6f67 203d 2073 656c        clog = sel
-000078a0: 662e 5f43 4f4e 5645 5254 4552 5f4c 4f47  f._CONVERTER_LOG
-000078b0: 4649 4c45 0a20 2020 2020 2020 2063 6c6f  FILE.        clo
-000078c0: 6720 3d20 636c 6f67 2e66 6f72 6d61 7428  g = clog.format(
-000078d0: 736c 7572 6d5f 6a6f 625f 6964 3d73 6c75  slurm_job_id=slu
-000078e0: 726d 5f6a 6f62 5f69 6429 0a20 2020 2020  rm_job_id).     
-000078f0: 2020 2072 6d63 6c6f 6720 3d20 6622 726d     rmclog = f"rm
-00007900: 207b 636c 6f67 7d22 0a20 2020 2020 2020   {clog}".       
-00007910: 2063 6d64 732e 6170 7065 6e64 2872 6d63   cmds.append(rmc
-00007920: 6c6f 6729 0a20 2020 2020 2020 200a 2020  log).        .  
-00007930: 2020 2020 2020 2320 6461 7461 0a20 2020        # data.   
-00007940: 2020 2020 2069 6620 6461 7461 5f6c 6f63       if data_loc
-00007950: 6174 696f 6e20 6973 204e 6f6e 653a 0a20  ation is None:. 
-00007960: 2020 2020 2020 2020 2020 2064 6174 615f             data_
-00007970: 6c6f 6361 7469 6f6e 203d 2073 656c 662e  location = self.
-00007980: 6578 7472 6163 745f 6461 7461 5f6c 6f63  extract_data_loc
-00007990: 6174 696f 6e5f 6672 6f6d 5f6c 6f67 286c  ation_from_log(l
-000079a0: 6f67 6669 6c65 290a 2020 2020 2020 2020  ogfile).        
-000079b0: 2020 2020 0a20 2020 2020 2020 2069 6620      .        if 
-000079c0: 6461 7461 5f6c 6f63 6174 696f 6e3a 0a20  data_location:. 
-000079d0: 2020 2020 2020 2020 2020 2072 6d64 6174             rmdat
-000079e0: 6120 3d20 6622 726d 202d 7266 205c 227b  a = f"rm -rf \"{
-000079f0: 6461 7461 5f6c 6f63 6174 696f 6e7d 5c22  data_location}\"
-00007a00: 205c 227b 6461 7461 5f6c 6f63 6174 696f   \"{data_locatio
-00007a10: 6e7d 5c22 2e2a 220a 2020 2020 2020 2020  n}\".*".        
-00007a20: 2020 2020 636d 6473 2e61 7070 656e 6428      cmds.append(
-00007a30: 726d 6461 7461 290a 2020 2020 2020 2020  rmdata).        
-00007a40: 2020 2020 0a20 2020 2020 2020 2020 2020      .           
-00007a50: 2023 2063 6f6e 7665 7274 2063 6f6e 6669   # convert confi
-00007a60: 6720 6669 6c65 0a20 2020 2020 2020 2020  g file.         
-00007a70: 2020 2063 6f6e 6669 675f 6669 6c65 203d     config_file =
-00007a80: 2066 2263 6f6e 6669 675f 7b6f 732e 7061   f"config_{os.pa
-00007a90: 7468 2e62 6173 656e 616d 6528 6461 7461  th.basename(data
-00007aa0: 5f6c 6f63 6174 696f 6e29 7d2e 7478 7422  _location)}.txt"
-00007ab0: 0a20 2020 2020 2020 2020 2020 2072 6d63  .            rmc
-00007ac0: 6f6e 6669 6720 3d20 6622 726d 205c 227b  onfig = f"rm \"{
-00007ad0: 636f 6e66 6967 5f66 696c 657d 5c22 220a  config_file}\"".
-00007ae0: 2020 2020 2020 2020 2020 2020 636d 6473              cmds
-00007af0: 2e61 7070 656e 6428 726d 636f 6e66 6967  .append(rmconfig
-00007b00: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
-00007b10: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
-00007b20: 6572 2e77 6172 6e69 6e67 2866 2243 6f75  er.warning(f"Cou
-00007b30: 6c64 206e 6f74 2065 7874 7261 6374 2064  ld not extract d
-00007b40: 6174 6120 6c6f 6361 7469 6f6e 2066 726f  ata location fro
-00007b50: 6d20 6c6f 6720 7b6c 6f67 6669 6c65 7d2e  m log {logfile}.
-00007b60: 2053 6b69 7070 696e 6720 636c 6561 6e75   Skipping cleanu
-00007b70: 702e 2229 0a0a 2020 2020 2020 2020 7472  p.")..        tr
-00007b80: 793a 0a20 2020 2020 2020 2020 2020 2023  y:.            #
-00007b90: 2064 6f20 6173 206d 7563 6820 6173 2070   do as much as p
-00007ba0: 6f73 7369 626c 652c 206e 6f74 2063 6f6e  ossible, not con
-00007bb0: 6469 7469 6f6e 616c 2072 656d 6f76 616c  ditional removal
-00007bc0: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
-00007bd0: 756c 7420 3d20 7365 6c66 2e72 756e 5f63  ult = self.run_c
-00007be0: 6f6d 6d61 6e64 7328 636d 6473 2c20 7365  ommands(cmds, se
-00007bf0: 703d 2720 3b20 2729 0a20 2020 2020 2020  p=' ; ').       
-00007c00: 2065 7863 6570 7420 556e 6578 7065 6374   except Unexpect
-00007c10: 6564 4578 6974 2061 7320 653a 0a20 2020  edExit as e:.   
-00007c20: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00007c30: 7761 726e 696e 6728 6529 0a20 2020 2020  warning(e).     
-00007c40: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00007c50: 652e 7265 7375 6c74 0a20 2020 2020 2020  e.result.       
-00007c60: 2072 6574 7572 6e20 7265 7375 6c74 206f   return result o
-00007c70: 7220 4e6f 6e65 0a0a 2020 2020 6465 6620  r None..    def 
-00007c80: 7661 6c69 6461 7465 2873 656c 662c 2076  validate(self, v
-00007c90: 616c 6964 6174 655f 736c 7572 6d5f 7365  alidate_slurm_se
-00007ca0: 7475 703a 2062 6f6f 6c20 3d20 4661 6c73  tup: bool = Fals
-00007cb0: 6529 3a0a 2020 2020 2020 2020 2222 2256  e):.        """V
-00007cc0: 616c 6964 6174 6520 7468 6520 636f 6e6e  alidate the conn
-00007cd0: 6563 7469 6f6e 2074 6f20 7468 6520 536c  ection to the Sl
-00007ce0: 7572 6d20 636c 7573 7465 7220 6279 2072  urm cluster by r
-00007cf0: 756e 6e69 6e67 0a20 2020 2020 2020 2061  unning.        a
-00007d00: 2073 696d 706c 6520 636f 6d6d 616e 642e   simple command.
-00007d10: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00007d20: 2020 2020 2020 2020 2020 2020 7661 6c69              vali
-00007d30: 6461 7465 5f73 6c75 726d 5f73 6574 7570  date_slurm_setup
-00007d40: 2028 626f 6f6c 293a 2057 6865 7468 6572   (bool): Whether
-00007d50: 2074 6f20 616c 736f 2063 6865 636b 0a20   to also check. 
-00007d60: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00007d70: 6e64 2066 6978 2074 6865 2053 6c75 726d  nd fix the Slurm
-00007d80: 2073 6574 7570 2028 666f 6c64 6572 732c   setup (folders,
-00007d90: 2069 6d61 6765 732c 2065 7463 2e29 0a0a   images, etc.)..
-00007da0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00007db0: 0a20 2020 2020 2020 2020 2020 2062 6f6f  .            boo
-00007dc0: 6c3a 0a20 2020 2020 2020 2020 2020 2020  l:.             
-00007dd0: 2020 2054 7275 6520 6966 2074 6865 2076     True if the v
-00007de0: 616c 6964 6174 696f 6e20 6973 2073 7563  alidation is suc
-00007df0: 6365 7373 6675 6c2c 0a20 2020 2020 2020  cessful,.       
-00007e00: 2020 2020 2020 2020 2046 616c 7365 206f           False o
-00007e10: 7468 6572 7769 7365 2e0a 2020 2020 2020  therwise..      
-00007e20: 2020 2222 220a 2020 2020 2020 2020 636f    """.        co
-00007e30: 6e6e 6563 7465 6420 3d20 7365 6c66 2e72  nnected = self.r
-00007e40: 756e 2827 6563 686f 2022 2022 2729 2e6f  un('echo " "').o
-00007e50: 6b0a 2020 2020 2020 2020 6966 2063 6f6e  k.        if con
-00007e60: 6e65 6374 6564 2061 6e64 2076 616c 6964  nected and valid
-00007e70: 6174 655f 736c 7572 6d5f 7365 7475 703a  ate_slurm_setup:
-00007e80: 0a20 2020 2020 2020 2020 2020 2074 7279  .            try
-00007e90: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00007ea0: 2020 7365 6c66 2e73 6574 7570 5f73 6c75    self.setup_slu
-00007eb0: 726d 2829 0a20 2020 2020 2020 2020 2020  rm().           
-00007ec0: 2065 7863 6570 7420 5353 4845 7863 6570   except SSHExcep
-00007ed0: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
-00007ee0: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
-00007ef0: 722e 6572 726f 7228 6529 0a20 2020 2020  r.error(e).     
-00007f00: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00007f10: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
-00007f20: 7265 7475 726e 2063 6f6e 6e65 6374 6564  return connected
-00007f30: 0a0a 2020 2020 6465 6620 6765 745f 7265  ..    def get_re
-00007f40: 6365 6e74 5f6c 6f67 5f63 6f6d 6d61 6e64  cent_log_command
-00007f50: 2873 656c 662c 206c 6f67 5f66 696c 653a  (self, log_file:
-00007f60: 2073 7472 2c20 6e3a 2069 6e74 203d 2031   str, n: int = 1
-00007f70: 3029 202d 3e20 7374 723a 0a20 2020 2020  0) -> str:.     
-00007f80: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
-00007f90: 6574 2074 6865 2063 6f6d 6d61 6e64 2074  et the command t
-00007fa0: 6f20 7265 7472 6965 7665 2074 6865 2072  o retrieve the r
-00007fb0: 6563 656e 7420 6c6f 6720 656e 7472 6965  ecent log entrie
-00007fc0: 7320 6672 6f6d 2061 0a20 2020 2020 2020  s from a.       
-00007fd0: 2073 7065 6369 6669 6564 206c 6f67 2066   specified log f
-00007fe0: 696c 652e 0a0a 2020 2020 2020 2020 4172  ile...        Ar
-00007ff0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00008000: 6c6f 675f 6669 6c65 2028 7374 7229 3a20  log_file (str): 
-00008010: 5468 6520 7061 7468 2074 6f20 7468 6520  The path to the 
-00008020: 6c6f 6720 6669 6c65 2e0a 2020 2020 2020  log file..      
-00008030: 2020 2020 2020 6e20 2869 6e74 2c20 6f70        n (int, op
-00008040: 7469 6f6e 616c 293a 2054 6865 206e 756d  tional): The num
-00008050: 6265 7220 6f66 2072 6563 656e 7420 6c6f  ber of recent lo
-00008060: 6720 656e 7472 6965 7320 746f 2072 6574  g entries to ret
-00008070: 7269 6576 652e 0a20 2020 2020 2020 2020  rieve..         
-00008080: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
-00008090: 746f 2031 302e 0a0a 2020 2020 2020 2020  to 10...        
-000080a0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-000080b0: 2020 2020 2073 7472 3a20 5468 6520 636f       str: The co
-000080c0: 6d6d 616e 6420 746f 2072 6574 7269 6576  mmand to retriev
-000080d0: 6520 7468 6520 7265 6365 6e74 206c 6f67  e the recent log
-000080e0: 2065 6e74 7269 6573 2e0a 2020 2020 2020   entries..      
-000080f0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
-00008100: 7475 726e 2073 656c 662e 5f54 4149 4c5f  turn self._TAIL_
-00008110: 4c4f 475f 434d 442e 666f 726d 6174 286e  LOG_CMD.format(n
-00008120: 3d6e 2c20 6c6f 675f 6669 6c65 3d6c 6f67  =n, log_file=log
-00008130: 5f66 696c 6529 0a0a 2020 2020 6465 6620  _file)..    def 
-00008140: 6765 745f 6163 7469 7665 5f6a 6f62 5f70  get_active_job_p
-00008150: 726f 6772 6573 7328 7365 6c66 2c0a 2020  rogress(self,.  
-00008160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008170: 2020 2020 2020 2020 2020 2020 2020 736c                sl
-00008180: 7572 6d5f 6a6f 625f 6964 3a20 7374 722c  urm_job_id: str,
-00008190: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00007340: 2020 2020 2020 2020 6461 7461 5f6c 6f63          data_loc
+00007350: 6174 696f 6e3a 2073 7472 203d 204e 6f6e  ation: str = Non
+00007360: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00007370: 2020 2020 2020 2020 2020 2020 206c 6f67               log
+00007380: 6669 6c65 3a20 7374 7220 3d20 4e6f 6e65  file: str = None
+00007390: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000073a0: 2020 2020 2020 2020 2020 2020 2920 2d3e              ) ->
+000073b0: 2052 6573 756c 743a 0a20 2020 2020 2020   Result:.       
+000073c0: 2022 2222 0a20 2020 2020 2020 2043 6c65   """.        Cle
+000073d0: 616e 7570 207a 6970 2061 6e64 2075 6e7a  anup zip and unz
+000073e0: 6970 7065 6420 6669 6c65 732f 666f 6c64  ipped files/fold
+000073f0: 6572 7320 6173 736f 6369 6174 6564 2077  ers associated w
+00007400: 6974 6820 6120 536c 7572 6d20 6a6f 622e  ith a Slurm job.
+00007410: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00007420: 2020 2020 2020 2020 2020 2020 736c 7572              slur
+00007430: 6d5f 6a6f 625f 6964 2028 7374 7229 3a20  m_job_id (str): 
+00007440: 5468 6520 6a6f 6220 4944 206f 6620 7468  The job ID of th
+00007450: 6520 536c 7572 6d20 7363 7269 7074 2e0a  e Slurm script..
+00007460: 2020 2020 2020 2020 2020 2020 6669 6c65              file
+00007470: 6e61 6d65 2028 7374 7229 3a20 5468 6520  name (str): The 
+00007480: 7a69 7020 6669 6c65 6e61 6d65 206f 6e20  zip filename on 
+00007490: 536c 7572 6d2e 0a20 2020 2020 2020 2020  Slurm..         
+000074a0: 2020 2064 6174 615f 6c6f 6361 7469 6f6e     data_location
+000074b0: 2028 7374 722c 206f 7074 696f 6e61 6c29   (str, optional)
+000074c0: 3a20 5468 6520 6c6f 6361 7469 6f6e 206f  : The location o
+000074d0: 6620 6461 7461 2066 696c 6573 206f 6e20  f data files on 
+000074e0: 536c 7572 6d2e 0a20 2020 2020 2020 2020  Slurm..         
+000074f0: 2020 2020 2020 2049 6620 6e6f 7420 7072         If not pr
+00007500: 6f76 6964 6564 2c20 6974 2077 696c 6c20  ovided, it will 
+00007510: 6265 2065 7874 7261 6374 6564 2066 726f  be extracted fro
+00007520: 6d20 7468 6520 6c6f 6720 6669 6c65 2e0a  m the log file..
+00007530: 2020 2020 2020 2020 2020 2020 6c6f 6766              logf
+00007540: 696c 6520 2873 7472 2c20 6f70 7469 6f6e  ile (str, option
+00007550: 616c 293a 2054 6865 206c 6f67 2066 696c  al): The log fil
+00007560: 6520 6f66 2074 6865 2053 6c75 726d 206a  e of the Slurm j
+00007570: 6f62 2e20 0a20 2020 2020 2020 2020 2020  ob. .           
+00007580: 2020 2020 2049 6620 6e6f 7420 7072 6f76       If not prov
+00007590: 6964 6564 2c20 6120 6465 6661 756c 7420  ided, a default 
+000075a0: 6c6f 6720 6669 6c65 2077 696c 6c20 6265  log file will be
+000075b0: 2075 7365 642e 0a0a 2020 2020 2020 2020   used...        
+000075c0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+000075d0: 2020 2020 2052 6573 756c 743a 2054 6865       Result: The
+000075e0: 2072 6573 756c 7420 6f66 2074 6865 2063   result of the c
+000075f0: 6c65 616e 7570 206f 7065 7261 7469 6f6e  leanup operation
+00007600: 2e0a 0a20 2020 2020 2020 204e 6f74 653a  ...        Note:
+00007610: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00007620: 2063 6c65 616e 7570 2070 726f 6365 7373   cleanup process
+00007630: 2069 6e76 6f6c 7665 7320 7265 6d6f 7669   involves removi
+00007640: 6e67 2074 6865 2073 7065 6369 6669 6564  ng the specified
+00007650: 207a 6970 2066 696c 652c 200a 2020 2020   zip file, .    
+00007660: 2020 2020 2020 2020 7468 6520 6c6f 6720          the log 
+00007670: 6669 6c65 2c20 616e 6420 6173 736f 6369  file, and associ
+00007680: 6174 6564 2064 6174 6120 6669 6c65 7320  ated data files 
+00007690: 616e 6420 666f 6c64 6572 732e 0a0a 2020  and folders...  
+000076a0: 2020 2020 2020 4578 616d 706c 653a 0a20        Example:. 
+000076b0: 2020 2020 2020 2020 2020 2023 2043 6c65             # Cle
+000076c0: 616e 7570 2074 656d 706f 7261 7279 2066  anup temporary f
+000076d0: 696c 6573 2066 6f72 2061 2053 6c75 726d  iles for a Slurm
+000076e0: 206a 6f62 0a20 2020 2020 2020 2020 2020   job.           
+000076f0: 2063 6c69 656e 742e 636c 6561 6e75 705f   client.cleanup_
+00007700: 746d 705f 6669 6c65 7328 2231 3233 3435  tmp_files("12345
+00007710: 222c 2022 6f75 7470 7574 2e7a 6970 2229  ", "output.zip")
+00007720: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00007730: 2020 2020 2063 6d64 7320 3d20 5b5d 0a20       cmds = []. 
+00007740: 2020 2020 2020 2023 207a 6970 0a20 2020         # zip.   
+00007750: 2020 2020 2069 6620 6669 6c65 6e61 6d65       if filename
+00007760: 3a0a 2020 2020 2020 2020 2020 2020 726d  :.            rm
+00007770: 7a69 7020 3d20 6622 726d 205c 227b 6669  zip = f"rm \"{fi
+00007780: 6c65 6e61 6d65 7d5c 222e 2a22 0a20 2020  lename}\".*".   
+00007790: 2020 2020 2020 2020 2063 6d64 732e 6170           cmds.ap
+000077a0: 7065 6e64 2872 6d7a 6970 290a 2020 2020  pend(rmzip).    
+000077b0: 2020 2020 2320 6c6f 670a 2020 2020 2020      # log.      
+000077c0: 2020 6966 206c 6f67 6669 6c65 2069 7320    if logfile is 
+000077d0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+000077e0: 2020 6c6f 6766 696c 6520 3d20 7365 6c66    logfile = self
+000077f0: 2e5f 4c4f 4746 494c 450a 2020 2020 2020  ._LOGFILE.      
+00007800: 2020 2020 2020 6c6f 6766 696c 6520 3d20        logfile = 
+00007810: 6c6f 6766 696c 652e 666f 726d 6174 2873  logfile.format(s
+00007820: 6c75 726d 5f6a 6f62 5f69 643d 736c 7572  lurm_job_id=slur
+00007830: 6d5f 6a6f 625f 6964 290a 2020 2020 2020  m_job_id).      
+00007840: 2020 726d 6c6f 6720 3d20 6622 726d 205c    rmlog = f"rm \
+00007850: 227b 6c6f 6766 696c 657d 5c22 220a 2020  "{logfile}\"".  
+00007860: 2020 2020 2020 636d 6473 2e61 7070 656e        cmds.appen
+00007870: 6428 726d 6c6f 6729 0a20 2020 2020 2020  d(rmlog).       
+00007880: 2023 2063 6f6e 7665 7274 6572 206c 6f67   # converter log
+00007890: 730a 2020 2020 2020 2020 636c 6f67 203d  s.        clog =
+000078a0: 2073 656c 662e 5f43 4f4e 5645 5254 4552   self._CONVERTER
+000078b0: 5f4c 4f47 4649 4c45 0a20 2020 2020 2020  _LOGFILE.       
+000078c0: 2063 6c6f 6720 3d20 636c 6f67 2e66 6f72   clog = clog.for
+000078d0: 6d61 7428 736c 7572 6d5f 6a6f 625f 6964  mat(slurm_job_id
+000078e0: 3d73 6c75 726d 5f6a 6f62 5f69 6429 0a20  =slurm_job_id). 
+000078f0: 2020 2020 2020 2072 6d63 6c6f 6720 3d20         rmclog = 
+00007900: 6622 726d 207b 636c 6f67 7d22 0a20 2020  f"rm {clog}".   
+00007910: 2020 2020 2063 6d64 732e 6170 7065 6e64       cmds.append
+00007920: 2872 6d63 6c6f 6729 0a20 2020 2020 2020  (rmclog).       
+00007930: 200a 2020 2020 2020 2020 2320 6461 7461   .        # data
+00007940: 0a20 2020 2020 2020 2069 6620 6461 7461  .        if data
+00007950: 5f6c 6f63 6174 696f 6e20 6973 204e 6f6e  _location is Non
+00007960: 653a 0a20 2020 2020 2020 2020 2020 2064  e:.            d
+00007970: 6174 615f 6c6f 6361 7469 6f6e 203d 2073  ata_location = s
+00007980: 656c 662e 6578 7472 6163 745f 6461 7461  elf.extract_data
+00007990: 5f6c 6f63 6174 696f 6e5f 6672 6f6d 5f6c  _location_from_l
+000079a0: 6f67 286c 6f67 6669 6c65 290a 2020 2020  og(logfile).    
+000079b0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000079c0: 2069 6620 6461 7461 5f6c 6f63 6174 696f   if data_locatio
+000079d0: 6e3a 0a20 2020 2020 2020 2020 2020 2072  n:.            r
+000079e0: 6d64 6174 6120 3d20 6622 726d 202d 7266  mdata = f"rm -rf
+000079f0: 205c 227b 6461 7461 5f6c 6f63 6174 696f   \"{data_locatio
+00007a00: 6e7d 5c22 205c 227b 6461 7461 5f6c 6f63  n}\" \"{data_loc
+00007a10: 6174 696f 6e7d 5c22 2e2a 220a 2020 2020  ation}\".*".    
+00007a20: 2020 2020 2020 2020 636d 6473 2e61 7070          cmds.app
+00007a30: 656e 6428 726d 6461 7461 290a 2020 2020  end(rmdata).    
+00007a40: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+00007a50: 2020 2020 2023 2063 6f6e 7665 7274 2063       # convert c
+00007a60: 6f6e 6669 6720 6669 6c65 0a20 2020 2020  onfig file.     
+00007a70: 2020 2020 2020 2063 6f6e 6669 675f 6669         config_fi
+00007a80: 6c65 203d 2066 2263 6f6e 6669 675f 7b6f  le = f"config_{o
+00007a90: 732e 7061 7468 2e62 6173 656e 616d 6528  s.path.basename(
+00007aa0: 6461 7461 5f6c 6f63 6174 696f 6e29 7d2e  data_location)}.
+00007ab0: 7478 7422 0a20 2020 2020 2020 2020 2020  txt".           
+00007ac0: 2072 6d63 6f6e 6669 6720 3d20 6622 726d   rmconfig = f"rm
+00007ad0: 205c 227b 636f 6e66 6967 5f66 696c 657d   \"{config_file}
+00007ae0: 5c22 220a 2020 2020 2020 2020 2020 2020  \"".            
+00007af0: 636d 6473 2e61 7070 656e 6428 726d 636f  cmds.append(rmco
+00007b00: 6e66 6967 290a 2020 2020 2020 2020 656c  nfig).        el
+00007b10: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00007b20: 6c6f 6767 6572 2e77 6172 6e69 6e67 2866  logger.warning(f
+00007b30: 2243 6f75 6c64 206e 6f74 2065 7874 7261  "Could not extra
+00007b40: 6374 2064 6174 6120 6c6f 6361 7469 6f6e  ct data location
+00007b50: 2066 726f 6d20 6c6f 6720 7b6c 6f67 6669   from log {logfi
+00007b60: 6c65 7d2e 2053 6b69 7070 696e 6720 636c  le}. Skipping cl
+00007b70: 6561 6e75 702e 2229 0a0a 2020 2020 2020  eanup.")..      
+00007b80: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00007b90: 2020 2023 2064 6f20 6173 206d 7563 6820     # do as much 
+00007ba0: 6173 2070 6f73 7369 626c 652c 206e 6f74  as possible, not
+00007bb0: 2063 6f6e 6469 7469 6f6e 616c 2072 656d   conditional rem
+00007bc0: 6f76 616c 0a20 2020 2020 2020 2020 2020  oval.           
+00007bd0: 2072 6573 756c 7420 3d20 7365 6c66 2e72   result = self.r
+00007be0: 756e 5f63 6f6d 6d61 6e64 7328 636d 6473  un_commands(cmds
+00007bf0: 2c20 7365 703d 2720 3b20 2729 0a20 2020  , sep=' ; ').   
+00007c00: 2020 2020 2065 7863 6570 7420 556e 6578       except Unex
+00007c10: 7065 6374 6564 4578 6974 2061 7320 653a  pectedExit as e:
+00007c20: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+00007c30: 6765 722e 7761 726e 696e 6728 6529 0a20  ger.warning(e). 
+00007c40: 2020 2020 2020 2020 2020 2072 6573 756c             resul
+00007c50: 7420 3d20 652e 7265 7375 6c74 0a20 2020  t = e.result.   
+00007c60: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
+00007c70: 6c74 206f 7220 4e6f 6e65 0a0a 2020 2020  lt or None..    
+00007c80: 6465 6620 7661 6c69 6461 7465 2873 656c  def validate(sel
+00007c90: 662c 2076 616c 6964 6174 655f 736c 7572  f, validate_slur
+00007ca0: 6d5f 7365 7475 703a 2062 6f6f 6c20 3d20  m_setup: bool = 
+00007cb0: 4661 6c73 6529 3a0a 2020 2020 2020 2020  False):.        
+00007cc0: 2222 2256 616c 6964 6174 6520 7468 6520  """Validate the 
+00007cd0: 636f 6e6e 6563 7469 6f6e 2074 6f20 7468  connection to th
+00007ce0: 6520 536c 7572 6d20 636c 7573 7465 7220  e Slurm cluster 
+00007cf0: 6279 2072 756e 6e69 6e67 0a20 2020 2020  by running.     
+00007d00: 2020 2061 2073 696d 706c 6520 636f 6d6d     a simple comm
+00007d10: 616e 642e 0a0a 2020 2020 2020 2020 4172  and...        Ar
+00007d20: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00007d30: 7661 6c69 6461 7465 5f73 6c75 726d 5f73  validate_slurm_s
+00007d40: 6574 7570 2028 626f 6f6c 293a 2057 6865  etup (bool): Whe
+00007d50: 7468 6572 2074 6f20 616c 736f 2063 6865  ther to also che
+00007d60: 636b 0a20 2020 2020 2020 2020 2020 2020  ck.             
+00007d70: 2020 2061 6e64 2066 6978 2074 6865 2053     and fix the S
+00007d80: 6c75 726d 2073 6574 7570 2028 666f 6c64  lurm setup (fold
+00007d90: 6572 732c 2069 6d61 6765 732c 2065 7463  ers, images, etc
+00007da0: 2e29 0a0a 2020 2020 2020 2020 5265 7475  .)..        Retu
+00007db0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00007dc0: 2062 6f6f 6c3a 0a20 2020 2020 2020 2020   bool:.         
+00007dd0: 2020 2020 2020 2054 7275 6520 6966 2074         True if t
+00007de0: 6865 2076 616c 6964 6174 696f 6e20 6973  he validation is
+00007df0: 2073 7563 6365 7373 6675 6c2c 0a20 2020   successful,.   
+00007e00: 2020 2020 2020 2020 2020 2020 2046 616c               Fal
+00007e10: 7365 206f 7468 6572 7769 7365 2e0a 2020  se otherwise..  
+00007e20: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00007e30: 2020 636f 6e6e 6563 7465 6420 3d20 7365    connected = se
+00007e40: 6c66 2e72 756e 2827 6563 686f 2022 2022  lf.run('echo " "
+00007e50: 2729 2e6f 6b0a 2020 2020 2020 2020 6966  ').ok.        if
+00007e60: 2063 6f6e 6e65 6374 6564 2061 6e64 2076   connected and v
+00007e70: 616c 6964 6174 655f 736c 7572 6d5f 7365  alidate_slurm_se
+00007e80: 7475 703a 0a20 2020 2020 2020 2020 2020  tup:.           
+00007e90: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
+00007ea0: 2020 2020 2020 7365 6c66 2e73 6574 7570        self.setup
+00007eb0: 5f73 6c75 726d 2829 0a20 2020 2020 2020  _slurm().       
+00007ec0: 2020 2020 2065 7863 6570 7420 5353 4845       except SSHE
+00007ed0: 7863 6570 7469 6f6e 2061 7320 653a 0a20  xception as e:. 
+00007ee0: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00007ef0: 6f67 6765 722e 6572 726f 7228 6529 0a20  ogger.error(e). 
+00007f00: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00007f10: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
+00007f20: 2020 2020 7265 7475 726e 2063 6f6e 6e65      return conne
+00007f30: 6374 6564 0a0a 2020 2020 6465 6620 6765  cted..    def ge
+00007f40: 745f 7265 6365 6e74 5f6c 6f67 5f63 6f6d  t_recent_log_com
+00007f50: 6d61 6e64 2873 656c 662c 206c 6f67 5f66  mand(self, log_f
+00007f60: 696c 653a 2073 7472 2c20 6e3a 2069 6e74  ile: str, n: int
+00007f70: 203d 2031 3029 202d 3e20 7374 723a 0a20   = 10) -> str:. 
+00007f80: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00007f90: 2020 2047 6574 2074 6865 2063 6f6d 6d61     Get the comma
+00007fa0: 6e64 2074 6f20 7265 7472 6965 7665 2074  nd to retrieve t
+00007fb0: 6865 2072 6563 656e 7420 6c6f 6720 656e  he recent log en
+00007fc0: 7472 6965 7320 6672 6f6d 2061 0a20 2020  tries from a.   
+00007fd0: 2020 2020 2073 7065 6369 6669 6564 206c       specified l
+00007fe0: 6f67 2066 696c 652e 0a0a 2020 2020 2020  og file...      
+00007ff0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00008000: 2020 2020 6c6f 675f 6669 6c65 2028 7374      log_file (st
+00008010: 7229 3a20 5468 6520 7061 7468 2074 6f20  r): The path to 
+00008020: 7468 6520 6c6f 6720 6669 6c65 2e0a 2020  the log file..  
+00008030: 2020 2020 2020 2020 2020 6e20 2869 6e74            n (int
+00008040: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
+00008050: 206e 756d 6265 7220 6f66 2072 6563 656e   number of recen
+00008060: 7420 6c6f 6720 656e 7472 6965 7320 746f  t log entries to
+00008070: 2072 6574 7269 6576 652e 0a20 2020 2020   retrieve..     
+00008080: 2020 2020 2020 2020 2020 2044 6566 6175             Defau
+00008090: 6c74 7320 746f 2031 302e 0a0a 2020 2020  lts to 10...    
+000080a0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+000080b0: 2020 2020 2020 2020 2073 7472 3a20 5468           str: Th
+000080c0: 6520 636f 6d6d 616e 6420 746f 2072 6574  e command to ret
+000080d0: 7269 6576 6520 7468 6520 7265 6365 6e74  rieve the recent
+000080e0: 206c 6f67 2065 6e74 7269 6573 2e0a 2020   log entries..  
+000080f0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00008100: 2020 7265 7475 726e 2073 656c 662e 5f54    return self._T
+00008110: 4149 4c5f 4c4f 475f 434d 442e 666f 726d  AIL_LOG_CMD.form
+00008120: 6174 286e 3d6e 2c20 6c6f 675f 6669 6c65  at(n=n, log_file
+00008130: 3d6c 6f67 5f66 696c 6529 0a0a 2020 2020  =log_file)..    
+00008140: 6465 6620 6765 745f 6163 7469 7665 5f6a  def get_active_j
+00008150: 6f62 5f70 726f 6772 6573 7328 7365 6c66  ob_progress(self
+00008160: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00008170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008180: 2020 736c 7572 6d5f 6a6f 625f 6964 3a20    slurm_job_id: 
+00008190: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
 000081a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081b0: 2070 6174 7465 726e 3a20 7374 7220 3d20   pattern: str = 
-000081c0: 7222 5c64 2b25 222c 0a20 2020 2020 2020  r"\d+%",.       
+000081b0: 2020 2020 2070 6174 7465 726e 3a20 7374       pattern: st
+000081c0: 7220 3d20 7222 5c64 2b25 222c 0a20 2020  r = r"\d+%",.   
 000081d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000081e0: 2020 2020 2020 2020 2065 6e76 3a20 4f70           env: Op
-000081f0: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
-00008200: 2073 7472 5d5d 203d 204e 6f6e 6529 202d   str]] = None) -
-00008210: 3e20 7374 723a 0a20 2020 2020 2020 2022  > str:.        "
-00008220: 2222 0a20 2020 2020 2020 2047 6574 2074  "".        Get t
-00008230: 6865 2070 726f 6772 6573 7320 6f66 2061  he progress of a
-00008240: 6e20 6163 7469 7665 2053 6c75 726d 206a  n active Slurm j
-00008250: 6f62 2066 726f 6d20 6974 7320 6c6f 6766  ob from its logf
-00008260: 696c 6573 2e0a 0a20 2020 2020 2020 2041  iles...        A
-00008270: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00008280: 2073 6c75 726d 5f6a 6f62 5f69 6420 2873   slurm_job_id (s
-00008290: 7472 293a 2054 6865 2049 4420 6f66 2074  tr): The ID of t
-000082a0: 6865 2053 6c75 726d 206a 6f62 2e0a 2020  he Slurm job..  
-000082b0: 2020 2020 2020 2020 2020 7061 7474 6572            patter
-000082c0: 6e20 2873 7472 293a 2054 6865 2070 6174  n (str): The pat
-000082d0: 7465 726e 2074 6f20 6d61 7463 6820 696e  tern to match in
-000082e0: 2074 6865 206a 6f62 206c 6f67 2074 6f20   the job log to 
-000082f0: 6578 7472 6163 740a 2020 2020 2020 2020  extract.        
-00008300: 2020 2020 2020 2020 7468 6520 7072 6f67          the prog
-00008310: 7265 7373 2028 6465 6661 756c 743a 2072  ress (default: r
-00008320: 225c 642b 2522 292e 0a0a 2020 2020 2020  "\d+%")...      
-00008330: 2020 2020 2020 656e 7620 2844 6963 745b        env (Dict[
-00008340: 7374 722c 2073 7472 5d2c 206f 7074 696f  str, str], optio
-00008350: 6e61 6c29 3a20 4f70 7469 6f6e 616c 2065  nal): Optional e
-00008360: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-00008370: 626c 6573 200a 2020 2020 2020 2020 2020  bles .          
-00008380: 2020 2020 2020 746f 2073 6574 2077 6865        to set whe
-00008390: 6e20 7275 6e6e 696e 6720 7468 6520 636f  n running the co
-000083a0: 6d6d 616e 642e 2044 6566 6175 6c74 7320  mmand. Defaults 
-000083b0: 746f 204e 6f6e 652e 0a0a 2020 2020 2020  to None...      
-000083c0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-000083d0: 2020 2020 2020 2073 7472 3a20 5468 6520         str: The 
-000083e0: 7072 6f67 7265 7373 206f 6620 7468 6520  progress of the 
-000083f0: 536c 7572 6d20 6a6f 622e 0a20 2020 2020  Slurm job..     
-00008400: 2020 2022 2222 0a20 2020 2020 2020 2063     """.        c
-00008410: 6d64 6c69 7374 203d 205b 5d0a 2020 2020  mdlist = [].    
-00008420: 2020 2020 636d 6420 3d20 7365 6c66 2e67      cmd = self.g
-00008430: 6574 5f72 6563 656e 745f 6c6f 675f 636f  et_recent_log_co
-00008440: 6d6d 616e 6428 0a20 2020 2020 2020 2020  mmand(.         
-00008450: 2020 206c 6f67 5f66 696c 653d 7365 6c66     log_file=self
-00008460: 2e5f 4c4f 4746 494c 452e 666f 726d 6174  ._LOGFILE.format
-00008470: 2873 6c75 726d 5f6a 6f62 5f69 643d 736c  (slurm_job_id=sl
-00008480: 7572 6d5f 6a6f 625f 6964 2929 0a20 2020  urm_job_id)).   
-00008490: 2020 2020 2063 6d64 6c69 7374 2e61 7070       cmdlist.app
-000084a0: 656e 6428 636d 6429 0a20 2020 2020 2020  end(cmd).       
-000084b0: 2069 6620 656e 7620 6973 204e 6f6e 653a   if env is None:
-000084c0: 0a20 2020 2020 2020 2020 2020 2065 6e76  .            env
-000084d0: 203d 207b 7d0a 2020 2020 2020 2020 7472   = {}.        tr
-000084e0: 793a 0a20 2020 2020 2020 2020 2020 2072  y:.            r
-000084f0: 6573 756c 7420 3d20 7365 6c66 2e72 756e  esult = self.run
-00008500: 5f63 6f6d 6d61 6e64 7328 636d 646c 6973  _commands(cmdlis
-00008510: 742c 2065 6e76 3d65 6e76 290a 2020 2020  t, env=env).    
-00008520: 2020 2020 6578 6365 7074 2045 7863 6570      except Excep
-00008530: 7469 6f6e 2061 7320 653a 0a20 2020 2020  tion as e:.     
-00008540: 2020 2020 2020 206c 6f67 6765 722e 6572         logger.er
-00008550: 726f 7228 6622 4973 7375 6520 7769 7468  ror(f"Issue with
-00008560: 2072 756e 2063 6f6d 6d61 6e64 3a20 7b65   run command: {e
-00008570: 7d22 290a 2020 2020 2020 2020 2320 4d61  }").        # Ma
-00008580: 7463 6820 7468 6520 7370 6563 6966 6965  tch the specifie
-00008590: 6420 7061 7474 6572 6e20 696e 2074 6865  d pattern in the
-000085a0: 2072 6573 756c 7427 7320 7374 646f 7574   result's stdout
-000085b0: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
-000085c0: 2020 2020 2020 2020 2020 6c61 7465 7374            latest
-000085d0: 5f70 726f 6772 6573 7320 3d20 7265 2e66  _progress = re.f
-000085e0: 696e 6461 6c6c 280a 2020 2020 2020 2020  indall(.        
-000085f0: 2020 2020 2020 2020 7061 7474 6572 6e2c          pattern,
-00008600: 2072 6573 756c 742e 7374 646f 7574 295b   result.stdout)[
-00008610: 2d31 5d0a 2020 2020 2020 2020 6578 6365  -1].        exce
-00008620: 7074 2045 7863 6570 7469 6f6e 2061 7320  pt Exception as 
-00008630: 653a 0a20 2020 2020 2020 2020 2020 206c  e:.            l
-00008640: 6f67 6765 722e 6572 726f 7228 6622 4973  ogger.error(f"Is
-00008650: 7375 6520 7769 7468 2065 7874 7261 6374  sue with extract
-00008660: 696e 6720 7072 6f67 7265 7373 3a20 7b65  ing progress: {e
-00008670: 7d22 290a 0a20 2020 2020 2020 2072 6574  }")..        ret
-00008680: 7572 6e20 6622 5072 6f67 7265 7373 3a20  urn f"Progress: 
-00008690: 7b6c 6174 6573 745f 7072 6f67 7265 7373  {latest_progress
-000086a0: 7d5c 6e22 0a0a 2020 2020 6465 6620 7275  }\n"..    def ru
-000086b0: 6e5f 636f 6d6d 616e 6473 2873 656c 662c  n_commands(self,
-000086c0: 2063 6d64 6c69 7374 3a20 4c69 7374 5b73   cmdlist: List[s
-000086d0: 7472 5d2c 0a20 2020 2020 2020 2020 2020  tr],.           
-000086e0: 2020 2020 2020 2020 2020 656e 763a 204f            env: O
-000086f0: 7074 696f 6e61 6c5b 4469 6374 5b73 7472  ptional[Dict[str
-00008700: 2c20 7374 725d 5d20 3d20 4e6f 6e65 2c0a  , str]] = None,.
-00008710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008720: 2020 2020 2073 6570 3a20 7374 7220 3d20       sep: str = 
-00008730: 2720 2626 2027 2c0a 2020 2020 2020 2020  ' && ',.        
-00008740: 2020 2020 2020 2020 2020 2020 202a 2a6b               **k
-00008750: 7761 7267 7329 202d 3e20 5265 7375 6c74  wargs) -> Result
-00008760: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00008770: 2020 2020 2020 5275 6e20 6120 6c69 7374        Run a list
-00008780: 206f 6620 7368 656c 6c20 636f 6d6d 616e   of shell comman
-00008790: 6473 2063 6f6e 7365 6375 7469 7665 6c79  ds consecutively
-000087a0: 206f 6e20 7468 6520 536c 7572 6d20 636c   on the Slurm cl
-000087b0: 7573 7465 722c 0a20 2020 2020 2020 2065  uster,.        e
-000087c0: 6e73 7572 696e 6720 7468 6520 7375 6363  nsuring the succ
-000087d0: 6573 7320 6f66 2065 6163 6820 6265 666f  ess of each befo
-000087e0: 7265 2070 726f 6365 6564 696e 6720 746f  re proceeding to
-000087f0: 2074 6865 206e 6578 742e 0a0a 2020 2020   the next...    
-00008800: 2020 2020 5468 6520 656e 7669 726f 6e6d      The environm
-00008810: 656e 7420 7661 7269 6162 6c65 7320 6361  ent variables ca
-00008820: 6e20 6265 2073 6574 2075 7369 6e67 2074  n be set using t
-00008830: 6865 2060 656e 7660 2061 7267 756d 656e  he `env` argumen
-00008840: 742e 0a20 2020 2020 2020 2054 6865 7365  t..        These
-00008850: 2063 6f6d 6d61 6e64 7320 7265 7461 696e   commands retain
-00008860: 2074 6865 2073 616d 6520 7365 7373 696f   the same sessio
-00008870: 6e20 2865 6e76 6972 6f6e 6d65 6e74 2076  n (environment v
-00008880: 6172 6961 626c 6573 0a20 2020 2020 2020  ariables.       
-00008890: 2065 7463 2e29 2c20 756e 6c69 6b65 2072   etc.), unlike r
-000088a0: 756e 6e69 6e67 2074 6865 6d20 7365 7061  unning them sepa
-000088b0: 7261 7465 6c79 2e0a 0a20 2020 2020 2020  rately...       
-000088c0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-000088d0: 2020 2063 6d64 6c69 7374 2028 4c69 7374     cmdlist (List
-000088e0: 5b73 7472 5d29 3a20 4120 6c69 7374 206f  [str]): A list o
-000088f0: 6620 7368 656c 6c20 636f 6d6d 616e 6473  f shell commands
-00008900: 2074 6f20 7275 6e20 6f6e 2053 6c75 726d   to run on Slurm
-00008910: 2e0a 2020 2020 2020 2020 2020 2020 656e  ..            en
-00008920: 7620 2844 6963 745b 7374 722c 2073 7472  v (Dict[str, str
-00008930: 5d2c 206f 7074 696f 6e61 6c29 3a20 4f70  ], optional): Op
-00008940: 7469 6f6e 616c 2065 6e76 6972 6f6e 6d65  tional environme
-00008950: 6e74 2076 6172 6961 626c 6573 2074 6f0a  nt variables to.
-00008960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008970: 7365 7420 7768 656e 2072 756e 6e69 6e67  set when running
-00008980: 2074 6865 2063 6f6d 6d61 6e64 2e20 4465   the command. De
-00008990: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0a  faults to None..
-000089a0: 2020 2020 2020 2020 2020 2020 7365 7020              sep 
-000089b0: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
-000089c0: 2054 6865 2073 6570 6172 6174 6f72 2075   The separator u
-000089d0: 7365 6420 746f 2063 6f6e 6361 7465 6e61  sed to concatena
-000089e0: 7465 2074 6865 200a 2020 2020 2020 2020  te the .        
-000089f0: 2020 2020 2020 2020 636f 6d6d 616e 6473          commands
-00008a00: 2e20 4465 6661 756c 7473 2074 6f20 2720  . Defaults to ' 
-00008a10: 2626 2027 2e0a 2020 2020 2020 2020 2020  && '..          
-00008a20: 2020 2a2a 6b77 6172 6773 3a20 4164 6469    **kwargs: Addi
-00008a30: 7469 6f6e 616c 206b 6579 776f 7264 2061  tional keyword a
-00008a40: 7267 756d 656e 7473 2e0a 0a20 2020 2020  rguments...     
-00008a50: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00008a60: 2020 2020 2020 2020 5265 7375 6c74 3a20          Result: 
-00008a70: 5468 6520 7265 7375 6c74 206f 6620 7468  The result of th
-00008a80: 6520 6c61 7374 2063 6f6d 6d61 6e64 2069  e last command i
-00008a90: 6e20 7468 6520 6c69 7374 2e0a 2020 2020  n the list..    
-00008aa0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00008ab0: 6966 2065 6e76 2069 7320 4e6f 6e65 3a0a  if env is None:.
-00008ac0: 2020 2020 2020 2020 2020 2020 656e 7620              env 
-00008ad0: 3d20 7b7d 0a20 2020 2020 2020 2063 6d64  = {}.        cmd
-00008ae0: 203d 2073 6570 2e6a 6f69 6e28 636d 646c   = sep.join(cmdl
-00008af0: 6973 7429 0a20 2020 2020 2020 206c 6f67  ist).        log
-00008b00: 6765 722e 696e 666f 280a 2020 2020 2020  ger.info(.      
-00008b10: 2020 2020 2020 6622 5275 6e6e 696e 6720        f"Running 
-00008b20: 636f 6d6d 616e 6473 2c20 7769 7468 2065  commands, with e
-00008b30: 6e76 207b 656e 767d 2061 6e64 2073 6570  nv {env} and sep
-00008b40: 207b 7365 707d 205c 0a20 2020 2020 2020   {sep} \.       
-00008b50: 2020 2020 2020 2020 2061 6e64 207b 6b77           and {kw
-00008b60: 6172 6773 7d3a 207b 636d 647d 2229 0a20  args}: {cmd}"). 
-00008b70: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00008b80: 7365 6c66 2e72 756e 2863 6d64 2c20 656e  self.run(cmd, en
-00008b90: 763d 656e 762c 202a 2a6b 7761 7267 7329  v=env, **kwargs)
-00008ba0: 2020 2320 6f75 745f 7374 7265 616d 3d6f    # out_stream=o
-00008bb0: 7574 5f73 7472 6561 6d2c 0a0a 2020 2020  ut_stream,..    
-00008bc0: 2020 2020 7472 793a 0a20 2020 2020 2020      try:.       
-00008bd0: 2020 2020 2023 2057 6174 6368 206f 7574       # Watch out
-00008be0: 2066 6f72 2055 6e69 636f 6465 456e 636f   for UnicodeEnco
-00008bf0: 6465 4572 726f 7220 7768 656e 2079 6f75  deError when you
-00008c00: 2073 7472 2829 2074 6869 732e 0a20 2020   str() this..   
-00008c10: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
-00008c20: 696e 666f 2866 227b 7265 7375 6c74 2e73  info(f"{result.s
-00008c30: 7464 6f75 747d 2229 0a20 2020 2020 2020  tdout}").       
-00008c40: 2065 7863 6570 7420 556e 6963 6f64 6545   except UnicodeE
-00008c50: 6e63 6f64 6545 7272 6f72 2061 7320 653a  ncodeError as e:
-00008c60: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-00008c70: 6765 722e 6572 726f 7228 6622 556e 6963  ger.error(f"Unic
-00008c80: 6f64 6520 6572 726f 723a 207b 657d 2229  ode error: {e}")
-00008c90: 0a20 2020 2020 2020 2020 2020 2023 2054  .            # T
-00008ca0: 4f44 4f3a 204f 4e4c 5920 7374 646f 7574  ODO: ONLY stdout
-00008cb0: 2052 4543 4f44 4520 4e45 4544 4544 3f3f   RECODE NEEDED??
-00008cc0: 206f 7220 616c 736f 2065 7272 6f72 3f0a   or also error?.
-00008cd0: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-00008ce0: 6c74 2e73 7464 6f75 7420 3d20 7265 7375  lt.stdout = resu
-00008cf0: 6c74 2e73 7464 6f75 742e 656e 636f 6465  lt.stdout.encode
-00008d00: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00008d10: 2020 2775 7466 2d38 272c 2027 6967 6e6f    'utf-8', 'igno
-00008d20: 7265 2729 2e64 6563 6f64 6528 2775 7466  re').decode('utf
-00008d30: 2d38 2729 0a20 2020 2020 2020 2072 6574  -8').        ret
-00008d40: 7572 6e20 7265 7375 6c74 0a0a 2020 2020  urn result..    
-00008d50: 6465 6620 7374 725f 746f 5f63 6c61 7373  def str_to_class
-00008d60: 2873 656c 662c 206d 6f64 756c 655f 6e61  (self, module_na
-00008d70: 6d65 3a20 7374 722c 2063 6c61 7373 5f6e  me: str, class_n
-00008d80: 616d 653a 2073 7472 2c20 2a61 7267 732c  ame: str, *args,
-00008d90: 202a 2a6b 7761 7267 7329 3a0a 2020 2020   **kwargs):.    
-00008da0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00008db0: 5265 7475 726e 2061 2063 6c61 7373 2069  Return a class i
-00008dc0: 6e73 7461 6e63 6520 6672 6f6d 2061 2073  nstance from a s
-00008dd0: 7472 696e 6720 7265 6665 7265 6e63 652e  tring reference.
-00008de0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-00008df0: 2020 2020 2020 2020 2020 2020 6d6f 6475              modu
-00008e00: 6c65 5f6e 616d 6520 2873 7472 293a 2054  le_name (str): T
-00008e10: 6865 206e 616d 6520 6f66 2074 6865 206d  he name of the m
-00008e20: 6f64 756c 652e 0a20 2020 2020 2020 2020  odule..         
-00008e30: 2020 2063 6c61 7373 5f6e 616d 6520 2873     class_name (s
-00008e40: 7472 293a 2054 6865 206e 616d 6520 6f66  tr): The name of
-00008e50: 2074 6865 2063 6c61 7373 2e0a 2020 2020   the class..    
-00008e60: 2020 2020 2020 2020 2a61 7267 733a 2041          *args: A
-00008e70: 6464 6974 696f 6e61 6c20 706f 7369 7469  dditional positi
-00008e80: 6f6e 616c 2061 7267 756d 656e 7473 2066  onal arguments f
-00008e90: 6f72 2074 6865 2063 6c61 7373 2063 6f6e  or the class con
-00008ea0: 7374 7275 6374 6f72 2e0a 2020 2020 2020  structor..      
-00008eb0: 2020 2020 2020 2a2a 6b77 6172 6773 3a20        **kwargs: 
-00008ec0: 4164 6469 7469 6f6e 616c 206b 6579 776f  Additional keywo
-00008ed0: 7264 2061 7267 756d 656e 7473 2066 6f72  rd arguments for
-00008ee0: 2074 6865 2063 6c61 7373 2063 6f6e 7374   the class const
-00008ef0: 7275 6374 6f72 2e0a 0a20 2020 2020 2020  ructor...       
-00008f00: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00008f10: 2020 2020 2020 6f62 6a65 6374 3a20 416e        object: An
-00008f20: 2069 6e73 7461 6e63 6520 6f66 2074 6865   instance of the
-00008f30: 2073 7065 6369 6669 6564 2063 6c61 7373   specified class
-00008f40: 2c20 6f72 204e 6f6e 6520 6966 2074 6865  , or None if the
-00008f50: 2063 6c61 7373 206f 720a 2020 2020 2020   class or.      
-00008f60: 2020 2020 2020 2020 2020 6d6f 6475 6c65            module
-00008f70: 2064 6f65 7320 6e6f 7420 6578 6973 742e   does not exist.
-00008f80: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00008f90: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
-00008fa0: 2020 2020 2020 6d6f 6475 6c65 5f20 3d20        module_ = 
-00008fb0: 696d 706f 7274 6c69 622e 696d 706f 7274  importlib.import
-00008fc0: 5f6d 6f64 756c 6528 6d6f 6475 6c65 5f6e  _module(module_n
-00008fd0: 616d 6529 0a20 2020 2020 2020 2020 2020  ame).           
-00008fe0: 2074 7279 3a0a 2020 2020 2020 2020 2020   try:.          
-00008ff0: 2020 2020 2020 636c 6173 735f 203d 2067        class_ = g
-00009000: 6574 6174 7472 286d 6f64 756c 655f 2c20  etattr(module_, 
-00009010: 636c 6173 735f 6e61 6d65 2928 2a61 7267  class_name)(*arg
-00009020: 732c 202a 2a6b 7761 7267 7329 0a20 2020  s, **kwargs).   
-00009030: 2020 2020 2020 2020 2065 7863 6570 7420           except 
-00009040: 4174 7472 6962 7574 6545 7272 6f72 3a0a  AttributeError:.
-00009050: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009060: 6c6f 6767 6572 2e65 7272 6f72 2827 436c  logger.error('Cl
-00009070: 6173 7320 646f 6573 206e 6f74 2065 7869  ass does not exi
-00009080: 7374 2729 0a20 2020 2020 2020 2065 7863  st').        exc
-00009090: 6570 7420 496d 706f 7274 4572 726f 723a  ept ImportError:
-000090a0: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-000090b0: 6765 722e 6572 726f 7228 274d 6f64 756c  ger.error('Modul
-000090c0: 6520 646f 6573 206e 6f74 2065 7869 7374  e does not exist
-000090d0: 2729 0a20 2020 2020 2020 2072 6574 7572  ').        retur
-000090e0: 6e20 636c 6173 735f 206f 7220 4e6f 6e65  n class_ or None
-000090f0: 0a0a 2020 2020 6465 6620 7275 6e5f 636f  ..    def run_co
-00009100: 6d6d 616e 6473 5f73 706c 6974 5f6f 7574  mmands_split_out
-00009110: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
+000081e0: 2020 2020 2020 2020 2020 2020 2065 6e76               env
+000081f0: 3a20 4f70 7469 6f6e 616c 5b44 6963 745b  : Optional[Dict[
+00008200: 7374 722c 2073 7472 5d5d 203d 204e 6f6e  str, str]] = Non
+00008210: 6529 202d 3e20 7374 723a 0a20 2020 2020  e) -> str:.     
+00008220: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
+00008230: 6574 2074 6865 2070 726f 6772 6573 7320  et the progress 
+00008240: 6f66 2061 6e20 6163 7469 7665 2053 6c75  of an active Slu
+00008250: 726d 206a 6f62 2066 726f 6d20 6974 7320  rm job from its 
+00008260: 6c6f 6766 696c 6573 2e0a 0a20 2020 2020  logfiles...     
+00008270: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00008280: 2020 2020 2073 6c75 726d 5f6a 6f62 5f69       slurm_job_i
+00008290: 6420 2873 7472 293a 2054 6865 2049 4420  d (str): The ID 
+000082a0: 6f66 2074 6865 2053 6c75 726d 206a 6f62  of the Slurm job
+000082b0: 2e0a 2020 2020 2020 2020 2020 2020 7061  ..            pa
+000082c0: 7474 6572 6e20 2873 7472 293a 2054 6865  ttern (str): The
+000082d0: 2070 6174 7465 726e 2074 6f20 6d61 7463   pattern to matc
+000082e0: 6820 696e 2074 6865 206a 6f62 206c 6f67  h in the job log
+000082f0: 2074 6f20 6578 7472 6163 740a 2020 2020   to extract.    
+00008300: 2020 2020 2020 2020 2020 2020 7468 6520              the 
+00008310: 7072 6f67 7265 7373 2028 6465 6661 756c  progress (defaul
+00008320: 743a 2072 225c 642b 2522 292e 0a0a 2020  t: r"\d+%")...  
+00008330: 2020 2020 2020 2020 2020 656e 7620 2844            env (D
+00008340: 6963 745b 7374 722c 2073 7472 5d2c 206f  ict[str, str], o
+00008350: 7074 696f 6e61 6c29 3a20 4f70 7469 6f6e  ptional): Option
+00008360: 616c 2065 6e76 6972 6f6e 6d65 6e74 2076  al environment v
+00008370: 6172 6961 626c 6573 200a 2020 2020 2020  ariables .      
+00008380: 2020 2020 2020 2020 2020 746f 2073 6574            to set
+00008390: 2077 6865 6e20 7275 6e6e 696e 6720 7468   when running th
+000083a0: 6520 636f 6d6d 616e 642e 2044 6566 6175  e command. Defau
+000083b0: 6c74 7320 746f 204e 6f6e 652e 0a0a 2020  lts to None...  
+000083c0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+000083d0: 2020 2020 2020 2020 2020 2073 7472 3a20             str: 
+000083e0: 5468 6520 7072 6f67 7265 7373 206f 6620  The progress of 
+000083f0: 7468 6520 536c 7572 6d20 6a6f 622e 0a20  the Slurm job.. 
+00008400: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00008410: 2020 2063 6d64 6c69 7374 203d 205b 5d0a     cmdlist = [].
+00008420: 2020 2020 2020 2020 636d 6420 3d20 7365          cmd = se
+00008430: 6c66 2e67 6574 5f72 6563 656e 745f 6c6f  lf.get_recent_lo
+00008440: 675f 636f 6d6d 616e 6428 0a20 2020 2020  g_command(.     
+00008450: 2020 2020 2020 206c 6f67 5f66 696c 653d         log_file=
+00008460: 7365 6c66 2e5f 4c4f 4746 494c 452e 666f  self._LOGFILE.fo
+00008470: 726d 6174 2873 6c75 726d 5f6a 6f62 5f69  rmat(slurm_job_i
+00008480: 643d 736c 7572 6d5f 6a6f 625f 6964 2929  d=slurm_job_id))
+00008490: 0a20 2020 2020 2020 2063 6d64 6c69 7374  .        cmdlist
+000084a0: 2e61 7070 656e 6428 636d 6429 0a20 2020  .append(cmd).   
+000084b0: 2020 2020 2069 6620 656e 7620 6973 204e       if env is N
+000084c0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+000084d0: 2065 6e76 203d 207b 7d0a 2020 2020 2020   env = {}.      
+000084e0: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+000084f0: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
+00008500: 2e72 756e 5f63 6f6d 6d61 6e64 7328 636d  .run_commands(cm
+00008510: 646c 6973 742c 2065 6e76 3d65 6e76 290a  dlist, env=env).
+00008520: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+00008530: 7863 6570 7469 6f6e 2061 7320 653a 0a20  xception as e:. 
+00008540: 2020 2020 2020 2020 2020 206c 6f67 6765             logge
+00008550: 722e 6572 726f 7228 6622 4973 7375 6520  r.error(f"Issue 
+00008560: 7769 7468 2072 756e 2063 6f6d 6d61 6e64  with run command
+00008570: 3a20 7b65 7d22 290a 2020 2020 2020 2020  : {e}").        
+00008580: 2320 4d61 7463 6820 7468 6520 7370 6563  # Match the spec
+00008590: 6966 6965 6420 7061 7474 6572 6e20 696e  ified pattern in
+000085a0: 2074 6865 2072 6573 756c 7427 7320 7374   the result's st
+000085b0: 646f 7574 0a20 2020 2020 2020 2074 7279  dout.        try
+000085c0: 3a0a 2020 2020 2020 2020 2020 2020 6c61  :.            la
+000085d0: 7465 7374 5f70 726f 6772 6573 7320 3d20  test_progress = 
+000085e0: 7265 2e66 696e 6461 6c6c 280a 2020 2020  re.findall(.    
+000085f0: 2020 2020 2020 2020 2020 2020 7061 7474              patt
+00008600: 6572 6e2c 2072 6573 756c 742e 7374 646f  ern, result.stdo
+00008610: 7574 295b 2d31 5d0a 2020 2020 2020 2020  ut)[-1].        
+00008620: 6578 6365 7074 2045 7863 6570 7469 6f6e  except Exception
+00008630: 2061 7320 653a 0a20 2020 2020 2020 2020   as e:.         
+00008640: 2020 206c 6f67 6765 722e 6572 726f 7228     logger.error(
+00008650: 6622 4973 7375 6520 7769 7468 2065 7874  f"Issue with ext
+00008660: 7261 6374 696e 6720 7072 6f67 7265 7373  racting progress
+00008670: 3a20 7b65 7d22 290a 0a20 2020 2020 2020  : {e}")..       
+00008680: 2072 6574 7572 6e20 6622 5072 6f67 7265   return f"Progre
+00008690: 7373 3a20 7b6c 6174 6573 745f 7072 6f67  ss: {latest_prog
+000086a0: 7265 7373 7d5c 6e22 0a0a 2020 2020 6465  ress}\n"..    de
+000086b0: 6620 7275 6e5f 636f 6d6d 616e 6473 2873  f run_commands(s
+000086c0: 656c 662c 2063 6d64 6c69 7374 3a20 4c69  elf, cmdlist: Li
+000086d0: 7374 5b73 7472 5d2c 0a20 2020 2020 2020  st[str],.       
+000086e0: 2020 2020 2020 2020 2020 2020 2020 656e                en
+000086f0: 763a 204f 7074 696f 6e61 6c5b 4469 6374  v: Optional[Dict
+00008700: 5b73 7472 2c20 7374 725d 5d20 3d20 4e6f  [str, str]] = No
+00008710: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00008720: 2020 2020 2020 2020 2073 6570 3a20 7374           sep: st
+00008730: 7220 3d20 2720 2626 2027 2c0a 2020 2020  r = ' && ',.    
+00008740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008750: 202a 2a6b 7761 7267 7329 202d 3e20 5265   **kwargs) -> Re
+00008760: 7375 6c74 3a0a 2020 2020 2020 2020 2222  sult:.        ""
+00008770: 220a 2020 2020 2020 2020 5275 6e20 6120  ".        Run a 
+00008780: 6c69 7374 206f 6620 7368 656c 6c20 636f  list of shell co
+00008790: 6d6d 616e 6473 2063 6f6e 7365 6375 7469  mmands consecuti
+000087a0: 7665 6c79 206f 6e20 7468 6520 536c 7572  vely on the Slur
+000087b0: 6d20 636c 7573 7465 722c 0a20 2020 2020  m cluster,.     
+000087c0: 2020 2065 6e73 7572 696e 6720 7468 6520     ensuring the 
+000087d0: 7375 6363 6573 7320 6f66 2065 6163 6820  success of each 
+000087e0: 6265 666f 7265 2070 726f 6365 6564 696e  before proceedin
+000087f0: 6720 746f 2074 6865 206e 6578 742e 0a0a  g to the next...
+00008800: 2020 2020 2020 2020 5468 6520 656e 7669          The envi
+00008810: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
+00008820: 7320 6361 6e20 6265 2073 6574 2075 7369  s can be set usi
+00008830: 6e67 2074 6865 2060 656e 7660 2061 7267  ng the `env` arg
+00008840: 756d 656e 742e 0a20 2020 2020 2020 2054  ument..        T
+00008850: 6865 7365 2063 6f6d 6d61 6e64 7320 7265  hese commands re
+00008860: 7461 696e 2074 6865 2073 616d 6520 7365  tain the same se
+00008870: 7373 696f 6e20 2865 6e76 6972 6f6e 6d65  ssion (environme
+00008880: 6e74 2076 6172 6961 626c 6573 0a20 2020  nt variables.   
+00008890: 2020 2020 2065 7463 2e29 2c20 756e 6c69       etc.), unli
+000088a0: 6b65 2072 756e 6e69 6e67 2074 6865 6d20  ke running them 
+000088b0: 7365 7061 7261 7465 6c79 2e0a 0a20 2020  separately...   
+000088c0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+000088d0: 2020 2020 2020 2063 6d64 6c69 7374 2028         cmdlist (
+000088e0: 4c69 7374 5b73 7472 5d29 3a20 4120 6c69  List[str]): A li
+000088f0: 7374 206f 6620 7368 656c 6c20 636f 6d6d  st of shell comm
+00008900: 616e 6473 2074 6f20 7275 6e20 6f6e 2053  ands to run on S
+00008910: 6c75 726d 2e0a 2020 2020 2020 2020 2020  lurm..          
+00008920: 2020 656e 7620 2844 6963 745b 7374 722c    env (Dict[str,
+00008930: 2073 7472 5d2c 206f 7074 696f 6e61 6c29   str], optional)
+00008940: 3a20 4f70 7469 6f6e 616c 2065 6e76 6972  : Optional envir
+00008950: 6f6e 6d65 6e74 2076 6172 6961 626c 6573  onment variables
+00008960: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
+00008970: 2020 2020 7365 7420 7768 656e 2072 756e      set when run
+00008980: 6e69 6e67 2074 6865 2063 6f6d 6d61 6e64  ning the command
+00008990: 2e20 4465 6661 756c 7473 2074 6f20 4e6f  . Defaults to No
+000089a0: 6e65 2e0a 2020 2020 2020 2020 2020 2020  ne..            
+000089b0: 7365 7020 2873 7472 2c20 6f70 7469 6f6e  sep (str, option
+000089c0: 616c 293a 2054 6865 2073 6570 6172 6174  al): The separat
+000089d0: 6f72 2075 7365 6420 746f 2063 6f6e 6361  or used to conca
+000089e0: 7465 6e61 7465 2074 6865 200a 2020 2020  tenate the .    
+000089f0: 2020 2020 2020 2020 2020 2020 636f 6d6d              comm
+00008a00: 616e 6473 2e20 4465 6661 756c 7473 2074  ands. Defaults t
+00008a10: 6f20 2720 2626 2027 2e0a 2020 2020 2020  o ' && '..      
+00008a20: 2020 2020 2020 2a2a 6b77 6172 6773 3a20        **kwargs: 
+00008a30: 4164 6469 7469 6f6e 616c 206b 6579 776f  Additional keywo
+00008a40: 7264 2061 7267 756d 656e 7473 2e0a 0a20  rd arguments... 
+00008a50: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00008a60: 2020 2020 2020 2020 2020 2020 5265 7375              Resu
+00008a70: 6c74 3a20 5468 6520 7265 7375 6c74 206f  lt: The result o
+00008a80: 6620 7468 6520 6c61 7374 2063 6f6d 6d61  f the last comma
+00008a90: 6e64 2069 6e20 7468 6520 6c69 7374 2e0a  nd in the list..
+00008aa0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00008ab0: 2020 2020 6966 2065 6e76 2069 7320 4e6f      if env is No
+00008ac0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00008ad0: 656e 7620 3d20 7b7d 0a20 2020 2020 2020  env = {}.       
+00008ae0: 2063 6d64 203d 2073 6570 2e6a 6f69 6e28   cmd = sep.join(
+00008af0: 636d 646c 6973 7429 0a20 2020 2020 2020  cmdlist).       
+00008b00: 206c 6f67 6765 722e 696e 666f 280a 2020   logger.info(.  
+00008b10: 2020 2020 2020 2020 2020 6622 5275 6e6e            f"Runn
+00008b20: 696e 6720 636f 6d6d 616e 6473 2c20 7769  ing commands, wi
+00008b30: 7468 2065 6e76 207b 656e 767d 2061 6e64  th env {env} and
+00008b40: 2073 6570 207b 7365 707d 205c 0a20 2020   sep {sep} \.   
+00008b50: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+00008b60: 207b 6b77 6172 6773 7d3a 207b 636d 647d   {kwargs}: {cmd}
+00008b70: 2229 0a20 2020 2020 2020 2072 6573 756c  ").        resul
+00008b80: 7420 3d20 7365 6c66 2e72 756e 2863 6d64  t = self.run(cmd
+00008b90: 2c20 656e 763d 656e 762c 202a 2a6b 7761  , env=env, **kwa
+00008ba0: 7267 7329 2020 2320 6f75 745f 7374 7265  rgs)  # out_stre
+00008bb0: 616d 3d6f 7574 5f73 7472 6561 6d2c 0a0a  am=out_stream,..
+00008bc0: 2020 2020 2020 2020 7472 793a 0a20 2020          try:.   
+00008bd0: 2020 2020 2020 2020 2023 2057 6174 6368           # Watch
+00008be0: 206f 7574 2066 6f72 2055 6e69 636f 6465   out for Unicode
+00008bf0: 456e 636f 6465 4572 726f 7220 7768 656e  EncodeError when
+00008c00: 2079 6f75 2073 7472 2829 2074 6869 732e   you str() this.
+00008c10: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+00008c20: 6765 722e 696e 666f 2866 227b 7265 7375  ger.info(f"{resu
+00008c30: 6c74 2e73 7464 6f75 747d 2229 0a20 2020  lt.stdout}").   
+00008c40: 2020 2020 2065 7863 6570 7420 556e 6963       except Unic
+00008c50: 6f64 6545 6e63 6f64 6545 7272 6f72 2061  odeEncodeError a
+00008c60: 7320 653a 0a20 2020 2020 2020 2020 2020  s e:.           
+00008c70: 206c 6f67 6765 722e 6572 726f 7228 6622   logger.error(f"
+00008c80: 556e 6963 6f64 6520 6572 726f 723a 207b  Unicode error: {
+00008c90: 657d 2229 0a20 2020 2020 2020 2020 2020  e}").           
+00008ca0: 2023 2054 4f44 4f3a 204f 4e4c 5920 7374   # TODO: ONLY st
+00008cb0: 646f 7574 2052 4543 4f44 4520 4e45 4544  dout RECODE NEED
+00008cc0: 4544 3f3f 206f 7220 616c 736f 2065 7272  ED?? or also err
+00008cd0: 6f72 3f0a 2020 2020 2020 2020 2020 2020  or?.            
+00008ce0: 7265 7375 6c74 2e73 7464 6f75 7420 3d20  result.stdout = 
+00008cf0: 7265 7375 6c74 2e73 7464 6f75 742e 656e  result.stdout.en
+00008d00: 636f 6465 280a 2020 2020 2020 2020 2020  code(.          
+00008d10: 2020 2020 2020 2775 7466 2d38 272c 2027        'utf-8', '
+00008d20: 6967 6e6f 7265 2729 2e64 6563 6f64 6528  ignore').decode(
+00008d30: 2775 7466 2d38 2729 0a20 2020 2020 2020  'utf-8').       
+00008d40: 2072 6574 7572 6e20 7265 7375 6c74 0a0a   return result..
+00008d50: 2020 2020 6465 6620 7374 725f 746f 5f63      def str_to_c
+00008d60: 6c61 7373 2873 656c 662c 206d 6f64 756c  lass(self, modul
+00008d70: 655f 6e61 6d65 3a20 7374 722c 2063 6c61  e_name: str, cla
+00008d80: 7373 5f6e 616d 653a 2073 7472 2c20 2a61  ss_name: str, *a
+00008d90: 7267 732c 202a 2a6b 7761 7267 7329 3a0a  rgs, **kwargs):.
+00008da0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00008db0: 2020 2020 5265 7475 726e 2061 2063 6c61      Return a cla
+00008dc0: 7373 2069 6e73 7461 6e63 6520 6672 6f6d  ss instance from
+00008dd0: 2061 2073 7472 696e 6720 7265 6665 7265   a string refere
+00008de0: 6e63 652e 0a0a 2020 2020 2020 2020 4172  nce...        Ar
+00008df0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00008e00: 6d6f 6475 6c65 5f6e 616d 6520 2873 7472  module_name (str
+00008e10: 293a 2054 6865 206e 616d 6520 6f66 2074  ): The name of t
+00008e20: 6865 206d 6f64 756c 652e 0a20 2020 2020  he module..     
+00008e30: 2020 2020 2020 2063 6c61 7373 5f6e 616d         class_nam
+00008e40: 6520 2873 7472 293a 2054 6865 206e 616d  e (str): The nam
+00008e50: 6520 6f66 2074 6865 2063 6c61 7373 2e0a  e of the class..
+00008e60: 2020 2020 2020 2020 2020 2020 2a61 7267              *arg
+00008e70: 733a 2041 6464 6974 696f 6e61 6c20 706f  s: Additional po
+00008e80: 7369 7469 6f6e 616c 2061 7267 756d 656e  sitional argumen
+00008e90: 7473 2066 6f72 2074 6865 2063 6c61 7373  ts for the class
+00008ea0: 2063 6f6e 7374 7275 6374 6f72 2e0a 2020   constructor..  
+00008eb0: 2020 2020 2020 2020 2020 2a2a 6b77 6172            **kwar
+00008ec0: 6773 3a20 4164 6469 7469 6f6e 616c 206b  gs: Additional k
+00008ed0: 6579 776f 7264 2061 7267 756d 656e 7473  eyword arguments
+00008ee0: 2066 6f72 2074 6865 2063 6c61 7373 2063   for the class c
+00008ef0: 6f6e 7374 7275 6374 6f72 2e0a 0a20 2020  onstructor...   
+00008f00: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00008f10: 2020 2020 2020 2020 2020 6f62 6a65 6374            object
+00008f20: 3a20 416e 2069 6e73 7461 6e63 6520 6f66  : An instance of
+00008f30: 2074 6865 2073 7065 6369 6669 6564 2063   the specified c
+00008f40: 6c61 7373 2c20 6f72 204e 6f6e 6520 6966  lass, or None if
+00008f50: 2074 6865 2063 6c61 7373 206f 720a 2020   the class or.  
+00008f60: 2020 2020 2020 2020 2020 2020 2020 6d6f                mo
+00008f70: 6475 6c65 2064 6f65 7320 6e6f 7420 6578  dule does not ex
+00008f80: 6973 742e 0a20 2020 2020 2020 2022 2222  ist..        """
+00008f90: 0a20 2020 2020 2020 2074 7279 3a0a 2020  .        try:.  
+00008fa0: 2020 2020 2020 2020 2020 6d6f 6475 6c65            module
+00008fb0: 5f20 3d20 696d 706f 7274 6c69 622e 696d  _ = importlib.im
+00008fc0: 706f 7274 5f6d 6f64 756c 6528 6d6f 6475  port_module(modu
+00008fd0: 6c65 5f6e 616d 6529 0a20 2020 2020 2020  le_name).       
+00008fe0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+00008ff0: 2020 2020 2020 2020 2020 636c 6173 735f            class_
+00009000: 203d 2067 6574 6174 7472 286d 6f64 756c   = getattr(modul
+00009010: 655f 2c20 636c 6173 735f 6e61 6d65 2928  e_, class_name)(
+00009020: 2a61 7267 732c 202a 2a6b 7761 7267 7329  *args, **kwargs)
+00009030: 0a20 2020 2020 2020 2020 2020 2065 7863  .            exc
+00009040: 6570 7420 4174 7472 6962 7574 6545 7272  ept AttributeErr
+00009050: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+00009060: 2020 2020 6c6f 6767 6572 2e65 7272 6f72      logger.error
+00009070: 2827 436c 6173 7320 646f 6573 206e 6f74  ('Class does not
+00009080: 2065 7869 7374 2729 0a20 2020 2020 2020   exist').       
+00009090: 2065 7863 6570 7420 496d 706f 7274 4572   except ImportEr
+000090a0: 726f 723a 0a20 2020 2020 2020 2020 2020  ror:.           
+000090b0: 206c 6f67 6765 722e 6572 726f 7228 274d   logger.error('M
+000090c0: 6f64 756c 6520 646f 6573 206e 6f74 2065  odule does not e
+000090d0: 7869 7374 2729 0a20 2020 2020 2020 2072  xist').        r
+000090e0: 6574 7572 6e20 636c 6173 735f 206f 7220  eturn class_ or 
+000090f0: 4e6f 6e65 0a0a 2020 2020 6465 6620 7275  None..    def ru
+00009100: 6e5f 636f 6d6d 616e 6473 5f73 706c 6974  n_commands_split
+00009110: 5f6f 7574 2873 656c 662c 0a20 2020 2020  _out(self,.     
 00009120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009130: 2020 2020 2020 636d 646c 6973 743a 204c        cmdlist: L
-00009140: 6973 745b 7374 725d 2c0a 2020 2020 2020  ist[str],.      
+00009130: 2020 2020 2020 2020 2020 636d 646c 6973            cmdlis
+00009140: 743a 204c 6973 745b 7374 725d 2c0a 2020  t: List[str],.  
 00009150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009160: 2020 2020 2020 2020 2065 6e76 3a20 4f70           env: Op
-00009170: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
-00009180: 2073 7472 5d5d 203d 204e 6f6e 650a 2020   str]] = None.  
-00009190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000091a0: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
-000091b0: 3e20 4c69 7374 5b73 7472 5d3a 0a20 2020  > List[str]:.   
-000091c0: 2020 2020 2022 2222 5275 6e20 6120 6c69       """Run a li
-000091d0: 7374 206f 6620 7368 656c 6c20 636f 6d6d  st of shell comm
-000091e0: 616e 6473 2063 6f6e 7365 6375 7469 7665  ands consecutive
-000091f0: 6c79 2061 6e64 2073 706c 6974 2074 6865  ly and split the
-00009200: 206f 7574 7075 740a 2020 2020 2020 2020   output.        
-00009210: 6f66 2065 6163 6820 636f 6d6d 616e 642e  of each command.
-00009220: 0a0a 2020 2020 2020 2020 4561 6368 2063  ..        Each c
-00009230: 6f6d 6d61 6e64 2069 6e20 7468 6520 6c69  ommand in the li
-00009240: 7374 2069 7320 6578 6563 7574 6564 2077  st is executed w
-00009250: 6974 6820 6120 7365 7061 7261 746f 7220  ith a separator 
-00009260: 696e 2062 6574 7765 656e 0a20 2020 2020  in between.     
-00009270: 2020 2074 6861 7420 6973 2075 6e69 7175     that is uniqu
-00009280: 6520 616e 6420 6361 6e20 6265 2075 7365  e and can be use
-00009290: 6420 746f 2073 706c 6974 0a20 2020 2020  d to split.     
-000092a0: 2020 2074 6865 206f 7574 7075 7420 6f66     the output of
-000092b0: 2065 6163 6820 636f 6d6d 616e 6420 6c61   each command la
-000092c0: 7465 722e 2054 6865 2073 6570 6172 6174  ter. The separat
-000092d0: 6f72 2075 7365 6420 6973 2073 7065 6369  or used is speci
-000092e0: 6669 6564 0a20 2020 2020 2020 2062 7920  fied.        by 
-000092f0: 7468 6520 605f 4f55 545f 5345 5060 2061  the `_OUT_SEP` a
-00009300: 7474 7269 6275 7465 206f 6620 7468 650a  ttribute of the.
-00009310: 2020 2020 2020 2020 536c 7572 6d43 6c69          SlurmCli
-00009320: 656e 7420 696e 7374 616e 6365 2e0a 0a20  ent instance... 
-00009330: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-00009340: 2020 2020 2020 2020 2063 6d64 6c69 7374           cmdlist
-00009350: 2028 4c69 7374 5b73 7472 5d29 3a20 4120   (List[str]): A 
-00009360: 6c69 7374 206f 6620 7368 656c 6c20 636f  list of shell co
-00009370: 6d6d 616e 6473 2074 6f20 7275 6e2e 0a20  mmands to run.. 
-00009380: 2020 2020 2020 2020 2020 2065 6e76 2028             env (
-00009390: 4469 6374 5b73 7472 2c20 7374 725d 2c20  Dict[str, str], 
-000093a0: 6f70 7469 6f6e 616c 293a 204f 7074 696f  optional): Optio
-000093b0: 6e61 6c20 656e 7669 726f 6e6d 656e 7420  nal environment 
-000093c0: 7661 7269 6162 6c65 7320 0a20 2020 2020  variables .     
-000093d0: 2020 2020 2020 2020 2020 2074 6f20 7365             to se
-000093e0: 7420 7768 656e 2072 756e 6e69 6e67 2074  t when running t
-000093f0: 6865 2063 6f6d 6d61 6e64 2e20 4465 6661  he command. Defa
-00009400: 756c 7473 2074 6f20 4e6f 6e65 2e0a 0a20  ults to None... 
-00009410: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00009420: 2020 2020 2020 2020 2020 2020 4c69 7374              List
-00009430: 5b73 7472 5d3a 0a20 2020 2020 2020 2020  [str]:.         
-00009440: 2020 2020 2020 2041 206c 6973 7420 6f66         A list of
-00009450: 2073 7472 696e 6773 2c20 7768 6572 6520   strings, where 
-00009460: 6561 6368 2073 7472 696e 6720 636f 7272  each string corr
-00009470: 6573 706f 6e64 7320 746f 0a20 2020 2020  esponds to.     
-00009480: 2020 2020 2020 2020 2020 2074 6865 206f             the o
-00009490: 7574 7075 7420 6f66 2061 2073 696e 676c  utput of a singl
-000094a0: 6520 636f 6d6d 616e 6420 696e 2060 636d  e command in `cm
-000094b0: 646c 6973 7460 2073 706c 6974 0a20 2020  dlist` split.   
-000094c0: 2020 2020 2020 2020 2020 2020 2062 7920               by 
-000094d0: 7468 6520 7365 7061 7261 746f 7220 605f  the separator `_
-000094e0: 4f55 545f 5345 5060 2e0a 0a20 2020 2020  OUT_SEP`...     
-000094f0: 2020 2052 6169 7365 733a 0a20 2020 2020     Raises:.     
-00009500: 2020 2020 2020 2053 5348 4578 6365 7074         SSHExcept
-00009510: 696f 6e3a 2049 6620 616e 7920 6f66 2074  ion: If any of t
-00009520: 6865 2063 6f6d 6d61 6e64 7320 6661 696c  he commands fail
-00009530: 2074 6f20 6578 6563 7574 6520 7375 6363   to execute succ
-00009540: 6573 7366 756c 6c79 2e0a 2020 2020 2020  essfully..      
-00009550: 2020 2222 220a 2020 2020 2020 2020 7472    """.        tr
-00009560: 793a 0a20 2020 2020 2020 2020 2020 2072  y:.            r
-00009570: 6573 756c 7420 3d20 7365 6c66 2e72 756e  esult = self.run
-00009580: 5f63 6f6d 6d61 6e64 7328 636d 646c 6973  _commands(cmdlis
-00009590: 743d 636d 646c 6973 742c 0a20 2020 2020  t=cmdlist,.     
+00009160: 2020 2020 2020 2020 2020 2020 2065 6e76               env
+00009170: 3a20 4f70 7469 6f6e 616c 5b44 6963 745b  : Optional[Dict[
+00009180: 7374 722c 2073 7472 5d5d 203d 204e 6f6e  str, str]] = Non
+00009190: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+000091a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000091b0: 2029 202d 3e20 4c69 7374 5b73 7472 5d3a   ) -> List[str]:
+000091c0: 0a20 2020 2020 2020 2022 2222 5275 6e20  .        """Run 
+000091d0: 6120 6c69 7374 206f 6620 7368 656c 6c20  a list of shell 
+000091e0: 636f 6d6d 616e 6473 2063 6f6e 7365 6375  commands consecu
+000091f0: 7469 7665 6c79 2061 6e64 2073 706c 6974  tively and split
+00009200: 2074 6865 206f 7574 7075 740a 2020 2020   the output.    
+00009210: 2020 2020 6f66 2065 6163 6820 636f 6d6d      of each comm
+00009220: 616e 642e 0a0a 2020 2020 2020 2020 4561  and...        Ea
+00009230: 6368 2063 6f6d 6d61 6e64 2069 6e20 7468  ch command in th
+00009240: 6520 6c69 7374 2069 7320 6578 6563 7574  e list is execut
+00009250: 6564 2077 6974 6820 6120 7365 7061 7261  ed with a separa
+00009260: 746f 7220 696e 2062 6574 7765 656e 0a20  tor in between. 
+00009270: 2020 2020 2020 2074 6861 7420 6973 2075         that is u
+00009280: 6e69 7175 6520 616e 6420 6361 6e20 6265  nique and can be
+00009290: 2075 7365 6420 746f 2073 706c 6974 0a20   used to split. 
+000092a0: 2020 2020 2020 2074 6865 206f 7574 7075         the outpu
+000092b0: 7420 6f66 2065 6163 6820 636f 6d6d 616e  t of each comman
+000092c0: 6420 6c61 7465 722e 2054 6865 2073 6570  d later. The sep
+000092d0: 6172 6174 6f72 2075 7365 6420 6973 2073  arator used is s
+000092e0: 7065 6369 6669 6564 0a20 2020 2020 2020  pecified.       
+000092f0: 2062 7920 7468 6520 605f 4f55 545f 5345   by the `_OUT_SE
+00009300: 5060 2061 7474 7269 6275 7465 206f 6620  P` attribute of 
+00009310: 7468 650a 2020 2020 2020 2020 536c 7572  the.        Slur
+00009320: 6d43 6c69 656e 7420 696e 7374 616e 6365  mClient instance
+00009330: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00009340: 0a20 2020 2020 2020 2020 2020 2063 6d64  .            cmd
+00009350: 6c69 7374 2028 4c69 7374 5b73 7472 5d29  list (List[str])
+00009360: 3a20 4120 6c69 7374 206f 6620 7368 656c  : A list of shel
+00009370: 6c20 636f 6d6d 616e 6473 2074 6f20 7275  l commands to ru
+00009380: 6e2e 0a20 2020 2020 2020 2020 2020 2065  n..            e
+00009390: 6e76 2028 4469 6374 5b73 7472 2c20 7374  nv (Dict[str, st
+000093a0: 725d 2c20 6f70 7469 6f6e 616c 293a 204f  r], optional): O
+000093b0: 7074 696f 6e61 6c20 656e 7669 726f 6e6d  ptional environm
+000093c0: 656e 7420 7661 7269 6162 6c65 7320 0a20  ent variables . 
+000093d0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+000093e0: 6f20 7365 7420 7768 656e 2072 756e 6e69  o set when runni
+000093f0: 6e67 2074 6865 2063 6f6d 6d61 6e64 2e20  ng the command. 
+00009400: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
+00009410: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00009420: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00009430: 4c69 7374 5b73 7472 5d3a 0a20 2020 2020  List[str]:.     
+00009440: 2020 2020 2020 2020 2020 2041 206c 6973             A lis
+00009450: 7420 6f66 2073 7472 696e 6773 2c20 7768  t of strings, wh
+00009460: 6572 6520 6561 6368 2073 7472 696e 6720  ere each string 
+00009470: 636f 7272 6573 706f 6e64 7320 746f 0a20  corresponds to. 
+00009480: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00009490: 6865 206f 7574 7075 7420 6f66 2061 2073  he output of a s
+000094a0: 696e 676c 6520 636f 6d6d 616e 6420 696e  ingle command in
+000094b0: 2060 636d 646c 6973 7460 2073 706c 6974   `cmdlist` split
+000094c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000094d0: 2062 7920 7468 6520 7365 7061 7261 746f   by the separato
+000094e0: 7220 605f 4f55 545f 5345 5060 2e0a 0a20  r `_OUT_SEP`... 
+000094f0: 2020 2020 2020 2052 6169 7365 733a 0a20         Raises:. 
+00009500: 2020 2020 2020 2020 2020 2053 5348 4578             SSHEx
+00009510: 6365 7074 696f 6e3a 2049 6620 616e 7920  ception: If any 
+00009520: 6f66 2074 6865 2063 6f6d 6d61 6e64 7320  of the commands 
+00009530: 6661 696c 2074 6f20 6578 6563 7574 6520  fail to execute 
+00009540: 7375 6363 6573 7366 756c 6c79 2e0a 2020  successfully..  
+00009550: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00009560: 2020 7472 793a 0a20 2020 2020 2020 2020    try:.         
+00009570: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
+00009580: 2e72 756e 5f63 6f6d 6d61 6e64 7328 636d  .run_commands(cm
+00009590: 646c 6973 743d 636d 646c 6973 742c 0a20  dlist=cmdlist,. 
 000095a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000095b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095c0: 2020 656e 763d 656e 762c 0a20 2020 2020    env=env,.     
+000095c0: 2020 2020 2020 656e 763d 656e 762c 0a20        env=env,. 
 000095d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000095e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000095f0: 2020 7365 703d 6622 203b 2065 6368 6f20    sep=f" ; echo 
-00009600: 7b73 656c 662e 5f4f 5554 5f53 4550 7d20  {self._OUT_SEP} 
-00009610: 3b20 2229 0a20 2020 2020 2020 2065 7863  ; ").        exc
-00009620: 6570 7420 556e 6578 7065 6374 6564 4578  ept UnexpectedEx
-00009630: 6974 2061 7320 653a 0a20 2020 2020 2020  it as e:.       
-00009640: 2020 2020 206c 6f67 6765 722e 7761 726e       logger.warn
-00009650: 696e 6728 6529 0a20 2020 2020 2020 2020  ing(e).         
-00009660: 2020 2072 6573 756c 7420 3d20 652e 7265     result = e.re
-00009670: 7375 6c74 0a20 2020 2020 2020 2069 6620  sult.        if 
-00009680: 7265 7375 6c74 2e6f 6b3a 0a20 2020 2020  result.ok:.     
-00009690: 2020 2020 2020 2072 6573 706f 6e73 6520         response 
-000096a0: 3d20 7265 7375 6c74 2e73 7464 6f75 740a  = result.stdout.
-000096b0: 2020 2020 2020 2020 2020 2020 7370 6c69              spli
-000096c0: 745f 7265 7370 6f6e 7365 7320 3d20 7265  t_responses = re
-000096d0: 7370 6f6e 7365 2e73 706c 6974 2873 656c  sponse.split(sel
-000096e0: 662e 5f4f 5554 5f53 4550 290a 2020 2020  f._OUT_SEP).    
-000096f0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00009700: 706c 6974 5f72 6573 706f 6e73 6573 0a20  plit_responses. 
-00009710: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00009720: 2020 2020 2020 2020 2023 2049 6620 7468           # If th
-00009730: 6520 7265 7375 6c74 2069 7320 6e6f 7420  e result is not 
-00009740: 6f6b 2c20 6c6f 6720 7468 6520 6572 726f  ok, log the erro
-00009750: 7220 616e 6420 7261 6973 6520 616e 2053  r and raise an S
-00009760: 5348 4578 6365 7074 696f 6e0a 2020 2020  SHException.    
-00009770: 2020 2020 2020 2020 6572 726f 7220 3d20          error = 
-00009780: 6622 5265 7375 6c74 2069 7320 6e6f 7420  f"Result is not 
-00009790: 6f6b 3a20 7b72 6573 756c 747d 220a 2020  ok: {result}".  
-000097a0: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-000097b0: 2e65 7272 6f72 2865 7272 6f72 290a 2020  .error(error).  
-000097c0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000097d0: 5353 4845 7863 6570 7469 6f6e 2865 7272  SSHException(err
-000097e0: 6f72 290a 0a20 2020 2064 6566 206c 6973  or)..    def lis
-000097f0: 745f 6163 7469 7665 5f6a 6f62 7328 7365  t_active_jobs(se
-00009800: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
-00009810: 2020 2020 2020 2020 2020 2020 2065 6e76               env
-00009820: 3a20 4f70 7469 6f6e 616c 5b44 6963 745b  : Optional[Dict[
-00009830: 7374 722c 2073 7472 5d5d 203d 204e 6f6e  str, str]] = Non
-00009840: 6529 202d 3e20 4c69 7374 5b73 7472 5d3a  e) -> List[str]:
-00009850: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00009860: 2020 2020 2047 6574 2061 206c 6973 7420       Get a list 
-00009870: 6f66 2061 6374 6976 6520 6a6f 6273 2066  of active jobs f
-00009880: 726f 6d20 534c 5552 4d2e 0a0a 2020 2020  rom SLURM...    
-00009890: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-000098a0: 2020 2020 2020 656e 7620 2844 6963 745b        env (Dict[
-000098b0: 7374 722c 2073 7472 5d2c 206f 7074 696f  str, str], optio
-000098c0: 6e61 6c29 3a20 4f70 7469 6f6e 616c 2065  nal): Optional e
-000098d0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-000098e0: 626c 6573 2074 6f20 0a20 2020 2020 2020  bles to .       
-000098f0: 2020 2020 2020 2020 2073 6574 2077 6865           set whe
-00009900: 6e20 7275 6e6e 696e 6720 7468 6520 636f  n running the co
-00009910: 6d6d 616e 642e 2044 6566 6175 6c74 7320  mmand. Defaults 
-00009920: 746f 204e 6f6e 652e 0a0a 2020 2020 2020  to None...      
-00009930: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-00009940: 2020 2020 2020 204c 6973 745b 7374 725d         List[str]
-00009950: 3a20 4120 6c69 7374 206f 6620 6a6f 6220  : A list of job 
-00009960: 4944 732e 0a20 2020 2020 2020 2022 2222  IDs..        """
-00009970: 0a20 2020 2020 2020 2023 2063 6d64 203d  .        # cmd =
-00009980: 2073 656c 662e 5f41 4354 4956 455f 4a4f   self._ACTIVE_JO
-00009990: 4253 5f43 4d44 0a20 2020 2020 2020 2063  BS_CMD.        c
-000099a0: 6d64 203d 2073 656c 662e 6765 745f 6a6f  md = self.get_jo
-000099b0: 6273 5f69 6e66 6f5f 636f 6d6d 616e 6428  bs_info_command(
-000099c0: 7374 6172 745f 7469 6d65 3d22 6e6f 7722  start_time="now"
-000099d0: 2c20 7374 6174 6573 3d22 7222 290a 2020  , states="r").  
-000099e0: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
-000099f0: 6f28 2252 6574 7269 6576 696e 6720 6c69  o("Retrieving li
-00009a00: 7374 206f 6620 6163 7469 7665 206a 6f62  st of active job
-00009a10: 7320 6672 6f6d 2053 6c75 726d 2229 0a20  s from Slurm"). 
-00009a20: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-00009a30: 7365 6c66 2e72 756e 5f63 6f6d 6d61 6e64  self.run_command
-00009a40: 7328 5b63 6d64 5d2c 2065 6e76 3d65 6e76  s([cmd], env=env
-00009a50: 290a 2020 2020 2020 2020 6a6f 625f 6c69  ).        job_li
-00009a60: 7374 203d 2072 6573 756c 742e 7374 646f  st = result.stdo
-00009a70: 7574 2e73 7472 6970 2829 2e73 706c 6974  ut.strip().split
-00009a80: 2827 5c6e 2729 0a20 2020 2020 2020 206a  ('\n').        j
-00009a90: 6f62 5f6c 6973 742e 7265 7665 7273 6528  ob_list.reverse(
-00009aa0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00009ab0: 206a 6f62 5f6c 6973 740a 0a20 2020 2064   job_list..    d
-00009ac0: 6566 206c 6973 745f 636f 6d70 6c65 7465  ef list_complete
-00009ad0: 645f 6a6f 6273 2873 656c 662c 0a20 2020  d_jobs(self,.   
-00009ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009af0: 2020 2020 2020 2020 2065 6e76 3a20 4f70           env: Op
-00009b00: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
-00009b10: 2073 7472 5d5d 203d 204e 6f6e 6529 202d   str]] = None) -
-00009b20: 3e20 4c69 7374 5b73 7472 5d3a 0a20 2020  > List[str]:.   
-00009b30: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00009b40: 2047 6574 2061 206c 6973 7420 6f66 2063   Get a list of c
-00009b50: 6f6d 706c 6574 6564 206a 6f62 7320 6672  ompleted jobs fr
-00009b60: 6f6d 2053 4c55 524d 2e0a 0a20 2020 2020  om SLURM...     
-00009b70: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00009b80: 2020 2020 2065 6e76 2028 4469 6374 5b73       env (Dict[s
-00009b90: 7472 2c20 7374 725d 2c20 6f70 7469 6f6e  tr, str], option
-00009ba0: 616c 293a 204f 7074 696f 6e61 6c20 656e  al): Optional en
-00009bb0: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
-00009bc0: 6c65 7320 746f 0a20 2020 2020 2020 2020  les to.         
-00009bd0: 2020 2020 2020 2073 6574 2077 6865 6e20         set when 
-00009be0: 7275 6e6e 696e 6720 7468 6520 636f 6d6d  running the comm
-00009bf0: 616e 642e 2044 6566 6175 6c74 7320 746f  and. Defaults to
-00009c00: 204e 6f6e 652e 0a0a 2020 2020 2020 2020   None...        
-00009c10: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-00009c20: 2020 2020 204c 6973 745b 7374 725d 3a20       List[str]: 
-00009c30: 4120 6c69 7374 206f 6620 6a6f 6220 4944  A list of job ID
-00009c40: 732e 0a20 2020 2020 2020 2022 2222 0a0a  s..        """..
-00009c50: 2020 2020 2020 2020 636d 6420 3d20 7365          cmd = se
-00009c60: 6c66 2e67 6574 5f6a 6f62 735f 696e 666f  lf.get_jobs_info
-00009c70: 5f63 6f6d 6d61 6e64 2873 7461 7465 733d  _command(states=
-00009c80: 2263 6422 290a 2020 2020 2020 2020 6c6f  "cd").        lo
-00009c90: 6767 6572 2e69 6e66 6f28 2252 6574 7269  gger.info("Retri
-00009ca0: 6576 696e 6720 6120 6c69 7374 206f 6620  eving a list of 
-00009cb0: 636f 6d70 6c65 7465 6420 6a6f 6273 2066  completed jobs f
-00009cc0: 726f 6d20 536c 7572 6d22 290a 2020 2020  rom Slurm").    
-00009cd0: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
-00009ce0: 662e 7275 6e5f 636f 6d6d 616e 6473 285b  f.run_commands([
-00009cf0: 636d 645d 2c20 656e 763d 656e 7629 0a20  cmd], env=env). 
-00009d00: 2020 2020 2020 206a 6f62 5f6c 6973 7420         job_list 
-00009d10: 3d20 5b6a 6f62 2e73 7472 6970 2829 2066  = [job.strip() f
-00009d20: 6f72 206a 6f62 2069 6e20 7265 7375 6c74  or job in result
-00009d30: 2e73 7464 6f75 742e 7374 7269 7028 292e  .stdout.strip().
-00009d40: 7370 6c69 7428 275c 6e27 295d 0a20 2020  split('\n')].   
-00009d50: 2020 2020 206a 6f62 5f6c 6973 742e 7265       job_list.re
-00009d60: 7665 7273 6528 290a 2020 2020 2020 2020  verse().        
-00009d70: 7265 7475 726e 206a 6f62 5f6c 6973 740a  return job_list.
-00009d80: 0a20 2020 2064 6566 206c 6973 745f 616c  .    def list_al
-00009d90: 6c5f 6a6f 6273 2873 656c 662c 2065 6e76  l_jobs(self, env
-00009da0: 3a20 4f70 7469 6f6e 616c 5b44 6963 745b  : Optional[Dict[
-00009db0: 7374 722c 2073 7472 5d5d 203d 204e 6f6e  str, str]] = Non
-00009dc0: 6529 202d 3e20 4c69 7374 5b73 7472 5d3a  e) -> List[str]:
-00009dd0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00009de0: 2020 2020 2047 6574 2061 206c 6973 7420       Get a list 
-00009df0: 6f66 2061 6c6c 206a 6f62 7320 6672 6f6d  of all jobs from
-00009e00: 2053 4c55 524d 2e0a 0a20 2020 2020 2020   SLURM...       
-00009e10: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
-00009e20: 2020 2065 6e76 2028 4469 6374 5b73 7472     env (Dict[str
-00009e30: 2c20 7374 725d 2c20 6f70 7469 6f6e 616c  , str], optional
-00009e40: 293a 204f 7074 696f 6e61 6c20 656e 7669  ): Optional envi
-00009e50: 726f 6e6d 656e 7420 7661 7269 6162 6c65  ronment variable
-00009e60: 7320 0a20 2020 2020 2020 2020 2020 2020  s .             
-00009e70: 2020 2074 6f20 7365 7420 7768 656e 2072     to set when r
-00009e80: 756e 6e69 6e67 2074 6865 2063 6f6d 6d61  unning the comma
-00009e90: 6e64 2e20 4465 6661 756c 7473 2074 6f20  nd. Defaults to 
-00009ea0: 4e6f 6e65 2e0a 0a20 2020 2020 2020 2052  None...        R
-00009eb0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00009ec0: 2020 2020 4c69 7374 5b73 7472 5d3a 2041      List[str]: A
-00009ed0: 206c 6973 7420 6f66 206a 6f62 2049 4473   list of job IDs
-00009ee0: 2e0a 2020 2020 2020 2020 2222 220a 0a20  ..        """.. 
-00009ef0: 2020 2020 2020 2063 6d64 203d 2073 656c         cmd = sel
-00009f00: 662e 6765 745f 6a6f 6273 5f69 6e66 6f5f  f.get_jobs_info_
-00009f10: 636f 6d6d 616e 6428 290a 2020 2020 2020  command().      
-00009f20: 2020 6c6f 6767 6572 2e69 6e66 6f28 2252    logger.info("R
-00009f30: 6574 7269 6576 696e 6720 6120 6c69 7374  etrieving a list
-00009f40: 206f 6620 616c 6c20 6a6f 6273 2066 726f   of all jobs fro
-00009f50: 6d20 536c 7572 6d22 290a 2020 2020 2020  m Slurm").      
-00009f60: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
-00009f70: 7275 6e5f 636f 6d6d 616e 6473 285b 636d  run_commands([cm
-00009f80: 645d 2c20 656e 763d 656e 7629 0a20 2020  d], env=env).   
-00009f90: 2020 2020 206a 6f62 5f6c 6973 7420 3d20       job_list = 
-00009fa0: 7265 7375 6c74 2e73 7464 6f75 742e 7374  result.stdout.st
-00009fb0: 7269 7028 292e 7370 6c69 7428 275c 6e27  rip().split('\n'
-00009fc0: 290a 2020 2020 2020 2020 6a6f 625f 6c69  ).        job_li
-00009fd0: 7374 2e72 6576 6572 7365 2829 0a20 2020  st.reverse().   
-00009fe0: 2020 2020 2072 6574 7572 6e20 6a6f 625f       return job_
-00009ff0: 6c69 7374 0a0a 2020 2020 6465 6620 6765  list..    def ge
-0000a000: 745f 6a6f 6273 5f69 6e66 6f5f 636f 6d6d  t_jobs_info_comm
-0000a010: 616e 6428 7365 6c66 2c20 7374 6172 745f  and(self, start_
-0000a020: 7469 6d65 3a20 7374 7220 3d20 2232 3032  time: str = "202
-0000a030: 332d 3031 2d30 3122 2c0a 2020 2020 2020  3-01-01",.      
+000095f0: 2020 2020 2020 7365 703d 6622 203b 2065        sep=f" ; e
+00009600: 6368 6f20 7b73 656c 662e 5f4f 5554 5f53  cho {self._OUT_S
+00009610: 4550 7d20 3b20 2229 0a20 2020 2020 2020  EP} ; ").       
+00009620: 2065 7863 6570 7420 556e 6578 7065 6374   except Unexpect
+00009630: 6564 4578 6974 2061 7320 653a 0a20 2020  edExit as e:.   
+00009640: 2020 2020 2020 2020 206c 6f67 6765 722e           logger.
+00009650: 7761 726e 696e 6728 6529 0a20 2020 2020  warning(e).     
+00009660: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
+00009670: 652e 7265 7375 6c74 0a20 2020 2020 2020  e.result.       
+00009680: 2069 6620 7265 7375 6c74 2e6f 6b3a 0a20   if result.ok:. 
+00009690: 2020 2020 2020 2020 2020 2072 6573 706f             respo
+000096a0: 6e73 6520 3d20 7265 7375 6c74 2e73 7464  nse = result.std
+000096b0: 6f75 740a 2020 2020 2020 2020 2020 2020  out.            
+000096c0: 7370 6c69 745f 7265 7370 6f6e 7365 7320  split_responses 
+000096d0: 3d20 7265 7370 6f6e 7365 2e73 706c 6974  = response.split
+000096e0: 2873 656c 662e 5f4f 5554 5f53 4550 290a  (self._OUT_SEP).
+000096f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00009700: 726e 2073 706c 6974 5f72 6573 706f 6e73  rn split_respons
+00009710: 6573 0a20 2020 2020 2020 2065 6c73 653a  es.        else:
+00009720: 0a20 2020 2020 2020 2020 2020 2023 2049  .            # I
+00009730: 6620 7468 6520 7265 7375 6c74 2069 7320  f the result is 
+00009740: 6e6f 7420 6f6b 2c20 6c6f 6720 7468 6520  not ok, log the 
+00009750: 6572 726f 7220 616e 6420 7261 6973 6520  error and raise 
+00009760: 616e 2053 5348 4578 6365 7074 696f 6e0a  an SSHException.
+00009770: 2020 2020 2020 2020 2020 2020 6572 726f              erro
+00009780: 7220 3d20 6622 5265 7375 6c74 2069 7320  r = f"Result is 
+00009790: 6e6f 7420 6f6b 3a20 7b72 6573 756c 747d  not ok: {result}
+000097a0: 220a 2020 2020 2020 2020 2020 2020 6c6f  ".            lo
+000097b0: 6767 6572 2e65 7272 6f72 2865 7272 6f72  gger.error(error
+000097c0: 290a 2020 2020 2020 2020 2020 2020 7261  ).            ra
+000097d0: 6973 6520 5353 4845 7863 6570 7469 6f6e  ise SSHException
+000097e0: 2865 7272 6f72 290a 0a20 2020 2064 6566  (error)..    def
+000097f0: 206c 6973 745f 6163 7469 7665 5f6a 6f62   list_active_job
+00009800: 7328 7365 6c66 2c0a 2020 2020 2020 2020  s(self,.        
+00009810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009820: 2065 6e76 3a20 4f70 7469 6f6e 616c 5b44   env: Optional[D
+00009830: 6963 745b 7374 722c 2073 7472 5d5d 203d  ict[str, str]] =
+00009840: 204e 6f6e 6529 202d 3e20 4c69 7374 5b73   None) -> List[s
+00009850: 7472 5d3a 0a20 2020 2020 2020 2022 2222  tr]:.        """
+00009860: 0a20 2020 2020 2020 2047 6574 2061 206c  .        Get a l
+00009870: 6973 7420 6f66 2061 6374 6976 6520 6a6f  ist of active jo
+00009880: 6273 2066 726f 6d20 534c 5552 4d2e 0a0a  bs from SLURM...
+00009890: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+000098a0: 2020 2020 2020 2020 2020 656e 7620 2844            env (D
+000098b0: 6963 745b 7374 722c 2073 7472 5d2c 206f  ict[str, str], o
+000098c0: 7074 696f 6e61 6c29 3a20 4f70 7469 6f6e  ptional): Option
+000098d0: 616c 2065 6e76 6972 6f6e 6d65 6e74 2076  al environment v
+000098e0: 6172 6961 626c 6573 2074 6f20 0a20 2020  ariables to .   
+000098f0: 2020 2020 2020 2020 2020 2020 2073 6574               set
+00009900: 2077 6865 6e20 7275 6e6e 696e 6720 7468   when running th
+00009910: 6520 636f 6d6d 616e 642e 2044 6566 6175  e command. Defau
+00009920: 6c74 7320 746f 204e 6f6e 652e 0a0a 2020  lts to None...  
+00009930: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00009940: 2020 2020 2020 2020 2020 204c 6973 745b             List[
+00009950: 7374 725d 3a20 4120 6c69 7374 206f 6620  str]: A list of 
+00009960: 6a6f 6220 4944 732e 0a20 2020 2020 2020  job IDs..       
+00009970: 2022 2222 0a20 2020 2020 2020 2023 2063   """.        # c
+00009980: 6d64 203d 2073 656c 662e 5f41 4354 4956  md = self._ACTIV
+00009990: 455f 4a4f 4253 5f43 4d44 0a20 2020 2020  E_JOBS_CMD.     
+000099a0: 2020 2063 6d64 203d 2073 656c 662e 6765     cmd = self.ge
+000099b0: 745f 6a6f 6273 5f69 6e66 6f5f 636f 6d6d  t_jobs_info_comm
+000099c0: 616e 6428 7374 6172 745f 7469 6d65 3d22  and(start_time="
+000099d0: 6e6f 7722 2c20 7374 6174 6573 3d22 7222  now", states="r"
+000099e0: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
+000099f0: 2e69 6e66 6f28 2252 6574 7269 6576 696e  .info("Retrievin
+00009a00: 6720 6c69 7374 206f 6620 6163 7469 7665  g list of active
+00009a10: 206a 6f62 7320 6672 6f6d 2053 6c75 726d   jobs from Slurm
+00009a20: 2229 0a20 2020 2020 2020 2072 6573 756c  ").        resul
+00009a30: 7420 3d20 7365 6c66 2e72 756e 5f63 6f6d  t = self.run_com
+00009a40: 6d61 6e64 7328 5b63 6d64 5d2c 2065 6e76  mands([cmd], env
+00009a50: 3d65 6e76 290a 2020 2020 2020 2020 6a6f  =env).        jo
+00009a60: 625f 6c69 7374 203d 2072 6573 756c 742e  b_list = result.
+00009a70: 7374 646f 7574 2e73 7472 6970 2829 2e73  stdout.strip().s
+00009a80: 706c 6974 2827 5c6e 2729 0a20 2020 2020  plit('\n').     
+00009a90: 2020 206a 6f62 5f6c 6973 742e 7265 7665     job_list.reve
+00009aa0: 7273 6528 290a 2020 2020 2020 2020 7265  rse().        re
+00009ab0: 7475 726e 206a 6f62 5f6c 6973 740a 0a20  turn job_list.. 
+00009ac0: 2020 2064 6566 206c 6973 745f 636f 6d70     def list_comp
+00009ad0: 6c65 7465 645f 6a6f 6273 2873 656c 662c  leted_jobs(self,
+00009ae0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00009af0: 2020 2020 2020 2020 2020 2020 2065 6e76               env
+00009b00: 3a20 4f70 7469 6f6e 616c 5b44 6963 745b  : Optional[Dict[
+00009b10: 7374 722c 2073 7472 5d5d 203d 204e 6f6e  str, str]] = Non
+00009b20: 6529 202d 3e20 4c69 7374 5b73 7472 5d3a  e) -> List[str]:
+00009b30: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00009b40: 2020 2020 2047 6574 2061 206c 6973 7420       Get a list 
+00009b50: 6f66 2063 6f6d 706c 6574 6564 206a 6f62  of completed job
+00009b60: 7320 6672 6f6d 2053 4c55 524d 2e0a 0a20  s from SLURM... 
+00009b70: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00009b80: 2020 2020 2020 2020 2065 6e76 2028 4469           env (Di
+00009b90: 6374 5b73 7472 2c20 7374 725d 2c20 6f70  ct[str, str], op
+00009ba0: 7469 6f6e 616c 293a 204f 7074 696f 6e61  tional): Optiona
+00009bb0: 6c20 656e 7669 726f 6e6d 656e 7420 7661  l environment va
+00009bc0: 7269 6162 6c65 7320 746f 0a20 2020 2020  riables to.     
+00009bd0: 2020 2020 2020 2020 2020 2073 6574 2077             set w
+00009be0: 6865 6e20 7275 6e6e 696e 6720 7468 6520  hen running the 
+00009bf0: 636f 6d6d 616e 642e 2044 6566 6175 6c74  command. Default
+00009c00: 7320 746f 204e 6f6e 652e 0a0a 2020 2020  s to None...    
+00009c10: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00009c20: 2020 2020 2020 2020 204c 6973 745b 7374           List[st
+00009c30: 725d 3a20 4120 6c69 7374 206f 6620 6a6f  r]: A list of jo
+00009c40: 6220 4944 732e 0a20 2020 2020 2020 2022  b IDs..        "
+00009c50: 2222 0a0a 2020 2020 2020 2020 636d 6420  ""..        cmd 
+00009c60: 3d20 7365 6c66 2e67 6574 5f6a 6f62 735f  = self.get_jobs_
+00009c70: 696e 666f 5f63 6f6d 6d61 6e64 2873 7461  info_command(sta
+00009c80: 7465 733d 2263 6422 290a 2020 2020 2020  tes="cd").      
+00009c90: 2020 6c6f 6767 6572 2e69 6e66 6f28 2252    logger.info("R
+00009ca0: 6574 7269 6576 696e 6720 6120 6c69 7374  etrieving a list
+00009cb0: 206f 6620 636f 6d70 6c65 7465 6420 6a6f   of completed jo
+00009cc0: 6273 2066 726f 6d20 536c 7572 6d22 290a  bs from Slurm").
+00009cd0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+00009ce0: 2073 656c 662e 7275 6e5f 636f 6d6d 616e   self.run_comman
+00009cf0: 6473 285b 636d 645d 2c20 656e 763d 656e  ds([cmd], env=en
+00009d00: 7629 0a20 2020 2020 2020 206a 6f62 5f6c  v).        job_l
+00009d10: 6973 7420 3d20 5b6a 6f62 2e73 7472 6970  ist = [job.strip
+00009d20: 2829 2066 6f72 206a 6f62 2069 6e20 7265  () for job in re
+00009d30: 7375 6c74 2e73 7464 6f75 742e 7374 7269  sult.stdout.stri
+00009d40: 7028 292e 7370 6c69 7428 275c 6e27 295d  p().split('\n')]
+00009d50: 0a20 2020 2020 2020 206a 6f62 5f6c 6973  .        job_lis
+00009d60: 742e 7265 7665 7273 6528 290a 2020 2020  t.reverse().    
+00009d70: 2020 2020 7265 7475 726e 206a 6f62 5f6c      return job_l
+00009d80: 6973 740a 0a20 2020 2064 6566 206c 6973  ist..    def lis
+00009d90: 745f 616c 6c5f 6a6f 6273 2873 656c 662c  t_all_jobs(self,
+00009da0: 2065 6e76 3a20 4f70 7469 6f6e 616c 5b44   env: Optional[D
+00009db0: 6963 745b 7374 722c 2073 7472 5d5d 203d  ict[str, str]] =
+00009dc0: 204e 6f6e 6529 202d 3e20 4c69 7374 5b73   None) -> List[s
+00009dd0: 7472 5d3a 0a20 2020 2020 2020 2022 2222  tr]:.        """
+00009de0: 0a20 2020 2020 2020 2047 6574 2061 206c  .        Get a l
+00009df0: 6973 7420 6f66 2061 6c6c 206a 6f62 7320  ist of all jobs 
+00009e00: 6672 6f6d 2053 4c55 524d 2e0a 0a20 2020  from SLURM...   
+00009e10: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+00009e20: 2020 2020 2020 2065 6e76 2028 4469 6374         env (Dict
+00009e30: 5b73 7472 2c20 7374 725d 2c20 6f70 7469  [str, str], opti
+00009e40: 6f6e 616c 293a 204f 7074 696f 6e61 6c20  onal): Optional 
+00009e50: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
+00009e60: 6162 6c65 7320 0a20 2020 2020 2020 2020  ables .         
+00009e70: 2020 2020 2020 2074 6f20 7365 7420 7768         to set wh
+00009e80: 656e 2072 756e 6e69 6e67 2074 6865 2063  en running the c
+00009e90: 6f6d 6d61 6e64 2e20 4465 6661 756c 7473  ommand. Defaults
+00009ea0: 2074 6f20 4e6f 6e65 2e0a 0a20 2020 2020   to None...     
+00009eb0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00009ec0: 2020 2020 2020 2020 4c69 7374 5b73 7472          List[str
+00009ed0: 5d3a 2041 206c 6973 7420 6f66 206a 6f62  ]: A list of job
+00009ee0: 2049 4473 2e0a 2020 2020 2020 2020 2222   IDs..        ""
+00009ef0: 220a 0a20 2020 2020 2020 2063 6d64 203d  "..        cmd =
+00009f00: 2073 656c 662e 6765 745f 6a6f 6273 5f69   self.get_jobs_i
+00009f10: 6e66 6f5f 636f 6d6d 616e 6428 290a 2020  nfo_command().  
+00009f20: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
+00009f30: 6f28 2252 6574 7269 6576 696e 6720 6120  o("Retrieving a 
+00009f40: 6c69 7374 206f 6620 616c 6c20 6a6f 6273  list of all jobs
+00009f50: 2066 726f 6d20 536c 7572 6d22 290a 2020   from Slurm").  
+00009f60: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+00009f70: 656c 662e 7275 6e5f 636f 6d6d 616e 6473  elf.run_commands
+00009f80: 285b 636d 645d 2c20 656e 763d 656e 7629  ([cmd], env=env)
+00009f90: 0a20 2020 2020 2020 206a 6f62 5f6c 6973  .        job_lis
+00009fa0: 7420 3d20 7265 7375 6c74 2e73 7464 6f75  t = result.stdou
+00009fb0: 742e 7374 7269 7028 292e 7370 6c69 7428  t.strip().split(
+00009fc0: 275c 6e27 290a 2020 2020 2020 2020 6a6f  '\n').        jo
+00009fd0: 625f 6c69 7374 2e72 6576 6572 7365 2829  b_list.reverse()
+00009fe0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00009ff0: 6a6f 625f 6c69 7374 0a0a 2020 2020 6465  job_list..    de
+0000a000: 6620 6765 745f 6a6f 6273 5f69 6e66 6f5f  f get_jobs_info_
+0000a010: 636f 6d6d 616e 6428 7365 6c66 2c20 7374  command(self, st
+0000a020: 6172 745f 7469 6d65 3a20 7374 7220 3d20  art_time: str = 
+0000a030: 2232 3032 332d 3031 2d30 3122 2c0a 2020  "2023-01-01",.  
 0000a040: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a050: 2020 2020 2020 2020 656e 645f 7469 6d65          end_time
-0000a060: 3a20 7374 7220 3d20 226e 6f77 222c 0a20  : str = "now",. 
-0000a070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a080: 2020 2020 2020 2020 2020 2020 2063 6f6c               col
-0000a090: 756d 6e73 3a20 7374 7220 3d20 224a 6f62  umns: str = "Job
-0000a0a0: 4964 222c 0a20 2020 2020 2020 2020 2020  Id",.           
+0000a050: 2020 2020 2020 2020 2020 2020 656e 645f              end_
+0000a060: 7469 6d65 3a20 7374 7220 3d20 226e 6f77  time: str = "now
+0000a070: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+0000a080: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a090: 2063 6f6c 756d 6e73 3a20 7374 7220 3d20   columns: str = 
+0000a0a0: 224a 6f62 4964 222c 0a20 2020 2020 2020  "JobId",.       
 0000a0b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a0c0: 2020 2073 7461 7465 733a 2073 7472 203d     states: str =
-0000a0d0: 2022 722c 6364 2c66 2c74 6f2c 7273 2c64   "r,cd,f,to,rs,d
-0000a0e0: 6c2c 6e66 2229 202d 3e20 7374 723a 0a20  l,nf") -> str:. 
-0000a0f0: 2020 2020 2020 2022 2222 5265 7475 726e         """Return
-0000a100: 2074 6865 2053 6c75 726d 2063 6f6d 6d61   the Slurm comma
-0000a110: 6e64 2074 6f20 7265 7472 6965 7665 2069  nd to retrieve i
-0000a120: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
-0000a130: 206f 6c64 206a 6f62 732e 0a0a 2020 2020   old jobs...    
-0000a140: 2020 2020 5468 6520 636f 6d6d 616e 6420      The command 
-0000a150: 7769 6c6c 2062 6520 666f 726d 6174 7465  will be formatte
-0000a160: 6420 7769 7468 2074 6865 2073 7065 6369  d with the speci
-0000a170: 6669 6564 2073 7461 7274 2074 696d 652c  fied start time,
-0000a180: 2077 6869 6368 2069 730a 2020 2020 2020   which is.      
-0000a190: 2020 6578 7065 6374 6564 2074 6f20 6265    expected to be
-0000a1a0: 2069 6e20 7468 6520 4953 4f20 666f 726d   in the ISO form
-0000a1b0: 6174 2022 5959 5959 2d4d 4d2d 4444 222e  at "YYYY-MM-DD".
-0000a1c0: 0a20 2020 2020 2020 2054 6865 2063 6f6d  .        The com
-0000a1d0: 6d61 6e64 2077 696c 6c20 7573 6520 7468  mand will use th
-0000a1e0: 6520 2273 6163 6374 2220 746f 6f6c 2074  e "sacct" tool t
-0000a1f0: 6f20 7175 6572 7920 7468 650a 2020 2020  o query the.    
-0000a200: 2020 2020 536c 7572 6d20 6163 636f 756e      Slurm accoun
-0000a210: 7469 6e67 2064 6174 6162 6173 6520 666f  ting database fo
-0000a220: 7220 6a6f 6273 2074 6861 7420 7374 6172  r jobs that star
-0000a230: 7465 6420 6f6e 206f 7220 6166 7465 7220  ted on or after 
-0000a240: 7468 650a 2020 2020 2020 2020 7370 6563  the.        spec
-0000a250: 6966 6965 6420 7374 6172 7420 7469 6d65  ified start time
-0000a260: 2c20 616e 6420 7769 6c6c 206f 7574 7075  , and will outpu
-0000a270: 7420 6f6e 6c79 2074 6865 206a 6f62 2049  t only the job I
-0000a280: 4473 2028 2d6f 204a 6f62 4964 290a 2020  Ds (-o JobId).  
-0000a290: 2020 2020 2020 7769 7468 6f75 7420 6865        without he
-0000a2a0: 6164 6572 206f 7220 7472 6169 6c65 7220  ader or trailer 
-0000a2b0: 6c69 6e65 7320 282d 6e20 2d58 292e 0a0a  lines (-n -X)...
-0000a2c0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-0000a2d0: 2020 2020 2020 2020 2020 7374 6172 745f            start_
-0000a2e0: 7469 6d65 2028 7374 7229 3a20 5468 6520  time (str): The 
-0000a2f0: 7374 6172 7420 7469 6d65 2066 726f 6d20  start time from 
-0000a300: 7768 6963 6820 746f 2072 6574 7269 6576  which to retriev
-0000a310: 6520 6a6f 620a 2020 2020 2020 2020 2020  e job.          
-0000a320: 2020 2020 2020 696e 666f 726d 6174 696f        informatio
-0000a330: 6e2e 2044 6566 6175 6c74 7320 746f 2022  n. Defaults to "
-0000a340: 3230 3233 2d30 312d 3031 222e 0a20 2020  2023-01-01"..   
-0000a350: 2020 2020 2020 2020 2065 6e64 5f74 696d           end_tim
-0000a360: 6520 2873 7472 293a 2054 6865 2065 6e64  e (str): The end
-0000a370: 2074 696d 6520 756e 7469 6c20 7768 6963   time until whic
-0000a380: 6820 746f 2072 6574 7269 6576 6520 6a6f  h to retrieve jo
-0000a390: 620a 2020 2020 2020 2020 2020 2020 2020  b.              
-0000a3a0: 2020 696e 666f 726d 6174 696f 6e2e 2044    information. D
-0000a3b0: 6566 6175 6c74 7320 746f 2022 6e6f 7722  efaults to "now"
-0000a3c0: 2e0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-0000a3d0: 6c75 6d6e 7320 2873 7472 293a 2054 6865  lumns (str): The
-0000a3e0: 2063 6f6c 756d 6e73 2074 6f20 7265 7472   columns to retr
-0000a3f0: 6965 7665 2066 726f 6d20 7468 6520 6a6f  ieve from the jo
-0000a400: 6220 696e 666f 726d 6174 696f 6e2e 0a20  b information.. 
-0000a410: 2020 2020 2020 2020 2020 2020 2020 2044                 D
-0000a420: 6566 6175 6c74 7320 746f 2022 4a6f 6249  efaults to "JobI
-0000a430: 6422 2e20 4974 2069 7320 636f 6d6d 6120  d". It is comma 
-0000a440: 7365 7061 7261 7465 642c 2065 2e67 2e20  separated, e.g. 
-0000a450: 224a 6f62 4964 2c53 7461 7465 222e 0a20  "JobId,State".. 
-0000a460: 2020 2020 2020 2020 2020 2073 7461 7465             state
-0000a470: 7320 2873 7472 293a 2054 6865 206a 6f62  s (str): The job
-0000a480: 2073 7461 7465 7320 746f 2069 6e63 6c75   states to inclu
-0000a490: 6465 2069 6e20 7468 6520 7175 6572 792e  de in the query.
-0000a4a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a4b0: 2044 6566 6175 6c74 7320 746f 2022 722c   Defaults to "r,
-0000a4c0: 6364 2c66 2c74 6f2c 7273 2c64 6c2c 6e66  cd,f,to,rs,dl,nf
-0000a4d0: 222e 0a0a 2020 2020 2020 2020 5265 7475  "...        Retu
-0000a4e0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-0000a4f0: 2073 7472 3a0a 2020 2020 2020 2020 2020   str:.          
-0000a500: 2020 2020 2020 4120 7374 7269 6e67 2072        A string r
-0000a510: 6570 7265 7365 6e74 696e 6720 7468 6520  epresenting the 
-0000a520: 536c 7572 6d20 636f 6d6d 616e 6420 746f  Slurm command to
-0000a530: 2072 6574 7269 6576 650a 2020 2020 2020   retrieve.      
-0000a540: 2020 2020 2020 2020 2020 696e 666f 726d            inform
-0000a550: 6174 696f 6e20 6162 6f75 7420 6f6c 6420  ation about old 
-0000a560: 6a6f 6273 2e0a 2020 2020 2020 2020 2222  jobs..        ""
-0000a570: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-0000a580: 2073 656c 662e 5f41 4c4c 5f4a 4f42 535f   self._ALL_JOBS_
-0000a590: 434d 442e 666f 726d 6174 2873 7461 7274  CMD.format(start
-0000a5a0: 5f74 696d 653d 7374 6172 745f 7469 6d65  _time=start_time
-0000a5b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000a0c0: 2020 2020 2020 2073 7461 7465 733a 2073         states: s
+0000a0d0: 7472 203d 2022 722c 6364 2c66 2c74 6f2c  tr = "r,cd,f,to,
+0000a0e0: 7273 2c64 6c2c 6e66 2229 202d 3e20 7374  rs,dl,nf") -> st
+0000a0f0: 723a 0a20 2020 2020 2020 2022 2222 5265  r:.        """Re
+0000a100: 7475 726e 2074 6865 2053 6c75 726d 2063  turn the Slurm c
+0000a110: 6f6d 6d61 6e64 2074 6f20 7265 7472 6965  ommand to retrie
+0000a120: 7665 2069 6e66 6f72 6d61 7469 6f6e 2061  ve information a
+0000a130: 626f 7574 206f 6c64 206a 6f62 732e 0a0a  bout old jobs...
+0000a140: 2020 2020 2020 2020 5468 6520 636f 6d6d          The comm
+0000a150: 616e 6420 7769 6c6c 2062 6520 666f 726d  and will be form
+0000a160: 6174 7465 6420 7769 7468 2074 6865 2073  atted with the s
+0000a170: 7065 6369 6669 6564 2073 7461 7274 2074  pecified start t
+0000a180: 696d 652c 2077 6869 6368 2069 730a 2020  ime, which is.  
+0000a190: 2020 2020 2020 6578 7065 6374 6564 2074        expected t
+0000a1a0: 6f20 6265 2069 6e20 7468 6520 4953 4f20  o be in the ISO 
+0000a1b0: 666f 726d 6174 2022 5959 5959 2d4d 4d2d  format "YYYY-MM-
+0000a1c0: 4444 222e 0a20 2020 2020 2020 2054 6865  DD"..        The
+0000a1d0: 2063 6f6d 6d61 6e64 2077 696c 6c20 7573   command will us
+0000a1e0: 6520 7468 6520 2273 6163 6374 2220 746f  e the "sacct" to
+0000a1f0: 6f6c 2074 6f20 7175 6572 7920 7468 650a  ol to query the.
+0000a200: 2020 2020 2020 2020 536c 7572 6d20 6163          Slurm ac
+0000a210: 636f 756e 7469 6e67 2064 6174 6162 6173  counting databas
+0000a220: 6520 666f 7220 6a6f 6273 2074 6861 7420  e for jobs that 
+0000a230: 7374 6172 7465 6420 6f6e 206f 7220 6166  started on or af
+0000a240: 7465 7220 7468 650a 2020 2020 2020 2020  ter the.        
+0000a250: 7370 6563 6966 6965 6420 7374 6172 7420  specified start 
+0000a260: 7469 6d65 2c20 616e 6420 7769 6c6c 206f  time, and will o
+0000a270: 7574 7075 7420 6f6e 6c79 2074 6865 206a  utput only the j
+0000a280: 6f62 2049 4473 2028 2d6f 204a 6f62 4964  ob IDs (-o JobId
+0000a290: 290a 2020 2020 2020 2020 7769 7468 6f75  ).        withou
+0000a2a0: 7420 6865 6164 6572 206f 7220 7472 6169  t header or trai
+0000a2b0: 6c65 7220 6c69 6e65 7320 282d 6e20 2d58  ler lines (-n -X
+0000a2c0: 292e 0a0a 2020 2020 2020 2020 4172 6773  )...        Args
+0000a2d0: 3a0a 2020 2020 2020 2020 2020 2020 7374  :.            st
+0000a2e0: 6172 745f 7469 6d65 2028 7374 7229 3a20  art_time (str): 
+0000a2f0: 5468 6520 7374 6172 7420 7469 6d65 2066  The start time f
+0000a300: 726f 6d20 7768 6963 6820 746f 2072 6574  rom which to ret
+0000a310: 7269 6576 6520 6a6f 620a 2020 2020 2020  rieve job.      
+0000a320: 2020 2020 2020 2020 2020 696e 666f 726d            inform
+0000a330: 6174 696f 6e2e 2044 6566 6175 6c74 7320  ation. Defaults 
+0000a340: 746f 2022 3230 3233 2d30 312d 3031 222e  to "2023-01-01".
+0000a350: 0a20 2020 2020 2020 2020 2020 2065 6e64  .            end
+0000a360: 5f74 696d 6520 2873 7472 293a 2054 6865  _time (str): The
+0000a370: 2065 6e64 2074 696d 6520 756e 7469 6c20   end time until 
+0000a380: 7768 6963 6820 746f 2072 6574 7269 6576  which to retriev
+0000a390: 6520 6a6f 620a 2020 2020 2020 2020 2020  e job.          
+0000a3a0: 2020 2020 2020 696e 666f 726d 6174 696f        informatio
+0000a3b0: 6e2e 2044 6566 6175 6c74 7320 746f 2022  n. Defaults to "
+0000a3c0: 6e6f 7722 2e0a 2020 2020 2020 2020 2020  now"..          
+0000a3d0: 2020 636f 6c75 6d6e 7320 2873 7472 293a    columns (str):
+0000a3e0: 2054 6865 2063 6f6c 756d 6e73 2074 6f20   The columns to 
+0000a3f0: 7265 7472 6965 7665 2066 726f 6d20 7468  retrieve from th
+0000a400: 6520 6a6f 6220 696e 666f 726d 6174 696f  e job informatio
+0000a410: 6e2e 0a20 2020 2020 2020 2020 2020 2020  n..             
+0000a420: 2020 2044 6566 6175 6c74 7320 746f 2022     Defaults to "
+0000a430: 4a6f 6249 6422 2e20 4974 2069 7320 636f  JobId". It is co
+0000a440: 6d6d 6120 7365 7061 7261 7465 642c 2065  mma separated, e
+0000a450: 2e67 2e20 224a 6f62 4964 2c53 7461 7465  .g. "JobId,State
+0000a460: 222e 0a20 2020 2020 2020 2020 2020 2073  "..            s
+0000a470: 7461 7465 7320 2873 7472 293a 2054 6865  tates (str): The
+0000a480: 206a 6f62 2073 7461 7465 7320 746f 2069   job states to i
+0000a490: 6e63 6c75 6465 2069 6e20 7468 6520 7175  nclude in the qu
+0000a4a0: 6572 792e 0a20 2020 2020 2020 2020 2020  ery..           
+0000a4b0: 2020 2020 2044 6566 6175 6c74 7320 746f       Defaults to
+0000a4c0: 2022 722c 6364 2c66 2c74 6f2c 7273 2c64   "r,cd,f,to,rs,d
+0000a4d0: 6c2c 6e66 222e 0a0a 2020 2020 2020 2020  l,nf"...        
+0000a4e0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+0000a4f0: 2020 2020 2073 7472 3a0a 2020 2020 2020       str:.      
+0000a500: 2020 2020 2020 2020 2020 4120 7374 7269            A stri
+0000a510: 6e67 2072 6570 7265 7365 6e74 696e 6720  ng representing 
+0000a520: 7468 6520 536c 7572 6d20 636f 6d6d 616e  the Slurm comman
+0000a530: 6420 746f 2072 6574 7269 6576 650a 2020  d to retrieve.  
+0000a540: 2020 2020 2020 2020 2020 2020 2020 696e                in
+0000a550: 666f 726d 6174 696f 6e20 6162 6f75 7420  formation about 
+0000a560: 6f6c 6420 6a6f 6273 2e0a 2020 2020 2020  old jobs..      
+0000a570: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+0000a580: 7475 726e 2073 656c 662e 5f41 4c4c 5f4a  turn self._ALL_J
+0000a590: 4f42 535f 434d 442e 666f 726d 6174 2873  OBS_CMD.format(s
+0000a5a0: 7461 7274 5f74 696d 653d 7374 6172 745f  tart_time=start_
+0000a5b0: 7469 6d65 2c0a 2020 2020 2020 2020 2020  time,.          
 0000a5c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5d0: 2020 2020 2020 2020 2020 2065 6e64 5f74             end_t
-0000a5e0: 696d 653d 656e 645f 7469 6d65 2c0a 2020  ime=end_time,.  
-0000a5f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a5d0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
+0000a5e0: 6e64 5f74 696d 653d 656e 645f 7469 6d65  nd_time=end_time
+0000a5f0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 0000a600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a610: 2020 2020 2020 2073 7461 7465 733d 7374         states=st
-0000a620: 6174 6573 2c0a 2020 2020 2020 2020 2020  ates,.          
+0000a610: 2020 2020 2020 2020 2020 2073 7461 7465             state
+0000a620: 733d 7374 6174 6573 2c0a 2020 2020 2020  s=states,.      
 0000a630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a640: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000a650: 6f6c 756d 6e73 3d63 6f6c 756d 6e73 290a  olumns=columns).
-0000a660: 0a20 2020 2064 6566 2074 7261 6e73 6665  .    def transfe
-0000a670: 725f 6461 7461 2873 656c 662c 206c 6f63  r_data(self, loc
-0000a680: 616c 5f70 6174 683a 2073 7472 2920 2d3e  al_path: str) ->
-0000a690: 2052 6573 756c 743a 0a20 2020 2020 2020   Result:.       
-0000a6a0: 2022 2222 0a20 2020 2020 2020 2054 7261   """.        Tra
-0000a6b0: 6e73 6665 7273 2061 2066 696c 6520 6f72  nsfers a file or
-0000a6c0: 2064 6972 6563 746f 7279 2066 726f 6d20   directory from 
-0000a6d0: 7468 6520 6c6f 6361 6c20 6d61 6368 696e  the local machin
-0000a6e0: 6520 746f 2074 6865 2072 656d 6f74 650a  e to the remote.
-0000a6f0: 2020 2020 2020 2020 536c 7572 6d20 636c          Slurm cl
-0000a700: 7573 7465 722e 0a0a 2020 2020 2020 2020  uster...        
-0000a710: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-0000a720: 2020 6c6f 6361 6c5f 7061 7468 2028 7374    local_path (st
-0000a730: 7229 3a20 5468 6520 6c6f 6361 6c20 7061  r): The local pa
-0000a740: 7468 2074 6f20 7468 6520 6669 6c65 206f  th to the file o
-0000a750: 7220 6469 7265 6374 6f72 7920 746f 0a20  r directory to. 
-0000a760: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000a770: 7261 6e73 6665 722e 0a0a 2020 2020 2020  ransfer...      
-0000a780: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
-0000a790: 2020 2020 2020 2052 6573 756c 743a 2054         Result: T
-0000a7a0: 6865 2072 6573 756c 7420 6f66 2074 6865  he result of the
-0000a7b0: 2066 696c 6520 7472 616e 7366 6572 206f   file transfer o
-0000a7c0: 7065 7261 7469 6f6e 2e0a 2020 2020 2020  peration..      
-0000a7d0: 2020 2222 220a 2020 2020 2020 2020 6c6f    """.        lo
-0000a7e0: 6767 6572 2e69 6e66 6f28 0a20 2020 2020  gger.info(.     
-0000a7f0: 2020 2020 2020 2066 2254 7261 6e73 6665         f"Transfe
-0000a800: 7269 6e67 2066 696c 6520 7b6c 6f63 616c  ring file {local
-0000a810: 5f70 6174 687d 2074 6f20 7b73 656c 662e  _path} to {self.
-0000a820: 736c 7572 6d5f 6461 7461 5f70 6174 687d  slurm_data_path}
-0000a830: 2229 0a20 2020 2020 2020 2072 6574 7572  ").        retur
-0000a840: 6e20 7365 6c66 2e70 7574 286c 6f63 616c  n self.put(local
-0000a850: 3d6c 6f63 616c 5f70 6174 682c 2072 656d  =local_path, rem
-0000a860: 6f74 653d 7365 6c66 2e73 6c75 726d 5f64  ote=self.slurm_d
-0000a870: 6174 615f 7061 7468 290a 0a20 2020 2064  ata_path)..    d
-0000a880: 6566 2075 6e70 6163 6b5f 6461 7461 2873  ef unpack_data(s
-0000a890: 656c 662c 207a 6970 6669 6c65 3a20 7374  elf, zipfile: st
-0000a8a0: 722c 0a20 2020 2020 2020 2020 2020 2020  r,.             
-0000a8b0: 2020 2020 2020 2065 6e76 3a20 4f70 7469         env: Opti
-0000a8c0: 6f6e 616c 5b44 6963 745b 7374 722c 2073  onal[Dict[str, s
-0000a8d0: 7472 5d5d 203d 204e 6f6e 6529 202d 3e20  tr]] = None) -> 
-0000a8e0: 5265 7375 6c74 3a0a 2020 2020 2020 2020  Result:.        
-0000a8f0: 2222 220a 2020 2020 2020 2020 556e 7061  """.        Unpa
-0000a900: 636b 7320 6120 7a69 7070 6564 2066 696c  cks a zipped fil
-0000a910: 6520 6f6e 2074 6865 2072 656d 6f74 6520  e on the remote 
-0000a920: 536c 7572 6d20 636c 7573 7465 722e 0a0a  Slurm cluster...
-0000a930: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-0000a940: 2020 2020 2020 2020 2020 7a69 7066 696c            zipfil
-0000a950: 6520 2873 7472 293a 2054 6865 206e 616d  e (str): The nam
-0000a960: 6520 6f66 2074 6865 207a 6970 7065 6420  e of the zipped 
-0000a970: 6669 6c65 2074 6f20 6265 2075 6e70 6163  file to be unpac
-0000a980: 6b65 642e 0a0a 2020 2020 2020 2020 2020  ked...          
-0000a990: 2020 656e 7620 2844 6963 745b 7374 722c    env (Dict[str,
-0000a9a0: 2073 7472 5d2c 206f 7074 696f 6e61 6c29   str], optional)
-0000a9b0: 3a20 4f70 7469 6f6e 616c 2065 6e76 6972  : Optional envir
-0000a9c0: 6f6e 6d65 6e74 2076 6172 6961 626c 6573  onment variables
-0000a9d0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-0000a9e0: 2020 746f 2073 6574 2077 6865 6e20 7275    to set when ru
-0000a9f0: 6e6e 696e 6720 7468 6520 636f 6d6d 616e  nning the comman
-0000aa00: 642e 2044 6566 6175 6c74 7320 746f 204e  d. Defaults to N
-0000aa10: 6f6e 652e 0a0a 2020 2020 2020 2020 5265  one...        Re
-0000aa20: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-0000aa30: 2020 2052 6573 756c 743a 2054 6865 2072     Result: The r
-0000aa40: 6573 756c 7420 6f66 2074 6865 2063 6f6d  esult of the com
-0000aa50: 6d61 6e64 2e0a 2020 2020 2020 2020 2222  mand..        ""
-0000aa60: 220a 2020 2020 2020 2020 636d 6420 3d20  ".        cmd = 
-0000aa70: 7365 6c66 2e67 6574 5f75 6e7a 6970 5f63  self.get_unzip_c
-0000aa80: 6f6d 6d61 6e64 287a 6970 6669 6c65 290a  ommand(zipfile).
-0000aa90: 2020 2020 2020 2020 6c6f 6767 6572 2e69          logger.i
-0000aaa0: 6e66 6f28 6622 556e 7061 636b 696e 6720  nfo(f"Unpacking 
-0000aab0: 7b7a 6970 6669 6c65 7d20 6f6e 2053 6c75  {zipfile} on Slu
-0000aac0: 726d 2229 0a20 2020 2020 2020 2072 6574  rm").        ret
-0000aad0: 7572 6e20 7365 6c66 2e72 756e 5f63 6f6d  urn self.run_com
-0000aae0: 6d61 6e64 7328 5b63 6d64 5d2c 2065 6e76  mands([cmd], env
-0000aaf0: 3d65 6e76 290a 0a20 2020 2064 6566 2067  =env)..    def g
-0000ab00: 656e 6572 6174 655f 736c 7572 6d5f 6a6f  enerate_slurm_jo
-0000ab10: 625f 666f 725f 776f 726b 666c 6f77 2873  b_for_workflow(s
-0000ab20: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+0000a640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a650: 2020 2063 6f6c 756d 6e73 3d63 6f6c 756d     columns=colum
+0000a660: 6e73 290a 0a20 2020 2064 6566 2074 7261  ns)..    def tra
+0000a670: 6e73 6665 725f 6461 7461 2873 656c 662c  nsfer_data(self,
+0000a680: 206c 6f63 616c 5f70 6174 683a 2073 7472   local_path: str
+0000a690: 2920 2d3e 2052 6573 756c 743a 0a20 2020  ) -> Result:.   
+0000a6a0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000a6b0: 2054 7261 6e73 6665 7273 2061 2066 696c   Transfers a fil
+0000a6c0: 6520 6f72 2064 6972 6563 746f 7279 2066  e or directory f
+0000a6d0: 726f 6d20 7468 6520 6c6f 6361 6c20 6d61  rom the local ma
+0000a6e0: 6368 696e 6520 746f 2074 6865 2072 656d  chine to the rem
+0000a6f0: 6f74 650a 2020 2020 2020 2020 536c 7572  ote.        Slur
+0000a700: 6d20 636c 7573 7465 722e 0a0a 2020 2020  m cluster...    
+0000a710: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0000a720: 2020 2020 2020 6c6f 6361 6c5f 7061 7468        local_path
+0000a730: 2028 7374 7229 3a20 5468 6520 6c6f 6361   (str): The loca
+0000a740: 6c20 7061 7468 2074 6f20 7468 6520 6669  l path to the fi
+0000a750: 6c65 206f 7220 6469 7265 6374 6f72 7920  le or directory 
+0000a760: 746f 0a20 2020 2020 2020 2020 2020 2020  to.             
+0000a770: 2020 2074 7261 6e73 6665 722e 0a0a 2020     transfer...  
+0000a780: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+0000a790: 2020 2020 2020 2020 2020 2052 6573 756c             Resul
+0000a7a0: 743a 2054 6865 2072 6573 756c 7420 6f66  t: The result of
+0000a7b0: 2074 6865 2066 696c 6520 7472 616e 7366   the file transf
+0000a7c0: 6572 206f 7065 7261 7469 6f6e 2e0a 2020  er operation..  
+0000a7d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+0000a7e0: 2020 6c6f 6767 6572 2e69 6e66 6f28 0a20    logger.info(. 
+0000a7f0: 2020 2020 2020 2020 2020 2066 2254 7261             f"Tra
+0000a800: 6e73 6665 7269 6e67 2066 696c 6520 7b6c  nsfering file {l
+0000a810: 6f63 616c 5f70 6174 687d 2074 6f20 7b73  ocal_path} to {s
+0000a820: 656c 662e 736c 7572 6d5f 6461 7461 5f70  elf.slurm_data_p
+0000a830: 6174 687d 2229 0a20 2020 2020 2020 2072  ath}").        r
+0000a840: 6574 7572 6e20 7365 6c66 2e70 7574 286c  eturn self.put(l
+0000a850: 6f63 616c 3d6c 6f63 616c 5f70 6174 682c  ocal=local_path,
+0000a860: 2072 656d 6f74 653d 7365 6c66 2e73 6c75   remote=self.slu
+0000a870: 726d 5f64 6174 615f 7061 7468 290a 0a20  rm_data_path).. 
+0000a880: 2020 2064 6566 2075 6e70 6163 6b5f 6461     def unpack_da
+0000a890: 7461 2873 656c 662c 207a 6970 6669 6c65  ta(self, zipfile
+0000a8a0: 3a20 7374 722c 0a20 2020 2020 2020 2020  : str,.         
+0000a8b0: 2020 2020 2020 2020 2020 2065 6e76 3a20             env: 
+0000a8c0: 4f70 7469 6f6e 616c 5b44 6963 745b 7374  Optional[Dict[st
+0000a8d0: 722c 2073 7472 5d5d 203d 204e 6f6e 6529  r, str]] = None)
+0000a8e0: 202d 3e20 5265 7375 6c74 3a0a 2020 2020   -> Result:.    
+0000a8f0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000a900: 556e 7061 636b 7320 6120 7a69 7070 6564  Unpacks a zipped
+0000a910: 2066 696c 6520 6f6e 2074 6865 2072 656d   file on the rem
+0000a920: 6f74 6520 536c 7572 6d20 636c 7573 7465  ote Slurm cluste
+0000a930: 722e 0a0a 2020 2020 2020 2020 4172 6773  r...        Args
+0000a940: 3a0a 2020 2020 2020 2020 2020 2020 7a69  :.            zi
+0000a950: 7066 696c 6520 2873 7472 293a 2054 6865  pfile (str): The
+0000a960: 206e 616d 6520 6f66 2074 6865 207a 6970   name of the zip
+0000a970: 7065 6420 6669 6c65 2074 6f20 6265 2075  ped file to be u
+0000a980: 6e70 6163 6b65 642e 0a0a 2020 2020 2020  npacked...      
+0000a990: 2020 2020 2020 656e 7620 2844 6963 745b        env (Dict[
+0000a9a0: 7374 722c 2073 7472 5d2c 206f 7074 696f  str, str], optio
+0000a9b0: 6e61 6c29 3a20 4f70 7469 6f6e 616c 2065  nal): Optional e
+0000a9c0: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
+0000a9d0: 626c 6573 200a 2020 2020 2020 2020 2020  bles .          
+0000a9e0: 2020 2020 2020 746f 2073 6574 2077 6865        to set whe
+0000a9f0: 6e20 7275 6e6e 696e 6720 7468 6520 636f  n running the co
+0000aa00: 6d6d 616e 642e 2044 6566 6175 6c74 7320  mmand. Defaults 
+0000aa10: 746f 204e 6f6e 652e 0a0a 2020 2020 2020  to None...      
+0000aa20: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+0000aa30: 2020 2020 2020 2052 6573 756c 743a 2054         Result: T
+0000aa40: 6865 2072 6573 756c 7420 6f66 2074 6865  he result of the
+0000aa50: 2063 6f6d 6d61 6e64 2e0a 2020 2020 2020   command..      
+0000aa60: 2020 2222 220a 2020 2020 2020 2020 636d    """.        cm
+0000aa70: 6420 3d20 7365 6c66 2e67 6574 5f75 6e7a  d = self.get_unz
+0000aa80: 6970 5f63 6f6d 6d61 6e64 287a 6970 6669  ip_command(zipfi
+0000aa90: 6c65 290a 2020 2020 2020 2020 6c6f 6767  le).        logg
+0000aaa0: 6572 2e69 6e66 6f28 6622 556e 7061 636b  er.info(f"Unpack
+0000aab0: 696e 6720 7b7a 6970 6669 6c65 7d20 6f6e  ing {zipfile} on
+0000aac0: 2053 6c75 726d 2229 0a20 2020 2020 2020   Slurm").       
+0000aad0: 2072 6574 7572 6e20 7365 6c66 2e72 756e   return self.run
+0000aae0: 5f63 6f6d 6d61 6e64 7328 5b63 6d64 5d2c  _commands([cmd],
+0000aaf0: 2065 6e76 3d65 6e76 290a 0a20 2020 2064   env=env)..    d
+0000ab00: 6566 2067 656e 6572 6174 655f 736c 7572  ef generate_slur
+0000ab10: 6d5f 6a6f 625f 666f 725f 776f 726b 666c  m_job_for_workfl
+0000ab20: 6f77 2873 656c 662c 0a20 2020 2020 2020  ow(self,.       
 0000ab30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab40: 2020 2020 2020 2020 2020 2020 2077 6f72               wor
-0000ab50: 6b66 6c6f 773a 2073 7472 2c0a 2020 2020  kflow: str,.    
+0000ab40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ab50: 2077 6f72 6b66 6c6f 773a 2073 7472 2c0a   workflow: str,.
 0000ab60: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ab70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab80: 2020 2020 7375 6273 7469 7475 7465 733a      substitutes:
-0000ab90: 2044 6963 745b 7374 722c 2073 7472 5d2c   Dict[str, str],
-0000aba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ab80: 2020 2020 2020 2020 7375 6273 7469 7475          substitu
+0000ab90: 7465 733a 2044 6963 745b 7374 722c 2073  tes: Dict[str, s
+0000aba0: 7472 5d2c 0a20 2020 2020 2020 2020 2020  tr],.           
 0000abb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000abc0: 2020 2020 2020 2020 2074 656d 706c 6174           templat
-0000abd0: 653a 2073 7472 203d 2022 6a6f 625f 7465  e: str = "job_te
-0000abe0: 6d70 6c61 7465 2e73 6822 0a20 2020 2020  mplate.sh".     
+0000abc0: 2020 2020 2020 2020 2020 2020 2074 656d               tem
+0000abd0: 706c 6174 653a 2073 7472 203d 2022 6a6f  plate: str = "jo
+0000abe0: 625f 7465 6d70 6c61 7465 2e73 6822 0a20  b_template.sh". 
 0000abf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 0000ac00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ac10: 2020 2029 202d 3e20 7374 723a 0a20 2020     ) -> str:.   
-0000ac20: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000ac30: 2047 656e 6572 6174 6520 6120 536c 7572   Generate a Slur
-0000ac40: 6d20 6a6f 6220 7363 7269 7074 2066 6f72  m job script for
-0000ac50: 2061 2073 7065 6369 6669 6320 776f 726b   a specific work
-0000ac60: 666c 6f77 2e0a 0a20 2020 2020 2020 2041  flow...        A
-0000ac70: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-0000ac80: 2077 6f72 6b66 6c6f 7720 2873 7472 293a   workflow (str):
-0000ac90: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
-0000aca0: 2077 6f72 6b66 6c6f 772e 0a20 2020 2020   workflow..     
-0000acb0: 2020 2020 2020 2073 7562 7374 6974 7574         substitut
-0000acc0: 6573 2028 4469 6374 5b73 7472 2c20 7374  es (Dict[str, st
-0000acd0: 725d 293a 2041 2064 6963 7469 6f6e 6172  r]): A dictionar
-0000ace0: 7920 636f 6e74 6169 6e69 6e67 206b 6579  y containing key
-0000acf0: 2d76 616c 7565 0a20 2020 2020 2020 2020  -value.         
-0000ad00: 2020 2020 2020 2070 6169 7273 2066 6f72         pairs for
-0000ad10: 2073 7562 7374 6974 7574 696e 6720 706c   substituting pl
-0000ad20: 6163 6568 6f6c 6465 7273 2069 6e20 7468  aceholders in th
-0000ad30: 6520 6a6f 6220 7465 6d70 6c61 7465 2e0a  e job template..
-0000ad40: 2020 2020 2020 2020 2020 2020 7465 6d70              temp
-0000ad50: 6c61 7465 2028 7374 722c 206f 7074 696f  late (str, optio
-0000ad60: 6e61 6c29 3a20 5468 6520 6669 6c65 6e61  nal): The filena
-0000ad70: 6d65 206f 6620 7468 6520 6a6f 6220 7465  me of the job te
-0000ad80: 6d70 6c61 7465 2e0a 2020 2020 2020 2020  mplate..        
-0000ad90: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
-0000ada0: 2074 6f20 226a 6f62 5f74 656d 706c 6174   to "job_templat
-0000adb0: 652e 7368 222e 0a0a 2020 2020 2020 2020  e.sh"...        
-0000adc0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-0000add0: 2020 2020 2073 7472 3a20 5468 6520 6765       str: The ge
-0000ade0: 6e65 7261 7465 6420 536c 7572 6d20 6a6f  nerated Slurm jo
-0000adf0: 6220 7363 7269 7074 2061 7320 6120 7374  b script as a st
-0000ae00: 7269 6e67 2e0a 2020 2020 2020 2020 2222  ring..        ""
-0000ae10: 220a 2020 2020 2020 2020 2320 6164 6420  ".        # add 
-0000ae20: 776f 726b 666c 6f77 2074 6f20 7375 6273  workflow to subs
-0000ae30: 7469 7475 7465 730a 2020 2020 2020 2020  titutes.        
-0000ae40: 7375 6273 7469 7475 7465 735b 276a 6f62  substitutes['job
-0000ae50: 6e61 6d65 275d 203d 2077 6f72 6b66 6c6f  name'] = workflo
-0000ae60: 770a 2020 2020 2020 2020 2320 6772 6162  w.        # grab
-0000ae70: 206a 6f62 2074 656d 706c 6174 650a 2020   job template.  
-0000ae80: 2020 2020 2020 7465 6d70 6c61 7465 5f66        template_f
-0000ae90: 203d 2066 696c 6573 2822 7265 736f 7572   = files("resour
-0000aea0: 6365 7322 292e 6a6f 696e 7061 7468 2874  ces").joinpath(t
-0000aeb0: 656d 706c 6174 6529 0a20 2020 2020 2020  emplate).       
-0000aec0: 2077 6974 6820 7465 6d70 6c61 7465 5f66   with template_f
-0000aed0: 2e6f 7065 6e28 2772 2729 2061 7320 663a  .open('r') as f:
-0000aee0: 0a20 2020 2020 2020 2020 2020 2073 7263  .            src
-0000aef0: 203d 2054 656d 706c 6174 6528 662e 7265   = Template(f.re
-0000af00: 6164 2829 290a 2020 2020 2020 2020 2020  ad()).          
-0000af10: 2020 6a6f 625f 7363 7269 7074 203d 2073    job_script = s
-0000af20: 7263 2e73 6166 655f 7375 6273 7469 7475  rc.safe_substitu
-0000af30: 7465 2873 7562 7374 6974 7574 6573 290a  te(substitutes).
-0000af40: 2020 2020 2020 2020 7265 7475 726e 206a          return j
-0000af50: 6f62 5f73 6372 6970 740a 0a20 2020 2064  ob_script..    d
-0000af60: 6566 2077 6f72 6b66 6c6f 775f 7061 7261  ef workflow_para
-0000af70: 6d73 5f74 6f5f 7375 6273 2873 656c 662c  ms_to_subs(self,
-0000af80: 2070 6172 616d 7329 202d 3e20 4469 6374   params) -> Dict
-0000af90: 5b73 7472 2c20 7374 725d 3a0a 2020 2020  [str, str]:.    
-0000afa0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000afb0: 436f 6e76 6572 7420 776f 726b 666c 6f77  Convert workflow
-0000afc0: 2070 6172 616d 6574 6572 7320 746f 2073   parameters to s
-0000afd0: 7562 7374 6974 7574 696f 6e20 6469 6374  ubstitution dict
-0000afe0: 696f 6e61 7279 2066 6f72 206a 6f62 2073  ionary for job s
-0000aff0: 6372 6970 742e 0a0a 2020 2020 2020 2020  cript...        
-0000b000: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-0000b010: 2020 7061 7261 6d73 3a20 4120 6469 6374    params: A dict
-0000b020: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
-0000b030: 6720 776f 726b 666c 6f77 2070 6172 616d  g workflow param
-0000b040: 6574 6572 732e 0a0a 2020 2020 2020 2020  eters...        
-0000b050: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
-0000b060: 2020 2020 2044 6963 745b 7374 722c 2073       Dict[str, s
-0000b070: 7472 5d3a 2041 2064 6963 7469 6f6e 6172  tr]: A dictionar
-0000b080: 7920 7769 7468 2070 6172 616d 6574 6572  y with parameter
-0000b090: 206e 616d 6573 2061 7320 6b65 7973 2061   names as keys a
-0000b0a0: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
-0000b0b0: 2020 2063 6f72 7265 7370 6f6e 6469 6e67     corresponding
-0000b0c0: 2066 6c61 6773 2077 6974 6820 706c 6163   flags with plac
-0000b0d0: 6568 6f6c 6465 7273 2061 7320 7661 6c75  eholders as valu
-0000b0e0: 6573 2e0a 2020 2020 2020 2020 2222 220a  es..        """.
-0000b0f0: 2020 2020 2020 2020 7375 6273 203d 207b          subs = {
-0000b100: 7d0a 2020 2020 2020 2020 666c 6167 7320  }.        flags 
-0000b110: 3d20 5b5d 0a20 2020 2020 2020 2066 6f72  = [].        for
-0000b120: 205f 2c20 7061 7261 6d20 696e 2070 6172   _, param in par
-0000b130: 616d 732e 6974 656d 7328 293a 0a20 2020  ams.items():.   
-0000b140: 2020 2020 2020 2020 2066 6c61 6720 3d20           flag = 
-0000b150: 7061 7261 6d5b 2763 6d64 5f66 6c61 6727  param['cmd_flag'
-0000b160: 5d0a 2020 2020 2020 2020 2020 2020 666c  ].            fl
-0000b170: 6167 203d 2066 6c61 6720 2b20 2220 2422  ag = flag + " $"
-0000b180: 202b 2070 6172 616d 5b27 6e61 6d65 275d   + param['name']
-0000b190: 2e75 7070 6572 2829 0a20 2020 2020 2020  .upper().       
-0000b1a0: 2020 2020 2066 6c61 6773 2e61 7070 656e       flags.appen
-0000b1b0: 6428 666c 6167 290a 2020 2020 2020 2020  d(flag).        
-0000b1c0: 7375 6273 5b27 5041 5241 4d53 275d 203d  subs['PARAMS'] =
-0000b1d0: 2022 2022 2e6a 6f69 6e28 666c 6167 7329   " ".join(flags)
-0000b1e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000b1f0: 7375 6273 0a0a 2020 2020 6465 6620 7570  subs..    def up
-0000b200: 6461 7465 5f73 6c75 726d 5f73 6372 6970  date_slurm_scrip
-0000b210: 7473 2873 656c 662c 0a20 2020 2020 2020  ts(self,.       
+0000ac10: 2020 2020 2020 2029 202d 3e20 7374 723a         ) -> str:
+0000ac20: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000ac30: 2020 2020 2047 656e 6572 6174 6520 6120       Generate a 
+0000ac40: 536c 7572 6d20 6a6f 6220 7363 7269 7074  Slurm job script
+0000ac50: 2066 6f72 2061 2073 7065 6369 6669 6320   for a specific 
+0000ac60: 776f 726b 666c 6f77 2e0a 0a20 2020 2020  workflow...     
+0000ac70: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000ac80: 2020 2020 2077 6f72 6b66 6c6f 7720 2873       workflow (s
+0000ac90: 7472 293a 2054 6865 206e 616d 6520 6f66  tr): The name of
+0000aca0: 2074 6865 2077 6f72 6b66 6c6f 772e 0a20   the workflow.. 
+0000acb0: 2020 2020 2020 2020 2020 2073 7562 7374             subst
+0000acc0: 6974 7574 6573 2028 4469 6374 5b73 7472  itutes (Dict[str
+0000acd0: 2c20 7374 725d 293a 2041 2064 6963 7469  , str]): A dicti
+0000ace0: 6f6e 6172 7920 636f 6e74 6169 6e69 6e67  onary containing
+0000acf0: 206b 6579 2d76 616c 7565 0a20 2020 2020   key-value.     
+0000ad00: 2020 2020 2020 2020 2020 2070 6169 7273             pairs
+0000ad10: 2066 6f72 2073 7562 7374 6974 7574 696e   for substitutin
+0000ad20: 6720 706c 6163 6568 6f6c 6465 7273 2069  g placeholders i
+0000ad30: 6e20 7468 6520 6a6f 6220 7465 6d70 6c61  n the job templa
+0000ad40: 7465 2e0a 2020 2020 2020 2020 2020 2020  te..            
+0000ad50: 7465 6d70 6c61 7465 2028 7374 722c 206f  template (str, o
+0000ad60: 7074 696f 6e61 6c29 3a20 5468 6520 6669  ptional): The fi
+0000ad70: 6c65 6e61 6d65 206f 6620 7468 6520 6a6f  lename of the jo
+0000ad80: 6220 7465 6d70 6c61 7465 2e0a 2020 2020  b template..    
+0000ad90: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+0000ada0: 756c 7473 2074 6f20 226a 6f62 5f74 656d  ults to "job_tem
+0000adb0: 706c 6174 652e 7368 222e 0a0a 2020 2020  plate.sh"...    
+0000adc0: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+0000add0: 2020 2020 2020 2020 2073 7472 3a20 5468           str: Th
+0000ade0: 6520 6765 6e65 7261 7465 6420 536c 7572  e generated Slur
+0000adf0: 6d20 6a6f 6220 7363 7269 7074 2061 7320  m job script as 
+0000ae00: 6120 7374 7269 6e67 2e0a 2020 2020 2020  a string..      
+0000ae10: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
+0000ae20: 6164 6420 776f 726b 666c 6f77 2074 6f20  add workflow to 
+0000ae30: 7375 6273 7469 7475 7465 730a 2020 2020  substitutes.    
+0000ae40: 2020 2020 7375 6273 7469 7475 7465 735b      substitutes[
+0000ae50: 276a 6f62 6e61 6d65 275d 203d 2077 6f72  'jobname'] = wor
+0000ae60: 6b66 6c6f 770a 2020 2020 2020 2020 2320  kflow.        # 
+0000ae70: 6772 6162 206a 6f62 2074 656d 706c 6174  grab job templat
+0000ae80: 650a 2020 2020 2020 2020 7465 6d70 6c61  e.        templa
+0000ae90: 7465 5f66 203d 2066 696c 6573 2822 7265  te_f = files("re
+0000aea0: 736f 7572 6365 7322 292e 6a6f 696e 7061  sources").joinpa
+0000aeb0: 7468 2874 656d 706c 6174 6529 0a20 2020  th(template).   
+0000aec0: 2020 2020 2077 6974 6820 7465 6d70 6c61       with templa
+0000aed0: 7465 5f66 2e6f 7065 6e28 2772 2729 2061  te_f.open('r') a
+0000aee0: 7320 663a 0a20 2020 2020 2020 2020 2020  s f:.           
+0000aef0: 2073 7263 203d 2054 656d 706c 6174 6528   src = Template(
+0000af00: 662e 7265 6164 2829 290a 2020 2020 2020  f.read()).      
+0000af10: 2020 2020 2020 6a6f 625f 7363 7269 7074        job_script
+0000af20: 203d 2073 7263 2e73 6166 655f 7375 6273   = src.safe_subs
+0000af30: 7469 7475 7465 2873 7562 7374 6974 7574  titute(substitut
+0000af40: 6573 290a 2020 2020 2020 2020 7265 7475  es).        retu
+0000af50: 726e 206a 6f62 5f73 6372 6970 740a 0a20  rn job_script.. 
+0000af60: 2020 2064 6566 2077 6f72 6b66 6c6f 775f     def workflow_
+0000af70: 7061 7261 6d73 5f74 6f5f 7375 6273 2873  params_to_subs(s
+0000af80: 656c 662c 2070 6172 616d 7329 202d 3e20  elf, params) -> 
+0000af90: 4469 6374 5b73 7472 2c20 7374 725d 3a0a  Dict[str, str]:.
+0000afa0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000afb0: 2020 2020 436f 6e76 6572 7420 776f 726b      Convert work
+0000afc0: 666c 6f77 2070 6172 616d 6574 6572 7320  flow parameters 
+0000afd0: 746f 2073 7562 7374 6974 7574 696f 6e20  to substitution 
+0000afe0: 6469 6374 696f 6e61 7279 2066 6f72 206a  dictionary for j
+0000aff0: 6f62 2073 6372 6970 742e 0a0a 2020 2020  ob script...    
+0000b000: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0000b010: 2020 2020 2020 7061 7261 6d73 3a20 4120        params: A 
+0000b020: 6469 6374 696f 6e61 7279 2063 6f6e 7461  dictionary conta
+0000b030: 696e 696e 6720 776f 726b 666c 6f77 2070  ining workflow p
+0000b040: 6172 616d 6574 6572 732e 0a0a 2020 2020  arameters...    
+0000b050: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+0000b060: 2020 2020 2020 2020 2044 6963 745b 7374           Dict[st
+0000b070: 722c 2073 7472 5d3a 2041 2064 6963 7469  r, str]: A dicti
+0000b080: 6f6e 6172 7920 7769 7468 2070 6172 616d  onary with param
+0000b090: 6574 6572 206e 616d 6573 2061 7320 6b65  eter names as ke
+0000b0a0: 7973 2061 6e64 0a20 2020 2020 2020 2020  ys and.         
+0000b0b0: 2020 2020 2020 2063 6f72 7265 7370 6f6e         correspon
+0000b0c0: 6469 6e67 2066 6c61 6773 2077 6974 6820  ding flags with 
+0000b0d0: 706c 6163 6568 6f6c 6465 7273 2061 7320  placeholders as 
+0000b0e0: 7661 6c75 6573 2e0a 2020 2020 2020 2020  values..        
+0000b0f0: 2222 220a 2020 2020 2020 2020 7375 6273  """.        subs
+0000b100: 203d 207b 7d0a 2020 2020 2020 2020 666c   = {}.        fl
+0000b110: 6167 7320 3d20 5b5d 0a20 2020 2020 2020  ags = [].       
+0000b120: 2066 6f72 205f 2c20 7061 7261 6d20 696e   for _, param in
+0000b130: 2070 6172 616d 732e 6974 656d 7328 293a   params.items():
+0000b140: 0a20 2020 2020 2020 2020 2020 2066 6c61  .            fla
+0000b150: 6720 3d20 7061 7261 6d5b 2763 6d64 5f66  g = param['cmd_f
+0000b160: 6c61 6727 5d0a 2020 2020 2020 2020 2020  lag'].          
+0000b170: 2020 666c 6167 203d 2066 6c61 6720 2b20    flag = flag + 
+0000b180: 2220 2422 202b 2070 6172 616d 5b27 6e61  " $" + param['na
+0000b190: 6d65 275d 2e75 7070 6572 2829 0a20 2020  me'].upper().   
+0000b1a0: 2020 2020 2020 2020 2066 6c61 6773 2e61           flags.a
+0000b1b0: 7070 656e 6428 666c 6167 290a 2020 2020  ppend(flag).    
+0000b1c0: 2020 2020 7375 6273 5b27 5041 5241 4d53      subs['PARAMS
+0000b1d0: 275d 203d 2022 2022 2e6a 6f69 6e28 666c  '] = " ".join(fl
+0000b1e0: 6167 7329 0a20 2020 2020 2020 2072 6574  ags).        ret
+0000b1f0: 7572 6e20 7375 6273 0a0a 2020 2020 6465  urn subs..    de
+0000b200: 6620 7570 6461 7465 5f73 6c75 726d 5f73  f update_slurm_s
+0000b210: 6372 6970 7473 2873 656c 662c 0a20 2020  cripts(self,.   
 0000b220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b230: 2020 2020 2020 6765 6e65 7261 7465 5f6a        generate_j
-0000b240: 6f62 733a 2062 6f6f 6c20 3d20 4661 6c73  obs: bool = Fals
-0000b250: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+0000b230: 2020 2020 2020 2020 2020 6765 6e65 7261            genera
+0000b240: 7465 5f6a 6f62 733a 2062 6f6f 6c20 3d20  te_jobs: bool = 
+0000b250: 4661 6c73 652c 0a20 2020 2020 2020 2020  False,.         
 0000b260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b270: 656e 763a 204f 7074 696f 6e61 6c5b 4469  env: Optional[Di
-0000b280: 6374 5b73 7472 2c20 7374 725d 5d20 3d20  ct[str, str]] = 
-0000b290: 4e6f 6e65 2920 2d3e 2052 6573 756c 743a  None) -> Result:
-0000b2a0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000b2b0: 2020 2020 2055 7064 6174 6573 2074 6865       Updates the
-0000b2c0: 206c 6f63 616c 2063 6f70 7920 6f66 2074   local copy of t
-0000b2d0: 6865 2053 6c75 726d 206a 6f62 2073 7562  he Slurm job sub
-0000b2e0: 6d69 7373 696f 6e20 7363 7269 7074 732e  mission scripts.
-0000b2f0: 0a0a 2020 2020 2020 2020 5468 6973 2066  ..        This f
-0000b300: 756e 6374 696f 6e20 7075 6c6c 7320 7468  unction pulls th
-0000b310: 6520 6c61 7465 7374 2076 6572 7369 6f6e  e latest version
-0000b320: 206f 6620 7468 6520 7363 7269 7074 7320   of the scripts 
-0000b330: 6672 6f6d 2074 6865 2047 6974 0a20 2020  from the Git.   
-0000b340: 2020 2020 2072 6570 6f73 6974 6f72 7920       repository 
-0000b350: 616e 6420 636f 7069 6573 2074 6865 6d20  and copies them 
-0000b360: 746f 2074 6865 2073 6c75 726d 5f73 6372  to the slurm_scr
-0000b370: 6970 745f 7061 7468 2064 6972 6563 746f  ipt_path directo
-0000b380: 7279 2e0a 2020 2020 2020 2020 416c 7465  ry..        Alte
-0000b390: 726e 6174 6976 656c 792c 2069 7420 6361  rnatively, it ca
-0000b3a0: 6e20 6765 6e65 7261 7465 2073 6372 6970  n generate scrip
-0000b3b0: 7473 2066 726f 6d20 6120 7465 6d70 6c61  ts from a templa
-0000b3c0: 7465 2e20 5468 6973 2069 7320 7468 650a  te. This is the.
-0000b3d0: 2020 2020 2020 2020 6465 6661 756c 7420          default 
-0000b3e0: 6265 6861 7669 6f72 2069 6620 6e6f 2047  behavior if no G
-0000b3f0: 6974 2072 6570 6f20 6973 2070 726f 7669  it repo is provi
-0000b400: 6465 6420 6f72 2063 616e 2062 6520 666f  ded or can be fo
-0000b410: 7263 6564 2076 6961 2074 6865 0a20 2020  rced via the.   
-0000b420: 2020 2020 2060 6765 6e65 7261 7465 5f6a       `generate_j
-0000b430: 6f62 7360 2070 6172 616d 6574 6572 2e0a  obs` parameter..
-0000b440: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-0000b450: 2020 2020 2020 2020 2020 2067 656e 6572             gener
-0000b460: 6174 655f 6a6f 6273 2028 626f 6f6c 293a  ate_jobs (bool):
-0000b470: 2057 6865 7468 6572 2074 6f20 6765 6e65   Whether to gene
-0000b480: 7261 7465 206e 6577 2073 6c75 726d 206a  rate new slurm j
-0000b490: 6f62 2073 6372 6970 7473 0a20 2020 2020  ob scripts.     
-0000b4a0: 2020 2020 2020 2020 2020 2049 4e53 5445             INSTE
-0000b4b0: 4144 2028 6f66 2070 756c 6c69 6e67 2066  AD (of pulling f
-0000b4c0: 726f 6d20 6769 7429 2e20 4465 6661 756c  rom git). Defaul
-0000b4d0: 7473 2074 6f20 4661 6c73 652c 2065 7863  ts to False, exc
-0000b4e0: 6570 740a 2020 2020 2020 2020 2020 2020  ept.            
-0000b4f0: 2020 2020 6966 206e 6f20 736c 7572 6d5f      if no slurm_
-0000b500: 7363 7269 7074 5f72 6570 6f20 6973 2063  script_repo is c
-0000b510: 6f6e 6669 6775 7265 642e 0a20 2020 2020  onfigured..     
-0000b520: 2020 2020 2020 2065 6e76 2028 4469 6374         env (Dict
-0000b530: 5b73 7472 2c20 7374 725d 2c20 6f70 7469  [str, str], opti
-0000b540: 6f6e 616c 293a 204f 7074 696f 6e61 6c20  onal): Optional 
-0000b550: 656e 7669 726f 6e6d 656e 7420 7661 7269  environment vari
-0000b560: 6162 6c65 7320 0a20 2020 2020 2020 2020  ables .         
-0000b570: 2020 2020 2020 2074 6f20 7365 7420 7768         to set wh
-0000b580: 656e 2072 756e 6e69 6e67 2074 6865 2063  en running the c
-0000b590: 6f6d 6d61 6e64 2e20 4465 6661 756c 7473  ommand. Defaults
-0000b5a0: 2074 6f20 4e6f 6e65 2e0a 0a20 2020 2020   to None...     
-0000b5b0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-0000b5c0: 2020 2020 2020 2020 5265 7375 6c74 3a20          Result: 
-0000b5d0: 5468 6520 7265 7375 6c74 206f 6620 7468  The result of th
-0000b5e0: 6520 636f 6d6d 616e 642e 0a20 2020 2020  e command..     
-0000b5f0: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
-0000b600: 6620 6e6f 7420 7365 6c66 2e73 6c75 726d  f not self.slurm
-0000b610: 5f73 6372 6970 745f 7265 706f 3a0a 2020  _script_repo:.  
-0000b620: 2020 2020 2020 2020 2020 6765 6e65 7261            genera
-0000b630: 7465 5f6a 6f62 7320 3d20 5472 7565 0a0a  te_jobs = True..
-0000b640: 2020 2020 2020 2020 6966 2067 656e 6572          if gener
-0000b650: 6174 655f 6a6f 6273 3a0a 2020 2020 2020  ate_jobs:.      
-0000b660: 2020 2020 2020 6c6f 6767 6572 2e69 6e66        logger.inf
-0000b670: 6f28 2247 656e 6572 6174 696e 6720 536c  o("Generating Sl
-0000b680: 7572 6d20 6a6f 6220 7363 7269 7074 7322  urm job scripts"
-0000b690: 290a 2020 2020 2020 2020 2020 2020 666f  ).            fo
-0000b6a0: 7220 7766 2c20 6a6f 625f 7061 7468 2069  r wf, job_path i
-0000b6b0: 6e20 7365 6c66 2e73 6c75 726d 5f6d 6f64  n self.slurm_mod
-0000b6c0: 656c 5f6a 6f62 732e 6974 656d 7328 293a  el_jobs.items():
-0000b6d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b6e0: 2023 2067 656e 6572 6174 6520 6a6f 6220   # generate job 
-0000b6f0: 7363 7269 7074 0a20 2020 2020 2020 2020  script.         
-0000b700: 2020 2020 2020 2070 6172 616d 7320 3d20         params = 
-0000b710: 7365 6c66 2e67 6574 5f77 6f72 6b66 6c6f  self.get_workflo
-0000b720: 775f 7061 7261 6d65 7465 7273 2877 6629  w_parameters(wf)
-0000b730: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000b740: 2073 7562 7320 3d20 7365 6c66 2e77 6f72   subs = self.wor
-0000b750: 6b66 6c6f 775f 7061 7261 6d73 5f74 6f5f  kflow_params_to_
-0000b760: 7375 6273 2870 6172 616d 7329 0a20 2020  subs(params).   
-0000b770: 2020 2020 2020 2020 2020 2020 206a 6f62               job
-0000b780: 5f73 6372 6970 7420 3d20 7365 6c66 2e67  _script = self.g
-0000b790: 656e 6572 6174 655f 736c 7572 6d5f 6a6f  enerate_slurm_jo
-0000b7a0: 625f 666f 725f 776f 726b 666c 6f77 2877  b_for_workflow(w
-0000b7b0: 662c 2073 7562 7329 0a20 2020 2020 2020  f, subs).       
-0000b7c0: 2020 2020 2020 2020 2023 2065 6e73 7572           # ensur
-0000b7d0: 6520 616c 6c20 6469 7273 2065 7869 7374  e all dirs exist
-0000b7e0: 2072 656d 6f74 656c 790a 2020 2020 2020   remotely.      
-0000b7f0: 2020 2020 2020 2020 2020 6675 6c6c 5f70            full_p
-0000b800: 6174 6820 3d20 7365 6c66 2e73 6c75 726d  ath = self.slurm
-0000b810: 5f73 6372 6970 745f 7061 7468 2b22 2f22  _script_path+"/"
-0000b820: 2b6a 6f62 5f70 6174 680a 2020 2020 2020  +job_path.      
-0000b830: 2020 2020 2020 2020 2020 6a6f 625f 6469            job_di
-0000b840: 722c 205f 203d 206f 732e 7061 7468 2e73  r, _ = os.path.s
-0000b850: 706c 6974 2866 756c 6c5f 7061 7468 290a  plit(full_path).
-0000b860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b870: 7365 6c66 2e72 756e 2866 226d 6b64 6972  self.run(f"mkdir
-0000b880: 202d 7020 5c22 7b6a 6f62 5f64 6972 7d5c   -p \"{job_dir}\
-0000b890: 2222 290a 2020 2020 2020 2020 2020 2020  "").            
-0000b8a0: 2020 2020 2320 636f 7079 2074 6f20 7265      # copy to re
-0000b8b0: 6d6f 7465 2066 696c 650a 2020 2020 2020  mote file.      
-0000b8c0: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0000b8d0: 203d 2073 656c 662e 7075 7428 6c6f 6361   = self.put(loca
-0000b8e0: 6c3d 696f 2e53 7472 696e 6749 4f28 6a6f  l=io.StringIO(jo
-0000b8f0: 625f 7363 7269 7074 292c 0a20 2020 2020  b_script),.     
+0000b270: 2020 2020 656e 763a 204f 7074 696f 6e61      env: Optiona
+0000b280: 6c5b 4469 6374 5b73 7472 2c20 7374 725d  l[Dict[str, str]
+0000b290: 5d20 3d20 4e6f 6e65 2920 2d3e 2052 6573  ] = None) -> Res
+0000b2a0: 756c 743a 0a20 2020 2020 2020 2022 2222  ult:.        """
+0000b2b0: 0a20 2020 2020 2020 2055 7064 6174 6573  .        Updates
+0000b2c0: 2074 6865 206c 6f63 616c 2063 6f70 7920   the local copy 
+0000b2d0: 6f66 2074 6865 2053 6c75 726d 206a 6f62  of the Slurm job
+0000b2e0: 2073 7562 6d69 7373 696f 6e20 7363 7269   submission scri
+0000b2f0: 7074 732e 0a0a 2020 2020 2020 2020 5468  pts...        Th
+0000b300: 6973 2066 756e 6374 696f 6e20 7075 6c6c  is function pull
+0000b310: 7320 7468 6520 6c61 7465 7374 2076 6572  s the latest ver
+0000b320: 7369 6f6e 206f 6620 7468 6520 7363 7269  sion of the scri
+0000b330: 7074 7320 6672 6f6d 2074 6865 2047 6974  pts from the Git
+0000b340: 0a20 2020 2020 2020 2072 6570 6f73 6974  .        reposit
+0000b350: 6f72 7920 616e 6420 636f 7069 6573 2074  ory and copies t
+0000b360: 6865 6d20 746f 2074 6865 2073 6c75 726d  hem to the slurm
+0000b370: 5f73 6372 6970 745f 7061 7468 2064 6972  _script_path dir
+0000b380: 6563 746f 7279 2e0a 2020 2020 2020 2020  ectory..        
+0000b390: 416c 7465 726e 6174 6976 656c 792c 2069  Alternatively, i
+0000b3a0: 7420 6361 6e20 6765 6e65 7261 7465 2073  t can generate s
+0000b3b0: 6372 6970 7473 2066 726f 6d20 6120 7465  cripts from a te
+0000b3c0: 6d70 6c61 7465 2e20 5468 6973 2069 7320  mplate. This is 
+0000b3d0: 7468 650a 2020 2020 2020 2020 6465 6661  the.        defa
+0000b3e0: 756c 7420 6265 6861 7669 6f72 2069 6620  ult behavior if 
+0000b3f0: 6e6f 2047 6974 2072 6570 6f20 6973 2070  no Git repo is p
+0000b400: 726f 7669 6465 6420 6f72 2063 616e 2062  rovided or can b
+0000b410: 6520 666f 7263 6564 2076 6961 2074 6865  e forced via the
+0000b420: 0a20 2020 2020 2020 2060 6765 6e65 7261  .        `genera
+0000b430: 7465 5f6a 6f62 7360 2070 6172 616d 6574  te_jobs` paramet
+0000b440: 6572 2e0a 0a20 2020 2020 2020 2041 7267  er...        Arg
+0000b450: 733a 0a20 2020 2020 2020 2020 2020 2067  s:.            g
+0000b460: 656e 6572 6174 655f 6a6f 6273 2028 626f  enerate_jobs (bo
+0000b470: 6f6c 293a 2057 6865 7468 6572 2074 6f20  ol): Whether to 
+0000b480: 6765 6e65 7261 7465 206e 6577 2073 6c75  generate new slu
+0000b490: 726d 206a 6f62 2073 6372 6970 7473 0a20  rm job scripts. 
+0000b4a0: 2020 2020 2020 2020 2020 2020 2020 2049                 I
+0000b4b0: 4e53 5445 4144 2028 6f66 2070 756c 6c69  NSTEAD (of pulli
+0000b4c0: 6e67 2066 726f 6d20 6769 7429 2e20 4465  ng from git). De
+0000b4d0: 6661 756c 7473 2074 6f20 4661 6c73 652c  faults to False,
+0000b4e0: 2065 7863 6570 740a 2020 2020 2020 2020   except.        
+0000b4f0: 2020 2020 2020 2020 6966 206e 6f20 736c          if no sl
+0000b500: 7572 6d5f 7363 7269 7074 5f72 6570 6f20  urm_script_repo 
+0000b510: 6973 2063 6f6e 6669 6775 7265 642e 0a20  is configured.. 
+0000b520: 2020 2020 2020 2020 2020 2065 6e76 2028             env (
+0000b530: 4469 6374 5b73 7472 2c20 7374 725d 2c20  Dict[str, str], 
+0000b540: 6f70 7469 6f6e 616c 293a 204f 7074 696f  optional): Optio
+0000b550: 6e61 6c20 656e 7669 726f 6e6d 656e 7420  nal environment 
+0000b560: 7661 7269 6162 6c65 7320 0a20 2020 2020  variables .     
+0000b570: 2020 2020 2020 2020 2020 2074 6f20 7365             to se
+0000b580: 7420 7768 656e 2072 756e 6e69 6e67 2074  t when running t
+0000b590: 6865 2063 6f6d 6d61 6e64 2e20 4465 6661  he command. Defa
+0000b5a0: 756c 7473 2074 6f20 4e6f 6e65 2e0a 0a20  ults to None... 
+0000b5b0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+0000b5c0: 2020 2020 2020 2020 2020 2020 5265 7375              Resu
+0000b5d0: 6c74 3a20 5468 6520 7265 7375 6c74 206f  lt: The result o
+0000b5e0: 6620 7468 6520 636f 6d6d 616e 642e 0a20  f the command.. 
+0000b5f0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000b600: 2020 2069 6620 6e6f 7420 7365 6c66 2e73     if not self.s
+0000b610: 6c75 726d 5f73 6372 6970 745f 7265 706f  lurm_script_repo
+0000b620: 3a0a 2020 2020 2020 2020 2020 2020 6765  :.            ge
+0000b630: 6e65 7261 7465 5f6a 6f62 7320 3d20 5472  nerate_jobs = Tr
+0000b640: 7565 0a0a 2020 2020 2020 2020 6966 2067  ue..        if g
+0000b650: 656e 6572 6174 655f 6a6f 6273 3a0a 2020  enerate_jobs:.  
+0000b660: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
+0000b670: 2e69 6e66 6f28 2247 656e 6572 6174 696e  .info("Generatin
+0000b680: 6720 536c 7572 6d20 6a6f 6220 7363 7269  g Slurm job scri
+0000b690: 7074 7322 290a 2020 2020 2020 2020 2020  pts").          
+0000b6a0: 2020 666f 7220 7766 2c20 6a6f 625f 7061    for wf, job_pa
+0000b6b0: 7468 2069 6e20 7365 6c66 2e73 6c75 726d  th in self.slurm
+0000b6c0: 5f6d 6f64 656c 5f6a 6f62 732e 6974 656d  _model_jobs.item
+0000b6d0: 7328 293a 0a20 2020 2020 2020 2020 2020  s():.           
+0000b6e0: 2020 2020 2023 2067 656e 6572 6174 6520       # generate 
+0000b6f0: 6a6f 6220 7363 7269 7074 0a20 2020 2020  job script.     
+0000b700: 2020 2020 2020 2020 2020 2070 6172 616d             param
+0000b710: 7320 3d20 7365 6c66 2e67 6574 5f77 6f72  s = self.get_wor
+0000b720: 6b66 6c6f 775f 7061 7261 6d65 7465 7273  kflow_parameters
+0000b730: 2877 6629 0a20 2020 2020 2020 2020 2020  (wf).           
+0000b740: 2020 2020 2073 7562 7320 3d20 7365 6c66       subs = self
+0000b750: 2e77 6f72 6b66 6c6f 775f 7061 7261 6d73  .workflow_params
+0000b760: 5f74 6f5f 7375 6273 2870 6172 616d 7329  _to_subs(params)
+0000b770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b780: 206a 6f62 5f73 6372 6970 7420 3d20 7365   job_script = se
+0000b790: 6c66 2e67 656e 6572 6174 655f 736c 7572  lf.generate_slur
+0000b7a0: 6d5f 6a6f 625f 666f 725f 776f 726b 666c  m_job_for_workfl
+0000b7b0: 6f77 2877 662c 2073 7562 7329 0a20 2020  ow(wf, subs).   
+0000b7c0: 2020 2020 2020 2020 2020 2020 2023 2065               # e
+0000b7d0: 6e73 7572 6520 616c 6c20 6469 7273 2065  nsure all dirs e
+0000b7e0: 7869 7374 2072 656d 6f74 656c 790a 2020  xist remotely.  
+0000b7f0: 2020 2020 2020 2020 2020 2020 2020 6675                fu
+0000b800: 6c6c 5f70 6174 6820 3d20 7365 6c66 2e73  ll_path = self.s
+0000b810: 6c75 726d 5f73 6372 6970 745f 7061 7468  lurm_script_path
+0000b820: 2b22 2f22 2b6a 6f62 5f70 6174 680a 2020  +"/"+job_path.  
+0000b830: 2020 2020 2020 2020 2020 2020 2020 6a6f                jo
+0000b840: 625f 6469 722c 205f 203d 206f 732e 7061  b_dir, _ = os.pa
+0000b850: 7468 2e73 706c 6974 2866 756c 6c5f 7061  th.split(full_pa
+0000b860: 7468 290a 2020 2020 2020 2020 2020 2020  th).            
+0000b870: 2020 2020 7365 6c66 2e72 756e 2866 226d      self.run(f"m
+0000b880: 6b64 6972 202d 7020 5c22 7b6a 6f62 5f64  kdir -p \"{job_d
+0000b890: 6972 7d5c 2222 290a 2020 2020 2020 2020  ir}\"").        
+0000b8a0: 2020 2020 2020 2020 2320 636f 7079 2074          # copy t
+0000b8b0: 6f20 7265 6d6f 7465 2066 696c 650a 2020  o remote file.  
+0000b8c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000b8d0: 7375 6c74 203d 2073 656c 662e 7075 7428  sult = self.put(
+0000b8e0: 6c6f 6361 6c3d 696f 2e53 7472 696e 6749  local=io.StringI
+0000b8f0: 4f28 6a6f 625f 7363 7269 7074 292c 0a20  O(job_script),. 
 0000b900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000b910: 2020 2020 2020 2020 2020 2020 2072 656d               rem
-0000b920: 6f74 653d 6675 6c6c 5f70 6174 6829 0a20  ote=full_path). 
-0000b930: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-0000b940: 2020 2020 2020 2020 2063 6d64 203d 2073           cmd = s
-0000b950: 656c 662e 6765 745f 7570 6461 7465 5f73  elf.get_update_s
-0000b960: 6c75 726d 5f73 6372 6970 7473 5f63 6f6d  lurm_scripts_com
-0000b970: 6d61 6e64 2829 0a20 2020 2020 2020 2020  mand().         
-0000b980: 2020 206c 6f67 6765 722e 696e 666f 2822     logger.info("
-0000b990: 5570 6461 7469 6e67 2053 6c75 726d 206a  Updating Slurm j
-0000b9a0: 6f62 2073 6372 6970 7473 206f 6e20 536c  ob scripts on Sl
-0000b9b0: 7572 6d22 290a 2020 2020 2020 2020 2020  urm").          
-0000b9c0: 2020 7265 7375 6c74 203d 2073 656c 662e    result = self.
-0000b9d0: 7275 6e5f 636f 6d6d 616e 6473 285b 636d  run_commands([cm
-0000b9e0: 645d 2c20 656e 763d 656e 7629 0a20 2020  d], env=env).   
-0000b9f0: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-0000ba00: 6c74 0a0a 2020 2020 6465 6620 7275 6e5f  lt..    def run_
-0000ba10: 776f 726b 666c 6f77 2873 656c 662c 0a20  workflow(self,. 
-0000ba20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ba30: 2020 2020 776f 726b 666c 6f77 5f6e 616d      workflow_nam
-0000ba40: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
-0000ba50: 2020 2020 2020 2020 2020 2020 2077 6f72               wor
-0000ba60: 6b66 6c6f 775f 7665 7273 696f 6e3a 2073  kflow_version: s
-0000ba70: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
-0000ba80: 2020 2020 2020 2020 2069 6e70 7574 5f64           input_d
-0000ba90: 6174 613a 2073 7472 2c0a 2020 2020 2020  ata: str,.      
-0000baa0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000bab0: 6d61 696c 3a20 4f70 7469 6f6e 616c 5b73  mail: Optional[s
-0000bac0: 7472 5d20 3d20 4e6f 6e65 2c0a 2020 2020  tr] = None,.    
+0000b910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000b920: 2072 656d 6f74 653d 6675 6c6c 5f70 6174   remote=full_pat
+0000b930: 6829 0a20 2020 2020 2020 2065 6c73 653a  h).        else:
+0000b940: 0a20 2020 2020 2020 2020 2020 2063 6d64  .            cmd
+0000b950: 203d 2073 656c 662e 6765 745f 7570 6461   = self.get_upda
+0000b960: 7465 5f73 6c75 726d 5f73 6372 6970 7473  te_slurm_scripts
+0000b970: 5f63 6f6d 6d61 6e64 2829 0a20 2020 2020  _command().     
+0000b980: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+0000b990: 666f 2822 5570 6461 7469 6e67 2053 6c75  fo("Updating Slu
+0000b9a0: 726d 206a 6f62 2073 6372 6970 7473 206f  rm job scripts o
+0000b9b0: 6e20 536c 7572 6d22 290a 2020 2020 2020  n Slurm").      
+0000b9c0: 2020 2020 2020 7265 7375 6c74 203d 2073        result = s
+0000b9d0: 656c 662e 7275 6e5f 636f 6d6d 616e 6473  elf.run_commands
+0000b9e0: 285b 636d 645d 2c20 656e 763d 656e 7629  ([cmd], env=env)
+0000b9f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+0000ba00: 7265 7375 6c74 0a0a 2020 2020 6465 6620  result..    def 
+0000ba10: 7275 6e5f 776f 726b 666c 6f77 2873 656c  run_workflow(sel
+0000ba20: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+0000ba30: 2020 2020 2020 2020 776f 726b 666c 6f77          workflow
+0000ba40: 5f6e 616d 653a 2073 7472 2c0a 2020 2020  _name: str,.    
+0000ba50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ba60: 2077 6f72 6b66 6c6f 775f 7665 7273 696f   workflow_versio
+0000ba70: 6e3a 2073 7472 2c0a 2020 2020 2020 2020  n: str,.        
+0000ba80: 2020 2020 2020 2020 2020 2020 2069 6e70               inp
+0000ba90: 7574 5f64 6174 613a 2073 7472 2c0a 2020  ut_data: str,.  
+0000baa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bab0: 2020 2065 6d61 696c 3a20 4f70 7469 6f6e     email: Option
+0000bac0: 616c 5b73 7472 5d20 3d20 4e6f 6e65 2c0a  al[str] = None,.
 0000bad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bae0: 2074 696d 653a 204f 7074 696f 6e61 6c5b   time: Optional[
-0000baf0: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-0000bb00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb10: 2020 2a2a 6b77 6172 6773 0a20 2020 2020    **kwargs.     
+0000bae0: 2020 2020 2074 696d 653a 204f 7074 696f       time: Optio
+0000baf0: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+0000bb00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000bb10: 2020 2020 2020 2a2a 6b77 6172 6773 0a20        **kwargs. 
 0000bb20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bb30: 2920 2d3e 2054 7570 6c65 5b52 6573 756c  ) -> Tuple[Resul
-0000bb40: 742c 2069 6e74 5d3a 0a20 2020 2020 2020  t, int]:.       
-0000bb50: 2022 2222 0a20 2020 2020 2020 2052 756e   """.        Run
-0000bb60: 2061 2073 7065 6369 6669 6564 2077 6f72   a specified wor
-0000bb70: 6b66 6c6f 7720 6f6e 2053 6c75 726d 2075  kflow on Slurm u
-0000bb80: 7369 6e67 2074 6865 2067 6976 656e 2070  sing the given p
-0000bb90: 6172 616d 6574 6572 732e 0a0a 2020 2020  arameters...    
-0000bba0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000bbb0: 2020 2020 2020 776f 726b 666c 6f77 5f6e        workflow_n
-0000bbc0: 616d 6520 2873 7472 293a 204e 616d 6520  ame (str): Name 
-0000bbd0: 6f66 2074 6865 2077 6f72 6b66 6c6f 7720  of the workflow 
-0000bbe0: 746f 2065 7865 6375 7465 2e0a 2020 2020  to execute..    
-0000bbf0: 2020 2020 2020 2020 776f 726b 666c 6f77          workflow
-0000bc00: 5f76 6572 7369 6f6e 2028 7374 7229 3a20  _version (str): 
-0000bc10: 5665 7273 696f 6e20 6f66 2074 6865 2077  Version of the w
-0000bc20: 6f72 6b66 6c6f 7720 2869 6d61 6765 2076  orkflow (image v
-0000bc30: 6572 7369 6f6e 200a 2020 2020 2020 2020  ersion .        
-0000bc40: 2020 2020 2020 2020 6f6e 2053 6c75 726d          on Slurm
-0000bc50: 292e 0a20 2020 2020 2020 2020 2020 2069  )..            i
-0000bc60: 6e70 7574 5f64 6174 6120 2873 7472 293a  nput_data (str):
-0000bc70: 204e 616d 6520 6f66 2074 6865 2069 6e70   Name of the inp
-0000bc80: 7574 2064 6174 6120 666f 6c64 6572 2063  ut data folder c
-0000bc90: 6f6e 7461 696e 696e 6720 696e 7075 740a  ontaining input.
-0000bca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bcb0: 696d 6167 6520 6669 6c65 732e 0a20 2020  image files..   
-0000bcc0: 2020 2020 2020 2020 2065 6d61 696c 2028           email (
-0000bcd0: 7374 722c 206f 7074 696f 6e61 6c29 3a20  str, optional): 
-0000bce0: 456d 6169 6c20 6164 6472 6573 7320 666f  Email address fo
-0000bcf0: 7220 536c 7572 6d20 6a6f 6220 6e6f 7469  r Slurm job noti
-0000bd00: 6669 6361 7469 6f6e 732e 0a20 2020 2020  fications..     
-0000bd10: 2020 2020 2020 2074 696d 6520 2873 7472         time (str
-0000bd20: 2c20 6f70 7469 6f6e 616c 293a 2054 696d  , optional): Tim
-0000bd30: 6520 6c69 6d69 7420 666f 7220 7468 6520  e limit for the 
-0000bd40: 536c 7572 6d20 6a6f 6220 696e 2074 6865  Slurm job in the
-0000bd50: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-0000bd60: 2020 666f 726d 6174 2048 483a 4d4d 3a53    format HH:MM:S
-0000bd70: 532e 0a20 2020 2020 2020 2020 2020 202a  S..            *
-0000bd80: 2a6b 7761 7267 733a 2041 6464 6974 696f  *kwargs: Additio
-0000bd90: 6e61 6c20 6b65 7977 6f72 6420 6172 6775  nal keyword argu
-0000bda0: 6d65 6e74 7320 666f 7220 7468 6520 776f  ments for the wo
-0000bdb0: 726b 666c 6f77 2e0a 0a20 2020 2020 2020  rkflow...       
-0000bdc0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-0000bdd0: 2020 2020 2020 5475 706c 655b 5265 7375        Tuple[Resu
-0000bde0: 6c74 2c20 696e 745d 3a0a 2020 2020 2020  lt, int]:.      
-0000bdf0: 2020 2020 2020 2020 2020 4120 7475 706c            A tupl
-0000be00: 6520 636f 6e74 6169 6e69 6e67 2074 6865  e containing the
-0000be10: 2072 6573 756c 7420 6f66 2073 7461 7274   result of start
-0000be20: 696e 6720 7468 6520 776f 726b 666c 6f77  ing the workflow
-0000be30: 206a 6f62 2061 6e64 0a20 2020 2020 2020   job and.       
-0000be40: 2020 2020 2020 2020 2074 6865 2053 6c75           the Slu
-0000be50: 726d 206a 6f62 2049 442c 206f 7220 2d31  rm job ID, or -1
-0000be60: 2069 6620 7468 6520 6a6f 6220 4944 2063   if the job ID c
-0000be70: 6f75 6c64 206e 6f74 2062 6520 6578 7472  ould not be extr
-0000be80: 6163 7465 642e 0a0a 2020 2020 2020 2020  acted...        
-0000be90: 4e6f 7465 3a0a 2020 2020 2020 2020 2020  Note:.          
-0000bea0: 2020 5468 6520 536c 7572 6d20 6a6f 6220    The Slurm job 
-0000beb0: 4944 2069 7320 6578 7472 6163 7465 6420  ID is extracted 
-0000bec0: 6672 6f6d 2074 6865 2072 6573 756c 7420  from the result 
-0000bed0: 6f66 2074 6865 200a 2020 2020 2020 2020  of the .        
-0000bee0: 2020 2020 6072 756e 5f63 6f6d 6d61 6e64      `run_command
-0000bef0: 7360 206d 6574 686f 642e 0a20 2020 2020  s` method..     
-0000bf00: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
-0000bf10: 6261 7463 685f 636d 642c 2073 6261 7463  batch_cmd, sbatc
-0000bf20: 685f 656e 7620 3d20 7365 6c66 2e67 6574  h_env = self.get
-0000bf30: 5f77 6f72 6b66 6c6f 775f 636f 6d6d 616e  _workflow_comman
-0000bf40: 6428 0a20 2020 2020 2020 2020 2020 2077  d(.            w
-0000bf50: 6f72 6b66 6c6f 775f 6e61 6d65 2c20 776f  orkflow_name, wo
-0000bf60: 726b 666c 6f77 5f76 6572 7369 6f6e 2c20  rkflow_version, 
-0000bf70: 696e 7075 745f 6461 7461 2c20 656d 6169  input_data, emai
-0000bf80: 6c2c 2074 696d 652c 202a 2a6b 7761 7267  l, time, **kwarg
-0000bf90: 7329 0a20 2020 2020 2020 2070 7269 6e74  s).        print
-0000bfa0: 2866 2252 756e 6e69 6e67 207b 776f 726b  (f"Running {work
-0000bfb0: 666c 6f77 5f6e 616d 657d 206a 6f62 206f  flow_name} job o
-0000bfc0: 6e20 7b69 6e70 7574 5f64 6174 617d 206f  n {input_data} o
-0000bfd0: 6e20 536c 7572 6d3a 5c0a 2020 2020 2020  n Slurm:\.      
-0000bfe0: 2020 2020 2020 7b73 6261 7463 685f 636d        {sbatch_cm
-0000bff0: 647d 2077 2f20 7b73 6261 7463 685f 656e  d} w/ {sbatch_en
-0000c000: 767d 2229 0a20 2020 2020 2020 206c 6f67  v}").        log
-0000c010: 6765 722e 696e 666f 2866 2252 756e 6e69  ger.info(f"Runni
-0000c020: 6e67 207b 776f 726b 666c 6f77 5f6e 616d  ng {workflow_nam
-0000c030: 657d 206a 6f62 206f 6e20 7b69 6e70 7574  e} job on {input
-0000c040: 5f64 6174 617d 206f 6e20 536c 7572 6d22  _data} on Slurm"
-0000c050: 290a 2020 2020 2020 2020 7265 7320 3d20  ).        res = 
-0000c060: 7365 6c66 2e72 756e 5f63 6f6d 6d61 6e64  self.run_command
-0000c070: 7328 5b73 6261 7463 685f 636d 645d 2c20  s([sbatch_cmd], 
-0000c080: 7362 6174 6368 5f65 6e76 290a 2020 2020  sbatch_env).    
-0000c090: 2020 2020 7265 7475 726e 2072 6573 2c20      return res, 
-0000c0a0: 7365 6c66 2e65 7874 7261 6374 5f6a 6f62  self.extract_job
-0000c0b0: 5f69 6428 7265 7329 0a0a 2020 2020 6465  _id(res)..    de
-0000c0c0: 6620 7275 6e5f 776f 726b 666c 6f77 5f6a  f run_workflow_j
-0000c0d0: 6f62 2873 656c 662c 0a20 2020 2020 2020  ob(self,.       
+0000bb30: 2020 2020 2920 2d3e 2054 7570 6c65 5b52      ) -> Tuple[R
+0000bb40: 6573 756c 742c 2069 6e74 5d3a 0a20 2020  esult, int]:.   
+0000bb50: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000bb60: 2052 756e 2061 2073 7065 6369 6669 6564   Run a specified
+0000bb70: 2077 6f72 6b66 6c6f 7720 6f6e 2053 6c75   workflow on Slu
+0000bb80: 726d 2075 7369 6e67 2074 6865 2067 6976  rm using the giv
+0000bb90: 656e 2070 6172 616d 6574 6572 732e 0a0a  en parameters...
+0000bba0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0000bbb0: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
+0000bbc0: 6f77 5f6e 616d 6520 2873 7472 293a 204e  ow_name (str): N
+0000bbd0: 616d 6520 6f66 2074 6865 2077 6f72 6b66  ame of the workf
+0000bbe0: 6c6f 7720 746f 2065 7865 6375 7465 2e0a  low to execute..
+0000bbf0: 2020 2020 2020 2020 2020 2020 776f 726b              work
+0000bc00: 666c 6f77 5f76 6572 7369 6f6e 2028 7374  flow_version (st
+0000bc10: 7229 3a20 5665 7273 696f 6e20 6f66 2074  r): Version of t
+0000bc20: 6865 2077 6f72 6b66 6c6f 7720 2869 6d61  he workflow (ima
+0000bc30: 6765 2076 6572 7369 6f6e 200a 2020 2020  ge version .    
+0000bc40: 2020 2020 2020 2020 2020 2020 6f6e 2053              on S
+0000bc50: 6c75 726d 292e 0a20 2020 2020 2020 2020  lurm)..         
+0000bc60: 2020 2069 6e70 7574 5f64 6174 6120 2873     input_data (s
+0000bc70: 7472 293a 204e 616d 6520 6f66 2074 6865  tr): Name of the
+0000bc80: 2069 6e70 7574 2064 6174 6120 666f 6c64   input data fold
+0000bc90: 6572 2063 6f6e 7461 696e 696e 6720 696e  er containing in
+0000bca0: 7075 740a 2020 2020 2020 2020 2020 2020  put.            
+0000bcb0: 2020 2020 696d 6167 6520 6669 6c65 732e      image files.
+0000bcc0: 0a20 2020 2020 2020 2020 2020 2065 6d61  .            ema
+0000bcd0: 696c 2028 7374 722c 206f 7074 696f 6e61  il (str, optiona
+0000bce0: 6c29 3a20 456d 6169 6c20 6164 6472 6573  l): Email addres
+0000bcf0: 7320 666f 7220 536c 7572 6d20 6a6f 6220  s for Slurm job 
+0000bd00: 6e6f 7469 6669 6361 7469 6f6e 732e 0a20  notifications.. 
+0000bd10: 2020 2020 2020 2020 2020 2074 696d 6520             time 
+0000bd20: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
+0000bd30: 2054 696d 6520 6c69 6d69 7420 666f 7220   Time limit for 
+0000bd40: 7468 6520 536c 7572 6d20 6a6f 6220 696e  the Slurm job in
+0000bd50: 2074 6865 200a 2020 2020 2020 2020 2020   the .          
+0000bd60: 2020 2020 2020 666f 726d 6174 2048 483a        format HH:
+0000bd70: 4d4d 3a53 532e 0a20 2020 2020 2020 2020  MM:SS..         
+0000bd80: 2020 202a 2a6b 7761 7267 733a 2041 6464     **kwargs: Add
+0000bd90: 6974 696f 6e61 6c20 6b65 7977 6f72 6420  itional keyword 
+0000bda0: 6172 6775 6d65 6e74 7320 666f 7220 7468  arguments for th
+0000bdb0: 6520 776f 726b 666c 6f77 2e0a 0a20 2020  e workflow...   
+0000bdc0: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+0000bdd0: 2020 2020 2020 2020 2020 5475 706c 655b            Tuple[
+0000bde0: 5265 7375 6c74 2c20 696e 745d 3a0a 2020  Result, int]:.  
+0000bdf0: 2020 2020 2020 2020 2020 2020 2020 4120                A 
+0000be00: 7475 706c 6520 636f 6e74 6169 6e69 6e67  tuple containing
+0000be10: 2074 6865 2072 6573 756c 7420 6f66 2073   the result of s
+0000be20: 7461 7274 696e 6720 7468 6520 776f 726b  tarting the work
+0000be30: 666c 6f77 206a 6f62 2061 6e64 0a20 2020  flow job and.   
+0000be40: 2020 2020 2020 2020 2020 2020 2074 6865               the
+0000be50: 2053 6c75 726d 206a 6f62 2049 442c 206f   Slurm job ID, o
+0000be60: 7220 2d31 2069 6620 7468 6520 6a6f 6220  r -1 if the job 
+0000be70: 4944 2063 6f75 6c64 206e 6f74 2062 6520  ID could not be 
+0000be80: 6578 7472 6163 7465 642e 0a0a 2020 2020  extracted...    
+0000be90: 2020 2020 4e6f 7465 3a0a 2020 2020 2020      Note:.      
+0000bea0: 2020 2020 2020 5468 6520 536c 7572 6d20        The Slurm 
+0000beb0: 6a6f 6220 4944 2069 7320 6578 7472 6163  job ID is extrac
+0000bec0: 7465 6420 6672 6f6d 2074 6865 2072 6573  ted from the res
+0000bed0: 756c 7420 6f66 2074 6865 200a 2020 2020  ult of the .    
+0000bee0: 2020 2020 2020 2020 6072 756e 5f63 6f6d          `run_com
+0000bef0: 6d61 6e64 7360 206d 6574 686f 642e 0a20  mands` method.. 
+0000bf00: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+0000bf10: 2020 2073 6261 7463 685f 636d 642c 2073     sbatch_cmd, s
+0000bf20: 6261 7463 685f 656e 7620 3d20 7365 6c66  batch_env = self
+0000bf30: 2e67 6574 5f77 6f72 6b66 6c6f 775f 636f  .get_workflow_co
+0000bf40: 6d6d 616e 6428 0a20 2020 2020 2020 2020  mmand(.         
+0000bf50: 2020 2077 6f72 6b66 6c6f 775f 6e61 6d65     workflow_name
+0000bf60: 2c20 776f 726b 666c 6f77 5f76 6572 7369  , workflow_versi
+0000bf70: 6f6e 2c20 696e 7075 745f 6461 7461 2c20  on, input_data, 
+0000bf80: 656d 6169 6c2c 2074 696d 652c 202a 2a6b  email, time, **k
+0000bf90: 7761 7267 7329 0a20 2020 2020 2020 2070  wargs).        p
+0000bfa0: 7269 6e74 2866 2252 756e 6e69 6e67 207b  rint(f"Running {
+0000bfb0: 776f 726b 666c 6f77 5f6e 616d 657d 206a  workflow_name} j
+0000bfc0: 6f62 206f 6e20 7b69 6e70 7574 5f64 6174  ob on {input_dat
+0000bfd0: 617d 206f 6e20 536c 7572 6d3a 5c0a 2020  a} on Slurm:\.  
+0000bfe0: 2020 2020 2020 2020 2020 7b73 6261 7463            {sbatc
+0000bff0: 685f 636d 647d 2077 2f20 7b73 6261 7463  h_cmd} w/ {sbatc
+0000c000: 685f 656e 767d 2229 0a20 2020 2020 2020  h_env}").       
+0000c010: 206c 6f67 6765 722e 696e 666f 2866 2252   logger.info(f"R
+0000c020: 756e 6e69 6e67 207b 776f 726b 666c 6f77  unning {workflow
+0000c030: 5f6e 616d 657d 206a 6f62 206f 6e20 7b69  _name} job on {i
+0000c040: 6e70 7574 5f64 6174 617d 206f 6e20 536c  nput_data} on Sl
+0000c050: 7572 6d22 290a 2020 2020 2020 2020 7265  urm").        re
+0000c060: 7320 3d20 7365 6c66 2e72 756e 5f63 6f6d  s = self.run_com
+0000c070: 6d61 6e64 7328 5b73 6261 7463 685f 636d  mands([sbatch_cm
+0000c080: 645d 2c20 7362 6174 6368 5f65 6e76 290a  d], sbatch_env).
+0000c090: 2020 2020 2020 2020 7265 7475 726e 2072          return r
+0000c0a0: 6573 2c20 7365 6c66 2e65 7874 7261 6374  es, self.extract
+0000c0b0: 5f6a 6f62 5f69 6428 7265 7329 0a0a 2020  _job_id(res)..  
+0000c0c0: 2020 6465 6620 7275 6e5f 776f 726b 666c    def run_workfl
+0000c0d0: 6f77 5f6a 6f62 2873 656c 662c 0a20 2020  ow_job(self,.   
 0000c0e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c0f0: 2020 776f 726b 666c 6f77 5f6e 616d 653a    workflow_name:
-0000c100: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
-0000c110: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-0000c120: 6f72 6b66 6c6f 775f 7665 7273 696f 6e3a  orkflow_version:
-0000c130: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
-0000c140: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000c150: 6e70 7574 5f64 6174 613a 2073 7472 2c0a  nput_data: str,.
-0000c160: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c170: 2020 2020 2020 2020 2065 6d61 696c 3a20           email: 
-0000c180: 4f70 7469 6f6e 616c 5b73 7472 5d20 3d20  Optional[str] = 
-0000c190: 4e6f 6e65 2c0a 2020 2020 2020 2020 2020  None,.          
-0000c1a0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-0000c1b0: 696d 653a 204f 7074 696f 6e61 6c5b 7374  ime: Optional[st
-0000c1c0: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
+0000c0f0: 2020 2020 2020 776f 726b 666c 6f77 5f6e        workflow_n
+0000c100: 616d 653a 2073 7472 2c0a 2020 2020 2020  ame: str,.      
+0000c110: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c120: 2020 2077 6f72 6b66 6c6f 775f 7665 7273     workflow_vers
+0000c130: 696f 6e3a 2073 7472 2c0a 2020 2020 2020  ion: str,.      
+0000c140: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c150: 2020 2069 6e70 7574 5f64 6174 613a 2073     input_data: s
+0000c160: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
+0000c170: 2020 2020 2020 2020 2020 2020 2065 6d61               ema
+0000c180: 696c 3a20 4f70 7469 6f6e 616c 5b73 7472  il: Optional[str
+0000c190: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 2020  ] = None,.      
+0000c1a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000c1b0: 2020 2074 696d 653a 204f 7074 696f 6e61     time: Optiona
+0000c1c0: 6c5b 7374 725d 203d 204e 6f6e 652c 0a20  l[str] = None,. 
 0000c1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c1e0: 2020 2020 2a2a 6b77 6172 6773 0a20 2020      **kwargs.   
-0000c1f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c200: 2020 2020 2020 2920 2d3e 2053 6c75 726d        ) -> Slurm
-0000c210: 4a6f 623a 0a20 2020 2020 2020 2022 2222  Job:.        """
-0000c220: 0a20 2020 2020 2020 2052 756e 2061 2073  .        Run a s
-0000c230: 7065 6369 6669 6564 2077 6f72 6b66 6c6f  pecified workflo
-0000c240: 7720 6f6e 2053 6c75 726d 2075 7369 6e67  w on Slurm using
-0000c250: 2074 6865 2067 6976 656e 2070 6172 616d   the given param
-0000c260: 6574 6572 7320 616e 6420 7265 7475 726e  eters and return
-0000c270: 2061 2053 6c75 726d 4a6f 6220 696e 7374   a SlurmJob inst
-0000c280: 616e 6365 2e0a 0a20 2020 2020 2020 2041  ance...        A
-0000c290: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-0000c2a0: 2077 6f72 6b66 6c6f 775f 6e61 6d65 2028   workflow_name (
-0000c2b0: 7374 7229 3a20 4e61 6d65 206f 6620 7468  str): Name of th
-0000c2c0: 6520 776f 726b 666c 6f77 2074 6f20 6578  e workflow to ex
-0000c2d0: 6563 7574 652e 0a20 2020 2020 2020 2020  ecute..         
-0000c2e0: 2020 2077 6f72 6b66 6c6f 775f 7665 7273     workflow_vers
-0000c2f0: 696f 6e20 2873 7472 293a 2056 6572 7369  ion (str): Versi
-0000c300: 6f6e 206f 6620 7468 6520 776f 726b 666c  on of the workfl
-0000c310: 6f77 2028 696d 6167 6520 7665 7273 696f  ow (image versio
-0000c320: 6e20 6f6e 2053 6c75 726d 292e 0a20 2020  n on Slurm)..   
-0000c330: 2020 2020 2020 2020 2069 6e70 7574 5f64           input_d
-0000c340: 6174 6120 2873 7472 293a 204e 616d 6520  ata (str): Name 
-0000c350: 6f66 2074 6865 2069 6e70 7574 2064 6174  of the input dat
-0000c360: 6120 666f 6c64 6572 2063 6f6e 7461 696e  a folder contain
-0000c370: 696e 6720 696e 7075 7420 696d 6167 6520  ing input image 
-0000c380: 6669 6c65 732e 0a20 2020 2020 2020 2020  files..         
-0000c390: 2020 2065 6d61 696c 2028 7374 722c 206f     email (str, o
-0000c3a0: 7074 696f 6e61 6c29 3a20 456d 6169 6c20  ptional): Email 
-0000c3b0: 6164 6472 6573 7320 666f 7220 536c 7572  address for Slur
-0000c3c0: 6d20 6a6f 6220 6e6f 7469 6669 6361 7469  m job notificati
-0000c3d0: 6f6e 732e 0a20 2020 2020 2020 2020 2020  ons..           
-0000c3e0: 2074 696d 6520 2873 7472 2c20 6f70 7469   time (str, opti
-0000c3f0: 6f6e 616c 293a 2054 696d 6520 6c69 6d69  onal): Time limi
-0000c400: 7420 666f 7220 7468 6520 536c 7572 6d20  t for the Slurm 
-0000c410: 6a6f 6220 696e 2074 6865 2066 6f72 6d61  job in the forma
-0000c420: 7420 4848 3a4d 4d3a 5353 2e0a 2020 2020  t HH:MM:SS..    
-0000c430: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
-0000c440: 3a20 4164 6469 7469 6f6e 616c 206b 6579  : Additional key
-0000c450: 776f 7264 2061 7267 756d 656e 7473 2066  word arguments f
-0000c460: 6f72 2074 6865 2077 6f72 6b66 6c6f 772e  or the workflow.
-0000c470: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-0000c480: 733a 0a20 2020 2020 2020 2020 2020 2053  s:.            S
-0000c490: 6c75 726d 4a6f 623a 2041 2053 6c75 726d  lurmJob: A Slurm
-0000c4a0: 4a6f 6220 696e 7374 616e 6365 2072 6570  Job instance rep
-0000c4b0: 7265 7365 6e74 696e 6720 7468 6520 7374  resenting the st
-0000c4c0: 6172 7465 6420 776f 726b 666c 6f77 206a  arted workflow j
-0000c4d0: 6f62 2e0a 2020 2020 2020 2020 2222 220a  ob..        """.
-0000c4e0: 2020 2020 2020 2020 7265 7375 6c74 2c20          result, 
-0000c4f0: 6a6f 625f 6964 203d 2073 656c 662e 7275  job_id = self.ru
-0000c500: 6e5f 776f 726b 666c 6f77 280a 2020 2020  n_workflow(.    
-0000c510: 2020 2020 2020 2020 776f 726b 666c 6f77          workflow
-0000c520: 5f6e 616d 652c 2077 6f72 6b66 6c6f 775f  _name, workflow_
-0000c530: 7665 7273 696f 6e2c 2069 6e70 7574 5f64  version, input_d
-0000c540: 6174 612c 2065 6d61 696c 2c20 7469 6d65  ata, email, time
-0000c550: 2c20 2a2a 6b77 6172 6773 290a 2020 2020  , **kwargs).    
-0000c560: 2020 2020 7265 7475 726e 2053 6c75 726d      return Slurm
-0000c570: 4a6f 6228 7265 7375 6c74 2c20 6a6f 625f  Job(result, job_
-0000c580: 6964 290a 0a20 2020 2064 6566 2072 756e  id)..    def run
-0000c590: 5f63 6f6e 7665 7273 696f 6e5f 776f 726b  _conversion_work
-0000c5a0: 666c 6f77 5f6a 6f62 2873 656c 662c 2066  flow_job(self, f
-0000c5b0: 6f6c 6465 725f 6e61 6d65 3a20 7374 722c  older_name: str,
-0000c5c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c1e0: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
+0000c1f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000c200: 2020 2020 2020 2020 2020 2920 2d3e 2053            ) -> S
+0000c210: 6c75 726d 4a6f 623a 0a20 2020 2020 2020  lurmJob:.       
+0000c220: 2022 2222 0a20 2020 2020 2020 2052 756e   """.        Run
+0000c230: 2061 2073 7065 6369 6669 6564 2077 6f72   a specified wor
+0000c240: 6b66 6c6f 7720 6f6e 2053 6c75 726d 2075  kflow on Slurm u
+0000c250: 7369 6e67 2074 6865 2067 6976 656e 2070  sing the given p
+0000c260: 6172 616d 6574 6572 7320 616e 6420 7265  arameters and re
+0000c270: 7475 726e 2061 2053 6c75 726d 4a6f 6220  turn a SlurmJob 
+0000c280: 696e 7374 616e 6365 2e0a 0a20 2020 2020  instance...     
+0000c290: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000c2a0: 2020 2020 2077 6f72 6b66 6c6f 775f 6e61       workflow_na
+0000c2b0: 6d65 2028 7374 7229 3a20 4e61 6d65 206f  me (str): Name o
+0000c2c0: 6620 7468 6520 776f 726b 666c 6f77 2074  f the workflow t
+0000c2d0: 6f20 6578 6563 7574 652e 0a20 2020 2020  o execute..     
+0000c2e0: 2020 2020 2020 2077 6f72 6b66 6c6f 775f         workflow_
+0000c2f0: 7665 7273 696f 6e20 2873 7472 293a 2056  version (str): V
+0000c300: 6572 7369 6f6e 206f 6620 7468 6520 776f  ersion of the wo
+0000c310: 726b 666c 6f77 2028 696d 6167 6520 7665  rkflow (image ve
+0000c320: 7273 696f 6e20 6f6e 2053 6c75 726d 292e  rsion on Slurm).
+0000c330: 0a20 2020 2020 2020 2020 2020 2069 6e70  .            inp
+0000c340: 7574 5f64 6174 6120 2873 7472 293a 204e  ut_data (str): N
+0000c350: 616d 6520 6f66 2074 6865 2069 6e70 7574  ame of the input
+0000c360: 2064 6174 6120 666f 6c64 6572 2063 6f6e   data folder con
+0000c370: 7461 696e 696e 6720 696e 7075 7420 696d  taining input im
+0000c380: 6167 6520 6669 6c65 732e 0a20 2020 2020  age files..     
+0000c390: 2020 2020 2020 2065 6d61 696c 2028 7374         email (st
+0000c3a0: 722c 206f 7074 696f 6e61 6c29 3a20 456d  r, optional): Em
+0000c3b0: 6169 6c20 6164 6472 6573 7320 666f 7220  ail address for 
+0000c3c0: 536c 7572 6d20 6a6f 6220 6e6f 7469 6669  Slurm job notifi
+0000c3d0: 6361 7469 6f6e 732e 0a20 2020 2020 2020  cations..       
+0000c3e0: 2020 2020 2074 696d 6520 2873 7472 2c20       time (str, 
+0000c3f0: 6f70 7469 6f6e 616c 293a 2054 696d 6520  optional): Time 
+0000c400: 6c69 6d69 7420 666f 7220 7468 6520 536c  limit for the Sl
+0000c410: 7572 6d20 6a6f 6220 696e 2074 6865 2066  urm job in the f
+0000c420: 6f72 6d61 7420 4848 3a4d 4d3a 5353 2e0a  ormat HH:MM:SS..
+0000c430: 2020 2020 2020 2020 2020 2020 2a2a 6b77              **kw
+0000c440: 6172 6773 3a20 4164 6469 7469 6f6e 616c  args: Additional
+0000c450: 206b 6579 776f 7264 2061 7267 756d 656e   keyword argumen
+0000c460: 7473 2066 6f72 2074 6865 2077 6f72 6b66  ts for the workf
+0000c470: 6c6f 772e 0a0a 2020 2020 2020 2020 5265  low...        Re
+0000c480: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+0000c490: 2020 2053 6c75 726d 4a6f 623a 2041 2053     SlurmJob: A S
+0000c4a0: 6c75 726d 4a6f 6220 696e 7374 616e 6365  lurmJob instance
+0000c4b0: 2072 6570 7265 7365 6e74 696e 6720 7468   representing th
+0000c4c0: 6520 7374 6172 7465 6420 776f 726b 666c  e started workfl
+0000c4d0: 6f77 206a 6f62 2e0a 2020 2020 2020 2020  ow job..        
+0000c4e0: 2222 220a 2020 2020 2020 2020 7265 7375  """.        resu
+0000c4f0: 6c74 2c20 6a6f 625f 6964 203d 2073 656c  lt, job_id = sel
+0000c500: 662e 7275 6e5f 776f 726b 666c 6f77 280a  f.run_workflow(.
+0000c510: 2020 2020 2020 2020 2020 2020 776f 726b              work
+0000c520: 666c 6f77 5f6e 616d 652c 2077 6f72 6b66  flow_name, workf
+0000c530: 6c6f 775f 7665 7273 696f 6e2c 2069 6e70  low_version, inp
+0000c540: 7574 5f64 6174 612c 2065 6d61 696c 2c20  ut_data, email, 
+0000c550: 7469 6d65 2c20 2a2a 6b77 6172 6773 290a  time, **kwargs).
+0000c560: 2020 2020 2020 2020 7265 7475 726e 2053          return S
+0000c570: 6c75 726d 4a6f 6228 7265 7375 6c74 2c20  lurmJob(result, 
+0000c580: 6a6f 625f 6964 290a 0a20 2020 2064 6566  job_id)..    def
+0000c590: 2072 756e 5f63 6f6e 7665 7273 696f 6e5f   run_conversion_
+0000c5a0: 776f 726b 666c 6f77 5f6a 6f62 2873 656c  workflow_job(sel
+0000c5b0: 662c 2066 6f6c 6465 725f 6e61 6d65 3a20  f, folder_name: 
+0000c5c0: 7374 722c 0a20 2020 2020 2020 2020 2020  str,.           
 0000c5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c5e0: 2020 2020 2073 6f75 7263 655f 666f 726d       source_form
-0000c5f0: 6174 3a20 7374 7220 3d20 277a 6172 7227  at: str = 'zarr'
-0000c600: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000c5e0: 2020 2020 2020 2020 2073 6f75 7263 655f           source_
+0000c5f0: 666f 726d 6174 3a20 7374 7220 3d20 277a  format: str = 'z
+0000c600: 6172 7227 2c0a 2020 2020 2020 2020 2020  arr',.          
 0000c610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c620: 2020 2020 2020 7461 7267 6574 5f66 6f72        target_for
-0000c630: 6d61 743a 2073 7472 203d 2027 7469 6666  mat: str = 'tiff
-0000c640: 270a 2020 2020 2020 2020 2020 2020 2020  '.              
+0000c620: 2020 2020 2020 2020 2020 7461 7267 6574            target
+0000c630: 5f66 6f72 6d61 743a 2073 7472 203d 2027  _format: str = '
+0000c640: 7469 6666 270a 2020 2020 2020 2020 2020  tiff'.          
 0000c650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000c660: 2020 2020 2020 2920 2d3e 2054 7570 6c65        ) -> Tuple
-0000c670: 5b52 6573 756c 742c 2069 6e74 5d3a 0a20  [Result, int]:. 
-0000c680: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000c690: 2020 2052 756e 2074 6865 2064 6174 6120     Run the data 
-0000c6a0: 636f 6e76 6572 7369 6f6e 2077 6f72 6b66  conversion workf
-0000c6b0: 6c6f 7720 6f6e 2053 6c75 726d 2075 7369  low on Slurm usi
-0000c6c0: 6e67 2074 6865 2067 6976 656e 2064 6174  ng the given dat
-0000c6d0: 6120 666f 6c64 6572 2e0a 0a20 2020 2020  a folder...     
-0000c6e0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-0000c6f0: 2020 2020 2066 6f6c 6465 725f 6e61 6d65       folder_name
-0000c700: 2028 7374 7229 3a20 5468 6520 6e61 6d65   (str): The name
-0000c710: 206f 6620 7468 6520 6461 7461 2066 6f6c   of the data fol
-0000c720: 6465 7220 636f 6e74 6169 6e69 6e67 2073  der containing s
-0000c730: 6f75 7263 6520 666f 726d 6174 2066 696c  ource format fil
-0000c740: 6573 2e0a 2020 2020 2020 2020 2020 2020  es..            
-0000c750: 736f 7572 6365 5f66 6f72 6d61 7420 2873  source_format (s
-0000c760: 7472 293a 2053 6f75 7263 6520 6461 7461  tr): Source data
-0000c770: 2066 6f72 6d61 7420 666f 7220 636f 6e76   format for conv
-0000c780: 6572 7369 6f6e 2028 6465 6661 756c 7420  ersion (default 
-0000c790: 6973 2027 7a61 7272 2729 2e0a 2020 2020  is 'zarr')..    
-0000c7a0: 2020 2020 2020 2020 7461 7267 6574 5f66          target_f
-0000c7b0: 6f72 6d61 7420 2873 7472 293a 2054 6172  ormat (str): Tar
-0000c7c0: 6765 7420 6461 7461 2066 6f72 6d61 7420  get data format 
-0000c7d0: 6166 7465 7220 636f 6e76 6572 7369 6f6e  after conversion
-0000c7e0: 2028 6465 6661 756c 7420 6973 2027 7469   (default is 'ti
-0000c7f0: 6666 2729 2e0a 0a20 2020 2020 2020 2052  ff')...        R
-0000c800: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-0000c810: 2020 2020 5475 706c 655b 5265 7375 6c74      Tuple[Result
-0000c820: 2c20 696e 745d 3a0a 2020 2020 2020 2020  , int]:.        
-0000c830: 2020 2020 2020 2020 4120 7475 706c 6520          A tuple 
-0000c840: 636f 6e74 6169 6e69 6e67 2074 6865 2072  containing the r
-0000c850: 6573 756c 7420 6f66 2073 7461 7274 696e  esult of startin
-0000c860: 6720 7468 6520 636f 6e76 6572 7369 6f6e  g the conversion
-0000c870: 206a 6f62 2061 6e64 0a20 2020 2020 2020   job and.       
-0000c880: 2020 2020 2020 2020 2074 6865 2053 6c75           the Slu
-0000c890: 726d 206a 6f62 2049 442c 206f 7220 2d31  rm job ID, or -1
-0000c8a0: 2069 6620 7468 6520 6a6f 6220 4944 2063   if the job ID c
-0000c8b0: 6f75 6c64 206e 6f74 2062 6520 6578 7472  ould not be extr
-0000c8c0: 6163 7465 642e 0a0a 2020 2020 2020 2020  acted...        
-0000c8d0: 5761 726e 696e 673a 0a20 2020 2020 2020  Warning:.       
-0000c8e0: 2020 2020 2054 6865 2064 6566 6175 6c74       The default
-0000c8f0: 2069 6d70 6c65 6d65 6e74 6174 696f 6e20   implementation 
-0000c900: 6f6e 6c79 2073 7570 706f 7274 7320 636f  only supports co
-0000c910: 6e76 6572 7369 6f6e 2066 726f 6d20 277a  nversion from 'z
-0000c920: 6172 7227 2074 6f20 2774 6966 6627 2e0a  arr' to 'tiff'..
-0000c930: 2020 2020 2020 2020 2020 2020 4966 2075              If u
-0000c940: 7369 6e67 206f 7468 6572 2073 6f75 7263  sing other sourc
-0000c950: 6520 6f72 2074 6172 6765 7420 666f 726d  e or target form
-0000c960: 6174 732c 2075 7365 7273 206d 7573 7420  ats, users must 
-0000c970: 696d 706c 656d 656e 7420 616e 6420 636f  implement and co
-0000c980: 6e66 6967 7572 650a 2020 2020 2020 2020  nfigure.        
-0000c990: 2020 2020 6164 6469 7469 6f6e 616c 2063      additional c
-0000c9a0: 6f6e 7665 7274 6572 7320 7468 656d 7365  onverters themse
-0000c9b0: 6c76 6573 2e0a 2020 2020 2020 2020 2222  lves..        ""
-0000c9c0: 220a 2020 2020 2020 2020 2320 4765 6e65  ".        # Gene
-0000c9d0: 7261 7465 2061 2075 6e69 7175 6520 636f  rate a unique co
-0000c9e0: 6e66 6967 2066 696c 6520 6e61 6d65 0a20  nfig file name. 
-0000c9f0: 2020 2020 2020 2063 6f6e 6669 675f 6669         config_fi
-0000ca00: 6c65 203d 2066 2263 6f6e 6669 675f 7b66  le = f"config_{f
-0000ca10: 6f6c 6465 725f 6e61 6d65 7d2e 7478 7422  older_name}.txt"
-0000ca20: 0a0a 2020 2020 2020 2020 2320 436f 6e73  ..        # Cons
-0000ca30: 7472 7563 7420 616c 6c20 636f 6d6d 616e  truct all comman
-0000ca40: 6473 2074 6f20 7275 6e20 636f 6e73 6563  ds to run consec
-0000ca50: 7574 6976 656c 790a 2020 2020 2020 2020  utively.        
-0000ca60: 6461 7461 5f70 6174 6820 3d20 6622 7b73  data_path = f"{s
-0000ca70: 656c 662e 736c 7572 6d5f 6461 7461 5f70  elf.slurm_data_p
-0000ca80: 6174 687d 2f7b 666f 6c64 6572 5f6e 616d  ath}/{folder_nam
-0000ca90: 657d 220a 2020 2020 2020 2020 636f 6e76  e}".        conv
-0000caa0: 6572 7369 6f6e 5f63 6d64 2c20 7362 6174  ersion_cmd, sbat
-0000cab0: 6368 5f65 6e76 203d 2073 656c 662e 6765  ch_env = self.ge
-0000cac0: 745f 636f 6e76 6572 7369 6f6e 5f63 6f6d  t_conversion_com
-0000cad0: 6d61 6e64 280a 2020 2020 2020 2020 2020  mand(.          
-0000cae0: 2020 6461 7461 5f70 6174 682c 2063 6f6e    data_path, con
-0000caf0: 6669 675f 6669 6c65 2c20 736f 7572 6365  fig_file, source
-0000cb00: 5f66 6f72 6d61 742c 2074 6172 6765 745f  _format, target_
-0000cb10: 666f 726d 6174 290a 2020 2020 2020 2020  format).        
-0000cb20: 636f 6d6d 616e 6473 203d 205b 0a20 2020  commands = [.   
-0000cb30: 2020 2020 2020 2020 2066 2266 696e 6420           f"find 
-0000cb40: 5c22 7b64 6174 615f 7061 7468 7d2f 6461  \"{data_path}/da
-0000cb50: 7461 2f69 6e5c 2220 2d6e 616d 6520 5c22  ta/in\" -name \"
-0000cb60: 2a2e 7b73 6f75 7263 655f 666f 726d 6174  *.{source_format
-0000cb70: 7d5c 2220 7c20 6177 6b20 277b 7b70 7269  }\" | awk '{{pri
-0000cb80: 6e74 204e 522c 2024 307d 7d27 203e 205c  nt NR, $0}}' > \
-0000cb90: 227b 636f 6e66 6967 5f66 696c 657d 5c22  "{config_file}\"
-0000cba0: 222c 0a20 2020 2020 2020 2020 2020 2066  ",.            f
-0000cbb0: 224e 3d24 2877 6320 2d6c 203c 205c 227b  "N=$(wc -l < \"{
-0000cbc0: 636f 6e66 6967 5f66 696c 657d 5c22 2922  config_file}\")"
-0000cbd0: 2c0a 2020 2020 2020 2020 2020 2020 6622  ,.            f"
-0000cbe0: 6563 686f 205c 224e 756d 6265 7220 6f66  echo \"Number of
-0000cbf0: 202e 7b73 6f75 7263 655f 666f 726d 6174   .{source_format
-0000cc00: 7d20 6669 6c65 733a 2024 4e5c 2222 2c0a  } files: $N\"",.
-0000cc10: 2020 2020 2020 2020 2020 2020 636f 6e76              conv
-0000cc20: 6572 7369 6f6e 5f63 6d64 0a20 2020 2020  ersion_cmd.     
-0000cc30: 2020 205d 0a0a 2020 2020 2020 2020 2320     ]..        # 
-0000cc40: 5275 6e20 616c 6c20 636f 6d6d 616e 6473  Run all commands
-0000cc50: 2063 6f6e 7365 6375 7469 7665 6c79 0a20   consecutively. 
-0000cc60: 2020 2020 2020 2072 6573 203d 2073 656c         res = sel
-0000cc70: 662e 7275 6e5f 636f 6d6d 616e 6473 2863  f.run_commands(c
-0000cc80: 6f6d 6d61 6e64 732c 2073 6261 7463 685f  ommands, sbatch_
-0000cc90: 656e 7629 0a0a 2020 2020 2020 2020 7265  env)..        re
-0000cca0: 7475 726e 2053 6c75 726d 4a6f 6228 7265  turn SlurmJob(re
-0000ccb0: 732c 2073 656c 662e 6578 7472 6163 745f  s, self.extract_
-0000ccc0: 6a6f 625f 6964 2872 6573 2929 0a0a 2020  job_id(res))..  
-0000ccd0: 2020 6465 6620 6578 7472 6163 745f 6a6f    def extract_jo
-0000cce0: 625f 6964 2873 656c 662c 2072 6573 756c  b_id(self, resul
-0000ccf0: 743a 2052 6573 756c 7429 202d 3e20 696e  t: Result) -> in
-0000cd00: 743a 0a20 2020 2020 2020 2022 2222 0a20  t:.        """. 
-0000cd10: 2020 2020 2020 2045 7874 7261 6374 2074         Extract t
-0000cd20: 6865 2053 6c75 726d 206a 6f62 2049 4420  he Slurm job ID 
-0000cd30: 6672 6f6d 2074 6865 2072 6573 756c 7420  from the result 
-0000cd40: 6f66 2061 2063 6f6d 6d61 6e64 2e0a 0a20  of a command... 
-0000cd50: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-0000cd60: 2020 2020 2020 2020 2072 6573 756c 7420           result 
-0000cd70: 2852 6573 756c 7429 3a20 5468 6520 7265  (Result): The re
-0000cd80: 7375 6c74 206f 6620 6120 636f 6d6d 616e  sult of a comman
-0000cd90: 6420 6578 6563 7574 696f 6e2e 0a0a 2020  d execution...  
-0000cda0: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-0000cdb0: 2020 2020 2020 2020 2020 2069 6e74 3a0a             int:.
-0000cdc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cdd0: 5468 6520 536c 7572 6d20 6a6f 6220 4944  The Slurm job ID
-0000cde0: 2065 7874 7261 6374 6564 2066 726f 6d20   extracted from 
-0000cdf0: 7468 6520 7265 7375 6c74 2c0a 2020 2020  the result,.    
-0000ce00: 2020 2020 2020 2020 2020 2020 6f72 202d              or -
-0000ce10: 3120 6966 206e 6f74 2066 6f75 6e64 2e0a  1 if not found..
-0000ce20: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000ce30: 2020 2020 736c 7572 6d5f 6a6f 625f 6964      slurm_job_id
-0000ce40: 203d 206e 6578 7428 2869 6e74 2873 2e73   = next((int(s.s
-0000ce50: 7472 6970 2829 2920 666f 7220 7320 696e  trip()) for s in
-0000ce60: 2072 6573 756c 742e 7374 646f 7574 2e73   result.stdout.s
-0000ce70: 706c 6974 280a 2020 2020 2020 2020 2020  plit(.          
+0000c660: 2020 2020 2020 2020 2020 2920 2d3e 2054            ) -> T
+0000c670: 7570 6c65 5b52 6573 756c 742c 2069 6e74  uple[Result, int
+0000c680: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
+0000c690: 2020 2020 2020 2052 756e 2074 6865 2064         Run the d
+0000c6a0: 6174 6120 636f 6e76 6572 7369 6f6e 2077  ata conversion w
+0000c6b0: 6f72 6b66 6c6f 7720 6f6e 2053 6c75 726d  orkflow on Slurm
+0000c6c0: 2075 7369 6e67 2074 6865 2067 6976 656e   using the given
+0000c6d0: 2064 6174 6120 666f 6c64 6572 2e0a 0a20   data folder... 
+0000c6e0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+0000c6f0: 2020 2020 2020 2020 2066 6f6c 6465 725f           folder_
+0000c700: 6e61 6d65 2028 7374 7229 3a20 5468 6520  name (str): The 
+0000c710: 6e61 6d65 206f 6620 7468 6520 6461 7461  name of the data
+0000c720: 2066 6f6c 6465 7220 636f 6e74 6169 6e69   folder containi
+0000c730: 6e67 2073 6f75 7263 6520 666f 726d 6174  ng source format
+0000c740: 2066 696c 6573 2e0a 2020 2020 2020 2020   files..        
+0000c750: 2020 2020 736f 7572 6365 5f66 6f72 6d61      source_forma
+0000c760: 7420 2873 7472 293a 2053 6f75 7263 6520  t (str): Source 
+0000c770: 6461 7461 2066 6f72 6d61 7420 666f 7220  data format for 
+0000c780: 636f 6e76 6572 7369 6f6e 2028 6465 6661  conversion (defa
+0000c790: 756c 7420 6973 2027 7a61 7272 2729 2e0a  ult is 'zarr')..
+0000c7a0: 2020 2020 2020 2020 2020 2020 7461 7267              targ
+0000c7b0: 6574 5f66 6f72 6d61 7420 2873 7472 293a  et_format (str):
+0000c7c0: 2054 6172 6765 7420 6461 7461 2066 6f72   Target data for
+0000c7d0: 6d61 7420 6166 7465 7220 636f 6e76 6572  mat after conver
+0000c7e0: 7369 6f6e 2028 6465 6661 756c 7420 6973  sion (default is
+0000c7f0: 2027 7469 6666 2729 2e0a 0a20 2020 2020   'tiff')...     
+0000c800: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+0000c810: 2020 2020 2020 2020 5475 706c 655b 5265          Tuple[Re
+0000c820: 7375 6c74 2c20 696e 745d 3a0a 2020 2020  sult, int]:.    
+0000c830: 2020 2020 2020 2020 2020 2020 4120 7475              A tu
+0000c840: 706c 6520 636f 6e74 6169 6e69 6e67 2074  ple containing t
+0000c850: 6865 2072 6573 756c 7420 6f66 2073 7461  he result of sta
+0000c860: 7274 696e 6720 7468 6520 636f 6e76 6572  rting the conver
+0000c870: 7369 6f6e 206a 6f62 2061 6e64 0a20 2020  sion job and.   
+0000c880: 2020 2020 2020 2020 2020 2020 2074 6865               the
+0000c890: 2053 6c75 726d 206a 6f62 2049 442c 206f   Slurm job ID, o
+0000c8a0: 7220 2d31 2069 6620 7468 6520 6a6f 6220  r -1 if the job 
+0000c8b0: 4944 2063 6f75 6c64 206e 6f74 2062 6520  ID could not be 
+0000c8c0: 6578 7472 6163 7465 642e 0a0a 2020 2020  extracted...    
+0000c8d0: 2020 2020 5761 726e 696e 673a 0a20 2020      Warning:.   
+0000c8e0: 2020 2020 2020 2020 2054 6865 2064 6566           The def
+0000c8f0: 6175 6c74 2069 6d70 6c65 6d65 6e74 6174  ault implementat
+0000c900: 696f 6e20 6f6e 6c79 2073 7570 706f 7274  ion only support
+0000c910: 7320 636f 6e76 6572 7369 6f6e 2066 726f  s conversion fro
+0000c920: 6d20 277a 6172 7227 2074 6f20 2774 6966  m 'zarr' to 'tif
+0000c930: 6627 2e0a 2020 2020 2020 2020 2020 2020  f'..            
+0000c940: 4966 2075 7369 6e67 206f 7468 6572 2073  If using other s
+0000c950: 6f75 7263 6520 6f72 2074 6172 6765 7420  ource or target 
+0000c960: 666f 726d 6174 732c 2075 7365 7273 206d  formats, users m
+0000c970: 7573 7420 696d 706c 656d 656e 7420 616e  ust implement an
+0000c980: 6420 636f 6e66 6967 7572 650a 2020 2020  d configure.    
+0000c990: 2020 2020 2020 2020 6164 6469 7469 6f6e          addition
+0000c9a0: 616c 2063 6f6e 7665 7274 6572 7320 7468  al converters th
+0000c9b0: 656d 7365 6c76 6573 2e0a 2020 2020 2020  emselves..      
+0000c9c0: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
+0000c9d0: 4765 6e65 7261 7465 2061 2075 6e69 7175  Generate a uniqu
+0000c9e0: 6520 636f 6e66 6967 2066 696c 6520 6e61  e config file na
+0000c9f0: 6d65 0a20 2020 2020 2020 2063 6f6e 6669  me.        confi
+0000ca00: 675f 6669 6c65 203d 2066 2263 6f6e 6669  g_file = f"confi
+0000ca10: 675f 7b66 6f6c 6465 725f 6e61 6d65 7d2e  g_{folder_name}.
+0000ca20: 7478 7422 0a0a 2020 2020 2020 2020 2320  txt"..        # 
+0000ca30: 436f 6e73 7472 7563 7420 616c 6c20 636f  Construct all co
+0000ca40: 6d6d 616e 6473 2074 6f20 7275 6e20 636f  mmands to run co
+0000ca50: 6e73 6563 7574 6976 656c 790a 2020 2020  nsecutively.    
+0000ca60: 2020 2020 6461 7461 5f70 6174 6820 3d20      data_path = 
+0000ca70: 6622 7b73 656c 662e 736c 7572 6d5f 6461  f"{self.slurm_da
+0000ca80: 7461 5f70 6174 687d 2f7b 666f 6c64 6572  ta_path}/{folder
+0000ca90: 5f6e 616d 657d 220a 2020 2020 2020 2020  _name}".        
+0000caa0: 636f 6e76 6572 7369 6f6e 5f63 6d64 2c20  conversion_cmd, 
+0000cab0: 7362 6174 6368 5f65 6e76 203d 2073 656c  sbatch_env = sel
+0000cac0: 662e 6765 745f 636f 6e76 6572 7369 6f6e  f.get_conversion
+0000cad0: 5f63 6f6d 6d61 6e64 280a 2020 2020 2020  _command(.      
+0000cae0: 2020 2020 2020 6461 7461 5f70 6174 682c        data_path,
+0000caf0: 2063 6f6e 6669 675f 6669 6c65 2c20 736f   config_file, so
+0000cb00: 7572 6365 5f66 6f72 6d61 742c 2074 6172  urce_format, tar
+0000cb10: 6765 745f 666f 726d 6174 290a 2020 2020  get_format).    
+0000cb20: 2020 2020 636f 6d6d 616e 6473 203d 205b      commands = [
+0000cb30: 0a20 2020 2020 2020 2020 2020 2066 2266  .            f"f
+0000cb40: 696e 6420 5c22 7b64 6174 615f 7061 7468  ind \"{data_path
+0000cb50: 7d2f 6461 7461 2f69 6e5c 2220 2d6e 616d  }/data/in\" -nam
+0000cb60: 6520 5c22 2a2e 7b73 6f75 7263 655f 666f  e \"*.{source_fo
+0000cb70: 726d 6174 7d5c 2220 7c20 6177 6b20 277b  rmat}\" | awk '{
+0000cb80: 7b70 7269 6e74 204e 522c 2024 307d 7d27  {print NR, $0}}'
+0000cb90: 203e 205c 227b 636f 6e66 6967 5f66 696c   > \"{config_fil
+0000cba0: 657d 5c22 222c 0a20 2020 2020 2020 2020  e}\"",.         
+0000cbb0: 2020 2066 224e 3d24 2877 6320 2d6c 203c     f"N=$(wc -l <
+0000cbc0: 205c 227b 636f 6e66 6967 5f66 696c 657d   \"{config_file}
+0000cbd0: 5c22 2922 2c0a 2020 2020 2020 2020 2020  \")",.          
+0000cbe0: 2020 6622 6563 686f 205c 224e 756d 6265    f"echo \"Numbe
+0000cbf0: 7220 6f66 202e 7b73 6f75 7263 655f 666f  r of .{source_fo
+0000cc00: 726d 6174 7d20 6669 6c65 733a 2024 4e5c  rmat} files: $N\
+0000cc10: 2222 2c0a 2020 2020 2020 2020 2020 2020  "",.            
+0000cc20: 636f 6e76 6572 7369 6f6e 5f63 6d64 0a20  conversion_cmd. 
+0000cc30: 2020 2020 2020 205d 0a0a 2020 2020 2020         ]..      
+0000cc40: 2020 2320 5275 6e20 616c 6c20 636f 6d6d    # Run all comm
+0000cc50: 616e 6473 2063 6f6e 7365 6375 7469 7665  ands consecutive
+0000cc60: 6c79 0a20 2020 2020 2020 2072 6573 203d  ly.        res =
+0000cc70: 2073 656c 662e 7275 6e5f 636f 6d6d 616e   self.run_comman
+0000cc80: 6473 2863 6f6d 6d61 6e64 732c 2073 6261  ds(commands, sba
+0000cc90: 7463 685f 656e 7629 0a0a 2020 2020 2020  tch_env)..      
+0000cca0: 2020 7265 7475 726e 2053 6c75 726d 4a6f    return SlurmJo
+0000ccb0: 6228 7265 732c 2073 656c 662e 6578 7472  b(res, self.extr
+0000ccc0: 6163 745f 6a6f 625f 6964 2872 6573 2929  act_job_id(res))
+0000ccd0: 0a0a 2020 2020 6465 6620 6578 7472 6163  ..    def extrac
+0000cce0: 745f 6a6f 625f 6964 2873 656c 662c 2072  t_job_id(self, r
+0000ccf0: 6573 756c 743a 2052 6573 756c 7429 202d  esult: Result) -
+0000cd00: 3e20 696e 743a 0a20 2020 2020 2020 2022  > int:.        "
+0000cd10: 2222 0a20 2020 2020 2020 2045 7874 7261  "".        Extra
+0000cd20: 6374 2074 6865 2053 6c75 726d 206a 6f62  ct the Slurm job
+0000cd30: 2049 4420 6672 6f6d 2074 6865 2072 6573   ID from the res
+0000cd40: 756c 7420 6f66 2061 2063 6f6d 6d61 6e64  ult of a command
+0000cd50: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+0000cd60: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+0000cd70: 756c 7420 2852 6573 756c 7429 3a20 5468  ult (Result): Th
+0000cd80: 6520 7265 7375 6c74 206f 6620 6120 636f  e result of a co
+0000cd90: 6d6d 616e 6420 6578 6563 7574 696f 6e2e  mmand execution.
+0000cda0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+0000cdb0: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
+0000cdc0: 6e74 3a0a 2020 2020 2020 2020 2020 2020  nt:.            
+0000cdd0: 2020 2020 5468 6520 536c 7572 6d20 6a6f      The Slurm jo
+0000cde0: 6220 4944 2065 7874 7261 6374 6564 2066  b ID extracted f
+0000cdf0: 726f 6d20 7468 6520 7265 7375 6c74 2c0a  rom the result,.
+0000ce00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce10: 6f72 202d 3120 6966 206e 6f74 2066 6f75  or -1 if not fou
+0000ce20: 6e64 2e0a 2020 2020 2020 2020 2222 220a  nd..        """.
+0000ce30: 2020 2020 2020 2020 736c 7572 6d5f 6a6f          slurm_jo
+0000ce40: 625f 6964 203d 206e 6578 7428 2869 6e74  b_id = next((int
+0000ce50: 2873 2e73 7472 6970 2829 2920 666f 7220  (s.strip()) for 
+0000ce60: 7320 696e 2072 6573 756c 742e 7374 646f  s in result.stdo
+0000ce70: 7574 2e73 706c 6974 280a 2020 2020 2020  ut.split(.      
 0000ce80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ce90: 2020 2253 7562 6d69 7474 6564 2062 6174    "Submitted bat
-0000cea0: 6368 206a 6f62 2229 2069 6620 732e 7374  ch job") if s.st
-0000ceb0: 7269 7028 292e 6973 6469 6769 7428 2929  rip().isdigit())
-0000cec0: 2c20 2d31 290a 2020 2020 2020 2020 7265  , -1).        re
-0000ced0: 7475 726e 2073 6c75 726d 5f6a 6f62 5f69  turn slurm_job_i
-0000cee0: 640a 0a20 2020 2064 6566 2067 6574 5f75  d..    def get_u
-0000cef0: 7064 6174 655f 736c 7572 6d5f 7363 7269  pdate_slurm_scri
-0000cf00: 7074 735f 636f 6d6d 616e 6428 7365 6c66  pts_command(self
-0000cf10: 2920 2d3e 2073 7472 3a0a 2020 2020 2020  ) -> str:.      
-0000cf20: 2020 2222 2247 656e 6572 6174 6520 7468    """Generate th
-0000cf30: 6520 636f 6d6d 616e 6420 746f 2075 7064  e command to upd
-0000cf40: 6174 6520 7468 6520 4769 7420 7265 706f  ate the Git repo
-0000cf50: 7369 746f 7279 2063 6f6e 7461 696e 696e  sitory containin
-0000cf60: 670a 2020 2020 2020 2020 7468 6520 536c  g.        the Sl
-0000cf70: 7572 6d20 7363 7269 7074 732c 2069 6620  urm scripts, if 
-0000cf80: 6e65 6365 7373 6172 792e 0a0a 2020 2020  necessary...    
-0000cf90: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-0000cfa0: 2020 2020 2020 2020 2073 7472 3a0a 2020           str:.  
-0000cfb0: 2020 2020 2020 2020 2020 2020 2020 4120                A 
-0000cfc0: 7374 7269 6e67 2063 6f6e 7461 696e 696e  string containin
-0000cfd0: 6720 7468 6520 4769 7420 636f 6d6d 616e  g the Git comman
-0000cfe0: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-0000cff0: 2020 746f 2075 7064 6174 6520 7468 6520    to update the 
-0000d000: 536c 7572 6d20 7363 7269 7074 732e 0a20  Slurm scripts.. 
-0000d010: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000d020: 2020 2075 7064 6174 655f 636d 6420 3d20     update_cmd = 
-0000d030: 6622 6769 7420 2d43 205c 227b 7365 6c66  f"git -C \"{self
-0000d040: 2e73 6c75 726d 5f73 6372 6970 745f 7061  .slurm_script_pa
-0000d050: 7468 7d5c 2220 7075 6c6c 220a 2020 2020  th}\" pull".    
-0000d060: 2020 2020 7265 7475 726e 2075 7064 6174      return updat
-0000d070: 655f 636d 640a 0a20 2020 2064 6566 2063  e_cmd..    def c
-0000d080: 6865 636b 5f6a 6f62 5f73 7461 7475 7328  heck_job_status(
-0000d090: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
-0000d0a0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000d0b0: 6c75 726d 5f6a 6f62 5f69 6473 3a20 4c69  lurm_job_ids: Li
-0000d0c0: 7374 5b69 6e74 5d2c 0a20 2020 2020 2020  st[int],.       
+0000ce90: 2020 2020 2020 2253 7562 6d69 7474 6564        "Submitted
+0000cea0: 2062 6174 6368 206a 6f62 2229 2069 6620   batch job") if 
+0000ceb0: 732e 7374 7269 7028 292e 6973 6469 6769  s.strip().isdigi
+0000cec0: 7428 2929 2c20 2d31 290a 2020 2020 2020  t()), -1).      
+0000ced0: 2020 7265 7475 726e 2073 6c75 726d 5f6a    return slurm_j
+0000cee0: 6f62 5f69 640a 0a20 2020 2064 6566 2067  ob_id..    def g
+0000cef0: 6574 5f75 7064 6174 655f 736c 7572 6d5f  et_update_slurm_
+0000cf00: 7363 7269 7074 735f 636f 6d6d 616e 6428  scripts_command(
+0000cf10: 7365 6c66 2920 2d3e 2073 7472 3a0a 2020  self) -> str:.  
+0000cf20: 2020 2020 2020 2222 2247 656e 6572 6174        """Generat
+0000cf30: 6520 7468 6520 636f 6d6d 616e 6420 746f  e the command to
+0000cf40: 2075 7064 6174 6520 7468 6520 4769 7420   update the Git 
+0000cf50: 7265 706f 7369 746f 7279 2063 6f6e 7461  repository conta
+0000cf60: 696e 696e 670a 2020 2020 2020 2020 7468  ining.        th
+0000cf70: 6520 536c 7572 6d20 7363 7269 7074 732c  e Slurm scripts,
+0000cf80: 2069 6620 6e65 6365 7373 6172 792e 0a0a   if necessary...
+0000cf90: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+0000cfa0: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
+0000cfb0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000cfc0: 2020 4120 7374 7269 6e67 2063 6f6e 7461    A string conta
+0000cfd0: 696e 696e 6720 7468 6520 4769 7420 636f  ining the Git co
+0000cfe0: 6d6d 616e 640a 2020 2020 2020 2020 2020  mmand.          
+0000cff0: 2020 2020 2020 746f 2075 7064 6174 6520        to update 
+0000d000: 7468 6520 536c 7572 6d20 7363 7269 7074  the Slurm script
+0000d010: 732e 0a20 2020 2020 2020 2022 2222 0a20  s..        """. 
+0000d020: 2020 2020 2020 2075 7064 6174 655f 636d         update_cm
+0000d030: 6420 3d20 6622 6769 7420 2d43 205c 227b  d = f"git -C \"{
+0000d040: 7365 6c66 2e73 6c75 726d 5f73 6372 6970  self.slurm_scrip
+0000d050: 745f 7061 7468 7d5c 2220 7075 6c6c 220a  t_path}\" pull".
+0000d060: 2020 2020 2020 2020 7265 7475 726e 2075          return u
+0000d070: 7064 6174 655f 636d 640a 0a20 2020 2064  pdate_cmd..    d
+0000d080: 6566 2063 6865 636b 5f6a 6f62 5f73 7461  ef check_job_sta
+0000d090: 7475 7328 7365 6c66 2c0a 2020 2020 2020  tus(self,.      
+0000d0a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d0b0: 2020 2073 6c75 726d 5f6a 6f62 5f69 6473     slurm_job_ids
+0000d0c0: 3a20 4c69 7374 5b69 6e74 5d2c 0a20 2020  : List[int],.   
 0000d0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d0e0: 2020 656e 763a 204f 7074 696f 6e61 6c5b    env: Optional[
-0000d0f0: 4469 6374 5b73 7472 2c20 7374 725d 5d20  Dict[str, str]] 
-0000d100: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+0000d0e0: 2020 2020 2020 656e 763a 204f 7074 696f        env: Optio
+0000d0f0: 6e61 6c5b 4469 6374 5b73 7472 2c20 7374  nal[Dict[str, st
+0000d100: 725d 5d20 3d20 4e6f 6e65 0a20 2020 2020  r]] = None.     
 0000d110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d120: 2920 2d3e 2054 7570 6c65 5b44 6963 745b  ) -> Tuple[Dict[
-0000d130: 696e 742c 2073 7472 5d2c 2052 6573 756c  int, str], Resul
-0000d140: 745d 3a0a 2020 2020 2020 2020 2222 220a  t]:.        """.
-0000d150: 2020 2020 2020 2020 4368 6563 6b20 7468          Check th
-0000d160: 6520 7374 6174 7573 206f 6620 536c 7572  e status of Slur
-0000d170: 6d20 6a6f 6273 2077 6974 6820 7468 6520  m jobs with the 
-0000d180: 6769 7665 6e20 6a6f 6220 4944 732e 0a0a  given job IDs...
-0000d190: 2020 2020 2020 2020 4e6f 7465 3a20 5468          Note: Th
-0000d1a0: 6973 2064 6f65 736e 2774 2072 6574 7572  is doesn't retur
-0000d1b0: 6e20 6a6f 6220 6172 7261 7973 2069 6e64  n job arrays ind
-0000d1c0: 6976 6964 7561 6c6c 792e 0a20 2020 2020  ividually..     
-0000d1d0: 2020 2049 7420 7461 6b65 7320 7468 6520     It takes the 
-0000d1e0: 6c61 7374 2076 616c 7565 2072 6574 7572  last value retur
-0000d1f0: 6e65 6420 666f 7220 7468 6f73 6520 7375  ned for those su
-0000d200: 6220 6964 7320 0a20 2020 2020 2020 2028  b ids .        (
-0000d210: 6765 6e65 7261 6c6c 7920 7468 6520 6f6e  generally the on
-0000d220: 6520 7374 696c 6c20 5045 4e44 494e 4729  e still PENDING)
-0000d230: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-0000d240: 0a20 2020 2020 2020 2020 2020 2073 6c75  .            slu
-0000d250: 726d 5f6a 6f62 5f69 6473 2028 4c69 7374  rm_job_ids (List
-0000d260: 5b69 6e74 5d29 3a20 5468 6520 6a6f 6220  [int]): The job 
-0000d270: 4944 7320 6f66 2074 6865 2053 6c75 726d  IDs of the Slurm
-0000d280: 206a 6f62 7320 746f 2063 6865 636b 2e0a   jobs to check..
-0000d290: 2020 2020 2020 2020 2020 2020 656e 7620              env 
-0000d2a0: 2844 6963 745b 7374 722c 2073 7472 5d2c  (Dict[str, str],
-0000d2b0: 206f 7074 696f 6e61 6c29 3a20 4f70 7469   optional): Opti
-0000d2c0: 6f6e 616c 2065 6e76 6972 6f6e 6d65 6e74  onal environment
-0000d2d0: 2076 6172 6961 626c 6573 2074 6f0a 2020   variables to.  
-0000d2e0: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000d2f0: 7420 7768 656e 2072 756e 6e69 6e67 2074  t when running t
-0000d300: 6865 2063 6f6d 6d61 6e64 2e20 4465 6661  he command. Defa
-0000d310: 756c 7473 2074 6f20 4e6f 6e65 2e0a 0a20  ults to None... 
-0000d320: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-0000d330: 2020 2020 2020 2020 2020 2020 5475 706c              Tupl
-0000d340: 655b 4469 6374 5b69 6e74 2c20 7374 725d  e[Dict[int, str]
-0000d350: 2c20 5265 7375 6c74 5d3a 0a20 2020 2020  , Result]:.     
-0000d360: 2020 2020 2020 2020 2020 2041 2074 7570             A tup
-0000d370: 6c65 2063 6f6e 7461 696e 696e 6720 7468  le containing th
-0000d380: 6520 7374 6174 7573 2070 6572 2069 6e70  e status per inp
-0000d390: 7574 2049 4420 616e 6420 7468 6520 7265  ut ID and the re
-0000d3a0: 7375 6c74 206f 6620 0a20 2020 2020 2020  sult of .       
-0000d3b0: 2020 2020 2020 2020 2074 6865 2063 6f6d           the com
-0000d3c0: 6d61 6e64 2065 7865 6375 7469 6f6e 2e0a  mand execution..
-0000d3d0: 0a20 2020 2020 2020 2052 6169 7365 733a  .        Raises:
-0000d3e0: 0a20 2020 2020 2020 2020 2020 2053 5348  .            SSH
-0000d3f0: 4578 6365 7074 696f 6e3a 2049 6620 7468  Exception: If th
-0000d400: 6520 636f 6d6d 616e 6420 6578 6563 7574  e command execut
-0000d410: 696f 6e20 6661 696c 7320 6f72 206e 6f20  ion fails or no 
-0000d420: 7265 7370 6f6e 7365 2069 730a 2020 2020  response is.    
-0000d430: 2020 2020 2020 2020 2020 2020 7265 6365              rece
-0000d440: 6976 6564 2061 6674 6572 206d 756c 7469  ived after multi
-0000d450: 706c 6520 7265 7472 6965 732e 0a20 2020  ple retries..   
-0000d460: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000d470: 2063 6d64 203d 2073 656c 662e 6765 745f   cmd = self.get_
-0000d480: 6a6f 625f 7374 6174 7573 5f63 6f6d 6d61  job_status_comma
-0000d490: 6e64 2873 6c75 726d 5f6a 6f62 5f69 6473  nd(slurm_job_ids
-0000d4a0: 290a 2020 2020 2020 2020 6c6f 6767 6572  ).        logger
-0000d4b0: 2e69 6e66 6f28 6622 4765 7474 696e 6720  .info(f"Getting 
-0000d4c0: 7374 6174 7573 206f 6620 7b73 6c75 726d  status of {slurm
-0000d4d0: 5f6a 6f62 5f69 6473 7d20 6f6e 2053 6c75  _job_ids} on Slu
-0000d4e0: 726d 2229 0a20 2020 2020 2020 2072 6574  rm").        ret
-0000d4f0: 7279 5f73 7461 7475 7320 3d20 300a 2020  ry_status = 0.  
-0000d500: 2020 2020 2020 7768 696c 6520 7265 7472        while retr
-0000d510: 795f 7374 6174 7573 203c 2033 3a0a 2020  y_status < 3:.  
-0000d520: 2020 2020 2020 2020 2020 7265 7375 6c74            result
-0000d530: 203d 2073 656c 662e 7275 6e5f 636f 6d6d   = self.run_comm
-0000d540: 616e 6473 285b 636d 645d 2c20 656e 763d  ands([cmd], env=
-0000d550: 656e 7629 0a20 2020 2020 2020 2020 2020  env).           
-0000d560: 206c 6f67 6765 722e 696e 666f 2872 6573   logger.info(res
-0000d570: 756c 7429 0a20 2020 2020 2020 2020 2020  ult).           
-0000d580: 2069 6620 7265 7375 6c74 2e6f 6b3a 0a20   if result.ok:. 
-0000d590: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000d5a0: 6620 6e6f 7420 7265 7375 6c74 2e73 7464  f not result.std
-0000d5b0: 6f75 743a 0a20 2020 2020 2020 2020 2020  out:.           
-0000d5c0: 2020 2020 2020 2020 2023 2077 6169 7420           # wait 
-0000d5d0: 666f 7220 3320 7365 636f 6e64 7320 6265  for 3 seconds be
-0000d5e0: 666f 7265 2063 6865 636b 696e 6720 6167  fore checking ag
-0000d5f0: 6169 6e0a 2020 2020 2020 2020 2020 2020  ain.            
-0000d600: 2020 2020 2020 2020 7469 6d65 736c 6565          timeslee
-0000d610: 702e 736c 6565 7028 3329 0a20 2020 2020  p.sleep(3).     
-0000d620: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000d630: 2072 6574 7279 0a20 2020 2020 2020 2020   retry.         
-0000d640: 2020 2020 2020 2020 2020 2072 6574 7279             retry
-0000d650: 5f73 7461 7475 7320 2b3d 2031 0a20 2020  _status += 1.   
-0000d660: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d670: 206c 6f67 6765 722e 6465 6275 6728 0a20   logger.debug(. 
-0000d680: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d690: 2020 2020 2020 2066 2252 6574 7279 207b         f"Retry {
-0000d6a0: 7265 7472 795f 7374 6174 7573 7d20 6765  retry_status} ge
-0000d6b0: 7474 696e 6720 7374 6174 7573 205c 0a20  tting status \. 
-0000d6c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d6d0: 2020 2020 2020 2020 2020 206f 6620 7b73             of {s
-0000d6e0: 6c75 726d 5f6a 6f62 5f69 6473 7d21 2229  lurm_job_ids}!")
-0000d6f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d700: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000d710: 2020 2020 2020 2020 2020 2023 0a20 2020             #.   
-0000d720: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d730: 206a 6f62 5f73 7461 7475 735f 6469 6374   job_status_dict
-0000d740: 203d 207b 696e 7428 6c69 6e65 2e73 706c   = {int(line.spl
-0000d750: 6974 2829 5b30 5d2e 7370 6c69 7428 275f  it()[0].split('_
-0000d760: 2729 5b30 5d29 3a20 6c69 6e65 2e73 706c  ')[0]): line.spl
-0000d770: 6974 280a 2020 2020 2020 2020 2020 2020  it(.            
-0000d780: 2020 2020 2020 2020 295b 315d 2066 6f72          )[1] for
-0000d790: 206c 696e 6520 696e 2072 6573 756c 742e   line in result.
-0000d7a0: 7374 646f 7574 2e73 706c 6974 2822 5c6e  stdout.split("\n
-0000d7b0: 2229 2069 6620 6c69 6e65 7d0a 2020 2020  ") if line}.    
+0000d120: 2020 2020 2920 2d3e 2054 7570 6c65 5b44      ) -> Tuple[D
+0000d130: 6963 745b 696e 742c 2073 7472 5d2c 2052  ict[int, str], R
+0000d140: 6573 756c 745d 3a0a 2020 2020 2020 2020  esult]:.        
+0000d150: 2222 220a 2020 2020 2020 2020 4368 6563  """.        Chec
+0000d160: 6b20 7468 6520 7374 6174 7573 206f 6620  k the status of 
+0000d170: 536c 7572 6d20 6a6f 6273 2077 6974 6820  Slurm jobs with 
+0000d180: 7468 6520 6769 7665 6e20 6a6f 6220 4944  the given job ID
+0000d190: 732e 0a0a 2020 2020 2020 2020 4e6f 7465  s...        Note
+0000d1a0: 3a20 5468 6973 2064 6f65 736e 2774 2072  : This doesn't r
+0000d1b0: 6574 7572 6e20 6a6f 6220 6172 7261 7973  eturn job arrays
+0000d1c0: 2069 6e64 6976 6964 7561 6c6c 792e 0a20   individually.. 
+0000d1d0: 2020 2020 2020 2049 7420 7461 6b65 7320         It takes 
+0000d1e0: 7468 6520 6c61 7374 2076 616c 7565 2072  the last value r
+0000d1f0: 6574 7572 6e65 6420 666f 7220 7468 6f73  eturned for thos
+0000d200: 6520 7375 6220 6964 7320 0a20 2020 2020  e sub ids .     
+0000d210: 2020 2028 6765 6e65 7261 6c6c 7920 7468     (generally th
+0000d220: 6520 6f6e 6520 7374 696c 6c20 5045 4e44  e one still PEND
+0000d230: 494e 4729 2e0a 0a20 2020 2020 2020 2041  ING)...        A
+0000d240: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+0000d250: 2073 6c75 726d 5f6a 6f62 5f69 6473 2028   slurm_job_ids (
+0000d260: 4c69 7374 5b69 6e74 5d29 3a20 5468 6520  List[int]): The 
+0000d270: 6a6f 6220 4944 7320 6f66 2074 6865 2053  job IDs of the S
+0000d280: 6c75 726d 206a 6f62 7320 746f 2063 6865  lurm jobs to che
+0000d290: 636b 2e0a 2020 2020 2020 2020 2020 2020  ck..            
+0000d2a0: 656e 7620 2844 6963 745b 7374 722c 2073  env (Dict[str, s
+0000d2b0: 7472 5d2c 206f 7074 696f 6e61 6c29 3a20  tr], optional): 
+0000d2c0: 4f70 7469 6f6e 616c 2065 6e76 6972 6f6e  Optional environ
+0000d2d0: 6d65 6e74 2076 6172 6961 626c 6573 2074  ment variables t
+0000d2e0: 6f0a 2020 2020 2020 2020 2020 2020 2020  o.              
+0000d2f0: 2020 7365 7420 7768 656e 2072 756e 6e69    set when runni
+0000d300: 6e67 2074 6865 2063 6f6d 6d61 6e64 2e20  ng the command. 
+0000d310: 4465 6661 756c 7473 2074 6f20 4e6f 6e65  Defaults to None
+0000d320: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0000d330: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0000d340: 5475 706c 655b 4469 6374 5b69 6e74 2c20  Tuple[Dict[int, 
+0000d350: 7374 725d 2c20 5265 7375 6c74 5d3a 0a20  str], Result]:. 
+0000d360: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+0000d370: 2074 7570 6c65 2063 6f6e 7461 696e 696e   tuple containin
+0000d380: 6720 7468 6520 7374 6174 7573 2070 6572  g the status per
+0000d390: 2069 6e70 7574 2049 4420 616e 6420 7468   input ID and th
+0000d3a0: 6520 7265 7375 6c74 206f 6620 0a20 2020  e result of .   
+0000d3b0: 2020 2020 2020 2020 2020 2020 2074 6865               the
+0000d3c0: 2063 6f6d 6d61 6e64 2065 7865 6375 7469   command executi
+0000d3d0: 6f6e 2e0a 0a20 2020 2020 2020 2052 6169  on...        Rai
+0000d3e0: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
+0000d3f0: 2053 5348 4578 6365 7074 696f 6e3a 2049   SSHException: I
+0000d400: 6620 7468 6520 636f 6d6d 616e 6420 6578  f the command ex
+0000d410: 6563 7574 696f 6e20 6661 696c 7320 6f72  ecution fails or
+0000d420: 206e 6f20 7265 7370 6f6e 7365 2069 730a   no response is.
+0000d430: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d440: 7265 6365 6976 6564 2061 6674 6572 206d  received after m
+0000d450: 756c 7469 706c 6520 7265 7472 6965 732e  ultiple retries.
+0000d460: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000d470: 2020 2020 2063 6d64 203d 2073 656c 662e       cmd = self.
+0000d480: 6765 745f 6a6f 625f 7374 6174 7573 5f63  get_job_status_c
+0000d490: 6f6d 6d61 6e64 2873 6c75 726d 5f6a 6f62  ommand(slurm_job
+0000d4a0: 5f69 6473 290a 2020 2020 2020 2020 6c6f  _ids).        lo
+0000d4b0: 6767 6572 2e69 6e66 6f28 6622 4765 7474  gger.info(f"Gett
+0000d4c0: 696e 6720 7374 6174 7573 206f 6620 7b73  ing status of {s
+0000d4d0: 6c75 726d 5f6a 6f62 5f69 6473 7d20 6f6e  lurm_job_ids} on
+0000d4e0: 2053 6c75 726d 2229 0a20 2020 2020 2020   Slurm").       
+0000d4f0: 2072 6574 7279 5f73 7461 7475 7320 3d20   retry_status = 
+0000d500: 300a 2020 2020 2020 2020 7768 696c 6520  0.        while 
+0000d510: 7265 7472 795f 7374 6174 7573 203c 2033  retry_status < 3
+0000d520: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000d530: 7375 6c74 203d 2073 656c 662e 7275 6e5f  sult = self.run_
+0000d540: 636f 6d6d 616e 6473 285b 636d 645d 2c20  commands([cmd], 
+0000d550: 656e 763d 656e 7629 0a20 2020 2020 2020  env=env).       
+0000d560: 2020 2020 206c 6f67 6765 722e 696e 666f       logger.info
+0000d570: 2872 6573 756c 7429 0a20 2020 2020 2020  (result).       
+0000d580: 2020 2020 2069 6620 7265 7375 6c74 2e6f       if result.o
+0000d590: 6b3a 0a20 2020 2020 2020 2020 2020 2020  k:.             
+0000d5a0: 2020 2069 6620 6e6f 7420 7265 7375 6c74     if not result
+0000d5b0: 2e73 7464 6f75 743a 0a20 2020 2020 2020  .stdout:.       
+0000d5c0: 2020 2020 2020 2020 2020 2020 2023 2077               # w
+0000d5d0: 6169 7420 666f 7220 3320 7365 636f 6e64  ait for 3 second
+0000d5e0: 7320 6265 666f 7265 2063 6865 636b 696e  s before checkin
+0000d5f0: 6720 6167 6169 6e0a 2020 2020 2020 2020  g again.        
+0000d600: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+0000d610: 736c 6565 702e 736c 6565 7028 3329 0a20  sleep.sleep(3). 
+0000d620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d630: 2020 2023 2072 6574 7279 0a20 2020 2020     # retry.     
+0000d640: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000d650: 6574 7279 5f73 7461 7475 7320 2b3d 2031  etry_status += 1
+0000d660: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d670: 2020 2020 206c 6f67 6765 722e 6465 6275       logger.debu
+0000d680: 6728 0a20 2020 2020 2020 2020 2020 2020  g(.             
+0000d690: 2020 2020 2020 2020 2020 2066 2252 6574             f"Ret
+0000d6a0: 7279 207b 7265 7472 795f 7374 6174 7573  ry {retry_status
+0000d6b0: 7d20 6765 7474 696e 6720 7374 6174 7573  } getting status
+0000d6c0: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
+0000d6d0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000d6e0: 6620 7b73 6c75 726d 5f6a 6f62 5f69 6473  f {slurm_job_ids
+0000d6f0: 7d21 2229 0a20 2020 2020 2020 2020 2020  }!").           
+0000d700: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000d710: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000d720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d730: 2020 2020 206a 6f62 5f73 7461 7475 735f       job_status_
+0000d740: 6469 6374 203d 207b 696e 7428 6c69 6e65  dict = {int(line
+0000d750: 2e73 706c 6974 2829 5b30 5d2e 7370 6c69  .split()[0].spli
+0000d760: 7428 275f 2729 5b30 5d29 3a20 6c69 6e65  t('_')[0]): line
+0000d770: 2e73 706c 6974 280a 2020 2020 2020 2020  .split(.        
+0000d780: 2020 2020 2020 2020 2020 2020 295b 315d              )[1]
+0000d790: 2066 6f72 206c 696e 6520 696e 2072 6573   for line in res
+0000d7a0: 756c 742e 7374 646f 7574 2e73 706c 6974  ult.stdout.split
+0000d7b0: 2822 5c6e 2229 2069 6620 6c69 6e65 7d0a  ("\n") if line}.
 0000d7c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d7d0: 6c6f 6767 6572 2e64 6562 7567 2866 224a  logger.debug(f"J
-0000d7e0: 6f62 2073 7461 7475 7365 733a 207b 6a6f  ob statuses: {jo
-0000d7f0: 625f 7374 6174 7573 5f64 6963 747d 2229  b_status_dict}")
-0000d800: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000d810: 2020 2020 200a 2020 2020 2020 2020 2020       .          
-0000d820: 2020 2020 2020 2020 2020 2320 4f4b 2c20            # OK, 
-0000d830: 7765 2068 6176 6520 746f 2066 6978 2061  we have to fix a
-0000d840: 2073 7475 7069 6420 7361 6363 7420 6675   stupid sacct fu
-0000d850: 6e63 7469 6f6e 616c 6974 793a 0a20 2020  nctionality:.   
-0000d860: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d870: 2023 2050 726f 626c 656d 3a0a 2020 2020   # Problem:.    
+0000d7d0: 2020 2020 6c6f 6767 6572 2e64 6562 7567      logger.debug
+0000d7e0: 2866 224a 6f62 2073 7461 7475 7365 733a  (f"Job statuses:
+0000d7f0: 207b 6a6f 625f 7374 6174 7573 5f64 6963   {job_status_dic
+0000d800: 747d 2229 0a20 2020 2020 2020 2020 2020  t}").           
+0000d810: 2020 2020 2020 2020 200a 2020 2020 2020           .      
+0000d820: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000d830: 4f4b 2c20 7765 2068 6176 6520 746f 2066  OK, we have to f
+0000d840: 6978 2061 2073 7475 7069 6420 7361 6363  ix a stupid sacc
+0000d850: 7420 6675 6e63 7469 6f6e 616c 6974 793a  t functionality:
+0000d860: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000d870: 2020 2020 2023 2050 726f 626c 656d 3a0a       # Problem:.
 0000d880: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d890: 2320 5768 656e 2079 6f75 2071 7565 7279  # When you query
-0000d8a0: 2066 6f72 2061 206a 6f62 2d69 642c 2074   for a job-id, t
-0000d8b0: 7572 6e73 206f 7574 2074 6861 7420 6974  urns out that it
-0000d8c0: 2071 7565 7269 6573 0a20 2020 2020 2020   queries.       
-0000d8d0: 2020 2020 2020 2020 2020 2020 2023 2066               # f
-0000d8e0: 6f72 2074 6869 7320 274a 6f62 4964 5261  or this 'JobIdRa
-0000d8f0: 7727 2e20 416e 6420 4a6f 6249 6452 6177  w'. And JobIdRaw
-0000d900: 2066 6f72 2061 7272 6179 7320 6973 2061   for arrays is a
-0000d910: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-0000d920: 2020 2020 2020 2320 7269 6469 6375 6c6f        # ridiculo
-0000d930: 7573 2073 756d 2c20 652e 672e 2027 4a6f  us sum, e.g. 'Jo
-0000d940: 6249 6427 2031 315f 3220 6765 7473 2061  bId' 11_2 gets a
-0000d950: 7373 6967 6e65 6420 0a20 2020 2020 2020  ssigned .       
-0000d960: 2020 2020 2020 2020 2020 2020 2023 2027               # '
-0000d970: 4a6f 6249 6452 6177 2720 3133 2028 3d20  JobIdRaw' 13 (= 
-0000d980: 3131 2b32 2921 0a20 2020 2020 2020 2020  11+2)!.         
-0000d990: 2020 2020 2020 2020 2020 2023 2055 6e74             # Unt
-0000d9a0: 696c 2079 6f75 2073 7562 6d69 7420 3220  il you submit 2 
-0000d9b0: 6d6f 7265 206a 6f62 7320 616e 6420 6163  more jobs and ac
-0000d9c0: 7475 616c 2027 4a6f 6249 6427 2031 3320  tual 'JobId' 13 
-0000d9d0: 636f 6d65 730a 2020 2020 2020 2020 2020  comes.          
-0000d9e0: 2020 2020 2020 2020 2020 2320 616c 6f6e            # alon
-0000d9f0: 672c 2066 726f 6d20 7468 656e 206f 6e20  g, from then on 
-0000da00: 796f 7520 6765 7420 7468 6174 2073 7461  you get that sta
-0000da10: 7475 7320 7265 7475 726e 6564 2e2e 2e0a  tus returned....
-0000da20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da30: 2020 2020 2320 466f 7220 7573 2c20 7468      # For us, th
-0000da40: 6973 2063 7265 6174 6573 2061 2072 6163  is creates a rac
-0000da50: 6520 636f 6e64 6974 696f 6e2c 2077 6865  e condition, whe
-0000da60: 7265 2077 6520 6765 7420 7468 0a20 2020  re we get th.   
-0000da70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000da80: 2023 2065 2077 726f 6e67 2064 6174 6120   # e wrong data 
-0000da90: 6261 636b 2e20 5765 2065 7870 6563 7420  back. We expect 
-0000daa0: 274a 6f62 4964 2720 3133 2c20 6275 7420  'JobId' 13, but 
-0000dab0: 6974 7320 6e6f 7420 0a20 2020 2020 2020  its not .       
-0000dac0: 2020 2020 2020 2020 2020 2020 2023 2074               # t
-0000dad0: 6865 7265 2079 6574 2066 6f72 2073 6f6d  here yet for som
-0000dae0: 6520 7265 6173 6f6e 2c20 736f 2077 6520  e reason, so we 
-0000daf0: 6765 7420 736f 6d65 2072 6573 756c 7420  get some result 
-0000db00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000db10: 2020 2020 2023 2066 726f 6d20 2731 315f       # from '11_
-0000db20: 3227 2062 6163 6b20 696e 7374 6561 642e  2' back instead.
-0000db30: 200a 2020 2020 2020 2020 2020 2020 2020   .              
-0000db40: 2020 2020 2020 2320 416e 6420 7468 6973        # And this
-0000db50: 2063 6175 7365 7320 6120 6b65 795f 6572   causes a key_er
-0000db60: 726f 7220 6c61 7465 7220 6f6e 2c20 6361  ror later on, ca
-0000db70: 7573 6520 7765 2065 7870 6563 740a 2020  use we expect.  
-0000db80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000db90: 2020 2320 2731 3327 2073 696e 6365 2077    # '13' since w
-0000dba0: 6520 7175 6572 6965 6420 666f 7220 7468  e queried for th
-0000dbb0: 6174 206f 6e65 2e0a 2020 2020 2020 2020  at one..        
-0000dbc0: 2020 2020 2020 2020 2020 2020 0a20 2020              .   
-0000dbd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dbe0: 2023 2043 7572 7265 6e74 2077 6f72 6b61   # Current worka
-0000dbf0: 726f 756e 643a 2061 7274 6966 6963 6961  round: artificia
-0000dc00: 6c6c 7920 6164 6420 2731 3327 2074 6f20  lly add '13' to 
-0000dc10: 6f75 7220 7265 7375 6c74 732e 0a20 2020  our results..   
-0000dc20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc30: 2023 2041 6e64 2072 656d 6f76 6520 7468   # And remove th
-0000dc40: 6520 6661 6b65 206f 6e65 2873 292e 0a20  e fake one(s).. 
-0000dc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc60: 2020 2072 6573 756c 745f 6469 6374 203d     result_dict =
-0000dc70: 207b 7d0a 2020 2020 2020 2020 2020 2020   {}.            
-0000dc80: 2020 2020 2020 2020 666f 7220 6a6f 625f          for job_
-0000dc90: 6964 2069 6e20 736c 7572 6d5f 6a6f 625f  id in slurm_job_
-0000dca0: 6964 733a 0a20 2020 2020 2020 2020 2020  ids:.           
-0000dcb0: 2020 2020 2020 2020 2020 2020 2023 2043               # C
-0000dcc0: 6865 636b 2069 6620 7468 6520 6a6f 6220  heck if the job 
-0000dcd0: 4944 2069 7320 6e6f 7420 616c 7265 6164  ID is not alread
-0000dce0: 7920 696e 2074 6865 206a 6f62 5f73 7461  y in the job_sta
-0000dcf0: 7475 735f 6469 6374 0a20 2020 2020 2020  tus_dict.       
+0000d890: 2020 2020 2320 5768 656e 2079 6f75 2071      # When you q
+0000d8a0: 7565 7279 2066 6f72 2061 206a 6f62 2d69  uery for a job-i
+0000d8b0: 642c 2074 7572 6e73 206f 7574 2074 6861  d, turns out tha
+0000d8c0: 7420 6974 2071 7565 7269 6573 0a20 2020  t it queries.   
+0000d8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d8e0: 2023 2066 6f72 2074 6869 7320 274a 6f62   # for this 'Job
+0000d8f0: 4964 5261 7727 2e20 416e 6420 4a6f 6249  IdRaw'. And JobI
+0000d900: 6452 6177 2066 6f72 2061 7272 6179 7320  dRaw for arrays 
+0000d910: 6973 2061 200a 2020 2020 2020 2020 2020  is a .          
+0000d920: 2020 2020 2020 2020 2020 2320 7269 6469            # ridi
+0000d930: 6375 6c6f 7573 2073 756d 2c20 652e 672e  culous sum, e.g.
+0000d940: 2027 4a6f 6249 6427 2031 315f 3220 6765   'JobId' 11_2 ge
+0000d950: 7473 2061 7373 6967 6e65 6420 0a20 2020  ts assigned .   
+0000d960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d970: 2023 2027 4a6f 6249 6452 6177 2720 3133   # 'JobIdRaw' 13
+0000d980: 2028 3d20 3131 2b32 2921 0a20 2020 2020   (= 11+2)!.     
+0000d990: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000d9a0: 2055 6e74 696c 2079 6f75 2073 7562 6d69   Until you submi
+0000d9b0: 7420 3220 6d6f 7265 206a 6f62 7320 616e  t 2 more jobs an
+0000d9c0: 6420 6163 7475 616c 2027 4a6f 6249 6427  d actual 'JobId'
+0000d9d0: 2031 3320 636f 6d65 730a 2020 2020 2020   13 comes.      
+0000d9e0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000d9f0: 616c 6f6e 672c 2066 726f 6d20 7468 656e  along, from then
+0000da00: 206f 6e20 796f 7520 6765 7420 7468 6174   on you get that
+0000da10: 2073 7461 7475 7320 7265 7475 726e 6564   status returned
+0000da20: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+0000da30: 2020 2020 2020 2020 2320 466f 7220 7573          # For us
+0000da40: 2c20 7468 6973 2063 7265 6174 6573 2061  , this creates a
+0000da50: 2072 6163 6520 636f 6e64 6974 696f 6e2c   race condition,
+0000da60: 2077 6865 7265 2077 6520 6765 7420 7468   where we get th
+0000da70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000da80: 2020 2020 2023 2065 2077 726f 6e67 2064       # e wrong d
+0000da90: 6174 6120 6261 636b 2e20 5765 2065 7870  ata back. We exp
+0000daa0: 6563 7420 274a 6f62 4964 2720 3133 2c20  ect 'JobId' 13, 
+0000dab0: 6275 7420 6974 7320 6e6f 7420 0a20 2020  but its not .   
+0000dac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dad0: 2023 2074 6865 7265 2079 6574 2066 6f72   # there yet for
+0000dae0: 2073 6f6d 6520 7265 6173 6f6e 2c20 736f   some reason, so
+0000daf0: 2077 6520 6765 7420 736f 6d65 2072 6573   we get some res
+0000db00: 756c 7420 0a20 2020 2020 2020 2020 2020  ult .           
+0000db10: 2020 2020 2020 2020 2023 2066 726f 6d20           # from 
+0000db20: 2731 315f 3227 2062 6163 6b20 696e 7374  '11_2' back inst
+0000db30: 6561 642e 200a 2020 2020 2020 2020 2020  ead. .          
+0000db40: 2020 2020 2020 2020 2020 2320 416e 6420            # And 
+0000db50: 7468 6973 2063 6175 7365 7320 6120 6b65  this causes a ke
+0000db60: 795f 6572 726f 7220 6c61 7465 7220 6f6e  y_error later on
+0000db70: 2c20 6361 7573 6520 7765 2065 7870 6563  , cause we expec
+0000db80: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+0000db90: 2020 2020 2020 2320 2731 3327 2073 696e        # '13' sin
+0000dba0: 6365 2077 6520 7175 6572 6965 6420 666f  ce we queried fo
+0000dbb0: 7220 7468 6174 206f 6e65 2e0a 2020 2020  r that one..    
+0000dbc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dbd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dbe0: 2020 2020 2023 2043 7572 7265 6e74 2077       # Current w
+0000dbf0: 6f72 6b61 726f 756e 643a 2061 7274 6966  orkaround: artif
+0000dc00: 6963 6961 6c6c 7920 6164 6420 2731 3327  icially add '13'
+0000dc10: 2074 6f20 6f75 7220 7265 7375 6c74 732e   to our results.
+0000dc20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dc30: 2020 2020 2023 2041 6e64 2072 656d 6f76       # And remov
+0000dc40: 6520 7468 6520 6661 6b65 206f 6e65 2873  e the fake one(s
+0000dc50: 292e 0a20 2020 2020 2020 2020 2020 2020  )..             
+0000dc60: 2020 2020 2020 2072 6573 756c 745f 6469         result_di
+0000dc70: 6374 203d 207b 7d0a 2020 2020 2020 2020  ct = {}.        
+0000dc80: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+0000dc90: 6a6f 625f 6964 2069 6e20 736c 7572 6d5f  job_id in slurm_
+0000dca0: 6a6f 625f 6964 733a 0a20 2020 2020 2020  job_ids:.       
+0000dcb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dcc0: 2023 2043 6865 636b 2069 6620 7468 6520   # Check if the 
+0000dcd0: 6a6f 6220 4944 2069 7320 6e6f 7420 616c  job ID is not al
+0000dce0: 7265 6164 7920 696e 2074 6865 206a 6f62  ready in the job
+0000dcf0: 5f73 7461 7475 735f 6469 6374 0a20 2020  _status_dict.   
 0000dd00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd10: 2069 6620 6a6f 625f 6964 206e 6f74 2069   if job_id not i
-0000dd20: 6e20 6a6f 625f 7374 6174 7573 5f64 6963  n job_status_dic
-0000dd30: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
-0000dd40: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-0000dd50: 6f67 6765 722e 6465 6275 6728 6622 4d69  ogger.debug(f"Mi
-0000dd60: 7373 696e 6720 6a6f 6220 7b6a 6f62 5f69  ssing job {job_i
-0000dd70: 647d 2069 6e20 6f75 7220 5c0a 2020 2020  d} in our \.    
+0000dd10: 2020 2020 2069 6620 6a6f 625f 6964 206e       if job_id n
+0000dd20: 6f74 2069 6e20 6a6f 625f 7374 6174 7573  ot in job_status
+0000dd30: 5f64 6963 743a 0a20 2020 2020 2020 2020  _dict:.         
+0000dd40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dd50: 2020 206c 6f67 6765 722e 6465 6275 6728     logger.debug(
+0000dd60: 6622 4d69 7373 696e 6720 6a6f 6220 7b6a  f"Missing job {j
+0000dd70: 6f62 5f69 647d 2069 6e20 6f75 7220 5c0a  ob_id} in our \.
 0000dd80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dd90: 2020 2020 2020 2020 2020 2020 7265 7375              resu
-0000dda0: 6c74 7321 2041 6464 696e 6720 6974 2061  lts! Adding it a
-0000ddb0: 7274 6966 6963 6961 6c6c 792e 2229 0a20  rtificially."). 
-0000ddc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ddd0: 2020 2020 2020 2020 2020 2023 2041 6464             # Add
-0000dde0: 2074 6865 206a 6f62 2049 4420 7769 7468   the job ID with
-0000ddf0: 2061 2064 6566 6175 6c74 2073 7461 7475   a default statu
-0000de00: 7320 6f66 2027 5045 4e44 494e 4727 0a20  s of 'PENDING'. 
-0000de10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de20: 2020 2020 2020 2020 2020 2072 6573 756c             resul
-0000de30: 745f 6469 6374 5b6a 6f62 5f69 645d 203d  t_dict[job_id] =
-0000de40: 2027 5045 4e44 494e 4727 0a20 2020 2020   'PENDING'.     
+0000dd90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dda0: 7265 7375 6c74 7321 2041 6464 696e 6720  results! Adding 
+0000ddb0: 6974 2061 7274 6966 6963 6961 6c6c 792e  it artificially.
+0000ddc0: 2229 0a20 2020 2020 2020 2020 2020 2020  ").             
+0000ddd0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000dde0: 2041 6464 2074 6865 206a 6f62 2049 4420   Add the job ID 
+0000ddf0: 7769 7468 2061 2064 6566 6175 6c74 2073  with a default s
+0000de00: 7461 7475 7320 6f66 2027 5045 4e44 494e  tatus of 'PENDIN
+0000de10: 4727 0a20 2020 2020 2020 2020 2020 2020  G'.             
+0000de20: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000de30: 6573 756c 745f 6469 6374 5b6a 6f62 5f69  esult_dict[job_i
+0000de40: 645d 203d 2027 5045 4e44 494e 4727 0a20  d] = 'PENDING'. 
 0000de50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de60: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000de60: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
 0000de70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000de80: 2020 2020 2023 2043 6f70 7920 7468 6f73       # Copy thos
-0000de90: 6520 7661 6c75 6573 2074 6861 7420 7765  e values that we
-0000dea0: 2077 616e 7420 7468 6520 6b65 7973 2066   want the keys f
-0000deb0: 726f 6d0a 2020 2020 2020 2020 2020 2020  rom.            
+0000de80: 2020 2020 2020 2020 2023 2043 6f70 7920           # Copy 
+0000de90: 7468 6f73 6520 7661 6c75 6573 2074 6861  those values tha
+0000dea0: 7420 7765 2077 616e 7420 7468 6520 6b65  t we want the ke
+0000deb0: 7973 2066 726f 6d0a 2020 2020 2020 2020  ys from.        
 0000dec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ded0: 7265 7375 6c74 5f64 6963 745b 6a6f 625f  result_dict[job_
-0000dee0: 6964 5d20 3d20 6a6f 625f 7374 6174 7573  id] = job_status
-0000def0: 5f64 6963 745b 6a6f 625f 6964 5d0a 2020  _dict[job_id].  
-0000df00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000df10: 2020 0a20 2020 2020 2020 2020 2020 2020    .             
-0000df20: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
-0000df30: 7375 6c74 5f64 6963 742c 2072 6573 756c  sult_dict, resul
-0000df40: 740a 2020 2020 2020 2020 2020 2020 656c  t.            el
-0000df50: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000df60: 2020 2020 6572 726f 7220 3d20 6622 5265      error = f"Re
-0000df70: 7375 6c74 2069 7320 6e6f 7420 6f6b 3a20  sult is not ok: 
-0000df80: 7b72 6573 756c 747d 220a 2020 2020 2020  {result}".      
-0000df90: 2020 2020 2020 2020 2020 6c6f 6767 6572            logger
-0000dfa0: 2e65 7272 6f72 2865 7272 6f72 290a 2020  .error(error).  
-0000dfb0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
-0000dfc0: 6973 6520 5353 4845 7863 6570 7469 6f6e  ise SSHException
-0000dfd0: 2865 7272 6f72 290a 2020 2020 2020 2020  (error).        
-0000dfe0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000dff0: 2020 6572 726f 7220 3d20 6622 4572 726f    error = f"Erro
-0000e000: 723a 2052 6574 7269 6564 207b 7265 7472  r: Retried {retr
-0000e010: 795f 7374 6174 7573 7d20 7469 6d65 7320  y_status} times 
-0000e020: 746f 2067 6574 205c 0a20 2020 2020 2020  to get \.       
-0000e030: 2020 2020 2020 2020 2073 7461 7475 7320           status 
-0000e040: 6f66 207b 736c 7572 6d5f 6a6f 625f 6964  of {slurm_job_id
-0000e050: 737d 2c20 6275 7420 6e6f 2072 6573 706f  s}, but no respo
-0000e060: 6e73 652e 220a 2020 2020 2020 2020 2020  nse.".          
-0000e070: 2020 6c6f 6767 6572 2e65 7272 6f72 2865    logger.error(e
-0000e080: 7272 6f72 290a 2020 2020 2020 2020 2020  rror).          
-0000e090: 2020 7261 6973 6520 5353 4845 7863 6570    raise SSHExcep
-0000e0a0: 7469 6f6e 2865 7272 6f72 290a 0a20 2020  tion(error)..   
-0000e0b0: 2064 6566 2067 6574 5f6a 6f62 5f73 7461   def get_job_sta
-0000e0c0: 7475 735f 636f 6d6d 616e 6428 7365 6c66  tus_command(self
-0000e0d0: 2c20 736c 7572 6d5f 6a6f 625f 6964 733a  , slurm_job_ids:
-0000e0e0: 204c 6973 745b 696e 745d 2920 2d3e 2073   List[int]) -> s
-0000e0f0: 7472 3a0a 2020 2020 2020 2020 2222 220a  tr:.        """.
-0000e100: 2020 2020 2020 2020 5265 7475 726e 2074          Return t
-0000e110: 6865 2053 6c75 726d 2063 6f6d 6d61 6e64  he Slurm command
-0000e120: 2074 6f20 6765 7420 7468 6520 7374 6174   to get the stat
-0000e130: 7573 206f 6620 6a6f 6273 2077 6974 6820  us of jobs with 
-0000e140: 7468 6520 6769 7665 6e0a 2020 2020 2020  the given.      
-0000e150: 2020 6a6f 6220 4944 732e 0a0a 2020 2020    job IDs...    
-0000e160: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-0000e170: 2020 2020 2020 736c 7572 6d5f 6a6f 625f        slurm_job_
-0000e180: 6964 7320 284c 6973 745b 696e 745d 293a  ids (List[int]):
-0000e190: 2054 6865 206a 6f62 2049 4473 206f 6620   The job IDs of 
-0000e1a0: 7468 6520 6a6f 6273 2074 6f20 6368 6563  the jobs to chec
-0000e1b0: 6b2e 0a0a 2020 2020 2020 2020 5265 7475  k...        Retu
-0000e1c0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-0000e1d0: 2073 7472 3a20 0a20 2020 2020 2020 2020   str: .         
-0000e1e0: 2020 2020 2020 2054 6865 2053 6c75 726d         The Slurm
-0000e1f0: 2063 6f6d 6d61 6e64 2074 6f20 6765 7420   command to get 
-0000e200: 7468 6520 7374 6174 7573 206f 6620 7468  the status of th
-0000e210: 6520 6a6f 6273 2e0a 2020 2020 2020 2020  e jobs..        
-0000e220: 2222 220a 2020 2020 2020 2020 2320 636f  """.        # co
-0000e230: 6e63 6174 206d 756c 7469 706c 6520 6a6f  ncat multiple jo
-0000e240: 6273 2069 6620 6e65 6564 6564 0a20 2020  bs if needed.   
-0000e250: 2020 2020 2073 6c75 726d 5f6a 6f62 5f69       slurm_job_i
-0000e260: 6420 3d20 2220 2d6a 2022 2e6a 6f69 6e28  d = " -j ".join(
-0000e270: 5b73 7472 2869 6429 2066 6f72 2069 6420  [str(id) for id 
-0000e280: 696e 2073 6c75 726d 5f6a 6f62 5f69 6473  in slurm_job_ids
-0000e290: 5d29 0a20 2020 2020 2020 2072 6574 7572  ]).        retur
-0000e2a0: 6e20 7365 6c66 2e5f 4a4f 425f 5354 4154  n self._JOB_STAT
-0000e2b0: 5553 5f43 4d44 2e66 6f72 6d61 7428 736c  US_CMD.format(sl
-0000e2c0: 7572 6d5f 6a6f 625f 6964 3d73 6c75 726d  urm_job_id=slurm
-0000e2d0: 5f6a 6f62 5f69 6429 0a0a 2020 2020 6465  _job_id)..    de
-0000e2e0: 6620 6578 7472 6163 745f 6461 7461 5f6c  f extract_data_l
-0000e2f0: 6f63 6174 696f 6e5f 6672 6f6d 5f6c 6f67  ocation_from_log
-0000e300: 2873 656c 662c 2073 6c75 726d 5f6a 6f62  (self, slurm_job
-0000e310: 5f69 643a 2073 7472 203d 204e 6f6e 652c  _id: str = None,
-0000e320: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ded0: 2020 2020 7265 7375 6c74 5f64 6963 745b      result_dict[
+0000dee0: 6a6f 625f 6964 5d20 3d20 6a6f 625f 7374  job_id] = job_st
+0000def0: 6174 7573 5f64 6963 745b 6a6f 625f 6964  atus_dict[job_id
+0000df00: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000df10: 2020 2020 2020 0a20 2020 2020 2020 2020        .         
+0000df20: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000df30: 6e20 7265 7375 6c74 5f64 6963 742c 2072  n result_dict, r
+0000df40: 6573 756c 740a 2020 2020 2020 2020 2020  esult.          
+0000df50: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000df60: 2020 2020 2020 2020 6572 726f 7220 3d20          error = 
+0000df70: 6622 5265 7375 6c74 2069 7320 6e6f 7420  f"Result is not 
+0000df80: 6f6b 3a20 7b72 6573 756c 747d 220a 2020  ok: {result}".  
+0000df90: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+0000dfa0: 6767 6572 2e65 7272 6f72 2865 7272 6f72  gger.error(error
+0000dfb0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000dfc0: 2020 7261 6973 6520 5353 4845 7863 6570    raise SSHExcep
+0000dfd0: 7469 6f6e 2865 7272 6f72 290a 2020 2020  tion(error).    
+0000dfe0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000dff0: 2020 2020 2020 6572 726f 7220 3d20 6622        error = f"
+0000e000: 4572 726f 723a 2052 6574 7269 6564 207b  Error: Retried {
+0000e010: 7265 7472 795f 7374 6174 7573 7d20 7469  retry_status} ti
+0000e020: 6d65 7320 746f 2067 6574 205c 0a20 2020  mes to get \.   
+0000e030: 2020 2020 2020 2020 2020 2020 2073 7461               sta
+0000e040: 7475 7320 6f66 207b 736c 7572 6d5f 6a6f  tus of {slurm_jo
+0000e050: 625f 6964 737d 2c20 6275 7420 6e6f 2072  b_ids}, but no r
+0000e060: 6573 706f 6e73 652e 220a 2020 2020 2020  esponse.".      
+0000e070: 2020 2020 2020 6c6f 6767 6572 2e65 7272        logger.err
+0000e080: 6f72 2865 7272 6f72 290a 2020 2020 2020  or(error).      
+0000e090: 2020 2020 2020 7261 6973 6520 5353 4845        raise SSHE
+0000e0a0: 7863 6570 7469 6f6e 2865 7272 6f72 290a  xception(error).
+0000e0b0: 0a20 2020 2064 6566 2067 6574 5f6a 6f62  .    def get_job
+0000e0c0: 5f73 7461 7475 735f 636f 6d6d 616e 6428  _status_command(
+0000e0d0: 7365 6c66 2c20 736c 7572 6d5f 6a6f 625f  self, slurm_job_
+0000e0e0: 6964 733a 204c 6973 745b 696e 745d 2920  ids: List[int]) 
+0000e0f0: 2d3e 2073 7472 3a0a 2020 2020 2020 2020  -> str:.        
+0000e100: 2222 220a 2020 2020 2020 2020 5265 7475  """.        Retu
+0000e110: 726e 2074 6865 2053 6c75 726d 2063 6f6d  rn the Slurm com
+0000e120: 6d61 6e64 2074 6f20 6765 7420 7468 6520  mand to get the 
+0000e130: 7374 6174 7573 206f 6620 6a6f 6273 2077  status of jobs w
+0000e140: 6974 6820 7468 6520 6769 7665 6e0a 2020  ith the given.  
+0000e150: 2020 2020 2020 6a6f 6220 4944 732e 0a0a        job IDs...
+0000e160: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+0000e170: 2020 2020 2020 2020 2020 736c 7572 6d5f            slurm_
+0000e180: 6a6f 625f 6964 7320 284c 6973 745b 696e  job_ids (List[in
+0000e190: 745d 293a 2054 6865 206a 6f62 2049 4473  t]): The job IDs
+0000e1a0: 206f 6620 7468 6520 6a6f 6273 2074 6f20   of the jobs to 
+0000e1b0: 6368 6563 6b2e 0a0a 2020 2020 2020 2020  check...        
+0000e1c0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+0000e1d0: 2020 2020 2073 7472 3a20 0a20 2020 2020       str: .     
+0000e1e0: 2020 2020 2020 2020 2020 2054 6865 2053             The S
+0000e1f0: 6c75 726d 2063 6f6d 6d61 6e64 2074 6f20  lurm command to 
+0000e200: 6765 7420 7468 6520 7374 6174 7573 206f  get the status o
+0000e210: 6620 7468 6520 6a6f 6273 2e0a 2020 2020  f the jobs..    
+0000e220: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000e230: 2320 636f 6e63 6174 206d 756c 7469 706c  # concat multipl
+0000e240: 6520 6a6f 6273 2069 6620 6e65 6564 6564  e jobs if needed
+0000e250: 0a20 2020 2020 2020 2073 6c75 726d 5f6a  .        slurm_j
+0000e260: 6f62 5f69 6420 3d20 2220 2d6a 2022 2e6a  ob_id = " -j ".j
+0000e270: 6f69 6e28 5b73 7472 2869 6429 2066 6f72  oin([str(id) for
+0000e280: 2069 6420 696e 2073 6c75 726d 5f6a 6f62   id in slurm_job
+0000e290: 5f69 6473 5d29 0a20 2020 2020 2020 2072  _ids]).        r
+0000e2a0: 6574 7572 6e20 7365 6c66 2e5f 4a4f 425f  eturn self._JOB_
+0000e2b0: 5354 4154 5553 5f43 4d44 2e66 6f72 6d61  STATUS_CMD.forma
+0000e2c0: 7428 736c 7572 6d5f 6a6f 625f 6964 3d73  t(slurm_job_id=s
+0000e2d0: 6c75 726d 5f6a 6f62 5f69 6429 0a0a 2020  lurm_job_id)..  
+0000e2e0: 2020 6465 6620 6578 7472 6163 745f 6461    def extract_da
+0000e2f0: 7461 5f6c 6f63 6174 696f 6e5f 6672 6f6d  ta_location_from
+0000e300: 5f6c 6f67 2873 656c 662c 2073 6c75 726d  _log(self, slurm
+0000e310: 5f6a 6f62 5f69 643a 2073 7472 203d 204e  _job_id: str = N
+0000e320: 6f6e 652c 0a20 2020 2020 2020 2020 2020  one,.           
 0000e330: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e340: 2020 2020 2020 2020 6c6f 6766 696c 653a          logfile:
-0000e350: 2073 7472 203d 204e 6f6e 6529 202d 3e20   str = None) -> 
-0000e360: 7374 723a 0a20 2020 2020 2020 2022 2222  str:.        """
-0000e370: 5265 6164 2053 4c55 524d 206a 6f62 206c  Read SLURM job l
-0000e380: 6f67 6669 6c65 2074 6f20 6669 6e64 206c  ogfile to find l
-0000e390: 6f63 6174 696f 6e20 6f66 2074 6865 2064  ocation of the d
-0000e3a0: 6174 612e 0a0a 2020 2020 2020 2020 4f6e  ata...        On
-0000e3b0: 6520 6f66 2074 6865 2070 6172 616d 6574  e of the paramet
-0000e3c0: 6572 7320 6973 2072 6571 7569 7265 642c  ers is required,
-0000e3d0: 2065 6974 6865 7220 6964 206f 7220 6669   either id or fi
-0000e3e0: 6c65 2e0a 0a20 2020 2020 2020 2041 7267  le...        Arg
-0000e3f0: 733a 0a20 2020 2020 2020 2020 2020 2073  s:.            s
-0000e400: 6c75 726d 5f6a 6f62 5f69 6420 2873 7472  lurm_job_id (str
-0000e410: 293a 2049 6420 6f66 2074 6865 2073 6c75  ): Id of the slu
-0000e420: 726d 206a 6f62 0a20 2020 2020 2020 2020  rm job.         
-0000e430: 2020 206c 6f67 6669 6c65 2028 7374 7229     logfile (str)
-0000e440: 3a20 5061 7468 2074 6f20 7468 6520 6c6f  : Path to the lo
-0000e450: 6766 696c 650a 0a20 2020 2020 2020 2052  gfile..        R
-0000e460: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-0000e470: 2020 2020 7374 723a 2044 6174 6120 6c6f      str: Data lo
-0000e480: 6361 7469 6f6e 2061 6363 6f72 6469 6e67  cation according
-0000e490: 2074 6f20 7468 6520 6c6f 670a 0a20 2020   to the log..   
-0000e4a0: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
-0000e4b0: 2020 2020 2020 2020 2053 5348 4578 6365           SSHExce
-0000e4c0: 7074 696f 6e3a 2049 6620 7468 6572 6520  ption: If there 
-0000e4d0: 6973 2061 6e20 6973 7375 6520 7769 7468  is an issue with
-0000e4e0: 2074 6865 2063 6f6d 6d61 6e64 2065 7865   the command exe
-0000e4f0: 6375 7469 6f6e 2e0a 2020 2020 2020 2020  cution..        
-0000e500: 2222 220a 2020 2020 2020 2020 6966 206c  """.        if l
-0000e510: 6f67 6669 6c65 2069 7320 4e6f 6e65 2061  ogfile is None a
-0000e520: 6e64 2073 6c75 726d 5f6a 6f62 5f69 6420  nd slurm_job_id 
-0000e530: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-0000e540: 2020 2020 2020 2020 206c 6f67 6669 6c65           logfile
-0000e550: 203d 2073 656c 662e 5f4c 4f47 4649 4c45   = self._LOGFILE
-0000e560: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-0000e570: 6669 6c65 203d 206c 6f67 6669 6c65 2e66  file = logfile.f
-0000e580: 6f72 6d61 7428 736c 7572 6d5f 6a6f 625f  ormat(slurm_job_
-0000e590: 6964 3d73 6c75 726d 5f6a 6f62 5f69 6429  id=slurm_job_id)
-0000e5a0: 0a20 2020 2020 2020 2063 6d64 203d 2073  .        cmd = s
-0000e5b0: 656c 662e 5f4c 4f47 4649 4c45 5f44 4154  elf._LOGFILE_DAT
-0000e5c0: 415f 434d 442e 666f 726d 6174 286c 6f67  A_CMD.format(log
-0000e5d0: 5f66 696c 653d 6c6f 6766 696c 6529 0a20  _file=logfile). 
-0000e5e0: 2020 2020 2020 2072 6573 756c 7420 3d20         result = 
-0000e5f0: 7365 6c66 2e72 756e 5f63 6f6d 6d61 6e64  self.run_command
-0000e600: 7328 5b63 6d64 5d29 0a20 2020 2020 2020  s([cmd]).       
-0000e610: 2069 6620 7265 7375 6c74 2e6f 6b3a 0a20   if result.ok:. 
-0000e620: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000e630: 6e20 7265 7375 6c74 2e73 7464 6f75 740a  n result.stdout.
-0000e640: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000e650: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-0000e660: 5353 4845 7863 6570 7469 6f6e 2872 6573  SSHException(res
-0000e670: 756c 7429 0a0a 2020 2020 6465 6620 6765  ult)..    def ge
-0000e680: 745f 776f 726b 666c 6f77 5f70 6172 616d  t_workflow_param
-0000e690: 6574 6572 7328 7365 6c66 2c0a 2020 2020  eters(self,.    
+0000e340: 2020 2020 2020 2020 2020 2020 6c6f 6766              logf
+0000e350: 696c 653a 2073 7472 203d 204e 6f6e 6529  ile: str = None)
+0000e360: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
+0000e370: 2022 2222 5265 6164 2053 4c55 524d 206a   """Read SLURM j
+0000e380: 6f62 206c 6f67 6669 6c65 2074 6f20 6669  ob logfile to fi
+0000e390: 6e64 206c 6f63 6174 696f 6e20 6f66 2074  nd location of t
+0000e3a0: 6865 2064 6174 612e 0a0a 2020 2020 2020  he data...      
+0000e3b0: 2020 4f6e 6520 6f66 2074 6865 2070 6172    One of the par
+0000e3c0: 616d 6574 6572 7320 6973 2072 6571 7569  ameters is requi
+0000e3d0: 7265 642c 2065 6974 6865 7220 6964 206f  red, either id o
+0000e3e0: 7220 6669 6c65 2e0a 0a20 2020 2020 2020  r file...       
+0000e3f0: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0000e400: 2020 2073 6c75 726d 5f6a 6f62 5f69 6420     slurm_job_id 
+0000e410: 2873 7472 293a 2049 6420 6f66 2074 6865  (str): Id of the
+0000e420: 2073 6c75 726d 206a 6f62 0a20 2020 2020   slurm job.     
+0000e430: 2020 2020 2020 206c 6f67 6669 6c65 2028         logfile (
+0000e440: 7374 7229 3a20 5061 7468 2074 6f20 7468  str): Path to th
+0000e450: 6520 6c6f 6766 696c 650a 0a20 2020 2020  e logfile..     
+0000e460: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+0000e470: 2020 2020 2020 2020 7374 723a 2044 6174          str: Dat
+0000e480: 6120 6c6f 6361 7469 6f6e 2061 6363 6f72  a location accor
+0000e490: 6469 6e67 2074 6f20 7468 6520 6c6f 670a  ding to the log.
+0000e4a0: 0a20 2020 2020 2020 2052 6169 7365 733a  .        Raises:
+0000e4b0: 0a20 2020 2020 2020 2020 2020 2053 5348  .            SSH
+0000e4c0: 4578 6365 7074 696f 6e3a 2049 6620 7468  Exception: If th
+0000e4d0: 6572 6520 6973 2061 6e20 6973 7375 6520  ere is an issue 
+0000e4e0: 7769 7468 2074 6865 2063 6f6d 6d61 6e64  with the command
+0000e4f0: 2065 7865 6375 7469 6f6e 2e0a 2020 2020   execution..    
+0000e500: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000e510: 6966 206c 6f67 6669 6c65 2069 7320 4e6f  if logfile is No
+0000e520: 6e65 2061 6e64 2073 6c75 726d 5f6a 6f62  ne and slurm_job
+0000e530: 5f69 6420 6973 206e 6f74 204e 6f6e 653a  _id is not None:
+0000e540: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+0000e550: 6669 6c65 203d 2073 656c 662e 5f4c 4f47  file = self._LOG
+0000e560: 4649 4c45 0a20 2020 2020 2020 2020 2020  FILE.           
+0000e570: 206c 6f67 6669 6c65 203d 206c 6f67 6669   logfile = logfi
+0000e580: 6c65 2e66 6f72 6d61 7428 736c 7572 6d5f  le.format(slurm_
+0000e590: 6a6f 625f 6964 3d73 6c75 726d 5f6a 6f62  job_id=slurm_job
+0000e5a0: 5f69 6429 0a20 2020 2020 2020 2063 6d64  _id).        cmd
+0000e5b0: 203d 2073 656c 662e 5f4c 4f47 4649 4c45   = self._LOGFILE
+0000e5c0: 5f44 4154 415f 434d 442e 666f 726d 6174  _DATA_CMD.format
+0000e5d0: 286c 6f67 5f66 696c 653d 6c6f 6766 696c  (log_file=logfil
+0000e5e0: 6529 0a20 2020 2020 2020 2072 6573 756c  e).        resul
+0000e5f0: 7420 3d20 7365 6c66 2e72 756e 5f63 6f6d  t = self.run_com
+0000e600: 6d61 6e64 7328 5b63 6d64 5d29 0a20 2020  mands([cmd]).   
+0000e610: 2020 2020 2069 6620 7265 7375 6c74 2e6f       if result.o
+0000e620: 6b3a 0a20 2020 2020 2020 2020 2020 2072  k:.            r
+0000e630: 6574 7572 6e20 7265 7375 6c74 2e73 7464  eturn result.std
+0000e640: 6f75 740a 2020 2020 2020 2020 656c 7365  out.        else
+0000e650: 3a0a 2020 2020 2020 2020 2020 2020 7261  :.            ra
+0000e660: 6973 6520 5353 4845 7863 6570 7469 6f6e  ise SSHException
+0000e670: 2872 6573 756c 7429 0a0a 2020 2020 6465  (result)..    de
+0000e680: 6620 6765 745f 776f 726b 666c 6f77 5f70  f get_workflow_p
+0000e690: 6172 616d 6574 6572 7328 7365 6c66 2c0a  arameters(self,.
 0000e6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6b0: 2020 2020 2020 2020 2020 2020 776f 726b              work
-0000e6c0: 666c 6f77 3a20 7374 7229 202d 3e20 4469  flow: str) -> Di
-0000e6d0: 6374 5b73 7472 2c20 4469 6374 5b73 7472  ct[str, Dict[str
-0000e6e0: 2c20 416e 795d 5d3a 0a20 2020 2020 2020  , Any]]:.       
-0000e6f0: 2022 2222 0a20 2020 2020 2020 2052 6574   """.        Ret
-0000e700: 7269 6576 6520 7468 6520 7061 7261 6d65  rieve the parame
-0000e710: 7465 7273 206f 6620 6120 776f 726b 666c  ters of a workfl
-0000e720: 6f77 2e0a 0a20 2020 2020 2020 2041 7267  ow...        Arg
-0000e730: 733a 0a20 2020 2020 2020 2020 2020 2077  s:.            w
-0000e740: 6f72 6b66 6c6f 7720 2873 7472 293a 2054  orkflow (str): T
-0000e750: 6865 2077 6f72 6b66 6c6f 7720 666f 7220  he workflow for 
-0000e760: 7768 6963 6820 746f 2072 6574 7269 6576  which to retriev
-0000e770: 6520 7468 6520 7061 7261 6d65 7465 7273  e the parameters
-0000e780: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
-0000e790: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
-0000e7a0: 4469 6374 5b73 7472 2c20 4469 6374 5b73  Dict[str, Dict[s
-0000e7b0: 7472 2c20 416e 795d 5d3a 0a20 2020 2020  tr, Any]]:.     
-0000e7c0: 2020 2020 2020 2020 2020 2041 2064 6963             A dic
-0000e7d0: 7469 6f6e 6172 7920 636f 6e74 6169 6e69  tionary containi
-0000e7e0: 6e67 2074 6865 2077 6f72 6b66 6c6f 7720  ng the workflow 
-0000e7f0: 7061 7261 6d65 7465 7273 2e0a 0a20 2020  parameters...   
-0000e800: 2020 2020 2052 6169 7365 733a 0a20 2020       Raises:.   
-0000e810: 2020 2020 2020 2020 2056 616c 7565 4572           ValueEr
-0000e820: 726f 723a 2049 6620 616e 2065 7272 6f72  ror: If an error
-0000e830: 206f 6363 7572 7320 7768 696c 6520 7265   occurs while re
-0000e840: 7472 6965 7669 6e67 2074 6865 2077 6f72  trieving the wor
-0000e850: 6b66 6c6f 770a 2020 2020 2020 2020 2020  kflow.          
-0000e860: 2020 2020 2020 7061 7261 6d65 7465 7273        parameters
-0000e870: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000e880: 2020 2020 2020 6a73 6f6e 5f64 6573 6372        json_descr
-0000e890: 6970 746f 7220 3d20 7365 6c66 2e70 756c  iptor = self.pul
-0000e8a0: 6c5f 6465 7363 7269 7074 6f72 5f66 726f  l_descriptor_fro
-0000e8b0: 6d5f 6769 7468 7562 2877 6f72 6b66 6c6f  m_github(workflo
-0000e8c0: 7729 0a20 2020 2020 2020 2023 2063 6f6e  w).        # con
-0000e8d0: 7665 7274 2074 6f20 6f6d 6572 6f20 7479  vert to omero ty
-0000e8e0: 7065 730a 2020 2020 2020 2020 6c6f 6767  pes.        logg
-0000e8f0: 6572 2e64 6562 7567 286a 736f 6e5f 6465  er.debug(json_de
-0000e900: 7363 7269 7074 6f72 290a 2020 2020 2020  scriptor).      
-0000e910: 2020 776f 726b 666c 6f77 5f64 6963 7420    workflow_dict 
-0000e920: 3d20 7b7d 0a20 2020 2020 2020 2066 6f72  = {}.        for
-0000e930: 2069 6e70 7574 2069 6e20 6a73 6f6e 5f64   input in json_d
-0000e940: 6573 6372 6970 746f 725b 2769 6e70 7574  escriptor['input
-0000e950: 7327 5d3a 0a20 2020 2020 2020 2020 2020  s']:.           
-0000e960: 2023 2066 696c 7465 7220 6379 746f 6d69   # filter cytomi
-0000e970: 6e65 2070 6172 616d 6574 6572 730a 2020  ne parameters.  
-0000e980: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-0000e990: 2069 6e70 7574 5b27 6964 275d 2e73 7461   input['id'].sta
-0000e9a0: 7274 7377 6974 6828 2763 7974 6f6d 696e  rtswith('cytomin
-0000e9b0: 6527 293a 0a20 2020 2020 2020 2020 2020  e'):.           
-0000e9c0: 2020 2020 2077 6f72 6b66 6c6f 775f 7061       workflow_pa
-0000e9d0: 7261 6d73 203d 207b 7d0a 2020 2020 2020  rams = {}.      
-0000e9e0: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
-0000e9f0: 6f77 5f70 6172 616d 735b 276e 616d 6527  ow_params['name'
-0000ea00: 5d20 3d20 696e 7075 745b 2769 6427 5d0a  ] = input['id'].
-0000ea10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ea20: 776f 726b 666c 6f77 5f70 6172 616d 735b  workflow_params[
-0000ea30: 2764 6566 6175 6c74 275d 203d 2069 6e70  'default'] = inp
-0000ea40: 7574 5b27 6465 6661 756c 742d 7661 6c75  ut['default-valu
-0000ea50: 6527 5d0a 2020 2020 2020 2020 2020 2020  e'].            
-0000ea60: 2020 2020 776f 726b 666c 6f77 5f70 6172      workflow_par
-0000ea70: 616d 735b 2763 7974 7970 6527 5d20 3d20  ams['cytype'] = 
-0000ea80: 696e 7075 745b 2774 7970 6527 5d0a 2020  input['type'].  
-0000ea90: 2020 2020 2020 2020 2020 2020 2020 776f                wo
-0000eaa0: 726b 666c 6f77 5f70 6172 616d 735b 276f  rkflow_params['o
-0000eab0: 7074 696f 6e61 6c27 5d20 3d20 696e 7075  ptional'] = inpu
-0000eac0: 745b 276f 7074 696f 6e61 6c27 5d0a 2020  t['optional'].  
-0000ead0: 2020 2020 2020 2020 2020 2020 2020 636d                cm
-0000eae0: 645f 666c 6167 203d 2069 6e70 7574 5b27  d_flag = input['
-0000eaf0: 636f 6d6d 616e 642d 6c69 6e65 2d66 6c61  command-line-fla
-0000eb00: 6727 5d0a 2020 2020 2020 2020 2020 2020  g'].            
-0000eb10: 2020 2020 636d 645f 666c 6167 203d 2063      cmd_flag = c
-0000eb20: 6d64 5f66 6c61 672e 7265 706c 6163 6528  md_flag.replace(
-0000eb30: 2240 6964 222c 2069 6e70 7574 5b27 6964  "@id", input['id
-0000eb40: 275d 290a 2020 2020 2020 2020 2020 2020  ']).            
-0000eb50: 2020 2020 776f 726b 666c 6f77 5f70 6172      workflow_par
-0000eb60: 616d 735b 2763 6d64 5f66 6c61 6727 5d20  ams['cmd_flag'] 
-0000eb70: 3d20 636d 645f 666c 6167 0a20 2020 2020  = cmd_flag.     
-0000eb80: 2020 2020 2020 2020 2020 2077 6f72 6b66             workf
-0000eb90: 6c6f 775f 7061 7261 6d73 5b27 6465 7363  low_params['desc
-0000eba0: 7269 7074 696f 6e27 5d20 3d20 696e 7075  ription'] = inpu
-0000ebb0: 745b 2764 6573 6372 6970 7469 6f6e 275d  t['description']
-0000ebc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ebd0: 2077 6f72 6b66 6c6f 775f 6469 6374 5b69   workflow_dict[i
-0000ebe0: 6e70 7574 5b27 6964 275d 5d20 3d20 776f  nput['id']] = wo
-0000ebf0: 726b 666c 6f77 5f70 6172 616d 730a 2020  rkflow_params.  
-0000ec00: 2020 2020 2020 7265 7475 726e 2077 6f72        return wor
-0000ec10: 6b66 6c6f 775f 6469 6374 0a0a 2020 2020  kflow_dict..    
-0000ec20: 6465 6620 636f 6e76 6572 745f 6379 7479  def convert_cyty
-0000ec30: 7065 5f74 6f5f 6f6d 7479 7065 2873 656c  pe_to_omtype(sel
-0000ec40: 662c 0a20 2020 2020 2020 2020 2020 2020  f,.             
+0000e6b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6c0: 776f 726b 666c 6f77 3a20 7374 7229 202d  workflow: str) -
+0000e6d0: 3e20 4469 6374 5b73 7472 2c20 4469 6374  > Dict[str, Dict
+0000e6e0: 5b73 7472 2c20 416e 795d 5d3a 0a20 2020  [str, Any]]:.   
+0000e6f0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000e700: 2052 6574 7269 6576 6520 7468 6520 7061   Retrieve the pa
+0000e710: 7261 6d65 7465 7273 206f 6620 6120 776f  rameters of a wo
+0000e720: 726b 666c 6f77 2e0a 0a20 2020 2020 2020  rkflow...       
+0000e730: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+0000e740: 2020 2077 6f72 6b66 6c6f 7720 2873 7472     workflow (str
+0000e750: 293a 2054 6865 2077 6f72 6b66 6c6f 7720  ): The workflow 
+0000e760: 666f 7220 7768 6963 6820 746f 2072 6574  for which to ret
+0000e770: 7269 6576 6520 7468 6520 7061 7261 6d65  rieve the parame
+0000e780: 7465 7273 2e0a 0a20 2020 2020 2020 2052  ters...        R
+0000e790: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+0000e7a0: 2020 2020 4469 6374 5b73 7472 2c20 4469      Dict[str, Di
+0000e7b0: 6374 5b73 7472 2c20 416e 795d 5d3a 0a20  ct[str, Any]]:. 
+0000e7c0: 2020 2020 2020 2020 2020 2020 2020 2041                 A
+0000e7d0: 2064 6963 7469 6f6e 6172 7920 636f 6e74   dictionary cont
+0000e7e0: 6169 6e69 6e67 2074 6865 2077 6f72 6b66  aining the workf
+0000e7f0: 6c6f 7720 7061 7261 6d65 7465 7273 2e0a  low parameters..
+0000e800: 0a20 2020 2020 2020 2052 6169 7365 733a  .        Raises:
+0000e810: 0a20 2020 2020 2020 2020 2020 2056 616c  .            Val
+0000e820: 7565 4572 726f 723a 2049 6620 616e 2065  ueError: If an e
+0000e830: 7272 6f72 206f 6363 7572 7320 7768 696c  rror occurs whil
+0000e840: 6520 7265 7472 6965 7669 6e67 2074 6865  e retrieving the
+0000e850: 2077 6f72 6b66 6c6f 770a 2020 2020 2020   workflow.      
+0000e860: 2020 2020 2020 2020 2020 7061 7261 6d65            parame
+0000e870: 7465 7273 2e0a 2020 2020 2020 2020 2222  ters..        ""
+0000e880: 220a 2020 2020 2020 2020 6a73 6f6e 5f64  ".        json_d
+0000e890: 6573 6372 6970 746f 7220 3d20 7365 6c66  escriptor = self
+0000e8a0: 2e70 756c 6c5f 6465 7363 7269 7074 6f72  .pull_descriptor
+0000e8b0: 5f66 726f 6d5f 6769 7468 7562 2877 6f72  _from_github(wor
+0000e8c0: 6b66 6c6f 7729 0a20 2020 2020 2020 2023  kflow).        #
+0000e8d0: 2063 6f6e 7665 7274 2074 6f20 6f6d 6572   convert to omer
+0000e8e0: 6f20 7479 7065 730a 2020 2020 2020 2020  o types.        
+0000e8f0: 6c6f 6767 6572 2e64 6562 7567 286a 736f  logger.debug(jso
+0000e900: 6e5f 6465 7363 7269 7074 6f72 290a 2020  n_descriptor).  
+0000e910: 2020 2020 2020 776f 726b 666c 6f77 5f64        workflow_d
+0000e920: 6963 7420 3d20 7b7d 0a20 2020 2020 2020  ict = {}.       
+0000e930: 2066 6f72 2069 6e70 7574 2069 6e20 6a73   for input in js
+0000e940: 6f6e 5f64 6573 6372 6970 746f 725b 2769  on_descriptor['i
+0000e950: 6e70 7574 7327 5d3a 0a20 2020 2020 2020  nputs']:.       
+0000e960: 2020 2020 2023 2066 696c 7465 7220 6379       # filter cy
+0000e970: 746f 6d69 6e65 2070 6172 616d 6574 6572  tomine parameter
+0000e980: 730a 2020 2020 2020 2020 2020 2020 6966  s.            if
+0000e990: 206e 6f74 2069 6e70 7574 5b27 6964 275d   not input['id']
+0000e9a0: 2e73 7461 7274 7377 6974 6828 2763 7974  .startswith('cyt
+0000e9b0: 6f6d 696e 6527 293a 0a20 2020 2020 2020  omine'):.       
+0000e9c0: 2020 2020 2020 2020 2077 6f72 6b66 6c6f           workflo
+0000e9d0: 775f 7061 7261 6d73 203d 207b 7d0a 2020  w_params = {}.  
+0000e9e0: 2020 2020 2020 2020 2020 2020 2020 776f                wo
+0000e9f0: 726b 666c 6f77 5f70 6172 616d 735b 276e  rkflow_params['n
+0000ea00: 616d 6527 5d20 3d20 696e 7075 745b 2769  ame'] = input['i
+0000ea10: 6427 5d0a 2020 2020 2020 2020 2020 2020  d'].            
+0000ea20: 2020 2020 776f 726b 666c 6f77 5f70 6172      workflow_par
+0000ea30: 616d 735b 2764 6566 6175 6c74 275d 203d  ams['default'] =
+0000ea40: 2069 6e70 7574 5b27 6465 6661 756c 742d   input['default-
+0000ea50: 7661 6c75 6527 5d0a 2020 2020 2020 2020  value'].        
+0000ea60: 2020 2020 2020 2020 776f 726b 666c 6f77          workflow
+0000ea70: 5f70 6172 616d 735b 2763 7974 7970 6527  _params['cytype'
+0000ea80: 5d20 3d20 696e 7075 745b 2774 7970 6527  ] = input['type'
+0000ea90: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000eaa0: 2020 776f 726b 666c 6f77 5f70 6172 616d    workflow_param
+0000eab0: 735b 276f 7074 696f 6e61 6c27 5d20 3d20  s['optional'] = 
+0000eac0: 696e 7075 745b 276f 7074 696f 6e61 6c27  input['optional'
+0000ead0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+0000eae0: 2020 636d 645f 666c 6167 203d 2069 6e70    cmd_flag = inp
+0000eaf0: 7574 5b27 636f 6d6d 616e 642d 6c69 6e65  ut['command-line
+0000eb00: 2d66 6c61 6727 5d0a 2020 2020 2020 2020  -flag'].        
+0000eb10: 2020 2020 2020 2020 636d 645f 666c 6167          cmd_flag
+0000eb20: 203d 2063 6d64 5f66 6c61 672e 7265 706c   = cmd_flag.repl
+0000eb30: 6163 6528 2240 6964 222c 2069 6e70 7574  ace("@id", input
+0000eb40: 5b27 6964 275d 290a 2020 2020 2020 2020  ['id']).        
+0000eb50: 2020 2020 2020 2020 776f 726b 666c 6f77          workflow
+0000eb60: 5f70 6172 616d 735b 2763 6d64 5f66 6c61  _params['cmd_fla
+0000eb70: 6727 5d20 3d20 636d 645f 666c 6167 0a20  g'] = cmd_flag. 
+0000eb80: 2020 2020 2020 2020 2020 2020 2020 2077                 w
+0000eb90: 6f72 6b66 6c6f 775f 7061 7261 6d73 5b27  orkflow_params['
+0000eba0: 6465 7363 7269 7074 696f 6e27 5d20 3d20  description'] = 
+0000ebb0: 696e 7075 745b 2764 6573 6372 6970 7469  input['descripti
+0000ebc0: 6f6e 275d 0a20 2020 2020 2020 2020 2020  on'].           
+0000ebd0: 2020 2020 2077 6f72 6b66 6c6f 775f 6469       workflow_di
+0000ebe0: 6374 5b69 6e70 7574 5b27 6964 275d 5d20  ct[input['id']] 
+0000ebf0: 3d20 776f 726b 666c 6f77 5f70 6172 616d  = workflow_param
+0000ec00: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
+0000ec10: 2077 6f72 6b66 6c6f 775f 6469 6374 0a0a   workflow_dict..
+0000ec20: 2020 2020 6465 6620 636f 6e76 6572 745f      def convert_
+0000ec30: 6379 7479 7065 5f74 6f5f 6f6d 7479 7065  cytype_to_omtype
+0000ec40: 2873 656c 662c 0a20 2020 2020 2020 2020  (self,.         
 0000ec50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ec60: 2020 2020 6379 7479 7065 3a20 7374 722c      cytype: str,
-0000ec70: 205f 6465 6661 756c 742c 202a 6172 6773   _default, *args
-0000ec80: 2c20 2a2a 6b77 6172 6773 0a20 2020 2020  , **kwargs.     
+0000ec60: 2020 2020 2020 2020 6379 7479 7065 3a20          cytype: 
+0000ec70: 7374 722c 205f 6465 6661 756c 742c 202a  str, _default, *
+0000ec80: 6172 6773 2c20 2a2a 6b77 6172 6773 0a20  args, **kwargs. 
 0000ec90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eca0: 2020 2020 2020 2020 2020 2020 2920 2d3e              ) ->
-0000ecb0: 2041 6e79 3a0a 2020 2020 2020 2020 2222   Any:.        ""
-0000ecc0: 220a 2020 2020 2020 2020 436f 6e76 6572  ".        Conver
-0000ecd0: 7420 6120 4379 746f 6d69 6e65 2074 7970  t a Cytomine typ
-0000ece0: 6520 746f 2061 6e20 4f4d 4552 4f20 7479  e to an OMERO ty
-0000ecf0: 7065 2061 6e64 2069 6e73 7461 6e74 6961  pe and instantia
-0000ed00: 7465 7320 6974 0a20 2020 2020 2020 2077  tes it.        w
-0000ed10: 6974 6820 6172 6773 2f6b 7761 7267 732e  ith args/kwargs.
-0000ed20: 0a0a 2020 2020 2020 2020 4e6f 7465 2074  ..        Note t
-0000ed30: 6861 7420 4379 746f 6d69 6e65 2068 6173  hat Cytomine has
-0000ed40: 2061 2050 7974 686f 6e20 436c 6965 6e74   a Python Client
-0000ed50: 2c20 616e 6420 736f 6d65 2063 6f6e 7665  , and some conve
-0000ed60: 7273 696f 6e20 6d65 7468 6f64 730a 2020  rsion methods.  
-0000ed70: 2020 2020 2020 746f 2070 7974 686f 6e20        to python 
-0000ed80: 7479 7065 732c 2062 7574 206e 6f74 6869  types, but nothi
-0000ed90: 6e67 2070 6172 7469 6375 6c61 726c 7920  ng particularly 
-0000eda0: 776f 7274 6820 6465 7065 6e64 696e 6720  worth depending 
-0000edb0: 6f6e 2074 6861 740a 2020 2020 2020 2020  on that.        
-0000edc0: 6c69 6272 6172 7920 666f 7220 7965 742e  library for yet.
-0000edd0: 204d 6967 6874 2062 6520 7573 6566 756c   Might be useful
-0000ede0: 2069 6e20 7468 6520 6675 7475 7265 2070   in the future p
-0000edf0: 6572 6861 7073 2e0a 2020 2020 2020 2020  erhaps..        
-0000ee00: 2865 2e67 2e20 6874 7470 733a 2f2f 6769  (e.g. https://gi
-0000ee10: 7468 7562 2e63 6f6d 2f43 7974 6f6d 696e  thub.com/Cytomin
-0000ee20: 652d 554c 6965 6765 2f43 7974 6f6d 696e  e-ULiege/Cytomin
-0000ee30: 652d 7079 7468 6f6e 2d63 6c69 656e 742f  e-python-client/
-0000ee40: 0a20 2020 2020 2020 2062 6c6f 622f 6d61  .        blob/ma
-0000ee50: 7374 6572 2f63 7974 6f6d 696e 652f 6379  ster/cytomine/cy
-0000ee60: 746f 6d69 6e65 5f6a 6f62 2e70 7929 0a0a  tomine_job.py)..
-0000ee70: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-0000ee80: 2020 2020 2020 2020 2020 6379 7479 7065            cytype
-0000ee90: 2028 7374 7229 3a20 5468 6520 4379 746f   (str): The Cyto
-0000eea0: 6d69 6e65 2074 7970 6520 746f 2063 6f6e  mine type to con
-0000eeb0: 7665 7274 2e0a 2020 2020 2020 2020 2020  vert..          
-0000eec0: 2020 5f64 6566 6175 6c74 3a20 5468 6520    _default: The 
-0000eed0: 6465 6661 756c 7420 7661 6c75 652e 2052  default value. R
-0000eee0: 6571 7569 7265 6420 746f 2064 6973 7469  equired to disti
-0000eef0: 6e67 7569 7368 2062 6574 7765 656e 2066  nguish between f
-0000ef00: 6c6f 6174 0a20 2020 2020 2020 2020 2020  loat.           
-0000ef10: 2020 2020 2061 6e64 2069 6e74 2e0a 2020       and int..  
-0000ef20: 2020 2020 2020 2020 2020 2a61 7267 733a            *args:
-0000ef30: 2041 6464 6974 696f 6e61 6c20 706f 7369   Additional posi
-0000ef40: 7469 6f6e 616c 2061 7267 756d 656e 7473  tional arguments
-0000ef50: 2e0a 2020 2020 2020 2020 2020 2020 2a2a  ..            **
-0000ef60: 6b77 6172 6773 3a20 4164 6469 7469 6f6e  kwargs: Addition
-0000ef70: 616c 206b 6579 776f 7264 2061 7267 756d  al keyword argum
-0000ef80: 656e 7473 2e0a 0a20 2020 2020 2020 2052  ents...        R
-0000ef90: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-0000efa0: 2020 2020 416e 793a 0a20 2020 2020 2020      Any:.       
-0000efb0: 2020 2020 2020 2020 2054 6865 2063 6f6e           The con
-0000efc0: 7665 7274 6564 204f 4d45 524f 2074 7970  verted OMERO typ
-0000efd0: 6520 636c 6173 7320 696e 7374 616e 6365  e class instance
-0000efe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000eff0: 206f 7220 4e6f 6e65 2069 6620 6572 726f   or None if erro
-0000f000: 7273 206f 6363 7572 6564 2e0a 0a20 2020  rs occured...   
-0000f010: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000f020: 2023 2054 4f44 4f20 6d61 6b65 2045 6e75   # TODO make Enu
-0000f030: 6d20 3f0a 2020 2020 2020 2020 6966 2063  m ?.        if c
-0000f040: 7974 7970 6520 3d3d 2027 4e75 6d62 6572  ytype == 'Number
-0000f050: 273a 0a20 2020 2020 2020 2020 2020 2069  ':.            i
-0000f060: 6620 6973 696e 7374 616e 6365 285f 6465  f isinstance(_de
-0000f070: 6661 756c 742c 2066 6c6f 6174 293a 0a20  fault, float):. 
-0000f080: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-0000f090: 2066 6c6f 6174 2069 6e73 7465 6164 0a20   float instead. 
-0000f0a0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000f0b0: 6574 7572 6e20 7365 6c66 2e73 7472 5f74  eturn self.str_t
-0000f0c0: 6f5f 636c 6173 7328 226f 6d65 726f 2e73  o_class("omero.s
-0000f0d0: 6372 6970 7473 222c 2022 466c 6f61 7422  cripts", "Float"
-0000f0e0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000eca0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ecb0: 2920 2d3e 2041 6e79 3a0a 2020 2020 2020  ) -> Any:.      
+0000ecc0: 2020 2222 220a 2020 2020 2020 2020 436f    """.        Co
+0000ecd0: 6e76 6572 7420 6120 4379 746f 6d69 6e65  nvert a Cytomine
+0000ece0: 2074 7970 6520 746f 2061 6e20 4f4d 4552   type to an OMER
+0000ecf0: 4f20 7479 7065 2061 6e64 2069 6e73 7461  O type and insta
+0000ed00: 6e74 6961 7465 7320 6974 0a20 2020 2020  ntiates it.     
+0000ed10: 2020 2077 6974 6820 6172 6773 2f6b 7761     with args/kwa
+0000ed20: 7267 732e 0a0a 2020 2020 2020 2020 4e6f  rgs...        No
+0000ed30: 7465 2074 6861 7420 4379 746f 6d69 6e65  te that Cytomine
+0000ed40: 2068 6173 2061 2050 7974 686f 6e20 436c   has a Python Cl
+0000ed50: 6965 6e74 2c20 616e 6420 736f 6d65 2063  ient, and some c
+0000ed60: 6f6e 7665 7273 696f 6e20 6d65 7468 6f64  onversion method
+0000ed70: 730a 2020 2020 2020 2020 746f 2070 7974  s.        to pyt
+0000ed80: 686f 6e20 7479 7065 732c 2062 7574 206e  hon types, but n
+0000ed90: 6f74 6869 6e67 2070 6172 7469 6375 6c61  othing particula
+0000eda0: 726c 7920 776f 7274 6820 6465 7065 6e64  rly worth depend
+0000edb0: 696e 6720 6f6e 2074 6861 740a 2020 2020  ing on that.    
+0000edc0: 2020 2020 6c69 6272 6172 7920 666f 7220      library for 
+0000edd0: 7965 742e 204d 6967 6874 2062 6520 7573  yet. Might be us
+0000ede0: 6566 756c 2069 6e20 7468 6520 6675 7475  eful in the futu
+0000edf0: 7265 2070 6572 6861 7073 2e0a 2020 2020  re perhaps..    
+0000ee00: 2020 2020 2865 2e67 2e20 6874 7470 733a      (e.g. https:
+0000ee10: 2f2f 6769 7468 7562 2e63 6f6d 2f43 7974  //github.com/Cyt
+0000ee20: 6f6d 696e 652d 554c 6965 6765 2f43 7974  omine-ULiege/Cyt
+0000ee30: 6f6d 696e 652d 7079 7468 6f6e 2d63 6c69  omine-python-cli
+0000ee40: 656e 742f 0a20 2020 2020 2020 2062 6c6f  ent/.        blo
+0000ee50: 622f 6d61 7374 6572 2f63 7974 6f6d 696e  b/master/cytomin
+0000ee60: 652f 6379 746f 6d69 6e65 5f6a 6f62 2e70  e/cytomine_job.p
+0000ee70: 7929 0a0a 2020 2020 2020 2020 4172 6773  y)..        Args
+0000ee80: 3a0a 2020 2020 2020 2020 2020 2020 6379  :.            cy
+0000ee90: 7479 7065 2028 7374 7229 3a20 5468 6520  type (str): The 
+0000eea0: 4379 746f 6d69 6e65 2074 7970 6520 746f  Cytomine type to
+0000eeb0: 2063 6f6e 7665 7274 2e0a 2020 2020 2020   convert..      
+0000eec0: 2020 2020 2020 5f64 6566 6175 6c74 3a20        _default: 
+0000eed0: 5468 6520 6465 6661 756c 7420 7661 6c75  The default valu
+0000eee0: 652e 2052 6571 7569 7265 6420 746f 2064  e. Required to d
+0000eef0: 6973 7469 6e67 7569 7368 2062 6574 7765  istinguish betwe
+0000ef00: 656e 2066 6c6f 6174 0a20 2020 2020 2020  en float.       
+0000ef10: 2020 2020 2020 2020 2061 6e64 2069 6e74           and int
+0000ef20: 2e0a 2020 2020 2020 2020 2020 2020 2a61  ..            *a
+0000ef30: 7267 733a 2041 6464 6974 696f 6e61 6c20  rgs: Additional 
+0000ef40: 706f 7369 7469 6f6e 616c 2061 7267 756d  positional argum
+0000ef50: 656e 7473 2e0a 2020 2020 2020 2020 2020  ents..          
+0000ef60: 2020 2a2a 6b77 6172 6773 3a20 4164 6469    **kwargs: Addi
+0000ef70: 7469 6f6e 616c 206b 6579 776f 7264 2061  tional keyword a
+0000ef80: 7267 756d 656e 7473 2e0a 0a20 2020 2020  rguments...     
+0000ef90: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+0000efa0: 2020 2020 2020 2020 416e 793a 0a20 2020          Any:.   
+0000efb0: 2020 2020 2020 2020 2020 2020 2054 6865               The
+0000efc0: 2063 6f6e 7665 7274 6564 204f 4d45 524f   converted OMERO
+0000efd0: 2074 7970 6520 636c 6173 7320 696e 7374   type class inst
+0000efe0: 616e 6365 0a20 2020 2020 2020 2020 2020  ance.           
+0000eff0: 2020 2020 206f 7220 4e6f 6e65 2069 6620       or None if 
+0000f000: 6572 726f 7273 206f 6363 7572 6564 2e0a  errors occured..
+0000f010: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000f020: 2020 2020 2023 2054 4f44 4f20 6d61 6b65       # TODO make
+0000f030: 2045 6e75 6d20 3f0a 2020 2020 2020 2020   Enum ?.        
+0000f040: 6966 2063 7974 7970 6520 3d3d 2027 4e75  if cytype == 'Nu
+0000f050: 6d62 6572 273a 0a20 2020 2020 2020 2020  mber':.         
+0000f060: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+0000f070: 285f 6465 6661 756c 742c 2066 6c6f 6174  (_default, float
+0000f080: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+0000f090: 2020 2023 2066 6c6f 6174 2069 6e73 7465     # float inste
+0000f0a0: 6164 0a20 2020 2020 2020 2020 2020 2020  ad.             
+0000f0b0: 2020 2072 6574 7572 6e20 7365 6c66 2e73     return self.s
+0000f0c0: 7472 5f74 6f5f 636c 6173 7328 226f 6d65  tr_to_class("ome
+0000f0d0: 726f 2e73 6372 6970 7473 222c 2022 466c  ro.scripts", "Fl
+0000f0e0: 6f61 7422 2c0a 2020 2020 2020 2020 2020  oat",.          
 0000f0f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f100: 2020 2020 2020 2020 2020 202a 6172 6773             *args
-0000f110: 2c20 2a2a 6b77 6172 6773 290a 2020 2020  , **kwargs).    
-0000f120: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000f130: 2020 2020 2020 2020 2020 2020 2020 7265                re
-0000f140: 7475 726e 2073 656c 662e 7374 725f 746f  turn self.str_to
-0000f150: 5f63 6c61 7373 2822 6f6d 6572 6f2e 7363  _class("omero.sc
-0000f160: 7269 7074 7322 2c20 2249 6e74 222c 0a20  ripts", "Int",. 
-0000f170: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f100: 2020 2020 2020 2020 2020 2020 2020 202a                 *
+0000f110: 6172 6773 2c20 2a2a 6b77 6172 6773 290a  args, **kwargs).
+0000f120: 2020 2020 2020 2020 2020 2020 656c 7365              else
+0000f130: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000f140: 2020 7265 7475 726e 2073 656c 662e 7374    return self.st
+0000f150: 725f 746f 5f63 6c61 7373 2822 6f6d 6572  r_to_class("omer
+0000f160: 6f2e 7363 7269 7074 7322 2c20 2249 6e74  o.scripts", "Int
+0000f170: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
 0000f180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f190: 2020 2020 2020 2020 2a61 7267 732c 202a          *args, *
-0000f1a0: 2a6b 7761 7267 7329 0a20 2020 2020 2020  *kwargs).       
-0000f1b0: 2065 6c69 6620 6379 7479 7065 203d 3d20   elif cytype == 
-0000f1c0: 2742 6f6f 6c65 616e 273a 0a20 2020 2020  'Boolean':.     
-0000f1d0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-0000f1e0: 6c66 2e73 7472 5f74 6f5f 636c 6173 7328  lf.str_to_class(
-0000f1f0: 226f 6d65 726f 2e73 6372 6970 7473 222c  "omero.scripts",
-0000f200: 2022 426f 6f6c 222c 0a20 2020 2020 2020   "Bool",.       
+0000f190: 2020 2020 2020 2020 2020 2020 2a61 7267              *arg
+0000f1a0: 732c 202a 2a6b 7761 7267 7329 0a20 2020  s, **kwargs).   
+0000f1b0: 2020 2020 2065 6c69 6620 6379 7479 7065       elif cytype
+0000f1c0: 203d 3d20 2742 6f6f 6c65 616e 273a 0a20   == 'Boolean':. 
+0000f1d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000f1e0: 6e20 7365 6c66 2e73 7472 5f74 6f5f 636c  n self.str_to_cl
+0000f1f0: 6173 7328 226f 6d65 726f 2e73 6372 6970  ass("omero.scrip
+0000f200: 7473 222c 2022 426f 6f6c 222c 0a20 2020  ts", "Bool",.   
 0000f210: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f220: 2020 2020 2020 2020 2020 2020 2020 2a61                *a
-0000f230: 7267 732c 202a 2a6b 7761 7267 7329 0a20  rgs, **kwargs). 
-0000f240: 2020 2020 2020 2065 6c69 6620 6379 7479         elif cyty
-0000f250: 7065 203d 3d20 2753 7472 696e 6727 3a0a  pe == 'String':.
-0000f260: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000f270: 726e 2073 656c 662e 7374 725f 746f 5f63  rn self.str_to_c
-0000f280: 6c61 7373 2822 6f6d 6572 6f2e 7363 7269  lass("omero.scri
-0000f290: 7074 7322 2c20 2253 7472 696e 6722 2c0a  pts", "String",.
-0000f2a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f230: 2020 2a61 7267 732c 202a 2a6b 7761 7267    *args, **kwarg
+0000f240: 7329 0a20 2020 2020 2020 2065 6c69 6620  s).        elif 
+0000f250: 6379 7479 7065 203d 3d20 2753 7472 696e  cytype == 'Strin
+0000f260: 6727 3a0a 2020 2020 2020 2020 2020 2020  g':.            
+0000f270: 7265 7475 726e 2073 656c 662e 7374 725f  return self.str_
+0000f280: 746f 5f63 6c61 7373 2822 6f6d 6572 6f2e  to_class("omero.
+0000f290: 7363 7269 7074 7322 2c20 2253 7472 696e  scripts", "Strin
+0000f2a0: 6722 2c0a 2020 2020 2020 2020 2020 2020  g",.            
 0000f2b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f2c0: 2020 2020 202a 6172 6773 2c20 2a2a 6b77       *args, **kw
-0000f2d0: 6172 6773 290a 0a20 2020 2064 6566 2065  args)..    def e
-0000f2e0: 7874 7261 6374 5f70 6172 7473 5f66 726f  xtract_parts_fro
-0000f2f0: 6d5f 7572 6c28 7365 6c66 2c20 696e 7075  m_url(self, inpu
-0000f300: 745f 7572 6c3a 2073 7472 2920 2d3e 2054  t_url: str) -> T
-0000f310: 7570 6c65 5b4c 6973 745b 7374 725d 2c20  uple[List[str], 
-0000f320: 7374 725d 3a0a 2020 2020 2020 2020 2222  str]:.        ""
-0000f330: 220a 2020 2020 2020 2020 4578 7472 6163  ".        Extrac
-0000f340: 7420 7468 6520 7265 706f 7369 746f 7279  t the repository
-0000f350: 2061 6e64 2062 7261 6e63 6820 696e 666f   and branch info
-0000f360: 726d 6174 696f 6e20 6672 6f6d 2074 6865  rmation from the
-0000f370: 2069 6e70 7574 2055 524c 2e0a 0a20 2020   input URL...   
-0000f380: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-0000f390: 2020 2020 2020 2069 6e70 7574 5f75 726c         input_url
-0000f3a0: 2028 7374 7229 3a20 5468 6520 696e 7075   (str): The inpu
-0000f3b0: 7420 4769 7448 7562 2055 524c 2e0a 0a20  t GitHub URL... 
-0000f3c0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-0000f3d0: 2020 2020 2020 2020 2020 2020 5475 706c              Tupl
-0000f3e0: 655b 4c69 7374 5b73 7472 5d2c 2073 7472  e[List[str], str
-0000f3f0: 5d3a 0a20 2020 2020 2020 2020 2020 2020  ]:.             
-0000f400: 2020 2054 6865 206c 6973 7420 6f66 2075     The list of u
-0000f410: 726c 2070 6172 7473 2061 6e64 2074 6865  rl parts and the
-0000f420: 2062 7261 6e63 682f 7665 7273 696f 6e2e   branch/version.
-0000f430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f440: 2049 6620 6e6f 2062 7261 6e63 6820 6973   If no branch is
-0000f450: 2066 6f75 6e64 2c20 6974 2077 696c 6c20   found, it will 
-0000f460: 7265 7475 726e 2022 6d61 7374 6572 220a  return "master".
-0000f470: 0a20 2020 2020 2020 2052 6169 7365 733a  .        Raises:
-0000f480: 0a20 2020 2020 2020 2020 2020 2056 616c  .            Val
-0000f490: 7565 4572 726f 723a 2049 6620 7468 6520  ueError: If the 
-0000f4a0: 696e 7075 7420 5552 4c20 6973 206e 6f74  input URL is not
-0000f4b0: 2061 2076 616c 6964 2047 6974 4875 6220   a valid GitHub 
-0000f4c0: 5552 4c2e 0a20 2020 2020 2020 2022 2222  URL..        """
-0000f4d0: 0a20 2020 2020 2020 2075 726c 5f70 6172  .        url_par
-0000f4e0: 7473 203d 2069 6e70 7574 5f75 726c 2e73  ts = input_url.s
-0000f4f0: 706c 6974 2822 2f22 290a 2020 2020 2020  plit("/").      
-0000f500: 2020 6966 206c 656e 2875 726c 5f70 6172    if len(url_par
-0000f510: 7473 2920 3c20 3520 6f72 2075 726c 5f70  ts) < 5 or url_p
-0000f520: 6172 7473 5b32 5d20 213d 2022 6769 7468  arts[2] != "gith
-0000f530: 7562 2e63 6f6d 223a 0a20 2020 2020 2020  ub.com":.       
-0000f540: 2020 2020 2072 6169 7365 2056 616c 7565       raise Value
-0000f550: 4572 726f 7228 2249 6e76 616c 6964 2047  Error("Invalid G
-0000f560: 6974 4875 6220 5552 4c22 290a 0a20 2020  itHub URL")..   
-0000f570: 2020 2020 2069 6620 2274 7265 6522 2069       if "tree" i
-0000f580: 6e20 7572 6c5f 7061 7274 733a 0a20 2020  n url_parts:.   
-0000f590: 2020 2020 2020 2020 2023 2043 6173 653a           # Case:
-0000f5a0: 2055 524c 2063 6f6e 7461 696e 7320 6120   URL contains a 
-0000f5b0: 6272 616e 6368 0a20 2020 2020 2020 2020  branch.         
-0000f5c0: 2020 2062 7261 6e63 685f 696e 6465 7820     branch_index 
-0000f5d0: 3d20 7572 6c5f 7061 7274 732e 696e 6465  = url_parts.inde
-0000f5e0: 7828 2274 7265 6522 2920 2b20 310a 2020  x("tree") + 1.  
-0000f5f0: 2020 2020 2020 2020 2020 6272 616e 6368            branch
-0000f600: 203d 2075 726c 5f70 6172 7473 5b62 7261   = url_parts[bra
-0000f610: 6e63 685f 696e 6465 785d 0a20 2020 2020  nch_index].     
-0000f620: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-0000f630: 2020 2020 2023 2043 6173 653a 2055 524c       # Case: URL
-0000f640: 2064 6f65 7320 6e6f 7420 7370 6563 6966   does not specif
-0000f650: 7920 6120 6272 616e 6368 0a20 2020 2020  y a branch.     
-0000f660: 2020 2020 2020 2062 7261 6e63 6820 3d20         branch = 
-0000f670: 226d 6173 7465 7222 0a0a 2020 2020 2020  "master"..      
-0000f680: 2020 7265 7475 726e 2075 726c 5f70 6172    return url_par
-0000f690: 7473 2c20 6272 616e 6368 0a0a 2020 2020  ts, branch..    
-0000f6a0: 6465 6620 636f 6e76 6572 745f 7572 6c28  def convert_url(
-0000f6b0: 7365 6c66 2c20 696e 7075 745f 7572 6c3a  self, input_url:
-0000f6c0: 2073 7472 2920 2d3e 2073 7472 3a0a 2020   str) -> str:.  
-0000f6d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-0000f6e0: 2020 436f 6e76 6572 7420 7468 6520 696e    Convert the in
-0000f6f0: 7075 7420 4769 7448 7562 2055 524c 2074  put GitHub URL t
-0000f700: 6f20 616e 206f 7574 7075 7420 5552 4c20  o an output URL 
-0000f710: 7468 6174 2072 6574 7269 6576 6573 0a20  that retrieves. 
-0000f720: 2020 2020 2020 2074 6865 2027 6465 7363         the 'desc
-0000f730: 7269 7074 6f72 2e6a 736f 6e27 2066 696c  riptor.json' fil
-0000f740: 6520 696e 2072 6177 2066 6f72 6d61 742e  e in raw format.
-0000f750: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-0000f760: 2020 2020 2020 2020 2020 2020 696e 7075              inpu
-0000f770: 745f 7572 6c20 2873 7472 293a 2054 6865  t_url (str): The
-0000f780: 2069 6e70 7574 2047 6974 4875 6220 5552   input GitHub UR
-0000f790: 4c2e 0a0a 2020 2020 2020 2020 5265 7475  L...        Retu
-0000f7a0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-0000f7b0: 2073 7472 3a20 5468 6520 6f75 7470 7574   str: The output
-0000f7c0: 2055 524c 2074 6f20 7468 6520 2764 6573   URL to the 'des
-0000f7d0: 6372 6970 746f 722e 6a73 6f6e 2720 6669  criptor.json' fi
-0000f7e0: 6c65 2e0a 0a20 2020 2020 2020 2052 6169  le...        Rai
-0000f7f0: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
-0000f800: 2056 616c 7565 4572 726f 723a 2049 6620   ValueError: If 
-0000f810: 7468 6520 696e 7075 7420 5552 4c20 6973  the input URL is
-0000f820: 206e 6f74 2061 2076 616c 6964 2047 6974   not a valid Git
-0000f830: 4875 6220 5552 4c2e 0a20 2020 2020 2020  Hub URL..       
-0000f840: 2022 2222 0a20 2020 2020 2020 2075 726c   """.        url
-0000f850: 5f70 6172 7473 2c20 6272 616e 6368 203d  _parts, branch =
-0000f860: 2073 656c 662e 6578 7472 6163 745f 7061   self.extract_pa
-0000f870: 7274 735f 6672 6f6d 5f75 726c 2869 6e70  rts_from_url(inp
-0000f880: 7574 5f75 726c 290a 0a20 2020 2020 2020  ut_url)..       
-0000f890: 2023 2043 6f6e 7374 7275 6374 2074 6865   # Construct the
-0000f8a0: 206f 7574 7075 7420 5552 4c20 6279 2063   output URL by c
-0000f8b0: 6f6d 6269 6e69 6e67 2074 6865 2065 7874  ombining the ext
-0000f8c0: 7261 6374 6564 2069 6e66 6f72 6d61 7469  racted informati
-0000f8d0: 6f6e 0a20 2020 2020 2020 2023 2077 6974  on.        # wit
-0000f8e0: 6820 7468 6520 6465 7369 7265 6420 6669  h the desired fi
-0000f8f0: 6c65 2070 6174 680a 2020 2020 2020 2020  le path.        
-0000f900: 6f75 7470 7574 5f75 726c 203d 2066 2268  output_url = f"h
-0000f910: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-0000f920: 6d2f 7b75 726c 5f70 6172 7473 5b33 5d7d  m/{url_parts[3]}
-0000f930: 2f7b 7572 6c5f 7061 7274 735b 345d 7d2f  /{url_parts[4]}/
-0000f940: 7261 772f 7b62 7261 6e63 687d 2f64 6573  raw/{branch}/des
-0000f950: 6372 6970 746f 722e 6a73 6f6e 220a 0a20  criptor.json".. 
-0000f960: 2020 2020 2020 2072 6574 7572 6e20 6f75         return ou
-0000f970: 7470 7574 5f75 726c 0a0a 2020 2020 6465  tput_url..    de
-0000f980: 6620 7075 6c6c 5f64 6573 6372 6970 746f  f pull_descripto
-0000f990: 725f 6672 6f6d 5f67 6974 6875 6228 7365  r_from_github(se
-0000f9a0: 6c66 2c20 776f 726b 666c 6f77 3a20 7374  lf, workflow: st
-0000f9b0: 7229 202d 3e20 4469 6374 3a0a 2020 2020  r) -> Dict:.    
-0000f9c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000f9d0: 5075 6c6c 2074 6865 2077 6f72 6b66 6c6f  Pull the workflo
-0000f9e0: 7720 6465 7363 7269 7074 6f72 2066 726f  w descriptor fro
-0000f9f0: 6d20 4769 7448 7562 2e0a 0a20 2020 2020  m GitHub...     
-0000fa00: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-0000fa10: 2020 2020 2077 6f72 6b66 6c6f 7720 2873       workflow (s
-0000fa20: 7472 293a 2054 6865 2077 6f72 6b66 6c6f  tr): The workflo
-0000fa30: 7720 666f 7220 7768 6963 6820 746f 2070  w for which to p
-0000fa40: 756c 6c20 7468 6520 6465 7363 7269 7074  ull the descript
-0000fa50: 6f72 2e0a 0a20 2020 2020 2020 2052 6574  or...        Ret
-0000fa60: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-0000fa70: 2020 4469 6374 3a20 5468 6520 4a53 4f4e    Dict: The JSON
-0000fa80: 2064 6573 6372 6970 746f 722e 0a0a 2020   descriptor...  
-0000fa90: 2020 2020 2020 5261 6973 6573 3a0a 2020        Raises:.  
-0000faa0: 2020 2020 2020 2020 2020 5661 6c75 6545            ValueE
-0000fab0: 7272 6f72 3a20 4966 2061 6e20 6572 726f  rror: If an erro
-0000fac0: 7220 6f63 6375 7273 2077 6869 6c65 2070  r occurs while p
-0000fad0: 756c 6c69 6e67 2074 6865 2064 6573 6372  ulling the descr
-0000fae0: 6970 746f 7220 6669 6c65 2e0a 2020 2020  iptor file..    
-0000faf0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-0000fb00: 6769 745f 7265 706f 203d 2073 656c 662e  git_repo = self.
-0000fb10: 736c 7572 6d5f 6d6f 6465 6c5f 7265 706f  slurm_model_repo
-0000fb20: 735b 776f 726b 666c 6f77 5d0a 2020 2020  s[workflow].    
-0000fb30: 2020 2020 2320 636f 6e76 6572 7420 6769      # convert gi
-0000fb40: 7420 7265 706f 2074 6f20 6a73 6f6e 2066  t repo to json f
-0000fb50: 696c 650a 2020 2020 2020 2020 7261 775f  ile.        raw_
-0000fb60: 7572 6c20 3d20 7365 6c66 2e63 6f6e 7665  url = self.conve
-0000fb70: 7274 5f75 726c 2867 6974 5f72 6570 6f29  rt_url(git_repo)
-0000fb80: 0a20 2020 2020 2020 206c 6f67 6765 722e  .        logger.
-0000fb90: 6465 6275 6728 6622 5075 6c6c 2077 6f72  debug(f"Pull wor
-0000fba0: 6b66 6c6f 773a 207b 776f 726b 666c 6f77  kflow: {workflow
-0000fbb0: 7d3a 207b 6769 745f 7265 706f 7d20 3e3e  }: {git_repo} >>
-0000fbc0: 207b 7261 775f 7572 6c7d 2229 0a20 2020   {raw_url}").   
-0000fbd0: 2020 2020 2023 2070 756c 6c20 776f 726b       # pull work
-0000fbe0: 666c 6f77 2070 6172 616d 730a 2020 2020  flow params.    
-0000fbf0: 2020 2020 6769 7468 7562 5f73 6573 7369      github_sessi
-0000fc00: 6f6e 203d 2073 656c 662e 6765 745f 6f72  on = self.get_or
-0000fc10: 5f63 7265 6174 655f 6769 7468 7562 5f73  _create_github_s
-0000fc20: 6573 7369 6f6e 2829 0a20 2020 2020 2020  ession().       
-0000fc30: 2067 6866 696c 6520 3d20 6769 7468 7562   ghfile = github
-0000fc40: 5f73 6573 7369 6f6e 2e67 6574 2872 6177  _session.get(raw
-0000fc50: 5f75 726c 290a 2020 2020 2020 2020 6966  _url).        if
-0000fc60: 2067 6866 696c 652e 6f6b 3a0a 2020 2020   ghfile.ok:.    
-0000fc70: 2020 2020 2020 2020 6c6f 6767 6572 2e64          logger.d
-0000fc80: 6562 7567 2866 2243 6163 6865 643f 207b  ebug(f"Cached? {
-0000fc90: 6768 6669 6c65 2e66 726f 6d5f 6361 6368  ghfile.from_cach
-0000fca0: 657d 2229 0a20 2020 2020 2020 2020 2020  e}").           
-0000fcb0: 206a 736f 6e5f 6465 7363 7269 7074 6f72   json_descriptor
-0000fcc0: 203d 2067 6866 696c 652e 6a73 6f6e 2829   = ghfile.json()
-0000fcd0: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
-0000fce0: 2020 2020 2020 2020 2020 2072 6169 7365             raise
-0000fcf0: 2056 616c 7565 4572 726f 7228 0a20 2020   ValueError(.   
-0000fd00: 2020 2020 2020 2020 2020 2020 2066 2745               f'E
-0000fd10: 7272 6f72 2077 6869 6c65 2070 756c 6c69  rror while pulli
-0000fd20: 6e67 2064 6573 6372 6970 746f 7220 6669  ng descriptor fi
-0000fd30: 6c65 2066 6f72 2077 6f72 6b66 6c6f 7720  le for workflow 
-0000fd40: 7b77 6f72 6b66 6c6f 777d 2c5c 0a20 2020  {workflow},\.   
-0000fd50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fd60: 2066 726f 6d20 7b72 6177 5f75 726c 7d3a   from {raw_url}:
-0000fd70: 207b 6768 6669 6c65 2e5f 5f64 6963 745f   {ghfile.__dict_
-0000fd80: 5f7d 2729 0a20 2020 2020 2020 2072 6574  _}').        ret
-0000fd90: 7572 6e20 6a73 6f6e 5f64 6573 6372 6970  urn json_descrip
-0000fda0: 746f 720a 0a20 2020 2064 6566 2067 6574  tor..    def get
-0000fdb0: 5f6f 725f 6372 6561 7465 5f67 6974 6875  _or_create_githu
-0000fdc0: 625f 7365 7373 696f 6e28 7365 6c66 293a  b_session(self):
-0000fdd0: 0a20 2020 2020 2020 2023 204e 6f74 652c  .        # Note,
-0000fde0: 2075 7369 6e67 2072 6571 7565 7374 735f   using requests_
-0000fdf0: 6361 6368 6520 312e 312e 312c 2063 6f6e  cache 1.1.1, con
-0000fe00: 6469 7469 6f6e 616c 2071 7565 7269 6573  ditional queries
-0000fe10: 2061 7265 2064 6566 6175 6c74 3a0a 2020   are default:.  
-0000fe20: 2020 2020 2020 2320 5468 6520 6361 6368        # The cach
-0000fe30: 6564 2072 6573 706f 6e73 6520 7769 6c6c  ed response will
-0000fe40: 2073 7469 6c6c 2062 6520 7573 6564 2075   still be used u
-0000fe50: 6e74 696c 2074 6865 2072 656d 6f74 6520  ntil the remote 
-0000fe60: 636f 6e74 656e 7420 6163 7475 616c 6c79  content actually
-0000fe70: 2063 6861 6e67 6573 0a20 2020 2020 2020   changes.       
-0000fe80: 2023 2045 7665 6e20 6966 2074 6865 2027   # Even if the '
-0000fe90: 6578 7069 7265 5f61 6674 6572 2720 6973  expire_after' is
-0000fea0: 2074 7269 6767 6572 6564 2e20 5468 6973   triggered. This
-0000feb0: 2069 7320 6275 696c 7420 696e 746f 2047   is built into G
-0000fec0: 6974 4875 622c 2077 6869 6368 2072 6574  itHub, which ret
-0000fed0: 7572 6e73 0a20 2020 2020 2020 2023 2061  urns.        # a
-0000fee0: 2045 7461 6720 696e 2074 6865 2068 6561   Etag in the hea
-0000fef0: 6465 7220 7468 6174 206f 6e6c 7920 6368  der that only ch
-0000ff00: 616e 6765 7320 7768 656e 2074 6865 2063  anges when the c
-0000ff10: 6f6e 7465 6e74 2028 652e 672e 2074 6865  ontent (e.g. the
-0000ff20: 2064 6573 6372 6970 746f 7229 2063 6861   descriptor) cha
-0000ff30: 6e67 6573 2e0a 2020 2020 2020 2020 2320  nges..        # 
-0000ff40: 4966 2079 6f75 2070 726f 7669 6465 2074  If you provide t
-0000ff50: 6869 7320 4574 6167 2077 6865 6e20 7175  his Etag when qu
-0000ff60: 6572 7969 6e67 2c20 796f 7520 7769 6c6c  erying, you will
-0000ff70: 2067 6574 2061 2033 3034 2028 276e 6f20   get a 304 ('no 
-0000ff80: 6368 616e 6765 2729 2061 6e64 2069 7420  change') and it 
-0000ff90: 7769 6c6c 0a20 2020 2020 2020 2023 204e  will.        # N
-0000ffa0: 4f54 2063 6f75 6e74 2074 6f77 6172 6473  OT count towards
-0000ffb0: 2079 6f75 7220 4769 7468 7562 206c 696d   your Github lim
-0000ffc0: 6974 732e 2041 6e64 2072 6571 7565 7374  its. And request
-0000ffd0: 735f 6361 6368 6520 646f 6573 2074 6861  s_cache does tha
-0000ffe0: 7420 666f 7220 7573 206e 6f77 2e0a 2020  t for us now..  
-0000fff0: 2020 2020 2020 2320 4e6f 7420 6176 6169        # Not avai
-00010000: 6c61 626c 6520 696e 2050 7974 686f 6e33  lable in Python3
-00010010: 2e36 2074 686f 7567 682e 0a20 2020 2020  .6 though..     
-00010020: 2020 2073 203d 2072 6571 7565 7374 735f     s = requests_
-00010030: 6361 6368 652e 4361 6368 6564 5365 7373  cache.CachedSess
-00010040: 696f 6e28 2767 6974 6875 625f 6361 6368  ion('github_cach
-00010050: 6527 2c0a 2020 2020 2020 2020 2020 2020  e',.            
+0000f2c0: 2020 2020 2020 2020 202a 6172 6773 2c20           *args, 
+0000f2d0: 2a2a 6b77 6172 6773 290a 0a20 2020 2064  **kwargs)..    d
+0000f2e0: 6566 2065 7874 7261 6374 5f70 6172 7473  ef extract_parts
+0000f2f0: 5f66 726f 6d5f 7572 6c28 7365 6c66 2c20  _from_url(self, 
+0000f300: 696e 7075 745f 7572 6c3a 2073 7472 2920  input_url: str) 
+0000f310: 2d3e 2054 7570 6c65 5b4c 6973 745b 7374  -> Tuple[List[st
+0000f320: 725d 2c20 7374 725d 3a0a 2020 2020 2020  r], str]:.      
+0000f330: 2020 2222 220a 2020 2020 2020 2020 4578    """.        Ex
+0000f340: 7472 6163 7420 7468 6520 7265 706f 7369  tract the reposi
+0000f350: 746f 7279 2061 6e64 2062 7261 6e63 6820  tory and branch 
+0000f360: 696e 666f 726d 6174 696f 6e20 6672 6f6d  information from
+0000f370: 2074 6865 2069 6e70 7574 2055 524c 2e0a   the input URL..
+0000f380: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
+0000f390: 2020 2020 2020 2020 2020 2069 6e70 7574             input
+0000f3a0: 5f75 726c 2028 7374 7229 3a20 5468 6520  _url (str): The 
+0000f3b0: 696e 7075 7420 4769 7448 7562 2055 524c  input GitHub URL
+0000f3c0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0000f3d0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0000f3e0: 5475 706c 655b 4c69 7374 5b73 7472 5d2c  Tuple[List[str],
+0000f3f0: 2073 7472 5d3a 0a20 2020 2020 2020 2020   str]:.         
+0000f400: 2020 2020 2020 2054 6865 206c 6973 7420         The list 
+0000f410: 6f66 2075 726c 2070 6172 7473 2061 6e64  of url parts and
+0000f420: 2074 6865 2062 7261 6e63 682f 7665 7273   the branch/vers
+0000f430: 696f 6e2e 0a20 2020 2020 2020 2020 2020  ion..           
+0000f440: 2020 2020 2049 6620 6e6f 2062 7261 6e63       If no branc
+0000f450: 6820 6973 2066 6f75 6e64 2c20 6974 2077  h is found, it w
+0000f460: 696c 6c20 7265 7475 726e 2022 6d61 7374  ill return "mast
+0000f470: 6572 220a 0a20 2020 2020 2020 2052 6169  er"..        Rai
+0000f480: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
+0000f490: 2056 616c 7565 4572 726f 723a 2049 6620   ValueError: If 
+0000f4a0: 7468 6520 696e 7075 7420 5552 4c20 6973  the input URL is
+0000f4b0: 206e 6f74 2061 2076 616c 6964 2047 6974   not a valid Git
+0000f4c0: 4875 6220 5552 4c2e 0a20 2020 2020 2020  Hub URL..       
+0000f4d0: 2022 2222 0a20 2020 2020 2020 2075 726c   """.        url
+0000f4e0: 5f70 6172 7473 203d 2069 6e70 7574 5f75  _parts = input_u
+0000f4f0: 726c 2e73 706c 6974 2822 2f22 290a 2020  rl.split("/").  
+0000f500: 2020 2020 2020 6966 206c 656e 2875 726c        if len(url
+0000f510: 5f70 6172 7473 2920 3c20 3520 6f72 2075  _parts) < 5 or u
+0000f520: 726c 5f70 6172 7473 5b32 5d20 213d 2022  rl_parts[2] != "
+0000f530: 6769 7468 7562 2e63 6f6d 223a 0a20 2020  github.com":.   
+0000f540: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+0000f550: 616c 7565 4572 726f 7228 2249 6e76 616c  alueError("Inval
+0000f560: 6964 2047 6974 4875 6220 5552 4c22 290a  id GitHub URL").
+0000f570: 0a20 2020 2020 2020 2069 6620 2274 7265  .        if "tre
+0000f580: 6522 2069 6e20 7572 6c5f 7061 7274 733a  e" in url_parts:
+0000f590: 0a20 2020 2020 2020 2020 2020 2023 2043  .            # C
+0000f5a0: 6173 653a 2055 524c 2063 6f6e 7461 696e  ase: URL contain
+0000f5b0: 7320 6120 6272 616e 6368 0a20 2020 2020  s a branch.     
+0000f5c0: 2020 2020 2020 2062 7261 6e63 685f 696e         branch_in
+0000f5d0: 6465 7820 3d20 7572 6c5f 7061 7274 732e  dex = url_parts.
+0000f5e0: 696e 6465 7828 2274 7265 6522 2920 2b20  index("tree") + 
+0000f5f0: 310a 2020 2020 2020 2020 2020 2020 6272  1.            br
+0000f600: 616e 6368 203d 2075 726c 5f70 6172 7473  anch = url_parts
+0000f610: 5b62 7261 6e63 685f 696e 6465 785d 0a20  [branch_index]. 
+0000f620: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000f630: 2020 2020 2020 2020 2023 2043 6173 653a           # Case:
+0000f640: 2055 524c 2064 6f65 7320 6e6f 7420 7370   URL does not sp
+0000f650: 6563 6966 7920 6120 6272 616e 6368 0a20  ecify a branch. 
+0000f660: 2020 2020 2020 2020 2020 2062 7261 6e63             branc
+0000f670: 6820 3d20 226d 6173 7465 7222 0a0a 2020  h = "master"..  
+0000f680: 2020 2020 2020 7265 7475 726e 2075 726c        return url
+0000f690: 5f70 6172 7473 2c20 6272 616e 6368 0a0a  _parts, branch..
+0000f6a0: 2020 2020 6465 6620 636f 6e76 6572 745f      def convert_
+0000f6b0: 7572 6c28 7365 6c66 2c20 696e 7075 745f  url(self, input_
+0000f6c0: 7572 6c3a 2073 7472 2920 2d3e 2073 7472  url: str) -> str
+0000f6d0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+0000f6e0: 2020 2020 2020 436f 6e76 6572 7420 7468        Convert th
+0000f6f0: 6520 696e 7075 7420 4769 7448 7562 2055  e input GitHub U
+0000f700: 524c 2074 6f20 616e 206f 7574 7075 7420  RL to an output 
+0000f710: 5552 4c20 7468 6174 2072 6574 7269 6576  URL that retriev
+0000f720: 6573 0a20 2020 2020 2020 2074 6865 2027  es.        the '
+0000f730: 6465 7363 7269 7074 6f72 2e6a 736f 6e27  descriptor.json'
+0000f740: 2066 696c 6520 696e 2072 6177 2066 6f72   file in raw for
+0000f750: 6d61 742e 0a0a 2020 2020 2020 2020 4172  mat...        Ar
+0000f760: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+0000f770: 696e 7075 745f 7572 6c20 2873 7472 293a  input_url (str):
+0000f780: 2054 6865 2069 6e70 7574 2047 6974 4875   The input GitHu
+0000f790: 6220 5552 4c2e 0a0a 2020 2020 2020 2020  b URL...        
+0000f7a0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+0000f7b0: 2020 2020 2073 7472 3a20 5468 6520 6f75       str: The ou
+0000f7c0: 7470 7574 2055 524c 2074 6f20 7468 6520  tput URL to the 
+0000f7d0: 2764 6573 6372 6970 746f 722e 6a73 6f6e  'descriptor.json
+0000f7e0: 2720 6669 6c65 2e0a 0a20 2020 2020 2020  ' file...       
+0000f7f0: 2052 6169 7365 733a 0a20 2020 2020 2020   Raises:.       
+0000f800: 2020 2020 2056 616c 7565 4572 726f 723a       ValueError:
+0000f810: 2049 6620 7468 6520 696e 7075 7420 5552   If the input UR
+0000f820: 4c20 6973 206e 6f74 2061 2076 616c 6964  L is not a valid
+0000f830: 2047 6974 4875 6220 5552 4c2e 0a20 2020   GitHub URL..   
+0000f840: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000f850: 2075 726c 5f70 6172 7473 2c20 6272 616e   url_parts, bran
+0000f860: 6368 203d 2073 656c 662e 6578 7472 6163  ch = self.extrac
+0000f870: 745f 7061 7274 735f 6672 6f6d 5f75 726c  t_parts_from_url
+0000f880: 2869 6e70 7574 5f75 726c 290a 0a20 2020  (input_url)..   
+0000f890: 2020 2020 2023 2043 6f6e 7374 7275 6374       # Construct
+0000f8a0: 2074 6865 206f 7574 7075 7420 5552 4c20   the output URL 
+0000f8b0: 6279 2063 6f6d 6269 6e69 6e67 2074 6865  by combining the
+0000f8c0: 2065 7874 7261 6374 6564 2069 6e66 6f72   extracted infor
+0000f8d0: 6d61 7469 6f6e 0a20 2020 2020 2020 2023  mation.        #
+0000f8e0: 2077 6974 6820 7468 6520 6465 7369 7265   with the desire
+0000f8f0: 6420 6669 6c65 2070 6174 680a 2020 2020  d file path.    
+0000f900: 2020 2020 6f75 7470 7574 5f75 726c 203d      output_url =
+0000f910: 2066 2268 7474 7073 3a2f 2f67 6974 6875   f"https://githu
+0000f920: 622e 636f 6d2f 7b75 726c 5f70 6172 7473  b.com/{url_parts
+0000f930: 5b33 5d7d 2f7b 7572 6c5f 7061 7274 735b  [3]}/{url_parts[
+0000f940: 345d 7d2f 7261 772f 7b62 7261 6e63 687d  4]}/raw/{branch}
+0000f950: 2f64 6573 6372 6970 746f 722e 6a73 6f6e  /descriptor.json
+0000f960: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
+0000f970: 6e20 6f75 7470 7574 5f75 726c 0a0a 2020  n output_url..  
+0000f980: 2020 6465 6620 7075 6c6c 5f64 6573 6372    def pull_descr
+0000f990: 6970 746f 725f 6672 6f6d 5f67 6974 6875  iptor_from_githu
+0000f9a0: 6228 7365 6c66 2c20 776f 726b 666c 6f77  b(self, workflow
+0000f9b0: 3a20 7374 7229 202d 3e20 4469 6374 3a0a  : str) -> Dict:.
+0000f9c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000f9d0: 2020 2020 5075 6c6c 2074 6865 2077 6f72      Pull the wor
+0000f9e0: 6b66 6c6f 7720 6465 7363 7269 7074 6f72  kflow descriptor
+0000f9f0: 2066 726f 6d20 4769 7448 7562 2e0a 0a20   from GitHub... 
+0000fa00: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+0000fa10: 2020 2020 2020 2020 2077 6f72 6b66 6c6f           workflo
+0000fa20: 7720 2873 7472 293a 2054 6865 2077 6f72  w (str): The wor
+0000fa30: 6b66 6c6f 7720 666f 7220 7768 6963 6820  kflow for which 
+0000fa40: 746f 2070 756c 6c20 7468 6520 6465 7363  to pull the desc
+0000fa50: 7269 7074 6f72 2e0a 0a20 2020 2020 2020  riptor...       
+0000fa60: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+0000fa70: 2020 2020 2020 4469 6374 3a20 5468 6520        Dict: The 
+0000fa80: 4a53 4f4e 2064 6573 6372 6970 746f 722e  JSON descriptor.
+0000fa90: 0a0a 2020 2020 2020 2020 5261 6973 6573  ..        Raises
+0000faa0: 3a0a 2020 2020 2020 2020 2020 2020 5661  :.            Va
+0000fab0: 6c75 6545 7272 6f72 3a20 4966 2061 6e20  lueError: If an 
+0000fac0: 6572 726f 7220 6f63 6375 7273 2077 6869  error occurs whi
+0000fad0: 6c65 2070 756c 6c69 6e67 2074 6865 2064  le pulling the d
+0000fae0: 6573 6372 6970 746f 7220 6669 6c65 2e0a  escriptor file..
+0000faf0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000fb00: 2020 2020 6769 745f 7265 706f 203d 2073      git_repo = s
+0000fb10: 656c 662e 736c 7572 6d5f 6d6f 6465 6c5f  elf.slurm_model_
+0000fb20: 7265 706f 735b 776f 726b 666c 6f77 5d0a  repos[workflow].
+0000fb30: 2020 2020 2020 2020 2320 636f 6e76 6572          # conver
+0000fb40: 7420 6769 7420 7265 706f 2074 6f20 6a73  t git repo to js
+0000fb50: 6f6e 2066 696c 650a 2020 2020 2020 2020  on file.        
+0000fb60: 7261 775f 7572 6c20 3d20 7365 6c66 2e63  raw_url = self.c
+0000fb70: 6f6e 7665 7274 5f75 726c 2867 6974 5f72  onvert_url(git_r
+0000fb80: 6570 6f29 0a20 2020 2020 2020 206c 6f67  epo).        log
+0000fb90: 6765 722e 6465 6275 6728 6622 5075 6c6c  ger.debug(f"Pull
+0000fba0: 2077 6f72 6b66 6c6f 773a 207b 776f 726b   workflow: {work
+0000fbb0: 666c 6f77 7d3a 207b 6769 745f 7265 706f  flow}: {git_repo
+0000fbc0: 7d20 3e3e 207b 7261 775f 7572 6c7d 2229  } >> {raw_url}")
+0000fbd0: 0a20 2020 2020 2020 2023 2070 756c 6c20  .        # pull 
+0000fbe0: 776f 726b 666c 6f77 2070 6172 616d 730a  workflow params.
+0000fbf0: 2020 2020 2020 2020 6769 7468 7562 5f73          github_s
+0000fc00: 6573 7369 6f6e 203d 2073 656c 662e 6765  ession = self.ge
+0000fc10: 745f 6f72 5f63 7265 6174 655f 6769 7468  t_or_create_gith
+0000fc20: 7562 5f73 6573 7369 6f6e 2829 0a20 2020  ub_session().   
+0000fc30: 2020 2020 2067 6866 696c 6520 3d20 6769       ghfile = gi
+0000fc40: 7468 7562 5f73 6573 7369 6f6e 2e67 6574  thub_session.get
+0000fc50: 2872 6177 5f75 726c 290a 2020 2020 2020  (raw_url).      
+0000fc60: 2020 6966 2067 6866 696c 652e 6f6b 3a0a    if ghfile.ok:.
+0000fc70: 2020 2020 2020 2020 2020 2020 6c6f 6767              logg
+0000fc80: 6572 2e64 6562 7567 2866 2243 6163 6865  er.debug(f"Cache
+0000fc90: 643f 207b 6768 6669 6c65 2e66 726f 6d5f  d? {ghfile.from_
+0000fca0: 6361 6368 657d 2229 0a20 2020 2020 2020  cache}").       
+0000fcb0: 2020 2020 206a 736f 6e5f 6465 7363 7269       json_descri
+0000fcc0: 7074 6f72 203d 2067 6866 696c 652e 6a73  ptor = ghfile.js
+0000fcd0: 6f6e 2829 0a20 2020 2020 2020 2065 6c73  on().        els
+0000fce0: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+0000fcf0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+0000fd00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fd10: 2066 2745 7272 6f72 2077 6869 6c65 2070   f'Error while p
+0000fd20: 756c 6c69 6e67 2064 6573 6372 6970 746f  ulling descripto
+0000fd30: 7220 6669 6c65 2066 6f72 2077 6f72 6b66  r file for workf
+0000fd40: 6c6f 7720 7b77 6f72 6b66 6c6f 777d 2c5c  low {workflow},\
+0000fd50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000fd60: 2020 2020 2066 726f 6d20 7b72 6177 5f75       from {raw_u
+0000fd70: 726c 7d3a 207b 6768 6669 6c65 2e5f 5f64  rl}: {ghfile.__d
+0000fd80: 6963 745f 5f7d 2729 0a20 2020 2020 2020  ict__}').       
+0000fd90: 2072 6574 7572 6e20 6a73 6f6e 5f64 6573   return json_des
+0000fda0: 6372 6970 746f 720a 0a20 2020 2064 6566  criptor..    def
+0000fdb0: 2067 6574 5f6f 725f 6372 6561 7465 5f67   get_or_create_g
+0000fdc0: 6974 6875 625f 7365 7373 696f 6e28 7365  ithub_session(se
+0000fdd0: 6c66 293a 0a20 2020 2020 2020 2023 204e  lf):.        # N
+0000fde0: 6f74 652c 2075 7369 6e67 2072 6571 7565  ote, using reque
+0000fdf0: 7374 735f 6361 6368 6520 312e 312e 312c  sts_cache 1.1.1,
+0000fe00: 2063 6f6e 6469 7469 6f6e 616c 2071 7565   conditional que
+0000fe10: 7269 6573 2061 7265 2064 6566 6175 6c74  ries are default
+0000fe20: 3a0a 2020 2020 2020 2020 2320 5468 6520  :.        # The 
+0000fe30: 6361 6368 6564 2072 6573 706f 6e73 6520  cached response 
+0000fe40: 7769 6c6c 2073 7469 6c6c 2062 6520 7573  will still be us
+0000fe50: 6564 2075 6e74 696c 2074 6865 2072 656d  ed until the rem
+0000fe60: 6f74 6520 636f 6e74 656e 7420 6163 7475  ote content actu
+0000fe70: 616c 6c79 2063 6861 6e67 6573 0a20 2020  ally changes.   
+0000fe80: 2020 2020 2023 2045 7665 6e20 6966 2074       # Even if t
+0000fe90: 6865 2027 6578 7069 7265 5f61 6674 6572  he 'expire_after
+0000fea0: 2720 6973 2074 7269 6767 6572 6564 2e20  ' is triggered. 
+0000feb0: 5468 6973 2069 7320 6275 696c 7420 696e  This is built in
+0000fec0: 746f 2047 6974 4875 622c 2077 6869 6368  to GitHub, which
+0000fed0: 2072 6574 7572 6e73 0a20 2020 2020 2020   returns.       
+0000fee0: 2023 2061 2045 7461 6720 696e 2074 6865   # a Etag in the
+0000fef0: 2068 6561 6465 7220 7468 6174 206f 6e6c   header that onl
+0000ff00: 7920 6368 616e 6765 7320 7768 656e 2074  y changes when t
+0000ff10: 6865 2063 6f6e 7465 6e74 2028 652e 672e  he content (e.g.
+0000ff20: 2074 6865 2064 6573 6372 6970 746f 7229   the descriptor)
+0000ff30: 2063 6861 6e67 6573 2e0a 2020 2020 2020   changes..      
+0000ff40: 2020 2320 4966 2079 6f75 2070 726f 7669    # If you provi
+0000ff50: 6465 2074 6869 7320 4574 6167 2077 6865  de this Etag whe
+0000ff60: 6e20 7175 6572 7969 6e67 2c20 796f 7520  n querying, you 
+0000ff70: 7769 6c6c 2067 6574 2061 2033 3034 2028  will get a 304 (
+0000ff80: 276e 6f20 6368 616e 6765 2729 2061 6e64  'no change') and
+0000ff90: 2069 7420 7769 6c6c 0a20 2020 2020 2020   it will.       
+0000ffa0: 2023 204e 4f54 2063 6f75 6e74 2074 6f77   # NOT count tow
+0000ffb0: 6172 6473 2079 6f75 7220 4769 7468 7562  ards your Github
+0000ffc0: 206c 696d 6974 732e 2041 6e64 2072 6571   limits. And req
+0000ffd0: 7565 7374 735f 6361 6368 6520 646f 6573  uests_cache does
+0000ffe0: 2074 6861 7420 666f 7220 7573 206e 6f77   that for us now
+0000fff0: 2e0a 2020 2020 2020 2020 2320 4e6f 7420  ..        # Not 
+00010000: 6176 6169 6c61 626c 6520 696e 2050 7974  available in Pyt
+00010010: 686f 6e33 2e36 2074 686f 7567 682e 0a20  hon3.6 though.. 
+00010020: 2020 2020 2020 2073 203d 2072 6571 7565         s = reque
+00010030: 7374 735f 6361 6368 652e 4361 6368 6564  sts_cache.Cached
+00010040: 5365 7373 696f 6e28 2767 6974 6875 625f  Session('github_
+00010050: 6361 6368 6527 2c0a 2020 2020 2020 2020  cache',.        
 00010060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010070: 2020 2020 2020 2020 2020 2020 2062 6163               bac
-00010080: 6b65 6e64 3d73 656c 662e 6361 6368 652c  kend=self.cache,
-00010090: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010080: 2062 6163 6b65 6e64 3d73 656c 662e 6361   backend=self.ca
+00010090: 6368 652c 0a20 2020 2020 2020 2020 2020  che,.           
 000100a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100b0: 2020 2020 2020 2020 2020 6578 7069 7265            expire
-000100c0: 5f61 6674 6572 3d31 2c0a 2020 2020 2020  _after=1,.      
+000100b0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+000100c0: 7069 7265 5f61 6674 6572 3d31 2c0a 2020  pire_after=1,.  
 000100d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000100e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000100f0: 2020 2063 6163 6865 5f63 6f6e 7472 6f6c     cache_control
-00010100: 3d54 7275 650a 2020 2020 2020 2020 2020  =True.          
+000100f0: 2020 2020 2020 2063 6163 6865 5f63 6f6e         cache_con
+00010100: 7472 6f6c 3d54 7275 650a 2020 2020 2020  trol=True.      
 00010110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010120: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00010130: 0a20 2020 2020 2020 2023 204d 6967 6874  .        # Might
-00010140: 2068 6176 6520 6269 6767 6572 2069 7373   have bigger iss
-00010150: 7565 732c 2074 6869 7320 6973 2072 656c  ues, this is rel
-00010160: 6174 6564 2074 6f20 7261 7465 206c 696d  ated to rate lim
-00010170: 6974 7320 6f6e 2047 6974 4875 620a 2020  its on GitHub.  
-00010180: 2020 2020 2020 2320 6874 7470 733a 2f2f        # https://
-00010190: 646f 6373 2e67 6974 6875 622e 636f 6d2f  docs.github.com/
-000101a0: 656e 2f72 6573 742f 7573 696e 672d 7468  en/rest/using-th
-000101b0: 652d 7265 7374 2d61 7069 2f72 6174 652d  e-rest-api/rate-
-000101c0: 6c69 6d69 7473 2d66 6f72 2d74 6865 2d72  limits-for-the-r
-000101d0: 6573 742d 6170 690a 2020 2020 2020 2020  est-api.        
-000101e0: 2320 4966 2069 7420 7374 6179 7320 6120  # If it stays a 
-000101f0: 7072 6f62 6c65 6d2c 2077 6520 6861 7665  problem, we have
-00010200: 2074 6f20 6164 6420 616e 206f 7074 696f   to add an optio
-00010210: 6e20 746f 2061 6464 2061 2047 4820 6b65  n to add a GH ke
-00010220: 7920 746f 2074 6865 2063 6f6e 6669 670a  y to the config.
-00010230: 2020 2020 2020 2020 2320 452e 672e 2073          # E.g. s
-00010240: 6565 2068 7474 7073 3a2f 2f67 6974 6875  ee https://githu
-00010250: 622e 636f 6d2f 7265 7175 6573 7473 2d63  b.com/requests-c
-00010260: 6163 6865 2f72 6571 7565 7374 732d 6361  ache/requests-ca
-00010270: 6368 652f 626c 6f62 2f35 3331 3334 6566  che/blob/53134ef
-00010280: 3065 3939 6437 3133 6665 6436 3235 3135  0e99d713fed62515
-00010290: 6466 6237 6263 6661 6163 3566 3633 6639  dfb7bcfaac5f63f9
-000102a0: 642f 6578 616d 706c 6573 2f70 7967 6974  d/examples/pygit
-000102b0: 6875 622e 7079 0a20 2020 2020 2020 2023  hub.py.        #
-000102c0: 2048 6572 6520 796f 7520 636f 756c 6420   Here you could 
-000102d0: 6861 7665 2061 6e20 4143 4345 5353 5f54  have an ACCESS_T
-000102e0: 4f4b 454e 2e0a 2020 2020 2020 2020 2320  OKEN..        # 
-000102f0: 416e 2041 4343 4553 535f 544f 4b45 4e20  An ACCESS_TOKEN 
-00010300: 636f 756c 6420 696d 7072 6f76 6520 6170  could improve ap
-00010310: 6920 6c69 6d69 7473 2074 6f20 3530 3030  i limits to 5000
-00010320: 2f68 2028 6672 6f6d 2036 302f 6829 2e0a  /h (from 60/h)..
-00010330: 2020 2020 2020 2020 7265 7472 795f 7374          retry_st
-00010340: 7261 7465 6779 203d 2052 6574 7279 280a  rategy = Retry(.
-00010350: 2020 2020 2020 2020 2020 2020 746f 7461              tota
-00010360: 6c3d 352c 2020 2020 2020 2020 2020 2020  l=5,            
-00010370: 2020 2023 204d 6178 696d 756d 206e 756d     # Maximum num
-00010380: 6265 7220 6f66 2072 6574 7269 6573 0a20  ber of retries. 
-00010390: 2020 2020 2020 2020 2020 2023 2045 7870             # Exp
-000103a0: 6f6e 656e 7469 616c 2062 6163 6b6f 6666  onential backoff
-000103b0: 2066 6163 746f 7220 2864 656c 6179 2062   factor (delay b
-000103c0: 6574 7765 656e 2072 6574 7269 6573 290a  etween retries).
-000103d0: 2020 2020 2020 2020 2020 2020 6261 636b              back
-000103e0: 6f66 665f 6661 6374 6f72 3d35 2c0a 2020  off_factor=5,.  
-000103f0: 2020 2020 2020 2020 2020 2320 5265 7472            # Retr
-00010400: 7920 6f6e 2074 6865 7365 2048 5454 5020  y on these HTTP 
-00010410: 7374 6174 7573 2063 6f64 6573 0a20 2020  status codes.   
-00010420: 2020 2020 2020 2020 2073 7461 7475 735f           status_
-00010430: 666f 7263 656c 6973 743d 5b35 3030 2c20  forcelist=[500, 
-00010440: 3530 322c 2035 3033 2c20 3530 342c 2034  502, 503, 504, 4
-00010450: 3033 2c20 3432 395d 2c0a 2020 2020 2020  03, 429],.      
-00010460: 2020 2020 2020 616c 6c6f 7765 645f 6d65        allowed_me
-00010470: 7468 6f64 733d 6672 6f7a 656e 7365 7428  thods=frozenset(
-00010480: 5b27 4745 5427 5d29 2020 2320 4f6e 6c79  ['GET'])  # Only
-00010490: 2072 6574 7279 2066 6f72 2047 4554 2072   retry for GET r
-000104a0: 6571 7565 7374 730a 2020 2020 2020 2020  equests.        
-000104b0: 290a 2020 2020 2020 2020 732e 6d6f 756e  ).        s.moun
-000104c0: 7428 2768 7474 7073 3a2f 2f67 6974 6875  t('https://githu
-000104d0: 622e 636f 6d2f 272c 2048 5454 5041 6461  b.com/', HTTPAda
-000104e0: 7074 6572 286d 6178 5f72 6574 7269 6573  pter(max_retries
-000104f0: 3d72 6574 7279 5f73 7472 6174 6567 7929  =retry_strategy)
-00010500: 290a 2020 2020 2020 2020 732e 6d6f 756e  ).        s.moun
-00010510: 7428 2768 7474 703a 2f2f 6769 7468 7562  t('http://github
-00010520: 2e63 6f6d 2f27 2c20 4854 5450 4164 6170  .com/', HTTPAdap
-00010530: 7465 7228 6d61 785f 7265 7472 6965 733d  ter(max_retries=
-00010540: 7265 7472 795f 7374 7261 7465 6779 2929  retry_strategy))
-00010550: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00010560: 730a 0a20 2020 2064 6566 2067 6574 5f77  s..    def get_w
-00010570: 6f72 6b66 6c6f 775f 636f 6d6d 616e 6428  orkflow_command(
-00010580: 7365 6c66 2c0a 2020 2020 2020 2020 2020  self,.          
+00010120: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010130: 2020 2029 0a20 2020 2020 2020 2023 204d     ).        # M
+00010140: 6967 6874 2068 6176 6520 6269 6767 6572  ight have bigger
+00010150: 2069 7373 7565 732c 2074 6869 7320 6973   issues, this is
+00010160: 2072 656c 6174 6564 2074 6f20 7261 7465   related to rate
+00010170: 206c 696d 6974 7320 6f6e 2047 6974 4875   limits on GitHu
+00010180: 620a 2020 2020 2020 2020 2320 6874 7470  b.        # http
+00010190: 733a 2f2f 646f 6373 2e67 6974 6875 622e  s://docs.github.
+000101a0: 636f 6d2f 656e 2f72 6573 742f 7573 696e  com/en/rest/usin
+000101b0: 672d 7468 652d 7265 7374 2d61 7069 2f72  g-the-rest-api/r
+000101c0: 6174 652d 6c69 6d69 7473 2d66 6f72 2d74  ate-limits-for-t
+000101d0: 6865 2d72 6573 742d 6170 690a 2020 2020  he-rest-api.    
+000101e0: 2020 2020 2320 4966 2069 7420 7374 6179      # If it stay
+000101f0: 7320 6120 7072 6f62 6c65 6d2c 2077 6520  s a problem, we 
+00010200: 6861 7665 2074 6f20 6164 6420 616e 206f  have to add an o
+00010210: 7074 696f 6e20 746f 2061 6464 2061 2047  ption to add a G
+00010220: 4820 6b65 7920 746f 2074 6865 2063 6f6e  H key to the con
+00010230: 6669 670a 2020 2020 2020 2020 2320 452e  fig.        # E.
+00010240: 672e 2073 6565 2068 7474 7073 3a2f 2f67  g. see https://g
+00010250: 6974 6875 622e 636f 6d2f 7265 7175 6573  ithub.com/reques
+00010260: 7473 2d63 6163 6865 2f72 6571 7565 7374  ts-cache/request
+00010270: 732d 6361 6368 652f 626c 6f62 2f35 3331  s-cache/blob/531
+00010280: 3334 6566 3065 3939 6437 3133 6665 6436  34ef0e99d713fed6
+00010290: 3235 3135 6466 6237 6263 6661 6163 3566  2515dfb7bcfaac5f
+000102a0: 3633 6639 642f 6578 616d 706c 6573 2f70  63f9d/examples/p
+000102b0: 7967 6974 6875 622e 7079 0a20 2020 2020  ygithub.py.     
+000102c0: 2020 2023 2048 6572 6520 796f 7520 636f     # Here you co
+000102d0: 756c 6420 6861 7665 2061 6e20 4143 4345  uld have an ACCE
+000102e0: 5353 5f54 4f4b 454e 2e0a 2020 2020 2020  SS_TOKEN..      
+000102f0: 2020 2320 416e 2041 4343 4553 535f 544f    # An ACCESS_TO
+00010300: 4b45 4e20 636f 756c 6420 696d 7072 6f76  KEN could improv
+00010310: 6520 6170 6920 6c69 6d69 7473 2074 6f20  e api limits to 
+00010320: 3530 3030 2f68 2028 6672 6f6d 2036 302f  5000/h (from 60/
+00010330: 6829 2e0a 2020 2020 2020 2020 7265 7472  h)..        retr
+00010340: 795f 7374 7261 7465 6779 203d 2052 6574  y_strategy = Ret
+00010350: 7279 280a 2020 2020 2020 2020 2020 2020  ry(.            
+00010360: 746f 7461 6c3d 352c 2020 2020 2020 2020  total=5,        
+00010370: 2020 2020 2020 2023 204d 6178 696d 756d         # Maximum
+00010380: 206e 756d 6265 7220 6f66 2072 6574 7269   number of retri
+00010390: 6573 0a20 2020 2020 2020 2020 2020 2023  es.            #
+000103a0: 2045 7870 6f6e 656e 7469 616c 2062 6163   Exponential bac
+000103b0: 6b6f 6666 2066 6163 746f 7220 2864 656c  koff factor (del
+000103c0: 6179 2062 6574 7765 656e 2072 6574 7269  ay between retri
+000103d0: 6573 290a 2020 2020 2020 2020 2020 2020  es).            
+000103e0: 6261 636b 6f66 665f 6661 6374 6f72 3d35  backoff_factor=5
+000103f0: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
+00010400: 5265 7472 7920 6f6e 2074 6865 7365 2048  Retry on these H
+00010410: 5454 5020 7374 6174 7573 2063 6f64 6573  TTP status codes
+00010420: 0a20 2020 2020 2020 2020 2020 2073 7461  .            sta
+00010430: 7475 735f 666f 7263 656c 6973 743d 5b35  tus_forcelist=[5
+00010440: 3030 2c20 3530 322c 2035 3033 2c20 3530  00, 502, 503, 50
+00010450: 342c 2034 3033 2c20 3432 395d 2c0a 2020  4, 403, 429],.  
+00010460: 2020 2020 2020 2020 2020 616c 6c6f 7765            allowe
+00010470: 645f 6d65 7468 6f64 733d 6672 6f7a 656e  d_methods=frozen
+00010480: 7365 7428 5b27 4745 5427 5d29 2020 2320  set(['GET'])  # 
+00010490: 4f6e 6c79 2072 6574 7279 2066 6f72 2047  Only retry for G
+000104a0: 4554 2072 6571 7565 7374 730a 2020 2020  ET requests.    
+000104b0: 2020 2020 290a 2020 2020 2020 2020 732e      ).        s.
+000104c0: 6d6f 756e 7428 2768 7474 7073 3a2f 2f67  mount('https://g
+000104d0: 6974 6875 622e 636f 6d2f 272c 2048 5454  ithub.com/', HTT
+000104e0: 5041 6461 7074 6572 286d 6178 5f72 6574  PAdapter(max_ret
+000104f0: 7269 6573 3d72 6574 7279 5f73 7472 6174  ries=retry_strat
+00010500: 6567 7929 290a 2020 2020 2020 2020 732e  egy)).        s.
+00010510: 6d6f 756e 7428 2768 7474 703a 2f2f 6769  mount('http://gi
+00010520: 7468 7562 2e63 6f6d 2f27 2c20 4854 5450  thub.com/', HTTP
+00010530: 4164 6170 7465 7228 6d61 785f 7265 7472  Adapter(max_retr
+00010540: 6965 733d 7265 7472 795f 7374 7261 7465  ies=retry_strate
+00010550: 6779 2929 0a20 2020 2020 2020 2072 6574  gy)).        ret
+00010560: 7572 6e20 730a 0a20 2020 2064 6566 2067  urn s..    def g
+00010570: 6574 5f77 6f72 6b66 6c6f 775f 636f 6d6d  et_workflow_comm
+00010580: 616e 6428 7365 6c66 2c0a 2020 2020 2020  and(self,.      
 00010590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000105a0: 2020 2077 6f72 6b66 6c6f 773a 2073 7472     workflow: str
-000105b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-000105c0: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-000105d0: 6f72 6b66 6c6f 775f 7665 7273 696f 6e3a  orkflow_version:
-000105e0: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
+000105a0: 2020 2020 2020 2077 6f72 6b66 6c6f 773a         workflow:
+000105b0: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
+000105c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000105d0: 2020 2077 6f72 6b66 6c6f 775f 7665 7273     workflow_vers
+000105e0: 696f 6e3a 2073 7472 2c0a 2020 2020 2020  ion: str,.      
 000105f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010600: 2020 2069 6e70 7574 5f64 6174 613a 2073     input_data: s
-00010610: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
+00010600: 2020 2020 2020 2069 6e70 7574 5f64 6174         input_dat
+00010610: 613a 2073 7472 2c0a 2020 2020 2020 2020  a: str,.        
 00010620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010630: 2065 6d61 696c 3a20 4f70 7469 6f6e 616c   email: Optional
-00010640: 5b73 7472 5d20 3d20 4e6f 6e65 2c0a 2020  [str] = None,.  
-00010650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010660: 2020 2020 2020 2020 2020 2074 696d 653a             time:
-00010670: 204f 7074 696f 6e61 6c5b 7374 725d 203d   Optional[str] =
-00010680: 204e 6f6e 652c 0a20 2020 2020 2020 2020   None,.         
+00010630: 2020 2020 2065 6d61 696c 3a20 4f70 7469       email: Opti
+00010640: 6f6e 616c 5b73 7472 5d20 3d20 4e6f 6e65  onal[str] = None
+00010650: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010660: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00010670: 696d 653a 204f 7074 696f 6e61 6c5b 7374  ime: Optional[st
+00010680: 725d 203d 204e 6f6e 652c 0a20 2020 2020  r] = None,.     
 00010690: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000106a0: 2020 2020 2a2a 6b77 6172 6773 2920 2d3e      **kwargs) ->
-000106b0: 2054 7570 6c65 5b73 7472 2c20 4469 6374   Tuple[str, Dict
-000106c0: 5d3a 0a20 2020 2020 2020 2022 2222 0a20  ]:.        """. 
-000106d0: 2020 2020 2020 2047 656e 6572 6174 6520         Generate 
-000106e0: 7468 6520 536c 7572 6d20 776f 726b 666c  the Slurm workfl
-000106f0: 6f77 2063 6f6d 6d61 6e64 2061 6e64 2065  ow command and e
-00010700: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
-00010710: 626c 6573 2e0a 0a20 2020 2020 2020 2041  bles...        A
-00010720: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00010730: 2077 6f72 6b66 6c6f 7720 2873 7472 293a   workflow (str):
-00010740: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
-00010750: 2077 6f72 6b66 6c6f 772e 0a20 2020 2020   workflow..     
-00010760: 2020 2020 2020 2077 6f72 6b66 6c6f 775f         workflow_
-00010770: 7665 7273 696f 6e20 2873 7472 293a 2054  version (str): T
-00010780: 6865 2076 6572 7369 6f6e 206f 6620 7468  he version of th
-00010790: 6520 776f 726b 666c 6f77 2e0a 2020 2020  e workflow..    
-000107a0: 2020 2020 2020 2020 696e 7075 745f 6461          input_da
-000107b0: 7461 2028 7374 7229 3a20 5468 6520 6e61  ta (str): The na
-000107c0: 6d65 206f 6620 7468 6520 696e 7075 7420  me of the input 
-000107d0: 6461 7461 2066 6f6c 6465 7220 636f 6e74  data folder cont
-000107e0: 6169 6e69 6e67 0a20 2020 2020 2020 2020  aining.         
-000107f0: 2020 2020 2020 2074 6865 2069 6e70 7574         the input
-00010800: 2069 6d61 6765 2066 696c 6573 2e0a 2020   image files..  
-00010810: 2020 2020 2020 2020 2020 656d 6169 6c20            email 
-00010820: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
-00010830: 2054 6865 2065 6d61 696c 2061 6464 7265   The email addre
-00010840: 7373 2066 6f72 206a 6f62 206e 6f74 6966  ss for job notif
-00010850: 6963 6174 696f 6e73 2e0a 2020 2020 2020  ications..      
-00010860: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-00010870: 7473 2074 6f20 4e6f 6e65 2c20 7768 6963  ts to None, whic
-00010880: 6820 6465 6661 756c 7473 2074 6f20 7768  h defaults to wh
-00010890: 6174 2069 7320 696e 2074 6865 206a 6f62  at is in the job
-000108a0: 2073 6372 6970 742e 0a20 2020 2020 2020   script..       
-000108b0: 2020 2020 2074 696d 6520 2873 7472 2c20       time (str, 
-000108c0: 6f70 7469 6f6e 616c 293a 2054 6865 2074  optional): The t
-000108d0: 696d 6520 6c69 6d69 7420 666f 7220 7468  ime limit for th
-000108e0: 6520 6a6f 6220 696e 2074 6865 200a 2020  e job in the .  
-000108f0: 2020 2020 2020 2020 2020 2020 2020 666f                fo
-00010900: 726d 6174 2048 483a 4d4d 3a53 532e 2044  rmat HH:MM:SS. D
-00010910: 6566 6175 6c74 7320 746f 204e 6f6e 652c  efaults to None,
-00010920: 2077 6869 6368 2064 6566 6175 6c74 7320   which defaults 
-00010930: 746f 2077 6861 7420 0a20 2020 2020 2020  to what .       
-00010940: 2020 2020 2020 2020 2069 7320 696e 2074           is in t
-00010950: 6865 206a 6f62 2073 6372 6970 742e 0a20  he job script.. 
-00010960: 2020 2020 2020 2020 2020 202a 2a6b 7761             **kwa
-00010970: 7267 733a 2041 6464 6974 696f 6e61 6c20  rgs: Additional 
-00010980: 6b65 7977 6f72 6420 6172 6775 6d65 6e74  keyword argument
-00010990: 7320 666f 7220 7468 6520 776f 726b 666c  s for the workfl
-000109a0: 6f77 2e0a 0a20 2020 2020 2020 2052 6574  ow...        Ret
-000109b0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-000109c0: 2020 5475 706c 655b 7374 722c 2044 6963    Tuple[str, Dic
-000109d0: 745d 3a0a 2020 2020 2020 2020 2020 2020  t]:.            
-000109e0: 2020 2020 4120 7475 706c 6520 636f 6e74      A tuple cont
-000109f0: 6169 6e69 6e67 2074 6865 2053 6c75 726d  aining the Slurm
-00010a00: 2077 6f72 6b66 6c6f 7720 636f 6d6d 616e   workflow comman
-00010a10: 6420 616e 640a 2020 2020 2020 2020 2020  d and.          
-00010a20: 2020 2020 2020 7468 6520 656e 7669 726f        the enviro
-00010a30: 6e6d 656e 7420 7661 7269 6162 6c65 732e  nment variables.
-00010a40: 0a0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00010a50: 2020 2020 2020 6d6f 6465 6c5f 7061 7468        model_path
-00010a60: 203d 2073 656c 662e 736c 7572 6d5f 6d6f   = self.slurm_mo
-00010a70: 6465 6c5f 7061 7468 735b 776f 726b 666c  del_paths[workfl
-00010a80: 6f77 2e6c 6f77 6572 2829 5d0a 2020 2020  ow.lower()].    
-00010a90: 2020 2020 6a6f 625f 7363 7269 7074 203d      job_script =
-00010aa0: 2073 656c 662e 736c 7572 6d5f 6d6f 6465   self.slurm_mode
-00010ab0: 6c5f 6a6f 6273 5b77 6f72 6b66 6c6f 772e  l_jobs[workflow.
-00010ac0: 6c6f 7765 7228 295d 0a20 2020 2020 2020  lower()].       
-00010ad0: 206a 6f62 5f70 6172 616d 7320 3d20 7365   job_params = se
-00010ae0: 6c66 2e73 6c75 726d 5f6d 6f64 656c 5f6a  lf.slurm_model_j
-00010af0: 6f62 735f 7061 7261 6d73 5b77 6f72 6b66  obs_params[workf
-00010b00: 6c6f 772e 6c6f 7765 7228 295d 0a20 2020  low.lower()].   
-00010b10: 2020 2020 2023 2067 7261 6220 6f6e 6c79       # grab only
-00010b20: 2074 6865 2069 6d61 6765 206e 616d 652c   the image name,
-00010b30: 206e 6f74 2074 6865 2067 726f 7570 2f63   not the group/c
-00010b40: 7265 6174 6f72 0a20 2020 2020 2020 2069  reator.        i
-00010b50: 6d61 6765 203d 2073 656c 662e 736c 7572  mage = self.slur
-00010b60: 6d5f 6d6f 6465 6c5f 696d 6167 6573 5b77  m_model_images[w
-00010b70: 6f72 6b66 6c6f 772e 6c6f 7765 7228 295d  orkflow.lower()]
-00010b80: 2e73 706c 6974 2822 2f22 295b 315d 0a0a  .split("/")[1]..
-00010b90: 2020 2020 2020 2020 7362 6174 6368 5f65          sbatch_e
-00010ba0: 6e76 203d 207b 0a20 2020 2020 2020 2020  nv = {.         
-00010bb0: 2020 2022 4441 5441 5f50 4154 4822 3a20     "DATA_PATH": 
-00010bc0: 6622 5c22 7b73 656c 662e 736c 7572 6d5f  f"\"{self.slurm_
-00010bd0: 6461 7461 5f70 6174 687d 2f7b 696e 7075  data_path}/{inpu
-00010be0: 745f 6461 7461 7d5c 2222 2c0a 2020 2020  t_data}\"",.    
-00010bf0: 2020 2020 2020 2020 2249 4d41 4745 5f50          "IMAGE_P
-00010c00: 4154 4822 3a20 6622 5c22 7b73 656c 662e  ATH": f"\"{self.
-00010c10: 736c 7572 6d5f 696d 6167 6573 5f70 6174  slurm_images_pat
-00010c20: 687d 2f7b 6d6f 6465 6c5f 7061 7468 7d5c  h}/{model_path}\
-00010c30: 2222 2c0a 2020 2020 2020 2020 2020 2020  "",.            
-00010c40: 2249 4d41 4745 5f56 4552 5349 4f4e 223a  "IMAGE_VERSION":
-00010c50: 2066 227b 776f 726b 666c 6f77 5f76 6572   f"{workflow_ver
-00010c60: 7369 6f6e 7d22 2c0a 2020 2020 2020 2020  sion}",.        
-00010c70: 2020 2020 2253 494e 4755 4c41 5249 5459      "SINGULARITY
-00010c80: 5f49 4d41 4745 223a 2066 225c 227b 696d  _IMAGE": f"\"{im
-00010c90: 6167 657d 5f7b 776f 726b 666c 6f77 5f76  age}_{workflow_v
-00010ca0: 6572 7369 6f6e 7d2e 7369 665c 2222 2c0a  ersion}.sif\"",.
-00010cb0: 2020 2020 2020 2020 2020 2020 2253 4352              "SCR
-00010cc0: 4950 545f 5041 5448 223a 2066 225c 227b  IPT_PATH": f"\"{
-00010cd0: 7365 6c66 2e73 6c75 726d 5f73 6372 6970  self.slurm_scrip
-00010ce0: 745f 7061 7468 7d5c 2222 0a20 2020 2020  t_path}\"".     
-00010cf0: 2020 207d 0a20 2020 2020 2020 2077 6f72     }.        wor
-00010d00: 6b66 6c6f 775f 656e 7620 3d20 7365 6c66  kflow_env = self
-00010d10: 2e77 6f72 6b66 6c6f 775f 7061 7261 6d73  .workflow_params
-00010d20: 5f74 6f5f 656e 7676 6172 7328 2a2a 6b77  _to_envvars(**kw
-00010d30: 6172 6773 290a 2020 2020 2020 2020 656e  args).        en
-00010d40: 7620 3d20 7b2a 2a73 6261 7463 685f 656e  v = {**sbatch_en
-00010d50: 762c 202a 2a77 6f72 6b66 6c6f 775f 656e  v, **workflow_en
-00010d60: 767d 0a0a 2020 2020 2020 2020 656d 6169  v}..        emai
-00010d70: 6c5f 7061 7261 6d20 3d20 2222 2069 6620  l_param = "" if 
-00010d80: 656d 6169 6c20 6973 204e 6f6e 6520 656c  email is None el
-00010d90: 7365 2066 2220 2d2d 6d61 696c 2d75 7365  se f" --mail-use
-00010da0: 723d 7b65 6d61 696c 7d22 0a20 2020 2020  r={email}".     
-00010db0: 2020 2074 696d 655f 7061 7261 6d20 3d20     time_param = 
-00010dc0: 2222 2069 6620 7469 6d65 2069 7320 4e6f  "" if time is No
-00010dd0: 6e65 2065 6c73 6520 6622 202d 2d74 696d  ne else f" --tim
-00010de0: 653d 7b74 696d 657d 220a 2020 2020 2020  e={time}".      
-00010df0: 2020 6a6f 625f 7061 7261 6d73 2e61 7070    job_params.app
-00010e00: 656e 6428 7469 6d65 5f70 6172 616d 290a  end(time_param).
-00010e10: 2020 2020 2020 2020 6a6f 625f 7061 7261          job_para
-00010e20: 6d73 2e61 7070 656e 6428 656d 6169 6c5f  ms.append(email_
-00010e30: 7061 7261 6d29 0a20 2020 2020 2020 206a  param).        j
-00010e40: 6f62 5f70 6172 616d 203d 2022 222e 6a6f  ob_param = "".jo
-00010e50: 696e 286a 6f62 5f70 6172 616d 7329 0a20  in(job_params). 
-00010e60: 2020 2020 2020 2073 6261 7463 685f 636d         sbatch_cm
-00010e70: 6420 3d20 6622 7362 6174 6368 7b6a 6f62  d = f"sbatch{job
-00010e80: 5f70 6172 616d 7d20 2d2d 6f75 7470 7574  _param} --output
-00010e90: 3d6f 6d65 726f 2d25 6a2e 6c6f 6720 5c0a  =omero-%j.log \.
-00010ea0: 2020 2020 2020 2020 2020 2020 5c22 7b73              \"{s
-00010eb0: 656c 662e 736c 7572 6d5f 7363 7269 7074  elf.slurm_script
-00010ec0: 5f70 6174 687d 2f7b 6a6f 625f 7363 7269  _path}/{job_scri
-00010ed0: 7074 7d5c 2222 0a0a 2020 2020 2020 2020  pt}\""..        
-00010ee0: 7265 7475 726e 2073 6261 7463 685f 636d  return sbatch_cm
-00010ef0: 642c 2065 6e76 0a0a 2020 2020 6465 6620  d, env..    def 
-00010f00: 6765 745f 636f 6e76 6572 7369 6f6e 5f63  get_conversion_c
-00010f10: 6f6d 6d61 6e64 2873 656c 662c 2064 6174  ommand(self, dat
-00010f20: 615f 7061 7468 3a20 7374 722c 0a20 2020  a_path: str,.   
-00010f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f40: 2020 2020 2020 2020 2020 2020 636f 6e66              conf
-00010f50: 6967 5f66 696c 653a 2073 7472 2c0a 2020  ig_file: str,.  
-00010f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f70: 2020 2020 2020 2020 2020 2020 2073 6f75               sou
-00010f80: 7263 655f 666f 726d 6174 3a20 7374 7220  rce_format: str 
-00010f90: 3d20 277a 6172 7227 2c0a 2020 2020 2020  = 'zarr',.      
+000106a0: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
+000106b0: 2920 2d3e 2054 7570 6c65 5b73 7472 2c20  ) -> Tuple[str, 
+000106c0: 4469 6374 5d3a 0a20 2020 2020 2020 2022  Dict]:.        "
+000106d0: 2222 0a20 2020 2020 2020 2047 656e 6572  "".        Gener
+000106e0: 6174 6520 7468 6520 536c 7572 6d20 776f  ate the Slurm wo
+000106f0: 726b 666c 6f77 2063 6f6d 6d61 6e64 2061  rkflow command a
+00010700: 6e64 2065 6e76 6972 6f6e 6d65 6e74 2076  nd environment v
+00010710: 6172 6961 626c 6573 2e0a 0a20 2020 2020  ariables...     
+00010720: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00010730: 2020 2020 2077 6f72 6b66 6c6f 7720 2873       workflow (s
+00010740: 7472 293a 2054 6865 206e 616d 6520 6f66  tr): The name of
+00010750: 2074 6865 2077 6f72 6b66 6c6f 772e 0a20   the workflow.. 
+00010760: 2020 2020 2020 2020 2020 2077 6f72 6b66             workf
+00010770: 6c6f 775f 7665 7273 696f 6e20 2873 7472  low_version (str
+00010780: 293a 2054 6865 2076 6572 7369 6f6e 206f  ): The version o
+00010790: 6620 7468 6520 776f 726b 666c 6f77 2e0a  f the workflow..
+000107a0: 2020 2020 2020 2020 2020 2020 696e 7075              inpu
+000107b0: 745f 6461 7461 2028 7374 7229 3a20 5468  t_data (str): Th
+000107c0: 6520 6e61 6d65 206f 6620 7468 6520 696e  e name of the in
+000107d0: 7075 7420 6461 7461 2066 6f6c 6465 7220  put data folder 
+000107e0: 636f 6e74 6169 6e69 6e67 0a20 2020 2020  containing.     
+000107f0: 2020 2020 2020 2020 2020 2074 6865 2069             the i
+00010800: 6e70 7574 2069 6d61 6765 2066 696c 6573  nput image files
+00010810: 2e0a 2020 2020 2020 2020 2020 2020 656d  ..            em
+00010820: 6169 6c20 2873 7472 2c20 6f70 7469 6f6e  ail (str, option
+00010830: 616c 293a 2054 6865 2065 6d61 696c 2061  al): The email a
+00010840: 6464 7265 7373 2066 6f72 206a 6f62 206e  ddress for job n
+00010850: 6f74 6966 6963 6174 696f 6e73 2e0a 2020  otifications..  
+00010860: 2020 2020 2020 2020 2020 2020 2020 4465                De
+00010870: 6661 756c 7473 2074 6f20 4e6f 6e65 2c20  faults to None, 
+00010880: 7768 6963 6820 6465 6661 756c 7473 2074  which defaults t
+00010890: 6f20 7768 6174 2069 7320 696e 2074 6865  o what is in the
+000108a0: 206a 6f62 2073 6372 6970 742e 0a20 2020   job script..   
+000108b0: 2020 2020 2020 2020 2074 696d 6520 2873           time (s
+000108c0: 7472 2c20 6f70 7469 6f6e 616c 293a 2054  tr, optional): T
+000108d0: 6865 2074 696d 6520 6c69 6d69 7420 666f  he time limit fo
+000108e0: 7220 7468 6520 6a6f 6220 696e 2074 6865  r the job in the
+000108f0: 200a 2020 2020 2020 2020 2020 2020 2020   .              
+00010900: 2020 666f 726d 6174 2048 483a 4d4d 3a53    format HH:MM:S
+00010910: 532e 2044 6566 6175 6c74 7320 746f 204e  S. Defaults to N
+00010920: 6f6e 652c 2077 6869 6368 2064 6566 6175  one, which defau
+00010930: 6c74 7320 746f 2077 6861 7420 0a20 2020  lts to what .   
+00010940: 2020 2020 2020 2020 2020 2020 2069 7320               is 
+00010950: 696e 2074 6865 206a 6f62 2073 6372 6970  in the job scrip
+00010960: 742e 0a20 2020 2020 2020 2020 2020 202a  t..            *
+00010970: 2a6b 7761 7267 733a 2041 6464 6974 696f  *kwargs: Additio
+00010980: 6e61 6c20 6b65 7977 6f72 6420 6172 6775  nal keyword argu
+00010990: 6d65 6e74 7320 666f 7220 7468 6520 776f  ments for the wo
+000109a0: 726b 666c 6f77 2e0a 0a20 2020 2020 2020  rkflow...       
+000109b0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+000109c0: 2020 2020 2020 5475 706c 655b 7374 722c        Tuple[str,
+000109d0: 2044 6963 745d 3a0a 2020 2020 2020 2020   Dict]:.        
+000109e0: 2020 2020 2020 2020 4120 7475 706c 6520          A tuple 
+000109f0: 636f 6e74 6169 6e69 6e67 2074 6865 2053  containing the S
+00010a00: 6c75 726d 2077 6f72 6b66 6c6f 7720 636f  lurm workflow co
+00010a10: 6d6d 616e 6420 616e 640a 2020 2020 2020  mmand and.      
+00010a20: 2020 2020 2020 2020 2020 7468 6520 656e            the en
+00010a30: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
+00010a40: 6c65 732e 0a0a 2020 2020 2020 2020 2222  les...        ""
+00010a50: 220a 2020 2020 2020 2020 6d6f 6465 6c5f  ".        model_
+00010a60: 7061 7468 203d 2073 656c 662e 736c 7572  path = self.slur
+00010a70: 6d5f 6d6f 6465 6c5f 7061 7468 735b 776f  m_model_paths[wo
+00010a80: 726b 666c 6f77 2e6c 6f77 6572 2829 5d0a  rkflow.lower()].
+00010a90: 2020 2020 2020 2020 6a6f 625f 7363 7269          job_scri
+00010aa0: 7074 203d 2073 656c 662e 736c 7572 6d5f  pt = self.slurm_
+00010ab0: 6d6f 6465 6c5f 6a6f 6273 5b77 6f72 6b66  model_jobs[workf
+00010ac0: 6c6f 772e 6c6f 7765 7228 295d 0a20 2020  low.lower()].   
+00010ad0: 2020 2020 206a 6f62 5f70 6172 616d 7320       job_params 
+00010ae0: 3d20 7365 6c66 2e73 6c75 726d 5f6d 6f64  = self.slurm_mod
+00010af0: 656c 5f6a 6f62 735f 7061 7261 6d73 5b77  el_jobs_params[w
+00010b00: 6f72 6b66 6c6f 772e 6c6f 7765 7228 295d  orkflow.lower()]
+00010b10: 0a20 2020 2020 2020 2023 2067 7261 6220  .        # grab 
+00010b20: 6f6e 6c79 2074 6865 2069 6d61 6765 206e  only the image n
+00010b30: 616d 652c 206e 6f74 2074 6865 2067 726f  ame, not the gro
+00010b40: 7570 2f63 7265 6174 6f72 0a20 2020 2020  up/creator.     
+00010b50: 2020 2069 6d61 6765 203d 2073 656c 662e     image = self.
+00010b60: 736c 7572 6d5f 6d6f 6465 6c5f 696d 6167  slurm_model_imag
+00010b70: 6573 5b77 6f72 6b66 6c6f 772e 6c6f 7765  es[workflow.lowe
+00010b80: 7228 295d 2e73 706c 6974 2822 2f22 295b  r()].split("/")[
+00010b90: 315d 0a0a 2020 2020 2020 2020 7362 6174  1]..        sbat
+00010ba0: 6368 5f65 6e76 203d 207b 0a20 2020 2020  ch_env = {.     
+00010bb0: 2020 2020 2020 2022 4441 5441 5f50 4154         "DATA_PAT
+00010bc0: 4822 3a20 6622 5c22 7b73 656c 662e 736c  H": f"\"{self.sl
+00010bd0: 7572 6d5f 6461 7461 5f70 6174 687d 2f7b  urm_data_path}/{
+00010be0: 696e 7075 745f 6461 7461 7d5c 2222 2c0a  input_data}\"",.
+00010bf0: 2020 2020 2020 2020 2020 2020 2249 4d41              "IMA
+00010c00: 4745 5f50 4154 4822 3a20 6622 5c22 7b73  GE_PATH": f"\"{s
+00010c10: 656c 662e 736c 7572 6d5f 696d 6167 6573  elf.slurm_images
+00010c20: 5f70 6174 687d 2f7b 6d6f 6465 6c5f 7061  _path}/{model_pa
+00010c30: 7468 7d5c 2222 2c0a 2020 2020 2020 2020  th}\"",.        
+00010c40: 2020 2020 2249 4d41 4745 5f56 4552 5349      "IMAGE_VERSI
+00010c50: 4f4e 223a 2066 227b 776f 726b 666c 6f77  ON": f"{workflow
+00010c60: 5f76 6572 7369 6f6e 7d22 2c0a 2020 2020  _version}",.    
+00010c70: 2020 2020 2020 2020 2253 494e 4755 4c41          "SINGULA
+00010c80: 5249 5459 5f49 4d41 4745 223a 2066 225c  RITY_IMAGE": f"\
+00010c90: 227b 696d 6167 657d 5f7b 776f 726b 666c  "{image}_{workfl
+00010ca0: 6f77 5f76 6572 7369 6f6e 7d2e 7369 665c  ow_version}.sif\
+00010cb0: 2222 2c0a 2020 2020 2020 2020 2020 2020  "",.            
+00010cc0: 2253 4352 4950 545f 5041 5448 223a 2066  "SCRIPT_PATH": f
+00010cd0: 225c 227b 7365 6c66 2e73 6c75 726d 5f73  "\"{self.slurm_s
+00010ce0: 6372 6970 745f 7061 7468 7d5c 2222 0a20  cript_path}\"". 
+00010cf0: 2020 2020 2020 207d 0a20 2020 2020 2020         }.       
+00010d00: 2077 6f72 6b66 6c6f 775f 656e 7620 3d20   workflow_env = 
+00010d10: 7365 6c66 2e77 6f72 6b66 6c6f 775f 7061  self.workflow_pa
+00010d20: 7261 6d73 5f74 6f5f 656e 7676 6172 7328  rams_to_envvars(
+00010d30: 2a2a 6b77 6172 6773 290a 2020 2020 2020  **kwargs).      
+00010d40: 2020 656e 7620 3d20 7b2a 2a73 6261 7463    env = {**sbatc
+00010d50: 685f 656e 762c 202a 2a77 6f72 6b66 6c6f  h_env, **workflo
+00010d60: 775f 656e 767d 0a0a 2020 2020 2020 2020  w_env}..        
+00010d70: 656d 6169 6c5f 7061 7261 6d20 3d20 2222  email_param = ""
+00010d80: 2069 6620 656d 6169 6c20 6973 204e 6f6e   if email is Non
+00010d90: 6520 656c 7365 2066 2220 2d2d 6d61 696c  e else f" --mail
+00010da0: 2d75 7365 723d 7b65 6d61 696c 7d22 0a20  -user={email}". 
+00010db0: 2020 2020 2020 2074 696d 655f 7061 7261         time_para
+00010dc0: 6d20 3d20 2222 2069 6620 7469 6d65 2069  m = "" if time i
+00010dd0: 7320 4e6f 6e65 2065 6c73 6520 6622 202d  s None else f" -
+00010de0: 2d74 696d 653d 7b74 696d 657d 220a 2020  -time={time}".  
+00010df0: 2020 2020 2020 6a6f 625f 7061 7261 6d73        job_params
+00010e00: 2e61 7070 656e 6428 7469 6d65 5f70 6172  .append(time_par
+00010e10: 616d 290a 2020 2020 2020 2020 6a6f 625f  am).        job_
+00010e20: 7061 7261 6d73 2e61 7070 656e 6428 656d  params.append(em
+00010e30: 6169 6c5f 7061 7261 6d29 0a20 2020 2020  ail_param).     
+00010e40: 2020 206a 6f62 5f70 6172 616d 203d 2022     job_param = "
+00010e50: 222e 6a6f 696e 286a 6f62 5f70 6172 616d  ".join(job_param
+00010e60: 7329 0a20 2020 2020 2020 2073 6261 7463  s).        sbatc
+00010e70: 685f 636d 6420 3d20 6622 7362 6174 6368  h_cmd = f"sbatch
+00010e80: 7b6a 6f62 5f70 6172 616d 7d20 2d2d 6f75  {job_param} --ou
+00010e90: 7470 7574 3d6f 6d65 726f 2d25 6a2e 6c6f  tput=omero-%j.lo
+00010ea0: 6720 5c0a 2020 2020 2020 2020 2020 2020  g \.            
+00010eb0: 5c22 7b73 656c 662e 736c 7572 6d5f 7363  \"{self.slurm_sc
+00010ec0: 7269 7074 5f70 6174 687d 2f7b 6a6f 625f  ript_path}/{job_
+00010ed0: 7363 7269 7074 7d5c 2222 0a0a 2020 2020  script}\""..    
+00010ee0: 2020 2020 7265 7475 726e 2073 6261 7463      return sbatc
+00010ef0: 685f 636d 642c 2065 6e76 0a0a 2020 2020  h_cmd, env..    
+00010f00: 6465 6620 6765 745f 636f 6e76 6572 7369  def get_conversi
+00010f10: 6f6e 5f63 6f6d 6d61 6e64 2873 656c 662c  on_command(self,
+00010f20: 2064 6174 615f 7061 7468 3a20 7374 722c   data_path: str,
+00010f30: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010f40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f50: 636f 6e66 6967 5f66 696c 653a 2073 7472  config_file: str
+00010f60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00010f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f80: 2073 6f75 7263 655f 666f 726d 6174 3a20   source_format: 
+00010f90: 7374 7220 3d20 277a 6172 7227 2c0a 2020  str = 'zarr',.  
 00010fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010fb0: 2020 2020 2020 2020 2074 6172 6765 745f           target_
-00010fc0: 666f 726d 6174 3a20 7374 7220 3d20 2774  format: str = 't
-00010fd0: 6966 6627 2920 2d3e 2054 7570 6c65 5b73  iff') -> Tuple[s
-00010fe0: 7472 2c20 4469 6374 5d3a 0a20 2020 2020  tr, Dict]:.     
-00010ff0: 2020 2022 2222 0a20 2020 2020 2020 2047     """.        G
-00011000: 656e 6572 6174 6520 536c 7572 6d20 636f  enerate Slurm co
-00011010: 6e76 6572 7369 6f6e 2063 6f6d 6d61 6e64  nversion command
-00011020: 2061 6e64 2065 6e76 6972 6f6e 6d65 6e74   and environment
-00011030: 2076 6172 6961 626c 6573 2066 6f72 2064   variables for d
-00011040: 6174 6120 636f 6e76 6572 7369 6f6e 2e0a  ata conversion..
-00011050: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00011060: 2020 2020 2020 2020 2020 2064 6174 615f             data_
-00011070: 7061 7468 2028 7374 7229 3a20 5061 7468  path (str): Path
-00011080: 2074 6f20 7468 6520 6461 7461 2066 6f6c   to the data fol
-00011090: 6465 722e 0a20 2020 2020 2020 2020 2020  der..           
-000110a0: 2063 6f6e 6669 675f 6669 6c65 2028 7374   config_file (st
-000110b0: 7229 3a20 5061 7468 2074 6f20 7468 6520  r): Path to the 
-000110c0: 636f 6e66 6967 7572 6174 696f 6e20 6669  configuration fi
-000110d0: 6c65 2e0a 2020 2020 2020 2020 2020 2020  le..            
-000110e0: 736f 7572 6365 5f66 6f72 6d61 7420 2873  source_format (s
-000110f0: 7472 293a 2053 6f75 7263 6520 6461 7461  tr): Source data
-00011100: 2066 6f72 6d61 7420 2864 6566 6175 6c74   format (default
-00011110: 2069 7320 277a 6172 7227 292e 0a20 2020   is 'zarr')..   
-00011120: 2020 2020 2020 2020 2074 6172 6765 745f           target_
-00011130: 666f 726d 6174 2028 7374 7229 3a20 5461  format (str): Ta
-00011140: 7267 6574 2064 6174 6120 666f 726d 6174  rget data format
-00011150: 2028 6465 6661 756c 7420 6973 2027 7469   (default is 'ti
-00011160: 6666 2729 2e0a 0a20 2020 2020 2020 2052  ff')...        R
-00011170: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00011180: 2020 2020 5475 706c 655b 7374 722c 2044      Tuple[str, D
-00011190: 6963 745d 3a0a 2020 2020 2020 2020 2020  ict]:.          
-000111a0: 2020 2020 2020 4120 7475 706c 6520 636f        A tuple co
-000111b0: 6e74 6169 6e69 6e67 2074 6865 2053 6c75  ntaining the Slu
-000111c0: 726d 2063 6f6e 7665 7273 696f 6e20 636f  rm conversion co
-000111d0: 6d6d 616e 6420 616e 640a 2020 2020 2020  mmand and.      
-000111e0: 2020 2020 2020 2020 2020 7468 6520 656e            the en
-000111f0: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
-00011200: 6c65 732e 0a0a 2020 2020 2020 2020 5761  les...        Wa
-00011210: 726e 696e 673a 0a20 2020 2020 2020 2020  rning:.         
-00011220: 2020 2054 6865 2064 6566 6175 6c74 2069     The default i
-00011230: 6d70 6c65 6d65 6e74 6174 696f 6e20 6f6e  mplementation on
-00011240: 6c79 2073 7570 706f 7274 7320 636f 6e76  ly supports conv
-00011250: 6572 7369 6f6e 2066 726f 6d20 277a 6172  ersion from 'zar
-00011260: 7227 2074 6f20 2774 6966 6627 2e0a 2020  r' to 'tiff'..  
-00011270: 2020 2020 2020 2020 2020 4966 2075 7369            If usi
-00011280: 6e67 206f 7468 6572 2073 6f75 7263 6520  ng other source 
-00011290: 6f72 2074 6172 6765 7420 666f 726d 6174  or target format
-000112a0: 732c 2075 7365 7273 206d 7573 7420 696d  s, users must im
-000112b0: 706c 656d 656e 7420 616e 6420 636f 6e66  plement and conf
-000112c0: 6967 7572 650a 2020 2020 2020 2020 2020  igure.          
-000112d0: 2020 6164 6469 7469 6f6e 616c 2063 6f6e    additional con
-000112e0: 7665 7274 6572 7320 7468 656d 7365 6c76  verters themselv
-000112f0: 6573 2e0a 2020 2020 2020 2020 2222 220a  es..        """.
-00011300: 2020 2020 2020 2020 6966 2073 6f75 7263          if sourc
-00011310: 655f 666f 726d 6174 2021 3d20 227a 6172  e_format != "zar
-00011320: 7222 206f 7220 7461 7267 6574 5f66 6f72  r" or target_for
-00011330: 6d61 7420 213d 2022 7469 6666 223a 0a20  mat != "tiff":. 
-00011340: 2020 2020 2020 2020 2020 2023 2057 6172             # War
-00011350: 6e20 6162 6f75 7420 756e 7375 7070 6f72  n about unsuppor
-00011360: 7465 6420 636f 6e76 6572 7369 6f6e 3b20  ted conversion; 
-00011370: 6164 6469 7469 6f6e 616c 2063 6f6e 7665  additional conve
-00011380: 7274 6572 7320 6361 6e20 6265 0a20 2020  rters can be.   
-00011390: 2020 2020 2020 2020 2023 2061 6464 6564           # added
-000113a0: 206f 7574 7369 6465 206f 7572 206b 6e6f   outside our kno
-000113b0: 776c 6564 6765 2e0a 2020 2020 2020 2020  wledge..        
-000113c0: 2020 2020 2320 4368 6563 6b69 6e67 2053      # Checking S
-000113d0: 6c75 726d 2773 2060 736c 7572 6d5f 636f  lurm's `slurm_co
-000113e0: 6e76 6572 7465 7273 5f70 6174 6860 2069  nverters_path` i
-000113f0: 7320 736b 6970 7065 6420 666f 720a 2020  s skipped for.  
-00011400: 2020 2020 2020 2020 2020 2320 7065 7266            # perf
-00011410: 6f72 6d61 6e63 6520 7265 6173 6f6e 732e  ormance reasons.
-00011420: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
-00011430: 6765 722e 7761 726e 696e 6728 0a20 2020  ger.warning(.   
-00011440: 2020 2020 2020 2020 2020 2020 2066 2243               f"C
-00011450: 6f6e 7665 7273 696f 6e20 6672 6f6d 207b  onversion from {
-00011460: 736f 7572 6365 5f66 6f72 6d61 747d 2074  source_format} t
-00011470: 6f20 7b74 6172 6765 745f 666f 726d 6174  o {target_format
-00011480: 7d20 6973 206e 6f74 2073 7570 706f 7274  } is not support
-00011490: 6564 2062 7920 6465 6661 756c 7421 2229  ed by default!")
-000114a0: 0a0a 2020 2020 2020 2020 6368 6f73 656e  ..        chosen
-000114b0: 5f63 6f6e 7665 7274 6572 203d 2066 2263  _converter = f"c
-000114c0: 6f6e 7665 7274 5f7b 736f 7572 6365 5f66  onvert_{source_f
-000114d0: 6f72 6d61 747d 5f74 6f5f 7b74 6172 6765  ormat}_to_{targe
-000114e0: 745f 666f 726d 6174 7d2e 7369 6622 0a20  t_format}.sif". 
-000114f0: 2020 2020 2020 2073 6261 7463 685f 656e         sbatch_en
-00011500: 7620 3d20 7b0a 2020 2020 2020 2020 2020  v = {.          
-00011510: 2020 2244 4154 415f 5041 5448 223a 2066    "DATA_PATH": f
-00011520: 225c 227b 6461 7461 5f70 6174 687d 5c22  "\"{data_path}\"
-00011530: 222c 0a20 2020 2020 2020 2020 2020 2022  ",.            "
-00011540: 434f 4e56 4552 5349 4f4e 5f50 4154 4822  CONVERSION_PATH"
-00011550: 3a20 6622 5c22 7b73 656c 662e 736c 7572  : f"\"{self.slur
-00011560: 6d5f 636f 6e76 6572 7465 7273 5f70 6174  m_converters_pat
-00011570: 687d 5c22 222c 0a20 2020 2020 2020 2020  h}\"",.         
-00011580: 2020 2022 434f 4e56 4552 5445 525f 494d     "CONVERTER_IM
-00011590: 4147 4522 3a20 6368 6f73 656e 5f63 6f6e  AGE": chosen_con
-000115a0: 7665 7274 6572 2c0a 2020 2020 2020 2020  verter,.        
-000115b0: 2020 2020 2253 4352 4950 545f 5041 5448      "SCRIPT_PATH
-000115c0: 223a 2066 225c 227b 7365 6c66 2e73 6c75  ": f"\"{self.slu
-000115d0: 726d 5f73 6372 6970 745f 7061 7468 7d5c  rm_script_path}\
-000115e0: 2222 2c0a 2020 2020 2020 2020 2020 2020  "",.            
-000115f0: 2243 4f4e 4649 475f 4649 4c45 223a 2066  "CONFIG_FILE": f
-00011600: 225c 227b 636f 6e66 6967 5f66 696c 657d  "\"{config_file}
-00011610: 5c22 220a 2020 2020 2020 2020 7d0a 0a20  \"".        }.. 
-00011620: 2020 2020 2020 2063 6f6e 7665 7273 696f         conversio
-00011630: 6e5f 636d 6420 3d20 2273 6261 7463 6820  n_cmd = "sbatch 
-00011640: 2d2d 6a6f 622d 6e61 6d65 3d63 6f6e 7665  --job-name=conve
-00011650: 7273 696f 6e20 2d2d 6578 706f 7274 3d41  rsion --export=A
-00011660: 4c4c 2c43 4f4e 4649 475f 5041 5448 3d5c  LL,CONFIG_PATH=\
-00011670: 2224 5057 442f 2443 4f4e 4649 475f 4649  "$PWD/$CONFIG_FI
-00011680: 4c45 5c22 202d 2d61 7272 6179 3d31 2d24  LE\" --array=1-$
-00011690: 4e20 5c22 2453 4352 4950 545f 5041 5448  N \"$SCRIPT_PATH
-000116a0: 2f63 6f6e 7665 7274 5f6a 6f62 5f61 7272  /convert_job_arr
-000116b0: 6179 2e73 685c 2222 0a20 2020 2020 2020  ay.sh\"".       
-000116c0: 2023 2063 6f6e 7665 7273 696f 6e5f 636d   # conversion_cm
-000116d0: 645f 7761 6974 696e 6720 3d20 2273 6261  d_waiting = "sba
-000116e0: 7463 6820 2d2d 6a6f 622d 6e61 6d65 3d63  tch --job-name=c
-000116f0: 6f6e 7665 7273 696f 6e20 2d2d 6578 706f  onversion --expo
-00011700: 7274 3d41 4c4c 2c43 4f4e 4649 475f 5041  rt=ALL,CONFIG_PA
-00011710: 5448 3d5c 2224 5057 442f 2443 4f4e 4649  TH=\"$PWD/$CONFI
-00011720: 475f 4649 4c45 5c22 202d 2d61 7272 6179  G_FILE\" --array
-00011730: 3d31 2d24 4e20 2d2d 7761 6974 2024 5343  =1-$N --wait $SC
-00011740: 5249 5054 5f50 4154 482f 636f 6e76 6572  RIPT_PATH/conver
-00011750: 745f 6a6f 625f 6172 7261 792e 7368 220a  t_job_array.sh".
-00011760: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00011770: 636f 6e76 6572 7369 6f6e 5f63 6d64 2c20  conversion_cmd, 
-00011780: 7362 6174 6368 5f65 6e76 0a0a 2020 2020  sbatch_env..    
-00011790: 6465 6620 776f 726b 666c 6f77 5f70 6172  def workflow_par
-000117a0: 616d 735f 746f 5f65 6e76 7661 7273 2873  ams_to_envvars(s
-000117b0: 656c 662c 202a 2a6b 7761 7267 7329 202d  elf, **kwargs) -
-000117c0: 3e20 4469 6374 3a0a 2020 2020 2020 2020  > Dict:.        
-000117d0: 2222 220a 2020 2020 2020 2020 436f 6e76  """.        Conv
-000117e0: 6572 7420 776f 726b 666c 6f77 2070 6172  ert workflow par
-000117f0: 616d 6574 6572 7320 746f 2065 6e76 6972  ameters to envir
-00011800: 6f6e 6d65 6e74 2076 6172 6961 626c 6573  onment variables
-00011810: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00011820: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
-00011830: 7761 7267 733a 2041 6464 6974 696f 6e61  wargs: Additiona
-00011840: 6c20 6b65 7977 6f72 6420 6172 6775 6d65  l keyword argume
-00011850: 6e74 7320 666f 7220 7468 6520 776f 726b  nts for the work
-00011860: 666c 6f77 2e0a 0a20 2020 2020 2020 2052  flow...        R
-00011870: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00011880: 2020 2020 4469 6374 3a20 4120 6469 6374      Dict: A dict
-00011890: 696f 6e61 7279 2063 6f6e 7461 696e 696e  ionary containin
-000118a0: 6720 7468 6520 656e 7669 726f 6e6d 656e  g the environmen
-000118b0: 7420 7661 7269 6162 6c65 732e 0a20 2020  t variables..   
-000118c0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000118d0: 2077 6f72 6b66 6c6f 775f 656e 7620 3d20   workflow_env = 
-000118e0: 7b6b 6579 2e75 7070 6572 2829 3a20 6622  {key.upper(): f"
-000118f0: 7b76 616c 7565 7d22 2066 6f72 206b 6579  {value}" for key
-00011900: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00011910: 2020 2020 2020 2020 2020 7661 6c75 6520            value 
-00011920: 696e 206b 7761 7267 732e 6974 656d 7328  in kwargs.items(
-00011930: 297d 0a20 2020 2020 2020 206c 6f67 6765  )}.        logge
-00011940: 722e 6465 6275 6728 776f 726b 666c 6f77  r.debug(workflow
-00011950: 5f65 6e76 290a 2020 2020 2020 2020 7265  _env).        re
-00011960: 7475 726e 2077 6f72 6b66 6c6f 775f 656e  turn workflow_en
-00011970: 760a 0a20 2020 2064 6566 2067 6574 5f63  v..    def get_c
-00011980: 656c 6c70 6f73 655f 636f 6d6d 616e 6428  ellpose_command(
-00011990: 7365 6c66 2c20 696d 6167 655f 7665 7273  self, image_vers
-000119a0: 696f 6e3a 2073 7472 2c0a 2020 2020 2020  ion: str,.      
+00010fb0: 2020 2020 2020 2020 2020 2020 2074 6172               tar
+00010fc0: 6765 745f 666f 726d 6174 3a20 7374 7220  get_format: str 
+00010fd0: 3d20 2774 6966 6627 2920 2d3e 2054 7570  = 'tiff') -> Tup
+00010fe0: 6c65 5b73 7472 2c20 4469 6374 5d3a 0a20  le[str, Dict]:. 
+00010ff0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00011000: 2020 2047 656e 6572 6174 6520 536c 7572     Generate Slur
+00011010: 6d20 636f 6e76 6572 7369 6f6e 2063 6f6d  m conversion com
+00011020: 6d61 6e64 2061 6e64 2065 6e76 6972 6f6e  mand and environ
+00011030: 6d65 6e74 2076 6172 6961 626c 6573 2066  ment variables f
+00011040: 6f72 2064 6174 6120 636f 6e76 6572 7369  or data conversi
+00011050: 6f6e 2e0a 0a20 2020 2020 2020 2041 7267  on...        Arg
+00011060: 733a 0a20 2020 2020 2020 2020 2020 2064  s:.            d
+00011070: 6174 615f 7061 7468 2028 7374 7229 3a20  ata_path (str): 
+00011080: 5061 7468 2074 6f20 7468 6520 6461 7461  Path to the data
+00011090: 2066 6f6c 6465 722e 0a20 2020 2020 2020   folder..       
+000110a0: 2020 2020 2063 6f6e 6669 675f 6669 6c65       config_file
+000110b0: 2028 7374 7229 3a20 5061 7468 2074 6f20   (str): Path to 
+000110c0: 7468 6520 636f 6e66 6967 7572 6174 696f  the configuratio
+000110d0: 6e20 6669 6c65 2e0a 2020 2020 2020 2020  n file..        
+000110e0: 2020 2020 736f 7572 6365 5f66 6f72 6d61      source_forma
+000110f0: 7420 2873 7472 293a 2053 6f75 7263 6520  t (str): Source 
+00011100: 6461 7461 2066 6f72 6d61 7420 2864 6566  data format (def
+00011110: 6175 6c74 2069 7320 277a 6172 7227 292e  ault is 'zarr').
+00011120: 0a20 2020 2020 2020 2020 2020 2074 6172  .            tar
+00011130: 6765 745f 666f 726d 6174 2028 7374 7229  get_format (str)
+00011140: 3a20 5461 7267 6574 2064 6174 6120 666f  : Target data fo
+00011150: 726d 6174 2028 6465 6661 756c 7420 6973  rmat (default is
+00011160: 2027 7469 6666 2729 2e0a 0a20 2020 2020   'tiff')...     
+00011170: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00011180: 2020 2020 2020 2020 5475 706c 655b 7374          Tuple[st
+00011190: 722c 2044 6963 745d 3a0a 2020 2020 2020  r, Dict]:.      
+000111a0: 2020 2020 2020 2020 2020 4120 7475 706c            A tupl
+000111b0: 6520 636f 6e74 6169 6e69 6e67 2074 6865  e containing the
+000111c0: 2053 6c75 726d 2063 6f6e 7665 7273 696f   Slurm conversio
+000111d0: 6e20 636f 6d6d 616e 6420 616e 640a 2020  n command and.  
+000111e0: 2020 2020 2020 2020 2020 2020 2020 7468                th
+000111f0: 6520 656e 7669 726f 6e6d 656e 7420 7661  e environment va
+00011200: 7269 6162 6c65 732e 0a0a 2020 2020 2020  riables...      
+00011210: 2020 5761 726e 696e 673a 0a20 2020 2020    Warning:.     
+00011220: 2020 2020 2020 2054 6865 2064 6566 6175         The defau
+00011230: 6c74 2069 6d70 6c65 6d65 6e74 6174 696f  lt implementatio
+00011240: 6e20 6f6e 6c79 2073 7570 706f 7274 7320  n only supports 
+00011250: 636f 6e76 6572 7369 6f6e 2066 726f 6d20  conversion from 
+00011260: 277a 6172 7227 2074 6f20 2774 6966 6627  'zarr' to 'tiff'
+00011270: 2e0a 2020 2020 2020 2020 2020 2020 4966  ..            If
+00011280: 2075 7369 6e67 206f 7468 6572 2073 6f75   using other sou
+00011290: 7263 6520 6f72 2074 6172 6765 7420 666f  rce or target fo
+000112a0: 726d 6174 732c 2075 7365 7273 206d 7573  rmats, users mus
+000112b0: 7420 696d 706c 656d 656e 7420 616e 6420  t implement and 
+000112c0: 636f 6e66 6967 7572 650a 2020 2020 2020  configure.      
+000112d0: 2020 2020 2020 6164 6469 7469 6f6e 616c        additional
+000112e0: 2063 6f6e 7665 7274 6572 7320 7468 656d   converters them
+000112f0: 7365 6c76 6573 2e0a 2020 2020 2020 2020  selves..        
+00011300: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
+00011310: 6f75 7263 655f 666f 726d 6174 2021 3d20  ource_format != 
+00011320: 227a 6172 7222 206f 7220 7461 7267 6574  "zarr" or target
+00011330: 5f66 6f72 6d61 7420 213d 2022 7469 6666  _format != "tiff
+00011340: 223a 0a20 2020 2020 2020 2020 2020 2023  ":.            #
+00011350: 2057 6172 6e20 6162 6f75 7420 756e 7375   Warn about unsu
+00011360: 7070 6f72 7465 6420 636f 6e76 6572 7369  pported conversi
+00011370: 6f6e 3b20 6164 6469 7469 6f6e 616c 2063  on; additional c
+00011380: 6f6e 7665 7274 6572 7320 6361 6e20 6265  onverters can be
+00011390: 0a20 2020 2020 2020 2020 2020 2023 2061  .            # a
+000113a0: 6464 6564 206f 7574 7369 6465 206f 7572  dded outside our
+000113b0: 206b 6e6f 776c 6564 6765 2e0a 2020 2020   knowledge..    
+000113c0: 2020 2020 2020 2020 2320 4368 6563 6b69          # Checki
+000113d0: 6e67 2053 6c75 726d 2773 2060 736c 7572  ng Slurm's `slur
+000113e0: 6d5f 636f 6e76 6572 7465 7273 5f70 6174  m_converters_pat
+000113f0: 6860 2069 7320 736b 6970 7065 6420 666f  h` is skipped fo
+00011400: 720a 2020 2020 2020 2020 2020 2020 2320  r.            # 
+00011410: 7065 7266 6f72 6d61 6e63 6520 7265 6173  performance reas
+00011420: 6f6e 732e 0a20 2020 2020 2020 2020 2020  ons..           
+00011430: 206c 6f67 6765 722e 7761 726e 696e 6728   logger.warning(
+00011440: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011450: 2066 2243 6f6e 7665 7273 696f 6e20 6672   f"Conversion fr
+00011460: 6f6d 207b 736f 7572 6365 5f66 6f72 6d61  om {source_forma
+00011470: 747d 2074 6f20 7b74 6172 6765 745f 666f  t} to {target_fo
+00011480: 726d 6174 7d20 6973 206e 6f74 2073 7570  rmat} is not sup
+00011490: 706f 7274 6564 2062 7920 6465 6661 756c  ported by defaul
+000114a0: 7421 2229 0a0a 2020 2020 2020 2020 6368  t!")..        ch
+000114b0: 6f73 656e 5f63 6f6e 7665 7274 6572 203d  osen_converter =
+000114c0: 2066 2263 6f6e 7665 7274 5f7b 736f 7572   f"convert_{sour
+000114d0: 6365 5f66 6f72 6d61 747d 5f74 6f5f 7b74  ce_format}_to_{t
+000114e0: 6172 6765 745f 666f 726d 6174 7d2e 7369  arget_format}.si
+000114f0: 6622 0a20 2020 2020 2020 2073 6261 7463  f".        sbatc
+00011500: 685f 656e 7620 3d20 7b0a 2020 2020 2020  h_env = {.      
+00011510: 2020 2020 2020 2244 4154 415f 5041 5448        "DATA_PATH
+00011520: 223a 2066 225c 227b 6461 7461 5f70 6174  ": f"\"{data_pat
+00011530: 687d 5c22 222c 0a20 2020 2020 2020 2020  h}\"",.         
+00011540: 2020 2022 434f 4e56 4552 5349 4f4e 5f50     "CONVERSION_P
+00011550: 4154 4822 3a20 6622 5c22 7b73 656c 662e  ATH": f"\"{self.
+00011560: 736c 7572 6d5f 636f 6e76 6572 7465 7273  slurm_converters
+00011570: 5f70 6174 687d 5c22 222c 0a20 2020 2020  _path}\"",.     
+00011580: 2020 2020 2020 2022 434f 4e56 4552 5445         "CONVERTE
+00011590: 525f 494d 4147 4522 3a20 6368 6f73 656e  R_IMAGE": chosen
+000115a0: 5f63 6f6e 7665 7274 6572 2c0a 2020 2020  _converter,.    
+000115b0: 2020 2020 2020 2020 2253 4352 4950 545f          "SCRIPT_
+000115c0: 5041 5448 223a 2066 225c 227b 7365 6c66  PATH": f"\"{self
+000115d0: 2e73 6c75 726d 5f73 6372 6970 745f 7061  .slurm_script_pa
+000115e0: 7468 7d5c 2222 2c0a 2020 2020 2020 2020  th}\"",.        
+000115f0: 2020 2020 2243 4f4e 4649 475f 4649 4c45      "CONFIG_FILE
+00011600: 223a 2066 225c 227b 636f 6e66 6967 5f66  ": f"\"{config_f
+00011610: 696c 657d 5c22 220a 2020 2020 2020 2020  ile}\"".        
+00011620: 7d0a 0a20 2020 2020 2020 2063 6f6e 7665  }..        conve
+00011630: 7273 696f 6e5f 636d 6420 3d20 2273 6261  rsion_cmd = "sba
+00011640: 7463 6820 2d2d 6a6f 622d 6e61 6d65 3d63  tch --job-name=c
+00011650: 6f6e 7665 7273 696f 6e20 2d2d 6578 706f  onversion --expo
+00011660: 7274 3d41 4c4c 2c43 4f4e 4649 475f 5041  rt=ALL,CONFIG_PA
+00011670: 5448 3d5c 2224 5057 442f 2443 4f4e 4649  TH=\"$PWD/$CONFI
+00011680: 475f 4649 4c45 5c22 202d 2d61 7272 6179  G_FILE\" --array
+00011690: 3d31 2d24 4e20 5c22 2453 4352 4950 545f  =1-$N \"$SCRIPT_
+000116a0: 5041 5448 2f63 6f6e 7665 7274 5f6a 6f62  PATH/convert_job
+000116b0: 5f61 7272 6179 2e73 685c 2222 0a20 2020  _array.sh\"".   
+000116c0: 2020 2020 2023 2063 6f6e 7665 7273 696f       # conversio
+000116d0: 6e5f 636d 645f 7761 6974 696e 6720 3d20  n_cmd_waiting = 
+000116e0: 2273 6261 7463 6820 2d2d 6a6f 622d 6e61  "sbatch --job-na
+000116f0: 6d65 3d63 6f6e 7665 7273 696f 6e20 2d2d  me=conversion --
+00011700: 6578 706f 7274 3d41 4c4c 2c43 4f4e 4649  export=ALL,CONFI
+00011710: 475f 5041 5448 3d5c 2224 5057 442f 2443  G_PATH=\"$PWD/$C
+00011720: 4f4e 4649 475f 4649 4c45 5c22 202d 2d61  ONFIG_FILE\" --a
+00011730: 7272 6179 3d31 2d24 4e20 2d2d 7761 6974  rray=1-$N --wait
+00011740: 2024 5343 5249 5054 5f50 4154 482f 636f   $SCRIPT_PATH/co
+00011750: 6e76 6572 745f 6a6f 625f 6172 7261 792e  nvert_job_array.
+00011760: 7368 220a 0a20 2020 2020 2020 2072 6574  sh"..        ret
+00011770: 7572 6e20 636f 6e76 6572 7369 6f6e 5f63  urn conversion_c
+00011780: 6d64 2c20 7362 6174 6368 5f65 6e76 0a0a  md, sbatch_env..
+00011790: 2020 2020 6465 6620 776f 726b 666c 6f77      def workflow
+000117a0: 5f70 6172 616d 735f 746f 5f65 6e76 7661  _params_to_envva
+000117b0: 7273 2873 656c 662c 202a 2a6b 7761 7267  rs(self, **kwarg
+000117c0: 7329 202d 3e20 4469 6374 3a0a 2020 2020  s) -> Dict:.    
+000117d0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000117e0: 436f 6e76 6572 7420 776f 726b 666c 6f77  Convert workflow
+000117f0: 2070 6172 616d 6574 6572 7320 746f 2065   parameters to e
+00011800: 6e76 6972 6f6e 6d65 6e74 2076 6172 6961  nvironment varia
+00011810: 626c 6573 2e0a 0a20 2020 2020 2020 2041  bles...        A
+00011820: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00011830: 202a 2a6b 7761 7267 733a 2041 6464 6974   **kwargs: Addit
+00011840: 696f 6e61 6c20 6b65 7977 6f72 6420 6172  ional keyword ar
+00011850: 6775 6d65 6e74 7320 666f 7220 7468 6520  guments for the 
+00011860: 776f 726b 666c 6f77 2e0a 0a20 2020 2020  workflow...     
+00011870: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00011880: 2020 2020 2020 2020 4469 6374 3a20 4120          Dict: A 
+00011890: 6469 6374 696f 6e61 7279 2063 6f6e 7461  dictionary conta
+000118a0: 696e 696e 6720 7468 6520 656e 7669 726f  ining the enviro
+000118b0: 6e6d 656e 7420 7661 7269 6162 6c65 732e  nment variables.
+000118c0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000118d0: 2020 2020 2077 6f72 6b66 6c6f 775f 656e       workflow_en
+000118e0: 7620 3d20 7b6b 6579 2e75 7070 6572 2829  v = {key.upper()
+000118f0: 3a20 6622 7b76 616c 7565 7d22 2066 6f72  : f"{value}" for
+00011900: 206b 6579 2c0a 2020 2020 2020 2020 2020   key,.          
+00011910: 2020 2020 2020 2020 2020 2020 2020 7661                va
+00011920: 6c75 6520 696e 206b 7761 7267 732e 6974  lue in kwargs.it
+00011930: 656d 7328 297d 0a20 2020 2020 2020 206c  ems()}.        l
+00011940: 6f67 6765 722e 6465 6275 6728 776f 726b  ogger.debug(work
+00011950: 666c 6f77 5f65 6e76 290a 2020 2020 2020  flow_env).      
+00011960: 2020 7265 7475 726e 2077 6f72 6b66 6c6f    return workflo
+00011970: 775f 656e 760a 0a20 2020 2064 6566 2067  w_env..    def g
+00011980: 6574 5f63 656c 6c70 6f73 655f 636f 6d6d  et_cellpose_comm
+00011990: 616e 6428 7365 6c66 2c20 696d 6167 655f  and(self, image_
+000119a0: 7665 7273 696f 6e3a 2073 7472 2c0a 2020  version: str,.  
 000119b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119c0: 2020 2020 2020 2069 6e70 7574 5f64 6174         input_dat
-000119d0: 613a 2073 7472 2c0a 2020 2020 2020 2020  a: str,.        
+000119c0: 2020 2020 2020 2020 2020 2069 6e70 7574             input
+000119d0: 5f64 6174 613a 2073 7472 2c0a 2020 2020  _data: str,.    
 000119e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000119f0: 2020 2020 2063 705f 6d6f 6465 6c3a 2073       cp_model: s
-00011a00: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
+000119f0: 2020 2020 2020 2020 2063 705f 6d6f 6465           cp_mode
+00011a00: 6c3a 2073 7472 2c0a 2020 2020 2020 2020  l: str,.        
 00011a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a20: 206e 7563 5f63 6861 6e6e 656c 3a20 696e   nuc_channel: in
-00011a30: 742c 0a20 2020 2020 2020 2020 2020 2020  t,.             
+00011a20: 2020 2020 206e 7563 5f63 6861 6e6e 656c       nuc_channel
+00011a30: 3a20 696e 742c 0a20 2020 2020 2020 2020  : int,.         
 00011a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a50: 7072 6f62 5f74 6872 6573 686f 6c64 3a20  prob_threshold: 
-00011a60: 666c 6f61 742c 0a20 2020 2020 2020 2020  float,.         
+00011a50: 2020 2020 7072 6f62 5f74 6872 6573 686f      prob_thresho
+00011a60: 6c64 3a20 666c 6f61 742c 0a20 2020 2020  ld: float,.     
 00011a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011a80: 2020 2020 6365 6c6c 5f64 6961 6d65 7465      cell_diamete
-00011a90: 723a 2066 6c6f 6174 2c0a 2020 2020 2020  r: float,.      
+00011a80: 2020 2020 2020 2020 6365 6c6c 5f64 6961          cell_dia
+00011a90: 6d65 7465 723a 2066 6c6f 6174 2c0a 2020  meter: float,.  
 00011aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011ab0: 2020 2020 2020 2065 6d61 696c 3a20 4f70         email: Op
-00011ac0: 7469 6f6e 616c 5b73 7472 5d20 3d20 4e6f  tional[str] = No
-00011ad0: 6e65 2c0a 2020 2020 2020 2020 2020 2020  ne,.            
+00011ab0: 2020 2020 2020 2020 2020 2065 6d61 696c             email
+00011ac0: 3a20 4f70 7469 6f6e 616c 5b73 7472 5d20  : Optional[str] 
+00011ad0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
 00011ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011af0: 2074 696d 653a 204f 7074 696f 6e61 6c5b   time: Optional[
-00011b00: 7374 725d 203d 204e 6f6e 652c 0a20 2020  str] = None,.   
-00011b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b20: 2020 2020 2020 2020 2020 7573 655f 6770            use_gp
-00011b30: 753a 2062 6f6f 6c20 3d20 5472 7565 2c0a  u: bool = True,.
-00011b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011b50: 2020 2020 2020 2020 2020 2020 206d 6f64               mod
-00011b60: 656c 3a20 7374 7220 3d20 2263 656c 6c70  el: str = "cellp
-00011b70: 6f73 6522 2920 2d3e 2054 7570 6c65 5b73  ose") -> Tuple[s
-00011b80: 7472 2c20 4469 6374 5d3a 0a20 2020 2020  tr, Dict]:.     
-00011b90: 2020 2022 2222 0a20 2020 2020 2020 2052     """.        R
-00011ba0: 6574 7572 6e20 7468 6520 636f 6d6d 616e  eturn the comman
-00011bb0: 6420 616e 6420 656e 7669 726f 6e6d 656e  d and environmen
-00011bc0: 7420 6469 6374 696f 6e61 7279 2074 6f20  t dictionary to 
-00011bd0: 7275 6e20 6120 4365 6c6c 506f 7365 206a  run a CellPose j
-00011be0: 6f62 0a20 2020 2020 2020 206f 6e20 7468  ob.        on th
-00011bf0: 6520 536c 7572 6d20 776f 726b 6c6f 6164  e Slurm workload
-00011c00: 206d 616e 6167 6572 2e0a 2020 2020 2020   manager..      
-00011c10: 2020 4120 7370 6563 6966 6963 2065 7861    A specific exa
-00011c20: 6d70 6c65 206f 6620 7573 696e 6720 7468  mple of using th
-00011c30: 6520 6765 6e65 7269 6320 2767 6574 5f77  e generic 'get_w
-00011c40: 6f72 6b66 6c6f 775f 636f 6d6d 616e 6427  orkflow_command'
-00011c50: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00011c60: 0a20 2020 2020 2020 2020 2020 2069 6d61  .            ima
-00011c70: 6765 5f76 6572 7369 6f6e 2028 7374 7229  ge_version (str)
-00011c80: 3a20 5468 6520 7665 7273 696f 6e20 6f66  : The version of
-00011c90: 2074 6865 2053 696e 6775 6c61 7269 7479   the Singularity
-00011ca0: 2069 6d61 6765 2074 6f20 7573 652e 0a20   image to use.. 
-00011cb0: 2020 2020 2020 2020 2020 2069 6e70 7574             input
-00011cc0: 5f64 6174 6120 2873 7472 293a 2054 6865  _data (str): The
-00011cd0: 206e 616d 6520 6f66 2074 6865 2069 6e70   name of the inp
-00011ce0: 7574 2064 6174 6120 666f 6c64 6572 206f  ut data folder o
-00011cf0: 6e20 7468 6520 7368 6172 6564 0a20 2020  n the shared.   
-00011d00: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-00011d10: 6520 7379 7374 656d 2e0a 2020 2020 2020  e system..      
-00011d20: 2020 2020 2020 6370 5f6d 6f64 656c 2028        cp_model (
-00011d30: 7374 7229 3a20 5468 6520 6e61 6d65 206f  str): The name o
-00011d40: 6620 7468 6520 4365 6c6c 506f 7365 206d  f the CellPose m
-00011d50: 6f64 656c 2074 6f20 7573 652e 0a20 2020  odel to use..   
-00011d60: 2020 2020 2020 2020 206e 7563 5f63 6861           nuc_cha
-00011d70: 6e6e 656c 2028 696e 7429 3a20 5468 6520  nnel (int): The 
-00011d80: 696e 6465 7820 6f66 2074 6865 206e 7563  index of the nuc
-00011d90: 6c65 6172 2063 6861 6e6e 656c 2e0a 2020  lear channel..  
-00011da0: 2020 2020 2020 2020 2020 7072 6f62 5f74            prob_t
-00011db0: 6872 6573 686f 6c64 2028 666c 6f61 7429  hreshold (float)
-00011dc0: 3a20 5468 6520 7072 6f62 6162 696c 6974  : The probabilit
-00011dd0: 7920 7468 7265 7368 6f6c 6420 666f 720a  y threshold for.
-00011de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011df0: 6e75 636c 6569 2064 6574 6563 7469 6f6e  nuclei detection
-00011e00: 2e0a 2020 2020 2020 2020 2020 2020 6365  ..            ce
-00011e10: 6c6c 5f64 6961 6d65 7465 7220 2866 6c6f  ll_diameter (flo
-00011e20: 6174 293a 2054 6865 2065 7870 6563 7465  at): The expecte
-00011e30: 6420 6365 6c6c 2064 6961 6d65 7465 7220  d cell diameter 
-00011e40: 696e 2070 6978 656c 732e 0a20 2020 2020  in pixels..     
-00011e50: 2020 2020 2020 2065 6d61 696c 2028 4f70         email (Op
-00011e60: 7469 6f6e 616c 5b73 7472 5d29 3a20 5468  tional[str]): Th
-00011e70: 6520 656d 6169 6c20 6164 6472 6573 7320  e email address 
-00011e80: 746f 2073 656e 6420 6e6f 7469 6669 6361  to send notifica
-00011e90: 7469 6f6e 7320 746f 2e0a 2020 2020 2020  tions to..      
-00011ea0: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-00011eb0: 7473 2074 6f20 4e6f 6e65 2e0a 2020 2020  ts to None..    
-00011ec0: 2020 2020 2020 2020 7469 6d65 2028 4f70          time (Op
-00011ed0: 7469 6f6e 616c 5b73 7472 5d29 3a20 5468  tional[str]): Th
-00011ee0: 6520 6d61 7869 6d75 6d20 7469 6d65 2066  e maximum time f
-00011ef0: 6f72 2074 6865 206a 6f62 2074 6f20 7275  or the job to ru
-00011f00: 6e2e 0a20 2020 2020 2020 2020 2020 2020  n..             
-00011f10: 2020 2044 6566 6175 6c74 7320 746f 204e     Defaults to N
-00011f20: 6f6e 652e 0a20 2020 2020 2020 2020 2020  one..           
-00011f30: 2075 7365 5f67 7075 2028 626f 6f6c 293a   use_gpu (bool):
-00011f40: 2057 6865 7468 6572 2074 6f20 7573 6520   Whether to use 
-00011f50: 4750 5520 666f 7220 7468 6520 4365 6c6c  GPU for the Cell
-00011f60: 506f 7365 206a 6f62 2e0a 2020 2020 2020  Pose job..      
-00011f70: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-00011f80: 7473 2074 6f20 5472 7565 2e0a 2020 2020  ts to True..    
-00011f90: 2020 2020 2020 2020 6d6f 6465 6c20 2873          model (s
-00011fa0: 7472 293a 2054 6865 206e 616d 6520 6f66  tr): The name of
-00011fb0: 2074 6865 2066 6f6c 6465 7220 6f66 2074   the folder of t
-00011fc0: 6865 2044 6f63 6b65 7220 696d 6167 6520  he Docker image 
-00011fd0: 746f 2075 7365 2e0a 2020 2020 2020 2020  to use..        
-00011fe0: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
-00011ff0: 2074 6f20 2263 656c 6c70 6f73 6522 2e0a   to "cellpose"..
-00012000: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
-00012010: 3a0a 2020 2020 2020 2020 2020 2020 5475  :.            Tu
-00012020: 706c 655b 7374 722c 2064 6963 745d 3a0a  ple[str, dict]:.
-00012030: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012040: 4120 7475 706c 6520 636f 6e74 6169 6e69  A tuple containi
-00012050: 6e67 2074 6865 2053 6c75 726d 2073 6261  ng the Slurm sba
-00012060: 7463 6820 636f 6d6d 616e 640a 2020 2020  tch command.    
-00012070: 2020 2020 2020 2020 2020 2020 616e 6420              and 
-00012080: 7468 6520 656e 7669 726f 6e6d 656e 7420  the environment 
-00012090: 6469 6374 696f 6e61 7279 2e0a 2020 2020  dictionary..    
-000120a0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000120b0: 7265 7475 726e 2073 656c 662e 6765 745f  return self.get_
-000120c0: 776f 726b 666c 6f77 5f63 6f6d 6d61 6e64  workflow_command
-000120d0: 2877 6f72 6b66 6c6f 773d 6d6f 6465 6c2c  (workflow=model,
-000120e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011af0: 2020 2020 2074 696d 653a 204f 7074 696f       time: Optio
+00011b00: 6e61 6c5b 7374 725d 203d 204e 6f6e 652c  nal[str] = None,
+00011b10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011b20: 2020 2020 2020 2020 2020 2020 2020 7573                us
+00011b30: 655f 6770 753a 2062 6f6f 6c20 3d20 5472  e_gpu: bool = Tr
+00011b40: 7565 2c0a 2020 2020 2020 2020 2020 2020  ue,.            
+00011b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011b60: 206d 6f64 656c 3a20 7374 7220 3d20 2263   model: str = "c
+00011b70: 656c 6c70 6f73 6522 2920 2d3e 2054 7570  ellpose") -> Tup
+00011b80: 6c65 5b73 7472 2c20 4469 6374 5d3a 0a20  le[str, Dict]:. 
+00011b90: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00011ba0: 2020 2052 6574 7572 6e20 7468 6520 636f     Return the co
+00011bb0: 6d6d 616e 6420 616e 6420 656e 7669 726f  mmand and enviro
+00011bc0: 6e6d 656e 7420 6469 6374 696f 6e61 7279  nment dictionary
+00011bd0: 2074 6f20 7275 6e20 6120 4365 6c6c 506f   to run a CellPo
+00011be0: 7365 206a 6f62 0a20 2020 2020 2020 206f  se job.        o
+00011bf0: 6e20 7468 6520 536c 7572 6d20 776f 726b  n the Slurm work
+00011c00: 6c6f 6164 206d 616e 6167 6572 2e0a 2020  load manager..  
+00011c10: 2020 2020 2020 4120 7370 6563 6966 6963        A specific
+00011c20: 2065 7861 6d70 6c65 206f 6620 7573 696e   example of usin
+00011c30: 6720 7468 6520 6765 6e65 7269 6320 2767  g the generic 'g
+00011c40: 6574 5f77 6f72 6b66 6c6f 775f 636f 6d6d  et_workflow_comm
+00011c50: 616e 6427 2e0a 0a20 2020 2020 2020 2041  and'...        A
+00011c60: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00011c70: 2069 6d61 6765 5f76 6572 7369 6f6e 2028   image_version (
+00011c80: 7374 7229 3a20 5468 6520 7665 7273 696f  str): The versio
+00011c90: 6e20 6f66 2074 6865 2053 696e 6775 6c61  n of the Singula
+00011ca0: 7269 7479 2069 6d61 6765 2074 6f20 7573  rity image to us
+00011cb0: 652e 0a20 2020 2020 2020 2020 2020 2069  e..            i
+00011cc0: 6e70 7574 5f64 6174 6120 2873 7472 293a  nput_data (str):
+00011cd0: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
+00011ce0: 2069 6e70 7574 2064 6174 6120 666f 6c64   input data fold
+00011cf0: 6572 206f 6e20 7468 6520 7368 6172 6564  er on the shared
+00011d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011d10: 2066 696c 6520 7379 7374 656d 2e0a 2020   file system..  
+00011d20: 2020 2020 2020 2020 2020 6370 5f6d 6f64            cp_mod
+00011d30: 656c 2028 7374 7229 3a20 5468 6520 6e61  el (str): The na
+00011d40: 6d65 206f 6620 7468 6520 4365 6c6c 506f  me of the CellPo
+00011d50: 7365 206d 6f64 656c 2074 6f20 7573 652e  se model to use.
+00011d60: 0a20 2020 2020 2020 2020 2020 206e 7563  .            nuc
+00011d70: 5f63 6861 6e6e 656c 2028 696e 7429 3a20  _channel (int): 
+00011d80: 5468 6520 696e 6465 7820 6f66 2074 6865  The index of the
+00011d90: 206e 7563 6c65 6172 2063 6861 6e6e 656c   nuclear channel
+00011da0: 2e0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00011db0: 6f62 5f74 6872 6573 686f 6c64 2028 666c  ob_threshold (fl
+00011dc0: 6f61 7429 3a20 5468 6520 7072 6f62 6162  oat): The probab
+00011dd0: 696c 6974 7920 7468 7265 7368 6f6c 6420  ility threshold 
+00011de0: 666f 720a 2020 2020 2020 2020 2020 2020  for.            
+00011df0: 2020 2020 6e75 636c 6569 2064 6574 6563      nuclei detec
+00011e00: 7469 6f6e 2e0a 2020 2020 2020 2020 2020  tion..          
+00011e10: 2020 6365 6c6c 5f64 6961 6d65 7465 7220    cell_diameter 
+00011e20: 2866 6c6f 6174 293a 2054 6865 2065 7870  (float): The exp
+00011e30: 6563 7465 6420 6365 6c6c 2064 6961 6d65  ected cell diame
+00011e40: 7465 7220 696e 2070 6978 656c 732e 0a20  ter in pixels.. 
+00011e50: 2020 2020 2020 2020 2020 2065 6d61 696c             email
+00011e60: 2028 4f70 7469 6f6e 616c 5b73 7472 5d29   (Optional[str])
+00011e70: 3a20 5468 6520 656d 6169 6c20 6164 6472  : The email addr
+00011e80: 6573 7320 746f 2073 656e 6420 6e6f 7469  ess to send noti
+00011e90: 6669 6361 7469 6f6e 7320 746f 2e0a 2020  fications to..  
+00011ea0: 2020 2020 2020 2020 2020 2020 2020 4465                De
+00011eb0: 6661 756c 7473 2074 6f20 4e6f 6e65 2e0a  faults to None..
+00011ec0: 2020 2020 2020 2020 2020 2020 7469 6d65              time
+00011ed0: 2028 4f70 7469 6f6e 616c 5b73 7472 5d29   (Optional[str])
+00011ee0: 3a20 5468 6520 6d61 7869 6d75 6d20 7469  : The maximum ti
+00011ef0: 6d65 2066 6f72 2074 6865 206a 6f62 2074  me for the job t
+00011f00: 6f20 7275 6e2e 0a20 2020 2020 2020 2020  o run..         
+00011f10: 2020 2020 2020 2044 6566 6175 6c74 7320         Defaults 
+00011f20: 746f 204e 6f6e 652e 0a20 2020 2020 2020  to None..       
+00011f30: 2020 2020 2075 7365 5f67 7075 2028 626f       use_gpu (bo
+00011f40: 6f6c 293a 2057 6865 7468 6572 2074 6f20  ol): Whether to 
+00011f50: 7573 6520 4750 5520 666f 7220 7468 6520  use GPU for the 
+00011f60: 4365 6c6c 506f 7365 206a 6f62 2e0a 2020  CellPose job..  
+00011f70: 2020 2020 2020 2020 2020 2020 2020 4465                De
+00011f80: 6661 756c 7473 2074 6f20 5472 7565 2e0a  faults to True..
+00011f90: 2020 2020 2020 2020 2020 2020 6d6f 6465              mode
+00011fa0: 6c20 2873 7472 293a 2054 6865 206e 616d  l (str): The nam
+00011fb0: 6520 6f66 2074 6865 2066 6f6c 6465 7220  e of the folder 
+00011fc0: 6f66 2074 6865 2044 6f63 6b65 7220 696d  of the Docker im
+00011fd0: 6167 6520 746f 2075 7365 2e0a 2020 2020  age to use..    
+00011fe0: 2020 2020 2020 2020 2020 2020 4465 6661              Defa
+00011ff0: 756c 7473 2074 6f20 2263 656c 6c70 6f73  ults to "cellpos
+00012000: 6522 2e0a 0a20 2020 2020 2020 2052 6574  e"...        Ret
+00012010: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+00012020: 2020 5475 706c 655b 7374 722c 2064 6963    Tuple[str, dic
+00012030: 745d 3a0a 2020 2020 2020 2020 2020 2020  t]:.            
+00012040: 2020 2020 4120 7475 706c 6520 636f 6e74      A tuple cont
+00012050: 6169 6e69 6e67 2074 6865 2053 6c75 726d  aining the Slurm
+00012060: 2073 6261 7463 6820 636f 6d6d 616e 640a   sbatch command.
+00012070: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012080: 616e 6420 7468 6520 656e 7669 726f 6e6d  and the environm
+00012090: 656e 7420 6469 6374 696f 6e61 7279 2e0a  ent dictionary..
+000120a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000120b0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
+000120c0: 6765 745f 776f 726b 666c 6f77 5f63 6f6d  get_workflow_com
+000120d0: 6d61 6e64 2877 6f72 6b66 6c6f 773d 6d6f  mand(workflow=mo
+000120e0: 6465 6c2c 0a20 2020 2020 2020 2020 2020  del,.           
 000120f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012100: 2020 2020 2020 2020 2020 776f 726b 666c            workfl
-00012110: 6f77 5f76 6572 7369 6f6e 3d69 6d61 6765  ow_version=image
-00012120: 5f76 6572 7369 6f6e 2c0a 2020 2020 2020  _version,.      
+00012100: 2020 2020 2020 2020 2020 2020 2020 776f                wo
+00012110: 726b 666c 6f77 5f76 6572 7369 6f6e 3d69  rkflow_version=i
+00012120: 6d61 6765 5f76 6572 7369 6f6e 2c0a 2020  mage_version,.  
 00012130: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012140: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012150: 2020 2069 6e70 7574 5f64 6174 613d 696e     input_data=in
-00012160: 7075 745f 6461 7461 2c0a 2020 2020 2020  put_data,.      
+00012150: 2020 2020 2020 2069 6e70 7574 5f64 6174         input_dat
+00012160: 613d 696e 7075 745f 6461 7461 2c0a 2020  a=input_data,.  
 00012170: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00012180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012190: 2020 2065 6d61 696c 3d65 6d61 696c 2c0a     email=email,.
-000121a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012190: 2020 2020 2020 2065 6d61 696c 3d65 6d61         email=ema
+000121a0: 696c 2c0a 2020 2020 2020 2020 2020 2020  il,.            
 000121b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121c0: 2020 2020 2020 2020 2074 696d 653d 7469           time=ti
-000121d0: 6d65 2c0a 2020 2020 2020 2020 2020 2020  me,.            
+000121c0: 2020 2020 2020 2020 2020 2020 2074 696d               tim
+000121d0: 653d 7469 6d65 2c0a 2020 2020 2020 2020  e=time,.        
 000121e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000121f0: 2020 2020 2020 2020 2020 2020 2063 705f               cp_
-00012200: 6d6f 6465 6c3d 6370 5f6d 6f64 656c 2c0a  model=cp_model,.
-00012210: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000121f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012200: 2063 705f 6d6f 6465 6c3d 6370 5f6d 6f64   cp_model=cp_mod
+00012210: 656c 2c0a 2020 2020 2020 2020 2020 2020  el,.            
 00012220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012230: 2020 2020 2020 2020 206e 7563 5f63 6861           nuc_cha
-00012240: 6e6e 656c 3d6e 7563 5f63 6861 6e6e 656c  nnel=nuc_channel
-00012250: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00012230: 2020 2020 2020 2020 2020 2020 206e 7563               nuc
+00012240: 5f63 6861 6e6e 656c 3d6e 7563 5f63 6861  _channel=nuc_cha
+00012250: 6e6e 656c 2c0a 2020 2020 2020 2020 2020  nnel,.          
 00012260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012270: 2020 2020 2020 2020 2020 2070 726f 625f             prob_
-00012280: 7468 7265 7368 6f6c 643d 7072 6f62 5f74  threshold=prob_t
-00012290: 6872 6573 686f 6c64 2c0a 2020 2020 2020  hreshold,.      
+00012270: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+00012280: 726f 625f 7468 7265 7368 6f6c 643d 7072  rob_threshold=pr
+00012290: 6f62 5f74 6872 6573 686f 6c64 2c0a 2020  ob_threshold,.  
 000122a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 000122b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000122c0: 2020 2063 656c 6c5f 6469 616d 6574 6572     cell_diameter
-000122d0: 3d63 656c 6c5f 6469 616d 6574 6572 2c0a  =cell_diameter,.
-000122e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000122c0: 2020 2020 2020 2063 656c 6c5f 6469 616d         cell_diam
+000122d0: 6574 6572 3d63 656c 6c5f 6469 616d 6574  eter=cell_diamet
+000122e0: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
 000122f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012300: 2020 2020 2020 2020 2075 7365 5f67 7075           use_gpu
-00012310: 3d75 7365 5f67 7075 290a 0a20 2020 2064  =use_gpu)..    d
-00012320: 6566 2063 6f70 795f 7a69 705f 6c6f 6361  ef copy_zip_loca
-00012330: 6c6c 7928 7365 6c66 2c20 6c6f 6361 6c5f  lly(self, local_
-00012340: 746d 705f 7374 6f72 6167 653a 2073 7472  tmp_storage: str
-00012350: 2c20 6669 6c65 6e61 6d65 3a20 7374 720a  , filename: str.
-00012360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012370: 2020 2020 2020 2020 2029 202d 3e20 5472           ) -> Tr
-00012380: 616e 7366 6572 5265 7375 6c74 3a0a 2020  ansferResult:.  
-00012390: 2020 2020 2020 2222 2220 436f 7079 2061        """ Copy a
-000123a0: 207a 6970 2066 696c 6520 6672 6f6d 2053   zip file from S
-000123b0: 6c75 726d 2074 6f20 7468 6520 6c6f 6361  lurm to the loca
-000123c0: 6c20 7365 7276 6572 2e0a 0a20 2020 2020  l server...     
-000123d0: 2020 204e 6f74 6520 6162 6f75 7420 2854     Note about (T
-000123e0: 7261 6e73 6665 7229 5265 7375 6c74 3a0a  ransfer)Result:.
-000123f0: 0a20 2020 2020 2020 2055 6e6c 696b 6520  .        Unlike 
-00012400: 7369 6d69 6c61 7220 636c 6173 7365 7320  similar classes 
-00012410: 7375 6368 2061 7320 696e 766f 6b65 2e72  such as invoke.r
-00012420: 756e 6e65 7273 2e52 6573 756c 7420 6f72  unners.Result or
-00012430: 0a20 2020 2020 2020 2066 6162 7269 632e  .        fabric.
-00012440: 7275 6e6e 6572 732e 5265 7375 6c74 0a20  runners.Result. 
-00012450: 2020 2020 2020 2028 7768 6963 6820 6861         (which ha
-00012460: 7665 2061 2063 6f6e 6365 7074 206f 6620  ve a concept of 
-00012470: e280 9c77 6172 6e20 616e 6420 7265 7475  ...warn and retu
-00012480: 726e 2061 6e79 7761 7973 206f 6e20 6661  rn anyways on fa
-00012490: 696c 7572 65e2 809d 290a 2020 2020 2020  ilure...).      
-000124a0: 2020 7468 6973 2063 6c61 7373 2068 6173    this class has
-000124b0: 206e 6f20 7573 6566 756c 2074 7275 7468   no useful truth
-000124c0: 696e 6573 7320 6265 6861 7669 6f72 2e0a  iness behavior..
-000124d0: 2020 2020 2020 2020 4966 2061 2066 696c          If a fil
-000124e0: 6520 7472 616e 7366 6572 2066 6169 6c73  e transfer fails
-000124f0: 2c20 736f 6d65 2065 7863 6570 7469 6f6e  , some exception
-00012500: 2077 696c 6c20 6265 2072 6169 7365 642c   will be raised,
-00012510: 0a20 2020 2020 2020 2065 6974 6865 7220  .        either 
-00012520: 616e 204f 5345 7272 6f72 206f 7220 616e  an OSError or an
-00012530: 2065 7272 6f72 2066 726f 6d20 7769 7468   error from with
-00012540: 696e 2050 6172 616d 696b 6f2e 0a0a 2020  in Paramiko...  
-00012550: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00012560: 2020 2020 2020 2020 6c6f 6361 6c5f 746d          local_tm
-00012570: 705f 7374 6f72 6167 6520 2853 7472 696e  p_storage (Strin
-00012580: 6729 3a20 5061 7468 2074 6f20 7374 6f72  g): Path to stor
-00012590: 6520 7468 6520 7a69 7020 6669 6c65 206c  e the zip file l
-000125a0: 6f63 616c 6c79 2e0a 2020 2020 2020 2020  ocally..        
-000125b0: 2020 2020 6669 6c65 6e61 6d65 2028 5374      filename (St
-000125c0: 7269 6e67 293a 205a 6970 2066 696c 656e  ring): Zip filen
-000125d0: 616d 6520 6f6e 2053 6c75 726d 2e0a 0a20  ame on Slurm... 
-000125e0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-000125f0: 2020 2020 2020 2020 2020 2020 5472 616e              Tran
-00012600: 7366 6572 5265 7375 6c74 3a20 5468 6520  sferResult: The 
-00012610: 7265 7375 6c74 206f 6620 7468 6520 7363  result of the sc
-00012620: 7020 6174 7465 6d70 742e 0a20 2020 2020  p attempt..     
-00012630: 2020 2022 2222 0a20 2020 2020 2020 206c     """.        l
-00012640: 6f67 6765 722e 696e 666f 2866 2243 6f70  ogger.info(f"Cop
-00012650: 7969 6e67 207a 6970 207b 6669 6c65 6e61  ying zip {filena
-00012660: 6d65 7d20 6672 6f6d 5c0a 2020 2020 2020  me} from\.      
-00012670: 2020 2020 2020 536c 7572 6d20 746f 207b        Slurm to {
-00012680: 6c6f 6361 6c5f 746d 705f 7374 6f72 6167  local_tmp_storag
-00012690: 657d 2229 0a20 2020 2020 2020 2072 6574  e}").        ret
-000126a0: 7572 6e20 7365 6c66 2e67 6574 280a 2020  urn self.get(.  
-000126b0: 2020 2020 2020 2020 2020 7265 6d6f 7465            remote
-000126c0: 3d66 227b 6669 6c65 6e61 6d65 7d2e 7a69  =f"{filename}.zi
-000126d0: 7022 2c0a 2020 2020 2020 2020 2020 2020  p",.            
-000126e0: 6c6f 6361 6c3d 6c6f 6361 6c5f 746d 705f  local=local_tmp_
-000126f0: 7374 6f72 6167 6529 0a0a 2020 2020 6465  storage)..    de
-00012700: 6620 7a69 705f 6461 7461 5f6f 6e5f 736c  f zip_data_on_sl
-00012710: 7572 6d5f 7365 7276 6572 2873 656c 662c  urm_server(self,
-00012720: 2064 6174 615f 6c6f 6361 7469 6f6e 3a20   data_location: 
-00012730: 7374 722c 2066 696c 656e 616d 653a 2073  str, filename: s
-00012740: 7472 2c0a 2020 2020 2020 2020 2020 2020  tr,.            
+00012300: 2020 2020 2020 2020 2020 2020 2075 7365               use
+00012310: 5f67 7075 3d75 7365 5f67 7075 290a 0a20  _gpu=use_gpu).. 
+00012320: 2020 2064 6566 2063 6f70 795f 7a69 705f     def copy_zip_
+00012330: 6c6f 6361 6c6c 7928 7365 6c66 2c20 6c6f  locally(self, lo
+00012340: 6361 6c5f 746d 705f 7374 6f72 6167 653a  cal_tmp_storage:
+00012350: 2073 7472 2c20 6669 6c65 6e61 6d65 3a20   str, filename: 
+00012360: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
+00012370: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
+00012380: 3e20 5472 616e 7366 6572 5265 7375 6c74  > TransferResult
+00012390: 3a0a 2020 2020 2020 2020 2222 2220 436f  :.        """ Co
+000123a0: 7079 2061 207a 6970 2066 696c 6520 6672  py a zip file fr
+000123b0: 6f6d 2053 6c75 726d 2074 6f20 7468 6520  om Slurm to the 
+000123c0: 6c6f 6361 6c20 7365 7276 6572 2e0a 0a20  local server... 
+000123d0: 2020 2020 2020 204e 6f74 6520 6162 6f75         Note abou
+000123e0: 7420 2854 7261 6e73 6665 7229 5265 7375  t (Transfer)Resu
+000123f0: 6c74 3a0a 0a20 2020 2020 2020 2055 6e6c  lt:..        Unl
+00012400: 696b 6520 7369 6d69 6c61 7220 636c 6173  ike similar clas
+00012410: 7365 7320 7375 6368 2061 7320 696e 766f  ses such as invo
+00012420: 6b65 2e72 756e 6e65 7273 2e52 6573 756c  ke.runners.Resul
+00012430: 7420 6f72 0a20 2020 2020 2020 2066 6162  t or.        fab
+00012440: 7269 632e 7275 6e6e 6572 732e 5265 7375  ric.runners.Resu
+00012450: 6c74 0a20 2020 2020 2020 2028 7768 6963  lt.        (whic
+00012460: 6820 6861 7665 2061 2063 6f6e 6365 7074  h have a concept
+00012470: 206f 6620 e280 9c77 6172 6e20 616e 6420   of ...warn and 
+00012480: 7265 7475 726e 2061 6e79 7761 7973 206f  return anyways o
+00012490: 6e20 6661 696c 7572 65e2 809d 290a 2020  n failure...).  
+000124a0: 2020 2020 2020 7468 6973 2063 6c61 7373        this class
+000124b0: 2068 6173 206e 6f20 7573 6566 756c 2074   has no useful t
+000124c0: 7275 7468 696e 6573 7320 6265 6861 7669  ruthiness behavi
+000124d0: 6f72 2e0a 2020 2020 2020 2020 4966 2061  or..        If a
+000124e0: 2066 696c 6520 7472 616e 7366 6572 2066   file transfer f
+000124f0: 6169 6c73 2c20 736f 6d65 2065 7863 6570  ails, some excep
+00012500: 7469 6f6e 2077 696c 6c20 6265 2072 6169  tion will be rai
+00012510: 7365 642c 0a20 2020 2020 2020 2065 6974  sed,.        eit
+00012520: 6865 7220 616e 204f 5345 7272 6f72 206f  her an OSError o
+00012530: 7220 616e 2065 7272 6f72 2066 726f 6d20  r an error from 
+00012540: 7769 7468 696e 2050 6172 616d 696b 6f2e  within Paramiko.
+00012550: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00012560: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
+00012570: 6c5f 746d 705f 7374 6f72 6167 6520 2853  l_tmp_storage (S
+00012580: 7472 696e 6729 3a20 5061 7468 2074 6f20  tring): Path to 
+00012590: 7374 6f72 6520 7468 6520 7a69 7020 6669  store the zip fi
+000125a0: 6c65 206c 6f63 616c 6c79 2e0a 2020 2020  le locally..    
+000125b0: 2020 2020 2020 2020 6669 6c65 6e61 6d65          filename
+000125c0: 2028 5374 7269 6e67 293a 205a 6970 2066   (String): Zip f
+000125d0: 696c 656e 616d 6520 6f6e 2053 6c75 726d  ilename on Slurm
+000125e0: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+000125f0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00012600: 5472 616e 7366 6572 5265 7375 6c74 3a20  TransferResult: 
+00012610: 5468 6520 7265 7375 6c74 206f 6620 7468  The result of th
+00012620: 6520 7363 7020 6174 7465 6d70 742e 0a20  e scp attempt.. 
+00012630: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00012640: 2020 206c 6f67 6765 722e 696e 666f 2866     logger.info(f
+00012650: 2243 6f70 7969 6e67 207a 6970 207b 6669  "Copying zip {fi
+00012660: 6c65 6e61 6d65 7d20 6672 6f6d 5c0a 2020  lename} from\.  
+00012670: 2020 2020 2020 2020 2020 536c 7572 6d20            Slurm 
+00012680: 746f 207b 6c6f 6361 6c5f 746d 705f 7374  to {local_tmp_st
+00012690: 6f72 6167 657d 2229 0a20 2020 2020 2020  orage}").       
+000126a0: 2072 6574 7572 6e20 7365 6c66 2e67 6574   return self.get
+000126b0: 280a 2020 2020 2020 2020 2020 2020 7265  (.            re
+000126c0: 6d6f 7465 3d66 227b 6669 6c65 6e61 6d65  mote=f"{filename
+000126d0: 7d2e 7a69 7022 2c0a 2020 2020 2020 2020  }.zip",.        
+000126e0: 2020 2020 6c6f 6361 6c3d 6c6f 6361 6c5f      local=local_
+000126f0: 746d 705f 7374 6f72 6167 6529 0a0a 2020  tmp_storage)..  
+00012700: 2020 6465 6620 7a69 705f 6461 7461 5f6f    def zip_data_o
+00012710: 6e5f 736c 7572 6d5f 7365 7276 6572 2873  n_slurm_server(s
+00012720: 656c 662c 2064 6174 615f 6c6f 6361 7469  elf, data_locati
+00012730: 6f6e 3a20 7374 722c 2066 696c 656e 616d  on: str, filenam
+00012740: 653a 2073 7472 2c0a 2020 2020 2020 2020  e: str,.        
 00012750: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012760: 2020 2020 2065 6e76 3a20 4f70 7469 6f6e       env: Option
-00012770: 616c 5b44 6963 745b 7374 722c 2073 7472  al[Dict[str, str
-00012780: 5d5d 203d 204e 6f6e 650a 2020 2020 2020  ]] = None.      
+00012760: 2020 2020 2020 2020 2065 6e76 3a20 4f70           env: Op
+00012770: 7469 6f6e 616c 5b44 6963 745b 7374 722c  tional[Dict[str,
+00012780: 2073 7472 5d5d 203d 204e 6f6e 650a 2020   str]] = None.  
 00012790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000127a0: 2020 2020 2020 2020 2020 2029 202d 3e20             ) -> 
-000127b0: 5265 7375 6c74 3a0a 2020 2020 2020 2020  Result:.        
-000127c0: 2222 225a 6970 2074 6865 206f 7574 7075  """Zip the outpu
-000127d0: 7420 666f 6c64 6572 206f 6620 6120 6a6f  t folder of a jo
-000127e0: 6220 6f6e 2053 6c75 726d 0a0a 2020 2020  b on Slurm..    
-000127f0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00012800: 2020 2020 2020 6461 7461 5f6c 6f63 6174        data_locat
-00012810: 696f 6e20 2853 7472 696e 6729 3a20 466f  ion (String): Fo
-00012820: 6c64 6572 206f 6e20 534c 5552 4d20 7769  lder on SLURM wi
-00012830: 7468 2074 6865 2022 6461 7461 2f6f 7574  th the "data/out
-00012840: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-00012850: 2020 7375 6266 6f6c 6465 722e 0a20 2020    subfolder..   
-00012860: 2020 2020 2020 2020 2066 696c 656e 616d           filenam
-00012870: 6520 2853 7472 696e 6729 3a20 4e61 6d65  e (String): Name
-00012880: 2074 6f20 6769 7665 2074 6f20 7468 6520   to give to the 
-00012890: 7a69 7066 696c 652e 0a20 2020 2020 2020  zipfile..       
-000128a0: 2020 2020 2065 6e76 2028 4469 6374 5b73       env (Dict[s
-000128b0: 7472 2c20 7374 725d 2c20 6f70 7469 6f6e  tr, str], option
-000128c0: 616c 293a 204f 7074 696f 6e61 6c20 656e  al): Optional en
-000128d0: 7669 726f 6e6d 656e 7420 7661 7269 6162  vironment variab
-000128e0: 6c65 7320 746f 200a 2020 2020 2020 2020  les to .        
-000128f0: 2020 2020 2020 2020 7365 7420 7768 656e          set when
-00012900: 2072 756e 6e69 6e67 2074 6865 2063 6f6d   running the com
-00012910: 6d61 6e64 2e20 4465 6661 756c 7473 2074  mand. Defaults t
-00012920: 6f20 4e6f 6e65 2e0a 0a20 2020 2020 2020  o None...       
-00012930: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-00012940: 2020 2020 2020 5265 7375 6c74 3a20 5468        Result: Th
-00012950: 6520 7265 7375 6c74 206f 6620 7468 6520  e result of the 
-00012960: 7a69 7020 6174 7465 6d70 742e 0a20 2020  zip attempt..   
-00012970: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012980: 2023 207a 6970 0a20 2020 2020 2020 207a   # zip.        z
-00012990: 6970 5f63 6d64 203d 2073 656c 662e 6765  ip_cmd = self.ge
-000129a0: 745f 7a69 705f 636f 6d6d 616e 6428 6461  t_zip_command(da
-000129b0: 7461 5f6c 6f63 6174 696f 6e2c 2066 696c  ta_location, fil
-000129c0: 656e 616d 6529 0a20 2020 2020 2020 206c  ename).        l
-000129d0: 6f67 6765 722e 696e 666f 2866 225a 6970  ogger.info(f"Zip
-000129e0: 7069 6e67 207b 6461 7461 5f6c 6f63 6174  ping {data_locat
-000129f0: 696f 6e7d 2061 7320 7b66 696c 656e 616d  ion} as {filenam
-00012a00: 657d 206f 6e20 536c 7572 6d22 290a 2020  e} on Slurm").  
-00012a10: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00012a20: 662e 7275 6e5f 636f 6d6d 616e 6473 285b  f.run_commands([
-00012a30: 7a69 705f 636d 645d 2c20 656e 763d 656e  zip_cmd], env=en
-00012a40: 7629 0a0a 2020 2020 6465 6620 6765 745f  v)..    def get_
-00012a50: 7a69 705f 636f 6d6d 616e 6428 7365 6c66  zip_command(self
-00012a60: 2c20 6461 7461 5f6c 6f63 6174 696f 6e3a  , data_location:
-00012a70: 2073 7472 2c20 6669 6c65 6e61 6d65 3a20   str, filename: 
-00012a80: 7374 7229 202d 3e20 7374 723a 0a20 2020  str) -> str:.   
-00012a90: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012aa0: 2047 656e 6572 6174 6520 6120 636f 6d6d   Generate a comm
-00012ab0: 616e 6420 7374 7269 6e67 2066 6f72 207a  and string for z
-00012ac0: 6970 7069 6e67 2074 6865 2064 6174 6120  ipping the data 
-00012ad0: 6f6e 2053 6c75 726d 2e0a 0a20 2020 2020  on Slurm...     
-00012ae0: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00012af0: 2020 2020 2064 6174 615f 6c6f 6361 7469       data_locati
-00012b00: 6f6e 2028 7374 7229 3a20 5468 6520 666f  on (str): The fo
-00012b10: 6c64 6572 2074 6f20 6265 207a 6970 7065  lder to be zippe
-00012b20: 642e 0a20 2020 2020 2020 2020 2020 2066  d..            f
-00012b30: 696c 656e 616d 6520 2873 7472 293a 2054  ilename (str): T
-00012b40: 6865 206e 616d 6520 6f66 2074 6865 207a  he name of the z
-00012b50: 6970 2061 7263 6869 7665 2066 696c 6520  ip archive file 
-00012b60: 746f 2065 7874 7261 6374 2e0a 2020 2020  to extract..    
-00012b70: 2020 2020 2020 2020 2020 2020 5769 7468              With
-00012b80: 6f75 7420 6578 7465 6e73 696f 6e2e 0a0a  out extension...
-00012b90: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
-00012ba0: 0a20 2020 2020 2020 2020 2020 2073 7472  .            str
-00012bb0: 3a20 5468 6520 636f 6d6d 616e 6420 746f  : The command to
-00012bc0: 2063 7265 6174 6520 7468 6520 7a69 7020   create the zip 
-00012bd0: 6669 6c65 2e0a 2020 2020 2020 2020 2222  file..        ""
-00012be0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
-00012bf0: 2073 656c 662e 5f5a 4950 5f43 4d44 2e66   self._ZIP_CMD.f
-00012c00: 6f72 6d61 7428 6669 6c65 6e61 6d65 3d66  ormat(filename=f
-00012c10: 696c 656e 616d 652c 0a20 2020 2020 2020  ilename,.       
+000127a0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000127b0: 202d 3e20 5265 7375 6c74 3a0a 2020 2020   -> Result:.    
+000127c0: 2020 2020 2222 225a 6970 2074 6865 206f      """Zip the o
+000127d0: 7574 7075 7420 666f 6c64 6572 206f 6620  utput folder of 
+000127e0: 6120 6a6f 6220 6f6e 2053 6c75 726d 0a0a  a job on Slurm..
+000127f0: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00012800: 2020 2020 2020 2020 2020 6461 7461 5f6c            data_l
+00012810: 6f63 6174 696f 6e20 2853 7472 696e 6729  ocation (String)
+00012820: 3a20 466f 6c64 6572 206f 6e20 534c 5552  : Folder on SLUR
+00012830: 4d20 7769 7468 2074 6865 2022 6461 7461  M with the "data
+00012840: 2f6f 7574 220a 2020 2020 2020 2020 2020  /out".          
+00012850: 2020 2020 2020 7375 6266 6f6c 6465 722e        subfolder.
+00012860: 0a20 2020 2020 2020 2020 2020 2066 696c  .            fil
+00012870: 656e 616d 6520 2853 7472 696e 6729 3a20  ename (String): 
+00012880: 4e61 6d65 2074 6f20 6769 7665 2074 6f20  Name to give to 
+00012890: 7468 6520 7a69 7066 696c 652e 0a20 2020  the zipfile..   
+000128a0: 2020 2020 2020 2020 2065 6e76 2028 4469           env (Di
+000128b0: 6374 5b73 7472 2c20 7374 725d 2c20 6f70  ct[str, str], op
+000128c0: 7469 6f6e 616c 293a 204f 7074 696f 6e61  tional): Optiona
+000128d0: 6c20 656e 7669 726f 6e6d 656e 7420 7661  l environment va
+000128e0: 7269 6162 6c65 7320 746f 200a 2020 2020  riables to .    
+000128f0: 2020 2020 2020 2020 2020 2020 7365 7420              set 
+00012900: 7768 656e 2072 756e 6e69 6e67 2074 6865  when running the
+00012910: 2063 6f6d 6d61 6e64 2e20 4465 6661 756c   command. Defaul
+00012920: 7473 2074 6f20 4e6f 6e65 2e0a 0a20 2020  ts to None...   
+00012930: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00012940: 2020 2020 2020 2020 2020 5265 7375 6c74            Result
+00012950: 3a20 5468 6520 7265 7375 6c74 206f 6620  : The result of 
+00012960: 7468 6520 7a69 7020 6174 7465 6d70 742e  the zip attempt.
+00012970: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00012980: 2020 2020 2023 207a 6970 0a20 2020 2020       # zip.     
+00012990: 2020 207a 6970 5f63 6d64 203d 2073 656c     zip_cmd = sel
+000129a0: 662e 6765 745f 7a69 705f 636f 6d6d 616e  f.get_zip_comman
+000129b0: 6428 6461 7461 5f6c 6f63 6174 696f 6e2c  d(data_location,
+000129c0: 2066 696c 656e 616d 6529 0a20 2020 2020   filename).     
+000129d0: 2020 206c 6f67 6765 722e 696e 666f 2866     logger.info(f
+000129e0: 225a 6970 7069 6e67 207b 6461 7461 5f6c  "Zipping {data_l
+000129f0: 6f63 6174 696f 6e7d 2061 7320 7b66 696c  ocation} as {fil
+00012a00: 656e 616d 657d 206f 6e20 536c 7572 6d22  ename} on Slurm"
+00012a10: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00012a20: 2073 656c 662e 7275 6e5f 636f 6d6d 616e   self.run_comman
+00012a30: 6473 285b 7a69 705f 636d 645d 2c20 656e  ds([zip_cmd], en
+00012a40: 763d 656e 7629 0a0a 2020 2020 6465 6620  v=env)..    def 
+00012a50: 6765 745f 7a69 705f 636f 6d6d 616e 6428  get_zip_command(
+00012a60: 7365 6c66 2c20 6461 7461 5f6c 6f63 6174  self, data_locat
+00012a70: 696f 6e3a 2073 7472 2c20 6669 6c65 6e61  ion: str, filena
+00012a80: 6d65 3a20 7374 7229 202d 3e20 7374 723a  me: str) -> str:
+00012a90: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00012aa0: 2020 2020 2047 656e 6572 6174 6520 6120       Generate a 
+00012ab0: 636f 6d6d 616e 6420 7374 7269 6e67 2066  command string f
+00012ac0: 6f72 207a 6970 7069 6e67 2074 6865 2064  or zipping the d
+00012ad0: 6174 6120 6f6e 2053 6c75 726d 2e0a 0a20  ata on Slurm... 
+00012ae0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+00012af0: 2020 2020 2020 2020 2064 6174 615f 6c6f           data_lo
+00012b00: 6361 7469 6f6e 2028 7374 7229 3a20 5468  cation (str): Th
+00012b10: 6520 666f 6c64 6572 2074 6f20 6265 207a  e folder to be z
+00012b20: 6970 7065 642e 0a20 2020 2020 2020 2020  ipped..         
+00012b30: 2020 2066 696c 656e 616d 6520 2873 7472     filename (str
+00012b40: 293a 2054 6865 206e 616d 6520 6f66 2074  ): The name of t
+00012b50: 6865 207a 6970 2061 7263 6869 7665 2066  he zip archive f
+00012b60: 696c 6520 746f 2065 7874 7261 6374 2e0a  ile to extract..
+00012b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012b80: 5769 7468 6f75 7420 6578 7465 6e73 696f  Without extensio
+00012b90: 6e2e 0a0a 2020 2020 2020 2020 5265 7475  n...        Retu
+00012ba0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00012bb0: 2073 7472 3a20 5468 6520 636f 6d6d 616e   str: The comman
+00012bc0: 6420 746f 2063 7265 6174 6520 7468 6520  d to create the 
+00012bd0: 7a69 7020 6669 6c65 2e0a 2020 2020 2020  zip file..      
+00012be0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+00012bf0: 7475 726e 2073 656c 662e 5f5a 4950 5f43  turn self._ZIP_C
+00012c00: 4d44 2e66 6f72 6d61 7428 6669 6c65 6e61  MD.format(filena
+00012c10: 6d65 3d66 696c 656e 616d 652c 0a20 2020  me=filename,.   
 00012c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c30: 2020 2020 2020 2020 2020 2020 2064 6174               dat
-00012c40: 615f 6c6f 6361 7469 6f6e 3d64 6174 615f  a_location=data_
-00012c50: 6c6f 6361 7469 6f6e 290a 0a20 2020 2064  location)..    d
-00012c60: 6566 2067 6574 5f6c 6f67 6669 6c65 5f66  ef get_logfile_f
-00012c70: 726f 6d5f 736c 7572 6d28 7365 6c66 2c0a  rom_slurm(self,.
-00012c80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012c90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00012ca0: 6c75 726d 5f6a 6f62 5f69 643a 2073 7472  lurm_job_id: str
-00012cb0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00012c30: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012c40: 2064 6174 615f 6c6f 6361 7469 6f6e 3d64   data_location=d
+00012c50: 6174 615f 6c6f 6361 7469 6f6e 290a 0a20  ata_location).. 
+00012c60: 2020 2064 6566 2067 6574 5f6c 6f67 6669     def get_logfi
+00012c70: 6c65 5f66 726f 6d5f 736c 7572 6d28 7365  le_from_slurm(se
+00012c80: 6c66 2c0a 2020 2020 2020 2020 2020 2020  lf,.            
+00012c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00012ca0: 2020 2073 6c75 726d 5f6a 6f62 5f69 643a     slurm_job_id:
+00012cb0: 2073 7472 2c0a 2020 2020 2020 2020 2020   str,.          
 00012cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012cd0: 206c 6f63 616c 5f74 6d70 5f73 746f 7261   local_tmp_stora
-00012ce0: 6765 3a20 7374 7220 3d20 222f 746d 702f  ge: str = "/tmp/
-00012cf0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+00012cd0: 2020 2020 206c 6f63 616c 5f74 6d70 5f73       local_tmp_s
+00012ce0: 746f 7261 6765 3a20 7374 7220 3d20 222f  torage: str = "/
+00012cf0: 746d 702f 222c 0a20 2020 2020 2020 2020  tmp/",.         
 00012d00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d10: 2020 6c6f 6766 696c 653a 2073 7472 203d    logfile: str =
-00012d20: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+00012d10: 2020 2020 2020 6c6f 6766 696c 653a 2073        logfile: s
+00012d20: 7472 203d 204e 6f6e 650a 2020 2020 2020  tr = None.      
 00012d30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012d40: 2020 2020 2029 202d 3e20 5475 706c 655b       ) -> Tuple[
-00012d50: 7374 722c 2073 7472 2c20 5472 616e 7366  str, str, Transf
-00012d60: 6572 5265 7375 6c74 5d3a 0a20 2020 2020  erResult]:.     
-00012d70: 2020 2022 2222 436f 7079 2074 6865 206c     """Copy the l
-00012d80: 6f67 6669 6c65 206f 6620 7468 6520 6769  ogfile of the gi
-00012d90: 7665 6e20 534c 5552 4d20 6a6f 6220 746f  ven SLURM job to
-00012da0: 2074 6865 206c 6f63 616c 2073 6572 7665   the local serve
-00012db0: 722e 0a0a 2020 2020 2020 2020 4e6f 7465  r...        Note
-00012dc0: 2061 626f 7574 2028 5472 616e 7366 6572   about (Transfer
-00012dd0: 2952 6573 756c 743a 0a0a 2020 2020 2020  )Result:..      
-00012de0: 2020 556e 6c69 6b65 2073 696d 696c 6172    Unlike similar
-00012df0: 2063 6c61 7373 6573 2073 7563 6820 6173   classes such as
-00012e00: 2069 6e76 6f6b 652e 7275 6e6e 6572 732e   invoke.runners.
-00012e10: 5265 7375 6c74 0a20 2020 2020 2020 206f  Result.        o
-00012e20: 7220 6661 6272 6963 2e72 756e 6e65 7273  r fabric.runners
-00012e30: 2e52 6573 756c 740a 2020 2020 2020 2020  .Result.        
-00012e40: 2877 6869 6368 2068 6176 6520 6120 636f  (which have a co
-00012e50: 6e63 6570 7420 6f66 20e2 809c 7761 726e  ncept of ...warn
-00012e60: 2061 6e64 2072 6574 7572 6e20 616e 7977   and return anyw
-00012e70: 6179 7320 6f6e 2066 6169 6c75 7265 e280  ays on failure..
-00012e80: 9d29 0a20 2020 2020 2020 2074 6869 7320  .).        this 
-00012e90: 636c 6173 7320 6861 7320 6e6f 2075 7365  class has no use
-00012ea0: 6675 6c20 7472 7574 6869 6e65 7373 2062  ful truthiness b
-00012eb0: 6568 6176 696f 722e 0a20 2020 2020 2020  ehavior..       
-00012ec0: 2049 6620 6120 6669 6c65 2074 7261 6e73   If a file trans
-00012ed0: 6665 7220 6661 696c 732c 2073 6f6d 6520  fer fails, some 
-00012ee0: 6578 6365 7074 696f 6e20 7769 6c6c 2062  exception will b
-00012ef0: 6520 7261 6973 6564 2c0a 2020 2020 2020  e raised,.      
-00012f00: 2020 6569 7468 6572 2061 6e20 4f53 4572    either an OSEr
-00012f10: 726f 7220 6f72 2061 6e20 6572 726f 7220  ror or an error 
-00012f20: 6672 6f6d 2077 6974 6869 6e20 5061 7261  from within Para
-00012f30: 6d69 6b6f 2e0a 0a20 2020 2020 2020 2041  miko...        A
-00012f40: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00012f50: 2073 6c75 726d 5f6a 6f62 5f69 6420 2873   slurm_job_id (s
-00012f60: 7472 293a 2054 6865 2049 4420 6f66 2074  tr): The ID of t
-00012f70: 6865 2053 4c55 524d 206a 6f62 2e0a 2020  he SLURM job..  
-00012f80: 2020 2020 2020 2020 2020 6c6f 6361 6c5f            local_
-00012f90: 746d 705f 7374 6f72 6167 6520 2873 7472  tmp_storage (str
-00012fa0: 2c20 6f70 7469 6f6e 616c 293a 2050 6174  , optional): Pat
-00012fb0: 6820 746f 2073 746f 7265 2074 6865 206c  h to store the l
-00012fc0: 6f67 6669 6c65 200a 2020 2020 2020 2020  ogfile .        
-00012fd0: 2020 2020 2020 2020 6c6f 6361 6c6c 792e          locally.
-00012fe0: 2044 6566 6175 6c74 7320 746f 2022 2f74   Defaults to "/t
-00012ff0: 6d70 2f22 2e0a 2020 2020 2020 2020 2020  mp/"..          
-00013000: 2020 6c6f 6766 696c 6520 2873 7472 2c20    logfile (str, 
-00013010: 6f70 7469 6f6e 616c 293a 2050 6174 6820  optional): Path 
-00013020: 746f 2074 6865 206c 6f67 6669 6c65 206f  to the logfile o
-00013030: 6e20 7468 6520 534c 5552 4d20 7365 7276  n the SLURM serv
-00013040: 6572 2e0a 2020 2020 2020 2020 2020 2020  er..            
-00013050: 2020 2020 4465 6661 756c 7473 2074 6f20      Defaults to 
-00013060: 4e6f 6e65 2e0a 0a20 2020 2020 2020 2052  None...        R
-00013070: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00013080: 2020 2020 5475 706c 653a 2064 6972 6563      Tuple: direc
-00013090: 746f 7279 2c20 6675 6c6c 2070 6174 6820  tory, full path 
-000130a0: 6f66 2074 6865 206c 6f67 6669 6c65 2c20  of the logfile, 
-000130b0: 616e 6420 5472 616e 7366 6572 5265 7375  and TransferResu
-000130c0: 6c74 0a20 2020 2020 2020 2022 2222 0a20  lt.        """. 
-000130d0: 2020 2020 2020 2069 6620 6c6f 6766 696c         if logfil
-000130e0: 6520 6973 204e 6f6e 653a 0a20 2020 2020  e is None:.     
-000130f0: 2020 2020 2020 206c 6f67 6669 6c65 203d         logfile =
-00013100: 2073 656c 662e 5f4c 4f47 4649 4c45 0a20   self._LOGFILE. 
-00013110: 2020 2020 2020 206c 6f67 6669 6c65 203d         logfile =
-00013120: 206c 6f67 6669 6c65 2e66 6f72 6d61 7428   logfile.format(
-00013130: 736c 7572 6d5f 6a6f 625f 6964 3d73 6c75  slurm_job_id=slu
-00013140: 726d 5f6a 6f62 5f69 6429 0a20 2020 2020  rm_job_id).     
-00013150: 2020 206c 6f67 6765 722e 696e 666f 2866     logger.info(f
-00013160: 2243 6f70 7969 6e67 206c 6f67 6669 6c65  "Copying logfile
-00013170: 207b 6c6f 6766 696c 657d 2066 726f 6d20   {logfile} from 
-00013180: 536c 7572 6d5c 0a20 2020 2020 2020 2020  Slurm\.         
-00013190: 2020 2074 6f20 7b6c 6f63 616c 5f74 6d70     to {local_tmp
-000131a0: 5f73 746f 7261 6765 7d22 290a 2020 2020  _storage}").    
-000131b0: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
-000131c0: 662e 6765 7428 0a20 2020 2020 2020 2020  f.get(.         
-000131d0: 2020 2072 656d 6f74 653d 6c6f 6766 696c     remote=logfil
-000131e0: 652c 0a20 2020 2020 2020 2020 2020 206c  e,.            l
-000131f0: 6f63 616c 3d6c 6f63 616c 5f74 6d70 5f73  ocal=local_tmp_s
-00013200: 746f 7261 6765 290a 2020 2020 2020 2020  torage).        
-00013210: 6578 706f 7274 5f66 696c 6520 3d20 6c6f  export_file = lo
-00013220: 6361 6c5f 746d 705f 7374 6f72 6167 652b  cal_tmp_storage+
-00013230: 6c6f 6766 696c 650a 2020 2020 2020 2020  logfile.        
-00013240: 7265 7475 726e 206c 6f63 616c 5f74 6d70  return local_tmp
-00013250: 5f73 746f 7261 6765 2c20 6578 706f 7274  _storage, export
-00013260: 5f66 696c 652c 2072 6573 756c 740a 0a20  _file, result.. 
-00013270: 2020 2064 6566 2067 6574 5f75 6e7a 6970     def get_unzip
-00013280: 5f63 6f6d 6d61 6e64 2873 656c 662c 207a  _command(self, z
-00013290: 6970 6669 6c65 3a20 7374 722c 0a20 2020  ipfile: str,.   
-000132a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000132b0: 2020 2020 2020 2066 696c 7465 725f 6669         filter_fi
-000132c0: 6c65 7479 7065 733a 2073 7472 203d 2022  letypes: str = "
-000132d0: 2a2e 7a61 7272 202a 2e74 6966 6620 2a2e  *.zarr *.tiff *.
-000132e0: 7469 6622 0a20 2020 2020 2020 2020 2020  tif".           
-000132f0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-00013300: 202d 3e20 7374 723a 0a20 2020 2020 2020   -> str:.       
-00013310: 2022 2222 0a20 2020 2020 2020 2047 656e   """.        Gen
-00013320: 6572 6174 6520 6120 636f 6d6d 616e 6420  erate a command 
-00013330: 7374 7269 6e67 2066 6f72 2075 6e7a 6970  string for unzip
-00013340: 7069 6e67 2061 2064 6174 6120 6172 6368  ping a data arch
-00013350: 6976 6520 616e 6420 6372 6561 7469 6e67  ive and creating
-00013360: 0a20 2020 2020 2020 2072 6571 7569 7265  .        require
-00013370: 6420 6469 7265 6374 6f72 6965 7320 666f  d directories fo
-00013380: 7220 536c 7572 6d20 6a6f 6273 2e0a 0a20  r Slurm jobs... 
-00013390: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-000133a0: 2020 2020 2020 2020 207a 6970 6669 6c65           zipfile
-000133b0: 2028 7374 7229 3a20 5468 6520 6e61 6d65   (str): The name
-000133c0: 206f 6620 7468 6520 7a69 7020 6172 6368   of the zip arch
-000133d0: 6976 6520 6669 6c65 2074 6f20 6578 7472  ive file to extr
-000133e0: 6163 742e 0a20 2020 2020 2020 2020 2020  act..           
-000133f0: 2020 2020 2057 6974 686f 7574 2065 7874       Without ext
-00013400: 656e 7369 6f6e 2e0a 2020 2020 2020 2020  ension..        
-00013410: 2020 2020 6669 6c74 6572 5f66 696c 6574      filter_filet
-00013420: 7970 6573 2028 7374 722c 206f 7074 696f  ypes (str, optio
-00013430: 6e61 6c29 3a20 4120 7370 6163 652d 7365  nal): A space-se
-00013440: 7061 7261 7465 6420 7374 7269 6e67 0a20  parated string. 
-00013450: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00013460: 6f6e 7461 696e 696e 6720 7468 6520 6669  ontaining the fi
-00013470: 6c65 2065 7874 656e 7369 6f6e 7320 746f  le extensions to
-00013480: 2065 7874 7261 6374 2066 726f 6d20 7468   extract from th
-00013490: 6520 7a69 7020 6669 6c65 2e0a 2020 2020  e zip file..    
-000134a0: 2020 2020 2020 2020 2020 2020 452e 672e              E.g.
-000134b0: 2064 6566 6175 6c74 7320 746f 2022 2a2e   defaults to "*.
-000134c0: 7a61 7272 202a 2e74 6966 6620 2a2e 7469  zarr *.tiff *.ti
-000134d0: 6622 2e0a 2020 2020 2020 2020 2020 2020  f"..            
-000134e0: 2020 2020 5365 7474 696e 6720 7468 6973      Setting this
-000134f0: 2061 7267 756d 656e 7420 746f 2060 4e6f   argument to `No
-00013500: 6e65 6020 7769 6c6c 206f 6d69 7420 7468  ne` will omit th
-00013510: 6520 6669 6c65 0a20 2020 2020 2020 2020  e file.         
-00013520: 2020 2020 2020 2066 696c 7465 7220 616e         filter an
-00013530: 6420 6578 7472 6163 7420 616c 6c20 6669  d extract all fi
-00013540: 6c65 732e 0a0a 2020 2020 2020 2020 5265  les...        Re
-00013550: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00013560: 2020 2073 7472 3a0a 2020 2020 2020 2020     str:.        
-00013570: 2020 2020 2020 2020 5468 6520 636f 6d6d          The comm
-00013580: 616e 6420 746f 2065 7874 7261 6374 2074  and to extract t
-00013590: 6865 2073 7065 6369 6669 6564 0a20 2020  he specified.   
-000135a0: 2020 2020 2020 2020 2020 2020 2066 696c               fil
-000135b0: 6574 7970 6573 2066 726f 6d20 7468 6520  etypes from the 
-000135c0: 7a69 7020 6669 6c65 2e0a 2020 2020 2020  zip file..      
-000135d0: 2020 2222 220a 2020 2020 2020 2020 756e    """.        un
-000135e0: 7a69 705f 636d 6420 3d20 6622 6d6b 6469  zip_cmd = f"mkdi
-000135f0: 7220 5c22 7b73 656c 662e 736c 7572 6d5f  r \"{self.slurm_
-00013600: 6461 7461 5f70 6174 687d 2f7b 7a69 7066  data_path}/{zipf
-00013610: 696c 657d 5c22 205c 0a20 2020 2020 2020  ile}\" \.       
-00013620: 2020 2020 2020 2020 2020 2020 205c 227b               \"{
-00013630: 7365 6c66 2e73 6c75 726d 5f64 6174 615f  self.slurm_data_
-00013640: 7061 7468 7d2f 7b7a 6970 6669 6c65 7d2f  path}/{zipfile}/
-00013650: 6461 7461 5c22 205c 0a20 2020 2020 2020  data\" \.       
-00013660: 2020 2020 2020 2020 2020 2020 205c 227b               \"{
-00013670: 7365 6c66 2e73 6c75 726d 5f64 6174 615f  self.slurm_data_
-00013680: 7061 7468 7d2f 7b7a 6970 6669 6c65 7d2f  path}/{zipfile}/
-00013690: 6461 7461 2f69 6e5c 2220 5c0a 2020 2020  data/in\" \.    
+00012d40: 2020 2020 2020 2020 2029 202d 3e20 5475           ) -> Tu
+00012d50: 706c 655b 7374 722c 2073 7472 2c20 5472  ple[str, str, Tr
+00012d60: 616e 7366 6572 5265 7375 6c74 5d3a 0a20  ansferResult]:. 
+00012d70: 2020 2020 2020 2022 2222 436f 7079 2074         """Copy t
+00012d80: 6865 206c 6f67 6669 6c65 206f 6620 7468  he logfile of th
+00012d90: 6520 6769 7665 6e20 534c 5552 4d20 6a6f  e given SLURM jo
+00012da0: 6220 746f 2074 6865 206c 6f63 616c 2073  b to the local s
+00012db0: 6572 7665 722e 0a0a 2020 2020 2020 2020  erver...        
+00012dc0: 4e6f 7465 2061 626f 7574 2028 5472 616e  Note about (Tran
+00012dd0: 7366 6572 2952 6573 756c 743a 0a0a 2020  sfer)Result:..  
+00012de0: 2020 2020 2020 556e 6c69 6b65 2073 696d        Unlike sim
+00012df0: 696c 6172 2063 6c61 7373 6573 2073 7563  ilar classes suc
+00012e00: 6820 6173 2069 6e76 6f6b 652e 7275 6e6e  h as invoke.runn
+00012e10: 6572 732e 5265 7375 6c74 0a20 2020 2020  ers.Result.     
+00012e20: 2020 206f 7220 6661 6272 6963 2e72 756e     or fabric.run
+00012e30: 6e65 7273 2e52 6573 756c 740a 2020 2020  ners.Result.    
+00012e40: 2020 2020 2877 6869 6368 2068 6176 6520      (which have 
+00012e50: 6120 636f 6e63 6570 7420 6f66 20e2 809c  a concept of ...
+00012e60: 7761 726e 2061 6e64 2072 6574 7572 6e20  warn and return 
+00012e70: 616e 7977 6179 7320 6f6e 2066 6169 6c75  anyways on failu
+00012e80: 7265 e280 9d29 0a20 2020 2020 2020 2074  re...).        t
+00012e90: 6869 7320 636c 6173 7320 6861 7320 6e6f  his class has no
+00012ea0: 2075 7365 6675 6c20 7472 7574 6869 6e65   useful truthine
+00012eb0: 7373 2062 6568 6176 696f 722e 0a20 2020  ss behavior..   
+00012ec0: 2020 2020 2049 6620 6120 6669 6c65 2074       If a file t
+00012ed0: 7261 6e73 6665 7220 6661 696c 732c 2073  ransfer fails, s
+00012ee0: 6f6d 6520 6578 6365 7074 696f 6e20 7769  ome exception wi
+00012ef0: 6c6c 2062 6520 7261 6973 6564 2c0a 2020  ll be raised,.  
+00012f00: 2020 2020 2020 6569 7468 6572 2061 6e20        either an 
+00012f10: 4f53 4572 726f 7220 6f72 2061 6e20 6572  OSError or an er
+00012f20: 726f 7220 6672 6f6d 2077 6974 6869 6e20  ror from within 
+00012f30: 5061 7261 6d69 6b6f 2e0a 0a20 2020 2020  Paramiko...     
+00012f40: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00012f50: 2020 2020 2073 6c75 726d 5f6a 6f62 5f69       slurm_job_i
+00012f60: 6420 2873 7472 293a 2054 6865 2049 4420  d (str): The ID 
+00012f70: 6f66 2074 6865 2053 4c55 524d 206a 6f62  of the SLURM job
+00012f80: 2e0a 2020 2020 2020 2020 2020 2020 6c6f  ..            lo
+00012f90: 6361 6c5f 746d 705f 7374 6f72 6167 6520  cal_tmp_storage 
+00012fa0: 2873 7472 2c20 6f70 7469 6f6e 616c 293a  (str, optional):
+00012fb0: 2050 6174 6820 746f 2073 746f 7265 2074   Path to store t
+00012fc0: 6865 206c 6f67 6669 6c65 200a 2020 2020  he logfile .    
+00012fd0: 2020 2020 2020 2020 2020 2020 6c6f 6361              loca
+00012fe0: 6c6c 792e 2044 6566 6175 6c74 7320 746f  lly. Defaults to
+00012ff0: 2022 2f74 6d70 2f22 2e0a 2020 2020 2020   "/tmp/"..      
+00013000: 2020 2020 2020 6c6f 6766 696c 6520 2873        logfile (s
+00013010: 7472 2c20 6f70 7469 6f6e 616c 293a 2050  tr, optional): P
+00013020: 6174 6820 746f 2074 6865 206c 6f67 6669  ath to the logfi
+00013030: 6c65 206f 6e20 7468 6520 534c 5552 4d20  le on the SLURM 
+00013040: 7365 7276 6572 2e0a 2020 2020 2020 2020  server..        
+00013050: 2020 2020 2020 2020 4465 6661 756c 7473          Defaults
+00013060: 2074 6f20 4e6f 6e65 2e0a 0a20 2020 2020   to None...     
+00013070: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00013080: 2020 2020 2020 2020 5475 706c 653a 2064          Tuple: d
+00013090: 6972 6563 746f 7279 2c20 6675 6c6c 2070  irectory, full p
+000130a0: 6174 6820 6f66 2074 6865 206c 6f67 6669  ath of the logfi
+000130b0: 6c65 2c20 616e 6420 5472 616e 7366 6572  le, and Transfer
+000130c0: 5265 7375 6c74 0a20 2020 2020 2020 2022  Result.        "
+000130d0: 2222 0a20 2020 2020 2020 2069 6620 6c6f  "".        if lo
+000130e0: 6766 696c 6520 6973 204e 6f6e 653a 0a20  gfile is None:. 
+000130f0: 2020 2020 2020 2020 2020 206c 6f67 6669             logfi
+00013100: 6c65 203d 2073 656c 662e 5f4c 4f47 4649  le = self._LOGFI
+00013110: 4c45 0a20 2020 2020 2020 206c 6f67 6669  LE.        logfi
+00013120: 6c65 203d 206c 6f67 6669 6c65 2e66 6f72  le = logfile.for
+00013130: 6d61 7428 736c 7572 6d5f 6a6f 625f 6964  mat(slurm_job_id
+00013140: 3d73 6c75 726d 5f6a 6f62 5f69 6429 0a20  =slurm_job_id). 
+00013150: 2020 2020 2020 206c 6f67 6765 722e 696e         logger.in
+00013160: 666f 2866 2243 6f70 7969 6e67 206c 6f67  fo(f"Copying log
+00013170: 6669 6c65 207b 6c6f 6766 696c 657d 2066  file {logfile} f
+00013180: 726f 6d20 536c 7572 6d5c 0a20 2020 2020  rom Slurm\.     
+00013190: 2020 2020 2020 2074 6f20 7b6c 6f63 616c         to {local
+000131a0: 5f74 6d70 5f73 746f 7261 6765 7d22 290a  _tmp_storage}").
+000131b0: 2020 2020 2020 2020 7265 7375 6c74 203d          result =
+000131c0: 2073 656c 662e 6765 7428 0a20 2020 2020   self.get(.     
+000131d0: 2020 2020 2020 2072 656d 6f74 653d 6c6f         remote=lo
+000131e0: 6766 696c 652c 0a20 2020 2020 2020 2020  gfile,.         
+000131f0: 2020 206c 6f63 616c 3d6c 6f63 616c 5f74     local=local_t
+00013200: 6d70 5f73 746f 7261 6765 290a 2020 2020  mp_storage).    
+00013210: 2020 2020 6578 706f 7274 5f66 696c 6520      export_file 
+00013220: 3d20 6c6f 6361 6c5f 746d 705f 7374 6f72  = local_tmp_stor
+00013230: 6167 652b 6c6f 6766 696c 650a 2020 2020  age+logfile.    
+00013240: 2020 2020 7265 7475 726e 206c 6f63 616c      return local
+00013250: 5f74 6d70 5f73 746f 7261 6765 2c20 6578  _tmp_storage, ex
+00013260: 706f 7274 5f66 696c 652c 2072 6573 756c  port_file, resul
+00013270: 740a 0a20 2020 2064 6566 2067 6574 5f75  t..    def get_u
+00013280: 6e7a 6970 5f63 6f6d 6d61 6e64 2873 656c  nzip_command(sel
+00013290: 662c 207a 6970 6669 6c65 3a20 7374 722c  f, zipfile: str,
+000132a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000132b0: 2020 2020 2020 2020 2020 2066 696c 7465             filte
+000132c0: 725f 6669 6c65 7479 7065 733a 2073 7472  r_filetypes: str
+000132d0: 203d 2022 2a2e 7a61 7272 202a 2e74 6966   = "*.zarr *.tif
+000132e0: 6620 2a2e 7469 6622 0a20 2020 2020 2020  f *.tif".       
+000132f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013300: 2020 2029 202d 3e20 7374 723a 0a20 2020     ) -> str:.   
+00013310: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00013320: 2047 656e 6572 6174 6520 6120 636f 6d6d   Generate a comm
+00013330: 616e 6420 7374 7269 6e67 2066 6f72 2075  and string for u
+00013340: 6e7a 6970 7069 6e67 2061 2064 6174 6120  nzipping a data 
+00013350: 6172 6368 6976 6520 616e 6420 6372 6561  archive and crea
+00013360: 7469 6e67 0a20 2020 2020 2020 2072 6571  ting.        req
+00013370: 7569 7265 6420 6469 7265 6374 6f72 6965  uired directorie
+00013380: 7320 666f 7220 536c 7572 6d20 6a6f 6273  s for Slurm jobs
+00013390: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+000133a0: 0a20 2020 2020 2020 2020 2020 207a 6970  .            zip
+000133b0: 6669 6c65 2028 7374 7229 3a20 5468 6520  file (str): The 
+000133c0: 6e61 6d65 206f 6620 7468 6520 7a69 7020  name of the zip 
+000133d0: 6172 6368 6976 6520 6669 6c65 2074 6f20  archive file to 
+000133e0: 6578 7472 6163 742e 0a20 2020 2020 2020  extract..       
+000133f0: 2020 2020 2020 2020 2057 6974 686f 7574           Without
+00013400: 2065 7874 656e 7369 6f6e 2e0a 2020 2020   extension..    
+00013410: 2020 2020 2020 2020 6669 6c74 6572 5f66          filter_f
+00013420: 696c 6574 7970 6573 2028 7374 722c 206f  iletypes (str, o
+00013430: 7074 696f 6e61 6c29 3a20 4120 7370 6163  ptional): A spac
+00013440: 652d 7365 7061 7261 7465 6420 7374 7269  e-separated stri
+00013450: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
+00013460: 2020 2063 6f6e 7461 696e 696e 6720 7468     containing th
+00013470: 6520 6669 6c65 2065 7874 656e 7369 6f6e  e file extension
+00013480: 7320 746f 2065 7874 7261 6374 2066 726f  s to extract fro
+00013490: 6d20 7468 6520 7a69 7020 6669 6c65 2e0a  m the zip file..
+000134a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000134b0: 452e 672e 2064 6566 6175 6c74 7320 746f  E.g. defaults to
+000134c0: 2022 2a2e 7a61 7272 202a 2e74 6966 6620   "*.zarr *.tiff 
+000134d0: 2a2e 7469 6622 2e0a 2020 2020 2020 2020  *.tif"..        
+000134e0: 2020 2020 2020 2020 5365 7474 696e 6720          Setting 
+000134f0: 7468 6973 2061 7267 756d 656e 7420 746f  this argument to
+00013500: 2060 4e6f 6e65 6020 7769 6c6c 206f 6d69   `None` will omi
+00013510: 7420 7468 6520 6669 6c65 0a20 2020 2020  t the file.     
+00013520: 2020 2020 2020 2020 2020 2066 696c 7465             filte
+00013530: 7220 616e 6420 6578 7472 6163 7420 616c  r and extract al
+00013540: 6c20 6669 6c65 732e 0a0a 2020 2020 2020  l files...      
+00013550: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00013560: 2020 2020 2020 2073 7472 3a0a 2020 2020         str:.    
+00013570: 2020 2020 2020 2020 2020 2020 5468 6520              The 
+00013580: 636f 6d6d 616e 6420 746f 2065 7874 7261  command to extra
+00013590: 6374 2074 6865 2073 7065 6369 6669 6564  ct the specified
+000135a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000135b0: 2066 696c 6574 7970 6573 2066 726f 6d20   filetypes from 
+000135c0: 7468 6520 7a69 7020 6669 6c65 2e0a 2020  the zip file..  
+000135d0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000135e0: 2020 756e 7a69 705f 636d 6420 3d20 6622    unzip_cmd = f"
+000135f0: 6d6b 6469 7220 5c22 7b73 656c 662e 736c  mkdir \"{self.sl
+00013600: 7572 6d5f 6461 7461 5f70 6174 687d 2f7b  urm_data_path}/{
+00013610: 7a69 7066 696c 657d 5c22 205c 0a20 2020  zipfile}\" \.   
+00013620: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013630: 205c 227b 7365 6c66 2e73 6c75 726d 5f64   \"{self.slurm_d
+00013640: 6174 615f 7061 7468 7d2f 7b7a 6970 6669  ata_path}/{zipfi
+00013650: 6c65 7d2f 6461 7461 5c22 205c 0a20 2020  le}/data\" \.   
+00013660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013670: 205c 227b 7365 6c66 2e73 6c75 726d 5f64   \"{self.slurm_d
+00013680: 6174 615f 7061 7468 7d2f 7b7a 6970 6669  ata_path}/{zipfi
+00013690: 6c65 7d2f 6461 7461 2f69 6e5c 2220 5c0a  le}/data/in\" \.
 000136a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000136b0: 5c22 7b73 656c 662e 736c 7572 6d5f 6461  \"{self.slurm_da
-000136c0: 7461 5f70 6174 687d 2f7b 7a69 7066 696c  ta_path}/{zipfil
-000136d0: 657d 2f64 6174 612f 6f75 745c 2220 5c0a  e}/data/out\" \.
-000136e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000136f0: 2020 2020 5c22 7b73 656c 662e 736c 7572      \"{self.slur
-00013700: 6d5f 6461 7461 5f70 6174 687d 2f7b 7a69  m_data_path}/{zi
-00013710: 7066 696c 657d 2f64 6174 612f 6774 5c22  pfile}/data/gt\"
-00013720: 3b20 5c0a 2020 2020 2020 2020 2020 2020  ; \.            
-00013730: 2020 2020 2020 2020 377a 2078 202d 7920          7z x -y 
-00013740: 2d6f 5c22 7b73 656c 662e 736c 7572 6d5f  -o\"{self.slurm_
-00013750: 6461 7461 5f70 6174 687d 2f7b 7a69 7066  data_path}/{zipf
-00013760: 696c 657d 2f64 6174 612f 696e 5c22 205c  ile}/data/in\" \
-00013770: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013780: 2020 2020 205c 227b 7365 6c66 2e73 6c75       \"{self.slu
-00013790: 726d 5f64 6174 615f 7061 7468 7d2f 7b7a  rm_data_path}/{z
-000137a0: 6970 6669 6c65 7d2e 7a69 705c 2220 7b66  ipfile}.zip\" {f
-000137b0: 696c 7465 725f 6669 6c65 7479 7065 737d  ilter_filetypes}
-000137c0: 220a 0a20 2020 2020 2020 2072 6574 7572  "..        retur
-000137d0: 6e20 756e 7a69 705f 636d 640a 0a20 2020  n unzip_cmd..   
-000137e0: 2064 6566 2067 6574 5f69 6d61 6765 5f76   def get_image_v
-000137f0: 6572 7369 6f6e 735f 616e 645f 6461 7461  ersions_and_data
-00013800: 5f66 696c 6573 2873 656c 662c 206d 6f64  _files(self, mod
-00013810: 656c 3a20 7374 720a 2020 2020 2020 2020  el: str.        
+000136b0: 2020 2020 5c22 7b73 656c 662e 736c 7572      \"{self.slur
+000136c0: 6d5f 6461 7461 5f70 6174 687d 2f7b 7a69  m_data_path}/{zi
+000136d0: 7066 696c 657d 2f64 6174 612f 6f75 745c  pfile}/data/out\
+000136e0: 2220 5c0a 2020 2020 2020 2020 2020 2020  " \.            
+000136f0: 2020 2020 2020 2020 5c22 7b73 656c 662e          \"{self.
+00013700: 736c 7572 6d5f 6461 7461 5f70 6174 687d  slurm_data_path}
+00013710: 2f7b 7a69 7066 696c 657d 2f64 6174 612f  /{zipfile}/data/
+00013720: 6774 5c22 3b20 5c0a 2020 2020 2020 2020  gt\"; \.        
+00013730: 2020 2020 2020 2020 2020 2020 377a 2078              7z x
+00013740: 202d 7920 2d6f 5c22 7b73 656c 662e 736c   -y -o\"{self.sl
+00013750: 7572 6d5f 6461 7461 5f70 6174 687d 2f7b  urm_data_path}/{
+00013760: 7a69 7066 696c 657d 2f64 6174 612f 696e  zipfile}/data/in
+00013770: 5c22 205c 0a20 2020 2020 2020 2020 2020  \" \.           
+00013780: 2020 2020 2020 2020 205c 227b 7365 6c66           \"{self
+00013790: 2e73 6c75 726d 5f64 6174 615f 7061 7468  .slurm_data_path
+000137a0: 7d2f 7b7a 6970 6669 6c65 7d2e 7a69 705c  }/{zipfile}.zip\
+000137b0: 2220 7b66 696c 7465 725f 6669 6c65 7479  " {filter_filety
+000137c0: 7065 737d 220a 0a20 2020 2020 2020 2072  pes}"..        r
+000137d0: 6574 7572 6e20 756e 7a69 705f 636d 640a  eturn unzip_cmd.
+000137e0: 0a20 2020 2064 6566 2067 6574 5f69 6d61  .    def get_ima
+000137f0: 6765 5f76 6572 7369 6f6e 735f 616e 645f  ge_versions_and_
+00013800: 6461 7461 5f66 696c 6573 2873 656c 662c  data_files(self,
+00013810: 206d 6f64 656c 3a20 7374 720a 2020 2020   model: str.    
 00013820: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013840: 2020 2920 2d3e 2054 7570 6c65 5b4c 6973    ) -> Tuple[Lis
-00013850: 745b 7374 725d 2c20 4c69 7374 5b73 7472  t[str], List[str
-00013860: 5d5d 3a0a 2020 2020 2020 2020 2222 220a  ]]:.        """.
-00013870: 2020 2020 2020 2020 5265 7472 6965 7665          Retrieve
-00013880: 2074 6865 2061 7661 696c 6162 6c65 2069   the available i
-00013890: 6d61 6765 2076 6572 7369 6f6e 7320 616e  mage versions an
-000138a0: 6420 696e 7075 7420 6461 7461 2066 696c  d input data fil
-000138b0: 6573 2066 6f72 2061 0a20 2020 2020 2020  es for a.       
-000138c0: 2067 6976 656e 206d 6f64 656c 2e0a 0a20   given model... 
-000138d0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-000138e0: 2020 2020 2020 2020 206d 6f64 656c 2028           model (
-000138f0: 7374 7229 3a20 5468 6520 6e61 6d65 206f  str): The name o
-00013900: 6620 7468 6520 6d6f 6465 6c20 746f 2071  f the model to q
-00013910: 7565 7279 2066 6f72 2e0a 0a20 2020 2020  uery for...     
-00013920: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00013930: 2020 2020 2020 2020 5475 706c 655b 4c69          Tuple[Li
-00013940: 7374 5b73 7472 5d2c 204c 6973 745b 7374  st[str], List[st
-00013950: 725d 5d3a 0a20 2020 2020 2020 2020 2020  r]]:.           
-00013960: 2020 2020 2041 2074 7570 6c65 2063 6f6e       A tuple con
-00013970: 7461 696e 696e 6720 7477 6f20 6c69 7374  taining two list
-00013980: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00013990: 2020 202d 2054 6865 2066 6972 7374 206c     - The first l
-000139a0: 6973 7420 696e 636c 7564 6573 2074 6865  ist includes the
-000139b0: 2061 7661 696c 6162 6c65 2069 6d61 6765   available image
-000139c0: 2076 6572 7369 6f6e 732c 200a 2020 2020   versions, .    
+00013840: 2020 2020 2020 2920 2d3e 2054 7570 6c65        ) -> Tuple
+00013850: 5b4c 6973 745b 7374 725d 2c20 4c69 7374  [List[str], List
+00013860: 5b73 7472 5d5d 3a0a 2020 2020 2020 2020  [str]]:.        
+00013870: 2222 220a 2020 2020 2020 2020 5265 7472  """.        Retr
+00013880: 6965 7665 2074 6865 2061 7661 696c 6162  ieve the availab
+00013890: 6c65 2069 6d61 6765 2076 6572 7369 6f6e  le image version
+000138a0: 7320 616e 6420 696e 7075 7420 6461 7461  s and input data
+000138b0: 2066 696c 6573 2066 6f72 2061 0a20 2020   files for a.   
+000138c0: 2020 2020 2067 6976 656e 206d 6f64 656c       given model
+000138d0: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+000138e0: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
+000138f0: 656c 2028 7374 7229 3a20 5468 6520 6e61  el (str): The na
+00013900: 6d65 206f 6620 7468 6520 6d6f 6465 6c20  me of the model 
+00013910: 746f 2071 7565 7279 2066 6f72 2e0a 0a20  to query for... 
+00013920: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00013930: 2020 2020 2020 2020 2020 2020 5475 706c              Tupl
+00013940: 655b 4c69 7374 5b73 7472 5d2c 204c 6973  e[List[str], Lis
+00013950: 745b 7374 725d 5d3a 0a20 2020 2020 2020  t[str]]:.       
+00013960: 2020 2020 2020 2020 2041 2074 7570 6c65           A tuple
+00013970: 2063 6f6e 7461 696e 696e 6720 7477 6f20   containing two 
+00013980: 6c69 7374 733a 0a20 2020 2020 2020 2020  lists:.         
+00013990: 2020 2020 2020 202d 2054 6865 2066 6972         - The fir
+000139a0: 7374 206c 6973 7420 696e 636c 7564 6573  st list includes
+000139b0: 2074 6865 2061 7661 696c 6162 6c65 2069   the available i
+000139c0: 6d61 6765 2076 6572 7369 6f6e 732c 200a  mage versions, .
 000139d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139e0: 736f 7274 6564 2069 6e20 6465 7363 656e  sorted in descen
-000139f0: 6469 6e67 206f 7264 6572 2e0a 2020 2020  ding order..    
-00013a00: 2020 2020 2020 2020 2020 2020 2d20 5468              - Th
-00013a10: 6520 7365 636f 6e64 206c 6973 7420 696e  e second list in
-00013a20: 636c 7564 6573 2074 6865 2061 7661 696c  cludes the avail
-00013a30: 6162 6c65 2064 6174 6120 6669 6c65 732e  able data files.
-00013a40: 0a0a 2020 2020 2020 2020 5261 6973 6573  ..        Raises
-00013a50: 3a0a 2020 2020 2020 2020 2020 2020 5661  :.            Va
-00013a60: 6c75 6545 7272 6f72 3a20 4966 2074 6865  lueError: If the
-00013a70: 2070 726f 7669 6465 6420 6d6f 6465 6c20   provided model 
-00013a80: 6973 206e 6f74 2066 6f75 6e64 2069 6e20  is not found in 
-00013a90: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
-00013aa0: 2020 2020 536c 7572 6d43 6c69 656e 7427      SlurmClient'
-00013ab0: 7320 6b6e 6f77 6e20 6d6f 6465 6c20 7061  s known model pa
-00013ac0: 7468 732e 0a20 2020 2020 2020 2022 2222  ths..        """
-00013ad0: 0a20 2020 2020 2020 2069 6d61 6765 5f70  .        image_p
-00013ae0: 6174 6820 3d20 7365 6c66 2e73 6c75 726d  ath = self.slurm
-00013af0: 5f6d 6f64 656c 5f70 6174 6873 2e67 6574  _model_paths.get
-00013b00: 286d 6f64 656c 290a 2020 2020 2020 2020  (model).        
-00013b10: 6966 206e 6f74 2069 6d61 6765 5f70 6174  if not image_pat
-00013b20: 683a 0a20 2020 2020 2020 2020 2020 2072  h:.            r
-00013b30: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
-00013b40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013b50: 2066 224e 6f20 7061 7468 206b 6e6f 776e   f"No path known
-00013b60: 2066 6f72 2070 726f 7669 6465 6420 6d6f   for provided mo
-00013b70: 6465 6c20 7b6d 6f64 656c 7d2c 205c 0a20  del {model}, \. 
-00013b80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013b90: 2020 2069 6e20 7b73 656c 662e 736c 7572     in {self.slur
-00013ba0: 6d5f 6d6f 6465 6c5f 7061 7468 737d 2229  m_model_paths}")
-00013bb0: 0a20 2020 2020 2020 2063 6d64 6c69 7374  .        cmdlist
-00013bc0: 203d 205b 0a20 2020 2020 2020 2020 2020   = [.           
-00013bd0: 2073 656c 662e 5f56 4552 5349 4f4e 5f43   self._VERSION_C
-00013be0: 4d44 2e66 6f72 6d61 7428 736c 7572 6d5f  MD.format(slurm_
-00013bf0: 696d 6167 6573 5f70 6174 683d 7365 6c66  images_path=self
-00013c00: 2e73 6c75 726d 5f69 6d61 6765 735f 7061  .slurm_images_pa
-00013c10: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
+000139e0: 2020 2020 736f 7274 6564 2069 6e20 6465      sorted in de
+000139f0: 7363 656e 6469 6e67 206f 7264 6572 2e0a  scending order..
+00013a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013a10: 2d20 5468 6520 7365 636f 6e64 206c 6973  - The second lis
+00013a20: 7420 696e 636c 7564 6573 2074 6865 2061  t includes the a
+00013a30: 7661 696c 6162 6c65 2064 6174 6120 6669  vailable data fi
+00013a40: 6c65 732e 0a0a 2020 2020 2020 2020 5261  les...        Ra
+00013a50: 6973 6573 3a0a 2020 2020 2020 2020 2020  ises:.          
+00013a60: 2020 5661 6c75 6545 7272 6f72 3a20 4966    ValueError: If
+00013a70: 2074 6865 2070 726f 7669 6465 6420 6d6f   the provided mo
+00013a80: 6465 6c20 6973 206e 6f74 2066 6f75 6e64  del is not found
+00013a90: 2069 6e20 7468 650a 2020 2020 2020 2020   in the.        
+00013aa0: 2020 2020 2020 2020 536c 7572 6d43 6c69          SlurmCli
+00013ab0: 656e 7427 7320 6b6e 6f77 6e20 6d6f 6465  ent's known mode
+00013ac0: 6c20 7061 7468 732e 0a20 2020 2020 2020  l paths..       
+00013ad0: 2022 2222 0a20 2020 2020 2020 2069 6d61   """.        ima
+00013ae0: 6765 5f70 6174 6820 3d20 7365 6c66 2e73  ge_path = self.s
+00013af0: 6c75 726d 5f6d 6f64 656c 5f70 6174 6873  lurm_model_paths
+00013b00: 2e67 6574 286d 6f64 656c 290a 2020 2020  .get(model).    
+00013b10: 2020 2020 6966 206e 6f74 2069 6d61 6765      if not image
+00013b20: 5f70 6174 683a 0a20 2020 2020 2020 2020  _path:.         
+00013b30: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
+00013b40: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
+00013b50: 2020 2020 2066 224e 6f20 7061 7468 206b       f"No path k
+00013b60: 6e6f 776e 2066 6f72 2070 726f 7669 6465  nown for provide
+00013b70: 6420 6d6f 6465 6c20 7b6d 6f64 656c 7d2c  d model {model},
+00013b80: 205c 0a20 2020 2020 2020 2020 2020 2020   \.             
+00013b90: 2020 2020 2020 2069 6e20 7b73 656c 662e         in {self.
+00013ba0: 736c 7572 6d5f 6d6f 6465 6c5f 7061 7468  slurm_model_path
+00013bb0: 737d 2229 0a20 2020 2020 2020 2063 6d64  s}").        cmd
+00013bc0: 6c69 7374 203d 205b 0a20 2020 2020 2020  list = [.       
+00013bd0: 2020 2020 2073 656c 662e 5f56 4552 5349       self._VERSI
+00013be0: 4f4e 5f43 4d44 2e66 6f72 6d61 7428 736c  ON_CMD.format(sl
+00013bf0: 7572 6d5f 696d 6167 6573 5f70 6174 683d  urm_images_path=
+00013c00: 7365 6c66 2e73 6c75 726d 5f69 6d61 6765  self.slurm_image
+00013c10: 735f 7061 7468 2c0a 2020 2020 2020 2020  s_path,.        
 00013c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013c30: 2020 2020 2020 2020 2069 6d61 6765 5f70           image_p
-00013c40: 6174 683d 696d 6167 655f 7061 7468 292c  ath=image_path),
-00013c50: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-00013c60: 662e 5f44 4154 415f 434d 442e 666f 726d  f._DATA_CMD.form
-00013c70: 6174 2873 6c75 726d 5f64 6174 615f 7061  at(slurm_data_pa
-00013c80: 7468 3d73 656c 662e 736c 7572 6d5f 6461  th=self.slurm_da
-00013c90: 7461 5f70 6174 6829 5d0a 2020 2020 2020  ta_path)].      
-00013ca0: 2020 2320 7370 6c69 7420 7265 7370 6f6e    # split respon
-00013cb0: 7365 7320 7065 7220 636f 6d6d 616e 640a  ses per command.
-00013cc0: 2020 2020 2020 2020 7265 7370 6f6e 7365          response
-00013cd0: 5f6c 6973 7420 3d20 7365 6c66 2e72 756e  _list = self.run
-00013ce0: 5f63 6f6d 6d61 6e64 735f 7370 6c69 745f  _commands_split_
-00013cf0: 6f75 7428 636d 646c 6973 7429 0a20 2020  out(cmdlist).   
-00013d00: 2020 2020 2023 2073 706c 6974 206c 696e       # split lin
-00013d10: 6573 2066 7572 7468 6572 2069 6e74 6f20  es further into 
-00013d20: 7375 626c 6973 7473 0a20 2020 2020 2020  sublists.       
-00013d30: 2072 6573 706f 6e73 655f 6c69 7374 203d   response_list =
-00013d40: 205b 7265 7370 6f6e 7365 2e73 7472 6970   [response.strip
-00013d50: 2829 2e73 706c 6974 2827 5c6e 2729 0a20  ().split('\n'). 
-00013d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013d70: 2020 2020 2020 2020 666f 7220 7265 7370          for resp
-00013d80: 6f6e 7365 2069 6e20 7265 7370 6f6e 7365  onse in response
-00013d90: 5f6c 6973 745d 0a20 2020 2020 2020 2072  _list].        r
-00013da0: 6573 706f 6e73 655f 6c69 7374 5b30 5d20  esponse_list[0] 
-00013db0: 3d20 736f 7274 6564 2872 6573 706f 6e73  = sorted(respons
-00013dc0: 655f 6c69 7374 5b30 5d2c 2072 6576 6572  e_list[0], rever
-00013dd0: 7365 3d54 7275 6529 0a20 2020 2020 2020  se=True).       
-00013de0: 2072 6574 7572 6e20 7265 7370 6f6e 7365   return response
-00013df0: 5f6c 6973 745b 305d 2c20 7265 7370 6f6e  _list[0], respon
-00013e00: 7365 5f6c 6973 745b 315d 0a0a 2020 2020  se_list[1]..    
-00013e10: 6465 6620 6765 745f 616c 6c5f 696d 6167  def get_all_imag
-00013e20: 655f 7665 7273 696f 6e73 5f61 6e64 5f64  e_versions_and_d
-00013e30: 6174 615f 6669 6c65 7328 7365 6c66 0a20  ata_files(self. 
-00013e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013c30: 2020 2020 2020 2020 2020 2020 2069 6d61               ima
+00013c40: 6765 5f70 6174 683d 696d 6167 655f 7061  ge_path=image_pa
+00013c50: 7468 292c 0a20 2020 2020 2020 2020 2020  th),.           
+00013c60: 2073 656c 662e 5f44 4154 415f 434d 442e   self._DATA_CMD.
+00013c70: 666f 726d 6174 2873 6c75 726d 5f64 6174  format(slurm_dat
+00013c80: 615f 7061 7468 3d73 656c 662e 736c 7572  a_path=self.slur
+00013c90: 6d5f 6461 7461 5f70 6174 6829 5d0a 2020  m_data_path)].  
+00013ca0: 2020 2020 2020 2320 7370 6c69 7420 7265        # split re
+00013cb0: 7370 6f6e 7365 7320 7065 7220 636f 6d6d  sponses per comm
+00013cc0: 616e 640a 2020 2020 2020 2020 7265 7370  and.        resp
+00013cd0: 6f6e 7365 5f6c 6973 7420 3d20 7365 6c66  onse_list = self
+00013ce0: 2e72 756e 5f63 6f6d 6d61 6e64 735f 7370  .run_commands_sp
+00013cf0: 6c69 745f 6f75 7428 636d 646c 6973 7429  lit_out(cmdlist)
+00013d00: 0a20 2020 2020 2020 2023 2073 706c 6974  .        # split
+00013d10: 206c 696e 6573 2066 7572 7468 6572 2069   lines further i
+00013d20: 6e74 6f20 7375 626c 6973 7473 0a20 2020  nto sublists.   
+00013d30: 2020 2020 2072 6573 706f 6e73 655f 6c69       response_li
+00013d40: 7374 203d 205b 7265 7370 6f6e 7365 2e73  st = [response.s
+00013d50: 7472 6970 2829 2e73 706c 6974 2827 5c6e  trip().split('\n
+00013d60: 2729 0a20 2020 2020 2020 2020 2020 2020  ').             
+00013d70: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00013d80: 7265 7370 6f6e 7365 2069 6e20 7265 7370  response in resp
+00013d90: 6f6e 7365 5f6c 6973 745d 0a20 2020 2020  onse_list].     
+00013da0: 2020 2072 6573 706f 6e73 655f 6c69 7374     response_list
+00013db0: 5b30 5d20 3d20 736f 7274 6564 2872 6573  [0] = sorted(res
+00013dc0: 706f 6e73 655f 6c69 7374 5b30 5d2c 2072  ponse_list[0], r
+00013dd0: 6576 6572 7365 3d54 7275 6529 0a20 2020  everse=True).   
+00013de0: 2020 2020 2072 6574 7572 6e20 7265 7370       return resp
+00013df0: 6f6e 7365 5f6c 6973 745b 305d 2c20 7265  onse_list[0], re
+00013e00: 7370 6f6e 7365 5f6c 6973 745b 315d 0a0a  sponse_list[1]..
+00013e10: 2020 2020 6465 6620 6765 745f 616c 6c5f      def get_all_
+00013e20: 696d 6167 655f 7665 7273 696f 6e73 5f61  image_versions_a
+00013e30: 6e64 5f64 6174 615f 6669 6c65 7328 7365  nd_data_files(se
+00013e40: 6c66 0a20 2020 2020 2020 2020 2020 2020  lf.             
 00013e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e60: 2020 2020 2020 2020 2020 2020 2029 202d               ) -
-00013e70: 3e20 5475 706c 655b 4469 6374 5b73 7472  > Tuple[Dict[str
-00013e80: 2c20 4c69 7374 5b73 7472 5d5d 2c0a 2020  , List[str]],.  
-00013e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013e70: 2029 202d 3e20 5475 706c 655b 4469 6374   ) -> Tuple[Dict
+00013e80: 5b73 7472 2c20 4c69 7374 5b73 7472 5d5d  [str, List[str]]
+00013e90: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
 00013ea0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00013eb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013ec0: 2020 2020 2020 204c 6973 745b 7374 725d         List[str]
-00013ed0: 5d3a 0a20 2020 2020 2020 2022 2222 5265  ]:.        """Re
-00013ee0: 7472 6965 7665 2061 6c6c 2061 7661 696c  trieve all avail
-00013ef0: 6162 6c65 2069 6d61 6765 2076 6572 7369  able image versi
-00013f00: 6f6e 7320 616e 6420 6461 7461 2066 696c  ons and data fil
-00013f10: 6573 2066 726f 6d0a 2020 2020 2020 2020  es from.        
-00013f20: 7468 6520 536c 7572 6d20 636c 7573 7465  the Slurm cluste
-00013f30: 722e 0a0a 2020 2020 2020 2020 5265 7475  r...        Retu
-00013f40: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00013f50: 5475 706c 655b 4469 6374 5b73 7472 2c20  Tuple[Dict[str, 
-00013f60: 4c69 7374 5b73 7472 5d5d 2c20 4c69 7374  List[str]], List
-00013f70: 5b73 7472 5d5d 3a0a 2020 2020 2020 2020  [str]]:.        
-00013f80: 2020 2020 2020 2020 4120 7475 706c 6520          A tuple 
-00013f90: 636f 6e74 6169 6e69 6e67 3a0a 2020 2020  containing:.    
-00013fa0: 2020 2020 2020 2020 2020 2020 2d20 4120              - A 
-00013fb0: 6469 6374 696f 6e61 7279 206d 6170 7069  dictionary mappi
-00013fc0: 6e67 206d 6f64 656c 7320 746f 2061 7661  ng models to ava
-00013fd0: 696c 6162 6c65 2076 6572 7369 6f6e 732e  ilable versions.
-00013fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013ff0: 202d 2041 206c 6973 7420 6f66 2061 7661   - A list of ava
-00014000: 696c 6162 6c65 2069 6e70 7574 2064 6174  ilable input dat
-00014010: 6120 666f 6c64 6572 732e 0a20 2020 2020  a folders..     
-00014020: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-00014030: 6573 756c 7464 6963 7420 3d20 7b7d 0a20  esultdict = {}. 
-00014040: 2020 2020 2020 2063 6d64 6c69 7374 203d         cmdlist =
-00014050: 205b 5d0a 0a20 2020 2020 2020 2066 6f72   []..        for
-00014060: 2070 6174 6820 696e 2073 656c 662e 736c   path in self.sl
-00014070: 7572 6d5f 6d6f 6465 6c5f 7061 7468 732e  urm_model_paths.
-00014080: 7661 6c75 6573 2829 3a0a 2020 2020 2020  values():.      
-00014090: 2020 2020 2020 7061 7468 636d 6420 3d20        pathcmd = 
-000140a0: 7365 6c66 2e5f 5645 5253 494f 4e5f 434d  self._VERSION_CM
-000140b0: 442e 666f 726d 6174 280a 2020 2020 2020  D.format(.      
-000140c0: 2020 2020 2020 2020 2020 736c 7572 6d5f            slurm_
-000140d0: 696d 6167 6573 5f70 6174 683d 7365 6c66  images_path=self
-000140e0: 2e73 6c75 726d 5f69 6d61 6765 735f 7061  .slurm_images_pa
-000140f0: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
-00014100: 2020 2020 696d 6167 655f 7061 7468 3d70      image_path=p
-00014110: 6174 6829 0a20 2020 2020 2020 2020 2020  ath).           
-00014120: 2063 6d64 6c69 7374 2e61 7070 656e 6428   cmdlist.append(
-00014130: 7061 7468 636d 6429 0a0a 2020 2020 2020  pathcmd)..      
-00014140: 2020 2320 4164 6420 6461 7461 2070 6174    # Add data pat
-00014150: 6820 746f 6f0a 2020 2020 2020 2020 636d  h too.        cm
-00014160: 646c 6973 742e 6170 7065 6e64 2873 656c  dlist.append(sel
-00014170: 662e 5f44 4154 415f 434d 442e 666f 726d  f._DATA_CMD.form
-00014180: 6174 280a 2020 2020 2020 2020 2020 2020  at(.            
-00014190: 736c 7572 6d5f 6461 7461 5f70 6174 683d  slurm_data_path=
-000141a0: 7365 6c66 2e73 6c75 726d 5f64 6174 615f  self.slurm_data_
-000141b0: 7061 7468 2929 0a0a 2020 2020 2020 2020  path))..        
-000141c0: 2320 5370 6c69 7420 7265 7370 6f6e 7365  # Split response
-000141d0: 7320 7065 7220 636f 6d6d 616e 640a 2020  s per command.  
-000141e0: 2020 2020 2020 7265 7370 6f6e 7365 5f6c        response_l
-000141f0: 6973 7420 3d20 7365 6c66 2e72 756e 5f63  ist = self.run_c
-00014200: 6f6d 6d61 6e64 735f 7370 6c69 745f 6f75  ommands_split_ou
-00014210: 7428 636d 646c 6973 7429 0a0a 2020 2020  t(cmdlist)..    
-00014220: 2020 2020 2320 5370 6c69 7420 6c69 6e65      # Split line
-00014230: 7320 6675 7274 6865 7220 696e 746f 2073  s further into s
-00014240: 7562 6c69 7374 730a 2020 2020 2020 2020  ublists.        
-00014250: 7265 7370 6f6e 7365 5f6c 6973 7420 3d20  response_list = 
-00014260: 5b72 6573 706f 6e73 652e 7374 7269 7028  [response.strip(
-00014270: 292e 7370 6c69 7428 275c 6e27 290a 2020  ).split('\n').  
-00014280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014290: 2020 2020 2020 2066 6f72 2072 6573 706f         for respo
-000142a0: 6e73 6520 696e 2072 6573 706f 6e73 655f  nse in response_
-000142b0: 6c69 7374 5d0a 0a20 2020 2020 2020 2066  list]..        f
-000142c0: 6f72 2069 2c20 6b20 696e 2065 6e75 6d65  or i, k in enume
-000142d0: 7261 7465 2873 656c 662e 736c 7572 6d5f  rate(self.slurm_
-000142e0: 6d6f 6465 6c5f 7061 7468 7329 3a0a 2020  model_paths):.  
-000142f0: 2020 2020 2020 2020 2020 2320 5265 7475            # Retu
-00014300: 726e 2068 6967 6865 7374 2076 6572 7369  rn highest versi
-00014310: 6f6e 2066 6972 7374 0a20 2020 2020 2020  on first.       
-00014320: 2020 2020 2072 6573 756c 7464 6963 745b       resultdict[
-00014330: 6b5d 203d 2073 6f72 7465 6428 7265 7370  k] = sorted(resp
-00014340: 6f6e 7365 5f6c 6973 745b 695d 2c20 7265  onse_list[i], re
-00014350: 7665 7273 653d 5472 7565 290a 0a20 2020  verse=True)..   
-00014360: 2020 2020 2072 6574 7572 6e20 7265 7375       return resu
-00014370: 6c74 6469 6374 2c20 7265 7370 6f6e 7365  ltdict, response
-00014380: 5f6c 6973 745b 2d31 5d0a                 _list[-1].
+00013ec0: 2020 2020 2020 2020 2020 204c 6973 745b             List[
+00013ed0: 7374 725d 5d3a 0a20 2020 2020 2020 2022  str]]:.        "
+00013ee0: 2222 5265 7472 6965 7665 2061 6c6c 2061  ""Retrieve all a
+00013ef0: 7661 696c 6162 6c65 2069 6d61 6765 2076  vailable image v
+00013f00: 6572 7369 6f6e 7320 616e 6420 6461 7461  ersions and data
+00013f10: 2066 696c 6573 2066 726f 6d0a 2020 2020   files from.    
+00013f20: 2020 2020 7468 6520 536c 7572 6d20 636c      the Slurm cl
+00013f30: 7573 7465 722e 0a0a 2020 2020 2020 2020  uster...        
+00013f40: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00013f50: 2020 2020 5475 706c 655b 4469 6374 5b73      Tuple[Dict[s
+00013f60: 7472 2c20 4c69 7374 5b73 7472 5d5d 2c20  tr, List[str]], 
+00013f70: 4c69 7374 5b73 7472 5d5d 3a0a 2020 2020  List[str]]:.    
+00013f80: 2020 2020 2020 2020 2020 2020 4120 7475              A tu
+00013f90: 706c 6520 636f 6e74 6169 6e69 6e67 3a0a  ple containing:.
+00013fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013fb0: 2d20 4120 6469 6374 696f 6e61 7279 206d  - A dictionary m
+00013fc0: 6170 7069 6e67 206d 6f64 656c 7320 746f  apping models to
+00013fd0: 2061 7661 696c 6162 6c65 2076 6572 7369   available versi
+00013fe0: 6f6e 732e 0a20 2020 2020 2020 2020 2020  ons..           
+00013ff0: 2020 2020 202d 2041 206c 6973 7420 6f66       - A list of
+00014000: 2061 7661 696c 6162 6c65 2069 6e70 7574   available input
+00014010: 2064 6174 6120 666f 6c64 6572 732e 0a20   data folders.. 
+00014020: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00014030: 2020 2072 6573 756c 7464 6963 7420 3d20     resultdict = 
+00014040: 7b7d 0a20 2020 2020 2020 2063 6d64 6c69  {}.        cmdli
+00014050: 7374 203d 205b 5d0a 0a20 2020 2020 2020  st = []..       
+00014060: 2066 6f72 2070 6174 6820 696e 2073 656c   for path in sel
+00014070: 662e 736c 7572 6d5f 6d6f 6465 6c5f 7061  f.slurm_model_pa
+00014080: 7468 732e 7661 6c75 6573 2829 3a0a 2020  ths.values():.  
+00014090: 2020 2020 2020 2020 2020 7061 7468 636d            pathcm
+000140a0: 6420 3d20 7365 6c66 2e5f 5645 5253 494f  d = self._VERSIO
+000140b0: 4e5f 434d 442e 666f 726d 6174 280a 2020  N_CMD.format(.  
+000140c0: 2020 2020 2020 2020 2020 2020 2020 736c                sl
+000140d0: 7572 6d5f 696d 6167 6573 5f70 6174 683d  urm_images_path=
+000140e0: 7365 6c66 2e73 6c75 726d 5f69 6d61 6765  self.slurm_image
+000140f0: 735f 7061 7468 2c0a 2020 2020 2020 2020  s_path,.        
+00014100: 2020 2020 2020 2020 696d 6167 655f 7061          image_pa
+00014110: 7468 3d70 6174 6829 0a20 2020 2020 2020  th=path).       
+00014120: 2020 2020 2063 6d64 6c69 7374 2e61 7070       cmdlist.app
+00014130: 656e 6428 7061 7468 636d 6429 0a0a 2020  end(pathcmd)..  
+00014140: 2020 2020 2020 2320 4164 6420 6461 7461        # Add data
+00014150: 2070 6174 6820 746f 6f0a 2020 2020 2020   path too.      
+00014160: 2020 636d 646c 6973 742e 6170 7065 6e64    cmdlist.append
+00014170: 2873 656c 662e 5f44 4154 415f 434d 442e  (self._DATA_CMD.
+00014180: 666f 726d 6174 280a 2020 2020 2020 2020  format(.        
+00014190: 2020 2020 736c 7572 6d5f 6461 7461 5f70      slurm_data_p
+000141a0: 6174 683d 7365 6c66 2e73 6c75 726d 5f64  ath=self.slurm_d
+000141b0: 6174 615f 7061 7468 2929 0a0a 2020 2020  ata_path))..    
+000141c0: 2020 2020 2320 5370 6c69 7420 7265 7370      # Split resp
+000141d0: 6f6e 7365 7320 7065 7220 636f 6d6d 616e  onses per comman
+000141e0: 640a 2020 2020 2020 2020 7265 7370 6f6e  d.        respon
+000141f0: 7365 5f6c 6973 7420 3d20 7365 6c66 2e72  se_list = self.r
+00014200: 756e 5f63 6f6d 6d61 6e64 735f 7370 6c69  un_commands_spli
+00014210: 745f 6f75 7428 636d 646c 6973 7429 0a0a  t_out(cmdlist)..
+00014220: 2020 2020 2020 2020 2320 5370 6c69 7420          # Split 
+00014230: 6c69 6e65 7320 6675 7274 6865 7220 696e  lines further in
+00014240: 746f 2073 7562 6c69 7374 730a 2020 2020  to sublists.    
+00014250: 2020 2020 7265 7370 6f6e 7365 5f6c 6973      response_lis
+00014260: 7420 3d20 5b72 6573 706f 6e73 652e 7374  t = [response.st
+00014270: 7269 7028 292e 7370 6c69 7428 275c 6e27  rip().split('\n'
+00014280: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00014290: 2020 2020 2020 2020 2020 2066 6f72 2072             for r
+000142a0: 6573 706f 6e73 6520 696e 2072 6573 706f  esponse in respo
+000142b0: 6e73 655f 6c69 7374 5d0a 0a20 2020 2020  nse_list]..     
+000142c0: 2020 2066 6f72 2069 2c20 6b20 696e 2065     for i, k in e
+000142d0: 6e75 6d65 7261 7465 2873 656c 662e 736c  numerate(self.sl
+000142e0: 7572 6d5f 6d6f 6465 6c5f 7061 7468 7329  urm_model_paths)
+000142f0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+00014300: 5265 7475 726e 2068 6967 6865 7374 2076  Return highest v
+00014310: 6572 7369 6f6e 2066 6972 7374 0a20 2020  ersion first.   
+00014320: 2020 2020 2020 2020 2072 6573 756c 7464           resultd
+00014330: 6963 745b 6b5d 203d 2073 6f72 7465 6428  ict[k] = sorted(
+00014340: 7265 7370 6f6e 7365 5f6c 6973 745b 695d  response_list[i]
+00014350: 2c20 7265 7665 7273 653d 5472 7565 290a  , reverse=True).
+00014360: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00014370: 7265 7375 6c74 6469 6374 2c20 7265 7370  resultdict, resp
+00014380: 6f6e 7365 5f6c 6973 745b 2d31 5d0a       onse_list[-1].
```

### Comparing `biomero-1.9.0/biomero.egg-info/PKG-INFO` & `biomero-1.9.1/biomero.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biomero
-Version: 1.9.0
+Version: 1.9.1
 Summary: A python library for easy connecting between OMERO (jobs) and a Slurm cluster
 Author: Core Facility - Cellular Imaging
 Author-email: Torec Luik <t.t.luik@amsterdamumc.nl>, cellularimaging@amsterdamumc.nl
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `biomero-1.9.0/biomero.egg-info/SOURCES.txt` & `biomero-1.9.1/biomero.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 biomero/slurm_client.py
 biomero.egg-info/PKG-INFO
 biomero.egg-info/SOURCES.txt
 biomero.egg-info/dependency_links.txt
 biomero.egg-info/requires.txt
 biomero.egg-info/top_level.txt
 docs/Makefile
+docs/biomero.rst
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/modules.rst
-docs/omero_slurm_client.rst
 docs/readme_link.md
 docs/requirements.txt
 docs/tutorial_link.md
 resources/__init__.py
 resources/convert_job_array.sh
 resources/convert_zarr_to_tiff.def
 resources/convert_zarr_to_tiff.py
```

### Comparing `biomero-1.9.0/docs/Makefile` & `biomero-1.9.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/docs/conf.py` & `biomero-1.9.1/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 sys.path.append(os.path.abspath('../..'))
 sys.path.append(os.path.abspath('../biomero'))
 sys.path.append(os.path.abspath('..'))
 
 # -- Project information -----------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#project-information
 
-project = 'Omero Slurm Client'
+project = 'BIOMERO'
 copyright = '2023, T.T.Luik'
 author = 'T.T.Luik'
 release = dynamicversion('biomero')
 
 # -- General configuration ---------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#general-configuration
```

### Comparing `biomero-1.9.0/docs/index.rst` & `biomero-1.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/docs/make.bat` & `biomero-1.9.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/pyproject.toml` & `biomero-1.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/resources/convert_job_array.sh` & `biomero-1.9.1/resources/convert_job_array.sh`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/resources/convert_zarr_to_tiff.py` & `biomero-1.9.1/resources/convert_zarr_to_tiff.py`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/resources/job_template.sh` & `biomero-1.9.1/resources/job_template.sh`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/resources/slurm-config.ini` & `biomero-1.9.1/resources/slurm-config.ini`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/resources/tutorials/images/Cells.tif` & `biomero-1.9.1/resources/tutorials/images/Cells.tif`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/resources/tutorials/images/cellexpansion.png` & `biomero-1.9.1/resources/tutorials/images/cellexpansion.png`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/resources/tutorials/images/gc_allow_ssh.PNG` & `biomero-1.9.1/resources/tutorials/images/gc_allow_ssh.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/resources/tutorials/images/nuclei_labels.png` & `biomero-1.9.1/resources/tutorials/images/nuclei_labels.png`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/resources/tutorials/images/webclient_init_env.PNG` & `biomero-1.9.1/resources/tutorials/images/webclient_init_env.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/resources/tutorials/images/webclient_init_env_done.PNG` & `biomero-1.9.1/resources/tutorials/images/webclient_init_env_done.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/resources/tutorials/images/webclient_run_cellpose.PNG` & `biomero-1.9.1/resources/tutorials/images/webclient_run_cellpose.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/resources/tutorials/images/webclient_run_workflow.PNG` & `biomero-1.9.1/resources/tutorials/images/webclient_run_workflow.PNG`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/resources/tutorials/tutorial_Azure_slurm.md` & `biomero-1.9.1/resources/tutorials/tutorial_Azure_slurm.md`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/resources/tutorials/tutorial_GoogleCloud_slurm.md` & `biomero-1.9.1/resources/tutorials/tutorial_GoogleCloud_slurm.md`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/resources/tutorials/tutorial_cellexpansion.md` & `biomero-1.9.1/resources/tutorials/tutorial_cellexpansion.md`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/resources/tutorials/tutorial_cellprofiler.md` & `biomero-1.9.1/resources/tutorials/tutorial_cellprofiler.md`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/resources/tutorials/tutorial_local_slurm.md` & `biomero-1.9.1/resources/tutorials/tutorial_local_slurm.md`

 * *Files identical despite different names*

### Comparing `biomero-1.9.0/tests/unit/test_slurm_client.py` & `biomero-1.9.1/tests/unit/test_slurm_client.py`

 * *Files identical despite different names*

