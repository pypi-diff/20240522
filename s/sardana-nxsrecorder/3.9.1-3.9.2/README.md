# Comparing `tmp/sardana-nxsrecorder-3.9.1.tar.gz` & `tmp/sardana-nxsrecorder-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sardana-nxsrecorder-3.9.1.tar", last modified: Wed Oct 19 06:03:26 2022, max compression
+gzip compressed data, was "dist/sardana-nxsrecorder-3.9.2.tar", last modified: Wed Oct 19 09:39:13 2022, max compression
```

## Comparing `sardana-nxsrecorder-3.9.1.tar` & `sardana-nxsrecorder-3.9.2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/
-drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/.ci/
-drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/.ci/debian10_py2/
--rw-r--r--   0 jkotan   (15949) hasylab     (39)     3088 2021-09-22 11:50:52.000000 sardana-nxsrecorder-3.9.1/.ci/debian10_py2/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/.ci/debian10_py3/
--rw-r--r--   0 jkotan   (15949) hasylab     (39)     3065 2021-02-24 14:30:16.000000 sardana-nxsrecorder-3.9.1/.ci/debian10_py3/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/.ci/debian8_py2/
--rw-r--r--   0 jkotan   (15949) hasylab     (39)     6882 2021-02-24 14:30:16.000000 sardana-nxsrecorder-3.9.1/.ci/debian8_py2/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/.ci/debian8_py3/
--rw-r--r--   0 jkotan   (15949) hasylab     (39)     2776 2021-02-24 14:30:16.000000 sardana-nxsrecorder-3.9.1/.ci/debian8_py3/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/.ci/debian9_py2/
--rw-r--r--   0 jkotan   (15949) hasylab     (39)     3159 2021-09-22 11:50:52.000000 sardana-nxsrecorder-3.9.1/.ci/debian9_py2/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/.ci/debian9_py3/
--rw-r--r--   0 jkotan   (15949) hasylab     (39)     3182 2021-02-24 14:30:16.000000 sardana-nxsrecorder-3.9.1/.ci/debian9_py3/Dockerfile
--rw-r--r--   0 jkotan   (15949) hasylab     (39)     8497 2022-05-17 07:31:27.000000 sardana-nxsrecorder-3.9.1/.ci/install.sh
--rw-r--r--   0 jkotan   (15949) hasylab     (39)      249 2022-03-21 09:24:01.000000 sardana-nxsrecorder-3.9.1/.ci/run.sh
-drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/.ci/ubuntu16.04_py2/
--rw-r--r--   0 jkotan   (15949) hasylab     (39)     2622 2021-02-24 14:30:16.000000 sardana-nxsrecorder-3.9.1/.ci/ubuntu16.04_py2/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/.ci/ubuntu16.04_py3/
--rw-r--r--   0 jkotan   (15949) hasylab     (39)     2629 2021-02-24 14:30:16.000000 sardana-nxsrecorder-3.9.1/.ci/ubuntu16.04_py3/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/.ci/ubuntu18.04_py2/
--rw-r--r--   0 jkotan   (15949) hasylab     (39)     2684 2021-09-22 11:50:52.000000 sardana-nxsrecorder-3.9.1/.ci/ubuntu18.04_py2/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/.ci/ubuntu18.04_py3/
--rw-r--r--   0 jkotan   (15949) hasylab     (39)     2686 2021-09-22 11:50:52.000000 sardana-nxsrecorder-3.9.1/.ci/ubuntu18.04_py3/Dockerfile
-drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/.ci/ubuntu20.04_py3/
--rw-r--r--   0 jkotan   (15949) hasylab     (39)     2896 2022-05-17 07:31:27.000000 sardana-nxsrecorder-3.9.1/.ci/ubuntu20.04_py3/Dockerfile
--rw-r--r--   0 jkotan   (15949) hasylab     (39)      171 2019-01-30 16:18:15.000000 sardana-nxsrecorder-3.9.1/.flake8
-drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/.github/
-drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/.github/workflows/
--rw-r--r--   0 jkotan   (15949) hasylab     (39)     1904 2022-05-17 07:31:27.000000 sardana-nxsrecorder-3.9.1/.github/workflows/tests.yml
--rw-r--r--   0 jkotan   (15949) hasylab     (39)       83 2015-07-28 11:55:52.000000 sardana-nxsrecorder-3.9.1/.gitignore
--rw-r--r--   0 jkotan   (15949) hasylab     (39)    35147 2015-07-28 12:06:26.000000 sardana-nxsrecorder-3.9.1/COPYRIGHT
--rw-r--r--   0 jkotan   (15949) hasylab     (39)     3570 2022-10-19 06:02:13.000000 sardana-nxsrecorder-3.9.1/ChangeLog
--rw-r--r--   0 jkotan   (15949) hasylab     (39)       69 2016-05-11 08:08:46.000000 sardana-nxsrecorder-3.9.1/MANIFEST.in
--rw-r--r--   0 jkotan   (15949) hasylab     (39)     7480 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/PKG-INFO
--rw-r--r--   0 jkotan   (15949) hasylab     (39)     4763 2022-10-18 19:29:35.000000 sardana-nxsrecorder-3.9.1/README.rst
-drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/doc/
--rw-r--r--   0 jkotan   (15949) hasylab     (39)     6810 2016-05-11 08:08:46.000000 sardana-nxsrecorder-3.9.1/doc/Makefile
--rw-r--r--   0 jkotan   (15949) hasylab     (39)    14007 2021-02-24 16:19:15.000000 sardana-nxsrecorder-3.9.1/doc/conf.py
--rw-r--r--   0 jkotan   (15949) hasylab     (39)      414 2016-05-11 08:08:46.000000 sardana-nxsrecorder-3.9.1/doc/index.rst
--rw-r--r--   0 jkotan   (15949) hasylab     (39)     6725 2016-05-11 08:08:46.000000 sardana-nxsrecorder-3.9.1/doc/make.bat
--rw-r--r--   0 jkotan   (15949) hasylab     (39)      590 2016-05-11 08:08:46.000000 sardana-nxsrecorder-3.9.1/doc/sardananxsrecorder.rst
-drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/man/
--rw-r--r--   0 jkotan   (15949) hasylab     (39)     9890 2022-10-18 19:29:35.000000 sardana-nxsrecorder-3.9.1/man/sardananxsrecorder.1
-drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/sardana_nxsrecorder.egg-info/
--rw-r--r--   0 jkotan   (15949) hasylab     (39)     7480 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/sardana_nxsrecorder.egg-info/PKG-INFO
--rw-r--r--   0 jkotan   (15949) hasylab     (39)      925 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/sardana_nxsrecorder.egg-info/SOURCES.txt
--rw-r--r--   0 jkotan   (15949) hasylab     (39)        1 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/sardana_nxsrecorder.egg-info/dependency_links.txt
--rw-r--r--   0 jkotan   (15949) hasylab     (39)        1 2019-10-14 13:29:19.000000 sardana-nxsrecorder-3.9.1/sardana_nxsrecorder.egg-info/not-zip-safe
--rw-r--r--   0 jkotan   (15949) hasylab     (39)       17 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/sardana_nxsrecorder.egg-info/requires.txt
--rw-r--r--   0 jkotan   (15949) hasylab     (39)       19 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/sardana_nxsrecorder.egg-info/top_level.txt
-drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/sardananxsrecorder/
--rw-r--r--   0 jkotan   (15949) hasylab     (39)      895 2022-10-19 05:56:33.000000 sardana-nxsrecorder-3.9.1/sardananxsrecorder/__init__.py
--rw-r--r--   0 jkotan   (15949) hasylab     (39)    43098 2022-10-19 06:01:52.000000 sardana-nxsrecorder-3.9.1/sardananxsrecorder/nxsrecorder.py
--rw-r--r--   0 jkotan   (15949) hasylab     (39)      231 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/setup.cfg
--rwxr-xr-x   0 jkotan   (15949) hasylab     (39)     3405 2022-10-18 19:29:35.000000 sardana-nxsrecorder-3.9.1/setup.py
-drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 06:03:26.000000 sardana-nxsrecorder-3.9.1/test/
--rw-r--r--   0 jkotan   (15949) hasylab     (39)      916 2019-10-14 13:28:42.000000 sardana-nxsrecorder-3.9.1/test/__init__.py
--rw-r--r--   0 jkotan   (15949) hasylab     (39)      945 2019-10-14 13:28:48.000000 sardana-nxsrecorder-3.9.1/test/__main__.py
--rwxr-xr-x   0 jkotan   (15949) hasylab     (39)     4296 2019-01-30 16:18:50.000000 sardana-nxsrecorder-3.9.1/test/main.py
+drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/
+drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/.ci/
+drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/.ci/debian10_py2/
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)     3088 2021-09-22 11:50:52.000000 sardana-nxsrecorder-3.9.2/.ci/debian10_py2/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/.ci/debian10_py3/
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)     3065 2021-02-24 14:30:16.000000 sardana-nxsrecorder-3.9.2/.ci/debian10_py3/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/.ci/debian8_py2/
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)     6882 2021-02-24 14:30:16.000000 sardana-nxsrecorder-3.9.2/.ci/debian8_py2/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/.ci/debian8_py3/
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)     2776 2021-02-24 14:30:16.000000 sardana-nxsrecorder-3.9.2/.ci/debian8_py3/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/.ci/debian9_py2/
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)     3159 2021-09-22 11:50:52.000000 sardana-nxsrecorder-3.9.2/.ci/debian9_py2/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/.ci/debian9_py3/
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)     3182 2021-02-24 14:30:16.000000 sardana-nxsrecorder-3.9.2/.ci/debian9_py3/Dockerfile
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)     8497 2022-05-17 07:31:27.000000 sardana-nxsrecorder-3.9.2/.ci/install.sh
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)      249 2022-03-21 09:24:01.000000 sardana-nxsrecorder-3.9.2/.ci/run.sh
+drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/.ci/ubuntu16.04_py2/
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)     2622 2021-02-24 14:30:16.000000 sardana-nxsrecorder-3.9.2/.ci/ubuntu16.04_py2/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/.ci/ubuntu16.04_py3/
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)     2629 2021-02-24 14:30:16.000000 sardana-nxsrecorder-3.9.2/.ci/ubuntu16.04_py3/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/.ci/ubuntu18.04_py2/
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)     2684 2021-09-22 11:50:52.000000 sardana-nxsrecorder-3.9.2/.ci/ubuntu18.04_py2/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/.ci/ubuntu18.04_py3/
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)     2686 2021-09-22 11:50:52.000000 sardana-nxsrecorder-3.9.2/.ci/ubuntu18.04_py3/Dockerfile
+drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/.ci/ubuntu20.04_py3/
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)     2896 2022-05-17 07:31:27.000000 sardana-nxsrecorder-3.9.2/.ci/ubuntu20.04_py3/Dockerfile
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)      171 2019-01-30 16:18:15.000000 sardana-nxsrecorder-3.9.2/.flake8
+drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/.github/
+drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/.github/workflows/
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)     1904 2022-05-17 07:31:27.000000 sardana-nxsrecorder-3.9.2/.github/workflows/tests.yml
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)       83 2015-07-28 11:55:52.000000 sardana-nxsrecorder-3.9.2/.gitignore
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)    35147 2015-07-28 12:06:26.000000 sardana-nxsrecorder-3.9.2/COPYRIGHT
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)     3682 2022-10-19 09:36:25.000000 sardana-nxsrecorder-3.9.2/ChangeLog
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)       69 2016-05-11 08:08:46.000000 sardana-nxsrecorder-3.9.2/MANIFEST.in
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)     7480 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)     4763 2022-10-18 19:29:35.000000 sardana-nxsrecorder-3.9.2/README.rst
+drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/doc/
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)     6810 2016-05-11 08:08:46.000000 sardana-nxsrecorder-3.9.2/doc/Makefile
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)    14007 2021-02-24 16:19:15.000000 sardana-nxsrecorder-3.9.2/doc/conf.py
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)      414 2016-05-11 08:08:46.000000 sardana-nxsrecorder-3.9.2/doc/index.rst
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)     6725 2016-05-11 08:08:46.000000 sardana-nxsrecorder-3.9.2/doc/make.bat
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)      590 2016-05-11 08:08:46.000000 sardana-nxsrecorder-3.9.2/doc/sardananxsrecorder.rst
+drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/man/
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)     9890 2022-10-18 19:29:35.000000 sardana-nxsrecorder-3.9.2/man/sardananxsrecorder.1
+drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/sardana_nxsrecorder.egg-info/
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)     7480 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/sardana_nxsrecorder.egg-info/PKG-INFO
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)      925 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/sardana_nxsrecorder.egg-info/SOURCES.txt
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)        1 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/sardana_nxsrecorder.egg-info/dependency_links.txt
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)        1 2019-10-14 13:29:19.000000 sardana-nxsrecorder-3.9.2/sardana_nxsrecorder.egg-info/not-zip-safe
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)       17 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/sardana_nxsrecorder.egg-info/requires.txt
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)       19 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/sardana_nxsrecorder.egg-info/top_level.txt
+drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/sardananxsrecorder/
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)      895 2022-10-19 09:36:25.000000 sardana-nxsrecorder-3.9.2/sardananxsrecorder/__init__.py
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)    43097 2022-10-19 09:36:25.000000 sardana-nxsrecorder-3.9.2/sardananxsrecorder/nxsrecorder.py
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)      231 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/setup.cfg
+-rwxr-xr-x   0 jkotan   (15949) hasylab     (39)     3405 2022-10-18 19:29:35.000000 sardana-nxsrecorder-3.9.2/setup.py
+drwxr-xr-x   0 jkotan   (15949) hasylab     (39)        0 2022-10-19 09:39:13.000000 sardana-nxsrecorder-3.9.2/test/
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)      916 2019-10-14 13:28:42.000000 sardana-nxsrecorder-3.9.2/test/__init__.py
+-rw-r--r--   0 jkotan   (15949) hasylab     (39)      945 2019-10-14 13:28:48.000000 sardana-nxsrecorder-3.9.2/test/__main__.py
+-rwxr-xr-x   0 jkotan   (15949) hasylab     (39)     4296 2019-01-30 16:18:50.000000 sardana-nxsrecorder-3.9.2/test/main.py
```

### Comparing `sardana-nxsrecorder-3.9.1/.ci/debian10_py2/Dockerfile` & `sardana-nxsrecorder-3.9.2/.ci/debian10_py2/Dockerfile`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/.ci/debian10_py3/Dockerfile` & `sardana-nxsrecorder-3.9.2/.ci/debian10_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/.ci/debian8_py2/Dockerfile` & `sardana-nxsrecorder-3.9.2/.ci/debian8_py2/Dockerfile`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/.ci/debian8_py3/Dockerfile` & `sardana-nxsrecorder-3.9.2/.ci/debian8_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/.ci/debian9_py2/Dockerfile` & `sardana-nxsrecorder-3.9.2/.ci/debian9_py2/Dockerfile`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/.ci/debian9_py3/Dockerfile` & `sardana-nxsrecorder-3.9.2/.ci/debian9_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/.ci/install.sh` & `sardana-nxsrecorder-3.9.2/.ci/install.sh`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/.ci/ubuntu16.04_py2/Dockerfile` & `sardana-nxsrecorder-3.9.2/.ci/ubuntu16.04_py2/Dockerfile`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/.ci/ubuntu16.04_py3/Dockerfile` & `sardana-nxsrecorder-3.9.2/.ci/ubuntu16.04_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/.ci/ubuntu18.04_py2/Dockerfile` & `sardana-nxsrecorder-3.9.2/.ci/ubuntu18.04_py2/Dockerfile`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/.ci/ubuntu18.04_py3/Dockerfile` & `sardana-nxsrecorder-3.9.2/.ci/ubuntu18.04_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/.ci/ubuntu20.04_py3/Dockerfile` & `sardana-nxsrecorder-3.9.2/.ci/ubuntu20.04_py3/Dockerfile`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/.github/workflows/tests.yml` & `sardana-nxsrecorder-3.9.2/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/COPYRIGHT` & `sardana-nxsrecorder-3.9.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/ChangeLog` & `sardana-nxsrecorder-3.9.2/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,12 @@
 2022-10-19 Jan Kotanski <jankotan@gmail.com>
+	* fix setting nexus_components variable (#44)
+	* tagged as 3.9.2
+
+2022-10-19 Jan Kotanski <jankotan@gmail.com>
 	* add nexus_components and measurement_group variables
 	* tagged as 3.9.1
 
 2022-07-06 Jan Kotanski <jankotan@gmail.com>
 	* append SciCat dataset to the list file if NXSAppendSciCatDataset is set
 	* tagged as 3.8.0
```

