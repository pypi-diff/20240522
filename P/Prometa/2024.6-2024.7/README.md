# Comparing `tmp/prometa-2024.6.tar.gz` & `tmp/prometa-2024.7.tar.gz`

## Comparing `prometa-2024.6.tar` & `prometa-2024.7.tar`

### file list

```diff
@@ -1,37 +1,39 @@
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 prometa-2024.6/.gitlab-ci.yml
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 prometa-2024.6/CITATION.cff
--rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 prometa-2024.6/TODO.md
--rw-r--r--   0        0        0     2970 2020-02-02 00:00:00.000000 prometa-2024.6/codemeta.json
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 prometa-2024.6/doc/Makefile
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 prometa-2024.6/doc/make.bat
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 prometa-2024.6/doc/requirements.txt
--rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 prometa-2024.6/doc/source/conf.py
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 prometa-2024.6/doc/source/readme.md
--rwxr-xr-x   0        0        0      960 2020-02-02 00:00:00.000000 prometa-2024.6/scripts/publish_documentation.sh
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/__init__.py
--rw-r--r--   0        0        0     4404 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/citation.py
--rw-r--r--   0        0        0     5234 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/codemeta.py
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/common.py
--rw-r--r--   0        0        0    10012 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/config.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/exception.py
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/file.py
--rw-r--r--   0        0        0     3136 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/insert.py
--rw-r--r--   0        0        0     3209 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/main.py
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/project.py
--rw-r--r--   0        0        0     5993 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/readme.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/version.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/gitlab/__init__.py
--rw-r--r--   0        0        0     7131 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/gitlab/ci.py
--rw-r--r--   0        0        0     3120 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/gitlab/repo.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/id/__init__.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/id/hal.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/id/orcid.py
--rw-r--r--   0        0        0     1864 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/id/swh.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/python/__init__.py
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/python/common.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 prometa-2024.6/src/prometa/python/venv.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 prometa-2024.6/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 prometa-2024.6/LICENSE.txt
--rw-r--r--   0        0        0     9498 2020-02-02 00:00:00.000000 prometa-2024.6/README.md
--rw-r--r--   0        0        0     1556 2020-02-02 00:00:00.000000 prometa-2024.6/pyproject.toml
--rw-r--r--   0        0        0    11490 2020-02-02 00:00:00.000000 prometa-2024.6/PKG-INFO
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 prometa-2024.7/.gitlab-ci.yml
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 prometa-2024.7/CITATION.cff
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 prometa-2024.7/TODO.md
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 prometa-2024.7/codemeta.json
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 prometa-2024.7/doc/Makefile
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 prometa-2024.7/doc/make.bat
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 prometa-2024.7/doc/requirements.txt
+-rw-r--r--   0        0        0     1461 2020-02-02 00:00:00.000000 prometa-2024.7/doc/source/conf.py
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 prometa-2024.7/doc/source/readme.md
+-rwxr-xr-x   0        0        0      960 2020-02-02 00:00:00.000000 prometa-2024.7/scripts/publish_documentation.sh
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/__init__.py
+-rw-r--r--   0        0        0     4584 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/citation.py
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/common.py
+-rw-r--r--   0        0        0    11677 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/config.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/exception.py
+-rw-r--r--   0        0        0     1940 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/file.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/insert.py
+-rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/main.py
+-rw-r--r--   0        0        0     4904 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/project.py
+-rw-r--r--   0        0        0     6080 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/readme.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/version.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/codemeta/__init__.py
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/codemeta/codemeta.py
+-rw-r--r--   0        0        0     3587 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/codemeta/pyproject.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/gitlab/__init__.py
+-rw-r--r--   0        0        0     7036 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/gitlab/ci.py
+-rw-r--r--   0        0        0     3142 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/gitlab/repo.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/id/__init__.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/id/hal.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/id/orcid.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/id/swh.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/python/__init__.py
+-rw-r--r--   0        0        0     4490 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/python/common.py
+-rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 prometa-2024.7/src/prometa/python/venv.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 prometa-2024.7/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 prometa-2024.7/LICENSE.txt
+-rw-r--r--   0        0        0    10387 2020-02-02 00:00:00.000000 prometa-2024.7/README.md
+-rw-r--r--   0        0        0     1569 2020-02-02 00:00:00.000000 prometa-2024.7/pyproject.toml
+-rw-r--r--   0        0        0    12400 2020-02-02 00:00:00.000000 prometa-2024.7/PKG-INFO
```

### Comparing `prometa-2024.6/.gitlab-ci.yml` & `prometa-2024.7/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `prometa-2024.6/CITATION.cff` & `prometa-2024.7/CITATION.cff`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 - description: The Software Heritage URL.
   type: url
   value: https://archive.softwareheritage.org/browse/origin/?origin_url=https%3A//gitlab.inria.fr/jrye/prometa.git
 license: MIT
 message: If you use this software, please cite it using these metadata.
 repository-code: https://gitlab.inria.fr/jrye/prometa.git
 title: Prometa
-version: '2024.6'
+version: '2024.7'
```

### Comparing `prometa-2024.6/codemeta.json` & `prometa-2024.7/codemeta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222221%*

 * *Differences: {"'softwareRequirements'": "{insert: [(2, OrderedDict([('@type', 'SoftwareApplication'), "*

 * *                           "('identifier', 'pyxdg'), ('name', 'pyxdg'), ('runtimePlatform', "*

 * *                           "'Python 3')]))]}",*

 * * "'version'": "'2024.7'"}*

```diff
@@ -54,14 +54,20 @@
             "@type": "SoftwareApplication",
             "identifier": "python-gitlab",
             "name": "python-gitlab",
             "runtimePlatform": "Python 3"
         },
         {
             "@type": "SoftwareApplication",
+            "identifier": "pyxdg",
+            "name": "pyxdg",
+            "runtimePlatform": "Python 3"
+        },
+        {
+            "@type": "SoftwareApplication",
             "identifier": "pyyaml",
             "name": "pyyaml",
             "runtimePlatform": "Python 3"
         },
         {
             "@type": "SoftwareApplication",
             "identifier": "requests",
@@ -97,9 +103,9 @@
         "@type": "CommandLineApplication",
         "description": "Update project metadata.",
         "executableName": "prometa",
         "name": "prometa",
         "runtimePlatform": "Python 3"
     },
     "url": "https://gitlab.inria.fr/jrye/prometa",
-    "version": "2024.6"
+    "version": "2024.7"
 }
```

### Comparing `prometa-2024.6/doc/Makefile` & `prometa-2024.7/doc/Makefile`

 * *Files identical despite different names*

### Comparing `prometa-2024.6/doc/make.bat` & `prometa-2024.7/doc/make.bat`

 * *Files identical despite different names*

### Comparing `prometa-2024.6/doc/source/conf.py` & `prometa-2024.7/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `prometa-2024.6/scripts/publish_documentation.sh` & `prometa-2024.7/scripts/publish_documentation.sh`

 * *Files identical despite different names*

### Comparing `prometa-2024.6/src/prometa/citation.py` & `prometa-2024.7/src/prometa/citation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 #!/usr/bin/env python
-'''
+"""
 Citation file format (.cff) functions.
 
 https://citation-file-format.github.io/
 https://github.com/citation-file-format/citation-file-format/blob/main/schema-guide.md
-'''
+"""
 
 
 import json
 
 import yaml
 
 from .file import update_content
 from .id.hal import get_hal_url_by_origin, get_hal_id_from_url
 from .id.swh import get_swhid_by_origin, get_swh_url_by_origin
 
 
-TEMPLATE = '''\
+TEMPLATE = """\
 cff-version: 1.2.0
 message: If you use this software, please cite it using these metadata.
 title: My Research Software
 abstract: This is my awesome research software. It does many things.
 authors:
   - family-names: Rye
     given-names: Jan-Michael
@@ -33,109 +33,118 @@
     type: doi
     value: "10.5281/zenodo.123456"
   - description: Archived snapshot of version 0.11.2 of My Research Software
     type: doi
     value: "10.5281/zenodo.123457"
 license: MIT
 repository-code: "https://github.com/citation-file-format/my-research-software"
-'''
+"""
 
 
-class Citation():
-    '''
+class Citation:
+    """
     Citation data manager.
-    '''
+    """
+
     def __init__(self, project):
-        '''
+        """
         Args:
             project:
                 A Project instance.
-        '''
+        """
         self.project = project
 
     @staticmethod
     def get_template():
-        '''
+        """
         Get the cff file template as an object.
-        '''
+        """
         return yaml.safe_load(TEMPLATE)
 
     @staticmethod
     def _transform_codemeta_authors(authors):
-        '''
+        """
         Transform the CodeMeta authors list to citation file format.
-        '''
+        """
         for author in authors:
             data = {}
             for cff_key, cm_key in (
-                ('family-names', 'familyName'),
-                ('given-names', 'givenName'),
-                ('email', 'email')
+                ("family-names", "familyName"),
+                ("given-names", "givenName"),
+                ("email", "email"),
             ):
                 data[cff_key] = author[cm_key]
