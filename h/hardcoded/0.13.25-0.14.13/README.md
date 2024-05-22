# Comparing `tmp/hardcoded-0.13.25.tar.gz` & `tmp/hardcoded-0.14.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hardcoded-0.13.25.tar", max compression
+gzip compressed data, was "hardcoded-0.14.13.tar", max compression
```

## Comparing `hardcoded-0.13.25.tar` & `hardcoded-0.14.13.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1871 2023-09-27 09:14:40.293985 hardcoded-0.13.25/README.md
--rw-r--r--   0        0        0     1112 2023-02-20 12:55:16.346319 hardcoded-0.13.25/hardcoded/__init__.py
--rw-r--r--   0        0        0     2477 2023-06-14 06:25:33.929564 hardcoded-0.13.25/hardcoded/cli.py
--rw-r--r--   0        0        0     1396 2024-02-19 13:26:48.977256 hardcoded-0.13.25/hardcoded/git.py
--rw-r--r--   0        0        0    22844 2024-04-30 13:46:06.767741 hardcoded-0.13.25/hardcoded/logic.py
--rw-r--r--   0        0        0      687 2024-04-30 07:21:02.525528 hardcoded-0.13.25/pyproject.toml
--rw-r--r--   0        0        0     2853 1970-01-01 00:00:00.000000 hardcoded-0.13.25/PKG-INFO
+-rw-r--r--   0        0        0     1871 2024-04-20 08:58:50.133334 hardcoded-0.14.13/README.md
+-rw-r--r--   0        0        0     1177 2024-05-21 20:05:41.903335 hardcoded-0.14.13/hardcoded/__init__.py
+-rw-r--r--   0        0        0     2755 2024-05-22 07:07:15.294230 hardcoded-0.14.13/hardcoded/cli.py
+-rw-r--r--   0        0        0     1414 2024-05-21 19:41:50.996478 hardcoded-0.14.13/hardcoded/git.py
+-rw-r--r--   0        0        0    25781 2024-05-22 08:24:07.526500 hardcoded-0.14.13/hardcoded/logic.py
+-rw-r--r--   0        0        0      687 2024-05-22 15:14:00.357138 hardcoded-0.14.13/pyproject.toml
+-rw-r--r--   0        0        0     2853 1970-01-01 00:00:00.000000 hardcoded-0.14.13/PKG-INFO
```

### Comparing `hardcoded-0.13.25/README.md` & `hardcoded-0.14.13/README.md`

 * *Files identical despite different names*

### Comparing `hardcoded-0.13.25/hardcoded/__init__.py` & `hardcoded-0.14.13/hardcoded/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 #!/usr/bin/env python3
 
 import sys
 import inspect
+from pathlib import Path
 
 from .cli import cli
-from .logic import *
+from .logic import NOT_GIVEN, DEFAULT_FILE_NAME, File
 from . import git
 
 # This bit of code is duplicated in logic.py.
 # This is because of the fact that this code looks at itself and finds the path of the file containing the code.
 stack = None
 try:
     stack = inspect.stack()
     this_code_file_path = stack[0].filename
     for frame in stack:
         caller_path = frame.filename
-        if caller_path != this_code_file_path and 'frozen' not in caller_path.lower():
+        if caller_path != this_code_file_path and "frozen" not in caller_path.lower():
             break
 finally:
     del stack
-repo_root = git.find_repo_path(caller_path)
+repo_root = git.find_repo_path(caller_path or ".")
 if repo_root:
     datafile_path = Path(repo_root) / DEFAULT_FILE_NAME
 else:
     datafile_path = NOT_GIVEN
 
 default_file = File(path=datafile_path)
-super(File, default_file).__setattr__('__spec__', __spec__)
-super(File, default_file).__setattr__('cli', cli)
+super(File, default_file).__setattr__("__spec__", __spec__)
+super(File, default_file).__setattr__("cli", cli)
 
 # Hack. This replaces the module "hardcoded" with an instance of the class File.
 # Now you can do this to use the default settings (hardcoded.json, secret, ask if not found):
 # import hardcoded
 # login(hardcoded.password)
 
 sys.modules[__name__] = default_file
```

### Comparing `hardcoded-0.13.25/hardcoded/cli.py` & `hardcoded-0.14.13/hardcoded/cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,63 +1,80 @@
 #!/usr/bin/env python3
 
 import yaml
 
-from hardcoded.logic import *
+from hardcoded.logic import File, _debug
 
 import click
 
+
 @click.command()
