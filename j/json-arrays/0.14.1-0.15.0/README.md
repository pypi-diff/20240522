# Comparing `tmp/json_arrays-0.14.1.tar.gz` & `tmp/json_arrays-0.15.0.tar.gz`

## Comparing `json_arrays-0.14.1.tar` & `json_arrays-0.15.0.tar`

### file list

```diff
@@ -1,83 +1,95 @@
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 json_arrays-0.14.1/.bumpversion.toml
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 json_arrays-0.14.1/.coveragerc
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 json_arrays-0.14.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 json_arrays-0.14.1/.sourcery.yaml
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 json_arrays-0.14.1/CHANGELOG.md
--rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 json_arrays-0.14.1/Makefile
--rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 json_arrays-0.14.1/cliff.toml
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 json_arrays-0.14.1/codecov.yml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 json_arrays-0.14.1/committed.toml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 json_arrays-0.14.1/mypy.ini
--rw-r--r--   0        0        0    71576 2020-02-02 00:00:00.000000 json_arrays-0.14.1/pdm.dev.orjson.lock
--rw-r--r--   0        0        0    64937 2020-02-02 00:00:00.000000 json_arrays-0.14.1/pdm.lock
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 json_arrays-0.14.1/ruff.toml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 json_arrays-0.14.1/.grit/patterns/avoid_pipe_unions.md
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 json_arrays-0.14.1/benches/update_doc.py
--rw-r--r--   0        0        0 17178958 2020-02-02 00:00:00.000000 json_arrays-0.14.1/benches/data/skbl.json
--rw-r--r--   0        0        0 10886024 2020-02-02 00:00:00.000000 json_arrays-0.14.1/benches/data/skbl.json.updated.json
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 json_arrays-0.14.1/examples/jq_length.py
--rw-r--r--   0        0        0     6660 2020-02-02 00:00:00.000000 json_arrays-0.14.1/src/json_arrays/__init__.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 json_arrays-0.14.1/src/json_arrays/_types.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 json_arrays-0.14.1/src/json_arrays/exceptions.py
--rw-r--r--   0        0        0     2386 2020-02-02 00:00:00.000000 json_arrays-0.14.1/src/json_arrays/files.py
--rw-r--r--   0        0        0     3061 2020-02-02 00:00:00.000000 json_arrays-0.14.1/src/json_arrays/json_iter.py
--rw-r--r--   0        0        0     1797 2020-02-02 00:00:00.000000 json_arrays-0.14.1/src/json_arrays/jsonl_iter.py
--rw-r--r--   0        0        0     1467 2020-02-02 00:00:00.000000 json_arrays-0.14.1/src/json_arrays/jsonlib.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 json_arrays-0.14.1/src/json_arrays/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 json_arrays-0.14.1/src/json_arrays/backends/__init__.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 json_arrays-0.14.1/src/json_arrays/backends/be_json.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 json_arrays-0.14.1/src/json_arrays/backends/be_orjson.py
--rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 json_arrays-0.14.1/src/json_arrays/encoders/__init__.py
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 json_arrays-0.14.1/src/json_arrays/encoders/decimal_encoders.py
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 json_arrays-0.14.1/src/json_arrays/utility/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/__init__.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/conftest.py
--rw-r--r--   0        0        0    28935 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/requirements-testing.lock
--rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/test_iter.py
--rw-r--r--   0        0        0     8689 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/test_json_arrays_api.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/test_json_iter_api.py
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/test_jsonlib_api.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/test_utility.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/utils.py
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/__snapshots__/test_json_arrays_api.ambr
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/__snapshots__/test_json_iter_api.ambr
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/__snapshots__/test_jsonlib_api.ambr
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/__snapshots__/test_iter/test_load_file_name[json_arrays.json_iter-testsdataarray.json-rb].json
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/__snapshots__/test_json_arrays_api/test_json_gzip_dump_fp.json
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/__snapshots__/test_json_arrays_api/test_json_gzip_load_fp.json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/__snapshots__/test_json_arrays_api/test_load[testsdataarray.json].json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/__snapshots__/test_json_arrays_api/test_load[testsdataarray.jsonl].json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/__snapshots__/test_json_arrays_api/test_load[testsdataarray.ndjson].json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/__snapshots__/test_json_arrays_api/test_load_from_file[testsdataarray.json.gz].json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/__snapshots__/test_json_arrays_api/test_load_from_file[testsdataarray.json].json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/__snapshots__/test_json_arrays_api/test_load_from_file[testsdataarray.jsonl.gz].json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/__snapshots__/test_json_arrays_api/test_load_from_file[testsdataarray.jsonl].json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/__snapshots__/test_json_arrays_api/test_load_from_file[testsdataarray.ndjson.gz].json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/__snapshots__/test_json_arrays_api/test_load_from_file[testsdataarray.ndjson].json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/__snapshots__/test_json_arrays_api/test_load_from_file_stdin[testsdataarray.json-json].json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/__snapshots__/test_json_arrays_api/test_load_from_file_stdin[testsdataarray.jsonl-None].json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/__snapshots__/test_json_arrays_api/test_load_from_file_stdin[testsdataarray.jsonl-jsonl].json
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/__snapshots__/test_jsonlib_api/test_load_from_file.json
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/data/array.json
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/data/array.json.gz
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/data/array.jsonl
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/data/array.jsonl.gz
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/data/array.ndjson -> array.jsonl
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/data/array.ndjson.gz -> array.jsonl.gz
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/data/dict.json
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/data/invalid.json
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/data/invalid_many.json
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/data/invalid_property.json
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/data/invalid_type.json
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/data/objs.jsonl.gz
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/data/schema_default.json
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/data/schema_test.json
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/data/valid_array.json
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/data/valid_object.json
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/data/validated.json
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/data/validated.jsonl
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 json_arrays-0.14.1/tests/unit/test_filenames.py
--rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 json_arrays-0.14.1/.gitignore
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 json_arrays-0.14.1/README.md
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 json_arrays-0.14.1/pyproject.toml
--rw-r--r--   0        0        0     4841 2020-02-02 00:00:00.000000 json_arrays-0.14.1/PKG-INFO
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 json_arrays-0.15.0/.bumpversion.toml
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 json_arrays-0.15.0/.coveragerc
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 json_arrays-0.15.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 json_arrays-0.15.0/.sourcery.yaml
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 json_arrays-0.15.0/CHANGELOG.md
+-rw-r--r--   0        0        0     3678 2020-02-02 00:00:00.000000 json_arrays-0.15.0/Makefile
+-rw-r--r--   0        0        0     3150 2020-02-02 00:00:00.000000 json_arrays-0.15.0/cliff.toml
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 json_arrays-0.15.0/codecov.yml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 json_arrays-0.15.0/committed.toml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 json_arrays-0.15.0/mypy.ini
+-rw-r--r--   0        0        0    71576 2020-02-02 00:00:00.000000 json_arrays-0.15.0/pdm.dev.orjson.lock
+-rw-r--r--   0        0        0    64937 2020-02-02 00:00:00.000000 json_arrays-0.15.0/pdm.lock
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 json_arrays-0.15.0/ruff.toml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 json_arrays-0.15.0/.grit/patterns/avoid_pipe_unions.md
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 json_arrays-0.15.0/benches/update_doc.py
+-rw-r--r--   0        0        0 17178958 2020-02-02 00:00:00.000000 json_arrays-0.15.0/benches/data/skbl.json
+-rw-r--r--   0        0        0 10886024 2020-02-02 00:00:00.000000 json_arrays-0.15.0/benches/data/skbl.json.updated.json
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 json_arrays-0.15.0/examples/jq_length.py
+-rw-r--r--   0        0        0     6660 2020-02-02 00:00:00.000000 json_arrays-0.15.0/src/json_arrays/__init__.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 json_arrays-0.15.0/src/json_arrays/_types.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 json_arrays-0.15.0/src/json_arrays/exceptions.py
+-rw-r--r--   0        0        0     3020 2020-02-02 00:00:00.000000 json_arrays-0.15.0/src/json_arrays/files.py
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 json_arrays-0.15.0/src/json_arrays/json_iter.py
+-rw-r--r--   0        0        0     1685 2020-02-02 00:00:00.000000 json_arrays-0.15.0/src/json_arrays/jsonl_iter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 json_arrays-0.15.0/src/json_arrays/py.typed
+-rw-r--r--   0        0        0      298 2020-02-02 00:00:00.000000 json_arrays-0.15.0/src/json_arrays/encoders/__init__.py
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 json_arrays-0.15.0/src/json_arrays/encoders/decimal_encoders.py
+-rw-r--r--   0        0        0     1475 2020-02-02 00:00:00.000000 json_arrays-0.15.0/src/json_arrays/jsonlib/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 json_arrays-0.15.0/src/json_arrays/jsonlib/backends/__init__.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 json_arrays-0.15.0/src/json_arrays/jsonlib/backends/be_json.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 json_arrays-0.15.0/src/json_arrays/jsonlib/backends/be_orjson.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 json_arrays-0.15.0/src/json_arrays/shared/__init__.py
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 json_arrays-0.15.0/src/json_arrays/shared/writer.py
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 json_arrays-0.15.0/src/json_arrays/utility/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__init__.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/conftest.py
+-rw-r--r--   0        0        0    28935 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/requirements-testing.lock
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/test_files.py
+-rw-r--r--   0        0        0     2471 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/test_iter.py
+-rw-r--r--   0        0        0    10316 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/test_json_arrays_api.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/test_json_iter_api.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/test_jsonlib_api.py
+-rw-r--r--   0        0        0     1516 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/test_utility.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/utils.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api.ambr
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_iter_api.ambr
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_jsonlib_api.ambr
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_iter/test_load_file_name[json_arrays.json_iter-testsdataarray.json-rb].json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api/test_json_bzip2_dump_fp.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api/test_json_bzip2_load_fileobj.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api/test_json_bzip2_load_fp.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api/test_json_gzip_dump_fp.json
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api/test_json_gzip_load_fp.json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api/test_load[testsdataarray.json].json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api/test_load[testsdataarray.jsonl].json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api/test_load[testsdataarray.ndjson].json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api/test_load_from_file[testsdataarray.json.bz2].json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api/test_load_from_file[testsdataarray.json.gz].json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api/test_load_from_file[testsdataarray.json].json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api/test_load_from_file[testsdataarray.jsonl.bz2].json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api/test_load_from_file[testsdataarray.jsonl.gz].json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api/test_load_from_file[testsdataarray.jsonl].json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api/test_load_from_file[testsdataarray.ndjson.bz2].json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api/test_load_from_file[testsdataarray.ndjson.gz].json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api/test_load_from_file[testsdataarray.ndjson].json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api/test_load_from_file_stdin[testsdataarray.json-json].json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api/test_load_from_file_stdin[testsdataarray.jsonl-None].json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api/test_load_from_file_stdin[testsdataarray.jsonl-jsonl].json
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/__snapshots__/test_jsonlib_api/test_load_from_file.json
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/data/array.json
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/data/array.json.bz2
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/data/array.json.gz
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/data/array.jsonl
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/data/array.jsonl.bz2
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/data/array.jsonl.gz
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/data/array.ndjson -> array.jsonl
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/data/array.ndjson.bz2 -> array.jsonl.bz2
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/data/array.ndjson.gz -> array.jsonl.gz
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/data/dict.json
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/data/invalid.json
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/data/invalid_many.json
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/data/invalid_property.json
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/data/invalid_type.json
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/data/objs.jsonl.gz
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/data/schema_default.json
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/data/schema_test.json
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/data/valid_array.json
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/data/valid_object.json
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/data/validated.json
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/data/validated.jsonl
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 json_arrays-0.15.0/tests/unit/test_filenames.py
+-rw-r--r--   0        0        0     1365 2020-02-02 00:00:00.000000 json_arrays-0.15.0/.gitignore
+-rw-r--r--   0        0        0     3724 2020-02-02 00:00:00.000000 json_arrays-0.15.0/README.md
+-rw-r--r--   0        0        0     2265 2020-02-02 00:00:00.000000 json_arrays-0.15.0/pyproject.toml
+-rw-r--r--   0        0        0     4849 2020-02-02 00:00:00.000000 json_arrays-0.15.0/PKG-INFO
```

