# Comparing `tmp/osint_comp-0.2.0.tar.gz` & `tmp/osint_comp-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osint_comp-0.2.0.tar", last modified: Tue May 21 22:16:24 2024, max compression
+gzip compressed data, was "osint_comp-0.2.1.tar", last modified: Tue May 21 22:46:04 2024, max compression
```

## Comparing `osint_comp-0.2.0.tar` & `osint_comp-0.2.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:16:24.023048 osint_comp-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-21 22:16:24.023048 osint_comp-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-21 22:16:18.000000 osint_comp-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-21 22:16:18.000000 osint_comp-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 22:16:24.023048 osint_comp-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:16:24.023048 osint_comp-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:16:24.023048 osint_comp-0.2.0/src/osint_comp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-21 22:16:24.000000 osint_comp-0.2.0/src/osint_comp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-21 22:16:24.000000 osint_comp-0.2.0/src/osint_comp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 22:16:24.000000 osint_comp-0.2.0/src/osint_comp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 22:16:24.000000 osint_comp-0.2.0/src/osint_comp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 22:16:24.000000 osint_comp-0.2.0/src/osint_comp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 22:16:24.000000 osint_comp-0.2.0/src/osint_comp.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:16:24.023048 osint_comp-0.2.0/src/osinter/
--rw-r--r--   0 runner    (1001) docker     (127)    13883 2024-05-21 22:16:18.000000 osint_comp-0.2.0/src/osinter/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:46:04.760207 osint_comp-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-21 22:46:04.760207 osint_comp-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-21 22:45:58.000000 osint_comp-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-21 22:45:58.000000 osint_comp-0.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 22:46:04.760207 osint_comp-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:46:04.760207 osint_comp-0.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:46:04.760207 osint_comp-0.2.1/src/osint_comp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-21 22:46:04.000000 osint_comp-0.2.1/src/osint_comp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-21 22:46:04.000000 osint_comp-0.2.1/src/osint_comp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 22:46:04.000000 osint_comp-0.2.1/src/osint_comp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 22:46:04.000000 osint_comp-0.2.1/src/osint_comp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 22:46:04.000000 osint_comp-0.2.1/src/osint_comp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 22:46:04.000000 osint_comp-0.2.1/src/osint_comp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 22:46:04.760207 osint_comp-0.2.1/src/osinter/
+-rw-r--r--   0 runner    (1001) docker     (127)    13927 2024-05-21 22:45:58.000000 osint_comp-0.2.1/src/osinter/__main__.py
```

### Comparing `osint_comp-0.2.0/src/osinter/__main__.py` & `osint_comp-0.2.1/src/osinter/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     else:
         if os.path.exists(f"osint/{file}"):
             raise click.ClickException(f"A file with the name {file} already exists.")        
     os.mkdir(f"osint/{file}")
     os.system(f"touch osint/{file}/init.oie")
     os.system(f"touch osint/{file}/name.oie")
     os.system(f"touch osint/{file}/address.oie")
+    os.system(f"touch osint/{file}/online")
     os.system(f"touch osint/{file}/online/usernames.oie")
     os.system(f"touch osint/{file}/online/emails.oie")
     fn = open(f"osint/{file}/name.oie", "a")
     fa = open(f"osint/{file}/address.oie", "a")
     fos = open(f"osint/{file}/online/socials.oie", "a")
     fn.write("\n\n\n\n\n")
     fa.write("\n\n\n\n\n\n\n")
```