-            author_id = author.get('@id')
-            if author_id and '//orcid.org/' in author_id:
-                data['orcid'] = author_id
+            author_id = author.get("@id")
+            if author_id and "//orcid.org/" in author_id:
+                data["orcid"] = author_id
             yield data
 
     def update(self):
-        '''
+        """
         Update the citation file with data from codemeta.json and other sources.
 
         Returns:
             The citation file object.
-        '''
+        """
         path = self.project.citation_cff_path
-        if not path.exists() and not self.project.config.get('citations_cff', default=False):
+        if not path.exists() and not self.project.config.get(
+            "citations_cff", default=False
+        ):
             return
         cff_data = self.get_template()
-        with self.project.codemeta_json_path.open('rb') as handle:
+        with self.project.codemeta_json_path.open("rb") as handle:
             cm_data = json.load(handle)
         for cff_key, cm_key in (
-            ('title', 'name'),
-            ('abstract', 'description'),
-            ('version', 'version'),
-            ('repository-code', 'codeRepository')
+            ("title", "name"),
+            ("abstract", "description"),
+            ("version", "version"),
+            ("repository-code", "codeRepository"),
         ):
             try:
                 cff_data[cff_key] = cm_data[cm_key]
             except KeyError:
                 del cff_data[cff_key]
 
         try:
-            cff_data['license'] = cm_data['license'].rsplit('/', 1)[1]
+            cff_data["license"] = cm_data["license"].rsplit("/", 1)[1]
         except KeyError:
-            del cff_data['license']
-        cff_data['authors'] = list(self._transform_codemeta_authors(cm_data['author']))
+            del cff_data["license"]
+        cff_data["authors"] = list(self._transform_codemeta_authors(cm_data["author"]))
 
-        identifiers = cff_data['identifiers']
+        identifiers = cff_data["identifiers"]
         identifiers.clear()
         git_url = self.project.git_repo.public_git_url
         swh_id = get_swhid_by_origin(git_url)
         if swh_id:
             # TODO
             # Uncomment once cff convert supports this.
             #  identifiers.append({
             #      'type': 'swh',
             #      'value': swh_id,
             #      'description': 'The Software Heritage identifier.'
             #  })
-            identifiers.append({
-                'type': 'url',
-                'value': get_swh_url_by_origin(git_url),
-                'description': 'The Software Heritage URL.'
-            })
+            identifiers.append(
+                {
+                    "type": "url",
+                    "value": get_swh_url_by_origin(git_url),
+                    "description": "The Software Heritage URL.",
+                }
+            )
             hal_url = get_hal_url_by_origin(git_url)
             if hal_url:
-                identifiers.append({
-                    'type': 'url',
-                    'value': hal_url,
-                    'description': 'HAL open science URL.'
-                })
-                identifiers.append({
-                    'type': 'other',
-                    'value': get_hal_id_from_url(hal_url),
-                    'description': 'HAL open science identifier.'
-                })
+                identifiers.append(
+                    {
+                        "type": "url",
+                        "value": hal_url,
+                        "description": "HAL open science URL.",
+                    }
+                )
+                identifiers.append(
+                    {
+                        "type": "other",
+                        "value": get_hal_id_from_url(hal_url),
+                        "description": "HAL open science identifier.",
+                    }
+                )
 
         content = yaml.dump(cff_data)
         update_content(content, path)
```

### Comparing `prometa-2024.6/src/prometa/codemeta.py` & `prometa-2024.7/src/prometa/codemeta/codemeta.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,158 +1,180 @@
 #!/usr/bin/env python
-'''
+"""
 CodeMeta functions.
-'''
+"""
 
 import contextlib
 import json
 import logging
-import pathlib
-import shutil
-import subprocess
-import tempfile
-import tomllib
-
-import tomli_w
-import tomli_w._writer
-
-from .file import diff
-from .id.orcid import get_orcid_url
-from .python.common import get_version
-from .python.venv import virtual_environment
+
+from ..exception import PrometaException
+from ..file import update_content
+from ..python.venv import VirtualEnvironment
 
 
 LOGGER = logging.getLogger(__name__)
 
 
+class CodeMetaError(PrometaException):
+    """
+    Custom exception raised when working with CodeMeta files.
+    """
+
+
 # https://codemeta.github.io/user-guide/
-class CodeMeta():
-    '''
-    Wrapper around the codemetapy command-line executable.
-    '''
+class CodeMeta:
+    """
+    Read and update CodeMeta files.
+    """
 
     def __init__(self, project):
-        '''
+        """
         Args:
             project:
                 The project object.
-        '''
+        """
         self.project = project
         self._data = None
 
+    def load(self):
+        """
+        Load the data from the CodeMeta file.
+        """
+        path = self.project.codemeta_json_path
+        LOGGER.debug("Loading CodeMeta data from %s", path)
+        try:
+            with path.open("rb") as handle:
+                self._data = json.load(handle)
+                return self._data
+        except FileNotFoundError:
+            return None
+        except (OSError, json.JSONDecodeError) as err:
+            raise CodeMetaError(err) from err
+
+    def update_file(self):
+        """
+        Update the CodeMeta file with the currently loaded data. If the file
+        already exists, a temporary file will be created and the merge tool will
+        be used to update the existing file.
+        """
+        path = self.project.codemeta_json_path
+        if self._data is None:
+            LOGGER.warning("No new data to update %s", path)
+            return
+        content = json.dumps(self._data, indent=2, sort_keys=True)
+        update_content(content, path)
+
     @property
     def data(self):
-        '''
+        """
         The CodeMeta data.
-        '''
+        """
         if self._data is None:
-            try:
-                with self.project.codemeta_json_path.open('rb') as handle:
-                    self._data = json.load(handle)
-            except FileNotFoundError:
-                return None
+            self.load()
         return self._data
 
     @property
     def name(self):
-        '''
+        """
         The project name.
-        '''
+        """
         try:
-            return self.data['name']
+            return self.data["name"]
         except TypeError:
             return None
 
-    @contextlib.contextmanager
-    def _modified_pyproject_toml(self):
-        '''
-        Context manager to create a temporary modified pyproject.toml file that
-        works around current bugs in CodeMetaPy. The origin of the problem is
-        that the project metadata now returns custom objects for the "readme"
-        and "license" fields while CodeMetaPy still expects these to be strings.
-        '''
-        with tempfile.TemporaryDirectory() as tmp_dir:
-            tmp_dir = pathlib.Path(tmp_dir)
-            git_dir = self.project.git_repo.path
-            shutil.copytree(git_dir, tmp_dir, dirs_exist_ok=True, symlinks=True)
-            ppt_path = git_dir / 'pyproject.toml'
-            tmp_ppt_path = tmp_dir / ppt_path.name
-
-            ppt_data = tomllib.loads(ppt_path.read_text(encoding='utf-8'))
-            for field in ('license', 'readme'):
-                try:
-                    del ppt_data['project'][field]
-                except KeyError:
-                    pass
-            content = tomli_w.dumps(ppt_data, multiline_strings=True)
-            tmp_ppt_path.write_text(content, encoding='utf-8')
-
-            yield tmp_ppt_path, ppt_data['project']['name']
-
-    def from_pyproject_toml(self, version=None):
-        '''
-        Update from a pyproject.toml file.
+    def _install_in_venv(self, venv):
+        """
+        Install CodeMetaPy in a Python virtual environment.
 
         Args:
-            version:
-                The version to set. This is necessary due to SCM incrementing
-                the version for unclean directories.
-        '''
-        author_data = []
-        for author in self.project.config.config['authors']:
-            data = {
-                '@type': 'Person',
-                'email': author['email'],
-                'givenName': author['given-names'],
-                'familyName': author['family-names']
-            }
-            orcid = author.get('orcid')
-            if orcid:
-                data['@id'] = get_orcid_url(orcid)
-            author_data.append(data)
+            venv:
+                An instance of VirtualEnvironment with its context currently
+                open.
+        """
+        # TODO
+        # Remove setuptools once CodeMetaPy is updated for Python > 3.12
+        venv.run_pip_in_venv([
+            "install",
+            "-U",
+            "CodeMetaPy",
+            "setuptools",
+        ])
+
+    def _run_codemeta_in_venv(self, venv, args, **kwargs):
+        """
+        Run a codemeta command in the virtual environment.
 
+        Args:
+            venv:
+                An instance of VirtualEnvironment with its context currently
+                open.
+
+            **kwargs:
+                Keyword arguments passed through to run_python_in_venv().
+
+        Returns:
+            The return value of run_python_in_venv().
+        """
+        # TODO
+        # Remove setuptools once CodeMetaPy is updated for Python > 3.12
+        return venv.run_python_in_venv(["-m", "codemeta.codemeta", *args], **kwargs)
+
+    def modify_codemeta_data(self, codemeta_data):
+        """
+        Modify the CodeMeta data. Override this method is a subclass to apply
+        custom modifications.
+
+        Args:
+            codemeta_data:
+                The input CodeMeta data.
+
+        Returns:
+            The possibly modified CodeMeta data.
+        """
+        return codemeta_data
+
+    def update(self, version=None, cwd=None, venv=None):
+        """
+        Update the CodeMeta file.
+
+        Args:
+            version:
+                The version to set. This is sometimes necessary to force a
+                version due to SCM incrementing the version for unclean
+                directories.
+
+            cwd:
+                The directory in which to run the codemeta command. If None, it
+                will default to the parent directory of the target codemeta.json
+                path.
+
+            venv:
+                An instance of VirtualEnvironment with the context currently
+                open. If None, a new instance will be created.
+        """
         codemeta_json_path = self.project.codemeta_json_path
