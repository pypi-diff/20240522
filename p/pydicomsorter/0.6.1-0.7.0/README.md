# Comparing `tmp/pydicomsorter-0.6.1.tar.gz` & `tmp/pydicomsorter-0.7.0.tar.gz`

## Comparing `pydicomsorter-0.6.1.tar` & `pydicomsorter-0.7.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0   237084 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/pixi.lock
--rw-r--r--   0        0        0     9331 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/.github/workflows/main.yaml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/config/.pypackage-builder-answers.yml
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/config/coverage.toml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/config/hatch.toml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/config/mkdocs.yaml
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/config/releaserc.toml
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/config/ruff.toml
--rw-r--r--   0        0        0     5509 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/docs/about.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/docs/index.md
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/src/pydicomsorter/__init__.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/src/pydicomsorter/io.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/src/pydicomsorter/main.py
--rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/src/pydicomsorter/options.py
--rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/src/pydicomsorter/parser.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/src/pydicomsorter/tags4format.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/src/pydicomsorter/sandbox/__init__.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/src/pydicomsorter/sandbox/dicomsort.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/src/pydicomsorter/sandbox/diffwork.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/tests/test_parser.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/tests/test_say_hello.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/LICENSE
--rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/README.md
--rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 pydicomsorter-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0   237059 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/pixi.lock
+-rw-r--r--   0        0        0     9331 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/.github/workflows/main.yaml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/config/.pypackage-builder-answers.yml
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/config/coverage.toml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/config/hatch.toml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/config/mkdocs.yaml
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/config/releaserc.toml
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/config/ruff.toml
+-rw-r--r--   0        0        0     6144 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/docs/about.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/docs/index.md
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/src/pydicomsorter/__init__.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/src/pydicomsorter/io.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/src/pydicomsorter/main.py
+-rw-r--r--   0        0        0      890 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/src/pydicomsorter/options.py
+-rw-r--r--   0        0        0     2829 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/src/pydicomsorter/parser.py
+-rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/src/pydicomsorter/tags4format.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/src/pydicomsorter/sandbox/__init__.py
+-rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/src/pydicomsorter/sandbox/dicomsort 2.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/src/pydicomsorter/sandbox/dicomsort.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/src/pydicomsorter/sandbox/diffwork.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/tests/test_parser.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/tests/test_say_hello.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/README.md
+-rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 pydicomsorter-0.7.0/PKG-INFO
```

### Comparing `pydicomsorter-0.6.1/.pre-commit-config.yaml` & `pydicomsorter-0.7.0/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 repos:
   - repo: local
     hooks:
       - id: pixi-install
         name: Run pixi install
-        entry: bash -c 'pixi install && pixi install -e dev && pixi install -e publish'
+        entry: bash -c 'pixi install --all && git add pixi.lock'
         language: system
         files: ^src/.*\.py$|^pyproject\.toml$|^pixi\.lock$
       - id: pixi-run-tests
         name: Run pixi tests
         entry: bash -c 'pixi run test'
         language: system
         files: ^src/.*\.py$|^pyproject\.toml$