### Comparing `sardana-nxsrecorder-3.9.1/PKG-INFO` & `sardana-nxsrecorder-3.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sardana-nxsrecorder
-Version: 3.9.1
+Version: 3.9.2
 Summary: NeXus Sardana Scan Recorder
 Home-page: https://github.com/nexdatas/sardana-nxs-filerecorder/
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Description: Welcome to sardananxsrecorder's documentation!
         ==============================================
```

### Comparing `sardana-nxsrecorder-3.9.1/README.rst` & `sardana-nxsrecorder-3.9.2/README.rst`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/doc/Makefile` & `sardana-nxsrecorder-3.9.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/doc/conf.py` & `sardana-nxsrecorder-3.9.2/doc/conf.py`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/doc/make.bat` & `sardana-nxsrecorder-3.9.2/doc/make.bat`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/doc/sardananxsrecorder.rst` & `sardana-nxsrecorder-3.9.2/doc/sardananxsrecorder.rst`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/man/sardananxsrecorder.1` & `sardana-nxsrecorder-3.9.2/man/sardananxsrecorder.1`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/sardana_nxsrecorder.egg-info/PKG-INFO` & `sardana-nxsrecorder-3.9.2/sardana_nxsrecorder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: sardana-nxsrecorder
-Version: 3.9.1
+Version: 3.9.2
 Summary: NeXus Sardana Scan Recorder
 Home-page: https://github.com/nexdatas/sardana-nxs-filerecorder/
 Author: Jan Kotanski
 Author-email: jankotan@gmail.com
 License: GNU GENERAL PUBLIC LICENSE v3
 Description: Welcome to sardananxsrecorder's documentation!
         ==============================================
```