-@click.option('--encrypt', is_flag=True, help='Write the data file encrypted, regardless of its previous status.')
-@click.option('--decrypt', is_flag=True, help='Write the data file in plain text, regardless of its previous status.')
-@click.option('--file', help=f'The file to work on. [{File()._x.path}]')
-#@click.option('--import-file', help=f'A file to import as key-values into {File()._x.path}.')
-@click.option('--where', is_flag=True, help=f'Show which file is used.')
-@click.argument('key', required=False)
-def cli(key, encrypt, decrypt, file, where):
+@click.option(
+    "--encrypt",
+    is_flag=True,
+    help="Write the data file encrypted, regardless of its previous status.",
+)
+@click.option(
+    "--decrypt",
+    is_flag=True,
+    help="Write the data file in plain text, regardless of its previous status.",
+)
+@click.option("--file", help=f"The file to work on. [{File()._x.path}]")
+# @click.option('--import-file', help=f'A file to import as key-values into {File()._x.path}.')
+@click.option("--where", is_flag=True, help="Show which file is used.")
+@click.option("-d", "--debug", is_flag=True, help="Turn on debug output.")
+@click.argument("key", required=False)
+def cli(key, encrypt, decrypt, file, where, debug):
+    if debug:
+        _debug.enabled = True
     if encrypt and decrypt:
-        raise ValueError('Please choose one of --encrypt and --decrypt.')
+        raise ValueError("Please choose one of --encrypt and --decrypt.")
     elif encrypt or decrypt:
         secret = encrypt
     else:
         secret = None
     datafile = File(secret=secret, path=file)
 
     if where:
         # TODO: If / when we implement hierarchical overlay files, show info about what is read from / written to which file.
         click.echo(File()._x.path)
         exit()
 
     # TODO: Allow to import from other simple YAML, two-column CSV, INI and .env files.
-    #if import_file:
+    # if import_file:
     #    click.echo('boo')
     #    exit()
 
     if key:
         click.echo(datafile.get(key), err=False, nl=False)
     else:
         data = datafile._x._get_all_decrypted_data()
         data_yaml = yaml.safe_dump(data)
         edited_data_yaml = data_yaml
         while True:
             edited_data_yaml = click.edit(edited_data_yaml)
             try:
-                if edited_data_yaml == None:
-                    click.echo('Data not changed.', err=True)
+                if edited_data_yaml is None:
+                    click.echo("Data not changed.", err=True)
                 else:
                     # Let's fail here if the user messed up the YAML.
                     edited_data = yaml.safe_load(edited_data_yaml)
                     datafile._x._set_all_data(edited_data)
-                    click.echo(f'{datafile._x.path} updated.', err=True)
+                    click.echo(f"{datafile._x.path} updated.", err=True)
                 break
             except yaml.YAMLError as ex:
-                if hasattr(ex, 'problem_mark'):
+                if hasattr(ex, "problem_mark"):
                     mark = ex.problem_mark
-                    click.echo(f'Error in {datafile._x.path} YAML at {mark.line+1}:{mark.column+1}: {ex}', err=True)
+                    click.echo(
+                        f"Error in {datafile._x.path} YAML at {mark.line+1}:{mark.column+1}: {ex}",
+                        err=True,
+                    )
                 else:
-                    click.echo(f'Error in {datafile._x.path} YAML: {ex}', err=True)
-                if not click.confirm('Do you want to try again?', default=True, err=True):
+                    click.echo(f"Error in {datafile._x.path} YAML: {ex}", err=True)
+                if not click.confirm(
+                    "Do you want to try again?", default=True, err=True
+                ):
                     break
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     cli()
```

### Comparing `hardcoded-0.13.25/hardcoded/git.py` & `hardcoded-0.14.13/hardcoded/git.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,51 +1,53 @@
 #!/usr/bin/env python3
 
 from pathlib import Path
 import subprocess
 
+
 def _git(path, *args):
     path = Path(path).expanduser().resolve()
     path = path.is_dir() and path or path.parent
-    cmd = ('git', '-C', path) + args
+    cmd = ("git", "-C", path) + args
     return subprocess.run(cmd, capture_output=True)
 
 
 def find_repo_path(path):
     path = Path(path).resolve()
     if path.is_dir():
-        git_subdir = path/'.git'
+        git_subdir = path / ".git"
         if git_subdir.exists() and git_subdir.is_dir():
             # Found the applicable git repo root.
             return path
     if len(path.parents) > 0:
         return find_repo_path(path.parent)
 
 
 def find_gitignore_path(path):
     if repo_path := find_repo_path(path):
-        return repo_path/'.gitignore'
+        return repo_path / ".gitignore"
 
 
 def get_gitignore_rules(path):
     gitignore_path = find_gitignore_path(path)
     if gitignore_path.exists():
-        with gitignore_path.open('r') as f:
-            return list(filter(bool, f.read().split('\n')))
+        with gitignore_path.open("r") as f:
+            return list(filter(bool, f.read().split("\n")))
     return []
 
 
 def add_gitignore_rule(path, rule):
-    rules = get_gitignore_rules(path) + [rule,]
-    with find_gitignore_path(path).open('w') as f:
-        f.write('\n'.join(rules))
+    rules = get_gitignore_rules(path) + [
+        rule,
+    ]
+    with find_gitignore_path(path).open("w") as f:
+        f.write("\n".join(rules))
 
 
 def is_file_matched_by_gitignore_rule(path):
     path = Path(path).resolve()
     if repo_root := find_repo_path(path):
         for rule in get_gitignore_rules(path):
             if path.relative_to(repo_root).match(rule):
                 return True
         return False
     return None