```

### Comparing `pydicomsorter-0.6.1/pixi.lock` & `pydicomsorter-0.7.0/pixi.lock`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0.1-py312h98912ed_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/pyzmq-26.0.3-py312h8fd38d8_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ruff-0.4.4-py312h5715c7c_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-70.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tornado-6.4-py312h98912ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
@@ -309,15 +309,15 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/pyyaml-6.0.1-py312h104f124_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/pyzmq-26.0.3-py312ha04878a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ruff-0.4.4-py312h675b354_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-70.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tornado-6.4-py312h41838bb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
@@ -409,15 +409,15 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pyyaml-6.0.1-py312h02f2b3b_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pyzmq-26.0.3-py312hfa13136_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ruff-0.4.4-py312h3402d49_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-70.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tornado-6.4-py312he37b823_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
@@ -503,15 +503,15 @@
       - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/pywin32-306-py312h53d5487_2.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/pyyaml-6.0.1-py312he70551f_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pyyaml-env-tag-0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/pyzmq-26.0.3-py312hd7027bb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ruff-0.4.4-py312h7a6832a_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/setuptools-70.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/tornado-6.4-py312he70551f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
@@ -616,15 +616,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-gitlab-4.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-semantic-release-9.7.3-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/requests-2.32.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/requests-2.32.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/secretstorage-3.3.3-py312h7900ff3_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/smmap-5.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
@@ -708,15 +708,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-gitlab-4.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-semantic-release-9.7.3-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/requests-2.32.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/requests-2.32.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/smmap-5.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
@@ -799,15 +799,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-gitlab-4.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-semantic-release-9.7.3-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/requests-2.32.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/requests-2.32.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/smmap-5.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
@@ -889,15 +889,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.3-h2628c8c_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-gitlab-4.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-semantic-release-9.7.3-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/pywin32-ctypes-0.2.2-py312h2e8e312_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/requests-2.32.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/requests-2.32.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/smmap-5.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
@@ -3974,40 +3974,40 @@
   purls:
   - pkg:pypi/pydantic?source=conda-forge-mapping
   size: 282275
   timestamp: 1713905769522
 - kind: pypi
   name: pydantic-core
   version: 2.18.2
-  url: https://files.pythonhosted.org/packages/e4/49/f29028068b5cb364ad066a58490dd26fd1d4ba2943d829eb0f85dbc8ab06/pydantic_core-2.18.2-cp312-none-win_amd64.whl
-  sha256: b1bd7e47b1558ea872bd16c8502c414f9e90dcf12f1395129d7bb42a09a95438
+  url: https://files.pythonhosted.org/packages/30/49/397da3f6910d62f092684a50bcaba2566825c6eee27a743846583a01fadf/pydantic_core-2.18.2-cp312-cp312-macosx_11_0_arm64.whl
+  sha256: 6132dd3bd52838acddca05a72aafb6eab6536aa145e923bb50f45e78b7251043
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.2
-  url: https://files.pythonhosted.org/packages/30/49/397da3f6910d62f092684a50bcaba2566825c6eee27a743846583a01fadf/pydantic_core-2.18.2-cp312-cp312-macosx_11_0_arm64.whl
-  sha256: 6132dd3bd52838acddca05a72aafb6eab6536aa145e923bb50f45e78b7251043
+  url: https://files.pythonhosted.org/packages/a1/c9/7d61469af6386e5846b5864bb93dc770979968c113863f923916c1a8bca2/pydantic_core-2.18.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: 7ca4ae5a27ad7a4ee5170aebce1574b375de390bc01284f87b18d43a3984df72
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.2
-  url: https://files.pythonhosted.org/packages/15/b1/e6edfe46402a5b415fc3de86aa64fb10009b323907f8d513175bfb839aa9/pydantic_core-2.18.2-cp312-cp312-macosx_10_12_x86_64.whl
-  sha256: fb2bd7be70c0fe4dfd32c951bc813d9fe6ebcbfdd15a07527796c8204bd36242
+  url: https://files.pythonhosted.org/packages/e4/49/f29028068b5cb364ad066a58490dd26fd1d4ba2943d829eb0f85dbc8ab06/pydantic_core-2.18.2-cp312-none-win_amd64.whl
+  sha256: b1bd7e47b1558ea872bd16c8502c414f9e90dcf12f1395129d7bb42a09a95438
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: pypi
   name: pydantic-core
   version: 2.18.2
-  url: https://files.pythonhosted.org/packages/a1/c9/7d61469af6386e5846b5864bb93dc770979968c113863f923916c1a8bca2/pydantic_core-2.18.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
-  sha256: 7ca4ae5a27ad7a4ee5170aebce1574b375de390bc01284f87b18d43a3984df72
+  url: https://files.pythonhosted.org/packages/15/b1/e6edfe46402a5b415fc3de86aa64fb10009b323907f8d513175bfb839aa9/pydantic_core-2.18.2-cp312-cp312-macosx_10_12_x86_64.whl
+  sha256: fb2bd7be70c0fe4dfd32c951bc813d9fe6ebcbfdd15a07527796c8204bd36242
   requires_dist:
   - typing-extensions>=4.6.0,!=4.7.0
   requires_python: '>=3.8'
 - kind: conda
   name: pydantic-core
   version: 2.18.2
   build: py312h2615798_0
@@ -4104,17 +4104,17 @@
   - sphinx-rtd-theme ; extra == 'docs'
   - sphinx-gallery ; extra == 'docs'
   - sphinxcontrib-napoleon ; extra == 'docs'
   - sphinx-copybutton ; extra == 'docs'
   requires_python: '>=3.7'
 - kind: pypi
   name: pydicomsorter
-  version: 0.6.1
+  version: 0.7.0
   path: .
-  sha256: c24df5e40b7201804870cc0343a4a76596da92c8532c671c68fa5c2eb867b703
+  sha256: 278573a875fae65ff58c04bf48067e51b64bc85484d47ff9ecf896b7e4289bd4
   requires_dist:
   - rich
   - rich-click
   - pydicom
   - pydantic
   requires_python: '>=3.12'
   editable: true
@@ -4750,35 +4750,34 @@
   - ncurses >=6.3,<7.0a0
   license: GPL-3.0-only
   license_family: GPL
   size: 255870
   timestamp: 1679532707590
 - kind: conda
   name: requests
-  version: 2.32.1
+  version: 2.32.2
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
-  url: https://conda.anaconda.org/conda-forge/noarch/requests-2.32.1-pyhd8ed1ab_0.conda
-  sha256: 6c64bb15baf632e99c39099cd7ba9201b258a6323b8b47c8a902d0932813ff65
-  md5: 20ce56db6c7aae9e6654b358ecbfc470
+  url: https://conda.anaconda.org/conda-forge/noarch/requests-2.32.2-pyhd8ed1ab_0.conda
+  sha256: 115b796fddc846bee6f47e3c57d04d12fa93a47a7a8ef639cefdc05203c1bf00
+  md5: e1643b34b19df8c028a4f00bf5df58a6
   depends:
   - certifi >=2017.4.17
   - charset-normalizer >=2,<4
   - idna >=2.5,<4
   - python >=3.7
   - urllib3 >=1.21.1,<3
   constrains:
   - chardet >=3.0.2,<6
   license: Apache-2.0
-  license_family: APACHE
   purls:
   - pkg:pypi/requests?source=conda-forge-mapping
-  size: 57720
-  timestamp: 1716263481344
+  size: 57885
+  timestamp: 1716354575895
 - kind: conda
   name: requests-toolbelt
   version: 1.0.0
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda
@@ -4952,29 +4951,29 @@
   license_family: BSD
   purls:
   - pkg:pypi/secretstorage?source=conda-forge-mapping
   size: 31766
   timestamp: 1695551875966
 - kind: conda
   name: setuptools
-  version: 69.5.1
+  version: 70.0.0
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
-  url: https://conda.anaconda.org/conda-forge/noarch/setuptools-69.5.1-pyhd8ed1ab_0.conda
-  sha256: 72d143408507043628b32bed089730b6d5f5445eccc44b59911ec9f262e365e7
-  md5: 7462280d81f639363e6e63c81276bd9e
+  url: https://conda.anaconda.org/conda-forge/noarch/setuptools-70.0.0-pyhd8ed1ab_0.conda
+  sha256: daa4638d288cfdf3b0ecea395d8efa25cafc4ebf4026464a36c797c84541d2be
+  md5: c8ddb4f34a208df4dd42509a0f6a1c89
   depends:
   - python >=3.8
   license: MIT
   license_family: MIT
   purls:
   - pkg:pypi/setuptools?source=conda-forge-mapping
-  size: 501790
-  timestamp: 1713094963112
+  size: 483015
+  timestamp: 1716368141661
 - kind: conda
   name: shellingham
   version: 1.5.4
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
```

