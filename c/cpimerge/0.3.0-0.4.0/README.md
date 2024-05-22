# Comparing `tmp/cpimerge-0.3.0.tar.gz` & `tmp/cpimerge-0.4.0.tar.gz`

## Comparing `cpimerge-0.3.0.tar` & `cpimerge-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.3.0/cpimerge/__init__.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 cpimerge-0.3.0/cpimerge/__main__.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 cpimerge-0.3.0/cpimerge/backup.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 cpimerge-0.3.0/cpimerge/config.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 cpimerge-0.3.0/cpimerge/descriptions.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 cpimerge-0.3.0/cpimerge/exclusions.py
--rw-r--r--   0        0        0    12170 2020-02-02 00:00:00.000000 cpimerge-0.3.0/cpimerge/gui.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 cpimerge-0.3.0/cpimerge/ical.py
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 cpimerge-0.3.0/cpimerge/load.py
--rw-r--r--   0        0        0     5990 2020-02-02 00:00:00.000000 cpimerge-0.3.0/cpimerge/merge.py
--rw-r--r--   0        0        0     3117 2020-02-02 00:00:00.000000 cpimerge-0.3.0/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cpimerge-0.3.0/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.3.0/README.md
--rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 cpimerge-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cpimerge-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.4.0/cpimerge/__init__.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 cpimerge-0.4.0/cpimerge/__main__.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 cpimerge-0.4.0/cpimerge/config.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 cpimerge-0.4.0/cpimerge/descriptions.py
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 cpimerge-0.4.0/cpimerge/exclusions.py
+-rw-r--r--   0        0        0    18593 2020-02-02 00:00:00.000000 cpimerge-0.4.0/cpimerge/gui.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 cpimerge-0.4.0/cpimerge/ical.py
+-rw-r--r--   0        0        0     3532 2020-02-02 00:00:00.000000 cpimerge-0.4.0/cpimerge/load.py
+-rw-r--r--   0        0        0     4910 2020-02-02 00:00:00.000000 cpimerge-0.4.0/cpimerge/merge.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 cpimerge-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 cpimerge-0.4.0/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpimerge-0.4.0/README.md
+-rw-r--r--   0        0        0      601 2020-02-02 00:00:00.000000 cpimerge-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 cpimerge-0.4.0/PKG-INFO
```

### Comparing `cpimerge-0.3.0/cpimerge/config.py` & `cpimerge-0.4.0/cpimerge/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,14 +9,20 @@
 
 # Get configuration file directory (per-OS)
 def get_appdir():
     config_dir = user_data_dir(APP_NAME, APP_AUTHOR)
     os.makedirs(config_dir, exist_ok=True)
     return os.path.join(config_dir, 'config.json')
 
+# Get save file directory (per-OS)
+def get_outdir():
+    config_dir = user_data_dir(APP_NAME, APP_AUTHOR)
+    os.makedirs(config_dir, exist_ok=True)
+    return os.path.join(config_dir, 'out.ics')
+
 # Load configuration from file
 def load_config(config_path):
     try:
         if os.path.exists(config_path):
             with open(config_path, 'r') as f:
                 return json.load(f)
         else:
```

### Comparing `cpimerge-0.3.0/cpimerge/exclusions.py` & `cpimerge-0.4.0/cpimerge/exclusions.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,19 +8,23 @@
             return [line.strip() for line in f]
     except Exception as e:
         messagebox.showerror("Error", f"Failed to load exclusions file: {file_path}\n{e}")
         return []
 
 # Filter events based on exclusions
 def filter_exclusions(events, exclusions, output_text):
+    count = 0;
     filtered_events = set()
     if exclusions:
-        output_text.insert(tk.END, "Excluding:\n")
+        output_text.insert(tk.END, "Excluded:\n\n")
     for event in events:
         if not any(excl.lower() in event[0].lower() for excl in exclusions):
             filtered_events.add(event)
         else:
             if exclusions:
+                count += 1
                 output_text.insert(tk.END, f"  - {event[0]} on {event[1].date()}\n")
+    if count == 0:
+            output_text.insert(tk.END, f"  - None\n")
     if exclusions:
         output_text.insert(tk.END, "\n")
     return filtered_events
```

### Comparing `cpimerge-0.3.0/cpimerge/ical.py` & `cpimerge-0.4.0/cpimerge/ical.py`

 * *Files identical despite different names*

### Comparing `cpimerge-0.3.0/.gitignore` & `cpimerge-0.4.0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -157,8 +157,7 @@
 #  be found at https://github.com/github/gitignore/blob/main/Global/JetBrains.gitignore
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 # Test files
 tests/
-cpimerge/graph.py
```

### Comparing `cpimerge-0.3.0/LICENSE` & `cpimerge-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cpimerge-0.3.0/pyproject.toml` & `cpimerge-0.4.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cpimerge"
-version = "0.3.0"
+version = "0.4.0"
 dependencies = [
   "icalendar",
   "appdirs",
 ]
 authors = [
   { name="Kirk Coombs", email="cpimerge@coombscloud.com" },
 ]
```