-        with self._modified_pyproject_toml() as (tmp_ppt_path, name):
-            tmp_dir = tmp_ppt_path.parent
+        with contextlib.ExitStack() as stack:
+            if venv is None:
+                venv = stack.enter_context(VirtualEnvironment(update_pip=True, inherit=False))
+            self._install_in_venv(venv)
+            tmp_dir = venv.tmp_dir
             tmp_path = tmp_dir / codemeta_json_path.name
-            with virtual_environment(update_pip=True, inherit=False) as (_venv_dir, venv_exe):
-                cmd = [
-                    venv_exe,
-                    '-m', 'pip',
-                    'install', '-U',
-                    str(tmp_dir),
-                    # TODO
-                    # Remove setuptools once CodeMetaPy is updated for Python >
-                    # 3.12
-                    'CodeMetaPy', 'setuptools'
-                ]
-                LOGGER.debug('Running command: %s', cmd)
-                subprocess.run(cmd, check=True)
-                cmd = [
-                    venv_exe,
-                    '-m',
-                    'codemeta.codemeta',
-                    '--enrich',
-                    '-O', str(tmp_path)
-                ]
-                LOGGER.debug('Running command: %s', cmd)
-                subprocess.run(cmd, check=True, cwd=str(tmp_dir))
-            with tmp_path.open('rb') as handle:
+            if cwd is None:
+                cwd = codemeta_json_path.parent
+
+            self._run_codemeta_in_venv(
+                venv,
+                ["--enrich", "-O", str(tmp_path)],
+                cwd=cwd
+            )
+
+            with tmp_path.open("rb") as handle:
                 codemeta = json.load(handle)
-            codemeta['name'] = name
-            codemeta['author'] = author_data
-            codemeta['readme'] = self.project.git_repo.readme_url
-            codemeta['maintainer'] = author_data[0]
-            for cont in codemeta.get('contributor', []):
-                if all(
-                    cont[key] == author_data[0][key]
-                    for key in ('familyName', 'givenName')
-                ):
-                    cont.clear()
-                    cont.update(author_data[0])
             if version:
-                codemeta['version'] = version
+                codemeta["version"] = version
+            codemeta = self.modify_codemeta_data(codemeta)
             codemeta_text = json.dumps(codemeta, indent=2, sort_keys=True)
-            if not codemeta_text.endswith('\n'):
-                codemeta_text += '\n'
-            tmp_path.write_text(codemeta_text, encoding='utf-8')
-            diff(tmp_path, codemeta_json_path)
+            if not codemeta_text.endswith("\n"):
+                codemeta_text += "\n"
+            update_content(codemeta_text, codemeta_json_path)
```

### Comparing `prometa-2024.6/src/prometa/common.py` & `prometa-2024.7/src/prometa/common.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 #!/usr/bin/env python3
-'''
+"""
 Common constants and functions.
-'''
+"""
 
 import logging
 
 
-NAME = 'prometa'
+NAME = "prometa"
 LOGGER = logging.getLogger(__name__)
 
 
 def choose(items, include_none=False):
-    '''
+    """
     Prompt the user to choose an item from an iterable of items.
 
     Args:
         items:
             The iterable of items.
 
         include_none:
             If True, allow the user to choose None even if it is not in the
             list.
 
     Returns:
         The chosen item.
-    '''
+    """
     items = sorted(items)
     if include_none and None not in items:
         items.append(None)
     if not items:
-        LOGGER.warning('No items to choose.')
+        LOGGER.warning("No items to choose.")
         return None
     n_items = len(items)
     if n_items == 1:
         return items[0]
     while True:
-        print('Choose one of the following:')
+        print("Choose one of the following:")
         for i, item in enumerate(items, start=1):
-            print(f'{i:d} {item}')
-        choice = input(f'Enter an integer in the range 1-{n_items:d} and press enter. ')
+            print(f"{i:d} {item}")
+        choice = input(f"Enter an integer in the range 1-{n_items:d} and press enter. ")
         try:
             choice = int(choice)
         except ValueError:
             LOGGER.error('"%s" is not a valid integer.', choice)
             continue
         if choice < 1 or choice > n_items:
-            LOGGER.error('Invalid choice.')
+            LOGGER.error("Invalid choice.")
             continue
         return items[choice - 1]
```

### Comparing `prometa-2024.6/src/prometa/config.py` & `prometa-2024.7/src/prometa/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 #!/usr/bin/env python
-'''
+"""
 Configuration.
-'''
+"""
 
 
 import logging
 import os
 import pathlib
 import shlex
 
 import gitlab
 import yaml
+from xdg.BaseDirectory import xdg_config_dirs
 
 from .common import NAME
 from .exception import PrometaException
 
 LOGGER = logging.getLogger(__name__)
-CONFIG_FILE = f'{NAME}.yaml'
+CONFIG_FILE = f"{NAME}.yaml"
 
-CONFIG_EXAMPLE = '''
+CONFIG_EXAMPLE = """
 # A list of authors. They will appear in various files (e.g. pyproject.toml,
 # codemeta.json, CITATIONS.cff).
 authors:
     # Given names (required)
   - given-names: John
 
     # Family names (required)
@@ -39,23 +40,14 @@
 
     # HAL Open Science identifier (optional)
     hal: XXXXXXX
 
 # If true, create missing CITATIONS.cff files.
 citations_cff: true
 
-# By default, Prometa will attempt to detect each project's license using the
-# spdx-matcher Python package. In some cases the detection fails (e.g. GPL v2
-# and GPL v2-only use the same license text). This option can be set to an SPDX
-# license identifier (https://spdx.org/licenses/) to force a particular license
-# when the detection fails. If null or an empty strign then it will be ignored.
-#
-# Note that it will not modify license file.
-license: null
-
 # GitLab settings (optional)
 gitlab:
   # Prometa uses python-gitlab to manage GitLab hooks that push code to other
   # open repositories (currently only Software Heritage). python-gitlab requires
   # both a configuration file and the name of the section in the configuration
   # file to use for a given project. For details, see the documentation:
   #
@@ -91,43 +83,60 @@
   # To apply the same tags to all jobs, use the regular expression ".".
   ci_tags:
       ".":
         - tag1
         - tag2
         - tag3
 
+# By default, Prometa will attempt to detect each project's license using the
+# spdx-matcher Python package. In some cases the detection fails (e.g. GPL v2
+# and GPL v2-only use the same license text). This option can be set to an SPDX
+# license identifier (https://spdx.org/licenses/) to force a particular license
+# when the detection fails. If null or an empty strign then it will be ignored.
+#
+# Note that it will not download a new license file or modify the existing
+# license file.
+license: null
+
 # The utility to use when merging changes. It must accept two file paths (the
 # modified file and the original) and return non-zero exit status to indicate an
 # error or abort.
 merger: vimdiff
-'''.strip()
+
+
+# The README interpolator can insert command output into the README. To prevent
+# arbitrary command execution, Prometa will prompt the user to confirm a command
+# before it is executed. This prompt can be surpressed for trusted READMEs by
+# setting the following to true.
+trust_commands: false
+""".strip()
 
 
 class ConfigError(PrometaException):
-    '''
+    """
     Custom error raised by the Config class.
-    '''
+    """
 
 
 def _nested_values(data):
-    '''
+    """
     A generator over all nested values in a dict.
-    '''
+    """
     if not isinstance(data, dict):
         yield data
         return
     for value in data.values():
         if isinstance(value, dict):
             yield from _nested_values(value)
         else:
             yield value
 
 
 def _nested_update(old_data, new_data, origin, new_path):
-    '''
+    """
     Updated nested values in a configuration dict recursively.
 
     Args:
         old_data:
             The dict to update in place.
 
         new_data:
@@ -135,171 +144,206 @@
 
         origin:
             A dict of the same layout as old_data but the values are updated
             with the filenames that provided them.
 
         new_path:
             The path from which new_data was loaded.
-    '''
+    """
     for key, new_value in new_data.items():
         old_value = old_data.get(key)
         if isinstance(new_value, dict) and isinstance(old_value, dict):
             _nested_update(old_value, new_value, origin[key], new_path)
         else:
             old_data[key] = new_value
             origin[key] = new_path
 
 
-class Config():
-    '''
+class Config:
+    """
     Common non-derivable configuration.
