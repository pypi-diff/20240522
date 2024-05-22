# Comparing `tmp/dotpkg-0.1.0.tar.gz` & `tmp/dotpkg-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotpkg-0.1.0.tar", last modified: Wed Aug 23 17:04:05 2023, max compression
+gzip compressed data, was "dotpkg-0.2.0.tar", last modified: Wed May 22 15:32:56 2024, max compression
```

## Comparing `dotpkg-0.1.0.tar` & `dotpkg-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 17:04:05.872017 dotpkg-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (999)     1061 2023-08-23 17:03:56.000000 dotpkg-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (999)     4512 2023-08-23 17:04:05.872017 dotpkg-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     2918 2023-08-23 17:03:56.000000 dotpkg-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 17:04:05.868018 dotpkg-0.1.0/dotpkg/
--rw-r--r--   0 runner    (1001) docker     (999)     1646 2023-08-23 17:03:56.000000 dotpkg-0.1.0/dotpkg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)       60 2023-08-23 17:03:56.000000 dotpkg-0.1.0/dotpkg/__main__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1716 2023-08-23 17:03:56.000000 dotpkg-0.1.0/dotpkg/commands.py
--rw-r--r--   0 runner    (1001) docker     (999)      357 2023-08-23 17:03:56.000000 dotpkg-0.1.0/dotpkg/constants.py
--rw-r--r--   0 runner    (1001) docker     (999)    10841 2023-08-23 17:03:56.000000 dotpkg-0.1.0/dotpkg/install.py
--rw-r--r--   0 runner    (1001) docker     (999)     2660 2023-08-23 17:03:56.000000 dotpkg-0.1.0/dotpkg/manifest.py
--rw-r--r--   0 runner    (1001) docker     (999)      154 2023-08-23 17:03:56.000000 dotpkg-0.1.0/dotpkg/options.py
--rw-r--r--   0 runner    (1001) docker     (999)      910 2023-08-23 17:03:56.000000 dotpkg-0.1.0/dotpkg/resolve.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 17:04:05.872017 dotpkg-0.1.0/dotpkg/utils/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-23 17:03:56.000000 dotpkg-0.1.0/dotpkg/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1444 2023-08-23 17:03:56.000000 dotpkg-0.1.0/dotpkg/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (999)      550 2023-08-23 17:03:56.000000 dotpkg-0.1.0/dotpkg/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (999)      819 2023-08-23 17:03:56.000000 dotpkg-0.1.0/dotpkg/utils/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-23 17:04:05.868018 dotpkg-0.1.0/dotpkg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     4512 2023-08-23 17:04:05.000000 dotpkg-0.1.0/dotpkg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      424 2023-08-23 17:04:05.000000 dotpkg-0.1.0/dotpkg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-23 17:04:05.000000 dotpkg-0.1.0/dotpkg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       39 2023-08-23 17:04:05.000000 dotpkg-0.1.0/dotpkg.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)       24 2023-08-23 17:04:05.000000 dotpkg-0.1.0/dotpkg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (999)      584 2023-08-23 17:03:56.000000 dotpkg-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-23 17:04:05.872017 dotpkg-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:32:56.116786 dotpkg-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-22 15:32:52.000000 dotpkg-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-22 15:32:56.116786 dotpkg-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-05-22 15:32:52.000000 dotpkg-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:32:56.112786 dotpkg-0.2.0/dotpkg/
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-22 15:32:52.000000 dotpkg-0.2.0/dotpkg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 15:32:52.000000 dotpkg-0.2.0/dotpkg/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-22 15:32:52.000000 dotpkg-0.2.0/dotpkg/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-22 15:32:52.000000 dotpkg-0.2.0/dotpkg/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-22 15:32:52.000000 dotpkg-0.2.0/dotpkg/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13500 2024-05-22 15:32:52.000000 dotpkg-0.2.0/dotpkg/install.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:32:56.116786 dotpkg-0.2.0/dotpkg/manifest/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:32:52.000000 dotpkg-0.2.0/dotpkg/manifest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-22 15:32:52.000000 dotpkg-0.2.0/dotpkg/manifest/alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7288 2024-05-22 15:32:52.000000 dotpkg-0.2.0/dotpkg/manifest/dotpkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-22 15:32:52.000000 dotpkg-0.2.0/dotpkg/manifest/installs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-22 15:32:52.000000 dotpkg-0.2.0/dotpkg/manifest/installs_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-22 15:32:52.000000 dotpkg-0.2.0/dotpkg/manifest/installs_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-22 15:32:52.000000 dotpkg-0.2.0/dotpkg/manifest/installs_v3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-05-22 15:32:52.000000 dotpkg-0.2.0/dotpkg/manifest/installs_v4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-22 15:32:52.000000 dotpkg-0.2.0/dotpkg/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-22 15:32:52.000000 dotpkg-0.2.0/dotpkg/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3520 2024-05-22 15:32:52.000000 dotpkg-0.2.0/dotpkg/resolve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:32:56.116786 dotpkg-0.2.0/dotpkg/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:32:52.000000 dotpkg-0.2.0/dotpkg/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-05-22 15:32:52.000000 dotpkg-0.2.0/dotpkg/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-22 15:32:52.000000 dotpkg-0.2.0/dotpkg/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-22 15:32:52.000000 dotpkg-0.2.0/dotpkg/utils/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:32:56.116786 dotpkg-0.2.0/dotpkg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4503 2024-05-22 15:32:56.000000 dotpkg-0.2.0/dotpkg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-22 15:32:56.000000 dotpkg-0.2.0/dotpkg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:32:56.000000 dotpkg-0.2.0/dotpkg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-22 15:32:56.000000 dotpkg-0.2.0/dotpkg.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:32:56.000000 dotpkg-0.2.0/dotpkg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-22 15:32:52.000000 dotpkg-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:32:56.116786 dotpkg-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:32:56.116786 dotpkg-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:32:52.000000 dotpkg-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-22 15:32:52.000000 dotpkg-0.2.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-22 15:32:52.000000 dotpkg-0.2.0/tests/test_copy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-22 15:32:52.000000 dotpkg-0.2.0/tests/test_install_manifest_upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-22 15:32:52.000000 dotpkg-0.2.0/tests/test_minimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-22 15:32:52.000000 dotpkg-0.2.0/tests/test_target_dir.py
```

### Comparing `dotpkg-0.1.0/LICENSE` & `dotpkg-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dotpkg-0.1.0/PKG-INFO` & `dotpkg-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotpkg
-Version: 0.1.0
+Version: 0.2.0
 Summary: Package manager for your dotfiles
 License: MIT License
         
         Copyright (c) 2022 fwcd
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -24,35 +24,35 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/fwcd/dotpkg
 Project-URL: Repository, https://github.com/fwcd/dotpkg
 Keywords: package-manager,dotfiles
 Classifier: Topic :: Utilities
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Dotpkg
 
 [![PyPI](https://img.shields.io/pypi/v/dotpkg)](https://pypi.org/project/dotpkg)
-[![Typecheck](https://github.com/fwcd/dotpkg/actions/workflows/typecheck.yml/badge.svg)](https://github.com/fwcd/dotpkg/actions/workflows/typecheck.yml)
+[![Check](https://github.com/fwcd/dotpkg/actions/workflows/check.yml/badge.svg)](https://github.com/fwcd/dotpkg/actions/workflows/check.yml)
 
 A package manager for your dotfiles.
 
 ## Why Dotpkg?
 
-- **Lightweight**: Pure Python 3.9 with no dependencies
+- **Lightweight**: Pure Python 3.10 with no dependencies
 - **JSON-configurable**: Easy to write, includes a schema for code completion
 - **Cross-platform**: Runs on Linux, macOS and Windows
 - **Flexible**: Configurable target locations, ignore lists, rename rules and more
 
 ## Usage
 
-First make sure to have Python 3.9+ installed. To create a dotfile package, set up a folder with the following layout (the top-level folder is assumed to be some folder, e.g. a Git repo, where you store all of your dotfiles):
+First make sure to have Python 3.10+ installed. To create a dotfile package, set up a folder with the following layout (the top-level folder is assumed to be some folder, e.g. a Git repo, where you store all of your dotfiles):
 
 ```
 dotfiles
 └─my-package
   ├─dotpkg.json
   ├─.some-dotfile-one
   ├─.some-dotfile-two
```

### Comparing `dotpkg-0.1.0/README.md` & `dotpkg-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Dotpkg
 
 [![PyPI](https://img.shields.io/pypi/v/dotpkg)](https://pypi.org/project/dotpkg)
-[![Typecheck](https://github.com/fwcd/dotpkg/actions/workflows/typecheck.yml/badge.svg)](https://github.com/fwcd/dotpkg/actions/workflows/typecheck.yml)
+[![Check](https://github.com/fwcd/dotpkg/actions/workflows/check.yml/badge.svg)](https://github.com/fwcd/dotpkg/actions/workflows/check.yml)
 
 A package manager for your dotfiles.
 
 ## Why Dotpkg?
 
-- **Lightweight**: Pure Python 3.9 with no dependencies
+- **Lightweight**: Pure Python 3.10 with no dependencies
 - **JSON-configurable**: Easy to write, includes a schema for code completion
 - **Cross-platform**: Runs on Linux, macOS and Windows
 - **Flexible**: Configurable target locations, ignore lists, rename rules and more
 
 ## Usage
 
-First make sure to have Python 3.9+ installed. To create a dotfile package, set up a folder with the following layout (the top-level folder is assumed to be some folder, e.g. a Git repo, where you store all of your dotfiles):
+First make sure to have Python 3.10+ installed. To create a dotfile package, set up a folder with the following layout (the top-level folder is assumed to be some folder, e.g. a Git repo, where you store all of your dotfiles):
 
 ```
 dotfiles
 └─my-package
   ├─dotpkg.json
   ├─.some-dotfile-one
   ├─.some-dotfile-two
```

### Comparing `dotpkg-0.1.0/dotpkg/install.py` & `dotpkg-0.2.0/dotpkg/install.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,215 +1,257 @@
 from itertools import zip_longest
 from pathlib import Path
-from typing import Callable, Iterable, Any, cast
+from typing import Any, cast
 
-from dotpkg.constants import IGNORED_NAMES, INSTALL_MANIFEST_PATH, INSTALL_MANIFEST_VERSION
-from dotpkg.manifest import manifest_name, find_target_dir, resolve_ignores, resolve_manifest_str
+from dotpkg.constants import INSTALL_MANIFEST_NAME
+from dotpkg.error import InvalidManifestError
+from dotpkg.manifest.alias import CurrentInstallsManifest
+from dotpkg.manifest.dotpkg import DotpkgManifest
+from dotpkg.manifest.installs import InstallsManifest
+from dotpkg.manifest.installs_v1 import InstallsV1Manifest
+from dotpkg.manifest.installs_v2 import InstallsV2Manifest
+from dotpkg.manifest.installs_v3 import InstallsV3Manifest
+from dotpkg.manifest.installs_v4 import InstallsV4Manifest
+from dotpkg.model import Dotpkg
 from dotpkg.options import Options
-from dotpkg.utils.file import file_digest, copy, move, link, touch, remove
+from dotpkg.resolve import find_link_candidates, find_target_dir, resolve_ignores, resolve_manifest_str
+from dotpkg.utils.file import path_digest, copy, move, link, touch, remove
 from dotpkg.utils.log import note, warn
 from dotpkg.utils.prompt import prompt, confirm
 
 import json
 import subprocess
 
 # Installation/uninstallation
 
-def find_link_candidates(src_dir: Path, target_dir: Path, renamer: Callable[[str], str] = lambda name: name) -> Iterable[tuple[Path, Path]]:
-    for src_path in src_dir.iterdir():
-        name = renamer(src_path.name)
-        target_path = target_dir / name
-
-        if name not in IGNORED_NAMES:
-            # We only descend into existing directories that are not Git repos
-            if target_path.exists() and not target_path.is_symlink() and target_path.is_dir() and not (target_path / '.git').exists():
-                yield from find_link_candidates(src_path, target_path)
-            else:
-                yield src_path, target_path
-
 def install_path(src_path: Path, target_path: Path, should_copy: bool, opts: Options):
     if should_copy:
         copy(src_path, target_path, opts)
     else:
-        link(src_path, target_path, opts)
+        link(src_path.resolve(), target_path, opts)
+
+def install_manifest_path(opts: Options) -> Path:
+    return opts.state_dir / INSTALL_MANIFEST_NAME
 
-def read_install_manifest(opts: Options) -> dict[str, Any]:
+def read_install_manifest(opts: Options) -> InstallsManifest:
     try:
-        with open(INSTALL_MANIFEST_PATH, 'r') as f:
-            manifest = json.load(f)
-            version = manifest.get('version', 0)
-            if version < INSTALL_MANIFEST_VERSION:
-                if not confirm(f'An older install manifest with version {version} (current is {INSTALL_MANIFEST_VERSION}) exists at {INSTALL_MANIFEST_PATH}, which may be incompatible with the current version. Should this be used anyway? If no, the old one will be ignored/overwritten.', opts):
-                    manifest['version'] = INSTALL_MANIFEST_VERSION
-                else:
-                    manifest = None
+        path = install_manifest_path(opts)
+        with open(path, 'r') as f:
+            raw_manifest = json.load(f)
+            version = raw_manifest.get('version', 0)
+            match version:
+                case 1: return InstallsV1Manifest.from_dict(raw_manifest)
+                case 2: return InstallsV2Manifest.from_dict(raw_manifest)
+                case 3: return InstallsV3Manifest.from_dict(raw_manifest)
+                case 4: return InstallsV4Manifest.from_dict(raw_manifest)
+                case _: raise InvalidManifestError(f'Invalid manifest version {version}')
     except FileNotFoundError:
-        manifest = None
-    return manifest or {
-        '$schema': 'https://raw.githubusercontent.com/fwcd/dotpkg/main/schemas/installs.schema.json',
-        'version': INSTALL_MANIFEST_VERSION,
-    }
-
-def write_install_manifest(manifest: dict[str, Any], opts: Options):
-    if INSTALL_MANIFEST_PATH.exists():
-        note(f'Updating {INSTALL_MANIFEST_PATH}')
+        return CurrentInstallsManifest()
+
+def write_install_manifest(manifest: InstallsManifest, opts: Options):
+    path = install_manifest_path(opts)
+    if path.exists():
+        note(f'Updating {path}')
     else:
-        print(f'Creating {INSTALL_MANIFEST_PATH}')
+        print(f'Creating {path}')
     if not opts.dry_run:
-        INSTALL_MANIFEST_PATH.parent.mkdir(parents=True, exist_ok=True)
-        with open(INSTALL_MANIFEST_PATH, 'w') as f:
-            json.dump(manifest, f, indent=2)
+        path.parent.mkdir(parents=True, exist_ok=True)
+        with open(path, 'w') as f:
+            json.dump(manifest.to_dict(), f, indent=2)
 
-def run_script(name: str, src_dir: Path, manifest: dict[str, Any], opts: Options):
-    script = manifest.get('scripts', {}).get(name, None)
+def run_script(name: str, pkg: Dotpkg, opts: Options):
+    script = getattr(pkg.manifest.scripts, name)
 
     if script:
         description = f"'{name}' ('{script}')"
         if opts.safe_mode:
             warn(f"Skipping script {description} in safe mode")
         else:
             print(f"Running script {description}...")
             if not opts.dry_run:
-                subprocess.run(script, shell=True, cwd=src_dir, check=True)
+                subprocess.run(script, shell=True, cwd=pkg.path, check=True)
 
-def display_caveats(src_dir: Path, manifest: dict[str, Any], opts: Options):
-    requires = manifest.get('requires', None)
+def display_caveats(manifest: DotpkgManifest):
+    requires = manifest.requires
     if requires == 'logout':
-        warn(f'{manifest_name(src_dir, manifest)} requires logging out and back in to apply!')
+        warn(f'{manifest.name} requires logging out and back in to apply!')
     elif requires == 'reboot':
-        warn(f'{manifest_name(src_dir, manifest)} requires rebooting the computer to apply!')
+        warn(f'{manifest.name} requires rebooting the computer to apply!')
 
-def install(src_dir: Path, manifest: dict[str, Any], opts: Options):
-    target_dir = find_target_dir(manifest)
+def install(pkg: Dotpkg, opts: Options):
+    target_dir = find_target_dir(pkg.manifest, opts)
 
     install_manifest = read_install_manifest(opts)
-    installs = install_manifest.get('installs', {})
-    install_key = str(src_dir)
+    installs = {**install_manifest.installs}
+    install_key = str(pkg.path)
 
     if install_key in installs:
         existing_install = installs[install_key]
-        existing_paths = [Path(path) for path in existing_install.get('paths', [])]
-        existing_target_dir = Path(existing_install.get('targetDir', str(target_dir)))
-        if confirm(f'The dotpkg {install_key} is already installed to {existing_target_dir} and currently targets {target_dir}. Should it be uninstalled first?', opts):
-            uninstall(src_dir, manifest, opts)
+        existing_paths = [Path(path) for path in existing_install.paths] if not isinstance(existing_install, InstallsV1Manifest.InstallsEntry) else []
+        existing_target_dir = Path(existing_install.target_dir or str(target_dir))
+        if confirm(f'The dotpkg {pkg.name} is already installed to {existing_target_dir} and currently targets {target_dir}. Should it be uninstalled first?', opts):
+            uninstall(pkg, opts)
         elif target_dir.resolve() != existing_target_dir.resolve():
             warn('\n'.join([
-                f'This will leave the installed files at the old target dir {existing_target_dir} orphaned, since the install for {install_key} in {INSTALL_MANIFEST_PATH} will be repointed to {target_dir}. These files are affected:',
+                f'This will leave the installed files at the old target dir {existing_target_dir} orphaned, since the install for {install_key} in {install_manifest_path(opts)} will be repointed to {target_dir}. These files are affected:',
                 *[f'  {path}' for path in existing_paths],
             ]))
 
-    run_script('preinstall', src_dir, manifest, opts)
+    run_script('preinstall', pkg, opts)
 
-    scripts_only = manifest.get('isScriptsOnly', False)
+    scripts_only = pkg.manifest.is_scripts_only
     src_paths: list[Path] = []
     installed_paths: list[Path] = []
 
     if not scripts_only:
         target_dir.mkdir(parents=True, exist_ok=True)
 
-        touch_files: list[str] = manifest.get('touchFiles', [])
+        touch_files: list[str] = pkg.manifest.touch_files
         for rel_path in touch_files:
             touch_path = target_dir / rel_path
             touch(touch_path, opts)
 
-        ignores = resolve_ignores(src_dir, manifest)
-        renames = manifest.get('renames', {})
-        should_copy = manifest.get('copy', False)
+        ignores = resolve_ignores(pkg, opts)
+        renames = pkg.manifest.renames
+        should_copy = pkg.manifest.copy
 
         def renamer(name: str) -> str:
             for pat, s in renames.items():
-                name = name.replace(resolve_manifest_str(pat), resolve_manifest_str(s))
+                name = name.replace(resolve_manifest_str(pat, opts), resolve_manifest_str(s, opts))
             return name
 
-        for src_path, target_path in find_link_candidates(src_dir, target_dir, renamer):
+        for src_path, target_path in find_link_candidates(pkg.path, target_dir, renamer):
+            def record_paths():
+                src_paths.append(src_path)
+                installed_paths.append(target_path)
+
             if src_path in ignores:
                 note(f'Ignoring {src_path}')
                 continue
 
             skipped = False
 
             if target_path.is_symlink() or target_path.exists():
                 if should_copy:
-                    if file_digest(target_path) == file_digest(src_path):
+                    legacy_order = install_manifest.version <= 3
+                    if path_digest(target_path, legacy_order=legacy_order) == path_digest(src_path, legacy_order=legacy_order):
                         note(f'Skipping {target_path} (target and src hashes match)')
+                        record_paths()
                         continue
                 else:
                     if target_path.is_symlink() and target_path.resolve() == src_path.resolve():
                         note(f'Skipping {target_path} (already linked)')
+                        record_paths()
                         continue
 
                 def backup():
                     move(target_path, target_path.with_name(f'{target_path.name}.backup'), opts)
                     install_path(src_path, target_path, should_copy, opts)
 
                 def overwrite():
                     remove(target_path, opts)
                     install_path(src_path, target_path, should_copy, opts)
-
+                
                 def skip():
                     note(f'Skipping {target_path}')
                     nonlocal skipped
                     skipped = True
 
+                def theirs():
+                    move(target_path, src_path, opts)
+                    install_path(src_path, target_path, should_copy, opts)
+
                 choices = {
                     'backup': backup,
                     'overwrite': overwrite,
-                    'skip': skip
+                    'skip': skip,
+                    'theirs': theirs,
                 }
 
                 if should_copy:
                     prompt_msg = f"{target_path} exists and is not a copy of the dotpkg's file."
                 else:
+                    # TODO: Add option to view the file e.g. with an editor if its a regular file
+                    #       and show non-dotpkg symlink destination otherwise.
                     prompt_msg = f'{target_path} exists and is not a link into the dotpkg.'
 
-                response = prompt(prompt_msg, sorted(choices.keys()), 'skip', opts)
+                response = prompt(prompt_msg, sorted(choices.keys()), 'backup', opts)
                 choices.get(response, skip)()
                 continue
 
             install_path(src_path, target_path, should_copy, opts)
 
             if not skipped:
-                src_paths.append(src_path)
-                installed_paths.append(target_path)
+                record_paths()
     
-    run_script('install', src_dir, manifest, opts)
-    run_script('postinstall', src_dir, manifest, opts)
+    run_script('install', pkg, opts)
+    run_script('postinstall', pkg, opts)
 
     if opts.update_install_manifest:
-        installs[install_key] = {
-            'targetDir': str(target_dir),
-            'srcPaths': [str(path) for path in src_paths],
-            'paths': [str(path) for path in installed_paths],
-        }
-        install_manifest['installs'] = installs
+        match install_manifest.version:
+            case 1:
+                installs[install_key] = InstallsV1Manifest.InstallsEntry(
+                    target_dir=str(target_dir),
+                )
+            case 2:
+                installs[install_key] = InstallsV2Manifest.InstallsEntry(
+                    target_dir=str(target_dir),
+                    src_paths=[str(path) for path in src_paths],
+                    paths=[str(path) for path in installed_paths],
+                )
+            case 3:
+                installs[install_key] = InstallsV3Manifest.InstallsEntry(
+                    target_dir=str(target_dir),
+                    src_paths=[str(path) for path in src_paths],
+                    paths=[str(path) for path in installed_paths],
+                    checksums=[path_digest(path, legacy_order=True) for path in installed_paths],
+                )
+            case 4:
+                installs[install_key] = InstallsV4Manifest.InstallsEntry(
+                    target_dir=str(target_dir),
+                    src_paths=[str(path) for path in src_paths],
+                    paths=[str(path) for path in installed_paths],
+                    checksums=[path_digest(path) for path in installed_paths],
+                )
+        # The type checker cannot verify that this is the same manifest type. We
+        # might be able to model that with "generics", i.e. type variables but
+        # that would probably require splitting out the majority of this
+        # function into a new one.
+        install_manifest.installs = cast(Any, installs)
         write_install_manifest(install_manifest, opts)
     
-    display_caveats(src_dir, manifest, opts)
+    display_caveats(pkg.manifest)
 
-def uninstall(src_dir: Path, manifest: dict[str, Any], opts: Options):
+def uninstall(pkg: Dotpkg, opts: Options):
     install_manifest = read_install_manifest(opts)
-    installs = install_manifest.get('installs', {})
-    install_key = str(src_dir)
-    install: dict[str, Any] = installs.get(install_key, {})
+    installs = {**install_manifest.installs}
+    install_key = str(pkg.path)
+    install = installs.get(install_key)
 
-    run_script('preuninstall', src_dir, manifest, opts)
-    run_script('uninstall', src_dir, manifest, opts)
+    run_script('preuninstall', pkg, opts)
+    run_script('uninstall', pkg, opts)
 
-    scripts_only = manifest.get('isScriptsOnly', False)
+    scripts_only = pkg.manifest.is_scripts_only
 
     if not scripts_only:
-        target_dir = Path(install['targetDir']) if 'targetDir' in install else find_target_dir(manifest)
-        should_copy = manifest.get('copy', False)
+        target_dir = Path(install.target_dir) if install and install.target_dir else find_target_dir(pkg.manifest, opts)
+        should_copy = pkg.manifest.copy
 
-        if 'paths' in install:
-            paths = zip_longest(map(Path, cast(list[str], install.get('srcPaths', []))), map(Path, install['paths']), fillvalue=None)
+        if install and not isinstance(install, InstallsV1Manifest.InstallsEntry):
+            paths = list(zip_longest(map(Path, install.src_paths), map(Path, install.paths), fillvalue=None))
         else:
-            paths = find_link_candidates(src_dir, target_dir)
+            paths = list(find_link_candidates(pkg.path, target_dir))
+        
+        if install and not isinstance(install, InstallsV1Manifest.InstallsEntry) and not isinstance(install, InstallsV2Manifest.InstallsEntry):
+            checksums = install.checksums
+        else:
+            legacy_order = install_manifest.version <= 3
+            checksums = [path_digest(src_path, legacy_order=legacy_order) if src_path else None for src_path, _ in paths]
 
-        for src_path, target_path in paths:
+        for (src_path, target_path), checksum in zip_longest(paths, checksums):
             if not target_path:
                 note(f'Skipping src path {src_path} (no target path)')
                 continue
 
             # TODO: Instead of just skipping these paths (and uninstalling the package from the install manifest)
             #       we should probably prompt the user (similar to the backup/overwrite options during installation)
             #       for how to proceed.
@@ -219,20 +261,30 @@
                     note(f'Skipping {target_path} (no src path in a copy-package)')
                     continue
 
                 if target_path.is_symlink():
                     note(f'Skipping {target_path} (is a symlink while the package is copy)')
                     continue
 
-                target_hash = file_digest(target_path)
-                src_hash = file_digest(src_path)
-
-                if target_hash != src_hash:
-                    note(f'Skipping {target_path} (target hash {target_hash} != src hash {src_hash})')
+                if not checksum:
+                    warn(f'Skipping {target_path} (missing checksum)')
                     continue
+                
+                if not target_path.exists():
+                    warn(f'Skipping {target_path} (file does not exist)')
+                    continue
+
+                if install_manifest.version >= 4 or not target_path.is_dir():
+                    target_checksum = path_digest(target_path)
+
+                    if target_checksum != checksum:
+                        note(f'Skipping {target_path} (target checksum {target_checksum} != {checksum})')
+                        continue
+                else:
+                    warn(f'Ignoring checksum for {target_path} since the legacy directory hashes (which were generated in non-deterministic order) are unreliable, unfortunately.')
             else:
                 if not target_path.is_symlink():
                     note(f'Skipping {target_path} (not a symlink)')
                     continue
                 
                 if src_path:
                     target_dest = target_path.resolve()
@@ -240,15 +292,19 @@
                     
                     if target_dest != src_dest:
                         note(f'Skipping {target_path} (target dest {target_dest} != src dest {src_dest}, probably not a link into the package)')
                         continue
 
             remove(target_path, opts)
     
-    run_script('postuninstall', src_dir, manifest, opts)
+    run_script('postuninstall', pkg, opts)
 
     if opts.update_install_manifest and install_key in installs:
         del installs[install_key]
-        install_manifest['installs'] = installs
+        # The type checker cannot verify that this is the same manifest type. We
+        # might be able to model that with "generics", i.e. type variables but
+        # that would probably require splitting out the majority of this
+        # function into a new one.
+        install_manifest.installs = cast(Any, installs)
         write_install_manifest(install_manifest, opts)
 
-    display_caveats(src_dir, manifest, opts)
+    display_caveats(pkg.manifest)
```

### Comparing `dotpkg-0.1.0/dotpkg/utils/log.py` & `dotpkg-0.2.0/dotpkg/utils/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 CLEAR_COLOR = '\033[0m'
 
 def message(msg: str, color: str):
     print(f'{color}==> {msg}{CLEAR_COLOR}')
 
 def error(msg: str):
     message(msg, RED_COLOR)
-    sys.exit(1)
 
 def warn(msg: str):
     message(msg, YELLOW_COLOR)
 
 def info(msg: str):
     message(msg, BLUE_COLOR)
```

### Comparing `dotpkg-0.1.0/dotpkg/utils/prompt.py` & `dotpkg-0.2.0/dotpkg/utils/prompt.py`

 * *Files identical despite different names*

### Comparing `dotpkg-0.1.0/dotpkg.egg-info/PKG-INFO` & `dotpkg-0.2.0/dotpkg.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotpkg
-Version: 0.1.0
+Version: 0.2.0
 Summary: Package manager for your dotfiles
 License: MIT License
         
         Copyright (c) 2022 fwcd
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -24,35 +24,35 @@
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://github.com/fwcd/dotpkg
 Project-URL: Repository, https://github.com/fwcd/dotpkg
 Keywords: package-manager,dotfiles
 Classifier: Topic :: Utilities
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Dotpkg
 
 [![PyPI](https://img.shields.io/pypi/v/dotpkg)](https://pypi.org/project/dotpkg)
-[![Typecheck](https://github.com/fwcd/dotpkg/actions/workflows/typecheck.yml/badge.svg)](https://github.com/fwcd/dotpkg/actions/workflows/typecheck.yml)
+[![Check](https://github.com/fwcd/dotpkg/actions/workflows/check.yml/badge.svg)](https://github.com/fwcd/dotpkg/actions/workflows/check.yml)
 
 A package manager for your dotfiles.
 
 ## Why Dotpkg?
 
-- **Lightweight**: Pure Python 3.9 with no dependencies
+- **Lightweight**: Pure Python 3.10 with no dependencies
 - **JSON-configurable**: Easy to write, includes a schema for code completion
 - **Cross-platform**: Runs on Linux, macOS and Windows
 - **Flexible**: Configurable target locations, ignore lists, rename rules and more
 
 ## Usage
 
-First make sure to have Python 3.9+ installed. To create a dotfile package, set up a folder with the following layout (the top-level folder is assumed to be some folder, e.g. a Git repo, where you store all of your dotfiles):
+First make sure to have Python 3.10+ installed. To create a dotfile package, set up a folder with the following layout (the top-level folder is assumed to be some folder, e.g. a Git repo, where you store all of your dotfiles):
 
 ```
 dotfiles
 └─my-package
   ├─dotpkg.json
   ├─.some-dotfile-one
   ├─.some-dotfile-two
```

### Comparing `dotpkg-0.1.0/pyproject.toml` & `dotpkg-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dotpkg"
-version = "0.1.0"
+version = "0.2.0"
 description = "Package manager for your dotfiles"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 license = { file = "LICENSE" }
 classifiers = ["Topic :: Utilities"]
 keywords = ["package-manager", "dotfiles"]
 dependencies = []
 
 [project.urls]
 Homepage = "https://github.com/fwcd/dotpkg"
```