### Comparing `pydicomsorter-0.6.1/.github/workflows/main.yaml` & `pydicomsorter-0.7.0/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.1/config/mkdocs.yaml` & `pydicomsorter-0.7.0/config/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.1/config/releaserc.toml` & `pydicomsorter-0.7.0/config/releaserc.toml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.1/config/ruff.toml` & `pydicomsorter-0.7.0/config/ruff.toml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.1/docs/CHANGELOG.md` & `pydicomsorter-0.7.0/docs/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,26 @@
 # CHANGELOG
 
 
 
+## v0.7.0 (2024-05-22)
+
+### Feature
+
+* feat: add pixi lock durin gpre-commit ([`a987074`](https://github.com/jjjermiah/PyDicomSorter/commit/a98707490ebd7d5beca515e0ddd8ec56cf223d13))
+
+### Fix
+
+* fix: update pre-commit with pixi lock ([`73fbad1`](https://github.com/jjjermiah/PyDicomSorter/commit/73fbad1a82fb98a27f34fe53a730bd7464435eaf))
+
+* fix: update pre-commit with pixi lock ([`1b0d911`](https://github.com/jjjermiah/PyDicomSorter/commit/1b0d9112d176342d055aea823e96e51af39492c8))
+
+* fix: update pre-commit with pixi lock ([`71c9aaa`](https://github.com/jjjermiah/PyDicomSorter/commit/71c9aaac7ea0e6c3cc6246a830d0088afa9fd482))
+
+
 ## v0.6.1 (2024-05-22)
 
 ### Fix
 
 * fix: lock ([`3bb9612`](https://github.com/jjjermiah/PyDicomSorter/commit/3bb96126c40d70b82bbffcbd5b3d1a9f12d0c533))
 
 * fix: lock ([`9603cac`](https://github.com/jjjermiah/PyDicomSorter/commit/9603cac4749df2bb5a6809961556adb879e8c3a7))
```

### Comparing `pydicomsorter-0.6.1/docs/about.md` & `pydicomsorter-0.7.0/docs/about.md`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.1/src/pydicomsorter/options.py` & `pydicomsorter-0.7.0/src/pydicomsorter/options.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.1/src/pydicomsorter/parser.py` & `pydicomsorter-0.7.0/src/pydicomsorter/parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.1/src/pydicomsorter/tags4format.py` & `pydicomsorter-0.7.0/src/pydicomsorter/tags4format.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.1/src/pydicomsorter/sandbox/dicomsort.py` & `pydicomsorter-0.7.0/src/pydicomsorter/sandbox/dicomsort.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.1/src/pydicomsorter/sandbox/diffwork.py` & `pydicomsorter-0.7.0/src/pydicomsorter/sandbox/diffwork.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.1/tests/test_parser.py` & `pydicomsorter-0.7.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.1/.gitignore` & `pydicomsorter-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.1/LICENSE` & `pydicomsorter-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.1/README.md` & `pydicomsorter-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.6.1/pyproject.toml` & `pydicomsorter-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #--------------------------------------------------------------------------------------------------#
 ######################################### Package Config ###########################################
 #__________________________________________________________________________________________________#
 [project]
 name = "pydicomsorter"
-version = "0.6.1"
+version = "0.7.0"
 description = "A Quick Tool For Sorting Dicom Files"
 license = "MIT"
 readme = "README.md"
 keywords = ["pydicomsorter", "pixi", "python", "package"]
 
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 maintainers = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
```

### Comparing `pydicomsorter-0.6.1/PKG-INFO` & `pydicomsorter-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pydicomsorter
-Version: 0.6.1
+Version: 0.7.0
 Summary: A Quick Tool For Sorting Dicom Files
 Project-URL: homepage, https://github.com/jjjermiah/pydicomsorter
 Project-URL: repository, https://github.com/jjjermiah/pydicomsorter
 Project-URL: documentation, https://jjjermiah.github.io/pydicomsorter/
 Project-URL: changelog, https://github.com/jjjermiah/pydicomsorter/blob/main/docs/CHANGELOG.md
 Project-URL: issues, https://github.com/jjjermiah/pydicomsorter/issues
 Author-email: Jermiah Joseph <jermiahjoseph98@gmail.com>
```