-
```

### Comparing `hardcoded-0.13.25/hardcoded/logic.py` & `hardcoded-0.14.13/hardcoded/logic.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,148 +11,163 @@
 import subprocess
 from pathlib import Path
 from collections import defaultdict
 from functools import lru_cache, cached_property
 
 import yaml
 import click
+
 try:
     from cryptography.fernet import Fernet, InvalidToken
     from cryptography.hazmat.primitives import hashes
     from cryptography.hazmat.primitives.kdf.pbkdf2 import PBKDF2HMAC
+
     cryptography_support = True
-except:
+except Exception:
+
     class InvalidToken(NotImplementedError):
         pass
+
     cryptography_support = False
 try:
     import gnupg
+
     env = os.environ
     try:
         if tty_name := os.ttyname(sys.stdin.fileno()):
-            env['GPG_TTY'] = tty_name
-    except:
+            env["GPG_TTY"] = tty_name
+    except Exception:
         pass
     _gpg = gnupg.GPG(use_agent=True, env=env)
-except:
+except Exception:
     _gpg = None
 
 try:
     import psutil
+
     possible_mounted_secrets = []
 
     class MountedFile:
         def __init__(self, path):
             self.path = path
 
         def match_name(self, search_string):
             # Full path match
             if str(self.path) == search_string:
                 return 5
             score = 0
             # /data/.shhh
-            if self.path.stem.strip('.') == search_string:
+            if self.path.stem.strip(".") == search_string:
                 score = 1
             # /data/shhh.txt
             elif self.path.stem == search_string:
                 score = 2
             # /data/shhh
             elif self.path.name == search_string:
                 score = 3
             # /var/secrets/shhh
-            if score > 0 and re.search(r'secret', str(self.path)):
+            if score > 0 and re.search(r"secret", str(self.path)):
                 score += 1
             return score
 
         def __repr__(self):
             return str(self)
+
         def __str__(self):
             return str(self.path)
 
         @property
         def value(self):
-            with self.path.open('r') as f:
+            with self.path.open("r") as f:
                 return f.read()
 
     for part in psutil.disk_partitions(all=True):
-        if part.fstype in ('proc', 'devpts', 'mqueue', 'sysfs', 'cgroup2'):
+        if part.fstype in ("proc", "devpts", "mqueue", "sysfs", "cgroup2"):
             continue
         mountpoint = Path(part.mountpoint)
         if mountpoint.is_file():
             possible_mounted_secrets.append(MountedFile(mountpoint))
         elif mountpoint.is_dir():
             for path in mountpoint.iterdir():
                 if path.is_file():
                     possible_mounted_secrets.append(MountedFile(path))
 
     def get_secret_from_mounted_file(name):
         possible_matches = defaultdict(list)
         for possible_mounted_secret in possible_mounted_secrets:
-            possible_matches[possible_mounted_secret.match_name(name)].append(possible_mounted_secret)
+            possible_matches[possible_mounted_secret.match_name(name)].append(
+                possible_mounted_secret
+            )
         try:
             highest_score = max(possible_matches.keys())
-        except:
-            raise KeyError(
-                    f'Found no mounted secrets')
+        except Exception:
+            raise KeyError("Found no mounted secrets")
         if highest_score == 0:
             num_non_matching = possible_matches[0]
             raise KeyError(
-                    f'Found {num_non_matching} mounted files, but none matching the name "{name}"')
+                f'Found {num_non_matching} mounted files, but none matching the name "{name}"'
+            )
         best_matches = possible_matches[highest_score]
         if len(best_matches) > 1:
             raise KeyError(
-                    f'Could not decide which mounted file to use for "{name}": {best_matches}')
+                f'Could not decide which mounted file to use for "{name}": {best_matches}'
+            )
         return best_matches[0].value
-except:
+except Exception:
     pass
 
 from . import git
 
-DEFAULT_FILE_NAME = '.hardcoded.yml'
-CONFIG_HOME = Path(os.environ.get('XDG_CONFIG_HOME', Path.home()/'.config'))
-DEFAULT_FILE_PATH = CONFIG_HOME / DEFAULT_FILE_NAME.strip('.')
+DEFAULT_FILE_NAME = ".hardcoded.yml"
+CONFIG_HOME = Path(os.environ.get("XDG_CONFIG_HOME", Path.home() / ".config"))
+DEFAULT_FILE_PATH = CONFIG_HOME / DEFAULT_FILE_NAME.strip(".")
 NOT_GIVEN = object()
 
+
+def _debug(*msg):
+    if _debug.enabled:
+        click.echo(click.style(" ".join(map(str, msg)), fg="blue"), err=True)
+
+
+_debug.enabled = False
+
+
 class _DataFile:
     def __init__(self, path):
         self.path = path
         self._explicitly_not_encrypted = dict()
 
-
     def get(self, key, default=None):
         return self.data.get(key, default)
 
-
     def set(self, key, value):
         data = self.data
         data[key] = value
         self.data = data
 
-
     @property
     def data(self):
         try:
-            with open(self.path, 'r') as f:
+            with open(self.path, "r") as f:
                 data = yaml.safe_load(f) or dict()
                 self._explicitly_not_encrypted = dict()
-                if set(data.keys()) > set(('salt', 'encrypted')):
+                if set(data.keys()) > set(("salt", "encrypted")):
                     for k, v in data.items():
-                        if k not in ('salt', 'encrypted'):
+                        if k not in ("salt", "encrypted"):
                             self._explicitly_not_encrypted[k] = v
                 return data
-        except FileNotFoundError as ex:
+        except FileNotFoundError:
             return dict()
 
-
     @data.setter
     def data(self, data):
-        if set(data.keys()) >= set(('salt', 'encrypted')):
+        if set(data.keys()) >= set(("salt", "encrypted")):
             data.update(self._explicitly_not_encrypted)
         self.path.parent.mkdir(parents=True, exist_ok=True)
-        with open(self.path, 'w') as f:
+        with open(self.path, "w") as f:
             yaml.safe_dump(data, f)
 
 
 class _OneLayerDeeper:
     def __init__(self):
         self._salt = None
         self._fernet = None
@@ -160,394 +175,493 @@
         self._wrong_password = False
         self.path = None
         self._datafile = None
         self._namespace = None
         self.secret = None
         self.ask_if_not_found = None
 
-
     def _get_all_decrypted_data(self):
         data = self._datafile.data
         data_was_decrypted = False
         # Decrypt data if necessary.
-        if set(data.keys()) >= set(('salt', 'encrypted')):
-            self._salt = base64.urlsafe_b64decode(data.get('salt'))
-            ciphertext = data.get('encrypted').encode()
+        if set(data.keys()) >= set(("salt", "encrypted")):
+            self._salt = base64.urlsafe_b64decode(data.get("salt"))
+            ciphertext = data.get("encrypted").encode()
             success = False
             for _ in range(3):
                 try:
                     data = yaml.safe_load(self.decrypt(ciphertext)) or dict()
                     success = True
                     break
                 except ImportError as ex:
                     raise ex
                 except click.Abort:
                     exit(1)
                 except InvalidToken as ex:
                     if exception_msg := str(ex):
-                        exception_msg = f' ({exception_msg})'
-                    click.echo(f'Error while decrypting data file. {exception_msg} Did you enter the correct password?', err=True)
+                        exception_msg = f" ({exception_msg})"
+                    click.echo(
+                        f"Error while decrypting data file. {exception_msg} Did you enter the correct password?",
+                        err=True,
+                    )
                     self._fernet = None
                     self._wrong_password = True
             if not success:
-                raise RuntimeError(f'Unable to successfully decrypt datafile {self.path}.')
+                raise RuntimeError(
+                    f"Unable to successfully decrypt datafile {self.path}."
+                )
             data_was_decrypted = True
         elif data and self.secret:
             # Data should be secret, but was just read without decryption. Write back to force applying encryption.
             self._set_all_data(data)
 
-        if self.secret == None:
+        if self.secret is None:
             # No secret preference was given. Set based on previous status.
             self.secret = data_was_decrypted
 
         return data
 
-
     @property
     def data(self):
         all_data = self._get_all_decrypted_data() or dict()
         namespace_data = all_data.get(self._namespace, dict())
         return namespace_data
 
-
     @data.setter
     def data(self, namespace_data):
         all_data = self._get_all_decrypted_data() or dict()
         all_data[self._namespace] = namespace_data
         self._set_all_data(all_data)
 
-
     @property
     def _warned_about_gitignore(self):
-        return self._datafile.get('warned_about_gitignore', False)
+        return self._datafile.get("warned_about_gitignore", False)
+
     @_warned_about_gitignore.setter
     def _warned_about_gitignore(self, value):
-        self._datafile.set('warned_about_gitignore', value)
-
+        self._datafile.set("warned_about_gitignore", value)
 
     def _set_all_data(self, data):
         # Format data human readable.
         if self.secret:
             # Encrypt data, format ciphertext and salt human readable again.
             data_bytes = yaml.safe_dump(data).encode()
             data = {
-                'salt': base64.urlsafe_b64encode(self.salt).decode(),
-                'encrypted': self.encrypt(data_bytes),
-                }
+                "salt": base64.urlsafe_b64encode(self.salt).decode(),
+                "encrypted": self.encrypt(data_bytes),
+            }
 
         # Save data to file.
         self._datafile.data = data
-        
+
         if self.secret and not self._warned_about_gitignore:
             # Check if file is protected against leaking via git.
             data_file_path = Path(self.path).resolve()
             data_file_name = data_file_path.name
             git_repo_root = git.find_repo_path(data_file_path)
             gitignore_path = git.find_gitignore_path(data_file_path)
