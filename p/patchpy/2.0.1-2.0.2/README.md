# Comparing `tmp/patchpy-2.0.1.tar.gz` & `tmp/patchpy-2.0.2.tar.gz`

## Comparing `patchpy-2.0.1.tar` & `patchpy-2.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 patchpy-2.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 patchpy-2.0.1/.python-version
--rw-r--r--   0        0        0    16031 2020-02-02 00:00:00.000000 patchpy-2.0.1/patchpy.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 patchpy-2.0.1/requirements-dev.lock
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 patchpy-2.0.1/requirements.lock
--rw-r--r--   0        0        0     5203 2020-02-02 00:00:00.000000 patchpy-2.0.1/test_patchpy.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 patchpy-2.0.1/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 patchpy-2.0.1/LICENSE.txt
--rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 patchpy-2.0.1/README.md
--rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 patchpy-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 patchpy-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 patchpy-2.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 patchpy-2.0.2/.python-version
+-rw-r--r--   0        0        0    15936 2020-02-02 00:00:00.000000 patchpy-2.0.2/patchpy.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 patchpy-2.0.2/requirements-dev.lock
+-rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 patchpy-2.0.2/requirements.lock
+-rw-r--r--   0        0        0     6027 2020-02-02 00:00:00.000000 patchpy-2.0.2/test_patchpy.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 patchpy-2.0.2/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 patchpy-2.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     2087 2020-02-02 00:00:00.000000 patchpy-2.0.2/README.md
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 patchpy-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2420 2020-02-02 00:00:00.000000 patchpy-2.0.2/PKG-INFO
```

### Comparing `patchpy-2.0.1/.pre-commit-config.yaml` & `patchpy-2.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `patchpy-2.0.1/patchpy.py` & `patchpy-2.0.2/patchpy.py`

 * *Files 3% similar despite different names*

```diff
@@ -192,16 +192,14 @@
             root_path / Path(*Path(self.source).parts[strip:]) if self.source else None
         )
         target_path = (
             root_path / Path(*Path(self.target).parts[strip:]) if self.target else None
         )
         if source_path and not source_path.exists():
             raise PatchPyError(f'Source file {source_path} does not exist')
-        if target_path and not target_path.exists():
-            raise PatchPyError(f'Target file {target_path} does not exist')
         if not self.source and not self.target:
             return
         if self.source and not self.target:
             os.unlink(source_path)
             return
         if not self.source and self.target:
             for hunk in self.hunks:
@@ -269,17 +267,17 @@
         source = next(lines).removeprefix('--- ')
         if not lines or not lines.peek().startswith('+++ '):
             raise PatchPyError(f'Invalid patch header: {line}')
         target = next(lines).removeprefix('+++ ')
         source = cls._decode_path(source)
         target = cls._decode_path(target)
         kind = ModificationKind.REGULAR
-        if source.startswith('a/') and target.startswith('b/'):
-            source = source.removeprefix('a/')
-            target = target.removeprefix('b/')
+        if header and header[0].startswith('diff --git'):
+            source = source.removeprefix('a/') if source else None
+            target = target.removeprefix('b/') if target else None
             kind = ModificationKind.GIT
         hunks = []
         while lines and lines.peek().startswith('@@ '):
             hunks.append(Hunk._parse(lines))
         return cls(kind=kind, header=header, source=source, target=target, hunks=hunks)
 
     @staticmethod
```

### Comparing `patchpy-2.0.1/requirements-dev.lock` & `patchpy-2.0.2/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `patchpy-2.0.1/test_patchpy.py` & `patchpy-2.0.2/test_patchpy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 import pytest
 from pathlib import Path
 import tempfile
 
 from patchpy import Hunk, FileModification, DiffFile, PatchPyError, ModificationKind
 
 # Sample diff for testing
-sample_diff = """--- a/sample.txt
+sample_diff = """diff --git a/sample.txt b/sample.txt
+--- a/sample.txt
 +++ b/sample.txt
 @@ -1,3 +1,4 @@
  Line 1
  Line 2
  Line 3
 +Line 4
 """
 
 # Sample diff with multiple hunks
-sample_diff_multi_hunk = """--- a/sample.txt
+sample_diff_multi_hunk = """diff --git a/sample.txt b/sample.txt
+--- a/sample.txt
 +++ b/sample.txt
 @@ -1,3 +1,4 @@
  Line 1
  Line 2
  Line 3
 +Line 4
 @@ -5,3 +6,4 @@
@@ -49,35 +51,37 @@
  Line 2
  Line 3
 +Line 4
 """
 
 
 # Sample invalid diff
