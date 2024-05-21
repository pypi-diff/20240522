# Comparing `tmp/pydicomsorter-0.5.0.tar.gz` & `tmp/pydicomsorter-0.5.1.tar.gz`

## Comparing `pydicomsorter-0.5.0.tar` & `pydicomsorter-0.5.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0   231019 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/pixi.lock
--rw-r--r--   0        0        0     9497 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/.github/workflows/main.yaml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/config/.pypackage-builder-answers.yml
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/config/coverage.toml
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/config/hatch.toml
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/config/mkdocs.yaml
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/config/releaserc.toml
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/config/ruff.toml
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/docs/CHANGELOG.md
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/docs/about.md
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/docs/index.md
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/src/pydicomsorter/__init__.py
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/src/pydicomsorter/io.py
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/src/pydicomsorter/main.py
--rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/src/pydicomsorter/parser.py
--rw-r--r--   0        0        0     1837 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/src/pydicomsorter/tags4format.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/src/pydicomsorter/sandbox/__init__.py
--rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/src/pydicomsorter/sandbox/diffwork.py
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/tests/test_parser.py
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/tests/test_say_hello.py
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/.gitignore
--rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/LICENSE
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/README.md
--rw-r--r--   0        0        0     4828 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     1965 2020-02-02 00:00:00.000000 pydicomsorter-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0   237084 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/pixi.lock
+-rw-r--r--   0        0        0     9497 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/.github/workflows/main.yaml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/config/.pypackage-builder-answers.yml
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/config/coverage.toml
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/config/hatch.toml
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/config/mkdocs.yaml
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/config/releaserc.toml
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/config/ruff.toml
+-rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/docs/CHANGELOG.md
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/docs/about.md
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/docs/index.md
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/src/pydicomsorter/__init__.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/src/pydicomsorter/io.py
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/src/pydicomsorter/main.py
+-rw-r--r--   0        0        0     2830 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/src/pydicomsorter/parser.py
+-rw-r--r--   0        0        0     1881 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/src/pydicomsorter/tags4format.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/src/pydicomsorter/sandbox/__init__.py
+-rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/src/pydicomsorter/sandbox/dicomsort.py
+-rw-r--r--   0        0        0     2188 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/src/pydicomsorter/sandbox/diffwork.py
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/tests/test_parser.py
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/tests/test_say_hello.py
+-rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1057 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1744 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/README.md
+-rw-r--r--   0        0        0     4840 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2584 2020-02-02 00:00:00.000000 pydicomsorter-0.5.1/PKG-INFO
```

### Comparing `pydicomsorter-0.5.0/pixi.lock` & `pydicomsorter-0.5.1/pixi.lock`

 * *Files 4% similar despite different names*

```diff
@@ -18,95 +18,107 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.2.0-h77fa898_7.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.1-hd590300_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.45.3-h2797004_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.5-h59595ed_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.3.0-hd590300_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.3.0-h4ab18f5_2.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
+      - pypi: https://files.pythonhosted.org/packages/78/b6/6307fbef88d9b5ee7421e68d78a9f162e0da4900bc5f5793f6d3d0e34fb8/annotated_types-0.7.0-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/00/2e/d53fa4befbf2cfa713304affc7ca780ce4fc1fd8710527771b58311a3229/click-8.1.7-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/42/d7/1ec15b46af6af88f19b8e5ffea08fa375d433c998b8a7639e76935c14f1f/markdown_it_py-3.0.0-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/b3/38/89ba8ad64ae25be8de66a6d463314cf1eb366222074cfda9ee839c56a4b4/mdurl-0.1.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ed/76/9a17032880ed27f2dbd490c77a3431cbc80f47ba81534131de3c2846e736/pydantic-2.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/a1/c9/7d61469af6386e5846b5864bb93dc770979968c113863f923916c1a8bca2/pydantic_core-2.18.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
       - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/f7/3f/01c8b82017c199075f8f788d0d906b9ffbbc5a47dc9918a945e13d5a2bda/pygments-2.18.0-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/87/67/a37f6214d0e9fe57f6ae54b2956d550ca8365857f42a1ce0392bb21d9410/rich-13.7.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/01/f3/936e209267d6ef7510322191003885de524fc48d1b43269810cd589ceaf5/typing_extensions-4.11.0-py3-none-any.whl
       - pypi: .
       osx-64:
       - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libexpat-2.6.2-h73e2aa4_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libffi-3.4.2-h0d85af4_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.3-h92b6c6a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.5-h5846eda_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.3.0-hd75f5a5_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.3.0-h87427d6_2.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