-    '''
-    def __init__(self, proj_path, custom_config_paths=None):
-        '''
+    """
+
+    def __init__(self, proj_path, custom_config_paths=None, use_xdg=True, **overrides):
+        """
         Args:
             proj_path:
                 The project path.
 
             custom_config_paths:
                 An iterable over custon configuration file paths to use in
                 addition to the standard configuration files that Prometa
                 normally detects.
-        '''
+
+            use_xdg:
+                If True, search for configuration files in standard XDG
+                configuration directories. These files will be given the lowest
+                priority.
+
+            **overrides:
+                Custom run-time overrides that take precedence over values in
+                all discovered configuration files.
+        """
         self.proj_path = pathlib.Path(proj_path).resolve()
         if not custom_config_paths:
             custom_config_paths = []
-        self.custom_config_paths = [pathlib.Path(path).resolve() for path in custom_config_paths]
+        self.custom_config_paths = [
+            pathlib.Path(path).resolve() for path in custom_config_paths
+        ]
         self._config = None
         self._origin = None
+        self.use_xdg = use_xdg
+        self.overrides = overrides
 
     @property
-    def config_paths(self):
-        '''
-        A generator over configuration file paths. The files are located by
-        scanning the project directory and then all parent directories, with
-        files closer to the project directory taking precedence. This allows
-        common settings to be placed in a common root directory.
-        '''
+    def possible_config_paths(self):
+        """
+        A generator over the possible configuration file paths. Custom paths are
+        yielded first, in the order they were given. Next the possible visible
+        and hidden configuration paths in the current project directory and all
+        of its parent directories are yielded, starting with the project
+        directory and moving up to the root directory. Finally, if use_xdg is
+        True, the standard XDG configuration directories are yielded, again in
+        the standard order.
+
+        The generator does not check if the paths exist but it will omit
+        duplicate paths.
+        """
         yielded = set()
         for path in self.custom_config_paths:
-            if not path.exists():
-                LOGGER.warning('Custom configuration path %s does not exist.', path)
-                continue
             if path not in yielded:
-                LOGGER.info('Found configuration file: %s', path)
                 yield path
                 yielded.add(path)
         dir_path = self.proj_path
         while True:
-            for fname in (CONFIG_FILE, f'.{CONFIG_FILE}'):
+            for fname in (CONFIG_FILE, f".{CONFIG_FILE}"):
                 path = (dir_path / fname).resolve()
-                if path.exists() and path not in yielded:
-                    LOGGER.info('Found configuration file: %s', path)
+                if path not in yielded:
                     yield path
                     yielded.add(path)
             next_dir_path = dir_path.parent
             if dir_path != next_dir_path:
                 dir_path = next_dir_path
             else:
-                return
+                break
+        if self.use_xdg:
+            for config_dir in xdg_config_dirs:
+                path = pathlib.Path(config_dir) / NAME / CONFIG_FILE
+                if path not in yielded:
+                    yield path
+                    yielded.add(path)
+
+    @property
+    def config_paths(self):
+        """
+        A generator over existing configuration paths. It is a wrapper around
+        possible_config_paths that checks for and logs existence.
+        """
+        for path in self.possible_config_paths:
+            if path.exists():
+                yield path
 
     @property
     def config(self):
-        '''
+        """
         The configuration file object. If None, there is no configuration file.
 
         Raises:
             ConfigError:
                 One of the configuration files failed to load.
-        '''
+        """
         if self._config is None:
             configs = []
             for path in self.config_paths:
+                LOGGER.info("Loading configuration file: %s", path)
                 try:
-                    with path.open('r', encoding='utf-8') as handle:
+                    with path.open("r", encoding="utf-8") as handle:
                         data = yaml.safe_load(handle)
                 except (yaml.YAMLError, OSError) as err:
-                    raise ConfigError(f'Failed to load {path}: {err}') from err
+                    raise ConfigError(f"Failed to load {path}: {err}") from err
                 configs.append((path, data))
             final_config = {}
             origin = {}
             for path, config in reversed(configs):
                 _nested_update(final_config, config, origin, path)
+            _nested_update(final_config, self.overrides, origin, "overrides")
             self._config = final_config
             self._origin = origin
         return self._config
 
     def get(self, *keys, default=None):
-        '''
+        """
         Retrieve a configuration file value. This will scan the loaded
         configuration files in order and return the first match.
 
         Args:
             *keys:
                 The keys to the field. For example, to retrieve the value of
                 "bar" under "foo", call get("foo", "bar"). Integers may also be
                 used to index lists.
 
             default:
                 The default value to return if no value was found.
 
         Returns:
             The target value, or the default if no value was found.
-        '''
+        """
         config = self.config
         origin = self._origin
         for i, key in enumerate(keys):
             try:
                 config = config[key]
                 try:
                     origin = origin[key]
                 except TypeError:
                     pass
             except (KeyError, IndexError):
                 return default
             except TypeError as err:
                 paths = sorted(set(_nested_values(origin)))
                 LOGGER.error(
-                    'Failed to retrieve configuration value for %s: %s [%s]',
-                    keys[:i + 1],
+                    "Failed to retrieve configuration value for %s: %s [%s]",
+                    keys[: i + 1],
                     err,
-                    ', '.join(shlex.quote(str(p)) for p in paths)
+                    ", ".join(shlex.quote(str(p)) for p in paths),
                 )
                 return default
         return config
 
     def _get_origin(self, *keys):
-        '''
+        """
         Similar to get() but returns the origin path for the given keys.
-        '''
+        """
         origin = self._origin
         if isinstance(origin, pathlib.Path):
             return origin
         for key in keys:
             origin = origin[key]
-            if isinstance(origin, pathlib.Path):
+            if origin:
                 return origin
         return None
 
     @property
     def gitlab(self):
-        '''
+        """
         The python-gitlab GitLab instance from the current configuration.
-        '''
-        path = self.get('gitlab', 'config')
+        """
+        path = self.get("gitlab", "config")
         if path is None:
-            LOGGER.warning('No python-gitlab configuration file specified.')
-            path = os.getenv('PYTHON_GITLAB_CFG')
+            LOGGER.warning("No python-gitlab configuration file specified.")
+            path = os.getenv("PYTHON_GITLAB_CFG")
             if path is None:
-                LOGGER.warning('PYTHON_GITLAB_CFG environment variable is unset.')
+                LOGGER.warning("PYTHON_GITLAB_CFG environment variable is unset.")
                 return None
             path = pathlib.Path(path)
         else:
-            path = self._get_origin('gitlab', 'config').parent.joinpath(path)
+            origin_path = self._get_origin("gitlab", "config")
+            if isinstance(origin_path, pathlib.Path):
+                path = origin_path.resolve().parent.joinpath(path)
         path = path.resolve()
-        section = self.get('gitlab', 'section')
+        section = self.get("gitlab", "section")
         if not section:
             LOGGER.warning(
-                'No section specified for the python-gitlab configuration file: %s',
-                path
+                "No section specified for the python-gitlab configuration file: %s",
+                path,
             )
         return gitlab.Gitlab.from_config(section, [str(path)])
```

### Comparing `prometa-2024.6/src/prometa/file.py` & `prometa-2024.7/src/prometa/file.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,68 @@
 #!/usr/bin/env python3
-'''
+"""
 File operations.
-'''
+"""
 
 import filecmp
 import logging
 import pathlib
 import shutil
 import subprocess
 import tempfile
 
 
 LOGGER = logging.getLogger(__name__)
 
 
-def diff(path_1, path_2, differ='vimdiff'):
-    '''
+def diff(path_1, path_2, differ="vimdiff"):
+    """
     Diff 2 paths.
-    '''
+    """
     if not path_2.exists():
+        LOGGER.debug("Copying %s to %s", path_1, path_2)
         shutil.copy(path_1, path_2)
         return
     if not filecmp.cmp(path_1, path_2, shallow=False):
         #  if path_1.read_bytes().rstrip(b'\n') == path_2.read_bytes().rstrip(b'\n'):
         #      return
         cmd = [differ, str(path_1), str(path_2)]
-        LOGGER.info('Diffing %s and %s', path_1, path_2)
+        LOGGER.info("Diffing %s and %s", path_1, path_2)
         subprocess.run(cmd, check=True)
 
 
-def update_content(content, path, encoding='utf-8'):
-    '''
-    Interactively compare and merge new content.
+def update_content(content, path, encoding="utf-8", **kwargs):
+    """
+    Interactively compare and merge new content. If the target path does not
+    exist, the content will be written directly to it.
 
     Args:
         content:
             The new content to merge.
 
         path:
             The target path.
-    '''
+
+        encoding:
+            The file encoding to use when writing the content. If None, the
+            content is assumed to be bytes.
+
+        **kwargs:
+            Keyword arguments passed through to diff().
+    """
     path = pathlib.Path(path).resolve()
+    if not path.exists():
+        LOGGER.debug("Writing content to %s", path)
+        path.parent.mkdir(parents=True, exist_ok=True)
+        if encoding is None:
+            path.write_bytes(content)
+        else:
+            path.write_text(content, encoding=encoding)
     with tempfile.TemporaryDirectory() as tmp_dir:
         tmp_dir = pathlib.Path(tmp_dir)