### Comparing `json_arrays-0.14.1/.bumpversion.toml` & `json_arrays-0.15.0/.bumpversion.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tool.bumpversion]
-current_version = "0.14.1"
+current_version = "0.15.0"
 parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
 serialize = ["{major}.{minor}.{patch}"]
 tag = true
 sign_tags = true
 tag_name = "v{new_version}"
 tag_message = "bump version: {current_version} → {new_version}"
 allow_dirty = false
```

### Comparing `json_arrays-0.14.1/.pre-commit-config.yaml` & `json_arrays-0.15.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `json_arrays-0.14.1/CHANGELOG.md` & `json_arrays-0.15.0/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,35 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [0.15.0] - 2024-05-22
+
+### Added
+
+- Add bzip2 support
+
+### Changed
+
+- Make jsonlib and backends to separate module
+- Move json_iter.dumps to writer
+- Use writer for json_lines
+
+### Documentation
+
+- Update CI badges
+- Update author
+- Use correct repo
+
+### Miscellaneous Tasks
+
+- Update cliff config
+- Use hashes from pdm.lock also
+- Remove nightly step in scheduled
+
 ## [0.14.1] - 2024-03-26
 
 ### Documentation
 
 - Add doc-test for encoders
 - Add pyversion classifiers
```

### Comparing `json_arrays-0.14.1/Makefile` & `json_arrays-0.15.0/Makefile`

 * *Files identical despite different names*