+      - pypi: https://files.pythonhosted.org/packages/78/b6/6307fbef88d9b5ee7421e68d78a9f162e0da4900bc5f5793f6d3d0e34fb8/annotated_types-0.7.0-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/00/2e/d53fa4befbf2cfa713304affc7ca780ce4fc1fd8710527771b58311a3229/click-8.1.7-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/42/d7/1ec15b46af6af88f19b8e5ffea08fa375d433c998b8a7639e76935c14f1f/markdown_it_py-3.0.0-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/b3/38/89ba8ad64ae25be8de66a6d463314cf1eb366222074cfda9ee839c56a4b4/mdurl-0.1.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ed/76/9a17032880ed27f2dbd490c77a3431cbc80f47ba81534131de3c2846e736/pydantic-2.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/15/b1/e6edfe46402a5b415fc3de86aa64fb10009b323907f8d513175bfb839aa9/pydantic_core-2.18.2-cp312-cp312-macosx_10_12_x86_64.whl
       - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/f7/3f/01c8b82017c199075f8f788d0d906b9ffbbc5a47dc9918a945e13d5a2bda/pygments-2.18.0-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/87/67/a37f6214d0e9fe57f6ae54b2956d550ca8365857f42a1ce0392bb21d9410/rich-13.7.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/01/f3/936e209267d6ef7510322191003885de524fc48d1b43269810cd589ceaf5/typing_extensions-4.11.0-py3-none-any.whl
       - pypi: .
       osx-arm64:
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ca-certificates-2024.2.2-hf0a4a13_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libexpat-2.6.2-hebf3989_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libffi-3.4.2-h3422bc3_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsqlite-3.45.3-h091b4b1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h53f4e23_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.5-hb89a1cb_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.3.0-h0d3ecfb_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.3.0-hfb2fe0b_2.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
+      - pypi: https://files.pythonhosted.org/packages/78/b6/6307fbef88d9b5ee7421e68d78a9f162e0da4900bc5f5793f6d3d0e34fb8/annotated_types-0.7.0-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/00/2e/d53fa4befbf2cfa713304affc7ca780ce4fc1fd8710527771b58311a3229/click-8.1.7-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/42/d7/1ec15b46af6af88f19b8e5ffea08fa375d433c998b8a7639e76935c14f1f/markdown_it_py-3.0.0-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/b3/38/89ba8ad64ae25be8de66a6d463314cf1eb366222074cfda9ee839c56a4b4/mdurl-0.1.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ed/76/9a17032880ed27f2dbd490c77a3431cbc80f47ba81534131de3c2846e736/pydantic-2.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/30/49/397da3f6910d62f092684a50bcaba2566825c6eee27a743846583a01fadf/pydantic_core-2.18.2-cp312-cp312-macosx_11_0_arm64.whl
       - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/f7/3f/01c8b82017c199075f8f788d0d906b9ffbbc5a47dc9918a945e13d5a2bda/pygments-2.18.0-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/87/67/a37f6214d0e9fe57f6ae54b2956d550ca8365857f42a1ce0392bb21d9410/rich-13.7.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/01/f3/936e209267d6ef7510322191003885de524fc48d1b43269810cd589ceaf5/typing_extensions-4.11.0-py3-none-any.whl
       - pypi: .
       win-64:
       - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libexpat-2.6.2-h63175ca_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.3-hcfcfb64_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.3.0-hcfcfb64_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.3.0-h2466b09_2.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.3-h2628c8c_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-ha32ba9b_20.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33135-h835141b_20.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33135-h22015db_20.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
+      - pypi: https://files.pythonhosted.org/packages/78/b6/6307fbef88d9b5ee7421e68d78a9f162e0da4900bc5f5793f6d3d0e34fb8/annotated_types-0.7.0-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/00/2e/d53fa4befbf2cfa713304affc7ca780ce4fc1fd8710527771b58311a3229/click-8.1.7-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/d1/d6/3965ed04c63042e047cb6a3e6ed1a63a35087b6a609aa3a15ed8ac56c221/colorama-0.4.6-py2.py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/42/d7/1ec15b46af6af88f19b8e5ffea08fa375d433c998b8a7639e76935c14f1f/markdown_it_py-3.0.0-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/b3/38/89ba8ad64ae25be8de66a6d463314cf1eb366222074cfda9ee839c56a4b4/mdurl-0.1.2-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/ed/76/9a17032880ed27f2dbd490c77a3431cbc80f47ba81534131de3c2846e736/pydantic-2.7.1-py3-none-any.whl
+      - pypi: https://files.pythonhosted.org/packages/e4/49/f29028068b5cb364ad066a58490dd26fd1d4ba2943d829eb0f85dbc8ab06/pydantic_core-2.18.2-cp312-none-win_amd64.whl
       - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/f7/3f/01c8b82017c199075f8f788d0d906b9ffbbc5a47dc9918a945e13d5a2bda/pygments-2.18.0-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/87/67/a37f6214d0e9fe57f6ae54b2956d550ca8365857f42a1ce0392bb21d9410/rich-13.7.1-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/01/f3/936e209267d6ef7510322191003885de524fc48d1b43269810cd589ceaf5/typing_extensions-4.11.0-py3-none-any.whl
       - pypi: .
   dev:
@@ -114,14 +126,15 @@
     - url: https://conda.anaconda.org/conda-forge/
     indexes:
     - https://pypi.org/simple
     packages:
       linux-64:
       - conda: https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2
+      - conda: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.7.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/cffi-1.16.0-py312hf06ca03_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
@@ -167,28 +180,30 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mergedeep-1.3.4-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-get-deps-0.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.5-h59595ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.8.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.3.0-hd590300_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.3.0-h4ab18f5_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.7.1-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.8-py312h98912ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pydantic-2.7.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/pydantic-core-2.18.2-py312h4413252_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda
@@ -202,28 +217,30 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tornado-6.4-py312h98912ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ukkonen-1.0.1-py312h8572e83_4.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.26.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/watchdog-4.0.0-py312h7900ff3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.5-h75354e8_4.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
       - pypi: .
       osx-64:
+      - conda: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.7.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/cffi-1.16.0-py312h38bf5a0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda
@@ -263,28 +280,30 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mergedeep-1.3.4-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-get-deps-0.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.5-h5846eda_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.8.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.3.0-hd75f5a5_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.3.0-h87427d6_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.7.1-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/psutil-5.9.8-py312h41838bb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pydantic-2.7.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/pydantic-core-2.18.2-py312h5b0d100_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.12-4_cp312.conda
@@ -298,28 +317,30 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tornado-6.4-py312h41838bb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ukkonen-1.0.1-py312h49ebfd2_4.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.26.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/watchdog-4.0.0-py312hc2c2f20_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/yaml-0.2.5-h0d85af4_2.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zeromq-4.3.5-hde137ed_4.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
       - pypi: .
       osx-arm64:
+      - conda: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.7.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/appnope-0.1.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ca-certificates-2024.2.2-hf0a4a13_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/cffi-1.16.0-py312h8e38eb3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-unix_pyh707e725_0.conda
@@ -359,28 +380,30 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mergedeep-1.3.4-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-get-deps-0.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.5-hb89a1cb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.8.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.3.0-h0d3ecfb_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.3.0-hfb2fe0b_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.7.1-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/psutil-5.9.8-py312he37b823_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pydantic-2.7.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/pydantic-core-2.18.2-py312hbdaf6d9_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.12-4_cp312.conda
@@ -394,28 +417,30 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tornado-6.4-py312he37b823_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ukkonen-1.0.1-py312h389731b_4.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.26.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/watchdog-4.0.0-py312he37b823_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.13-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/yaml-0.2.5-h3422bc3_2.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zeromq-4.3.5-hcc0f68c_4.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
       - pypi: .
       win-64:
+      - conda: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.7.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/asttokens-2.4.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/cffi-1.16.0-py312he70551f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/cfgv-3.3.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/click-8.1.7-win_pyh7428d3b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/colorama-0.4.6-pyhd8ed1ab_0.tar.bz2
@@ -451,26 +476,28 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.7-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mergedeep-1.3.4-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mkdocs-get-deps-0.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.6.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/nodeenv-1.8.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.3.0-hcfcfb64_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.3.0-h2466b09_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/parso-0.8.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pre-commit-3.7.1-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.42-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/psutil-5.9.8-py312he70551f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/pydantic-2.7.1-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/pydantic-core-2.18.2-py312h2615798_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-8.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-cov-5.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pytest-xdist-3.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.3-h2628c8c_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.12-4_cp312.conda
@@ -484,14 +511,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/toml-0.10.2-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/tornado-6.4-py312he70551f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/traitlets-5.14.3-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/ukkonen-1.0.1-py312h0d7def4_4.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-ha32ba9b_20.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33135-h835141b_20.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.26.2-pyhd8ed1ab_0.conda
@@ -510,15 +538,15 @@
     - url: https://conda.anaconda.org/conda-forge/
     indexes:
     - https://pypi.org/simple
     packages:
       linux-64:
       - conda: https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.7.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/backports.tarfile-1.0.0-pyhd8ed1ab_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/brotli-python-1.1.0-py312h30efb56_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-hd590300_5.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2024.2.2-hbcca054_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda
@@ -570,15 +598,15 @@
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libxcrypt-4.4.36-hd590300_1.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-hd590300_5.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.5-py312h98912ed_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/more-itertools-10.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.5-h59595ed_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.3.0-hd590300_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.3.0-h4ab18f5_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/pcre2-10.43-hcad00b1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
@@ -588,15 +616,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python-3.12.3-hab00c5b_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-gitlab-4.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-semantic-release-9.7.3-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/requests-2.32.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/secretstorage-3.3.3-py312h7900ff3_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/smmap-5.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.13-noxft_h4845f30_101.conda
@@ -605,25 +633,25 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.5-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.5.17-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/linux-64/uv-0.1.44-h0ea3d13_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/linux-64/uv-0.1.45-h0ea3d13_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.26.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zstandard-0.22.0-py312hd58854c_0.conda
       - conda: https://conda.anaconda.org/conda-forge/linux-64/zstd-1.5.5-hfc55251_0.conda
       - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
       - pypi: .
       osx-64:
-      - conda: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.7.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/backports.tarfile-1.0.0-pyhd8ed1ab_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/brotli-python-1.1.0-py312heafc425_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/bzip2-1.0.8-h10d778d_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ca-certificates-2024.2.2-h8857fd0_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda
@@ -663,15 +691,15 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libsqlite-3.45.3-h92b6c6a_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/libzlib-1.2.13-h8a1eda9_5.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/markupsafe-2.1.5-py312h41838bb_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/more-itertools-10.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/ncurses-6.5-h5846eda_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.3.0-hd75f5a5_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.3.0-h87427d6_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
@@ -680,15 +708,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python-3.12.3-h1411813_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-gitlab-4.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-semantic-release-9.7.3-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/readline-8.2-h9e318b2_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/requests-2.32.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/smmap-5.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/tk-8.6.13-h1abcd95_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
@@ -696,25 +724,25 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.5-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.5.17-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/osx-64/uv-0.1.44-h0a647a2_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-64/uv-0.1.45-h4e38c46_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.26.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/xz-5.2.6-h775f41a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zstandard-0.22.0-py312h7a629f7_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-64/zstd-1.5.5-h829000d_0.conda
       - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
       - pypi: .
       osx-arm64:
-      - conda: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.7.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/backports.tarfile-1.0.0-pyhd8ed1ab_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/brotli-python-1.1.0-py312h9f69965_1.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/bzip2-1.0.8-h93a5062_5.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ca-certificates-2024.2.2-hf0a4a13_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda
@@ -754,15 +782,15 @@
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libsqlite-3.45.3-h091b4b1_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/libzlib-1.2.13-h53f4e23_5.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/markupsafe-2.1.5-py312he37b823_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/more-itertools-10.2.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/ncurses-6.5-hb89a1cb_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.3.0-h0d3ecfb_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.3.0-hfb2fe0b_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
@@ -771,15 +799,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python-3.12.3-h4a7b5fc_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-gitlab-4.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-semantic-release-9.7.3-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/readline-8.2-h92ec313_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/requests-2.32.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/smmap-5.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/tk-8.6.13-h5083fa2_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
@@ -787,25 +815,25 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomlkit-0.12.5-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.5.17-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/uv-0.1.44-hc069d6b_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/osx-arm64/uv-0.1.45-hc069d6b_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.26.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/xz-5.2.6-h57fd34a_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zstandard-0.22.0-py312h7975427_0.conda
       - conda: https://conda.anaconda.org/conda-forge/osx-arm64/zstd-1.5.5-h4f39d0f_0.conda
       - pypi: https://files.pythonhosted.org/packages/35/2a/8c0f6fe243e6b6793868c6834203a44cc8f3f25abad780e1c7b21e15594d/pydicom-2.4.4-py3-none-any.whl
       - pypi: https://files.pythonhosted.org/packages/2f/89/a1942f45644cf14e3f8ca64f4a3efe0afad50383caf60328cc51e92d4c88/rich_click-1.8.2-py3-none-any.whl
       - pypi: .
       win-64:
-      - conda: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.6.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.7.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/backports.tarfile-1.0.0-pyhd8ed1ab_1.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/brotli-python-1.1.0-py312h53d5487_1.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/bzip2-1.0.8-hcfcfb64_5.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ca-certificates-2024.2.2-h56e8100_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/certifi-2024.2.2-pyhd8ed1ab_0.conda
@@ -844,15 +872,15 @@
       - conda: https://conda.anaconda.org/conda-forge/win-64/libffi-3.4.2-h8ffe710_5.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/libsqlite-3.45.3-hcfcfb64_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/libzlib-1.2.13-hcfcfb64_5.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/markdown-it-py-3.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/markupsafe-2.1.5-py312he70551f_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/mdurl-0.1.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/more-itertools-10.2.0-pyhd8ed1ab_0.conda
-      - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.3.0-hcfcfb64_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/openssl-3.3.0-h2466b09_2.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pathspec-0.12.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pexpect-4.9.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/platformdirs-4.2.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pluggy-1.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/pycparser-2.22-pyhd8ed1ab_0.conda
@@ -861,15 +889,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/pygments-2.18.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyh0701188_6.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/python-3.12.3-h2628c8c_0_cpython.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-gitlab-4.5.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/python-semantic-release-9.7.3-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/python_abi-3.12-4_cp312.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/pywin32-ctypes-0.2.2-py312h2e8e312_1.conda
-      - conda: https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/noarch/requests-2.32.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/rich-13.7.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/shellingham-1.5.4-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/smmap-5.0.0-pyhd8ed1ab_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/tk-8.6.13-h5226925_1.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2
@@ -878,15 +906,15 @@
       - conda: https://conda.anaconda.org/conda-forge/noarch/trove-classifiers-2024.5.17-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.11.0-hd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.11.0-pyha770c72_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/tzdata-2024a-h0c530f3_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/ucrt-10.0.22621.0-h57928b3_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/urllib3-2.2.1-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/userpath-1.7.0-pyhd8ed1ab_0.tar.bz2
-      - conda: https://conda.anaconda.org/conda-forge/win-64/uv-0.1.44-ha08ef0e_0.conda
+      - conda: https://conda.anaconda.org/conda-forge/win-64/uv-0.1.45-ha08ef0e_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-ha32ba9b_20.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vc14_runtime-14.38.33135-h835141b_20.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/virtualenv-20.26.2-pyhd8ed1ab_0.conda
       - conda: https://conda.anaconda.org/conda-forge/win-64/vs2015_runtime-14.38.33135-h22015db_20.conda
       - conda: https://conda.anaconda.org/conda-forge/noarch/win_inet_pton-1.1.0-pyhd8ed1ab_6.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/win-64/xz-5.2.6-h8d14728_0.tar.bz2
       - conda: https://conda.anaconda.org/conda-forge/noarch/zipp-3.17.0-pyhd8ed1ab_0.conda
@@ -921,32 +949,40 @@
   - libgomp >=7.5.0
   constrains:
   - openmp_impl 9999
   license: BSD-3-Clause
   license_family: BSD
   size: 23621
   timestamp: 1650670423406
+- kind: pypi
+  name: annotated-types
+  version: 0.7.0
+  url: https://files.pythonhosted.org/packages/78/b6/6307fbef88d9b5ee7421e68d78a9f162e0da4900bc5f5793f6d3d0e34fb8/annotated_types-0.7.0-py3-none-any.whl
+  sha256: 1f02e8b43a8fbbc3f3e0d4f0f4bfc8131bcb4eebe8849b8e5c773f3a1c582a53
+  requires_dist:
+  - typing-extensions>=4.0.0 ; python_version < '3.9'
+  requires_python: '>=3.8'
 - kind: conda
   name: annotated-types
-  version: 0.6.0
+  version: 0.7.0
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
-  url: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.6.0-pyhd8ed1ab_0.conda
-  sha256: 3a2c98154d95cfd54daba6b7d507d31f5ba07ac2ad955c44eb041b66563193cd
-  md5: 997c29372bdbe2afee073dff71f35923
+  url: https://conda.anaconda.org/conda-forge/noarch/annotated-types-0.7.0-pyhd8ed1ab_0.conda
+  sha256: 668f0825b6c18e4012ca24a0070562b6ec801ebc7008228a428eb52b4038873f
+  md5: 7e9f4612544c8edbfd6afad17f1bd045
   depends:
   - python >=3.7
   - typing-extensions >=4.0.0
   license: MIT
   license_family: MIT
   purls:
   - pkg:pypi/annotated-types?source=conda-forge-mapping
-  size: 17026
-  timestamp: 1696634393637
+  size: 18235
+  timestamp: 1716290348421
 - kind: conda
   name: anyio
   version: 4.3.0
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/anyio-4.3.0-pyhd8ed1ab_0.conda
@@ -3532,79 +3568,85 @@
   purls:
   - pkg:pypi/nodeenv?source=conda-forge-mapping
   size: 34358
   timestamp: 1683893151613
 - kind: conda
   name: openssl
   version: 3.3.0
-  build: h0d3ecfb_0
-  subdir: osx-arm64
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.3.0-h0d3ecfb_0.conda
-  sha256: 51f9be8fe929c2bb3243cd0707b6dfcec27541f8284b4bd9b063c288fc46f482
-  md5: 25b0e522c3131886a637e347b2ca0c0f
+  build: h2466b09_2
+  build_number: 2
+  subdir: win-64
+  url: https://conda.anaconda.org/conda-forge/win-64/openssl-3.3.0-h2466b09_2.conda
+  sha256: 0f9fc8244ee65b0b78b637f4a51cc47800ac364f31b6e7de91db0f49cd3bb204
+  md5: 67d5f8749ee4ae3c4060d7a13fc8872f
   depends:
   - ca-certificates
+  - ucrt >=10.0.20348.0
+  - vc >=14.2,<15
+  - vc14_runtime >=14.29.30139
   constrains:
   - pyopenssl >=22.1
   license: Apache-2.0
   license_family: Apache
-  size: 2888226
-  timestamp: 1714466346030
+  size: 8330419
+  timestamp: 1716288210872
 - kind: conda
   name: openssl
   version: 3.3.0
