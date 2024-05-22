# Comparing `tmp/ddeutil_io-0.1.6.tar.gz` & `tmp/ddeutil_io-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ddeutil_io-0.1.6.tar", last modified: Fri May 17 10:22:54 2024, max compression
+gzip compressed data, was "ddeutil_io-0.1.7.tar", last modified: Wed May 22 02:05:18 2024, max compression
```

## Comparing `ddeutil_io-0.1.6.tar` & `ddeutil_io-0.1.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:54.564652 ddeutil_io-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-17 10:22:54.564652 ddeutil_io-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 10:22:54.564652 ddeutil_io-0.1.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:54.556652 ddeutil_io-0.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:54.556652 ddeutil_io-0.1.6/src/ddeutil/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:54.560652 ddeutil_io-0.1.6/src/ddeutil/io/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/src/ddeutil/io/__about__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:54.560652 ddeutil_io-0.1.6/src/ddeutil/io/__base/
--rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/src/ddeutil/io/__base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5525 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/src/ddeutil/io/__base/__regex.py
--rw-r--r--   0 runner    (1001) docker     (127)    15375 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/src/ddeutil/io/__base/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/src/ddeutil/io/__base/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/src/ddeutil/io/__conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/src/ddeutil/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12641 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/src/ddeutil/io/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/src/ddeutil/io/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/src/ddeutil/io/param.py
--rw-r--r--   0 runner    (1001) docker     (127)    17702 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/src/ddeutil/io/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/src/ddeutil/io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:54.564652 ddeutil_io-0.1.6/src/ddeutil_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-17 10:22:54.000000 ddeutil_io-0.1.6/src/ddeutil_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-17 10:22:54.000000 ddeutil_io-0.1.6/src/ddeutil_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 10:22:54.000000 ddeutil_io-0.1.6/src/ddeutil_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-17 10:22:54.000000 ddeutil_io-0.1.6/src/ddeutil_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 10:22:54.000000 ddeutil_io-0.1.6/src/ddeutil_io.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 10:22:54.564652 ddeutil_io-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/tests/test_base_csv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/tests/test_base_dir.py
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/tests/test_base_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/tests/test_base_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/tests/test_base_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/tests/test_config_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/tests/test_config_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     3627 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/tests/test_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/tests/test_register.py
--rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-17 10:22:49.000000 ddeutil_io-0.1.6/tests/test_register_deploy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:05:18.879441 ddeutil_io-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-22 02:05:18.879441 ddeutil_io-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 02:05:18.879441 ddeutil_io-0.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:05:18.875441 ddeutil_io-0.1.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:05:18.875441 ddeutil_io-0.1.7/src/ddeutil/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:05:18.875441 ddeutil_io-0.1.7/src/ddeutil/io/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/__about__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:05:18.875441 ddeutil_io-0.1.7/src/ddeutil/io/__base/
+-rw-r--r--   0 runner    (1001) docker     (127)     4618 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/__base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/__base/__regex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15375 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/__base/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6781 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/__base/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/__conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12651 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/param.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19666 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/src/ddeutil/io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:05:18.879441 ddeutil_io-0.1.7/src/ddeutil_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-22 02:05:18.000000 ddeutil_io-0.1.7/src/ddeutil_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-22 02:05:18.000000 ddeutil_io-0.1.7/src/ddeutil_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:05:18.000000 ddeutil_io-0.1.7/src/ddeutil_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-22 02:05:18.000000 ddeutil_io-0.1.7/src/ddeutil_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 02:05:18.000000 ddeutil_io-0.1.7/src/ddeutil_io.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:05:18.879441 ddeutil_io-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/tests/test_base_csv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/tests/test_base_dir.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/tests/test_base_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6370 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/tests/test_base_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6385 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/tests/test_base_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/tests/test_config_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/tests/test_config_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/tests/test_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/tests/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1814 2024-05-22 02:05:14.000000 ddeutil_io-0.1.7/tests/test_register_deploy.py
```

### Comparing `ddeutil_io-0.1.6/LICENSE` & `ddeutil_io-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.6/PKG-INFO` & `ddeutil_io-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddeutil-io
-Version: 0.1.6
+Version: 0.1.7
 Summary: Data Developer & Engineer IO Utility Objects
 Author-email: ddeutils <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/korawica/ddeutil-io/
 Project-URL: Source Code, https://github.com/korawica/ddeutil-io/
 Keywords: data,config,utility
 Classifier: Topic :: Utilities