-            datafile_matched_by_gitignore_rule = git.is_file_matched_by_gitignore_rule(data_file_path)
-            if datafile_matched_by_gitignore_rule == False:
+            datafile_matched_by_gitignore_rule = git.is_file_matched_by_gitignore_rule(
+                data_file_path
+            )
+            if datafile_matched_by_gitignore_rule is False:
                 if gitignore_path.exists():
                     # Our data file path did not match any .gitignore rule.
                     question = f'Data file {data_file_path} is not matched by any of the rules in {gitignore_path}. Do you want to add the rule "{data_file_name}"?'
                 else:
                     # No .gitignore found in the repo.
                     question = f'{git_repo_root} seems to be a git repository, but there is no .gitignore file protecting data file {data_file_path}. Do you want to create a .gitignore file protecting "{data_file_name}"?'
-                if click.confirm(f'WARNING: {question}', default=True, err=True):
+                if click.confirm(f"WARNING: {question}", default=True, err=True):
                     git.add_gitignore_rule(git_repo_root, data_file_name)
                     click.edit(filename=gitignore_path)
                 self._warned_about_gitignore = True
 
-
     @property
     def salt(self):
         if not self._salt:
             self._salt = os.urandom(16)
         return self._salt
 
-
     def generate_random_password(self):
         minimum_length = 32
-        alphabet = string.digits + string.ascii_letters + '-_.,'
+        alphabet = string.digits + string.ascii_letters + "-_.,"
         while True:
-            password = ''.join(secrets.choice(alphabet) for i in range(minimum_length)).strip()
+            password = "".join(
+                secrets.choice(alphabet) for i in range(minimum_length)
+            ).strip()
             # TODO: Combine this with the current check on manually entered passwords.
-            if (any(c.islower() for c in password)
-                    and any(c.isupper() for c in password)
-                    and sum(c.isdigit() for c in password) >= 3
-                    and len(password) >= minimum_length):
+            if (
+                any(c.islower() for c in password)
+                and any(c.isupper() for c in password)
+                and sum(c.isdigit() for c in password) >= 3
+                and len(password) >= minimum_length
+            ):
                 return password
 
-
     def get_password(self):
         account = str(Path(self.path).resolve())
         password = None
-        
+
         # Try the Apple Keychain.
         save_to_keychain = False
-        if (not password) and shutil.which('security'):
+        if (not password) and shutil.which("security"):
             save_to_keychain = True
             if not self._wrong_password:
                 try:
-                    completed_process = subprocess.run(['security', 'find-internet-password', '-a', account, '-s', 'hardcoded', '-w'], capture_output=True)
+                    completed_process = subprocess.run(
+                        [
+                            "security",
+                            "find-internet-password",
+                            "-a",
+                            account,
+                            "-s",
+                            "hardcoded",
+                            "-w",
+                        ],
+                        capture_output=True,
+                    )
                     if completed_process.returncode == 0:
                         # We received a password from Apple Keychain.
                         password = completed_process.stdout.decode().strip()
                         save_to_keychain = False
                     elif completed_process.returncode == 44:
                         # Apple Keychain told us that no such password was found. Generate one, and stash it in Apple Keychain.
                         password = self.generate_random_password()
                     elif completed_process.returncode == 128:
                         # User cancelled.
                         pass
                     else:
-                        click.echo(f'Apple Keychain exit code {completed_process.returncode}:', err=True)
+                        click.echo(
+                            f"Apple Keychain exit code {completed_process.returncode}:",
+                            err=True,
+                        )
                         click.echo(completed_process.stdout.decode(), err=True)
                         click.echo(completed_process.stderr.decode(), err=True)
                         exit(completed_process.returncode)
                 except Exception as ex:
                     click.echo(ex, err=True)
                     pass
 
         if not password:
             if not sys.stdin.isatty():
                 raise RuntimeError(
-                        f'We need an encryption password for {self.path}, but stdin is not a TTY (so we cannot expect input).')
+                    f"We need an encryption password for {self.path}, but stdin is not a TTY (so we cannot expect input)."
+                )
             try:
-                password = click.prompt(f'Please enter the encryption password for {self.path}', hide_input=True, err=True)
+                password = click.prompt(
+                    f"Please enter the encryption password for {self.path}",
+                    hide_input=True,
+                    err=True,
+                )
             except ValueError as ex:
-                if 'closed file' in str(ex):
+                if "closed file" in str(ex):
                     raise RuntimeError(
-                            f'We need an encryption password for {self.path}, but stdin is closed (so we cannot expect input).')
+                        f"We need an encryption password for {self.path}, but stdin is closed (so we cannot expect input)."
+                    )
                 raise
         if save_to_keychain:
-            completed_process = subprocess.run(['security', 'add-internet-password', '-U', '-a', account, '-s', 'hardcoded', '-l', f'hardcoded {account}', '-T', '', '-w', password,], capture_output=True)
+            completed_process = subprocess.run(
+                [
+                    "security",
+                    "add-internet-password",
+                    "-U",
+                    "-a",
+                    account,
+                    "-s",
+                    "hardcoded",
+                    "-l",
+                    f"hardcoded {account}",
+                    "-T",
+                    "",
+                    "-w",
+                    password,
+                ],
+                capture_output=True,
+            )
         return password
 