-        tmp_path = tmp_dir / path.with_stem('new').name
-        tmp_path.write_text(content, encoding=encoding)
-        diff(tmp_path, path)
+        tmp_path = tmp_dir / path.with_stem("new").name
+        LOGGER.debug("Writing content to %s", tmp_path)
+        if encoding is None:
+            tmp_path.write_bytes(content)
+        else:
+            tmp_path.write_text(content, encoding=encoding)
+        diff(tmp_path, path, **kwargs)
```

### Comparing `prometa-2024.6/src/prometa/insert.py` & `prometa-2024.7/src/prometa/insert.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,111 +1,113 @@
 #!/usr/bin/env python3
-'''
+"""
 Base class for inserting content into text files.
-'''
+"""
 
 import pathlib
 import re
 
 
 from .file import update_content
 
 
-class Inserter():
-    '''
+class Inserter:
+    """
     Insert updated content into a text file.
-    '''
+    """
+
     def __init__(self, regex):
-        '''
+        """
         Args:
             regex:
                 A compiled regular expression.
-        '''
+        """
         self.regex = regex
 
     def insert(self, match):
-        '''
+        """
         Given a regular expression match, return the content to insert.
 
         Args:
             match:
                 The Match object.
 
         Returns:
             The string to substitute for the match.
-        '''
+        """
         return match.group(0)
 
-    def update(self, path, encoding='utf-8'):
-        '''
+    def update(self, path, encoding="utf-8"):
+        """
         Insert the configured content into the file.
-        '''
+        """
         text = pathlib.Path(path).resolve().read_text(encoding=encoding)
         text = self.regex.sub(self.insert, text)
         update_content(text, path)
 
 
 class MarkdownInserter(Inserter):
-    '''
+    """
     Inserter with custom regex for invisible comments in Markdown files.
 
     In Markdown, a link label for a simple hash results in no output for most
     common Markdown processors: "[comment]: #". Note that these must be
     proceeded by blank lines to be recognized in Markdown.
 
     This class recognized blocks that begin with a comment prefixed with
     "insert: " and end with a comment containing only "/insert". Both comments
     must have the same indentation level and the inserted text will be indented
     to the same level.
-    '''
+    """
+
     def __init__(self):
         regex = re.compile(
-            r'^(?P<indent>[ \t]*)\[insert: (?P<label>.+?)\]: #\n'
-            r'(?:(?P<content>.*?)\n)?'
-            r'^(?P=indent)\[/insert: (?P=label)]: #\n',
-            re.MULTILINE | re.DOTALL
+            r"^(?P<indent>[ \t]*)\[insert: (?P<label>.+?)\]: #\n"
+            r"(?:(?P<content>.*?)\n)?"
+            r"^(?P=indent)\[/insert: (?P=label)]: #\n",
+            re.MULTILINE | re.DOTALL,
         )
         super().__init__(regex)
 
     @staticmethod
     def get_link(label, url):
-        '''
+        """
         Get the Markdown link.
 
         Args:
             label:
                 The label shown for the link.
 
             url:
                 The URL of the link.
 
         Return:
             The Markdown link as a string.
-        '''
-        return f'[{label}]({url})'
+        """
+        return f"[{label}]({url})"
 
     def get_output(self, label, content):  # pylint: disable=unused-argument
-        '''
+        """
         Get output to replace the given label. Override this to insert custom
         content.
 
         Args:
             label:
                 The label in the comment pair that was matched.
 
             content:
                 The content between the matched comments.
 
         Returns:
             The content to insert, or None if the label was not recognized.
-        '''
+        """
         return None
 
     def insert(self, match):
-        indent = match['indent']
-        label = match['label'].strip()
-        content = match['content']
+        indent = match["indent"]
+        label = match["label"].strip()
+        content = match["content"]
         output = self.get_output(label, content)  # pylint: disable=assignment-from-none
         if output is None:
             return match.group(0)
-        output = '\n'.join(f'{indent}{line}' for line in output.strip('\n').split('\n'))
-        return f'{indent}[insert: {label}]: #\n\n{output}\n\n{indent}[/insert: {label}]: #\n'
+        output = "\n".join(f"{indent}{line}" for line in output.strip("\n").split("\n"))
+        return f"{indent}[insert: {label}]: #\n\n{output}\n\n{indent}[/insert: {label}]: #\n"
```

### Comparing `prometa-2024.6/src/prometa/project.py` & `prometa-2024.7/src/prometa/project.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,161 +1,164 @@
 #!/usr/bin/env python
-'''
+"""
 Project class.
-'''
+"""
 
 import logging
 
 import spdx_matcher
 from spdx_license_list import LICENSES as SPDX_LICENSES
 
 from .citation import Citation
 from .common import choose
-from .codemeta import CodeMeta
+from .codemeta.codemeta import CodeMeta
+from .codemeta.pyproject import PyprojectCodeMeta
 from .config import Config
 from .gitlab.ci import GitlabCI
 from .gitlab.repo import GitlabRepo
 from .python.common import update_pyproject_toml, get_version
 from .readme import ReadmeInserter
 
 
 LOGGER = logging.getLogger(__name__)
 
 
-class Project():
-    '''
+class Project:
+    """
     Project class.
-    '''
-    def __init__(self, path, trust_commands=False, custom_config_paths=None):
-        '''
+    """
+
+    def __init__(self, path, **config_kwargs):
+        """
         Args:
             path:
                 The path to the project.
 
-            custom_config_paths:
-                Passed through to Config.
-        '''
+            **config_kwargs:
+                Keyword arguments passed through to Config.
+        """
         self.git_repo = GitlabRepo(path)
         self.gitlab_ci = GitlabCI(self)
-        self.config = Config(self.git_repo.path, custom_config_paths=custom_config_paths)
-        self.trust_commands = trust_commands
+        self.config = Config(self.git_repo.path, **config_kwargs)
         self.codemeta = CodeMeta(self)
 
     @property
     def readme_md_path(self):
-        '''
+        """
         The README.md path.
-        '''
-        return self.git_repo.path / 'README.md'
+        """
+        return self.git_repo.path / "README.md"
 
     @property
     def pyproject_toml_path(self):
-        '''
+        """
         The pyproject.toml path.
-        '''
-        return self.git_repo.path / 'pyproject.toml'
+        """
+        return self.git_repo.path / "pyproject.toml"
 
     @property
     def license_txt_path(self):
-        '''
+        """
         The path to the LICENSE.txt file.
-        '''
-        return self.git_repo.path / 'LICENSE.txt'
+        """
+        return self.git_repo.path / "LICENSE.txt"
 
     @property
     def spdx_license(self):
-        '''
+        """
         The detected SPDX license name.
-        '''
-        config_license = self.config.get('license')
+        """
+        config_license = self.config.get("license")
         if config_license:
-            LOGGER.info('Using license from configuration file: %s', config_license)
+            LOGGER.info("Using license from configuration file: %s", config_license)
             if config_license not in SPDX_LICENSES:
                 LOGGER.warning('"%s" is not a recognized SPDX license', config_license)
             return config_license
         path = self.license_txt_path
-        LOGGER.info('Attempting to detect license from %s', path)
+        LOGGER.info("Attempting to detect license from %s", path)
         try:
-            detected, percent = spdx_matcher.analyse_license_text(path.read_text(encoding='utf-8'))
+            detected, percent = spdx_matcher.analyse_license_text(
+                path.read_text(encoding="utf-8")
+            )
         except FileNotFoundError:
-            LOGGER.error('No license file found at %s', path)
+            LOGGER.error("No license file found at %s", path)
             return None
-        licenses = list(detected['licenses'])
+        licenses = list(detected["licenses"])
         if not licenses:
-            LOGGER.error('Failed to detect license in %s', path)
+            LOGGER.error("Failed to detect license in %s", path)
             return None
         lic = choose(licenses)
         if percent < 0.9:
             LOGGER.warning(
-                'Detected %s license in %s but certainty is only %(0.0f) %',
+                "Detected %s license in %s but certainty is only %(0.0f) %",
                 lic,
                 path,
-                percent * 100.
+                percent * 100.0,
             )
         return lic
 
     @property
     def codemeta_json_path(self):
-        '''
+        """
         The path to the codemeta.json file.
-        '''
-        return self.git_repo.path / 'codemeta.json'
+        """
+        return self.git_repo.path / "codemeta.json"
 
     @property
     def citation_cff_path(self):
-        '''
+        """
         The path to the CITATION.cff file.
-        '''
-        return self.git_repo.path / 'CITATION.cff'
+        """
+        return self.git_repo.path / "CITATION.cff"
 
     @property
     def urls(self):
-        '''
+        """
         A dict of URLs for the project.