-  build: hcfcfb64_0
-  subdir: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/openssl-3.3.0-hcfcfb64_0.conda
-  sha256: ca7573b7503711b53b2464fa35e4efa6f89dcd3d436fb5f128722b853e356dfd
-  md5: a6c544c9f060740c625dbf6d92cf3495
+  build: h4ab18f5_2
+  build_number: 2
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.3.0-h4ab18f5_2.conda
+  sha256: e56d9121f553f16ef21d2664c569cd50336291fa1458be5e5c654553a43737e7
+  md5: b8934d399b56d73e323403e183d009c5
   depends:
   - ca-certificates
-  - ucrt >=10.0.20348.0
-  - vc >=14.2,<15
-  - vc14_runtime >=14.29.30139
+  - libgcc-ng >=12
   constrains:
   - pyopenssl >=22.1
   license: Apache-2.0
   license_family: Apache
-  size: 8358240
-  timestamp: 1714468180752
+  size: 2894882
+  timestamp: 1716285197781
 - kind: conda
   name: openssl
   version: 3.3.0
-  build: hd590300_0
-  subdir: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/openssl-3.3.0-hd590300_0.conda
-  sha256: fdbf05e4db88c592366c90bb82e446edbe33c6e49e5130d51c580b2629c0b5d5
-  md5: c0f3abb4a16477208bbd43a39bd56f18
+  build: h87427d6_2
+  build_number: 2
+  subdir: osx-64
+  url: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.3.0-h87427d6_2.conda
+  sha256: 8a690c05bf3e1016a7dfc44d9b508e9883bbc7bcf5569e9e808c1e028ebb72ab
+  md5: fa4859f58b1810d77089b0482c886da0
   depends:
+  - __osx >=10.13
   - ca-certificates
-  - libgcc-ng >=12
   constrains:
   - pyopenssl >=22.1
   license: Apache-2.0
   license_family: Apache
-  size: 2895187
-  timestamp: 1714466138265
+  size: 2543706
+  timestamp: 1716285526027
 - kind: conda
   name: openssl
   version: 3.3.0
-  build: hd75f5a5_0
-  subdir: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/openssl-3.3.0-hd75f5a5_0.conda
-  sha256: d3889b0c89c2742e92e20f01e8f298b64c221df5d577c639b823a0bfe314e2e3
-  md5: eb8c33aa7929a7714eab8b90c1d88afe
+  build: hfb2fe0b_2
+  build_number: 2
+  subdir: osx-arm64
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/openssl-3.3.0-hfb2fe0b_2.conda
+  sha256: 503b34722d53224c5ebbabd0ffba2681287a810f9b129adb717dc6f6eb193752
+  md5: c9602073e34599f40b8c4ce9e19cabf6
   depends:
+  - __osx >=11.0
   - ca-certificates
   constrains:
   - pyopenssl >=22.1
   license: Apache-2.0
   license_family: Apache
-  size: 2541802
-  timestamp: 1714467068742
+  size: 2892345
+  timestamp: 1716285397137
 - kind: conda
   name: packaging
   version: '24.0'
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/packaging-24.0-pyhd8ed1ab_0.conda
@@ -3898,14 +3940,25 @@
   - python >=3.8
   license: BSD-3-Clause
   license_family: BSD
   purls:
   - pkg:pypi/pycparser?source=conda-forge-mapping
   size: 105098
   timestamp: 1711811634025
+- kind: pypi
+  name: pydantic
+  version: 2.7.1
+  url: https://files.pythonhosted.org/packages/ed/76/9a17032880ed27f2dbd490c77a3431cbc80f47ba81534131de3c2846e736/pydantic-2.7.1-py3-none-any.whl
+  sha256: e029badca45266732a9a79898a15ae2e8b14840b1eabbb25844be28f0b33f3d5
+  requires_dist:
+  - annotated-types>=0.4.0
+  - pydantic-core==2.18.2
+  - typing-extensions>=4.6.1
+  - email-validator>=2.0.0 ; extra == 'email'
+  requires_python: '>=3.8'
 - kind: conda
   name: pydantic
   version: 2.7.1
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/pydantic-2.7.1-pyhd8ed1ab_0.conda
@@ -3918,14 +3971,46 @@
   - typing-extensions >=4.6.1
   license: MIT
   license_family: MIT
   purls:
   - pkg:pypi/pydantic?source=conda-forge-mapping
   size: 282275
   timestamp: 1713905769522
+- kind: pypi
+  name: pydantic-core
+  version: 2.18.2
+  url: https://files.pythonhosted.org/packages/a1/c9/7d61469af6386e5846b5864bb93dc770979968c113863f923916c1a8bca2/pydantic_core-2.18.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl
+  sha256: 7ca4ae5a27ad7a4ee5170aebce1574b375de390bc01284f87b18d43a3984df72
+  requires_dist:
+  - typing-extensions>=4.6.0,!=4.7.0
+  requires_python: '>=3.8'
+- kind: pypi
+  name: pydantic-core
+  version: 2.18.2
+  url: https://files.pythonhosted.org/packages/30/49/397da3f6910d62f092684a50bcaba2566825c6eee27a743846583a01fadf/pydantic_core-2.18.2-cp312-cp312-macosx_11_0_arm64.whl
+  sha256: 6132dd3bd52838acddca05a72aafb6eab6536aa145e923bb50f45e78b7251043
+  requires_dist:
+  - typing-extensions>=4.6.0,!=4.7.0
+  requires_python: '>=3.8'
+- kind: pypi
+  name: pydantic-core
+  version: 2.18.2
+  url: https://files.pythonhosted.org/packages/e4/49/f29028068b5cb364ad066a58490dd26fd1d4ba2943d829eb0f85dbc8ab06/pydantic_core-2.18.2-cp312-none-win_amd64.whl
+  sha256: b1bd7e47b1558ea872bd16c8502c414f9e90dcf12f1395129d7bb42a09a95438
+  requires_dist:
+  - typing-extensions>=4.6.0,!=4.7.0
+  requires_python: '>=3.8'
+- kind: pypi
+  name: pydantic-core
+  version: 2.18.2
+  url: https://files.pythonhosted.org/packages/15/b1/e6edfe46402a5b415fc3de86aa64fb10009b323907f8d513175bfb839aa9/pydantic_core-2.18.2-cp312-cp312-macosx_10_12_x86_64.whl
+  sha256: fb2bd7be70c0fe4dfd32c951bc813d9fe6ebcbfdd15a07527796c8204bd36242
+  requires_dist:
+  - typing-extensions>=4.6.0,!=4.7.0
+  requires_python: '>=3.8'
 - kind: conda
   name: pydantic-core
   version: 2.18.2
   build: py312h2615798_0
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/pydantic-core-2.18.2-py312h2615798_0.conda
   sha256: 82de91ebd3938dfc8b18f10dbfbe3342580a3051877ffc901023820f821bf4a2