### Comparing `json_arrays-0.14.1/cliff.toml` & `json_arrays-0.15.0/cliff.toml`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
   { message = "^style", group = "Styling" },
   { message = "^test", group = "Testing" },
   { message = "^chore\\(release\\): prepare for", skip = true },
   { message = "^chore\\(deps\\)", skip = true },
   { message = "^chore\\(pr\\)", skip = true },
   { message = "^chore\\(pull\\)", skip = true },
   { message = "^build\\(release\\): prepare for", skip = true },
-  { message = "^build\\(deps\\)", skip = true },
+  { message = "^build\\(deps.*\\)", skip = true },
   { message = "^build\\(pr\\)", skip = true },
   { message = "^build\\(pull\\)", skip = true },
   { message = "^chore|ci", group = "Miscellaneous Tasks" },
   { body = ".*security", group = "Security" },
   { message = "^revert", group = "Revert" },
 ]
 # protect breaking changes from being skipped due to matching a skipping commit_parser
```

### Comparing `json_arrays-0.14.1/pdm.dev.orjson.lock` & `json_arrays-0.15.0/pdm.dev.orjson.lock`

 * *Files identical despite different names*

### Comparing `json_arrays-0.14.1/pdm.lock` & `json_arrays-0.15.0/pdm.lock`

 * *Files identical despite different names*

### Comparing `json_arrays-0.14.1/ruff.toml` & `json_arrays-0.15.0/ruff.toml`

 * *Files identical despite different names*

### Comparing `json_arrays-0.14.1/benches/data/skbl.json` & `json_arrays-0.15.0/benches/data/skbl.json`

 * *Files identical despite different names*

### Comparing `json_arrays-0.14.1/benches/data/skbl.json.updated.json` & `json_arrays-0.15.0/benches/data/skbl.json.updated.json`

 * *Files identical despite different names*

### Comparing `json_arrays-0.14.1/src/json_arrays/__init__.py` & `json_arrays-0.15.0/src/json_arrays/__init__.py`

 * *Files identical despite different names*

### Comparing `json_arrays-0.14.1/src/json_arrays/json_iter.py` & `json_arrays-0.15.0/src/json_arrays/json_iter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,38 @@
 """Handle JSON lazily."""
 
+import typing
 from typing import Iterable, Union
 
 import ijson  # type: ignore
 
