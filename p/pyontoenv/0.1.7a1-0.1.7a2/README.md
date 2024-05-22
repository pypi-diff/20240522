# Comparing `tmp/pyontoenv-0.1.7a1.tar.gz` & `tmp/pyontoenv-0.1.7a2.tar.gz`

## Comparing `pyontoenv-0.1.7a1.tar` & `pyontoenv-0.1.7a2.tar`

### file list

```diff
@@ -1,60 +1,60 @@
--rw-r--r--   0     1001      127      776 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/Cargo.toml
--rw-r--r--   0     1001      127     5324 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/src/config.rs
--rw-r--r--   0     1001      127     2180 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/src/consts.rs
--rw-r--r--   0     1001      127     3267 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/src/doctor.rs
--rw-r--r--   0     1001      127      350 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/src/errors.rs
--rw-r--r--   0     1001      127    38662 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/src/lib.rs
--rw-r--r--   0     1001      127    13633 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/src/ontology.rs
--rw-r--r--   0     1001      127     3521 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/src/policy.rs
--rw-r--r--   0     1001      127     4646 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/src/transform.rs
--rw-r--r--   0     1001      127     6428 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/src/util.rs
--rw-r--r--   0     1001      127  1689944 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/Brick-1.3.ttl
--rw-r--r--   0     1001      127     1248 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/model
--rw-r--r--   0     1001      127      321 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/model.n3
--rw-r--r--   0     1001      127      537 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/model.nt
--rw-r--r--   0     1001      127     1248 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/model.ttl
--rw-r--r--   0     1001      127      789 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/model.xml
--rw-r--r--   0     1001      127      909 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl
--rw-r--r--   0     1001      127   146214 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl
--rw-r--r--   0     1001      127    30521 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl
--rw-r--r--   0     1001      127   163975 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl
--rw-r--r--   0     1001      127    18438 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl
--rw-r--r--   0     1001      127    18438 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl
--rw-r--r--   0     1001      127  1323794 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl
--rw-r--r--   0     1001      127    17472 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl
--rw-r--r--   0     1001      127  1456008 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl
--rw-r--r--   0     1001      127   104496 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl
--rw-r--r--   0     1001      127  1255550 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/bacnet.ttl
--rw-r--r--   0     1001      127    44502 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/brickpatches.ttl
--rw-r--r--   0     1001      127    81761 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/rec.ttl
--rw-r--r--   0     1001      127     4069 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/recimports.ttl
--rw-r--r--   0     1001      127    11876 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data/support/ref-schema.ttl
--rw-r--r--   0     1001      127     1160 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data2/ont1.ttl
--rw-r--r--   0     1001      127     1132 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data2/ont2.ttl
--rw-r--r--   0     1001      127     1135 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data2/ont3.ttl
--rw-r--r--   0     1001      127     1106 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/data2/ont4.ttl
--rw-r--r--   0     1001      127     1248 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/fileendings/model
--rw-r--r--   0     1001      127      321 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/fileendings/model.n3
--rw-r--r--   0     1001      127      537 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/fileendings/model.nt
--rw-r--r--   0     1001      127     1248 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/fileendings/model.ttl
--rw-r--r--   0     1001      127      789 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/fileendings/model.xml
--rw-r--r--   0     1001      127  1689944 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl
--rw-r--r--   0     1001      127     1160 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/updates/v1/ont1.ttl
--rw-r--r--   0     1001      127     1132 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/updates/v1/ont2.ttl
--rw-r--r--   0     1001      127     1135 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/updates/v1/ont3.ttl
--rw-r--r--   0     1001      127     1106 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/updates/v1/ont4.ttl
--rw-r--r--   0     1001      127     1135 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/updates/v2/ont3.ttl
--rw-r--r--   0     1001      127     1129 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/lib/tests/updates/v2/ont5.ttl
--rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a1/python/Cargo.toml
--rw-r--r--   0     1001      127     2886 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/python/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/python/.gitignore
--rw-r--r--   0     1001      127      731 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/python/README.md
--rw-r--r--   0     1001      127       71 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/python/build.rs
--rw-r--r--   0     1001      127     5241 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/python/poetry.lock
--rw-r--r--   0     1001      127       71 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/python/requirements.dev.txt
--rw-r--r--   0     1001      127    14445 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/python/src/lib.rs
--rw-r--r--   0     1001      127      694 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/python/test.py
--rw-r--r--   0     1001      127    73227 2024-05-21 16:21:56.000000 pyontoenv-0.1.7a1/Cargo.lock
--rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a1/Cargo.toml
--rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a1/pyproject.toml
--rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a1/PKG-INFO
+-rw-r--r--   0     1001      127      776 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/Cargo.toml
+-rw-r--r--   0     1001      127     5324 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/src/config.rs
+-rw-r--r--   0     1001      127     2180 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/src/consts.rs
+-rw-r--r--   0     1001      127     3267 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/src/doctor.rs
+-rw-r--r--   0     1001      127      350 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/src/errors.rs
+-rw-r--r--   0     1001      127    38662 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/src/lib.rs
+-rw-r--r--   0     1001      127    13633 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/src/ontology.rs
+-rw-r--r--   0     1001      127     3521 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/src/policy.rs
+-rw-r--r--   0     1001      127     4646 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/src/transform.rs
+-rw-r--r--   0     1001      127     6428 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/src/util.rs
+-rw-r--r--   0     1001      127  1689944 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data/Brick-1.3.ttl
+-rw-r--r--   0     1001      127     1248 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data/model
+-rw-r--r--   0     1001      127      321 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data/model.n3
+-rw-r--r--   0     1001      127      537 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data/model.nt
+-rw-r--r--   0     1001      127     1248 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data/model.ttl
+-rw-r--r--   0     1001      127      789 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data/model.xml
+-rw-r--r--   0     1001      127      909 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl
+-rw-r--r--   0     1001      127   146214 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl
+-rw-r--r--   0     1001      127    30521 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl
+-rw-r--r--   0     1001      127   163975 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl
+-rw-r--r--   0     1001      127    18438 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl
+-rw-r--r--   0     1001      127    18438 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl
+-rw-r--r--   0     1001      127  1323794 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl
+-rw-r--r--   0     1001      127    17472 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl
+-rw-r--r--   0     1001      127  1456008 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl
+-rw-r--r--   0     1001      127   104496 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl
+-rw-r--r--   0     1001      127  1255550 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data/support/bacnet.ttl
+-rw-r--r--   0     1001      127    44502 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data/support/brickpatches.ttl
+-rw-r--r--   0     1001      127    81761 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data/support/rec.ttl
+-rw-r--r--   0     1001      127     4069 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data/support/recimports.ttl
+-rw-r--r--   0     1001      127    11876 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data/support/ref-schema.ttl
+-rw-r--r--   0     1001      127     1160 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data2/ont1.ttl
+-rw-r--r--   0     1001      127     1132 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data2/ont2.ttl
+-rw-r--r--   0     1001      127     1135 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data2/ont3.ttl
+-rw-r--r--   0     1001      127     1106 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/data2/ont4.ttl
+-rw-r--r--   0     1001      127     1248 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/fileendings/model
+-rw-r--r--   0     1001      127      321 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/fileendings/model.n3
+-rw-r--r--   0     1001      127      537 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/fileendings/model.nt
+-rw-r--r--   0     1001      127     1248 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/fileendings/model.ttl
+-rw-r--r--   0     1001      127      789 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/fileendings/model.xml
+-rw-r--r--   0     1001      127  1689944 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl
+-rw-r--r--   0     1001      127     1160 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/updates/v1/ont1.ttl
+-rw-r--r--   0     1001      127     1132 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/updates/v1/ont2.ttl
+-rw-r--r--   0     1001      127     1135 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/updates/v1/ont3.ttl
+-rw-r--r--   0     1001      127     1106 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/updates/v1/ont4.ttl
+-rw-r--r--   0     1001      127     1135 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/updates/v2/ont3.ttl
+-rw-r--r--   0     1001      127     1129 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/lib/tests/updates/v2/ont5.ttl
+-rw-r--r--   0        0        0      749 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a2/python/Cargo.toml
+-rw-r--r--   0     1001      127     2886 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/python/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/python/.gitignore
+-rw-r--r--   0     1001      127      731 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/python/README.md
+-rw-r--r--   0     1001      127       71 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/python/build.rs
+-rw-r--r--   0     1001      127     5241 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/python/poetry.lock
+-rw-r--r--   0     1001      127       71 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/python/requirements.dev.txt
+-rw-r--r--   0     1001      127    14231 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/python/src/lib.rs
+-rw-r--r--   0     1001      127      694 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/python/test.py
+-rw-r--r--   0     1001      127    73227 2024-05-22 14:51:41.000000 pyontoenv-0.1.7a2/Cargo.lock
+-rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a2/Cargo.toml
+-rw-r--r--   0        0        0      821 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a2/pyproject.toml
+-rw-r--r--   0        0        0     1375 1970-01-01 00:00:00.000000 pyontoenv-0.1.7a2/PKG-INFO
```