@@ -4019,21 +4104,22 @@
   - sphinx-rtd-theme ; extra == 'docs'
   - sphinx-gallery ; extra == 'docs'
   - sphinxcontrib-napoleon ; extra == 'docs'
   - sphinx-copybutton ; extra == 'docs'
   requires_python: '>=3.7'
 - kind: pypi
   name: pydicomsorter
-  version: 0.5.0
+  version: 0.5.1
   path: .
-  sha256: f2203ddb1c827d562e9173a6986da4fdfcd84fe2b6860dd9621e1f6e26a23322
+  sha256: 0c0adf531580037c43b03bb82b4f051852893b937dd0927fa0eea7d020b32b33
   requires_dist:
   - rich
   - rich-click
   - pydicom
+  - pydantic
   requires_python: '>=3.12'
   editable: true
 - kind: pypi
   name: pygments
   version: 2.18.0
   url: https://files.pythonhosted.org/packages/f7/3f/01c8b82017c199075f8f788d0d906b9ffbbc5a47dc9918a945e13d5a2bda/pygments-2.18.0-py3-none-any.whl
   sha256: b8e6aca0523f3ab76fee51799c488e38782ac06eafcf95e7ba832985c8e7b13a
@@ -4664,35 +4750,35 @@
   - ncurses >=6.3,<7.0a0
   license: GPL-3.0-only
   license_family: GPL
   size: 255870
   timestamp: 1679532707590
 - kind: conda
   name: requests
-  version: 2.31.0
+  version: 2.32.1
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
-  url: https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda
-  sha256: 9f629d6fd3c8ac5f2a198639fe7af87c4db2ac9235279164bfe0fcb49d8c4bad
-  md5: a30144e4156cdbb236f99ebb49828f8b
+  url: https://conda.anaconda.org/conda-forge/noarch/requests-2.32.1-pyhd8ed1ab_0.conda
+  sha256: 6c64bb15baf632e99c39099cd7ba9201b258a6323b8b47c8a902d0932813ff65
+  md5: 20ce56db6c7aae9e6654b358ecbfc470
   depends:
   - certifi >=2017.4.17
   - charset-normalizer >=2,<4
   - idna >=2.5,<4
   - python >=3.7
   - urllib3 >=1.21.1,<3
   constrains:
   - chardet >=3.0.2,<6
   license: Apache-2.0
   license_family: APACHE
   purls:
   - pkg:pypi/requests?source=conda-forge-mapping
-  size: 56690
-  timestamp: 1684774408600
+  size: 57720
+  timestamp: 1716263481344
 - kind: conda
   name: requests-toolbelt
   version: 1.0.0
   build: pyhd8ed1ab_0
   subdir: noarch
   noarch: python
   url: https://conda.anaconda.org/conda-forge/noarch/requests-toolbelt-1.0.0-pyhd8ed1ab_0.conda
@@ -5394,73 +5480,73 @@
   license_family: MIT
   purls:
   - pkg:pypi/userpath?source=conda-forge-mapping
   size: 17423
   timestamp: 1632758637093
 - kind: conda
   name: uv
-  version: 0.1.44
-  build: h0a647a2_0
+  version: 0.1.45
+  build: h0ea3d13_0
+  subdir: linux-64
+  url: https://conda.anaconda.org/conda-forge/linux-64/uv-0.1.45-h0ea3d13_0.conda
+  sha256: 2fdfcd0ef1d0790dc737d97a34c7025ac24cd2439255330b65f1e2cfb25a751d
+  md5: bc8413b4df51004db881047acf34eced
+  depends:
+  - libgcc-ng >=12
+  - libstdcxx-ng >=12
+  license: Apache-2.0 OR MIT
+  size: 12371123
+  timestamp: 1716265064010
+- kind: conda
+  name: uv
+  version: 0.1.45
+  build: h4e38c46_0
   subdir: osx-64
-  url: https://conda.anaconda.org/conda-forge/osx-64/uv-0.1.44-h0a647a2_0.conda
-  sha256: 26ff47ea2c7885f59bf96b0c4454bb7561749264a8d17d765479cfa0a9b2b593
-  md5: 6e46f8afee2fd39a38a09d3a45473d2e
+  url: https://conda.anaconda.org/conda-forge/osx-64/uv-0.1.45-h4e38c46_0.conda
+  sha256: 8c11774ca1940dcd90187ce240afea26b76e2942f9b18d65f6d4b483534193fd
+  md5: 754ce8a22c94a30c7bbd42274c7fae31
   depends:
   - __osx >=10.13
   - libcxx >=16
   constrains:
   - __osx >=10.12
   license: Apache-2.0 OR MIT
-  size: 8883416
-  timestamp: 1715727900529
-- kind: conda
-  name: uv
-  version: 0.1.44
-  build: h0ea3d13_0
-  subdir: linux-64
-  url: https://conda.anaconda.org/conda-forge/linux-64/uv-0.1.44-h0ea3d13_0.conda
-  sha256: d13c088e0c9cc8046b8ac93ac8534b5f1621480df7f07ff7e40cfffb34d2ef8a
-  md5: 211687f8af1e40c9802920b64d927135
-  depends:
-  - libgcc-ng >=12
-  - libstdcxx-ng >=12
-  license: Apache-2.0 OR MIT
-  size: 12280622
-  timestamp: 1715727676955
+  size: 8937335
+  timestamp: 1716265195083
 - kind: conda
   name: uv
-  version: 0.1.44
+  version: 0.1.45
   build: ha08ef0e_0
   subdir: win-64