-from json_arrays import _types, files, jsonlib, utility
+from json_arrays import _types, files, jsonlib, shared, utility
 
 
 def dump(data: Union[dict, Iterable], fileobj: _types.File, **kwargs):
     """Dump array to a file object.
 
     Parameters
     ----------
     data : dict | Iterable
         Iterable object to write.
     fileobj : _types.File
         File object to write to. Must be writable.
 
     """
     fp = files.BinaryFileWrite(fileobj=fileobj)
-    for chunk in dumps(data, **kwargs):
+    writer = shared.JsonArrayWriter()
+    for chunk in writer.dumps(data, **kwargs):
         fp.write(chunk)
     fp.close()
 
 
-def dumps(obj, **kwargs) -> Iterable[bytes]:
-    if isinstance(obj, str):
-        yield jsonlib.dumps(obj, **kwargs)
-    elif isinstance(obj, dict):
-        yield b"{"
-        for i, (key, value) in enumerate(obj.items()):
-            if i > 0:
-                yield b","
-            yield b'"%s":' % utility.to_bytes(key)
-            yield from dumps(value, **kwargs)
-        yield b"}"
-    else:
-        try:
-            it = iter(obj)
-        except TypeError:
-            yield jsonlib.dumps(obj, **kwargs)
-        else:
-            yield b"["
-            for i, o in enumerate(it):
-                if i > 0:
-                    yield b","
-                yield jsonlib.dumps(o, **kwargs)
-
-            yield b"]"
+def dumps(obj, **kwargs) -> typing.Iterable[bytes]:
+    writer = shared.JsonArrayWriter()
+    yield from writer.dumps(obj, **kwargs)
 
 
 def load(fileobj: _types.File, *, use_float: bool = True, **kwargs) -> Iterable:
     fp = files.BinaryFileRead(fileobj=fileobj)
     kwargs = {"use_float": use_float} | kwargs
     yield from ijson.items(fp.file, "item", **kwargs)
```

### Comparing `json_arrays-0.14.1/src/json_arrays/jsonl_iter.py` & `json_arrays-0.15.0/src/json_arrays/jsonl_iter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 """Handle JSON-LINES lazily."""
 
 import contextlib
 from typing import Iterable, Union
 
-from json_arrays import _types, files, jsonlib, utility
+from json_arrays import _types, files, jsonlib, shared, utility
 
 
 def dump(data: Union[dict, Iterable], fileobj: _types.File, **kwargs):
     fp = files.BinaryFileWrite(fileobj=fileobj)
-    if isinstance(data, (dict, str)):
-        fp.write(jsonlib.dumps(data, **kwargs))
-        fp.write(b"\n")
-        return
-
-    try:
-        for obj in data:
-            fp.write(jsonlib.dumps(obj, **kwargs))
-            fp.write(b"\n")
-    except TypeError:
-        fp.write(jsonlib.dumps(data, **kwargs))
+    writer = shared.JsonArrayWriter(json_lines=True)
+    did_write = False
+    for chunk in writer.dumps(data, **kwargs):
+        fp.write(chunk)
+        did_write = True
+    if did_write:
         fp.write(b"\n")
     fp.close()
 
 
 def load(fileobj: _types.File, **kwargs) -> Iterable:
     fp = files.BinaryFileRead(fileobj=fileobj)
     for line in fp.file:
```

### Comparing `json_arrays-0.14.1/src/json_arrays/jsonlib.py` & `json_arrays-0.15.0/src/json_arrays/jsonlib/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from json_arrays import _types, files
 
 
 def get_backend(backend_name: str):
     """Import the backend named `backend`"""
     import importlib
 
-    return importlib.import_module(f"json_arrays.backends.{backend_name}")
+    return importlib.import_module(f"json_arrays.jsonlib.backends.{backend_name}")
 
 
 def _default_backend():
     for backend_name in ("be_orjson", "be_json"):
         try:
             return get_backend(backend_name)
         except ImportError:
```

### Comparing `json_arrays-0.14.1/src/json_arrays/utility/__init__.py` & `json_arrays-0.15.0/src/json_arrays/utility/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,26 +22,32 @@
 
     Returns:
         {bool} -- True if this name is jsonl.
     """
     if name in ["<stdin>", "<stdout>"]:
         return True
     base, suffix = os.path.splitext(str(name))
-    if suffix == ".gz":
+    if suffix in [".gz", ".bz2"]:
         _, suffix = os.path.splitext(base)
     # print('suffix = {suffix}'.format(suffix=suffix))
     return suffix in [".jsonl", ".jl", ".ndjson"]
 
 
 def is_gzip(name: _types.Pathlike) -> bool:
     """Test if a filename is gzip."""
     _, suffix = os.path.splitext(str(name))
     return suffix == ".gz"
 
 
+def is_bzip2(name: _types.Pathlike) -> bool:
+    """Test if a filename is gzip."""
+    _, suffix = os.path.splitext(str(name))
+    return suffix == ".bz2"
+
+
 def to_bytes(s: Union[str, bytes, bytearray]) -> Union[bytes, bytearray]:
     """Convert str to bytes, otherwise pass through s
 
     Args:
         s (Union[str, bytes, bytearray]): the argument to assure bytes
 
     Returns:
```

### Comparing `json_arrays-0.14.1/tests/conftest.py` & `json_arrays-0.15.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `json_arrays-0.14.1/tests/requirements-testing.lock` & `json_arrays-0.15.0/tests/requirements-testing.lock`

 * *Files identical despite different names*

