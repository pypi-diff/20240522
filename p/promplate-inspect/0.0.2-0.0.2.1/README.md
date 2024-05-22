# Comparing `tmp/promplate_inspect-0.0.2.tar.gz` & `tmp/promplate_inspect-0.0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promplate_inspect-0.0.2.tar", last modified: Sun Apr 14 17:02:44 2024, max compression
+gzip compressed data, was "promplate_inspect-0.0.2.1.tar", last modified: Wed May 22 05:44:10 2024, max compression
```

## Comparing `promplate_inspect-0.0.2.tar` & `promplate_inspect-0.0.2.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     2221 2024-04-14 16:45:34.850684 promplate_inspect-0.0.2/README.md
--rw-r--r--   0        0        0      723 2024-04-14 17:02:44.242028 promplate_inspect-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3544 2024-04-14 16:58:09.907096 promplate_inspect-0.0.2/src/promplate_inspect.py
--rw-r--r--   0        0        0     2455 1970-01-01 00:00:00.000000 promplate_inspect-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2221 2024-04-14 16:45:34.850684 promplate_inspect-0.0.2.1/README.md
+-rw-r--r--   0        0        0      782 2024-05-22 05:44:10.610400 promplate_inspect-0.0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3593 2024-05-22 05:44:06.198006 promplate_inspect-0.0.2.1/src/promplate_inspect.py
+-rw-r--r--   0        0        0      414 2024-04-19 10:41:00.567018 promplate_inspect-0.0.2.1/tests/test_template.py
+-rw-r--r--   0        0        0     2457 1970-01-01 00:00:00.000000 promplate_inspect-0.0.2.1/PKG-INFO
```

### Comparing `promplate_inspect-0.0.2/README.md` & `promplate_inspect-0.0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `promplate_inspect-0.0.2/pyproject.toml` & `promplate_inspect-0.0.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "promplate-inspect"
-version = "0.0.2"
+version = "0.0.2.1"
 description = "[WIP] Inspect a promplate.Template to get its signatures"
 authors = [
     { name = "Muspi Merol", email = "me@promplate.dev" },
 ]
 dependencies = [
     "promplate>=0.3.3.1.post1,<0.4",
 ]
@@ -24,16 +24,20 @@
 distribution = true
 
 [tool.pdm.dev-dependencies]
 dev = [
     "isort>=5.13.2",
     "black>=24.4.0",
     "ruff>=0.3.7",
+    "pytest>=8.1.1",
 ]
 
+[tool.pdm.scripts]
+test = "pytest"
+
 [tool.pdm.scripts.fmt]
 composite = [
     "ruff check --fix --exit-zero",
     "isort .",
     "black .",
 ]
```

### Comparing `promplate_inspect-0.0.2/src/promplate_inspect.py` & `promplate_inspect-0.0.2.1/src/promplate_inspect.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,16 @@
 
 def find_input_variables_in_template(template: Union[Template, str], exclude_builtins=True) -> Set[str]:
     text = template if isinstance(template, str) else template.text
 
     tokens = []
 
     for token in split_template_tokens(text):
+        if token is None:
+            continue
         token = token.strip()
         if (
             (token.startswith("{{") and token.endswith("}}"))
             or (token.startswith("{#") and token.endswith("#}"))
             or (token.startswith("{%") and token.endswith("%}") and token[2:].strip().split(" ", 1)[0] in {"if", "for", "while", "elif", "else", "endif", "endfor", "endwhile"})
         ):
             tokens.append(token if token[-3] != "-" else f"{token[:-3]}{token[-2:]}")
```

### Comparing `promplate_inspect-0.0.2/PKG-INFO` & `promplate_inspect-0.0.2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promplate-inspect
-Version: 0.0.2
+Version: 0.0.2.1
 Summary: [WIP] Inspect a promplate.Template to get its signatures
 Author-Email: Muspi Merol <me@promplate.dev>
 License: MIT
 Requires-Python: <3.13,>=3.8
 Requires-Dist: promplate<0.4,>=0.3.3.1.post1
 Description-Content-Type: text/markdown
```