-  url: https://conda.anaconda.org/conda-forge/win-64/uv-0.1.44-ha08ef0e_0.conda
-  sha256: 5151a6f3e0ef8b2a67c51a407fc4520b3d950ad3d1d80d6aa0e98f10d15732cd
-  md5: 8457ca587914aa187d6e3482cc61f28a
+  url: https://conda.anaconda.org/conda-forge/win-64/uv-0.1.45-ha08ef0e_0.conda
+  sha256: 6410e55c5c07006ab831594a4b3d4d13f6788d83946f84500142625882545fdb
+  md5: eb33a574fcd15e42928a98387343b6a0
   depends:
   - ucrt >=10.0.20348.0
   - vc >=14.2,<15
   - vc14_runtime >=14.29.30139
   license: Apache-2.0 OR MIT
-  size: 7556166
-  timestamp: 1715728623661
+  size: 7597264
+  timestamp: 1716266180906
 - kind: conda
   name: uv
-  version: 0.1.44
+  version: 0.1.45
   build: hc069d6b_0
   subdir: osx-arm64
-  url: https://conda.anaconda.org/conda-forge/osx-arm64/uv-0.1.44-hc069d6b_0.conda
-  sha256: 050a905e12fa53fd8b3cc03371562a1bebd08098a830f3d010b361dfef9ff9d5
-  md5: 0d2ed6566cd4dc8746d1f4d9b9d39b7c
+  url: https://conda.anaconda.org/conda-forge/osx-arm64/uv-0.1.45-hc069d6b_0.conda
+  sha256: 80dfc19f2ef473e86e718361847d1d598e95ffd0c0f5de7d07cda35d25f6aef5
+  md5: 9192238a60bc6da9c41092990c31eb41
   depends:
   - __osx >=11.0
   - libcxx >=16
   constrains:
   - __osx >=11.0
   license: Apache-2.0 OR MIT
-  size: 9181988
-  timestamp: 1715727491691
+  size: 9231858
+  timestamp: 1716265232676
 - kind: conda
   name: vc
   version: '14.3'
   build: ha32ba9b_20
   build_number: 20
   subdir: win-64
   url: https://conda.anaconda.org/conda-forge/win-64/vc-14.3-ha32ba9b_20.conda
```

### Comparing `pydicomsorter-0.5.0/.github/workflows/main.yaml` & `pydicomsorter-0.5.1/.github/workflows/main.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.0/config/mkdocs.yaml` & `pydicomsorter-0.5.1/config/mkdocs.yaml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.0/config/releaserc.toml` & `pydicomsorter-0.5.1/config/releaserc.toml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.0/config/ruff.toml` & `pydicomsorter-0.5.1/config/ruff.toml`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.0/docs/CHANGELOG.md` & `pydicomsorter-0.5.1/docs/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,30 @@
 # CHANGELOG
 
 
 
+## v0.5.1 (2024-05-21)
+
+### Chore
+
+* chore: Update pre-commit configuration to include src/.*\.py$ files ([`74082dc`](https://github.com/jjjermiah/PyDicomSorter/commit/74082dc9bcdbed0813da6f14f056a29dbbd0421b))
+
+* chore: Update dependencies and add DICOMSorter class ([`640f409`](https://github.com/jjjermiah/PyDicomSorter/commit/640f409859c60bc3bd5294b09a660a8057360198))
+
+### Fix
+
+* fix: imports ([`ecb459e`](https://github.com/jjjermiah/PyDicomSorter/commit/ecb459e0a6963c5d591f160a3d06303ccc043282))
+
+### Unknown
+
+* update precommit ([`16b1844`](https://github.com/jjjermiah/PyDicomSorter/commit/16b18443cf13eced2c639734cd013bba1bf71d1a))
+
+* update precommit ([`879f5c5`](https://github.com/jjjermiah/PyDicomSorter/commit/879f5c5c6e62cc35c612147012321dead42b8aa7))
+
+
 ## v0.5.0 (2024-05-21)
 
 ### Chore
 
 * chore: update pre-commit dependency version to &gt;=3.7.1,&lt;3.8 ([`446a5cc`](https://github.com/jjjermiah/PyDicomSorter/commit/446a5ccfc32a34705f0aa234113db32c6296de13))
 
 * chore: remove unused .pypackage-builder-answers.yml file and update README badges ([`bcd0a59`](https://github.com/jjjermiah/PyDicomSorter/commit/bcd0a599bceeaa38fdd29a241992237077aae7f1))
```

### Comparing `pydicomsorter-0.5.0/docs/about.md` & `pydicomsorter-0.5.1/docs/about.md`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.0/src/pydicomsorter/parser.py` & `pydicomsorter-0.5.1/src/pydicomsorter/parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.0/src/pydicomsorter/tags4format.py` & `pydicomsorter-0.5.1/src/pydicomsorter/tags4format.py`

 * *Files 10% similar despite different names*

```diff
@@ -30,33 +30,37 @@
 
 
 all_dicom_tags: list[str] = [
     item for key, value in DicomDictionary.items() for item in (value[2], value[4])
 ]
 
 
-def build_tree(tree: ttk.Treeview, ds: pydicom.Dataset, parent: str | None = None) -> None:
+def build_tree(
+    tree: ttk.Treeview, ds: pydicom.Dataset, parent: str | None = None
+) -> None:
     """Build out the tree.
 
     Parameters
     ----------
     tree : ttk.Treeview
         The treeview object.
     ds : pydicom.dataset.Dataset
         The dataset object to add to the `tree`.
     parent : str | None
         The item ID of the parent item in the tree (if any), default ``None``.
     """
     # For each DataElement in the current Dataset
     for idx, elem in enumerate(ds):
-        tree_item = tree.insert('', tk.END, text=str(elem))
+        tree_item = tree.insert("", tk.END, text=str(elem))
         if parent:
             tree.move(tree_item, parent, idx)
 
-        if elem.VR == 'SQ':
+        if elem.VR == "SQ":
             # DataElement is a sequence, containing 0 or more Datasets
             for seq_idx, seq_item in enumerate(elem.value):
-                tree_seq_item = tree.insert('', tk.END, text=f'{elem.name} Item {seq_idx + 1}')
+                tree_seq_item = tree.insert(
+                    "", tk.END, text=f"{elem.name} Item {seq_idx + 1}"
+                )
                 tree.move(tree_seq_item, tree_item, seq_idx)
 
                 # Recurse into the sequence item(s)
                 build_tree(tree, seq_item, tree_seq_item)
```

