# Comparing `tmp/python_version_manager-2024.4.1.tar.gz` & `tmp/python_version_manager-2024.5.tar.gz`

## Comparing `python_version_manager-2024.4.1.tar` & `python_version_manager-2024.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0    19033 2020-02-02 00:00:00.000000 python_version_manager-2024.4.1/pyvm.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 python_version_manager-2024.4.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 python_version_manager-2024.4.1/LICENSE
--rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 python_version_manager-2024.4.1/README.md
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 python_version_manager-2024.4.1/pyproject.toml
--rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 python_version_manager-2024.4.1/PKG-INFO
+-rwxr-xr-x   0        0        0    22693 2020-02-02 00:00:00.000000 python_version_manager-2024.5/pyvm.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 python_version_manager-2024.5/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 python_version_manager-2024.5/LICENSE
+-rw-r--r--   0        0        0     8618 2020-02-02 00:00:00.000000 python_version_manager-2024.5/README.md
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 python_version_manager-2024.5/pyproject.toml
+-rw-r--r--   0        0        0     9019 2020-02-02 00:00:00.000000 python_version_manager-2024.5/PKG-INFO
```

### Comparing `python_version_manager-2024.4.1/pyvm.py` & `python_version_manager-2024.5/pyvm.py`

 * *Files 18% similar despite different names*

```diff
@@ -66,24 +66,27 @@
 
 exec "$PYVM_HOME/3.12/bin/python3.12" "$0" "$@"
 """
 # endregion
 
 # ruff: noqa: E401 EXE003 A001
 import os
+
 __doc__ = f"""Python Version Manager
 
 This tool is designed to download and install python versions from the 
 https://github.com/indygreg/python-build-standalone project into {os.environ.get('PYVM_HOME', '$HOME/.pyvm')}
 and add versioned executables (ie `python3.12` for python 3.12) into a directory on the PATH.
 
 Environment Variables:
-    PYVM_PBS_RELEASE: The release of python-build-standalone to target. Defaults to 'latest', can be set to a release name (eg '20240224')
     PYVM_HOME: The directory to install python versions into. Defaults to $HOME/.pyvm
     PYVM_BIN: The directory to install versioned executables into. Defaults to $HOME/.local/bin
