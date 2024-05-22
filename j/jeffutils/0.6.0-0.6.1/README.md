# Comparing `tmp/jeffutils-0.6.0.tar.gz` & `tmp/jeffutils-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeffutils-0.6.0.tar", last modified: Mon May 20 22:29:47 2024, max compression
+gzip compressed data, was "jeffutils-0.6.1.tar", last modified: Wed May 22 16:23:30 2024, max compression
```

## Comparing `jeffutils-0.6.0.tar` & `jeffutils-0.6.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-20 22:29:47.816292 jeffutils-0.6.0/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.6.0/LICENSE.txt
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-20 22:29:47.816292 jeffutils-0.6.0/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.6.0/README.md
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.6.0/pyproject.toml
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-20 22:29:47.816292 jeffutils-0.6.0/setup.cfg
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-05-20 22:29:43.000000 jeffutils-0.6.0/setup.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-20 22:29:47.816292 jeffutils-0.6.0/src/
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-20 22:29:47.816292 jeffutils-0.6.0/src/jeffutils/
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.6.0/src/jeffutils/__init__.py
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    25233 2024-05-20 22:29:12.000000 jeffutils-0.6.0/src/jeffutils/utils.py
-drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-20 22:29:47.816292 jeffutils-0.6.0/src/jeffutils.egg-info/
--rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-20 22:29:47.000000 jeffutils-0.6.0/src/jeffutils.egg-info/PKG-INFO
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-20 22:29:47.000000 jeffutils-0.6.0/src/jeffutils.egg-info/SOURCES.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-20 22:29:47.000000 jeffutils-0.6.0/src/jeffutils.egg-info/dependency_links.txt
--rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-20 22:29:47.000000 jeffutils-0.6.0/src/jeffutils.egg-info/top_level.txt
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-22 16:23:30.430934 jeffutils-0.6.1/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)     1070 2024-03-16 21:55:37.000000 jeffutils-0.6.1/LICENSE.txt
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-22 16:23:30.430934 jeffutils-0.6.1/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       12 2024-03-16 21:29:21.000000 jeffutils-0.6.1/README.md
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       84 2024-03-16 21:54:38.000000 jeffutils-0.6.1/pyproject.toml
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       38 2024-05-22 16:23:30.430934 jeffutils-0.6.1/setup.cfg
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      559 2024-05-22 16:23:25.000000 jeffutils-0.6.1/setup.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-22 16:23:30.426934 jeffutils-0.6.1/src/
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-22 16:23:30.426934 jeffutils-0.6.1/src/jeffutils/
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        0 2024-03-16 21:50:41.000000 jeffutils-0.6.1/src/jeffutils/__init__.py
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)    25603 2024-05-22 16:22:44.000000 jeffutils-0.6.1/src/jeffutils/utils.py
+drwxrwxr-x   0 jeffx     (1000) jeffx     (1000)        0 2024-05-22 16:23:30.430934 jeffutils-0.6.1/src/jeffutils.egg-info/
+-rw-r--r--   0 jeffx     (1000) jeffx     (1000)      420 2024-05-22 16:23:30.000000 jeffutils-0.6.1/src/jeffutils.egg-info/PKG-INFO
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)      242 2024-05-22 16:23:30.000000 jeffutils-0.6.1/src/jeffutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)        1 2024-05-22 16:23:30.000000 jeffutils-0.6.1/src/jeffutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeffx     (1000) jeffx     (1000)       10 2024-05-22 16:23:30.000000 jeffutils-0.6.1/src/jeffutils.egg-info/top_level.txt
```

### Comparing `jeffutils-0.6.0/LICENSE.txt` & `jeffutils-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jeffutils-0.6.0/setup.py` & `jeffutils-0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 setup(
     name='jeffutils',
-    version='0.6.0',
+    version='0.6.1',
     author='Jeff Hansen',
     author_email='jeffxhansen@gmail.com',
     description='A series of useful functions and decorators I use in most of my projects. Feel free to use them as well :)',
     package_dir={"": "src"},
     packages = find_packages(where="src"),
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `jeffutils-0.6.0/src/jeffutils/utils.py` & `jeffutils-0.6.1/src/jeffutils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -394,14 +394,23 @@
     if place == 'Before':
         seg1 = cols[:list(cols).index(ref_col)]
         seg2 = cols_to_move + [ref_col]
     seg1 = [i for i in seg1 if i not in seg2]
     seg3 = [i for i in cols if i not in seg1 + seg2]
     return df[seg1 + seg2 + seg3]
 
+def rename_duplicate_columns(df):
+    """ renames duplicate columns in a pandas dataframe by appending a number to the end """
+    df = df.copy()
+    cols = pd.Series(df.columns)
+    for dup in cols[cols.duplicated()].unique():
+        cols[cols[cols == dup].index.values[1:]] = [f"{dup}{i}" for i in range(2, sum(cols == dup)+2-1)]
+    df.columns = cols
+    return df
+
     
 ###################
 # NUMPY FUNCTIONS #
 ###################
 
 def rolling_window(a, window=15):
     """returns a numpy rolling window
```