-sample_invalid_diff = """--- a/sample.txt
+sample_invalid_diff = """diff --git a/sample.txt b/sample.txt
+--- a/sample.txt
 +++ b/sample.txt
 @@ -1,3 +1,4 @@
  Line 1
  Line 2
  Line 3
  Line 4
 """
 
-sample_diff_with_escaping_path = """--- "foo/../../sample.txt
+sample_diff_with_escaping_path = """diff --git "foo/../../sample.txt" "bar/../../sample.txt"
+--- "foo/../../sample.txt
 +++ "bar/../../sample.txt
 @@ -1,3 +1,4 @@
  Line 1
  Line 2
  Line 3
 +Line 4
 """
 
 
 def test_hunk_parsing():
-    hunk = Hunk.parse(''.join(sample_diff.splitlines(keepends=True)[2:]))
+    hunk = Hunk.parse('@@ ' + sample_diff.split('@@ ', 1)[1])
     assert hunk.original_start == 1
     assert hunk.original_length == 3
     assert hunk.new_start == 1
     assert hunk.new_length == 4
     assert hunk.original_lines == ['Line 1\n', 'Line 2\n', 'Line 3\n']
     assert hunk.new_lines == ['Line 1\n', 'Line 2\n', 'Line 3\n', 'Line 4\n']
 
@@ -118,15 +122,16 @@
 
 
 def test_diff_file_reversed():
     diff_file = DiffFile.from_string(sample_diff)
     reversed_diff = diff_file.reversed()
     assert (
         reversed_diff.to_string()
-        == """--- a/sample.txt
+        == """diff --git a/sample.txt b/sample.txt
+--- a/sample.txt
 +++ b/sample.txt
 @@ -1,4 +1,3 @@
  Line 1
  Line 2
  Line 3
 -Line 4
 """
@@ -197,7 +202,31 @@
         diff_file.reversed().apply(root=tempdir)
         assert sample_path.read_text() == 'Line 1\nLine 2\nLine 3\n'
 
 
 def test_apply_with_escaping_path():
     with pytest.raises(PatchPyError):
         DiffFile.from_string(sample_diff_with_escaping_path).validate()
+
+
+def test_diff_with_empty_source():
+    diff_file = DiffFile.from_string(
+        """diff --git a/sample.txt b/sample.txt
+--- /dev/null
++++ b/sample.txt
+@@ -0,0 +1,4 @@
++Line 1
++Line 2
++Line 3
++Line 4
+"""
+    )
+    assert len(diff_file.modifications) == 1
+    mod = diff_file.modifications[0]
+    assert mod.source is None
+    assert mod.target == 'sample.txt'
+    assert len(mod.hunks) == 1
+    # Apply the diff
+    with tempfile.TemporaryDirectory() as tempdir:
+        diff_file.apply(root=tempdir)
+        sample_path = Path(tempdir) / 'sample.txt'
+        assert sample_path.read_text() == 'Line 1\nLine 2\nLine 3\nLine 4\n'
```

### Comparing `patchpy-2.0.1/LICENSE.txt` & `patchpy-2.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `patchpy-2.0.1/README.md` & `patchpy-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `patchpy-2.0.1/pyproject.toml` & `patchpy-2.0.2/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "patchpy"
-version = "2.0.1"
+version = "2.0.2"
 description = "A modern Python library for patch file parsing (diff file parsing)"
 authors = [
     { name = "Matthew D. Scholefield", email = "matthew331199@gmail.com" },
 ]
 dependencies = ["more-itertools>=10.2.0"]
 readme = "README.md"
 requires-python = ">= 3.9"
```

### Comparing `patchpy-2.0.1/PKG-INFO` & `patchpy-2.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: patchpy
-Version: 2.0.1
+Version: 2.0.2
 Summary: A modern Python library for patch file parsing (diff file parsing)
 Author-email: "Matthew D. Scholefield" <matthew331199@gmail.com>
 License: MIT
 License-File: LICENSE.txt
 Requires-Python: >=3.9
 Requires-Dist: more-itertools>=10.2.0
 Description-Content-Type: text/markdown
```

