# Comparing `tmp/tgwrap-0.9.2.tar.gz` & `tmp/tgwrap-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgwrap-0.9.2.tar", max compression
+gzip compressed data, was "tgwrap-0.9.3.tar", max compression
```

## Comparing `tgwrap-0.9.2.tar` & `tgwrap-0.9.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.9.2/LICENSE
--rw-r--r--   0        0        0    12159 2024-04-24 11:33:21.171629 tgwrap-0.9.2/README.md
--rw-r--r--   0        0        0      922 2024-04-30 12:18:23.521352 tgwrap-0.9.2/pyproject.toml
--rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.9.2/tgwrap/__init__.py
--rw-r--r--   0        0        0     8726 2023-10-20 14:35:12.875311 tgwrap-0.9.2/tgwrap/analyze.py
--rwxr-xr-x   0        0        0    29727 2024-04-24 07:14:54.956803 tgwrap-0.9.2/tgwrap/cli.py
--rw-r--r--   0        0        0    10243 2024-04-29 11:10:37.178306 tgwrap-0.9.2/tgwrap/deploy.py
--rwxr-xr-x   0        0        0    81157 2024-04-30 12:17:52.165017 tgwrap-0.9.2/tgwrap/main.py
--rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.9.2/tgwrap/printer.py
--rw-r--r--   0        0        0    13334 1970-01-01 00:00:00.000000 tgwrap-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2022-12-25 10:02:18.884994 tgwrap-0.9.3/LICENSE
+-rw-r--r--   0        0        0    12159 2024-04-24 11:33:21.171629 tgwrap-0.9.3/README.md
+-rw-r--r--   0        0        0      922 2024-05-22 13:11:22.733006 tgwrap-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-12-26 11:59:24.403826 tgwrap-0.9.3/tgwrap/__init__.py
+-rw-r--r--   0        0        0     8726 2023-10-20 14:35:12.875311 tgwrap-0.9.3/tgwrap/analyze.py
+-rwxr-xr-x   0        0        0    29728 2024-05-22 13:10:28.828756 tgwrap-0.9.3/tgwrap/cli.py
+-rw-r--r--   0        0        0    10243 2024-04-29 11:10:37.178306 tgwrap-0.9.3/tgwrap/deploy.py
+-rwxr-xr-x   0        0        0    81157 2024-04-30 12:17:52.165017 tgwrap-0.9.3/tgwrap/main.py
+-rw-r--r--   0        0        0     2663 2023-01-16 19:18:54.217701 tgwrap-0.9.3/tgwrap/printer.py
+-rw-r--r--   0        0        0    13334 1970-01-01 00:00:00.000000 tgwrap-0.9.3/PKG-INFO
```

### Comparing `tgwrap-0.9.2/LICENSE` & `tgwrap-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tgwrap-0.9.2/README.md` & `tgwrap-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `tgwrap-0.9.2/pyproject.toml` & `tgwrap-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tgwrap"
-version = "0.9.2"
+version = "0.9.3"
 description = "A (terragrunt) wrapper around a (terraform) wrapper around ...."
 authors = ["Gerco Grandia <gerco.grandia@4synergy.nl>", "Pascal Alma <pascal.alma@4synergy.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/lunadata/tgwrap"
 repository = "https://gitlab.com/lunadata/tgwrap"
 documentation = "https://gitlab.com/lunadata/tgwrap/"
```

### Comparing `tgwrap-0.9.2/tgwrap/analyze.py` & `tgwrap-0.9.3/tgwrap/analyze.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.9.2/tgwrap/cli.py` & `tgwrap-0.9.3/tgwrap/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
         elif verbose:
             echo(f'You are running version {__version__}, latest is {latest_version}')
 
     except ValueError:
         # this happens when your local version is ahead of the pypi version,
         # which happens only in development
         pass
-    except KeyError:
+    except Exception:
         echo('Could not determine package version, continue nevertheless.')
         pass
 
 CLICK_CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
 
 TG_COMMANDS=[
     'init', 'validate', 'validate-inputs', 'plan', 'apply',
```

### Comparing `tgwrap-0.9.2/tgwrap/deploy.py` & `tgwrap-0.9.3/tgwrap/deploy.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.9.2/tgwrap/main.py` & `tgwrap-0.9.3/tgwrap/main.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.9.2/tgwrap/printer.py` & `tgwrap-0.9.3/tgwrap/printer.py`

 * *Files identical despite different names*

### Comparing `tgwrap-0.9.2/PKG-INFO` & `tgwrap-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tgwrap
-Version: 0.9.2
+Version: 0.9.3
 Summary: A (terragrunt) wrapper around a (terraform) wrapper around ....
 Home-page: https://gitlab.com/lunadata/tgwrap
 License: MIT
 Keywords: terraform,terragrunt,terrasafe,python
 Author: Gerco Grandia
 Author-email: gerco.grandia@4synergy.nl
 Requires-Python: >=3.8,<4.0
```