+    PYVM_PBS_RELEASE: The release of python-build-standalone to target. Defaults to 'latest', can be set to a release name (eg '20240224')
+    PYVM_PIPX_RELEASE: The release of pipx to target. Defaults to 'latest', can be set to a release name (eg '1.5.0')
+    PYVM_PIPX_DEFAULT_PYTHON_VERSION: The default python version to use when installing pipx onto your PATH. Defaults to '3.12'
 """
 import sys
 import argparse
 import datetime
 import hashlib
 import json
 import logging
@@ -98,21 +101,23 @@
 from typing import Any, Dict, List, Literal, TYPE_CHECKING
 import urllib.error
 from urllib.request import urlopen
 
 
 if TYPE_CHECKING:
     from typing import overload
+
     @overload
     def _fetch(url: str, type: Literal["json"]) -> dict | list: ...
     @overload
     def _fetch(url: str, type: Literal["file"]) -> bytes: ...
     @overload
     def _fetch(url: str, type: Literal["checksum"]) -> str: ...
 
+
 # Much of the code in this module is adapted with extreme gratitude from
 # https://github.com/tusharsadhwani/yen/blob/main/src/yen/github.py
 
 MACHINE_SUFFIX: Dict[str, Dict[str, Any]] = {
     "Darwin": {
         "arm64": "aarch64-apple-darwin-install_only.tar.gz",
         "x86_64": "x86_64-apple-darwin-install_only.tar.gz",
@@ -126,232 +131,315 @@
             "glibc": "x86_64_v3-unknown-linux-gnu-install_only.tar.gz",
             "musl": "x86_64_v3-unknown-linux-musl-install_only.tar.gz",
         },
     },
     "Windows": {"AMD64": "x86_64-pc-windows-msvc-shared-install_only.tar.gz"},
 }
 
-GITHUB_API_URL = "https://api.github.com/repos/indygreg/python-build-standalone/releases"
+GITHUB_API_URL = (
+    "https://api.github.com/repos/indygreg/python-build-standalone/releases"
+)
+PIPX_API_URL = "https://api.github.com/repos/pypa/pipx/releases"
 PYTHON_VERSION_REGEX = re.compile(r"cpython-(\d+\.\d+\.\d+)")
 
 WINDOWS = platform.system() == "Windows"
-PYVM_HOME = Path(os.environ.get('PYVM_HOME', os.path.join(os.environ['HOME'], '.pyvm')))
-PYVM_TMP = PYVM_HOME / 'tmp'
-PYVM_BIN = Path(os.environ.get('PYVM_BIN', os.path.join(os.environ['HOME'], '.local/bin')))
+PYVM_HOME = Path(os.environ.get("PYVM_HOME", os.path.join(os.environ["HOME"], ".pyvm")))
+PYVM_TMP = PYVM_HOME / "tmp"
+PYVM_BIN = Path(
+    os.environ.get("PYVM_BIN", os.path.join(os.environ["HOME"], ".local/bin"))
+)
 PYVM_PBS_RELEASE = os.environ.get("PYVM_PBS_RELEASE", "latest")
+PYVM_PIPX_RELEASE = os.environ.get("PYVM_PIPX_RELEASE", "latest")
+PYVM_PIPX_DEFAULT_PYTHON_VERSION = os.environ.get("PYVM_PIPX_DEFAULT_PYTHON_VERSION", "3.12")
 
 
 class override:
     """Helper class to temporarily override module-level variables."""
+    # TODO: there has got to be a better way to do this
+
     def __init__(self):
         pass
 
     def __enter__(self):
         self.GITHUB_API_URL = GITHUB_API_URL
+        self.PIPX_API_URL = PIPX_API_URL
         self.PYTHON_VERSION_REGEX = PYTHON_VERSION_REGEX
         self.PYVM_HOME = PYVM_HOME
         self.PYVM_TMP = PYVM_TMP
         self.PYVM_BIN = PYVM_BIN
         self.PYVM_PBS_RELEASE = PYVM_PBS_RELEASE
-
+        self.PYVM_PIPX_RELEASE = PYVM_PIPX_RELEASE
+        self.PYVM_PIPX_DEFAULT_PYTHON_VERSION = PYVM_PIPX_DEFAULT_PYTHON_VERSION
 
     def __exit__(self, *args):
-        global GITHUB_API_URL, PYTHON_VERSION_REGEX, PYVM_HOME, PYVM_TMP, PYVM_BIN, PYVM_PBS_RELEASE
+        global GITHUB_API_URL, PIPX_API_URL, PYTHON_VERSION_REGEX, PYVM_HOME, PYVM_TMP, PYVM_BIN
+        global PYVM_PBS_RELEASE, PYVM_PIPX_RELEASE, PYVM_PIPX_DEFAULT_PYTHON_VERSION
         GITHUB_API_URL = self.GITHUB_API_URL
+        PIPX_API_URL = self.PIPX_API_URL
         PYTHON_VERSION_REGEX = self.PYTHON_VERSION_REGEX
         PYVM_HOME = self.PYVM_HOME
         PYVM_TMP = self.PYVM_TMP
         PYVM_BIN = self.PYVM_BIN
         PYVM_PBS_RELEASE = self.PYVM_PBS_RELEASE
+        PYVM_PIPX_RELEASE = self.PYVM_PIPX_RELEASE
+        PYVM_PIPX_DEFAULT_PYTHON_VERSION = self.PYVM_PIPX_DEFAULT_PYTHON_VERSION
 
 
 class NotAvailable(Exception):
     """Raised when the asked Python version is not available."""
 
 
 logger = logging.getLogger(__name__)
 
 
 def list_installed_versions():
     installations_found = False
     for major_minor, path in _installed_versions():
-        msg = f'python{major_minor} is installed'
+        msg = f"python{major_minor} is installed"
         _ensure_shim(path, major_minor)
         logger.info(msg)
         installations_found = True
     if not installations_found:
-        logger.info('No python installations installed through pyvm')
+        logger.info("No python installations installed through pyvm")
 
 
 def list_available_versions():
     pythons = _list_pythons()
     installed_pythons = [major_minor for major_minor, _ in _installed_versions()]
     logger.info("Available python versions:")
-    pythons = [version.split('.') for version in pythons]
+    pythons = [version.split(".") for version in pythons]
     pythons = sorted(pythons, key=lambda version: [int(k) for k in version])
     for version in pythons:
         major, minor, patch, *_ = version
         msg = f"{major}.{minor:2} --> {major}.{minor}.{patch}"
         if f"{major}.{minor}" in installed_pythons:
             msg += " (installed)"
         logger.info(msg)
 
 
 def install_version(version: str):
     """Install the given python version and return the path to the python binary."""
     version = _normalize_python_version(version)
     if python_bin := _installed_version(version):
-        logger.warning(f'Python version {version} is already installed')
+        logger.warning(f"Python version {version} is already installed")
         return python_bin
-    logger.info(f'Installing python {version}...')
+    logger.info(f"Installing python {version}...")
     python_bin = _download_python_build_standalone(version)
     _ensure_shim(python_bin, version)
     return python_bin
 
 
 def ensure_version(version: str):
     """Ensure that the given python version is installed and return the path to the python binary."""
     version = _normalize_python_version(version)
-    if (python_bin := _installed_version(version)):
+    if python_bin := _installed_version(version):
         return python_bin
     else:
-        return install_version(version)
+        return _download_python_build_standalone(version)
 
 
 def uninstall_version(version: str):
     version = _normalize_python_version(version)
     _uninstall_version(version)
     _remove_shim(version)
 
 
 def update_all_versions():
+    maybe_update_pipx()
     available_pythons = _list_pythons()
-    available_pythons = {'.'.join(v.split('.')[:2]): v for v in available_pythons}
+    available_pythons = {".".join(v.split(".")[:2]): v for v in available_pythons}
     for major_minor, path in _installed_versions():
-        version = subprocess.check_output([path, '--version']).decode().split()[1]
-        if major_minor in available_pythons and version != available_pythons[major_minor]:
+        version = subprocess.check_output([path, "--version"]).decode().split()[1]
+        if (
+            major_minor in available_pythons
+            and version != available_pythons[major_minor]
+        ):
             _uninstall_version(major_minor)
             _remove_shim(major_minor)
-            logger.info(f'Updating python {major_minor} from {version} to {available_pythons[major_minor]}...')
+            logger.info(
+                f"Updating python {major_minor} from {version} to {available_pythons[major_minor]}..."
+            )
             python_bin = _download_python_build_standalone(major_minor)
             _ensure_shim(python_bin, major_minor)
 
 
+def maybe_update_pipx():
+    "Update pipx, but only if it's already been downloaded"
+    pipx_zipapp = PYVM_HOME / "pipx.pyz"
+    if pipx_zipapp.exists():
+        logger.info("Updating pipx...")
+        download_pipx()
+
+
+def download_pipx():
+    # step one: get the latest release of pipx
+    # TODO: a lot of this logic is pulled from _get_github_release_assets. i should refactor that function to be more generic
+    url = PIPX_API_URL
+    if PYVM_PIPX_RELEASE == "latest":
+        url += "/latest"
+    release_data = _fetch(url, "json")
+    if PYVM_PIPX_RELEASE != "latest":
+        release_data = [
+            release
+            for release in release_data
+            if release["tag_name"] == PYVM_PIPX_RELEASE
+        ]
+        if not release_data:
+            raise Exception(f"Unable to find pipx release {PYVM_PIPX_RELEASE}.")
+        release_data = release_data[0]
+    pyz_download_url = [
+        asset["browser_download_url"]
+        for asset in release_data["assets"] # type: ignore
+        if asset["name"].endswith(".pyz")
+    ][0]
+    _download("pipx.pyz", pyz_download_url, PYVM_HOME / "pipx.pyz")
+    return PYVM_HOME / "pipx.pyz"
+
+
+def ensure_pipx():
+    """Ensure that pipx is installed and return the path to the pipx zipapp."""
+    pipx_zipapp = PYVM_HOME / "pipx.pyz"
+    if pipx_zipapp.exists():
+        return pipx_zipapp
+    logger.info("Aquiring pipx...")
+    pipx_zipapp = download_pipx()
+    return pipx_zipapp
+
+
+def install_pipx():
+    """Download the pipx zipapp into PYVM_HOME and install a shim into PYVM_BIN."""
+    pipx_zipapp = ensure_pipx()
+    default_python = ensure_version(PYVM_PIPX_DEFAULT_PYTHON_VERSION)
+    shim = PYVM_BIN / "pipx"
+    if not shim.exists():
+        logger.info(f"Creating shim for pipx at {shim}")
+        shim.write_text(f'#!/bin/sh\nexec {default_python} {pipx_zipapp} "$@"\n')
+        shim.chmod(0o755)
+    return shim
+
+
 def _installed_versions():
-    for installed_version in PYVM_HOME.glob('3.*/bin'):
+    for installed_version in PYVM_HOME.glob("3.*/bin"):
         major_minor = installed_version.parent.name
-        installed_bin = installed_version / f'python{major_minor}'
+        installed_bin = installed_version / f"python{major_minor}"
         yield major_minor, installed_bin
 
 
 def _installed_version(version: str):
     for major_minor, installed_bin in _installed_versions():
         if major_minor == version:
             return installed_bin
     return None
 
 
 def _uninstall_version(version: str):
     if not _installed_version(version):
-        logger.warning(f'Python version {version} is not installed')
+        logger.warning(f"Python version {version} is not installed")
         return
     shutil.rmtree(PYVM_HOME / version)
-    logger.info(f'Uninstalled python {version}')
+    logger.info(f"Uninstalled python {version}")
 
 
 def _ensure_shim(path: Path, version: str):
     """Ensure that the python binary is available in the pyvm bin directory"""
-    # This needs to be a shim, rather than a symlink, for reasons explained in the README, 
+    # This needs to be a shim, rather than a symlink, for reasons explained in the README,
     # under heading `## Why a shim, and not a symlink?`
     # The shim sets the TERMINFO_DIRS environment variable to include most common terminfo directories
     # as a workaround to https://gregoryszorc.com/docs/python-build-standalone/main/quirks.html#backspace-key-doesn-t-work-in-python-repl
     _ensure_pyvm_bin_dir()
-    shim = Path(PYVM_BIN / f'python{version}')
+    shim = Path(PYVM_BIN / f"python{version}")
     if not shim.exists():
-        logger.info(f'Creating shim for {version} at {shim}')
+        logger.info(f"Creating shim for {version} at {shim}")
         shim.write_text(f'#!/bin/sh\nexec {path} "$@"\n')
         shim.chmod(0o755)
     return shim
 
 
 def _ensure_pyvm_bin_dir():
     Path(PYVM_BIN).mkdir(parents=True, exist_ok=True)
-    for bin_dir in os.environ['PATH'].split(os.pathsep):
+    for bin_dir in os.environ["PATH"].split(os.pathsep):
         if PYVM_BIN.samefile(bin_dir):
             return
     else:
-        logger.warning(f'Please add {PYVM_BIN} to your PATH')
-        logger.warning(f'Ex, add the following to your shell profile: export PATH=$PATH:{PYVM_BIN}')
+        logger.warning(f"Please add {PYVM_BIN} to your PATH")
+        logger.warning(
+            f"Ex, add the following to your shell profile: export PATH=$PATH:{PYVM_BIN}"
+        )
 
 
 def _remove_shim(version: str):
     # only remove the shim if it points to the version we're uninstalling
-    shim = PYVM_BIN / f'python{version}'
+    shim = PYVM_BIN / f"python{version}"
     path = _installed_version(version)
     if not path:
         return
     if str(path) in shim.read_text():
         shim.unlink()
-        logger.info(f'Removed {shim}')
+        logger.info(f"Removed {shim}")
 
 
 def _normalize_python_version(python_version: str) -> str:
     # python_version can be a bare version number like "3.9" or a "binary name" like python3.10
     # we'll convert it to a bare version number
     return re.sub(r"[c]?python", "", python_version)
 
 
 def _download_python_build_standalone(python_version: str):
     """Attempt to download and use an appropriate python build
     from https://github.com/indygreg/python-build-standalone