### Comparing `pyontoenv-0.1.7a1/lib/Cargo.toml` & `pyontoenv-0.1.7a2/lib/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/src/config.rs` & `pyontoenv-0.1.7a2/lib/src/config.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/src/consts.rs` & `pyontoenv-0.1.7a2/lib/src/consts.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/src/doctor.rs` & `pyontoenv-0.1.7a2/lib/src/doctor.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/src/lib.rs` & `pyontoenv-0.1.7a2/lib/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/src/ontology.rs` & `pyontoenv-0.1.7a2/lib/src/ontology.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/src/policy.rs` & `pyontoenv-0.1.7a2/lib/src/policy.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/src/transform.rs` & `pyontoenv-0.1.7a2/lib/src/transform.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/src/util.rs` & `pyontoenv-0.1.7a2/lib/src/util.rs`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data/Brick-1.3.ttl` & `pyontoenv-0.1.7a2/lib/tests/data/Brick-1.3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data/model` & `pyontoenv-0.1.7a2/lib/tests/data/model`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data/model.nt` & `pyontoenv-0.1.7a2/lib/tests/data/model.nt`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data/model.ttl` & `pyontoenv-0.1.7a2/lib/tests/data/model.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data/model.xml` & `pyontoenv-0.1.7a2/lib/tests/data/model.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl` & `pyontoenv-0.1.7a2/lib/tests/data/support/SCHEMA-FACADE_QUDT-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl` & `pyontoenv-0.1.7a2/lib/tests/data/support/SCHEMA_QUDT_NoOWL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl` & `pyontoenv-0.1.7a2/lib/tests/data/support/SHACL-SCHEMA-SUPPLEMENT_QUDT-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl` & `pyontoenv-0.1.7a2/lib/tests/data/support/VOCAB_QUDT-DIMENSION-VECTORS-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl` & `pyontoenv-0.1.7a2/lib/tests/data/support/VOCAB_QUDT-PREFIX-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl` & `pyontoenv-0.1.7a2/lib/tests/data/support/VOCAB_QUDT-PREFIXES-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl` & `pyontoenv-0.1.7a2/lib/tests/data/support/VOCAB_QUDT-QUANTITY-KINDS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl` & `pyontoenv-0.1.7a2/lib/tests/data/support/VOCAB_QUDT-SYSTEM-OF-UNITS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl` & `pyontoenv-0.1.7a2/lib/tests/data/support/VOCAB_QUDT-UNITS-ALL-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl` & `pyontoenv-0.1.7a2/lib/tests/data/support/VOCAB_QUDT-UNITS-CURRENCY-v2.1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data/support/bacnet.ttl` & `pyontoenv-0.1.7a2/lib/tests/data/support/bacnet.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data/support/brickpatches.ttl` & `pyontoenv-0.1.7a2/lib/tests/data/support/brickpatches.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data/support/rec.ttl` & `pyontoenv-0.1.7a2/lib/tests/data/support/rec.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data/support/recimports.ttl` & `pyontoenv-0.1.7a2/lib/tests/data/support/recimports.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data/support/ref-schema.ttl` & `pyontoenv-0.1.7a2/lib/tests/data/support/ref-schema.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data2/ont1.ttl` & `pyontoenv-0.1.7a2/lib/tests/data2/ont1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data2/ont2.ttl` & `pyontoenv-0.1.7a2/lib/tests/data2/ont2.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data2/ont3.ttl` & `pyontoenv-0.1.7a2/lib/tests/data2/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/data2/ont4.ttl` & `pyontoenv-0.1.7a2/lib/tests/data2/ont4.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/fileendings/model` & `pyontoenv-0.1.7a2/lib/tests/fileendings/model`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/fileendings/model.nt` & `pyontoenv-0.1.7a2/lib/tests/fileendings/model.nt`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/fileendings/model.ttl` & `pyontoenv-0.1.7a2/lib/tests/fileendings/model.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/fileendings/model.xml` & `pyontoenv-0.1.7a2/lib/tests/fileendings/model.xml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl` & `pyontoenv-0.1.7a2/lib/tests/updated-ontologies/Brick-1.4-rc1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/updates/v1/ont1.ttl` & `pyontoenv-0.1.7a2/lib/tests/updates/v1/ont1.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/updates/v1/ont2.ttl` & `pyontoenv-0.1.7a2/lib/tests/updates/v1/ont2.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/updates/v1/ont3.ttl` & `pyontoenv-0.1.7a2/lib/tests/updates/v1/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/updates/v1/ont4.ttl` & `pyontoenv-0.1.7a2/lib/tests/updates/v1/ont4.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/updates/v2/ont3.ttl` & `pyontoenv-0.1.7a2/lib/tests/updates/v2/ont3.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/lib/tests/updates/v2/ont5.ttl` & `pyontoenv-0.1.7a2/lib/tests/updates/v2/ont5.ttl`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/python/Cargo.toml` & `pyontoenv-0.1.7a2/python/Cargo.toml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/python/.github/workflows/CI.yml` & `pyontoenv-0.1.7a2/python/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/python/.gitignore` & `pyontoenv-0.1.7a2/python/.gitignore`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/python/README.md` & `pyontoenv-0.1.7a2/python/README.md`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/python/poetry.lock` & `pyontoenv-0.1.7a2/python/poetry.lock`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/python/src/lib.rs` & `pyontoenv-0.1.7a2/python/src/lib.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 use ::ontoenv as ontoenvrs;
 use ::ontoenv::consts::{ONTOLOGY, TYPE};
 use ::ontoenv::ontology::OntologyLocation;
 use ::ontoenv::transform;
 use anyhow::Error;