### Comparing `pydicomsorter-0.5.0/src/pydicomsorter/sandbox/diffwork.py` & `pydicomsorter-0.5.1/src/pydicomsorter/sandbox/diffwork.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.0/tests/test_parser.py` & `pydicomsorter-0.5.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.0/.gitignore` & `pydicomsorter-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.0/LICENSE` & `pydicomsorter-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydicomsorter-0.5.0/README.md` & `pydicomsorter-0.5.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -9,7 +9,29 @@
 [![Built with Material for MkDocs](https://img.shields.io/badge/mkdocs--material-gray?logo=materialformkdocs)](https://github.com/squidfunk/mkdocs-material)
 
 [![PyPI - Version](https://img.shields.io/pypi/v/PyDicomSorter)](https://pypi.org/project/pydicomsorter/)
 [![PyPI - Format](https://img.shields.io/pypi/format/PyDicomSorter)](https://pypi.org/project/pydicomsorter/)
 [![pixi-badge](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/prefix-dev/pixi/main/assets/badge/v0.json&style=flat-square)](https://github.com/prefix-dev/pixi)
 
 Testing the pydicom library to sort dicom files by patient name and study date.
+
+Designing:
+
+``` bash
+
+dicomsort [options] sourceDir destinationDir/<TARGET_PATTERN>
+
+options:
+
+- [-d, --deleteSource] 
+- [-k, --keepGoing]
+- [-s, --symlink]
+- [-n, --dryRun]
+- [-v, --verbose]
+
+```
+
+<!-- [![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra)](https://github.com/anuraghazra/github-readme-stats)
+
+[![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=jjjermiah)](https://github.com/jjjermiah/github-readme-stats) -->
+
+[![GitHub Trends SVG](https://api.githubtrends.io/user/svg/jjjermiah/langs)](https://githubtrends.io)
```

### Comparing `pydicomsorter-0.5.0/pyproject.toml` & `pydicomsorter-0.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #--------------------------------------------------------------------------------------------------#
 ######################################### Package Config ###########################################
 #__________________________________________________________________________________________________#
 [project]
 name = "pydicomsorter"
-version = "0.5.0"
+version = "0.5.1"
 description = "A Quick Tool For Sorting Dicom Files"
 license = "MIT"
 readme = "README.md"
 keywords = ["pydicomsorter", "pixi", "python", "package"]
 
 authors = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 maintainers = [{ name = "Jermiah Joseph", email = "jermiahjoseph98@gmail.com" }]
 
 requires-python = ">= 3.12"
-dependencies = ["rich", "rich-click", "pydicom"]
+dependencies = ["rich", "rich-click", "pydicom", "pydantic"]
 
 [project.urls]
 homepage = "https://github.com/jjjermiah/pydicomsorter"
 repository = "https://github.com/jjjermiah/pydicomsorter"
 documentation = "https://jjjermiah.github.io/pydicomsorter/"
 changelog = "https://github.com/jjjermiah/pydicomsorter/blob/main/docs/CHANGELOG.md"
 issues = "https://github.com/jjjermiah/pydicomsorter/issues"
```

### Comparing `pydicomsorter-0.5.0/PKG-INFO` & `pydicomsorter-0.5.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.3
 Name: pydicomsorter
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Quick Tool For Sorting Dicom Files
 Project-URL: homepage, https://github.com/jjjermiah/pydicomsorter
 Project-URL: repository, https://github.com/jjjermiah/pydicomsorter
 Project-URL: documentation, https://jjjermiah.github.io/pydicomsorter/
 Project-URL: changelog, https://github.com/jjjermiah/pydicomsorter/blob/main/docs/CHANGELOG.md
 Project-URL: issues, https://github.com/jjjermiah/pydicomsorter/issues
 Author-email: Jermiah Joseph <jermiahjoseph98@gmail.com>
 Maintainer-email: Jermiah Joseph <jermiahjoseph98@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: package,pixi,pydicomsorter,python
 Requires-Python: >=3.12
+Requires-Dist: pydantic
 Requires-Dist: pydicom
 Requires-Dist: rich
 Requires-Dist: rich-click
 Description-Content-Type: text/markdown
 
 # pydicomsorter
 
@@ -29,7 +30,29 @@
 [![Built with Material for MkDocs](https://img.shields.io/badge/mkdocs--material-gray?logo=materialformkdocs)](https://github.com/squidfunk/mkdocs-material)
 
 [![PyPI - Version](https://img.shields.io/pypi/v/PyDicomSorter)](https://pypi.org/project/pydicomsorter/)
 [![PyPI - Format](https://img.shields.io/pypi/format/PyDicomSorter)](https://pypi.org/project/pydicomsorter/)
 [![pixi-badge](https://img.shields.io/endpoint?url=https://raw.githubusercontent.com/prefix-dev/pixi/main/assets/badge/v0.json&style=flat-square)](https://github.com/prefix-dev/pixi)
 
 Testing the pydicom library to sort dicom files by patient name and study date.
+
+Designing:
+
+``` bash
+
+dicomsort [options] sourceDir destinationDir/<TARGET_PATTERN>
+
+options:
+
+- [-d, --deleteSource] 
+- [-k, --keepGoing]
+- [-s, --symlink]
+- [-n, --dryRun]
+- [-v, --verbose]
+
+```
+
+<!-- [![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=anuraghazra)](https://github.com/anuraghazra/github-readme-stats)
+
+[![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=jjjermiah)](https://github.com/jjjermiah/github-readme-stats) -->
+
+[![GitHub Trends SVG](https://api.githubtrends.io/user/svg/jjjermiah/langs)](https://githubtrends.io)
```