-    and unpack it into the PYVM_HOME directory. 
+    and unpack it into the PYVM_HOME directory.
     Returns the full path to the python binary within that build"""
-    python_bin = "python.exe" if WINDOWS else f"python{python_version}"
 
     install_dir = PYVM_HOME / python_version
-    installed_python = install_dir / "bin" / python_bin
+    installed_python = (
+        install_dir / "python.exe" if WINDOWS else install_dir / "bin" / "python3"
+    )
 
     if installed_python.exists():
         return installed_python
 
     if install_dir.exists():
-        logger.warning(f"A previous attempt to install python {python_version} failed. Retrying.")
+        logger.warning(
+            f"A previous attempt to install python {python_version} failed. Retrying."
+        )
         shutil.rmtree(install_dir)
 
     try:
         full_version, download_link = _resolve_python_version(python_version)
     except NotAvailable as e:
-        raise Exception(f"Unable to acquire a standalone python build matching {python_version}.") from e
+        raise Exception(
+            f"Unable to acquire a standalone python build matching {python_version}."
+        ) from e
 
     with tempfile.TemporaryDirectory() as tempdir:
         archive = Path(tempdir) / f"python-{full_version}.tar.gz"
         download_dir = Path(tempdir) / "download"
 
         # download the python build gz
-        _download(full_version, download_link, archive)
+        _download(f"python {full_version} build", download_link, archive)
 
         # unpack the python build
         _unpack(full_version, download_link, archive, download_dir)
 
         # the python installation we want is nested in the tarball
         # under a directory named 'python'. We move it to the install
         # directory
         extracted_dir = download_dir / "python"
-        extracted_dir.rename(install_dir)
+        shutil.move(extracted_dir, install_dir)
 
     return installed_python
 
 
-def _download(full_version: str, download_link: str, archive: Path):
-    logger.info(f"Downloading python {full_version} build")
+def _download(what: str, from_url: str, to_path: Path):
+    logger.info(f"Downloading {what}")
     try:
-        archive.write_bytes(_fetch(download_link, "file"))
-        
+        to_path.write_bytes(_fetch(from_url, "file"))
+
     except urllib.error.URLError as e:
-        raise Exception(f"Unable to download python {full_version} build.") from e
+        raise Exception(f"Unable to download {what}.") from e
 
 
 def _fetch(url, type: Literal["json", "file", "checksum"]):
     # A single mockable function to fetch json, files, or checksums from github
     if type == "json":
         with urlopen(url) as response:
             return json.load(response)
@@ -363,29 +451,32 @@
             for data in iter(partial(response.read, 32768), b""):
                 res.write(data)
         res.seek(0)
         return res.read()
     elif type == "checksum":
         return urlopen(url).read().decode().rstrip("\n")
     else:
-        raise ValueError(f"Argumen `type` must be one of ['json', 'file', 'checksum'], not {type}")
+        raise ValueError(
+            f"Argumen `type` must be one of ['json', 'file', 'checksum'], not {type}"
+        )
 
 
 def _unpack(full_version, download_link, archive: Path, download_dir: Path):
     logger.info(f"Unpacking python {full_version} build")
     # Calculate checksum
     with open(archive, "rb") as python_zip:
         checksum = hashlib.sha256(python_zip.read()).hexdigest()
 
     # Validate checksum
     checksum_link = download_link + ".sha256"
     expected_checksum = _fetch(checksum_link, "checksum")
     if checksum != expected_checksum:
         raise Exception(
-            f"Checksum mismatch for python {full_version} build. " f"Expected {expected_checksum}, got {checksum}."
+            f"Checksum mismatch for python {full_version} build. "
+            f"Expected {expected_checksum}, got {checksum}."
         )
 
     with tarfile.open(archive, mode="r:gz") as tar:
         tar.extractall(download_dir)
 
 
 def _get_or_update_index():
@@ -421,44 +512,56 @@
     if PYVM_PBS_RELEASE == "latest":
         url += "/latest"
 
     try:
         release_data = _fetch(url, "json")
     except urllib.error.URLError as e:
         # raise
-        raise Exception(f"Unable to fetch python-build-standalone release data (from {url}).") from e
+        raise Exception(
+            f"Unable to fetch python-build-standalone release data (from {url})."
+        ) from e
 
     if PYVM_PBS_RELEASE != "latest":
-        release_data = [release for release in release_data if release["tag_name"] == PYVM_PBS_RELEASE]
+        release_data = [
+            release
+            for release in release_data
+            if release["tag_name"] == PYVM_PBS_RELEASE
+        ]
         if not release_data:
-            raise Exception(f"Unable to find python-build-standalone release {PYVM_PBS_RELEASE}.")
+            raise Exception(
+                f"Unable to find python-build-standalone release {PYVM_PBS_RELEASE}."
+            )
         release_data = release_data[0]
 
-    return [asset["browser_download_url"] for asset in release_data["assets"]] # type: ignore
+    return [asset["browser_download_url"] for asset in release_data["assets"]]  # type: ignore
 
 
 def _list_pythons() -> Dict[str, str]:
     """Returns available python versions for your machine and their download links."""
     system, machine = platform.system(), platform.machine()
     download_link_suffix = MACHINE_SUFFIX[system][machine]
     # linux suffixes are nested under glibc or musl builds
     if system == "Linux":
         # fallback to musl if libc version is not found
         libc_version = platform.libc_ver()[0] or "musl"
         download_link_suffix = download_link_suffix[libc_version]
 
     python_assets = _get_or_update_index()["assets"]
 
-    available_python_links = [link for link in python_assets if link.endswith(download_link_suffix)]
+    available_python_links = [
+        link for link in python_assets if link.endswith(download_link_suffix)
+    ]
 
     python_versions: dict[str, str] = {}
     for link in available_python_links:
         match = PYTHON_VERSION_REGEX.search(link)
         if match is None:
-            logger.warning(f"Could not parse python version from link {link}. Skipping.")
+            logger.warning(
+                f"Could not parse python version from link {link}. Skipping."
+            )
             continue
         python_version = match[1]
         python_versions[python_version] = link
 
     sorted_python_versions = {
         version: python_versions[version]
         for version in sorted(
@@ -482,44 +585,66 @@
     else:
         raise NotAvailable(f"Python version {requested_version} is not available.")
 
     return python_version, download_link
 
 
 def main():
-    logging.basicConfig(level=logging.INFO, stream=sys.stderr, format='%(message)s')
-    parser = argparse.ArgumentParser(description=__doc__, formatter_class=argparse.RawDescriptionHelpFormatter)
-    subparsers = parser.add_subparsers(dest='command')
-    list_parser = subparsers.add_parser('list', help='List installed python versions')
-    install_parser = subparsers.add_parser('install', help='Install a python version')
-    install_parser.add_argument('version', nargs='?', help='The version of python to install')
-    uninstall_parser = subparsers.add_parser('uninstall', help='Uninstall a python version')
-    uninstall_parser.add_argument('version', nargs='?', help='The version of python to install')
-    update_parser = subparsers.add_parser('update', help='Update all installed python versions')
-    run_parser = subparsers.add_parser('run', help='Run a python version')
-    run_parser.add_argument('version', help='The version of python to run')
-    run_parser.add_argument('args', nargs=argparse.REMAINDER, help='Arguments to pass to the python binary')
-    
-    args= parser.parse_args()
+    logging.basicConfig(level=logging.INFO, stream=sys.stderr, format="%(message)s")
+    parser = argparse.ArgumentParser(
+        description=__doc__, formatter_class=argparse.RawDescriptionHelpFormatter
+    )
+    subparsers = parser.add_subparsers(dest="command")
+    list_parser = subparsers.add_parser("list", help="List installed python versions")
+    install_parser = subparsers.add_parser("install", help="Install a python version")
+    install_parser.add_argument(
+        "version", nargs="?", help="The version of python to install"
+    )
+    uninstall_parser = subparsers.add_parser(
+        "uninstall", help="Uninstall a python version"
+    )
+    uninstall_parser.add_argument(
+        "version", nargs="?", help="The version of python to install"
+    )
+    update_parser = subparsers.add_parser(
+        "update", help="Update all installed python versions"
+    )
+    run_parser = subparsers.add_parser("run", help="Run a python version")
+    run_parser.add_argument("version", help="The version of python to run")
+    run_parser.add_argument(
+        "args", nargs=argparse.REMAINDER, help="Arguments to pass to the python binary"
+    )
+    pipx_parser = subparsers.add_parser("pipx", help="Run pipx")
+    pipx_parser.add_argument("version", help="The version of python to run pipx with")
+    pipx_parser.add_argument(
+        "args", nargs=argparse.REMAINDER, help="Arguments to pass to pipx"
+    )
+
+    args = parser.parse_args()
 
     match args.command:
-        case 'list':
+        case "list":
             list_installed_versions()
-        case 'install':
+        case "install":
             if not args.version:
                 list_available_versions()
                 exit(1)
             install_version(args.version)
-        case 'uninstall':
-            assert args.version, 'Please specify a version to uninstall'
+        case "uninstall":
+            assert args.version, "Please specify a version to uninstall"
             uninstall_version(args.version)
-        case 'update':
+        case "update":
             update_all_versions()
-        case 'run':
+        case "run":
             bin = ensure_version(args.version)
             os.execl(bin, bin, *args.args)
+        case "pipx":
+            bin = ensure_version(args.version)
+            pipx_zipapp = ensure_pipx()
+            os.execl(bin, bin, pipx_zipapp, *args.args)
         case None:
             parser.print_help()
             exit(1)
 
+
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `python_version_manager-2024.4.1/.gitignore` & `python_version_manager-2024.5/.gitignore`

 * *Files identical despite different names*

### Comparing `python_version_manager-2024.4.1/LICENSE` & `python_version_manager-2024.5/LICENSE`

 * *Files identical despite different names*

### Comparing `python_version_manager-2024.4.1/pyproject.toml` & `python_version_manager-2024.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 name = "python-version-manager" # pyvm was already taken by an unrelated project, and pyvm-lib is too similar to pyvm :(
 description = "dead-simple python version manager powered by python-build-standalone"
 authors = [
     { name = "Alex Tremblay", email = "alex.tremblay@utoronto.ca" },
 ]
 requires-python = ">=3.6"
 readme = "README.md"
-version = "2024.4.1"
+version = "2024.5"
 
 license = { text = "MIT" }
 
 [project.urls]
 Repository = "https://github.com/alextremblay/pyvm"
 Homepage = "https://alextremblay.github.io/pyvm/"
```

### Comparing `python_version_manager-2024.4.1/PKG-INFO` & `python_version_manager-2024.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: python-version-manager
-Version: 2024.4.1
-Summary: dead-simple python version manager powered by python-build-standalone
-Project-URL: Repository, https://github.com/alextremblay/pyvm
-Project-URL: Homepage, https://alextremblay.github.io/pyvm/
-Author-email: Alex Tremblay <alex.tremblay@utoronto.ca>
-License: MIT
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 ![PyVM Logo](https://alextremblay.github.io/pyvm/logo.png)
 
 # PyVM
 dead-simple python version manager powered by [python-build-standalone](https://github.com/indygreg/python-build-standalone)
 
 # Installation
 
@@ -26,14 +15,16 @@
 ```
 
 `pyvm` will work on any modern-ish Linux/MacOS computer that has either `curl` or `wget` installed.
 
 # features
 - Can manage multiple portable python installations sourced from the amazing [PBS](https://github.com/indygreg/python-build-standalone) project
 - installs python versions to isolated location, doesn't interfere with or interact with any version of python installed/used by your operating system
+- Can cache and run python installations without altering your PATH
+- Can bootstrap and run pipx commands without needing to install any pipx or python version beforehand
 
 # Use Cases
 
 ## I want python3.10 and 3.11 on my PATH
 
 ```console
 pyvm install 3.10
@@ -68,38 +59,144 @@
     pyvm.PYVM_HOME = pathlib.Path('/your/preferred/python/installation/path')
     pyvm.PYVM_BIN = pathlib.Path('/your/preferred/PATH/directory')
 
     py311_binary = pyvm.install_version("3.11")
     assert 'Python 3.11' in subprocess.run([py311_binary, "--version"], capture_output=True).stdout.decode()
 ```
 
+## I want to run a python script without installing anything in my PATH (including pyvm)
+
+This works too! 
+
+Assuming you have a script called `myscript.py`, simply download pyvm to your current directory and run it:
+
+```console
+$ curl -sSfLo ./pyvm alextremblay.github.io/pyvm/pyvm.py && chmod +x ./pyvm
+
+$ ./pyvm run 3.12 myscript.py
+```
+
+
+## I want to run a script that has dependencies, installing nothing other than pyvm
+
+Let's say you have a script called `myscript.py`, and it depends on external PYPI packages `requests` and `rich`
+
+you want to be able to run this script as a shell script/command and have it bootstrap its preferred python version (eg 3.11) AND all of its dependencies
+
+That's a tall order! but with PyVM installed, it's possible!
+
+Add this code block to the top of your script:
+
+```sh
+#!/usr/bin/env -S pyvm pipx 3.11 run --path
+
+# /// script
+# dependencies = [
+#   "requests",
+#   "rich",
+# ]
+# ///
+```
+
+Then make your script executable:
+
+```console
+$ chmod +x ./myscript.py
+```
+
+and run it!
+
+```console
+$ ./myscript.py
+```
+
+## I want to share a script with colleagues that requires NO pre-installed dependencies (even on PyVM)
+
+You wrote a script that requires a specific version of python, specific dependencies/libraries installed,
+
+and you want to be able to send your script to friends and colleagues such that they can execute your script and have it bootstrap all of its own dependencies, without having to install any other software before running your script, not even PyVM itself...
+
+Well, this will look weird, but it works! and it should work on every POSIX-compliant python-build-standalone-compatible UNIX OS
+
+`example.py`:
+```python
+#!/bin/bash
+""":"
+set -euo pipefail
+
+PYTHON_VERSION="3.12"
+
+HERE="$( dirname -- "$( readlink -f -- "$0"; )"; )"
+PYVM="$HERE/pyvm"
+if [ ! -f "$PYVM" ]; then
+
+  # define a function which selects curl or wget based on availability
+  download() {
+      if command -v curl &> /dev/null; then
+          curl -s -L -o $1 $2
+      elif command -v wget &> /dev/null; then
+          wget -q -O $1 $2
+      else
+          echo "Neither curl nor wget found. Please install one of these packages."
+          exit 1
+      fi
+  }
+
+  echo "Bootstrapping PyVM..."
+  download $PYVM alextremblay.github.io/pyvm/pyvm.py
+  chmod +x $PYVM
+
+fi
+
+exec "$PYVM" pipx $PYTHON_VERSION run --path "$0" "$@"
+"""
+
+# /// script
+# dependencies = [
+#   "requests",
+#   "rich",
+# ]
+# ///
+
+
+import requests
+from rich import print
+
+print(requests.get("https://httpbin.org").text)
+```
+
+You set your preferred python version with the shell variable on line 5, you set your dependencies within the `# /// script` comment block, and your python code goes in after the `# ///` at the end of the comment block
+
 # Command Line Interface
 
 ```console
 $ pyvm -h
-usage: pyvm [-h] {list,install,uninstall,update,run} ...
+usage: pyvm [-h] {list,install,uninstall,update,run,pipx} ...
 
 Python Version Manager
 
 This tool is designed to download and install python versions from the 
 https://github.com/indygreg/python-build-standalone project into /home/atremblay/.pyvm
 and add versioned executables (ie `python3.12` for python 3.12) into a directory on the PATH.
 
 Environment Variables:
-    PYVM_PBS_RELEASE: The release of python-build-standalone to target. Defaults to 'latest', can be set to a release name (eg '20240224')
     PYVM_HOME: The directory to install python versions into. Defaults to $HOME/.pyvm
     PYVM_BIN: The directory to install versioned executables into. Defaults to $HOME/.local/bin
+    PYVM_PBS_RELEASE: The release of python-build-standalone to target. Defaults to 'latest', can be set to a release name (eg '20240224')
+    PYVM_PIPX_RELEASE: The release of pipx to target. Defaults to 'latest', can be set to a release name (eg '1.5.0')
+    PYVM_PIPX_DEFAULT_PYTHON_VERSION: The default python version to use when installing pipx onto your PATH. Defaults to '3.12'
 
 positional arguments:
-  {list,install,uninstall,update,run}
+  {list,install,uninstall,update,run,pipx}
     list                List installed python versions
     install             Install a python version
     uninstall           Uninstall a python version
     update              Update all installed python versions
     run                 Run a python version
+    pipx                Run pipx
 
 options:
   -h, --help            show this help message and exit
 ```
 
 # Extra Info
 
@@ -119,15 +216,14 @@
 
 # Compatibility
 `pyvm` has been tested in linux (ubuntu x86_64 14.04+ and fedora 32+) and macos (macOS 13.6 aarch64), but should theoretically work in any linux x86_64 or aarch64 distribution (as long as `curl` or `wget` are installed), and any version of macOS
 
 # Stretch goals
 `pyvm` is still a very young project, and there are many features that have yet to be implemented:
 
-- pipx integration (possibly by bootstrapping the pipx pex file into PYVM_HOME)
 - a `--global` flag which will set `$PYVM_HOME` default value to `/opt/pyvm` and `$PYVM_BIN` to `/usr/local/bin`
 - test coverage >=80%
 - windows support
 - musl support
 - an install script for people who think copy-pasting 3 lines into their terminal is 2 too many :P
 
 # contributing
```