-
     def fernet(self, password_policy=None):
         if not self._fernet:
             kdf = PBKDF2HMAC(
-                    algorithm=hashes.SHA256(),
-                    length=32,
-                    salt=self.salt,
-                    iterations=1000000,
-                    )
+                algorithm=hashes.SHA256(),
+                length=32,
+                salt=self.salt,
+                iterations=1000000,
+            )
             while True:
                 password = self.get_password()
                 if password_policy:
                     if not password_policy.search(password):
-                        click.echo(f'That password does not conform to the password policy regex: {password_policy.pattern}', err=True)
+                        click.echo(
+                            f"That password does not conform to the password policy regex: {password_policy.pattern}",
+                            err=True,
+                        )
                         self._wrong_password = True
                         continue
                 break
             key = base64.urlsafe_b64encode(kdf.derive(password.encode()))
             self._fernet = Fernet(key)
         return self._fernet
 
-
     @cached_property
     def _gpg_recipient(self):
         if self._saved_gpg_recipient:
             return self._saved_gpg_recipient
         user_level_datafile = _DataFile(path=DEFAULT_FILE_PATH)
-        config_key = 'Default GnuPG encryption key'
+        config_key = "Default GnuPG encryption key"
         if _saved_gpg_recipient := user_level_datafile.get(config_key):
             self._saved_gpg_recipient = _saved_gpg_recipient
             return self._saved_gpg_recipient
 
-        if not (private_keys := _gpg.list_keys(True)):
+        if not _gpg.list_keys(True):
             return None
 
-        click.echo('Available GnuPG secret keys:', err=False)
+        click.echo("Available GnuPG secret keys:", err=False)
         private_key = None
         for private_key in _gpg.list_keys(True):
-            click.echo('\t' + private_key.get('keyid') + '\t' + ' / '.join(private_key.get('uids')), err=False)
-        self._saved_gpg_recipient = click.prompt(text='Please choose a default GnuPG key to encrypt hardcoded data with', default=next(iter(private_key.get('uids', [private_key.get('keyid'),]))), err=True)
+            click.echo(
+                "\t"
+                + private_key.get("keyid")
+                + "\t"
+                + " / ".join(private_key.get("uids")),
+                err=False,
+            )
+        self._saved_gpg_recipient = click.prompt(
+            text="Please choose a default GnuPG key to encrypt hardcoded data with",
+            default=next(
+                iter(
+                    private_key.get(
+                        "uids",
+                        [
+                            private_key.get("keyid"),
+                        ],
+                    )
+                )
+            ),
+            err=True,
+        )
         user_level_datafile.set(config_key, self._saved_gpg_recipient)
         return self._saved_gpg_recipient
 
-
-
     def encrypt(self, data_bytes):
-        if (_gpg != None) and self._gpg_recipient:
+        if (_gpg is not None) and self._gpg_recipient:
             # Prefer encrypting directly with GPG.
             encrypted = _gpg.encrypt(data_bytes, self._gpg_recipient, always_trust=True)
             if encrypted.ok:
                 return encrypted.data.decode()
             else:
                 raise RuntimeError(
-                        f'GPG encryption for {self.path} failed: {encrypted.status}; {encrypted.stderr}')
+                    f"GPG encryption for {self.path} failed: {encrypted.status}; {encrypted.stderr}"
+                )
         elif cryptography_support:
             # Fall back to encrypting with the cryptography library.
-            password_policy = re.compile(r'.{8}')
-            return self.fernet(password_policy=password_policy).encrypt(data_bytes).decode()
+            password_policy = re.compile(r".{8}")
+            return (
+                self.fernet(password_policy=password_policy)
+                .encrypt(data_bytes)
+                .decode()
+            )
         else:
-            if (_gpg != None) and not self._gpg_recipient:
+            if (_gpg is not None) and not self._gpg_recipient:
                 raise RuntimeError(
-                        f'No GPG recipient found and no cryptography library found. Please either generate a GPG keypair or pip install \'hardcoded[encryption_without_pgp]\'.')
+                    "No GPG recipient found and no cryptography library found. Please either generate a GPG keypair or pip install 'hardcoded[encryption_without_pgp]'."
+                )
             else:
                 raise RuntimeError(
-                        f'No GPG found and no cryptography library found. Please either fix your GPG setup or pip install \'hardcoded[encryption_without_pgp]\'.')
-
+                    "No GPG found and no cryptography library found. Please either fix your GPG setup or pip install 'hardcoded[encryption_without_pgp]'."
+                )
 
     def decrypt(self, ciphertext):
         if not ciphertext:
-            return ''
-        if b'BEGIN PGP MESSAGE' in ciphertext:
-            if _gpg == None:
+            return ""
+        if b"BEGIN PGP MESSAGE" in ciphertext:
+            if _gpg is None:
                 raise RuntimeError(
-                        f'{self.path} contains PGP encrypted data. pip install python-gnupg to use it.')
+                    f"{self.path} contains PGP encrypted data. pip install python-gnupg to use it."
+                )
             else:
                 decrypted = _gpg.decrypt(ciphertext, always_trust=True)
                 if decrypted.ok:
                     return decrypted.data.decode()
                 else:
                     raise RuntimeError(
-                            f'GPG decryption of {self.path} failed: {decrypted.status}; {decrypted.stderr}')
+                        f"GPG decryption of {self.path} failed: {decrypted.status}; {decrypted.stderr}"
+                    )
         elif cryptography_support:
             # Does not look like PGP ciphertext. Assume Fernet.
             return self.fernet().decrypt(ciphertext).decode()
         else:
             raise RuntimeError(
-                    f'{self.path} contains symmetrically encrypted data. Please pip install \'hardcoded[encryption_without_pgp]\' to be able to decrypt it.')
+                f"{self.path} contains symmetrically encrypted data. Please pip install 'hardcoded[encryption_without_pgp]' to be able to decrypt it."
+            )
 
 
-class File():
+class File:
     def __init__(self, path=None, secret=True, ask_if_not_found=True, namespace=None):
-        '''A file with that data that you're not hardcoding.
+        """A file with that data that you're not hardcoding.
 
         path:    The path to the file. If your code is in a git repository, path is <repo_root>/.hardcoded.yml by default. Otherwise, ~/.hardcoded.yml.
         secret:  If True (the default), encrypt data and try not to put the file on Github.
         ask_if_not_found: If True (the default), the user will be prompted for missing values. Any default value in get() will be presented for easy cofirmation with [enter]. If False, the user will not be prompted for missing values, and any default in get() will be used straight away.
         namespace:        Two programs using the same namespace and the same file path can access each others values. By default, the namespace is based on path.
-        '''
-        super().__setattr__('__spec__', None)
-        super().__setattr__('__name__', 'File')
-        super().__setattr__('File', File)
-        super().__setattr__('DEFAULT_FILE_NAME', DEFAULT_FILE_NAME)
-        super().__setattr__('cli', None)
-        super().__setattr__('_x', _OneLayerDeeper())
+        """
+        super().__setattr__("__spec__", None)
+        super().__setattr__("__name__", "File")
+        super().__setattr__("File", File)
+        super().__setattr__("DEFAULT_FILE_NAME", DEFAULT_FILE_NAME)
+        super().__setattr__("cli", None)
+        super().__setattr__("_x", _OneLayerDeeper())
         self._x.secret = secret
         self._x.ask_if_not_found = ask_if_not_found
         if path and path != NOT_GIVEN:
-            path = Path(path).expanduser().resolve()
-            self._x.path = path
-            self._x._datafile = _DataFile(path=path)
-            self._x._namespace = namespace or str(path.parent)
+            self._x.path = Path(path).expanduser().resolve()
+            _debug("Datafile path set to", self._x.path)
         else:
             # This bit of code is duplicated in __init__.py.
             # This is because of the fact that this code looks at itself and finds the path of the file containing the code.
             caller_path = None
+            repo_root = None
             if path != NOT_GIVEN:
                 stack = None
                 try:
                     stack = inspect.stack()
                     this_code_file_path = stack[0].filename
                     for frame in stack:
-                        caller_path = frame.filename
-                        if caller_path != this_code_file_path and 'frozen' not in caller_path.lower():
+                        _debug("Called from", frame.filename)
+                        if (
+                            frame.filename != this_code_file_path
+                            and "frozen" not in frame.filename.lower()
+                            and "hardcoded" not in frame.filename.lower()
+                        ):
+                            caller_path = frame.filename
+                            _debug(
+                                frame.filename,
+                                "is the most recent code file calling hardcoded",
+                            )
                             break
                 finally:
                     del stack
-                repo_root = git.find_repo_path(caller_path)
-            else:
-                repo_root = None
+                if caller_path:
+                    _debug(
+                        "Searching for git repository root path containing", caller_path
+                    )
+                    repo_root = git.find_repo_path(caller_path)
+                if not repo_root:
+                    _debug(
+                        "Searching for git repository root path containing the current working directory"
+                    )
+                    repo_root = git.find_repo_path(".")
             if repo_root:
                 self._x.path = Path(repo_root) / DEFAULT_FILE_NAME
-                self._x._datafile = _DataFile(path=Path(repo_root)/DEFAULT_FILE_NAME)
-                self._x._namespace = namespace or 'data'
+                _debug(
+                    "Datafile path set to default filename inside repo root:",
+                    self._x.path,
+                )
             else:
                 self._x.path = DEFAULT_FILE_PATH
-                self._x._datafile = _DataFile(path=DEFAULT_FILE_PATH)
-                self._x._namespace = namespace or (caller_path and str(Path(caller_path).parent.resolve())) or 'data'
-
+                _debug(
+                    "Not inside a git repo. Datafile path set to default:",
+                    self._x.path,
+                )
+        self._x._datafile = _DataFile(path=self._x.path)
+        if namespace:
+            self._x._namespace = namespace
+            _debug("Namespace set to", self._x._namespace)
+        else:
+            # self._x._namespace = str(self._x.path.parent)
+            self._x._namespace = "data"
+            _debug(f"Namespace defaulting to {self._x._namespace!r}")
 
     def __setattr__(self, name, value):
         code_context = None
         stack = None
         try:
             stack = inspect.stack()
             this_code_file_path = stack[0].filename
             for frame in stack:
-                if frame.filename != this_code_file_path and 'frozen' not in frame.filename.lower():
+                if (
+                    frame.filename != this_code_file_path
+                    and "frozen" not in frame.filename.lower()
+                ):
                     code_context = frame.code_context
                     break
         finally:
             del stack
         raise NotImplementedError(
-                f'You weren\'t actually trying to hardcode {code_context.pop().strip()}, right? Please implicitly prompt the user for the value of {name} by just trying to use the value of {name}.')
-
+            f"You weren't actually trying to hardcode {code_context.pop().strip()}, right? Please implicitly prompt the user for the value of {name} by just trying to use the value of {name}."
+        )
 
     def __getattr__(self, name):
         return self.get(name)
 
     def __call__(self, *args, **kwargs):
         return self.get(*args, **kwargs)
 
     # Using the LRU cache cuts time to do repeated lookups by about 10000%.
     @lru_cache()
     def get(self, name, *, default=None, text=None, type=str):
-        '''Get the named variable from the data file.
+        """Get the named variable from the data file.
         If a value with this name doesn't exist and ask_if_not_found is True (the default), prompt the user for the value of a variable to be saved.
         In that case:
         text    may be used to customise the question to the user
         type    ensures that the entered data is saved as a specific data type
         default is the default value offered to the user, and also specifies type.