### Comparing `sardana-nxsrecorder-3.9.1/sardana_nxsrecorder.egg-info/SOURCES.txt` & `sardana-nxsrecorder-3.9.2/sardana_nxsrecorder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/sardananxsrecorder/__init__.py` & `sardana-nxsrecorder-3.9.2/sardananxsrecorder/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 #    You should have received a copy of the GNU General Public License
 #    along with nexdatas.  If not, see <http://www.gnu.org/licenses/>.
 #
 
 """ Sardana Scan Recorders """
 
 #: package version
-__version__ = "3.9.1"
+__version__ = "3.9.2"
```

### Comparing `sardana-nxsrecorder-3.9.1/sardananxsrecorder/nxsrecorder.py` & `sardana-nxsrecorder-3.9.2/sardananxsrecorder/nxsrecorder.py`

 * *Files 0% similar despite different names*

```diff
@@ -809,23 +809,23 @@
                                     None, True, pass_default=self.__oddmntgrp)
             allcp = list(nexuscomponents)
             allcp.extend(list(toswitch))
             och = och or []
             self.__aliases = [ch for ch in och if ch in allcp]
             if self.__aliases:
                 self.__vars["vars"]["mgchannels"] = " ".join(self.__aliases)
+            self.__vars["vars"]["nexus_components"] = " ".join(nexuscomponents)
             self.__nexussettings_device.configVariables = json.dumps(
                 dict(nexusvariables, **self.__vars["vars"]),
                 cls=NXS_FileRecorder.numpyEncoder)
             if self.__macro:
                 self.__macro().debug(
                     "VAR %s" % self.__nexussettings_device.configVariables)
             self.__command(self.__nexussettings_device,
                            "updateConfigVariables")