### Comparing `json_arrays-0.14.1/tests/test_iter.py` & `json_arrays-0.15.0/tests/test_iter.py`

 * *Files identical despite different names*

### Comparing `json_arrays-0.14.1/tests/test_json_arrays_api.py` & `json_arrays-0.15.0/tests/test_json_arrays_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import bz2
 import gzip
 import io
 import json
 import tempfile
 from pathlib import Path
 from typing import Optional
 from unittest.mock import patch
@@ -17,14 +18,17 @@
     [
         "tests/data/array.json",
         "tests/data/array.jsonl",
         "tests/data/array.ndjson",
         "tests/data/array.json.gz",
         "tests/data/array.jsonl.gz",
         "tests/data/array.ndjson.gz",
+        "tests/data/array.json.bz2",
+        "tests/data/array.jsonl.bz2",
+        "tests/data/array.ndjson.bz2",
     ],
 )
 def test_load_from_file(file_name: str, snapshot_json):
     assert list(json_arrays.load_from_file(file_name)) == snapshot_json
 
 
 @pytest.mark.parametrize(
@@ -112,20 +116,23 @@
 
     assert data_written == snapshot
 
 
 @pytest.mark.parametrize(
     "file_name",
     [
-        "tests/data/gen/api_array.json",
-        "tests/data/gen/api_array.jsonl",
-        "tests/data/gen/api_array.ndjson",
-        "tests/data/gen/api_array.json.gz",
-        "tests/data/gen/api_array.jsonl.gz",
-        "tests/data/gen/api_array.ndjson.gz",
+        "tests/data/gen/api_dump_array.json",
+        "tests/data/gen/api_dump_array.jsonl",
+        "tests/data/gen/api_dump_array.ndjson",
+        "tests/data/gen/api_dump_array.json.gz",
+        "tests/data/gen/api_dump_array.jsonl.gz",
+        "tests/data/gen/api_dump_array.ndjson.gz",
+        "tests/data/gen/api_dump_array.json.bz2",
+        "tests/data/gen/api_dump_array.jsonl.bz2",
+        "tests/data/gen/api_dump_array.ndjson.bz2",
     ],
 )
 def test_dump_to_file(file_name: str, snapshot, array_of_dicts: list[dict]) -> None:
     json_arrays.dump_to_file(array_of_dicts, file_name)
 
     with files.BinaryFileRead(file_name).file as fp:
         bytes_written = fp.read()
@@ -190,20 +197,23 @@
 
     assert data_written == snapshot
 
 
 @pytest.mark.parametrize(
     "file_name",
     [
-        "tests/data/gen/api_array.json",
-        "tests/data/gen/api_array.jsonl",
-        "tests/data/gen/api_array.ndjson",
-        "tests/data/gen/api_array.json.gz",
-        "tests/data/gen/api_array.jsonl.gz",
-        "tests/data/gen/api_array.ndjson.gz",
+        "tests/data/gen/api_sink_array.json",
+        "tests/data/gen/api_sink_array.jsonl",
+        "tests/data/gen/api_sink_array.ndjson",
+        "tests/data/gen/api_sink_array.json.gz",
+        "tests/data/gen/api_sink_array.jsonl.gz",
+        "tests/data/gen/api_sink_array.ndjson.gz",
+        "tests/data/gen/api_sink_array.json.bz2",
+        "tests/data/gen/api_sink_array.jsonl.bz2",
+        "tests/data/gen/api_sink_array.ndjson.bz2",
     ],
 )
 def test_sink_from_file(file_name: str, snapshot, array_of_dicts: list[dict]) -> None:
     with json_arrays.sink_from_file(file_name) as sink:
         for obj in array_of_dicts:
             sink.send(obj)
 
@@ -276,7 +286,43 @@
     with gzip.open(filename, "wt") as fp:
         json.dump(array_of_dicts, fp)
 
     with open(filename, "rb") as fp:  # type: ignore
         loaded_entries = list(json_arrays.load(fp))  # type: ignore
 
     assert loaded_entries == snapshot_json
+
+
+def test_json_bzip2_dump_fp(array_of_dicts: list[dict], snapshot_json):
+    filename = Path("tests/data/gen/json_bzip2_dump_fp.json.bz2")
+
+    with open(filename, "wb") as fp:
+        json_arrays.dump(array_of_dicts, fp)
+
+    with bz2.open(filename) as fp:  # type: ignore
+        loaded_entries = json.load(fp)
+
+    assert loaded_entries == snapshot_json
+
+
+def test_json_bzip2_load_fp(array_of_dicts: list[dict], snapshot_json):
+    filename = Path("tests/data/gen/json_bzip2_load_fp.json.bz2")
+
+    with bz2.open(filename, "wt") as fp:
+        json.dump(array_of_dicts, fp)
+
+    with open(filename, "rb") as fp:  # type: ignore
+        loaded_entries = list(json_arrays.load(fp))  # type: ignore
+
+    assert loaded_entries == snapshot_json
+
+
+def test_json_bzip2_load_fileobj(array_of_dicts: list[dict], snapshot_json):
+    filename = Path("tests/data/gen/json_bzip2_load_fileobj.json.bz2")
+
+    with bz2.open(filename, "wt") as fp:
+        json.dump(array_of_dicts, fp)
+
+    fp = bz2.BZ2File(filename, "rb")  # type: ignore
+    loaded_entries = list(json_arrays.load(fp))  # type: ignore
+
+    assert loaded_entries == snapshot_json
```

### Comparing `json_arrays-0.14.1/tests/test_jsonlib_api.py` & `json_arrays-0.15.0/tests/test_jsonlib_api.py`

 * *Files identical despite different names*

### Comparing `json_arrays-0.14.1/tests/test_utility.py` & `json_arrays-0.15.0/tests/test_utility.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,68 @@
 import pytest
-from json_arrays.utility import get_name_of_file, is_jsonl
+from json_arrays.utility import get_name_of_file, is_bzip2, is_gzip, is_jsonl
 
 
 @pytest.mark.parametrize(
     "filename",
     [
         "test.jsonl",
         "test.jl",
+        "test.ndjson",
         "test.jsonl.gz",
         "test.jl.gz",
+        "test.ndjson.gz",
+        "test.jsonl.bz2",
+        "test.jl.bz2",
+        "test.ndjson.bz2",
     ],
 )
 def test_filename_is_jsonl(filename: str):
     assert is_jsonl(filename)
 
 
 @pytest.mark.parametrize(
     "filename",
+    ["test.json.gz", "test.jsonl.gz", "test.jl.gz", "test.ndjson.gz"],
+)
+def test_filename_is_gzip(filename: str):
+    assert is_gzip(filename)
+
+
+@pytest.mark.parametrize(
+    "filename",
+    ["test.json.bz2", "test.jsonl.bz2", "test.jl.bz2", "test.ndjson.bz2"],
+)
+def test_filename_is_bzip2(filename: str):
+    assert is_bzip2(filename)
+
+
+@pytest.mark.parametrize(
+    "filename",
     [
         "test.json",
         "test.json.gz",
     ],
 )
 def test_filename_is_not_jsonl(filename: str):
     assert not is_jsonl(filename)
 
 
+@pytest.mark.parametrize(
+    "filename",
+    ["test.json", "test.jsonl", "test.jl", "test.ndjson"],
+)
+def test_filename_is_not_gzip(filename: str):
+    assert not is_gzip(filename)
+
+
+@pytest.mark.parametrize(
+    "filename",
+    ["test.json", "test.jsonl", "test.jl", "test.ndjson"],
+)
+def test_filename_is_not_bzip2(filename: str):
+    assert not is_bzip2(filename)
+
+
 @pytest.mark.parametrize("fp, expected", [(None, "")])
 def test_get_name_of_file(fp, expected):
     assert get_name_of_file(fp) == expected
```

### Comparing `json_arrays-0.14.1/tests/__snapshots__/test_json_arrays_api.ambr` & `json_arrays-0.15.0/tests/__snapshots__/test_json_arrays_api.ambr`

 * *Files 17% similar despite different names*

```diff
@@ -19,30 +19,39 @@
 # ---
 # name: test_dump_str[json]
   b'"just an ordinary\\n string"'
 # ---
 # name: test_dump_str[jsonl]
   b'"just an ordinary\\n string"\n'
 # ---
-# name: test_dump_to_file[tests/data/gen/api_array.json.gz]
+# name: test_dump_to_file[tests/data/gen/api_dump_array.json.bz2]
   b'[{"a":"a1"},{"b":["b1","b2"]},{"c":{"c1":"c11"}}]'
 # ---
-# name: test_dump_to_file[tests/data/gen/api_array.json]
+# name: test_dump_to_file[tests/data/gen/api_dump_array.json.gz]
   b'[{"a":"a1"},{"b":["b1","b2"]},{"c":{"c1":"c11"}}]'
 # ---
-# name: test_dump_to_file[tests/data/gen/api_array.jsonl.gz]
+# name: test_dump_to_file[tests/data/gen/api_dump_array.json]
+  b'[{"a":"a1"},{"b":["b1","b2"]},{"c":{"c1":"c11"}}]'
+# ---
+# name: test_dump_to_file[tests/data/gen/api_dump_array.jsonl.bz2]
+  b'{"a":"a1"}\n{"b":["b1","b2"]}\n{"c":{"c1":"c11"}}\n'
+# ---
+# name: test_dump_to_file[tests/data/gen/api_dump_array.jsonl.gz]
+  b'{"a":"a1"}\n{"b":["b1","b2"]}\n{"c":{"c1":"c11"}}\n'
+# ---
+# name: test_dump_to_file[tests/data/gen/api_dump_array.jsonl]
   b'{"a":"a1"}\n{"b":["b1","b2"]}\n{"c":{"c1":"c11"}}\n'
 # ---
-# name: test_dump_to_file[tests/data/gen/api_array.jsonl]
+# name: test_dump_to_file[tests/data/gen/api_dump_array.ndjson.bz2]
   b'{"a":"a1"}\n{"b":["b1","b2"]}\n{"c":{"c1":"c11"}}\n'
 # ---
-# name: test_dump_to_file[tests/data/gen/api_array.ndjson.gz]
+# name: test_dump_to_file[tests/data/gen/api_dump_array.ndjson.gz]
   b'{"a":"a1"}\n{"b":["b1","b2"]}\n{"c":{"c1":"c11"}}\n'
 # ---
-# name: test_dump_to_file[tests/data/gen/api_array.ndjson]
+# name: test_dump_to_file[tests/data/gen/api_dump_array.ndjson]
   b'{"a":"a1"}\n{"b":["b1","b2"]}\n{"c":{"c1":"c11"}}\n'
 # ---
 # name: test_dump_to_file_fails_without_file_name
   'You must give a FILENAME or USE_STDOUT_AS_DEFAULT=`True` or USE_STDERR_AS_DEFAULT=`True`'
 # ---
 # name: test_dump_to_file_stderr[None]
   b'{"a":"a1"}\n{"b":["b1","b2"]}\n{"c":{"c1":"c11"}}\n'
@@ -79,30 +88,39 @@
 # ---
 # name: test_sink_dict[.jsonl]
   b'{"a":"b"}\n'
 # ---
 # name: test_sink_dict[.ndjson]
   b'{"a":"b"}\n'
 # ---
-# name: test_sink_from_file[tests/data/gen/api_array.json.gz]
+# name: test_sink_from_file[tests/data/gen/api_sink_array.json.bz2]
   b'[\n{"a":"a1"},\n{"b":["b1","b2"]},\n{"c":{"c1":"c11"}}\n]'
 # ---
-# name: test_sink_from_file[tests/data/gen/api_array.json]
+# name: test_sink_from_file[tests/data/gen/api_sink_array.json.gz]
   b'[\n{"a":"a1"},\n{"b":["b1","b2"]},\n{"c":{"c1":"c11"}}\n]'
 # ---
-# name: test_sink_from_file[tests/data/gen/api_array.jsonl.gz]
+# name: test_sink_from_file[tests/data/gen/api_sink_array.json]
+  b'[\n{"a":"a1"},\n{"b":["b1","b2"]},\n{"c":{"c1":"c11"}}\n]'
+# ---
+# name: test_sink_from_file[tests/data/gen/api_sink_array.jsonl.bz2]
+  b'{"a":"a1"}\n{"b":["b1","b2"]}\n{"c":{"c1":"c11"}}\n'
+# ---
+# name: test_sink_from_file[tests/data/gen/api_sink_array.jsonl.gz]
+  b'{"a":"a1"}\n{"b":["b1","b2"]}\n{"c":{"c1":"c11"}}\n'
+# ---
+# name: test_sink_from_file[tests/data/gen/api_sink_array.jsonl]
   b'{"a":"a1"}\n{"b":["b1","b2"]}\n{"c":{"c1":"c11"}}\n'
 # ---
-# name: test_sink_from_file[tests/data/gen/api_array.jsonl]
+# name: test_sink_from_file[tests/data/gen/api_sink_array.ndjson.bz2]
   b'{"a":"a1"}\n{"b":["b1","b2"]}\n{"c":{"c1":"c11"}}\n'
 # ---
-# name: test_sink_from_file[tests/data/gen/api_array.ndjson.gz]
+# name: test_sink_from_file[tests/data/gen/api_sink_array.ndjson.gz]
   b'{"a":"a1"}\n{"b":["b1","b2"]}\n{"c":{"c1":"c11"}}\n'
 # ---
-# name: test_sink_from_file[tests/data/gen/api_array.ndjson]
+# name: test_sink_from_file[tests/data/gen/api_sink_array.ndjson]
   b'{"a":"a1"}\n{"b":["b1","b2"]}\n{"c":{"c1":"c11"}}\n'
 # ---
 # name: test_sink_from_file_fails_without_file_name
   'You must give a FILENAME or USE_STDOUT_AS_DEFAULT=`True` or USE_STDERR_AS_DEFAULT=`True`'
 # ---
 # name: test_sink_from_file_stdout[None]
   b'{"a":"a1"}\n{"b":["b1","b2"]}\n{"c":{"c1":"c11"}}\n'
```

### Comparing `json_arrays-0.14.1/tests/unit/test_filenames.py` & `json_arrays-0.15.0/tests/unit/test_filenames.py`

 * *Files identical despite different names*

### Comparing `json_arrays-0.14.1/.gitignore` & `json_arrays-0.15.0/.gitignore`

 * *Files identical despite different names*

### Comparing `json_arrays-0.14.1/README.md` & `json_arrays-0.15.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # json-arrays
 
 [![PyPI version](https://badge.fury.io/py/json-arrays.svg)](https://pypi.org/project/json-arrays/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/json-arrays)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/json-arrays)](https://pypi.org/project/json-arrays/)
 
 [![Maturity badge - level 3](https://img.shields.io/badge/Maturity-Level%203%20--%20Stable-green.svg)](https://github.com/spraakbanken/getting-started/blob/main/scorecard.md)
-[![Stage](https://img.shields.io/pypi/status/sparv-sbx-word-prediction-kb-bert)](https://pypi.org/project/sparv-sbx-word-prediction-kb-bert/)
+[![Stage](https://img.shields.io/pypi/status/json-arrays)](https://pypi.org/project/json-arrays/)
 
 [![Code Coverage](https://codecov.io/gh/spraakbanken/json-arrays-py/branch/main/graph/badge.svg)](https://codecov.io/gh/spraakbanken/json-arrays-py/)
-[![CI(check)](https://github.com/spraakbanken/json-arrays-py/workflows/check.yml/badge.svg)](https://github.com/spraakbanken/json-arrays-py/actions/check.yml)
-[![CI(release)](https://github.com/spraakbanken/json-arrays-py/workflows/release.yml/badge.svg)](https://github.com/spraakbanken/json-arrays-py/actions/release.yml)
-[![CI(scheduled)](https://github.com/spraakbanken/json-arrays-py/workflows/scheduled.yml/badge.svg)](https://github.com/spraakbanken/json-arrays-py/actions/scheduled.yml)
-[![CI(test)](https://github.com/spraakbanken/json-arrays-py/workflows/test.yml/badge.svg)](https://github.com/spraakbanken/json-arrays-py/actions/test.yml)
+
+[![CI(check)](https://github.com/spraakbanken/json-arrays-py/actions/workflows/check.yml/badge.svg)](https://github.com/spraakbanken/json-arrays-py/actions/workflows/check.yml)
+[![CI(release)](https://github.com/spraakbanken/json-arrays-py/actions/workflows/release.yml/badge.svg)](https://github.com/spraakbanken/json-arrays-py/actions/workflows/release.yml)
+[![CI(scheduled)](https://github.com/spraakbanken/json-arrays-py/actions/workflows/scheduled.yml/badge.svg)](https://github.com/spraakbanken/json-arrays-py/actions/workflows/scheduled.yml)
+[![CI(test)](https://github.com/spraakbanken/json-arrays-py/actions/workflows/test.yml/badge.svg)](https://github.com/spraakbanken/json-arrays-py/actions/workflows/test.yml)
 
 Read and write JSON lazy, especially json-arrays.
 
 Handles both the JSON format:
 
 ```json
 [
```

### Comparing `json_arrays-0.14.1/pyproject.toml` & `json_arrays-0.15.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "json-arrays"
-version = "0.14.1"
+version = "0.15.0"
 description = "Stream JSON and JSON-Lines lazily."
 authors = [
+    { name = "Språkbanken Text", email = "sb-info@svenska.gu.se" },
     { name = "Kristoffer Andersson", email = "kristoffer.andersson@gu.se" },
-    { name = "Språkbanken at Göteborgs universitet", email = "sb-info@svenska.gu.se" },
 ]
 license = { text = "MIT" }
 dependencies = ["ijson>=3.2.3"]
 readme = "README.md"
 requires-python = ">= 3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `json_arrays-0.14.1/PKG-INFO` & `json_arrays-0.15.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.3
 Name: json-arrays
-Version: 0.14.1
+Version: 0.15.0
 Summary: Stream JSON and JSON-Lines lazily.
 Project-URL: Homepage, https://github.com/spraakbanken/json-arrays-py
 Project-URL: Repository, https://github.com/spraakbanken/json-arrays-py
 Project-URL: Bug Tracker, https://github.com/spraakbanken/json-arrays-py/issues
-Author-email: Kristoffer Andersson <kristoffer.andersson@gu.se>, Språkbanken at Göteborgs universitet <sb-info@svenska.gu.se>
+Author-email: Språkbanken Text <sb-info@svenska.gu.se>, Kristoffer Andersson <kristoffer.andersson@gu.se>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.9
@@ -27,21 +27,22 @@
 # json-arrays
 
 [![PyPI version](https://badge.fury.io/py/json-arrays.svg)](https://pypi.org/project/json-arrays/)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/json-arrays)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/json-arrays)](https://pypi.org/project/json-arrays/)
 
 [![Maturity badge - level 3](https://img.shields.io/badge/Maturity-Level%203%20--%20Stable-green.svg)](https://github.com/spraakbanken/getting-started/blob/main/scorecard.md)
-[![Stage](https://img.shields.io/pypi/status/sparv-sbx-word-prediction-kb-bert)](https://pypi.org/project/sparv-sbx-word-prediction-kb-bert/)
+[![Stage](https://img.shields.io/pypi/status/json-arrays)](https://pypi.org/project/json-arrays/)
 
 [![Code Coverage](https://codecov.io/gh/spraakbanken/json-arrays-py/branch/main/graph/badge.svg)](https://codecov.io/gh/spraakbanken/json-arrays-py/)
-[![CI(check)](https://github.com/spraakbanken/json-arrays-py/workflows/check.yml/badge.svg)](https://github.com/spraakbanken/json-arrays-py/actions/check.yml)
-[![CI(release)](https://github.com/spraakbanken/json-arrays-py/workflows/release.yml/badge.svg)](https://github.com/spraakbanken/json-arrays-py/actions/release.yml)
-[![CI(scheduled)](https://github.com/spraakbanken/json-arrays-py/workflows/scheduled.yml/badge.svg)](https://github.com/spraakbanken/json-arrays-py/actions/scheduled.yml)
-[![CI(test)](https://github.com/spraakbanken/json-arrays-py/workflows/test.yml/badge.svg)](https://github.com/spraakbanken/json-arrays-py/actions/test.yml)
+
+[![CI(check)](https://github.com/spraakbanken/json-arrays-py/actions/workflows/check.yml/badge.svg)](https://github.com/spraakbanken/json-arrays-py/actions/workflows/check.yml)
+[![CI(release)](https://github.com/spraakbanken/json-arrays-py/actions/workflows/release.yml/badge.svg)](https://github.com/spraakbanken/json-arrays-py/actions/workflows/release.yml)
+[![CI(scheduled)](https://github.com/spraakbanken/json-arrays-py/actions/workflows/scheduled.yml/badge.svg)](https://github.com/spraakbanken/json-arrays-py/actions/workflows/scheduled.yml)
+[![CI(test)](https://github.com/spraakbanken/json-arrays-py/actions/workflows/test.yml/badge.svg)](https://github.com/spraakbanken/json-arrays-py/actions/workflows/test.yml)
 
 Read and write JSON lazy, especially json-arrays.
 
 Handles both the JSON format:
 
 ```json
 [
```