```

### Comparing `ddeutil_io-0.1.6/README.md` & `ddeutil_io-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.6/pyproject.toml` & `ddeutil_io-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.6/src/ddeutil/io/__base/__init__.py` & `ddeutil_io-0.1.7/src/ddeutil/io/__base/__init__.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.6/src/ddeutil/io/__base/__regex.py` & `ddeutil_io-0.1.7/src/ddeutil/io/__base/__regex.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,135 +12,139 @@
     Pattern,
 )
 
 
 class RegexConf:
     """Core Configuration Model"""
 
-    # Normal regular expression for the secret value.
+    # NOTE: Normal regular expression for the secret value.
     # ---
     # [\"\']?                             # single or double quoted value
     # (?P<search>@secrets{                # search string for replacement
     #     (?P<braced>.*?)                 # value if use braced {}
     #     (?::(?P<braced_default>.*?))?   # value default with sep :
     # })                                  # end with }
     # [\"\']?                             # single or double-quoted value
     #
-    # Note: For secrets grouping level.
+    # NOTE: For secrets grouping level.
     # ---
     # [\"\']?                             # single or double quoted value
     # (?P<search>@secrets                 # search string for replacement
     # (?P<group>(\.\w+)*)?{               # search groups
     #     (?P<braced>.*?)                 # value if use braced {}
     #     (:(?P<braced_default>.*?))?     # value default with sep :
     # })                                  # end with }
     # [\"\']?                             # single or double-quoted value