-        '''
+        """
         host, namespace, name = self.git_repo.parsed_origin
-        homepage = f'https://{host}/{namespace}/{name}'
+        homepage = f"https://{host}/{namespace}/{name}"
 
         urls = {}
-        urls['Homepage'] = homepage
-        urls['Source'] = f'{homepage}.git'
-        if self.gitlab_ci.data.get('pages'):
-            pages_fmt = self.config.get('gitlab', 'pages_urls', host)
+        urls["Homepage"] = homepage
+        urls["Source"] = f"{homepage}.git"
+        if self.gitlab_ci.data.get("pages"):
+            pages_fmt = self.config.get("gitlab", "pages_urls", host)
             if pages_fmt:
-                urls['Documentation'] = pages_fmt.format(namespace=namespace, name=name)
-        urls['Issues'] = f'{homepage}/-/issues'
+                urls["Documentation"] = pages_fmt.format(namespace=namespace, name=name)
+        urls["Issues"] = f"{homepage}/-/issues"
         return urls
 
     def update(self):
-        '''
+        """
         Update project metadata.
-        '''
+        """
         if self.pyproject_toml_path.exists():
             # TODO
             # Find a better way to automate version management while updating
             # the files. The issue is that prometa has to modify several files
             # but these modifications are visible to the VCS. This causes tools
             # such as setuptools-scm to miscalculate the version because it
             # doesn't know that the changes will be merged into the previous
             # commit.
             version = get_version(self.git_repo.path)
             update_pyproject_toml(self)
-            self.codemeta.from_pyproject_toml(version=version)
+            PyprojectCodeMeta(self).update(version=version)
 
         if self.codemeta_json_path.exists():
             Citation(self).update()
 
         readme_inserter = ReadmeInserter(self)
         readme_inserter.update(self.readme_md_path)
 
         self.gitlab_ci.update()
 
     @property
     def name(self):
-        '''
+        """
         The project name. It will use the value in codemeta.name if it exists,
         otherwise it will use the name of the project's directory.
-        '''
+        """
         name = self.codemeta.name
         if name is not None:
             return name
         return self.git_repo.path.name
```

### Comparing `prometa-2024.6/src/prometa/readme.py` & `prometa-2024.7/src/prometa/readme.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python3
-'''
+"""
 Insert data into the README.
-'''
+"""
 
 import logging
 import shlex
 import subprocess
 import tomllib
 
 from .id.hal import get_hal_url_by_origin
@@ -14,168 +14,171 @@
 from .python.common import get_pypi_url
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 class ReadmeInserter(MarkdownInserter):
-    '''
+    """
     Insert data into the Markdown file.
-    '''
+    """
+
     def __init__(self, project):
         super().__init__()
         self.project = project
         self._labels_found = set()
 
     @staticmethod
     def _split_level(label):
-        '''
+        """
         Extract the header level from a label.
 
         Args:
             label:
                 A string with the label and header leavel in format "<label>
                 <level>".
 
         Returns:
             The label and the level. If no level was found, the level defaults
             to 1.
-        '''
+        """
         label = label.strip()
         try:
             label, level = label.split(None, 1)
         except ValueError:
-            LOGGER.debug('Missing header level in label [%s]: assuming 1', label)
+            LOGGER.debug("Missing header level in label [%s]: assuming 1", label)
             return label, 1
         return label, int(level)
 
     @staticmethod
     def _get_lang_and_command(label):
-        '''
+        """
         Extract command and optional language from the label.
 
         Args:
             label:
                 A string of the format "command[:<lang>] <cmd>", e.g. "command
                 echo test" or "command:yaml some_cmd_to_print_yaml". The command
                 string will be parsed by shlex.split().
 
         Returns:
             The language and the command. The language will be None if not found
             and the command will be a list of command words.
-        '''
+        """
         label, command = label.split(None, 1)
         try:
-            label, lang = label.split(':', 1)
+            label, lang = label.split(":", 1)
             lang = lang.strip()
         except ValueError:
             lang = None
         return lang, shlex.split(command)
 
     def _get_links_section(self, label):
-        '''
+        """
         Get the section containing standard links.
-        '''
+        """
         label, level = self._split_level(label)
-        header_prefix = '#' * (level + 1)
+        header_prefix = "#" * (level + 1)
         is_pyproject = self.project.pyproject_toml_path.exists()
 
-        lines = [f'{header_prefix} GitLab', '']
+        lines = [f"{header_prefix} GitLab", ""]
 
         lines.extend(
             self.get_link(name.title(), link)
             for name, link in self.project.urls.items()
         )
 
         other_repos = []
         if is_pyproject:
-            lines.append(self.get_link(
-                'GitLab package registry',
-                self.project.git_repo.get_section_url('packages')
-            ))
+            lines.append(
+                self.get_link(
+                    "GitLab package registry",
+                    self.project.git_repo.get_section_url("packages"),
+                )
+            )
             pyproj_data = tomllib.loads(
-                self.project.pyproject_toml_path.read_text(encoding='utf-8')
+                self.project.pyproject_toml_path.read_text(encoding="utf-8")
             )
-            pypi_url = get_pypi_url(pyproj_data['project']['name'])
+            pypi_url = get_pypi_url(pyproj_data["project"]["name"])
             if pypi_url:
-                other_repos.append(self.get_link('Python Package Index', pypi_url))
+                other_repos.append(self.get_link("Python Package Index", pypi_url))
 
         origin_url = self.project.git_repo.public_git_url
         if swh_project_exists(origin_url):
             other_repos.append(
-                self.get_link('Software Heritage', get_swh_url_by_origin(origin_url))
+                self.get_link("Software Heritage", get_swh_url_by_origin(origin_url))
             )
 
         hal_url = get_hal_url_by_origin(origin_url)
         if hal_url:
-            other_repos.append(self.get_link('HAL open science', hal_url))
+            other_repos.append(self.get_link("HAL open science", hal_url))
 
         if other_repos:
-            lines.extend((
-                '',
-                f'{header_prefix} Other Repositories',
-                '',
-                *other_repos
-            ))
-
-        return '\n'.join(
-            line if not line or line.startswith('#') else f'* {line}'
-            for line in lines
+            lines.extend(("", f"{header_prefix} Other Repositories", "", *other_repos))
+
+        return "\n".join(
+            line if not line or line.startswith("#") else f"* {line}" for line in lines
         )
 
     def _get_citation_section(self, _label):
-        '''
+        """
         Get the section containing citation examples for different targets.
-        '''
+        """
         path = self.project.citation_cff_path
         citation_cff_url = self.project.git_repo.get_main_blob_url(path.name)
         blocks = [
-            'Please cite this software using the metadata provided in '
-            f'[{path.name}]({citation_cff_url}). '
-            'The following extracts are provided for different applications.',
-            ''
+            "Please cite this software using the metadata provided in "
+            f"[{path.name}]({citation_cff_url}). "
+            "The following extracts are provided for different applications.",
+            "",
         ]
         if path.exists():
-            for fmt in ('cff', 'apalike', 'bibtex', 'endnote', 'ris', 'schema.org', 'zenodo'):
-                cmd = ['cffconvert', '-i', str(path), '-f', fmt]
-                LOGGER.debug('Converting %s to %s', path, fmt)
+            for fmt in (
+                "cff",
+                "apalike",
+                "bibtex",
+                "endnote",
+                "ris",
+                "schema.org",
+                "zenodo",
+            ):
+                cmd = ["cffconvert", "-i", str(path), "-f", fmt]
+                LOGGER.debug("Converting %s to %s", path, fmt)
                 output = subprocess.run(
                     cmd,
                     check=True,
                     stdout=subprocess.PIPE,
                 ).stdout.decode()
-                blocks.append(f'{fmt}\n: ~~~\n{output.strip()}\n~~~\n')
-        return '\n'.join(blocks)
+                blocks.append(f"{fmt}\n: ~~~\n{output.strip()}\n~~~\n")
+        return "\n".join(blocks)
 
     def _get_command_output_section(self, label):
-        '''
+        """
         Get the output of a command.
-        '''
+        """
         lang, command = self._get_lang_and_command(label)
-        if not self.project.trust_commands:
-            ans = input(f'Run command {command}? [y/N] ')
-            if ans.strip().lower() != 'y':
-                LOGGER.info('Skipping command %s', command)
+        if not self.project.config.get("trust_commands", default=False):
+            ans = input(f"Run command {command}? [y/N] ")
+            if ans.strip().lower() != "y":
+                LOGGER.info("Skipping command %s", command)
                 return None
-        LOGGER.info('Running command: %s', command)
+        LOGGER.info("Running command: %s", command)
         output = subprocess.run(
-            command,
-            check=True,
-            stdout=subprocess.PIPE
+            command, check=True, stdout=subprocess.PIPE
         ).stdout.decode()
-        lang = lang if lang else ''
-        return f'~~~{lang}\n$ {shlex.join(command)}\n{output}\n~~~\n'
+        lang = lang if lang else ""
+        return f"~~~{lang}\n$ {shlex.join(command)}\n{output}\n~~~\n"
 
     def get_output(self, label, content):
-        '''
+        """
         Override parent get_output.
-        '''
+        """
         self._labels_found.add(label)
-        if label.startswith('citations'):
+        if label.startswith("citations"):
             return self._get_citation_section(label)
-        if label.startswith('links'):
+        if label.startswith("links"):
             return self._get_links_section(label)
-        if label.startswith('command_output'):
+        if label.startswith("command_output"):
             output = self._get_command_output_section(label)
             return content if output is None else output
-        LOGGER.warning('Unhandled label in README: %s', label)
+        LOGGER.warning("Unhandled label in README: %s", label)
         return content
```

### Comparing `prometa-2024.6/src/prometa/gitlab/repo.py` & `prometa-2024.7/src/prometa/gitlab/repo.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,120 +1,122 @@
 #!/usr/bin/env python
-'''
+"""
 Git functions.
-'''
+"""
 
 import logging
 import pathlib
 import subprocess
 
 
 LOGGER = logging.getLogger(__name__)
 
 
-class GitlabRepo():
-    '''
+class GitlabRepo:
+    """
     Basic functionality for retrieving Git information.
-    '''
+    """
 
-    def __init__(self, path, remote='origin'):
-        '''
+    def __init__(self, path, remote="origin"):
+        """
         Args:
             path:
                 A path to the Git repository or any non-submodule path within
                 it.
 
             remote:
                 The remote repository name to use for generating URLs.
-        '''
+        """
         self.path = pathlib.Path(path).resolve()
         self.path = self.top_level
         self.remote = remote
         self._origin_url = None
 
     def run_cmd(self, cmd):
-        '''
+        """
         Run a git command and return its output.
 
         Args:
             cmd:
                 The git sub-command and arguments.
 
         Returns:
             The command output.
-        '''
-        cmd = ('git', '-C', str(self.path), *cmd)
-        LOGGER.debug('Running command: %s', cmd)
-        return subprocess.run(cmd, check=True, capture_output=True).stdout.decode().strip()
+        """
+        cmd = ("git", "-C", str(self.path), *cmd)
+        LOGGER.debug("Running command: %s", cmd)
+        return (
+            subprocess.run(cmd, check=True, capture_output=True).stdout.decode().strip()
+        )
 
     @property
     def top_level(self):
-        '''
+        """
         The top-level directory.
-        '''
-        path = self.run_cmd(('rev-parse', '--show-toplevel'))
+        """
+        path = self.run_cmd(("rev-parse", "--show-toplevel"))
         return pathlib.Path(path).resolve()
 
     @property
     def remote_url(self):
-        '''
+        """
         The origin URL.
-        '''
+        """
         if self._origin_url is None:
-            self._origin_url = self.run_cmd(('config', '--get', 'remote.origin.url'))
+            self._origin_url = self.run_cmd(("config", "--get", "remote.origin.url"))
         return self._origin_url
 
     @property
     def parsed_origin(self):
-        '''
+        """
         A 3-tuple of the origin's host, namespace and project name.
-        '''
-        host, subpath = self.remote_url.split(':', 1)
-        subpath = subpath.rsplit('.', 1)[0]
-        namespace, name = subpath.split('/', 1)
-        host = host.split('@', 1)[1]
+        """
+        host, subpath = self.remote_url.split(":", 1)
+        subpath = subpath.rsplit(".", 1)[0]
+        namespace, name = subpath.split("/", 1)
+        host = host.split("@", 1)[1]
         return host, namespace, name
 
     @property
     def public_url(self):
-        '''
+        """
         The URL for the main project page.
-        '''
+        """
         host, namespace, name = self.parsed_origin
-        return f'https://{host}/{namespace}/{name}'
+        return f"https://{host}/{namespace}/{name}"
 
     def get_section_url(self, section):
-        '''
+        """
         The URL to one of the various GitLab sections, e.g. "blob/main" or
         "packages".
-        '''
+        """
         section = section.lstrip()
-        return f'{self.public_url}/-/{section}'
+        return f"{self.public_url}/-/{section}"
 
     @property
     def public_git_url(self):
-        '''
+        """
         The publically accessible HTTPS URL.
-        '''
-        return f'{self.public_url}.git'
+        """
+        return f"{self.public_url}.git"
 
     def get_main_blob_url(self, path):
-        '''
+        """
         Get the main branch URL to the given path.
-        '''
-        path = path.lstrip('/')
-        return self.get_section_url(f'blob/main/{path}')
+        """
+        path = path.lstrip("/")
+        return self.get_section_url(f"blob/main/{path}")
 
     @property
     def readme_url(self):
-        '''
+        """
         The URL to the README.
-        '''
-        return self.get_main_blob_url('README.md')
+        """
+        return self.get_main_blob_url("README.md")
 
     def get_gitlab_project(self, glab):
-        '''
+        """
         Get the python-gitlab Project instance from a python-gitlab GitLab
         instance.
-        '''
+        """
         _host, namespace, name = self.parsed_origin
-        return glab.projects.get(f'{namespace}/{name}')
+        return glab.projects.get(f"{namespace}/{name}")
```

### Comparing `prometa-2024.6/src/prometa/id/hal.py` & `prometa-2024.7/src/prometa/id/hal.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 #!/usr/bin/env python
-'''
+"""
 HAL open science functions.
 
 https://api.archives-ouvertes.fr/docs/search
-'''
+"""
 
 import logging
 from urllib.parse import quote as urlquote
 
 import requests
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 def get_hal_url_by_origin(origin):
-    '''
+    """
     Get the HAL ID by origin.
-    '''
+    """
     cache = get_hal_url_by_origin.cache
     try:
         return cache[origin]
     except KeyError:
         pass
 
     timeout = 5
-    query = origin.split('://', 1)[1]
-    search_url = f'https://api.archives-ouvertes.fr/search/?q={urlquote(query)}'
-    LOGGER.debug('Querying %s', search_url)
+    query = origin.split("://", 1)[1]
+    search_url = f"https://api.archives-ouvertes.fr/search/?q={urlquote(query)}"
+    LOGGER.debug("Querying %s", search_url)
     resp = requests.get(search_url, timeout=timeout).json()
-    for doc in resp['response']['docs']:
-        label = doc['label_s']
-        if f'origin={origin};' in label:
-            url = doc['uri_s']
+    for doc in resp["response"]["docs"]:
+        label = doc["label_s"]
+        if f"origin={origin};" in label:
+            url = doc["uri_s"]
             cache[origin] = url
             return url
     return None
 
 
 get_hal_url_by_origin.cache = {}
 
 
 def get_hal_id_from_url(url):
-    '''
+    """
     Extract the HAL ID from a HAL URL.
-    '''
-    return url.rsplit('/', 1)[1]
+    """
+    return url.rsplit("/", 1)[1]
```

### Comparing `prometa-2024.6/src/prometa/id/swh.py` & `prometa-2024.7/src/prometa/id/swh.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,76 +1,78 @@
 #!/usr/bin/env python
-'''
+"""
 Software Heritage functions.
-'''
+"""
 
 import logging
 from urllib.parse import quote as urlquote
 
 import requests
 
 
 LOGGER = logging.getLogger(__name__)
 
 
 def get_swhid_by_origin(origin):
-    '''
+    """
     Get a Software Heritage ID from an origin URL. This only includes the origin
     and repository ID.
 
     Args:
         origin:
             The origin URL of the software project.
 
     Returns:
         A Software Heritage ID string.
-    '''
+    """
     cache = get_swhid_by_origin.cache
     try:
         return cache[origin]
     except KeyError:
         pass
 
     timeout = 5
-    url = f'https://archive.softwareheritage.org/api/1/origin/{origin}/get/'
-    LOGGER.debug('Querying %s', url)
+    url = f"https://archive.softwareheritage.org/api/1/origin/{origin}/get/"
+    LOGGER.debug("Querying %s", url)
     resp = requests.get(url, timeout=timeout).json()
     try:
-        resp = requests.get(resp['origin_visits_url'], timeout=timeout).json()
-        resp = requests.get(resp[0]['snapshot_url'], timeout=timeout).json()
-        resp = requests.get(resp['branches']['HEAD']['target_url'], timeout=timeout).json()
+        resp = requests.get(resp["origin_visits_url"], timeout=timeout).json()
+        resp = requests.get(resp[0]["snapshot_url"], timeout=timeout).json()
+        resp = requests.get(
+            resp["branches"]["HEAD"]["target_url"], timeout=timeout
+        ).json()
         swhid = f'swh:1:dir:{resp["directory"]};origin={urlquote(origin)}'
         cache[origin] = swhid
         return swhid
     except KeyError:
         return None
 
 
 get_swhid_by_origin.cache = {}
 
 
 def get_swh_url_by_origin(origin):
-    '''
+    """
     Get a Software Heritage link for an origin URL.
 
     Args:
         origin:
             The origin URL of the software project.
 
     Returns:
         A Software Heritage URL. The page may not exist.
-    '''
-    return f'https://archive.softwareheritage.org/browse/origin/?origin_url={urlquote(origin)}'
+    """
+    return f"https://archive.softwareheritage.org/browse/origin/?origin_url={urlquote(origin)}"
 
 
 def swh_project_exists(origin):
-    '''
+    """
     Check if the project exists on Software Heritage.
 
     Args:
         origin:
             The origin URL of the software project.
 
     Returns:
         True if the project exists, False otherwise.
-    '''
+    """
     return get_swhid_by_origin(origin) is not None
```

### Comparing `prometa-2024.6/LICENSE.txt` & `prometa-2024.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prometa-2024.6/README.md` & `prometa-2024.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -66,23 +66,14 @@
 
     # HAL Open Science identifier (optional)
     hal: XXXXXXX
 
 # If true, create missing CITATIONS.cff files.
 citations_cff: true
 
-# By default, Prometa will attempt to detect each project's license using the
-# spdx-matcher Python package. In some cases the detection fails (e.g. GPL v2
-# and GPL v2-only use the same license text). This option can be set to an SPDX
-# license identifier (https://spdx.org/licenses/) to force a particular license
-# when the detection fails. If null or an empty strign then it will be ignored.
-#
-# Note that it will not modify license file.
-license: null
-
 # GitLab settings (optional)
 gitlab:
   # Prometa uses python-gitlab to manage GitLab hooks that push code to other
   # open repositories (currently only Software Heritage). python-gitlab requires
   # both a configuration file and the name of the section in the configuration
   # file to use for a given project. For details, see the documentation:
   #
@@ -118,19 +109,36 @@
   # To apply the same tags to all jobs, use the regular expression ".".
   ci_tags:
       ".":
         - tag1
         - tag2
         - tag3
 
+# By default, Prometa will attempt to detect each project's license using the
+# spdx-matcher Python package. In some cases the detection fails (e.g. GPL v2
+# and GPL v2-only use the same license text). This option can be set to an SPDX
+# license identifier (https://spdx.org/licenses/) to force a particular license
+# when the detection fails. If null or an empty strign then it will be ignored.
+#
+# Note that it will not download a new license file or modify the existing
+# license file.
+license: null
+
 # The utility to use when merging changes. It must accept two file paths (the
 # modified file and the original) and return non-zero exit status to indicate an
 # error or abort.
 merger: vimdiff
 
+
+# The README interpolator can insert command output into the README. To prevent
+# arbitrary command execution, Prometa will prompt the user to confirm a command
+# before it is executed. This prompt can be surpressed for trusted READMEs by
+# setting the following to true.
+trust_commands: false
+
 ~~~
 
 [/insert: command_output:yaml prometa --gen-config -]: #
 
 ## README Content Insertion
 
 Content can be inserted into the README.md file using invisible comments of the format:
@@ -169,15 +177,16 @@
 
 # Usage
 
 [insert: command_output prometa -h]: #
 
 ~~~
 $ prometa -h
-usage: prometa [-h] [--config PATH [PATH ...]] [--gen-config PATH] [--trust]
+usage: prometa [-h] [--config PATH [PATH ...]] [--gen-config PATH]
+               [--list-config {all,existing}] [--no-xdg] [--trust]
                [path ...]
 
 Update project metadata.
 
 positional arguments:
   path                  Path to project directory.
 
@@ -193,14 +202,22 @@
                         take precedence over the detected configuration files.
                         If multiple configuration paths are given with this
                         command, their order determines their precedence.
   --gen-config PATH     Generate a configuration file template at the given
                         path. If the path is "-", the file will be printed to
                         STDOUT. Note that prometa will only look for files
                         named "prometa.yaml" or ".prometa.yaml".
+  --list-config {all,existing}
+                        List either all paths that will be scanned for
+                        configuration files for each given project, or only
+                        existing ones. The output is printed as a YAML file
+                        mapping project directory paths to lists of possible
+                        configuration files.
+  --no-xdg              Disable loading of configuration files in standard XDG
+                        locations.
   --trust               It is possible to insert arbitrary command output into
                         the README file. By default, prometa will prompt the
                         user for confirmation before running the command to
                         prevent arbitrary code execution in the context of a
                         collaborative environment. This option can be used to
                         disable the prompt if the user trusts all of the
                         commands in the README.
```

### Comparing `prometa-2024.6/pyproject.toml` & `prometa-2024.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 [project]
 name = "Prometa"
 description = "Manage project metadata."
 dependencies = [
     "CodeMetaPy",
     "PyYAML",
     "python-gitlab",
+    "pyxdg",
     "requests",
     "spdx-license-list",
     "spdx-matcher",
     "tomli-w",
     "trove-classifiers",
 ]
 requires-python = ">=3.6"
```

### Comparing `prometa-2024.6/PKG-INFO` & `prometa-2024.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: Prometa
-Version: 2024.6
+Version: 2024.7
 Summary: Manage project metadata.
 Project-URL: Homepage, https://gitlab.inria.fr/jrye/prometa
 Project-URL: Source, https://gitlab.inria.fr/jrye/prometa.git
 Project-URL: Documentation, https://jrye.gitlabpages.inria.fr/prometa
 Project-URL: Issues, https://gitlab.inria.fr/jrye/prometa/-/issues
 Author-email: Jan-Michael Rye <jan-michael.rye@inria.fr>
 License: MIT License
@@ -19,14 +19,15 @@
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Requires-Dist: codemetapy
 Requires-Dist: python-gitlab
+Requires-Dist: pyxdg
 Requires-Dist: pyyaml
 Requires-Dist: requests
 Requires-Dist: spdx-license-list
 Requires-Dist: spdx-matcher
 Requires-Dist: tomli-w
 Requires-Dist: trove-classifiers
 Description-Content-Type: text/markdown
@@ -99,23 +100,14 @@
 
     # HAL Open Science identifier (optional)
     hal: XXXXXXX
 
 # If true, create missing CITATIONS.cff files.
 citations_cff: true
 
-# By default, Prometa will attempt to detect each project's license using the
-# spdx-matcher Python package. In some cases the detection fails (e.g. GPL v2
-# and GPL v2-only use the same license text). This option can be set to an SPDX
-# license identifier (https://spdx.org/licenses/) to force a particular license
-# when the detection fails. If null or an empty strign then it will be ignored.
-#
-# Note that it will not modify license file.
-license: null
-
 # GitLab settings (optional)
 gitlab:
   # Prometa uses python-gitlab to manage GitLab hooks that push code to other
   # open repositories (currently only Software Heritage). python-gitlab requires
   # both a configuration file and the name of the section in the configuration
   # file to use for a given project. For details, see the documentation:
   #
@@ -151,19 +143,36 @@
   # To apply the same tags to all jobs, use the regular expression ".".
   ci_tags:
       ".":
         - tag1
         - tag2
         - tag3
 
+# By default, Prometa will attempt to detect each project's license using the
+# spdx-matcher Python package. In some cases the detection fails (e.g. GPL v2
+# and GPL v2-only use the same license text). This option can be set to an SPDX
+# license identifier (https://spdx.org/licenses/) to force a particular license
+# when the detection fails. If null or an empty strign then it will be ignored.
+#
+# Note that it will not download a new license file or modify the existing
+# license file.
+license: null
+
 # The utility to use when merging changes. It must accept two file paths (the
 # modified file and the original) and return non-zero exit status to indicate an
 # error or abort.
 merger: vimdiff
 
+
+# The README interpolator can insert command output into the README. To prevent
+# arbitrary command execution, Prometa will prompt the user to confirm a command
+# before it is executed. This prompt can be surpressed for trusted READMEs by
+# setting the following to true.
+trust_commands: false
+
 ~~~
 
 [/insert: command_output:yaml prometa --gen-config -]: #
 
 ## README Content Insertion
 
 Content can be inserted into the README.md file using invisible comments of the format:
@@ -202,15 +211,16 @@
 
 # Usage
 
 [insert: command_output prometa -h]: #
 
 ~~~
 $ prometa -h
-usage: prometa [-h] [--config PATH [PATH ...]] [--gen-config PATH] [--trust]
+usage: prometa [-h] [--config PATH [PATH ...]] [--gen-config PATH]
+               [--list-config {all,existing}] [--no-xdg] [--trust]
                [path ...]
 
 Update project metadata.
 
 positional arguments:
   path                  Path to project directory.
 
@@ -226,14 +236,22 @@
                         take precedence over the detected configuration files.
                         If multiple configuration paths are given with this
                         command, their order determines their precedence.
   --gen-config PATH     Generate a configuration file template at the given
                         path. If the path is "-", the file will be printed to
                         STDOUT. Note that prometa will only look for files
                         named "prometa.yaml" or ".prometa.yaml".
+  --list-config {all,existing}
+                        List either all paths that will be scanned for
+                        configuration files for each given project, or only
+                        existing ones. The output is printed as a YAML file
+                        mapping project directory paths to lists of possible
+                        configuration files.
+  --no-xdg              Disable loading of configuration files in standard XDG
+                        locations.
   --trust               It is possible to insert arbitrary command output into
                         the README file. By default, prometa will prompt the
                         user for confirmation before running the command to
                         prevent arbitrary code execution in the context of a
                         collaborative environment. This option can be used to
                         disable the prompt if the user trusts all of the
                         commands in the README.
```