+use std::sync::{Arc, Mutex, Once, OnceLock};
 use oxigraph::model::{BlankNode, Literal, NamedNode, Term, SubjectRef};
 use pyo3::{
     prelude::*,
     types::{PyString, PyTuple, IntoPyDict},
 };
 use std::borrow::Borrow;
 use std::path::{Path, PathBuf};
-use std::sync::Once;
 
 static INIT: Once = Once::new();
+static ONTOENV_SINGLETON: OnceLock<Arc<Mutex<ontoenvrs::OntoEnv>>> = OnceLock::new();
 
 fn anyhow_to_pyerr(e: Error) -> PyErr {
     PyErr::new::<pyo3::exceptions::PyValueError, _>(e.to_string())
 }
 
 #[allow(dead_code)]
 struct MyTerm(Term);
@@ -59,15 +60,15 @@
         };
         MyTerm(n)
     }
 }
 
 fn term_to_python<'a>(
     py: Python,
-    rdflib: &'a Bound<PyModule>,
+    rdflib: &Bound<'a, PyModule>,
     node: Term,
 ) -> PyResult<Bound<'a, PyAny>> {
     let dtype: Option<String> = match &node {
         Term::Literal(lit) => {
             let mut s = lit.datatype().to_string();
             s.remove(0);
             s.remove(s.len() - 1);
@@ -76,15 +77,15 @@
         _ => None,
     };
     let lang: Option<&str> = match &node {
         Term::Literal(lit) => lit.language(),
         _ => None,
     };
 
-    let res: Bound<PyAny> = match &node {
+    let res: Bound<'_, PyAny> = match &node {
         Term::NamedNode(uri) => {
             let mut uri = uri.to_string();
             uri.remove(0);
             uri.remove(uri.len() - 1);
             rdflib.getattr("URIRef")?.call1((uri,))?
         }
         Term::Literal(literal) => {
@@ -161,112 +162,115 @@
             .map_err(|e| PyErr::new::<pyo3::exceptions::PyValueError, _>(e.to_string()))?,
         })
     }
 }
 
 #[pyclass]
 struct OntoEnv {
-    inner: ontoenvrs::OntoEnv,
+    inner: Arc<Mutex<ontoenvrs::OntoEnv>>,
 }
 
 #[pymethods]
 impl OntoEnv {
     #[new]
     #[pyo3(signature = (config=None, path=Path::new(".").to_owned(), recreate=false))]
     fn new(
         _py: Python,
-        config: Option<&Bound<'_, Config>>,
+        config: Option<&Config>,
         path: Option<PathBuf>,
         recreate: bool,
     ) -> PyResult<Self> {
         // wrap env_logger::init() in a Once to ensure it's only called once. This can
         // happen if a user script creates multiple OntoEnv instances
         INIT.call_once(|| {
             env_logger::init();
         });
 
-        let mut env = if let Some(p) = path {
-            let config_path = p.join(".ontoenv").join("ontoenv.json");
-            if let Ok(e) = ontoenvrs::OntoEnv::from_file(&config_path) {
-                println!("Loaded OntoEnv from file");
-                OntoEnv { inner: e }
-            } else {
-                println!("Creating new OntoEnv");
-                OntoEnv {
-                    inner: ontoenvrs::OntoEnv::new(config.unwrap().borrow().cfg.clone(), recreate)
-                        .map_err(anyhow_to_pyerr)?,
+        let env = ONTOENV_SINGLETON.get_or_init(|| {
+            let inner = if let Some(p) = path {
+                let config_path = p.join(".ontoenv").join("ontoenv.json");
+                if let Ok(env) = ontoenvrs::OntoEnv::from_file(&config_path) {
+                    println!("Loaded OntoEnv from file");
+                    env
+                } else {
+                    println!("Creating new OntoEnv");
+                    ontoenvrs::OntoEnv::new(config.unwrap().borrow().cfg.clone(), recreate)
+                        .expect("Failed to create OntoEnv")
                 }
-            }
-        } else {
-            OntoEnv {
-                inner: ontoenvrs::OntoEnv::new(config.unwrap().borrow().cfg.clone(), recreate)
-                    .map_err(anyhow_to_pyerr)?,
-            }
-        };
+            } else {
+                ontoenvrs::OntoEnv::new(config.unwrap().borrow().cfg.clone(), recreate)
+                    .expect("Failed to create OntoEnv")
+            };
+            Arc::new(Mutex::new(inner))
+        });
+
+        {
+            let mut env = env.lock().unwrap();
+            env.update().map_err(anyhow_to_pyerr)?;
+            env.save_to_directory().map_err(anyhow_to_pyerr)?;
+        }
 
-        env.inner.update().map_err(anyhow_to_pyerr)?;
-        env.inner.save_to_directory().map_err(anyhow_to_pyerr)?;
-        Ok(env)
+        Ok(OntoEnv {
+            inner: env.clone(),
+        })
     }
 
-    fn update(&mut self) -> PyResult<()> {
-        self.inner.update().map_err(anyhow_to_pyerr)?;
+    fn update(&self) -> PyResult<()> {
+        let mut inner = self.inner.lock().unwrap();
+        inner.update().map_err(anyhow_to_pyerr)?;
         Ok(())
     }
 
-    // define __repr__ for OntoEnv. It prints out the # of graphs in the OntoEnv
-    // and the total # of triples across all graphs
     fn __repr__(&self) -> PyResult<String> {
+        let inner = self.inner.lock().unwrap();
         Ok(format!(
             "<OntoEnv: {} graphs, {} triples>",
-            self.inner.num_graphs(),
-            self.inner.num_triples().map_err(anyhow_to_pyerr)?
+            inner.num_graphs(),
+            inner.num_triples().map_err(anyhow_to_pyerr)?
         ))
     }
 
+    // The following methods will now access the inner OntoEnv in a thread-safe manner:
+
     fn import_graph(&self, py: Python, destination_graph: &Bound<'_, PyAny>, uri: &str) -> PyResult<()> {
+        let inner = self.inner.lock().unwrap();
         let rdflib = py.import_bound("rdflib")?;
         let iri = NamedNode::new(uri)
             .map_err(|e| PyErr::new::<pyo3::exceptions::PyValueError, _>(e.to_string()))?;
-        let ont = self
-            .inner
+        let ont = inner
             .get_ontology_by_name(iri.as_ref())
             .ok_or_else(|| PyErr::new::<pyo3::exceptions::PyValueError, _>("Ontology not found"))?;
         let mut graph = ont.graph().map_err(anyhow_to_pyerr)?;
 
-        // get the owl:Ontology IRI from the destination_graph
-        // call value with TYPE and ONTOLOGY
         let uriref_constructor = rdflib.getattr("URIRef")?;
         let type_uri = uriref_constructor.call1((TYPE.as_str(),))?;
         let ontology_uri = uriref_constructor.call1((ONTOLOGY.as_str(),))?;
         let kwargs = [("predicate", type_uri), ("object", ontology_uri)].into_py_dict_bound(py);
         let result = destination_graph.call_method("value", (), Some(&kwargs))?;
         if !result.is_none() {
-            // extract the IRI from the result, turn into a SubjectRef
             let ontology = NamedNode::new(result.extract::<String>()?).map_err(|e| PyErr::new::<pyo3::exceptions::PyValueError, _>(e.to_string()))?;
             let base_ontology: SubjectRef = SubjectRef::NamedNode(ontology.as_ref());
 
-            // apply the transforms to make the graph compatible with the destination graph
             transform::rewrite_sh_prefixes_graph(&mut graph, base_ontology);
             transform::remove_ontology_declarations_graph(&mut graph, base_ontology);
         }
         transform::remove_owl_imports_graph(&mut graph);
 
         Python::with_gil(|_py| {
             for triple in graph.into_iter() {
                 let s: Term = triple.subject.into();
                 let p: Term = triple.predicate.into();
                 let o: Term = triple.object.into();
 
                 let t = PyTuple::new_bound(
-                    destination_graph.py(),
+                    py,
                     &[
-                        term_to_python(destination_graph.py(), &rdflib, s)?,
-                        term_to_python(destination_graph.py(), &rdflib, p)?,
-                        term_to_python(destination_graph.py(), &rdflib, o)?,
+                        term_to_python(py, &rdflib, s)?,
+                        term_to_python(py, &rdflib, p)?,
+                        term_to_python(py, &rdflib, o)?,
                     ],
                 );
 
                 destination_graph.getattr("add")?.call1((t,))?;
             }
             Ok::<(), PyErr>(())
         })?;
@@ -281,96 +285,92 @@
         destination_graph: &Bound<'_, PyAny>,
         rewrite_sh_prefixes: bool,
         remove_owl_imports: bool,
     ) -> PyResult<()> {
         let rdflib = py.import_bound("rdflib")?;
         let iri = NamedNode::new(uri)
             .map_err(|e| PyErr::new::<pyo3::exceptions::PyValueError, _>(e.to_string()))?;
-        let ont = self
-            .inner
+        let inner = self.inner.lock().unwrap();
+        let ont = inner
             .get_ontology_by_name(iri.as_ref())
             .ok_or_else(|| PyErr::new::<pyo3::exceptions::PyValueError, _>("Ontology not found"))?;
-        let closure = self
-            .inner
+        let closure = inner
             .get_dependency_closure(ont.id())
             .map_err(anyhow_to_pyerr)?;
-        let graph = self
-            .inner
+        let graph = inner
             .get_union_graph(
                 &closure,
                 Some(rewrite_sh_prefixes),
                 Some(remove_owl_imports),
             )
             .map_err(anyhow_to_pyerr)?;
         Python::with_gil(|_py| {
             for triple in graph.into_iter() {
                 let s: Term = triple.subject.into();
                 let p: Term = triple.predicate.into();
                 let o: Term = triple.object.into();
 
                 let t = PyTuple::new_bound(
-                    destination_graph.py(),
+                    py,
                     &[
-                        term_to_python(destination_graph.py(), &rdflib, s)?,
-                        term_to_python(destination_graph.py(), &rdflib, p)?,
-                        term_to_python(destination_graph.py(), &rdflib, o)?,
+                        term_to_python(py, &rdflib, s)?,
+                        term_to_python(py, &rdflib, p)?,
+                        term_to_python(py, &rdflib, o)?,
                     ],
                 );
 
                 destination_graph.getattr("add")?.call1((t,))?;
             }
             Ok::<(), PyErr>(())
         })?;
         Ok(())
     }
 
     fn dump(&self) -> PyResult<()> {
-        self.inner.dump();
+        let inner = self.inner.lock().unwrap();
+        inner.dump();
         Ok(())
     }
 
-    fn import_dependencies(&mut self, py: Python, graph: &Bound<'_, PyAny>) -> PyResult<()> {
+    fn import_dependencies(&self, py: Python, graph: &Bound<'_, PyAny>) -> PyResult<()> {
         let rdflib = py.import_bound("rdflib")?;
-        // get the subject of rdf:type owl:Ontology from the provided rdflib graph
         let py_rdf_type = term_to_python(py, &rdflib, Term::NamedNode(TYPE.into()))?;
         let py_ontology = term_to_python(py, &rdflib, Term::NamedNode(ONTOLOGY.into()))?;
         let value_fun: Py<PyAny> = graph.getattr("value")?.into();
         let ontology = value_fun.call1(py, (py_rdf_type, py_ontology))?;
 
-        // if ontology is null, return
-        // else, get the ontology IRI and add it to the OntoEnv
         if ontology.is_none(py) {
             return Ok(());
         }
 
-        // turn ontology into a string
         let ontology = ontology.to_string();
 
         self.get_closure(py, &ontology, graph, true, true)
     }
 
-    fn add(&mut self, _py: Python, location: &Bound<'_, PyAny>) -> PyResult<()> {
+    fn add(&self, location: &Bound<'_, PyAny>) -> PyResult<()> {
+        let mut inner = self.inner.lock().unwrap();
         let location =
             OntologyLocation::from_str(&location.to_string()).map_err(anyhow_to_pyerr)?;
-        self.inner.add(location).map_err(anyhow_to_pyerr)?;
+        inner.add(location).map_err(anyhow_to_pyerr)?;
         Ok(())
     }
 
-    fn refresh(&mut self) -> PyResult<()> {
-        self.inner.update().map_err(anyhow_to_pyerr)?;
+    fn refresh(&self) -> PyResult<()> {
+        let mut inner = self.inner.lock().unwrap();
+        inner.update().map_err(anyhow_to_pyerr)?;
         Ok(())
     }
 
-    #[pyo3(signature = (uri))]
     fn get_graph(&self, py: Python, uri: &Bound<'_, PyString>) -> PyResult<Py<PyAny>> {
         let rdflib = py.import_bound("rdflib")?;
         let iri = NamedNode::new(uri.to_string())
             .map_err(|e| PyErr::new::<pyo3::exceptions::PyValueError, _>(e.to_string()))?;
-        let graph = self
-            .inner
+        let inner = self.inner.lock().unwrap();
+        let graph = inner
             .get_graph_by_name(iri.as_ref())
             .map_err(anyhow_to_pyerr)?;
         let res = rdflib.getattr("Graph")?.call0()?;
         for triple in graph.into_iter() {
             let s: Term = triple.subject.into();
             let p: Term = triple.predicate.into();
             let o: Term = triple.object.into();
@@ -382,28 +382,27 @@
                     term_to_python(py, &rdflib, p)?,
                     term_to_python(py, &rdflib, o)?,
                 ],
             );
 
             res.getattr("add")?.call1((t,))?;
         }
-        Ok(res.unbind())
+        Ok(res.into())
     }
 
     fn get_ontology_names(&self) -> PyResult<Vec<String>> {
-        let names: Vec<String> = self
-            .inner
+        let inner = self.inner.lock().unwrap();
+        let names: Vec<String> = inner
             .ontologies()
             .keys()
             .map(|k| k.name().to_string())
             .collect();
         Ok(names)
     }
 }
 
-/// A Python module implemented in Rust.
 #[pymodule]
-fn ontoenv(_py: Python, m: Bound<PyModule>) -> PyResult<()> {
+fn ontoenv(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
     m.add_class::<Config>()?;
     m.add_class::<OntoEnv>()?;
     Ok(())
 }
```

### Comparing `pyontoenv-0.1.7a1/python/test.py` & `pyontoenv-0.1.7a2/python/test.py`

 * *Files identical despite different names*

### Comparing `pyontoenv-0.1.7a1/Cargo.lock` & `pyontoenv-0.1.7a2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1375,15 +1375,15 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "ontoenv"
-version = "0.1.7-a1"
+version = "0.1.7-a2"
 dependencies = [
  "anyhow",
  "chrono",
  "clap",
  "derive_builder",
  "env_logger",
  "glob",
@@ -1401,15 +1401,15 @@
  "tempdir",
  "tempfile",
  "walkdir",
 ]
 
 [[package]]
 name = "ontoenv-cli"
-version = "0.1.7-a1"
+version = "0.1.7-a2"
 dependencies = [
  "anyhow",
  "chrono",
  "clap",
  "env_logger",
  "ontoenv",
  "oxigraph",
@@ -1719,15 +1719,15 @@
  "pyo3-build-config",
  "quote",
  "syn 2.0.60",
 ]
 
 [[package]]
 name = "pyontoenv"
-version = "0.1.7-a1"
+version = "0.1.7-a2"
 dependencies = [
  "anyhow",
  "env_logger",
  "log",
  "ontoenv",
  "oxigraph",
  "pyo3",
```

### Comparing `pyontoenv-0.1.7a1/Cargo.toml` & `pyontoenv-0.1.7a2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [workspace]
 members = ["python"]
 resolver = "2"
 
 [workspace.package]
-version = "0.1.7-a1"
+version = "0.1.7-a2"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 license = "BSD-3-Clause"
 edition = "2021"
 rust-version = "1.70"
 repository = "https://github.com/gtfierro/ontoenv-rs"
 homepage = "https://github.com/gtfierro/ontoenv-rs"
 description = "A tool for managing ontologies and their dependencies"
@@ -27,8 +27,8 @@
 glob = "0.3.1"
 chrono = { version = "0.4.33", features = ["serde"] }
 petgraph = { version = "0.6.4", features = ["serde-1"] }
 clap = { version = "4.4.18", features = ["derive"] }
 derive_builder = "0.13.0"
 oxigraph = "0.3.22"
 
-ontoenv = { version = "0.1.7-a1", path = "lib" }
+ontoenv = { version = "0.1.7-a2", path = "lib" }
```

### Comparing `pyontoenv-0.1.7a1/pyproject.toml` & `pyontoenv-0.1.7a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 [tool.maturin]
 features = ["pyo3/extension-module"]
 manifest-path = "python/Cargo.toml"
 
 [tool.poetry]
 name = "ontoenv"
-version = "0.1.7a1"
+version = "0.1.7a2"
 description = "Python bindings for the OntoEnv Rust library. Manages ontology-based environments for building knowledge graphs."
 license = "bsd-3-clause"
 authors = ["Gabe Fierro <gtfierro@mines.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `pyontoenv-0.1.7a1/PKG-INFO` & `pyontoenv-0.1.7a2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyontoenv
-Version: 0.1.7a1
+Version: 0.1.7a2
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Command line tool to manage ontologies and their imports in a local environment
 Home-Page: https://github.com/gtfierro/ontoenv-rs
 Author: Gabe Fierro <gtfierro@mines.edu>
 Author-email: Gabe Fierro <gtfierro@mines.edu>
```