-            self.__vars["vars"]["nexus_components"] = " ".join(nexuscomponents)
 
             self.debug("Aliases: %s" % str(self.__aliases))
             self.debug("Switching to STEP mode: %s" % toswitch)
             oldtoswitch = self.__getServerVar("stepdatasources", "[]", False)
             stepdss = str(json.dumps(list(toswitch)))
             self.__nexussettings_device.stepdatasources = stepdss
             if hasattr(self.__nexussettings_device, "linkdatasources"):
@@ -860,15 +860,14 @@
             appendentry = not self.__setFileName(
                 self.__base_filename, not appendentry)
             envRec = self.recordlist.getEnviron()
             self.__vars["vars"]["serialno"] = envRec["serialno"] \
                 if appendentry else ""
             self.__vars["vars"]["scan_id"] = envRec["serialno"]
             self.__vars["vars"]["scan_title"] = envRec["title"]
-
             tzone = self.__getConfVar("TimeZone", self.__timezone)
             self.__vars["data"]["start_time"] = \
                 self.__timeToString(envRec['starttime'], tzone)
             self.__vars["vars"]["filename"] = str(self.filename)
 
             envrecord = self.__appendRecord(self.__vars, 'INIT')
             rec = json.dumps(
```

### Comparing `sardana-nxsrecorder-3.9.1/setup.py` & `sardana-nxsrecorder-3.9.2/setup.py`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/test/__init__.py` & `sardana-nxsrecorder-3.9.2/test/__init__.py`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/test/__main__.py` & `sardana-nxsrecorder-3.9.2/test/__main__.py`

 * *Files identical despite different names*

### Comparing `sardana-nxsrecorder-3.9.1/test/main.py` & `sardana-nxsrecorder-3.9.2/test/main.py`

 * *Files identical despite different names*