-    RE_SECRETS: Pattern = re.compile(
-        r"""
+    __re_secrets: str = r"""
         [\"\']?                             # single or double quoted value
         (?P<search>@secrets{                # search string for replacement
             (?P<braced>.*?)                 # value if use braced {}
             (?::(?P<braced_default>.*?))?   # value default with sep :
         })                                  # end with }
         [\"\']?                             # single or double-quoted value
-    """,
-        MULTILINE | UNICODE | IGNORECASE | VERBOSE,
+    """
+    RE_SECRETS: Pattern = re.compile(
+        __re_secrets, MULTILINE | UNICODE | IGNORECASE | VERBOSE
     )
 
-    # Normal regular expression for the function value.
+    # NOTE: Normal regular expression for the function value.
     # ---
     # [\"\']?                             # single or double quoted value
     # (?P<search>@function{               # search string for replacement
     #     (?P<function>[\w.].*?)          # called function
     #     (?::(?P<arguments>.*?))?        # arguments for calling function
     # })                                  # end with }
     # [\"\']?                             # single or double-quoted value
-    RE_FUNCTION: Pattern = re.compile(
-        r"""
+    __re_function: str = r"""
         [\"\']?                             # single or double quoted value
         (?P<search>@function{               # search string for replacement
             (?P<function>[\w.].*?)          # called function
             (?::(?P<arguments>.*?))?        # arguments for calling function
         })                                  # end with }
         [\"\']?                             # single or double-quoted value
-    """,
-        MULTILINE | UNICODE | IGNORECASE | VERBOSE,
+    """
+    RE_FUNCTION: Pattern = re.compile(
+        __re_function, MULTILINE | UNICODE | IGNORECASE | VERBOSE
     )
 
-    # Normal regular expression for dotenv variable
+    # NOTE: Normal regular expression for dotenv variable
     # ---
     # (\\)?(\$)({?([A-Z0-9_]+)}?)
-    RE_DOTENV_VAR: Pattern = re.compile(
-        r"""
+    __re_dotenv_var: str = r"""
         (\\)?               # is it escaped with a backslash?
         (\$)                # literal $
         (                   # collect braces with var for sub
             {?              # allow brace wrapping
             ([A-Z0-9_]+)    # match the variable
             }?              # closing brace
         )                   # braces end
-    """,
-        IGNORECASE | VERBOSE,
-    )
+    """
+    RE_DOTENV_VAR: Pattern = re.compile(__re_dotenv_var, IGNORECASE | VERBOSE)
 
-    # Normal regular expression for dotenv
+    # NOTE: Normal regular expression for dotenv
     # ---
     # ^\s*(?:export\s+)?(?P<name>[\w.-]+)(?:\s*=\s*?|:\s+?)(?P<value>\s*\'(?:\\'|[^'])*\'|\s*\"(?:\\"|[^"])*\"
     # |\s*`(?:\\`|[^`])*`|[^#\r\n]+)?\s*$
-    RE_DOTENV: Pattern = re.compile(
-        r"""
-        ^\s*(?:export\s+)?      # optional export
-        (?P<name>[\w.-]+)       # name of key
-        (?:\s*=\s*?|:\s+?)      # separator `=` or `:`
+    __re_dotenv: str = r"""
+        ^\s*(?:export\s+)?          # optional export
+        (?P<name>[\w.-]+)           # name of key
+        (?:\s*=\s*?|:\s+?)          # separator `=` or `:`
         (?P<value>
             \s*\'(?:\\'|[^'])*\'    # single quoted value
             |
             \s*\"(?:\\"|[^"])*\"    # double quoted value
             |
             \s*`(?:\\`|[^`])*`      # backticks value
             |
-            [^#\r\n]+           # unquoted value
-        )?\s*                   # optional space
+            [^#\r\n]+               # unquoted value
+        )?\s*                       # optional space
         (?:[^\S\r\n]*\#[^\r\n]*)?
         $
-    """,
-        MULTILINE | VERBOSE,
-    )
+    """
+    RE_DOTENV: Pattern = re.compile(__re_dotenv, MULTILINE | VERBOSE)
 
-    # Note
+    # NOTE:
     # ---
     # (\s|^)#.*
+    __re_yaml_comment: str = r"(\s|^)#.*"
     RE_YAML_COMMENT: Pattern = re.compile(
-        r"(\s|^)#.*",
-        MULTILINE | UNICODE | IGNORECASE,
+        __re_yaml_comment, MULTILINE | UNICODE | IGNORECASE
     )
 
-    # Note
+    # NOTE:
     # ---
     # [\"\']?(\$(?:(?P<escaped>\$|\d+)|({(?P<braced>.*?)(:(?P<braced_default>.*?))?})))[\"\']?
-    RE_ENV_SEARCH: Pattern = re.compile(
-        r"""
+    #
+    # NOTE: If you want to catch only string not number:
+    #   ... `([a-zA-Z0-9_.\s'\"\[\]\(\)]+?)`
+    __re_env_search: str = r"""
         [\"\']?                             # single or double quoted value
         (\$(?:                              # start with non-capturing group
             (?P<escaped>\$|\d+)             # escape $ or number like $1
             |
             (\{
-                (?P<braced>.*?)             # value if use braced {}
-                (:(?P<braced_default>.*?))? # value default with sep :
+                (?P<braced>([^{}]*?))       # value in braced {} not contain {}
+                (:                          # : seperator for default
+                    (?P<braced_default>[^{}]*?) # value default with sep :
+                )?
             })
         ))
         [\"\']?                             # single or double quoted value
-    """,
-        MULTILINE | UNICODE | IGNORECASE | VERBOSE,
+    """
+    RE_ENV_SEARCH: Pattern = re.compile(
+        __re_env_search, MULTILINE | UNICODE | IGNORECASE | VERBOSE
     )
 
-    RE_ENV_VALUE_QUOTED: Pattern = re.compile(
-        r"""
+    __re_env_value_quoted: str = r"""
         ^
-            (?P<quoted>[\'\"`])
+            (?P<quoted>[\'\"`])     # single or double quoted value
             (?P<value>.*)\1
         $
-    """,
-        MULTILINE | VERBOSE,
+    """
+    RE_ENV_VALUE_QUOTED: Pattern = re.compile(
+        __re_env_value_quoted,
+        MULTILINE | UNICODE | VERBOSE,
     )
 
-    RE_ENV_ESCAPE: Pattern = re.compile(r"\\([^$])")
+    # NOTE:
+    __re_env_escape: str = r"\\([^$])"
+    RE_ENV_ESCAPE: Pattern = re.compile(__re_env_escape, MULTILINE | UNICODE)
```

### Comparing `ddeutil_io-0.1.6/src/ddeutil/io/__base/files.py` & `ddeutil_io-0.1.7/src/ddeutil/io/__base/files.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.6/src/ddeutil/io/__base/utils.py` & `ddeutil_io-0.1.7/src/ddeutil/io/__base/utils.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.6/src/ddeutil/io/__init__.py` & `ddeutil_io-0.1.7/src/ddeutil/io/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 from .exceptions import (
     ConfigArgumentError,
     ConfigNotFound,
     IOBaseError,
 )
 from .param import (
     Engine,
-    Flag,
     Params,
     PathData,
     Rule,
     Stage,
     Value,
 )
 from .register import Register
```

### Comparing `ddeutil_io-0.1.6/src/ddeutil/io/config.py` & `ddeutil_io-0.1.7/src/ddeutil/io/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,15 +307,15 @@
             if result := cur.fetchall():
                 return {_["name"]: self.convert_type(_) for _ in result}
             return default if (default is not None) else {}
 
     def save_stage(
         self,
         table: str,
-        data: dict,
+        data: dict[str, Any],
         merge: bool = False,
     ) -> None:
         """Write content data to database with table name. If merge is true, it
         will update or insert the data content.
         """
         _db, _table = table.rsplit("/", maxsplit=1)
         _data: dict = self.prepare_values(data.get(list(data.keys())[0]))
```

### Comparing `ddeutil_io-0.1.6/src/ddeutil/io/exceptions.py` & `ddeutil_io-0.1.7/src/ddeutil/io/exceptions.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.6/src/ddeutil/io/param.py` & `ddeutil_io-0.1.7/src/ddeutil/io/param.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,22 +39,21 @@
     "version",
     "compress",
 )
 
 
 class Rule(BaseModel):
     """Rule Model that keep rule setting data for Register object.
-    .. example::
-        {
-            "timestamp": {
-                "minutes": 15
-            },
-            "excluded": [],
-            "compress": None,
-        }
+
+    Examples:
+        >>> rule = {
+        ...     "timestamp": {"minutes": 15},
+        ...     "excluded": [],
+        ...     "compress": None,
+        ... }
     """
 
     timestamp: Optional[dict[str, int]] = Field(default_factory=dict)
     version: Annotated[Optional[str], Field()] = None
     excluded: Optional[list[str]] = Field(default_factory=list)
     compress: Annotated[
         Optional[str],
@@ -125,42 +124,36 @@
         return value
 
 
 class PathData(BaseModel):
     root: Path = Field(default_factory=Path)
     data: Path = Field(default=None, validate_default=True)
     conf: Path = Field(default=None, validate_default=True)
-    archive: Path = Field(default=None, validate_default=True)
 
     @field_validator("root", mode="before")
     def prepare_root(cls, v: Union[str, Path]) -> Path:
         return Path(v) if isinstance(v, str) else v
 
-    @field_validator("data", "conf", "archive", mode="before")
+    @field_validator("data", "conf", mode="before")
     def prepare_path_from_path_str(cls, v, info: ValidationInfo) -> Path:
         if v is not None:
             return Path(v) if isinstance(v, str) else v
         if info.field_name == "archive":
             return info.data["root"] / ".archive"
         return info.data["root"] / info.field_name
 
 
-class Flag(BaseModel):
-    archive: bool = Field(default=False)
-
-
 class Value(BaseModel):
     dt_fmt: str = Field(default="%Y-%m-%d %H:%M:%S")
     excluded: TupleStr = Field(default=(VERSION_KEY, UPDATE_KEY))
 
 
 class Engine(BaseModel):
     paths: PathData = Field(default_factory=PathData)
     values: Value = Field(default_factory=Value)
-    flags: Flag = Field(default_factory=Flag)
 
 
 class Params(BaseModel, validate_assignment=True):
     stages: dict[str, Stage] = Field(default_factory=dict)
     engine: Engine = Field(default_factory=Engine)
 
     @classmethod
```

### Comparing `ddeutil_io-0.1.6/src/ddeutil/io/register.py` & `ddeutil_io-0.1.7/src/ddeutil/io/register.py`

 * *Files 3% similar despite different names*

```diff
@@ -482,22 +482,14 @@
 
         if upper_bound is not None:
             for _, data in filter(
                 lambda x: x[1]["parse"] < upper_bound,
                 rs.items(),
             ):
                 _file: str = data["file"]
-                if self.params.engine.flags.archive:
-                    _ac_path: str = (
-                        f"{stage.lower()}_{self.updt:%Y%m%d%H%M%S}_{_file}"
-                    )
-                    loading.move(
-                        _file,
-                        dest=self.params.engine.paths.archive / _ac_path,
-                    )
                 rm(loading.path / _file)
 
     def deploy(self, stop: Optional[str] = None) -> Register:
         """Deploy data that move from base to final stage.
 
         :param stop: A stage name for stop when move config from base stage
             to final stage.
@@ -530,19 +522,87 @@
             open_file_stg=self.loader_stg,
         )
 
         # Remove all files from the stage.
         data: StageFiles
         for _, data in self.__stage_files(_stage, loading).items():
             _file: str = data["file"]
-            if self.params.engine.flags.archive:
+            rm(loading.path / _file)
+
+
+class FullRegister(Register):
+    """Full register that implement archiving step on base Register."""
+
+    def purge(self, stage: Optional[str] = None) -> None:
+        """Purge configuration files that match with any rules in the stage
+        setting.
+        """
+        _stage: str = stage or self.stage
+        if not (_rules := self.params.get_stage(_stage).rules):
+            return
+        loading: ConfFl = ConfFl(
+            path=self.params.engine.paths.data / stage,
+            compress=_rules.compress,
+            open_file=self.loader,
+            open_file_stg=self.loader_stg,
+        )
+        rs: dict[int, StageFiles] = self.__stage_files(_stage, loading)
+        max_file: FormatterGroup = max(
+            rs.items(),
+            key=lambda x: (x[1]["parse"],),
+        )[1]["parse"]
+
+        upper_bound: Optional[FormatterGroup] = None
+        if _rtt_ts := _rules.timestamp:
+            upper_bound = max_file.adjust(
+                {"timestamp": relativedelta(**_rtt_ts)}
+            )
+
+        if upper_bound is not None:
+            for _, data in filter(
+                lambda x: x[1]["parse"] < upper_bound,
+                rs.items(),
+            ):
+                _file: str = data["file"]
+                # NOTE: Archive step
                 _ac_path: str = (
-                    f"{_stage.lower()}_{self.updt:%Y%m%d%H%M%S}_{_file}"
+                    f"{stage.lower()}_{self.updt:%Y%m%d%H%M%S}_{_file}"
                 )
                 loading.move(
                     _file,
-                    dest=self.params.engine.paths.archive / _ac_path,
+                    dest=self.params.engine.paths.data / ".archive" / _ac_path,
                 )
+                rm(loading.path / _file)
+
+    def remove(self, stage: Optional[str] = None) -> None:
+        """Remove config file from the stage storage.
+
+        :param stage: a stage value that want to remove.
+        :type stage: Optional[str]
+        """
+        _stage: str = stage or self.stage
+        assert (
+            _stage != "base"
+        ), "The remove method can not process on the 'base' stage."
+        loading: ConfFl = ConfFl(
+            path=self.params.engine.paths.data / _stage,
+            open_file=self.loader,
+            open_file_stg=self.loader_stg,
+        )
+
+        # NOTE: Remove all files from the stage.
+        data: StageFiles
+        for _, data in self.__stage_files(_stage, loading).items():
+            _file: str = data["file"]
+            # NOTE: Archive step
+            _ac_path: str = f"{_stage.lower()}_{self.updt:%Y%m%d%H%M%S}_{_file}"
+            loading.move(
+                _file,
+                dest=self.params.engine.paths / ".archive" / _ac_path,
+            )
             rm(loading.path / _file)
 
 
-__all__ = ("Register",)
+__all__ = (
+    "Register",
+    "FullRegister",
+)
```

### Comparing `ddeutil_io-0.1.6/src/ddeutil/io/utils.py` & `ddeutil_io-0.1.7/src/ddeutil/io/utils.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.6/src/ddeutil_io.egg-info/PKG-INFO` & `ddeutil_io-0.1.7/src/ddeutil_io.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddeutil-io
-Version: 0.1.6
+Version: 0.1.7
 Summary: Data Developer & Engineer IO Utility Objects
 Author-email: ddeutils <korawich.anu@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/korawica/ddeutil-io/
 Project-URL: Source Code, https://github.com/korawica/ddeutil-io/
 Keywords: data,config,utility
 Classifier: Topic :: Utilities
```

### Comparing `ddeutil_io-0.1.6/src/ddeutil_io.egg-info/SOURCES.txt` & `ddeutil_io-0.1.7/src/ddeutil_io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.6/tests/test_base_csv.py` & `ddeutil_io-0.1.7/tests/test_base_csv.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.6/tests/test_base_dir.py` & `ddeutil_io-0.1.7/tests/test_base_dir.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.6/tests/test_base_env.py` & `ddeutil_io-0.1.7/tests/test_base_env.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.6/tests/test_base_file.py` & `ddeutil_io-0.1.7/tests/test_base_file.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.6/tests/test_base_yaml.py` & `ddeutil_io-0.1.7/tests/test_base_yaml.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,25 +101,27 @@
             sub_key:
                 key01: 'test ${DEMO_ENV_VALUE} value'
                 key02: $1 This is escape with number
                 key03: $$ESCAPE This is escape with $
                 key04: ['i1', 'i2', '${DEMO_ENV_VALUE}']
                 key05: ${DEMO_ENV_VALUE_EMPTY:default}
                 key06: $${DEMO_ENV_VALUE}
+                key07: This ${DEMO_ENV_VALUE} ${{DEMO_ENV_VALUE}}
         """
         ).strip()
         self.yaml_data: dict = {
             "main_key": {
                 "sub_key": {
                     "key01": "test demo value",
                     "key02": "$1 This is escape with number",
                     "key03": "$ESCAPE This is escape with $",
                     "key04": ["i1", "i2", "demo"],
                     "key05": "default",
                     "key06": "${DEMO_ENV_VALUE}",
+                    "key07": "This demo ${{DEMO_ENV_VALUE}}",
                 }
             }
         }
 
     def test_read_yaml_file_with_safe_mode(self):
         yaml_path: str = f"{self.root_path}/test_read_file_env.yaml"
 
@@ -150,14 +152,15 @@
                     "sub_key": {
                         "key01": "test demo!! value",
                         "key02": "$1 This is escape with number",
                         "key03": "$ESCAPE This is escape with $",
                         "key04": ["i1", "i2", "demo!!"],
                         "key05": "default!!",
                         "key06": "${DEMO_ENV_VALUE}",
+                        "key07": "This demo!! ${{DEMO_ENV_VALUE}}",
                     }
                 }
             },
             data,
         )
 
         os.remove(yaml_path)
@@ -183,14 +186,15 @@
                     "sub_key": {
                         "key01": "test P%40ssW0rd value",
                         "key02": "$1 This is escape with number",
                         "key03": "$ESCAPE This is escape with $",
                         "key04": ["i1", "i2", "P%40ssW0rd"],
                         "key05": "default",
                         "key06": "${DEMO_ENV_VALUE}",
+                        "key07": "This P%40ssW0rd ${{DEMO_ENV_VALUE}}",
                     }
                 }
             },
             data,
         )
 
         os.remove(yaml_path)
```

### Comparing `ddeutil_io-0.1.6/tests/test_config_file.py` & `ddeutil_io-0.1.7/tests/test_config_file.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.6/tests/test_config_sqlite.py` & `ddeutil_io-0.1.7/tests/test_config_sqlite.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.6/tests/test_param.py` & `ddeutil_io-0.1.7/tests/test_param.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,32 +14,29 @@
 
 
 def test_model_path_data():
     p = md.PathData.model_validate(
         {
             "data": Path("."),
             "conf": Path("."),
-            "archive": Path("."),
         }
     )
 
     assert {
         "data": Path("."),
         "conf": Path("."),
-        "archive": Path("."),
         "root": Path("."),
     } == p.model_dump()
 
 
 def test_model_path_data_with_root():
     p = md.PathData.model_validate({"root": "./src/"})
     assert {
         "data": Path("./src/data"),
         "conf": Path("./src/conf"),
-        "archive": Path("./src/.archive"),
         "root": Path("./src/"),
     } == p.model_dump()
 
 
 def test_model_rule_data():
     assert {
         "timestamp": {},
@@ -120,18 +117,14 @@
             },
         },
         "engine": {
             "values": {
                 "dt_fmt": "%Y-%m-%d %H:%M:%S",
                 "excluded": (VERSION_KEY, UPDATE_KEY),
             },
-            "flags": {
-                "archive": False,
-            },
             "paths": {
-                "archive": Path(".archive"),
                 "conf": Path("conf"),
                 "data": Path("data"),
                 "root": Path("."),
             },
         },
     } == params.model_dump()
```

### Comparing `ddeutil_io-0.1.6/tests/test_register.py` & `ddeutil_io-0.1.7/tests/test_register.py`

 * *Files identical despite different names*

### Comparing `ddeutil_io-0.1.6/tests/test_register_deploy.py` & `ddeutil_io-0.1.7/tests/test_register_deploy.py`

 * *Files identical despite different names*