-        '''
-        if name in ('__path__', '__file__'):
+        """
+        if name in ("__path__", "__file__"):
             return None
-        elif name == '__origin__':
+        elif name == "__origin__":
             return File
 
         if environment_variable := os.environ.get(name):
             return type(environment_variable)
 
         try:
             return type(get_secret_from_mounted_file(name))
-        except:
+        except Exception:
             pass
 
         data = self._x.data
         if name in data:
             return data.get(name)
 
-        if (not self._x.ask_if_not_found) and default != None:
+        if (not self._x.ask_if_not_found) and default is not None:
             return default
 
         # Don't try to ask for input if stdin is not a TTY.
         if self._x.ask_if_not_found:
             if not sys.stdin.isatty():
-                click.echo(f'We need input ({name}), but stdin is not interactive and environment variable ${name} is empty!', err=True)
-                raise KeyError(
-                        f'Missing hardcoded.{name}')
+                click.echo(
+                    f"We need input ({name}), but stdin is not interactive and environment variable ${name} is empty!",
+                    err=True,
+                )
+                raise KeyError(f"Missing hardcoded.{name}")
             if not text:
-                text = f'Please enter {name} (will be saved in {self._x.path})'
+                text = f"Please enter {name} (will be saved in {self._x.path})"
             try:
                 if type == bool or default in (True, False):
                     # Boolean return value expected. Ask a boolean question.
                     click.echo(text, nl=False, err=True)
                     value = click.getchar(echo=True)
-                    while not value in 'yn':
-                        click.echo(f'\r{text} [yn]', nl=False, err=True)
+                    while value not in "yn":
+                        click.echo(f"\r{text} [yn]", nl=False, err=True)
                         value = click.getchar(echo=True)
                     click.echo(err=True)
-                    value = (value.lower() == 'y')
+                    value = value.lower() == "y"
                 else:
-                    value = click.prompt(text=text, type=type, default=default, err=True)
+                    value = click.prompt(
+                        text=text, type=type, default=default, err=True
+                    )
             except ValueError as ex:
-                if 'closed file' in str(ex):
+                if "closed file" in str(ex):
                     raise RuntimeError(
-                            f'We need input ({name}), but stdin is closed and environment variable ${name} is empty!')
+                        f"We need input ({name}), but stdin is closed and environment variable ${name} is empty!"
+                    )
                 raise
             data = self._x.data
             data[name] = value
             self._x.data = data
             return value
         else:
-            raise KeyError(
-                    f'Missing hardcoded.{name}')
-
+            raise KeyError(f"Missing hardcoded.{name}")
 
     def dict(self):
-        '''Return a dict containing all the keys and values from this file.'''
+        """Return a dict containing all the keys and values from this file."""
         return self._x.data
-
```

### Comparing `hardcoded-0.13.25/pyproject.toml` & `hardcoded-0.14.13/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hardcoded"
-version = "0.13.25"
+version = "0.14.13"
 description = "For everything that you really should not be hardcoding."
 license = "LGPL-3.0-or-later"
 authors = ["moizuo <no_spam@example.com>"]
 readme = "README.md"
 homepage = "https://pypi.org/project/hardcoded"
 
 [tool.poetry.dependencies]
```

### Comparing `hardcoded-0.13.25/PKG-INFO` & `hardcoded-0.14.13/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hardcoded
-Version: 0.13.25
+Version: 0.14.13
 Summary: For everything that you really should not be hardcoding.
 Home-page: https://pypi.org/project/hardcoded
 License: LGPL-3.0-or-later
 Author: moizuo
 Author-email: no_spam@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
```

