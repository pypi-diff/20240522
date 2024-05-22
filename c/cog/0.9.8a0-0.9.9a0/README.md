# Comparing `tmp/cog-0.9.8a0-py3-none-any.whl.zip` & `tmp/cog-0.9.9a0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,111 +1,112 @@
-Zip file size: 96063 bytes, number of entries: 109
--rw-r--r--  2.0 unx       13 b- defN 24-May-10 17:11 cog/.gitignore
--rw-r--r--  2.0 unx      384 b- defN 24-May-10 17:11 cog/__init__.py
--rw-r--r--  2.0 unx      413 b- defN 24-May-10 17:12 cog/_version.py
--rw-r--r--  2.0 unx    10313 b- defN 24-May-10 17:11 cog/code_xforms.py
--rw-r--r--  2.0 unx      286 b- defN 24-May-10 17:11 cog/errors.py
--rw-r--r--  2.0 unx     2124 b- defN 24-May-10 17:11 cog/files.py
--rw-r--r--  2.0 unx     1945 b- defN 24-May-10 17:11 cog/json.py
--rw-r--r--  2.0 unx     3171 b- defN 24-May-10 17:11 cog/logging.py
--rw-r--r--  2.0 unx    17163 b- defN 24-May-10 17:11 cog/predictor.py
--rw-r--r--  2.0 unx     3308 b- defN 24-May-10 17:11 cog/schema.py
--rw-r--r--  2.0 unx      645 b- defN 24-May-10 17:11 cog/suppress_output.py
--rw-r--r--  2.0 unx     8993 b- defN 24-May-10 17:11 cog/types.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-10 17:11 cog/command/__init__.py
--rw-r--r--  2.0 unx    18782 b- defN 24-May-10 17:11 cog/command/ast_openapi_schema.py
--rw-r--r--  2.0 unx     1934 b- defN 24-May-10 17:11 cog/command/openapi_schema.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-10 17:11 cog/server/__init__.py
--rw-r--r--  2.0 unx      593 b- defN 24-May-10 17:11 cog/server/eventtypes.py
--rw-r--r--  2.0 unx      149 b- defN 24-May-10 17:11 cog/server/exceptions.py
--rw-r--r--  2.0 unx     5349 b- defN 24-May-10 17:11 cog/server/helpers.py
--rw-r--r--  2.0 unx    16945 b- defN 24-May-10 17:11 cog/server/http.py
--rw-r--r--  2.0 unx      971 b- defN 24-May-10 17:11 cog/server/probes.py
--rw-r--r--  2.0 unx      689 b- defN 24-May-10 17:11 cog/server/response_throttler.py
--rw-r--r--  2.0 unx    15515 b- defN 24-May-10 17:11 cog/server/runner.py
--rw-r--r--  2.0 unx     3326 b- defN 24-May-10 17:11 cog/server/webhook.py
--rw-r--r--  2.0 unx     8050 b- defN 24-May-10 17:11 cog/server/worker.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-10 17:11 tests/__init__.py
--rw-r--r--  2.0 unx      536 b- defN 24-May-10 17:11 tests/conftest.py
--rw-r--r--  2.0 unx     1737 b- defN 24-May-10 17:11 tests/test_json.py
--rw-r--r--  2.0 unx     1154 b- defN 24-May-10 17:11 tests/test_predictor.py
--rw-r--r--  2.0 unx     4895 b- defN 24-May-10 17:11 tests/test_types.py
--rw-r--r--  2.0 unx      113 b- defN 24-May-10 17:11 tests/fixtures/argv_override.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-10 17:11 tests/server/__init__.py
--rw-r--r--  2.0 unx     2800 b- defN 24-May-10 17:11 tests/server/conftest.py
--rw-r--r--  2.0 unx     2564 b- defN 24-May-10 17:11 tests/server/test_code_xforms.py
--rw-r--r--  2.0 unx     4692 b- defN 24-May-10 17:11 tests/server/test_helpers.py
--rw-r--r--  2.0 unx    16956 b- defN 24-May-10 17:11 tests/server/test_http.py
--rw-r--r--  2.0 unx     9181 b- defN 24-May-10 17:11 tests/server/test_http_input.py
--rw-r--r--  2.0 unx     4020 b- defN 24-May-10 17:11 tests/server/test_http_output.py
--rw-r--r--  2.0 unx     2775 b- defN 24-May-10 17:11 tests/server/test_predictor.py
--rw-r--r--  2.0 unx     1334 b- defN 24-May-10 17:11 tests/server/test_probes.py
--rw-r--r--  2.0 unx     1210 b- defN 24-May-10 17:11 tests/server/test_response_throttler.py
--rw-r--r--  2.0 unx    10931 b- defN 24-May-10 17:11 tests/server/test_runner.py
--rw-r--r--  2.0 unx     3225 b- defN 24-May-10 17:11 tests/server/test_webhook.py
--rw-r--r--  2.0 unx    16162 b- defN 24-May-10 17:11 tests/server/test_worker.py
--rw-r--r--  2.0 unx      209 b- defN 24-May-10 17:11 tests/server/fixtures/async_setup_uses_same_loop_as_predict.py
--rw-r--r--  2.0 unx      198 b- defN 24-May-10 17:11 tests/server/fixtures/catch_in_predict.py
--rw-r--r--  2.0 unx      232 b- defN 24-May-10 17:11 tests/server/fixtures/complex_output.py
--rw-r--r--  2.0 unx      131 b- defN 24-May-10 17:11 tests/server/fixtures/count_up.py
--rw-r--r--  2.0 unx      136 b- defN 24-May-10 17:11 tests/server/fixtures/exc_in_predict.py
--rw-r--r--  2.0 unx      133 b- defN 24-May-10 17:11 tests/server/fixtures/exc_in_setup.py
--rw-r--r--  2.0 unx      151 b- defN 24-May-10 17:11 tests/server/fixtures/exc_in_setup_and_predict.py
--rw-r--r--  2.0 unx       56 b- defN 24-May-10 17:11 tests/server/fixtures/exc_on_import.py
--rw-r--r--  2.0 unx      122 b- defN 24-May-10 17:11 tests/server/fixtures/exit_in_predict.py
--rw-r--r--  2.0 unx      124 b- defN 24-May-10 17:11 tests/server/fixtures/exit_in_setup.py
--rw-r--r--  2.0 unx       23 b- defN 24-May-10 17:11 tests/server/fixtures/exit_on_import.py
--rw-r--r--  2.0 unx       58 b- defN 24-May-10 17:11 tests/server/fixtures/function.py
--rw-r--r--  2.0 unx      159 b- defN 24-May-10 17:11 tests/server/fixtures/hello_world.py
--rw-r--r--  2.0 unx      197 b- defN 24-May-10 17:11 tests/server/fixtures/input_choices.py
--rw-r--r--  2.0 unx      153 b- defN 24-May-10 17:11 tests/server/fixtures/input_choices_integer.py
--rw-r--r--  2.0 unx      139 b- defN 24-May-10 17:11 tests/server/fixtures/input_file.py
--rw-r--r--  2.0 unx      160 b- defN 24-May-10 17:11 tests/server/fixtures/input_ge_le.py
--rw-r--r--  2.0 unx      126 b- defN 24-May-10 17:11 tests/server/fixtures/input_integer.py
--rw-r--r--  2.0 unx      152 b- defN 24-May-10 17:11 tests/server/fixtures/input_integer_default.py
--rw-r--r--  2.0 unx      317 b- defN 24-May-10 17:11 tests/server/fixtures/input_multiple.py
--rw-r--r--  2.0 unx      118 b- defN 24-May-10 17:11 tests/server/fixtures/input_none.py
--rw-r--r--  2.0 unx      236 b- defN 24-May-10 17:11 tests/server/fixtures/input_path.py
--rw-r--r--  2.0 unx      137 b- defN 24-May-10 17:11 tests/server/fixtures/input_path_2.py
--rw-r--r--  2.0 unx      159 b- defN 24-May-10 17:11 tests/server/fixtures/input_secret.py
--rw-r--r--  2.0 unx      125 b- defN 24-May-10 17:11 tests/server/fixtures/input_string.py
--rw-r--r--  2.0 unx      262 b- defN 24-May-10 17:11 tests/server/fixtures/input_union_integer_or_list_of_integers.py
--rw-r--r--  2.0 unx      266 b- defN 24-May-10 17:11 tests/server/fixtures/input_union_string_or_list_of_strings.py
--rw-r--r--  2.0 unx      205 b- defN 24-May-10 17:11 tests/server/fixtures/input_unsupported_type.py
--rw-r--r--  2.0 unx      122 b- defN 24-May-10 17:11 tests/server/fixtures/input_untyped.py
--rw-r--r--  2.0 unx      160 b- defN 24-May-10 17:11 tests/server/fixtures/killed_in_predict.py
--rw-r--r--  2.0 unx      882 b- defN 24-May-10 17:11 tests/server/fixtures/logging.py
--rw-r--r--  2.0 unx      109 b- defN 24-May-10 17:11 tests/server/fixtures/missing_predict.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-10 17:11 tests/server/fixtures/missing_predictor.py
--rw-r--r--  2.0 unx      482 b- defN 24-May-10 17:11 tests/server/fixtures/openapi_complex_input.py
--rw-r--r--  2.0 unx      332 b- defN 24-May-10 17:11 tests/server/fixtures/openapi_custom_output_type.py
--rw-r--r--  2.0 unx      169 b- defN 24-May-10 17:11 tests/server/fixtures/openapi_input_int_choices.py
--rw-r--r--  2.0 unx      153 b- defN 24-May-10 17:11 tests/server/fixtures/openapi_output_list.py
--rw-r--r--  2.0 unx      374 b- defN 24-May-10 17:11 tests/server/fixtures/openapi_output_type.py
--rw-r--r--  2.0 unx      161 b- defN 24-May-10 17:11 tests/server/fixtures/openapi_output_yield.py
--rw-r--r--  2.0 unx      264 b- defN 24-May-10 17:11 tests/server/fixtures/output_complex.py
--rw-r--r--  2.0 unx      148 b- defN 24-May-10 17:11 tests/server/fixtures/output_file.py
--rw-r--r--  2.0 unx      192 b- defN 24-May-10 17:11 tests/server/fixtures/output_file_named.py
--rw-r--r--  2.0 unx      257 b- defN 24-May-10 17:11 tests/server/fixtures/output_iterator_complex.py
--rw-r--r--  2.0 unx      151 b- defN 24-May-10 17:11 tests/server/fixtures/output_numpy.py
--rw-r--r--  2.0 unx      355 b- defN 24-May-10 17:11 tests/server/fixtures/output_path_image.py
--rw-r--r--  2.0 unx      323 b- defN 24-May-10 17:11 tests/server/fixtures/output_path_text.py
--rw-r--r--  2.0 unx      115 b- defN 24-May-10 17:11 tests/server/fixtures/output_wrong_type.py
--rw-r--r--  2.0 unx      175 b- defN 24-May-10 17:11 tests/server/fixtures/setup.py
--rw-r--r--  2.0 unx      262 b- defN 24-May-10 17:11 tests/server/fixtures/setup_uses_async.py
--rw-r--r--  2.0 unx      167 b- defN 24-May-10 17:11 tests/server/fixtures/setup_weights.py
--rw-r--r--  2.0 unx      118 b- defN 24-May-10 17:11 tests/server/fixtures/simple.py
--rw-r--r--  2.0 unx      193 b- defN 24-May-10 17:11 tests/server/fixtures/sleep.py
--rw-r--r--  2.0 unx      219 b- defN 24-May-10 17:11 tests/server/fixtures/slow_predict.py
--rw-r--r--  2.0 unx      122 b- defN 24-May-10 17:11 tests/server/fixtures/slow_setup.py
--rw-r--r--  2.0 unx      290 b- defN 24-May-10 17:11 tests/server/fixtures/steps.py
--rw-r--r--  2.0 unx      359 b- defN 24-May-10 17:11 tests/server/fixtures/train.py
--rw-r--r--  2.0 unx      263 b- defN 24-May-10 17:11 tests/server/fixtures/yield_concatenate_iterator.py
--rw-r--r--  2.0 unx      506 b- defN 24-May-10 17:11 tests/server/fixtures/yield_files.py
--rw-r--r--  2.0 unx      245 b- defN 24-May-10 17:11 tests/server/fixtures/yield_strings.py
--rw-r--r--  2.0 unx      339 b- defN 24-May-10 17:11 tests/server/fixtures/yield_strings_file_input.py
--rw-r--r--  2.0 unx    11347 b- defN 24-May-10 17:12 cog-0.9.8a0.dist-info/LICENSE
--rw-r--r--  2.0 unx    36706 b- defN 24-May-10 17:12 cog-0.9.8a0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-10 17:12 cog-0.9.8a0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-May-10 17:12 cog-0.9.8a0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     9639 b- defN 24-May-10 17:12 cog-0.9.8a0.dist-info/RECORD
-109 files, 275631 bytes uncompressed, 80631 bytes compressed:  70.7%
+Zip file size: 96854 bytes, number of entries: 110
+-rw-r--r--  2.0 unx       13 b- defN 24-May-20 15:22 cog/.gitignore
+-rw-r--r--  2.0 unx      384 b- defN 24-May-20 15:22 cog/__init__.py
+-rw-r--r--  2.0 unx      413 b- defN 24-May-20 15:23 cog/_version.py
+-rw-r--r--  2.0 unx    10313 b- defN 24-May-20 15:22 cog/code_xforms.py
+-rw-r--r--  2.0 unx      286 b- defN 24-May-20 15:22 cog/errors.py
+-rw-r--r--  2.0 unx     2520 b- defN 24-May-20 15:22 cog/files.py
+-rw-r--r--  2.0 unx     1945 b- defN 24-May-20 15:22 cog/json.py
+-rw-r--r--  2.0 unx     3171 b- defN 24-May-20 15:22 cog/logging.py
+-rw-r--r--  2.0 unx    17163 b- defN 24-May-20 15:22 cog/predictor.py
+-rw-r--r--  2.0 unx     3308 b- defN 24-May-20 15:22 cog/schema.py
+-rw-r--r--  2.0 unx      645 b- defN 24-May-20 15:22 cog/suppress_output.py
+-rw-r--r--  2.0 unx     8993 b- defN 24-May-20 15:22 cog/types.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 15:22 cog/command/__init__.py
+-rw-r--r--  2.0 unx    18782 b- defN 24-May-20 15:22 cog/command/ast_openapi_schema.py
+-rw-r--r--  2.0 unx     1934 b- defN 24-May-20 15:22 cog/command/openapi_schema.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 15:22 cog/server/__init__.py
+-rw-r--r--  2.0 unx      593 b- defN 24-May-20 15:22 cog/server/eventtypes.py
+-rw-r--r--  2.0 unx      149 b- defN 24-May-20 15:22 cog/server/exceptions.py
+-rw-r--r--  2.0 unx     5349 b- defN 24-May-20 15:22 cog/server/helpers.py
+-rw-r--r--  2.0 unx    16945 b- defN 24-May-20 15:22 cog/server/http.py
+-rw-r--r--  2.0 unx      971 b- defN 24-May-20 15:22 cog/server/probes.py
+-rw-r--r--  2.0 unx      689 b- defN 24-May-20 15:22 cog/server/response_throttler.py
+-rw-r--r--  2.0 unx    15648 b- defN 24-May-20 15:22 cog/server/runner.py
+-rw-r--r--  2.0 unx     3326 b- defN 24-May-20 15:22 cog/server/webhook.py
+-rw-r--r--  2.0 unx     8050 b- defN 24-May-20 15:22 cog/server/worker.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 15:22 tests/__init__.py
+-rw-r--r--  2.0 unx      536 b- defN 24-May-20 15:22 tests/conftest.py
+-rw-r--r--  2.0 unx     1737 b- defN 24-May-20 15:22 tests/test_json.py
+-rw-r--r--  2.0 unx     1154 b- defN 24-May-20 15:22 tests/test_predictor.py
+-rw-r--r--  2.0 unx     4895 b- defN 24-May-20 15:22 tests/test_types.py
+-rw-r--r--  2.0 unx     2633 b- defN 24-May-20 15:22 tests/cog/test_files.py
+-rw-r--r--  2.0 unx      113 b- defN 24-May-20 15:22 tests/fixtures/argv_override.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 15:22 tests/server/__init__.py
+-rw-r--r--  2.0 unx     2800 b- defN 24-May-20 15:22 tests/server/conftest.py
+-rw-r--r--  2.0 unx     2564 b- defN 24-May-20 15:22 tests/server/test_code_xforms.py
+-rw-r--r--  2.0 unx     4692 b- defN 24-May-20 15:22 tests/server/test_helpers.py
+-rw-r--r--  2.0 unx    16956 b- defN 24-May-20 15:22 tests/server/test_http.py
+-rw-r--r--  2.0 unx     9181 b- defN 24-May-20 15:22 tests/server/test_http_input.py
+-rw-r--r--  2.0 unx     4020 b- defN 24-May-20 15:22 tests/server/test_http_output.py
+-rw-r--r--  2.0 unx     2775 b- defN 24-May-20 15:22 tests/server/test_predictor.py
+-rw-r--r--  2.0 unx     1334 b- defN 24-May-20 15:22 tests/server/test_probes.py
+-rw-r--r--  2.0 unx     1210 b- defN 24-May-20 15:22 tests/server/test_response_throttler.py
+-rw-r--r--  2.0 unx    10931 b- defN 24-May-20 15:22 tests/server/test_runner.py
+-rw-r--r--  2.0 unx     3225 b- defN 24-May-20 15:22 tests/server/test_webhook.py
+-rw-r--r--  2.0 unx    16162 b- defN 24-May-20 15:22 tests/server/test_worker.py
+-rw-r--r--  2.0 unx      209 b- defN 24-May-20 15:22 tests/server/fixtures/async_setup_uses_same_loop_as_predict.py
+-rw-r--r--  2.0 unx      198 b- defN 24-May-20 15:22 tests/server/fixtures/catch_in_predict.py
+-rw-r--r--  2.0 unx      232 b- defN 24-May-20 15:22 tests/server/fixtures/complex_output.py
+-rw-r--r--  2.0 unx      131 b- defN 24-May-20 15:22 tests/server/fixtures/count_up.py
+-rw-r--r--  2.0 unx      136 b- defN 24-May-20 15:22 tests/server/fixtures/exc_in_predict.py
+-rw-r--r--  2.0 unx      133 b- defN 24-May-20 15:22 tests/server/fixtures/exc_in_setup.py
+-rw-r--r--  2.0 unx      151 b- defN 24-May-20 15:22 tests/server/fixtures/exc_in_setup_and_predict.py
+-rw-r--r--  2.0 unx       56 b- defN 24-May-20 15:22 tests/server/fixtures/exc_on_import.py
+-rw-r--r--  2.0 unx      122 b- defN 24-May-20 15:22 tests/server/fixtures/exit_in_predict.py
+-rw-r--r--  2.0 unx      124 b- defN 24-May-20 15:22 tests/server/fixtures/exit_in_setup.py
+-rw-r--r--  2.0 unx       23 b- defN 24-May-20 15:22 tests/server/fixtures/exit_on_import.py
+-rw-r--r--  2.0 unx       58 b- defN 24-May-20 15:22 tests/server/fixtures/function.py
+-rw-r--r--  2.0 unx      159 b- defN 24-May-20 15:22 tests/server/fixtures/hello_world.py
+-rw-r--r--  2.0 unx      197 b- defN 24-May-20 15:22 tests/server/fixtures/input_choices.py
+-rw-r--r--  2.0 unx      153 b- defN 24-May-20 15:22 tests/server/fixtures/input_choices_integer.py
+-rw-r--r--  2.0 unx      139 b- defN 24-May-20 15:22 tests/server/fixtures/input_file.py
+-rw-r--r--  2.0 unx      160 b- defN 24-May-20 15:22 tests/server/fixtures/input_ge_le.py
+-rw-r--r--  2.0 unx      126 b- defN 24-May-20 15:22 tests/server/fixtures/input_integer.py
+-rw-r--r--  2.0 unx      152 b- defN 24-May-20 15:22 tests/server/fixtures/input_integer_default.py
+-rw-r--r--  2.0 unx      317 b- defN 24-May-20 15:22 tests/server/fixtures/input_multiple.py
+-rw-r--r--  2.0 unx      118 b- defN 24-May-20 15:22 tests/server/fixtures/input_none.py
+-rw-r--r--  2.0 unx      236 b- defN 24-May-20 15:22 tests/server/fixtures/input_path.py
+-rw-r--r--  2.0 unx      137 b- defN 24-May-20 15:22 tests/server/fixtures/input_path_2.py
+-rw-r--r--  2.0 unx      159 b- defN 24-May-20 15:22 tests/server/fixtures/input_secret.py
+-rw-r--r--  2.0 unx      125 b- defN 24-May-20 15:22 tests/server/fixtures/input_string.py
+-rw-r--r--  2.0 unx      262 b- defN 24-May-20 15:22 tests/server/fixtures/input_union_integer_or_list_of_integers.py
+-rw-r--r--  2.0 unx      266 b- defN 24-May-20 15:22 tests/server/fixtures/input_union_string_or_list_of_strings.py
+-rw-r--r--  2.0 unx      205 b- defN 24-May-20 15:22 tests/server/fixtures/input_unsupported_type.py
+-rw-r--r--  2.0 unx      122 b- defN 24-May-20 15:22 tests/server/fixtures/input_untyped.py
+-rw-r--r--  2.0 unx      160 b- defN 24-May-20 15:22 tests/server/fixtures/killed_in_predict.py
+-rw-r--r--  2.0 unx      882 b- defN 24-May-20 15:22 tests/server/fixtures/logging.py
+-rw-r--r--  2.0 unx      109 b- defN 24-May-20 15:22 tests/server/fixtures/missing_predict.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-20 15:22 tests/server/fixtures/missing_predictor.py
+-rw-r--r--  2.0 unx      482 b- defN 24-May-20 15:22 tests/server/fixtures/openapi_complex_input.py
+-rw-r--r--  2.0 unx      332 b- defN 24-May-20 15:22 tests/server/fixtures/openapi_custom_output_type.py
+-rw-r--r--  2.0 unx      169 b- defN 24-May-20 15:22 tests/server/fixtures/openapi_input_int_choices.py
+-rw-r--r--  2.0 unx      153 b- defN 24-May-20 15:22 tests/server/fixtures/openapi_output_list.py
+-rw-r--r--  2.0 unx      374 b- defN 24-May-20 15:22 tests/server/fixtures/openapi_output_type.py
+-rw-r--r--  2.0 unx      161 b- defN 24-May-20 15:22 tests/server/fixtures/openapi_output_yield.py
+-rw-r--r--  2.0 unx      264 b- defN 24-May-20 15:22 tests/server/fixtures/output_complex.py
+-rw-r--r--  2.0 unx      148 b- defN 24-May-20 15:22 tests/server/fixtures/output_file.py
+-rw-r--r--  2.0 unx      192 b- defN 24-May-20 15:22 tests/server/fixtures/output_file_named.py
+-rw-r--r--  2.0 unx      257 b- defN 24-May-20 15:22 tests/server/fixtures/output_iterator_complex.py
+-rw-r--r--  2.0 unx      151 b- defN 24-May-20 15:22 tests/server/fixtures/output_numpy.py
+-rw-r--r--  2.0 unx      355 b- defN 24-May-20 15:22 tests/server/fixtures/output_path_image.py
+-rw-r--r--  2.0 unx      323 b- defN 24-May-20 15:22 tests/server/fixtures/output_path_text.py
+-rw-r--r--  2.0 unx      115 b- defN 24-May-20 15:22 tests/server/fixtures/output_wrong_type.py
+-rw-r--r--  2.0 unx      175 b- defN 24-May-20 15:22 tests/server/fixtures/setup.py
+-rw-r--r--  2.0 unx      262 b- defN 24-May-20 15:22 tests/server/fixtures/setup_uses_async.py
+-rw-r--r--  2.0 unx      167 b- defN 24-May-20 15:22 tests/server/fixtures/setup_weights.py
+-rw-r--r--  2.0 unx      118 b- defN 24-May-20 15:22 tests/server/fixtures/simple.py
+-rw-r--r--  2.0 unx      193 b- defN 24-May-20 15:22 tests/server/fixtures/sleep.py
+-rw-r--r--  2.0 unx      219 b- defN 24-May-20 15:22 tests/server/fixtures/slow_predict.py
+-rw-r--r--  2.0 unx      122 b- defN 24-May-20 15:22 tests/server/fixtures/slow_setup.py
+-rw-r--r--  2.0 unx      290 b- defN 24-May-20 15:22 tests/server/fixtures/steps.py
+-rw-r--r--  2.0 unx      359 b- defN 24-May-20 15:22 tests/server/fixtures/train.py
+-rw-r--r--  2.0 unx      263 b- defN 24-May-20 15:22 tests/server/fixtures/yield_concatenate_iterator.py
+-rw-r--r--  2.0 unx      506 b- defN 24-May-20 15:22 tests/server/fixtures/yield_files.py
+-rw-r--r--  2.0 unx      245 b- defN 24-May-20 15:22 tests/server/fixtures/yield_strings.py
+-rw-r--r--  2.0 unx      339 b- defN 24-May-20 15:22 tests/server/fixtures/yield_strings_file_input.py
+-rw-r--r--  2.0 unx    11347 b- defN 24-May-20 15:23 cog-0.9.9a0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    36706 b- defN 24-May-20 15:23 cog-0.9.9a0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-20 15:23 cog-0.9.9a0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-May-20 15:23 cog-0.9.9a0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     9719 b- defN 24-May-20 15:23 cog-0.9.9a0.dist-info/RECORD
+110 files, 278873 bytes uncompressed, 81300 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -84,14 +84,17 @@
 
 Filename: tests/test_predictor.py
 Comment: 
 
 Filename: tests/test_types.py
 Comment: 
 
+Filename: tests/cog/test_files.py
+Comment: 
+
 Filename: tests/fixtures/argv_override.py
 Comment: 
 
 Filename: tests/server/__init__.py
 Comment: 
 
 Filename: tests/server/conftest.py
@@ -306,23 +309,23 @@
 
 Filename: tests/server/fixtures/yield_strings.py
 Comment: 
 
 Filename: tests/server/fixtures/yield_strings_file_input.py
 Comment: 
 
-Filename: cog-0.9.8a0.dist-info/LICENSE
+Filename: cog-0.9.9a0.dist-info/LICENSE
 Comment: 
 
-Filename: cog-0.9.8a0.dist-info/METADATA
+Filename: cog-0.9.9a0.dist-info/METADATA
 Comment: 
 
-Filename: cog-0.9.8a0.dist-info/WHEEL
+Filename: cog-0.9.9a0.dist-info/WHEEL
 Comment: 
 
-Filename: cog-0.9.8a0.dist-info/top_level.txt
+Filename: cog-0.9.9a0.dist-info/top_level.txt
 Comment: 
 
-Filename: cog-0.9.8a0.dist-info/RECORD
+Filename: cog-0.9.9a0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cog/_version.py

```diff
@@ -8,9 +8,9 @@
     VERSION_TUPLE = object
 
 version: str
 __version__: str
 __version_tuple__: VERSION_TUPLE
 version_tuple: VERSION_TUPLE
 
-__version__ = version = '0.9.8a0'
-__version_tuple__ = version_tuple = (0, 9, 8)
+__version__ = version = '0.9.9a0'
+__version_tuple__ = version_tuple = (0, 9, 9)
```

## cog/files.py

```diff
@@ -1,11 +1,12 @@
 import base64
 import io
 import mimetypes
 import os
+from typing import Optional
 from urllib.parse import urlparse
 
 import requests
 
 
 def upload_file(fh: io.IOBase, output_file_prefix: str = None) -> str:
     fh.seek(0)
@@ -35,38 +36,48 @@
 def guess_filename(obj: io.IOBase) -> str:
     """Tries to guess the filename of the given object."""
     name = getattr(obj, "name", "file")
     return os.path.basename(name)
 
 
 def put_file_to_signed_endpoint(
-    fh: io.IOBase, endpoint: str, client: requests.Session
+    fh: io.IOBase, endpoint: str, client: requests.Session, prediction_id: Optional[str]
 ) -> str:
     fh.seek(0)
 
     filename = guess_filename(fh)
     content_type, _ = mimetypes.guess_type(filename)
 
     # set connect timeout to slightly more than a multiple of 3 to avoid
     # aligning perfectly with TCP retransmission timer
     connect_timeout = 10
     read_timeout = 15
 
+    headers = {
+        "Content-Type": content_type,
+    }
+    if prediction_id is not None:
+        headers["X-Prediction-ID"] = prediction_id
+
     resp = client.put(
         ensure_trailing_slash(endpoint) + filename,
         fh,  # type: ignore
-        headers={"Content-type": content_type},
+        headers=headers,
         timeout=(connect_timeout, read_timeout),
     )
     resp.raise_for_status()
 
-    # strip any signing gubbins from the URL
-    final_url = urlparse(resp.url)._replace(query="").geturl()
+    # Try to extract the final asset URL from the `Location` header
+    # otherwise fallback to the URL of the final request.
+    final_url = resp.url
+    if "location" in resp.headers:
+        final_url = resp.headers.get("location")
 
-    return final_url
+    # strip any signing gubbins from the URL
+    return str(urlparse(final_url)._replace(query="").geturl())
 
 
 def ensure_trailing_slash(url: str) -> str:
     """
     Adds a trailing slash to `url` if not already present, and then returns it.
     """
     if url.endswith("/"):
```

## cog/server/runner.py

```diff
@@ -189,29 +189,33 @@
 
     webhook_sender = None
     if webhook is not None:
         webhook_sender = webhook_caller_filtered(webhook, set(events_filter))
 
     file_uploader = None
     if upload_url is not None:
-        file_uploader = generate_file_uploader(upload_url)
+        file_uploader = generate_file_uploader(upload_url, prediction_id=prediction.id)
 
     event_handler = PredictionEventHandler(
         response, webhook_sender=webhook_sender, file_uploader=file_uploader
     )
 
     return event_handler
 
 
-def generate_file_uploader(upload_url: str) -> Callable[[Any], Any]:
+def generate_file_uploader(
+    upload_url: str, prediction_id: Optional[str]
+) -> Callable[[Any], Any]:
     client = _make_file_upload_http_client()
 
     def file_uploader(output: Any) -> Any:
         def upload_file(fh: io.IOBase) -> str:
-            return put_file_to_signed_endpoint(fh, upload_url, client=client)
+            return put_file_to_signed_endpoint(
+                fh, endpoint=upload_url, prediction_id=prediction_id, client=client
+            )
 
         return upload_files(output, upload_file=upload_file)
 
     return file_uploader
 
 
 class PredictionEventHandler:
```

## Comparing `cog-0.9.8a0.dist-info/LICENSE` & `cog-0.9.9a0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cog-0.9.8a0.dist-info/METADATA` & `cog-0.9.9a0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cog
-Version: 0.9.8a0
+Version: 0.9.9a0
 Summary: Containers for machine learning
 Author-email: Replicate <team@replicate.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

## Comparing `cog-0.9.8a0.dist-info/RECORD` & `cog-0.9.9a0.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 cog/.gitignore,sha256=OIzCsCr9oYv3wBtJU_TppxWi-OhuDmwCBrrUqcE6kfY,13
 cog/__init__.py,sha256=QcRZ-RsRIoasGN4JsxgKSxfhtMyWbiOCn0sjQAQimB4,384
-cog/_version.py,sha256=86viJm00gkhn-XuC4vbew1a8LT1hsIbo2Ny2AICZHkg,413
+cog/_version.py,sha256=FVAgnJGDhsRXi0NR_uWfKXkHMUDqcg_xHHmxeS0GCWE,413
 cog/code_xforms.py,sha256=ZCiXn1bN5fIoY_GU91mwNeZr7B4rmE_GXiJVcZONyaM,10313
 cog/errors.py,sha256=pB29TjzvXmyqbqi3zPOlLobFJnVWb6GJ9WsLE-77TIQ,286
-cog/files.py,sha256=8PENbdvtuVl6sbgsoZSAHId60TSM8iU-dNMpNPS9h1A,2124
+cog/files.py,sha256=Plr_c9hQK5Gzg_XxDpIj30QQbd5Rn-CL5Wch-ETcS-c,2520
 cog/json.py,sha256=xNwlgqYY7egcHZzcWs94S17q3KbtZVyaDe5gCyZG-Vo,1945
 cog/logging.py,sha256=3I7jOG1HKU5oh6-xJF1dh_qFMJMBrjo9Z60zM6sr3qU,3171
 cog/predictor.py,sha256=4L5lGT89FJAeCo0n4GzM4zy0wwFSEc-1OuokEd2J2AE,17163
 cog/schema.py,sha256=NaVXnqMQ-duhWkS8vomg2NrXhdLn9nEkFKHPnhRtb7A,3308
 cog/suppress_output.py,sha256=HHSNGR9j4rkyLL4mGnkluxzSQAYYIUcEWGdNCtYfwZc,645
 cog/types.py,sha256=aDKkuYeG55HNVo3JDzo_iFsxbznrZfEC9N1DTbi2M4U,8993
 cog/command/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -16,22 +16,23 @@
 cog/server/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 cog/server/eventtypes.py,sha256=s2iJKjiXFG_cRIS_a4VQE_wVQosoyppRqTJfevBD_XI,593
 cog/server/exceptions.py,sha256=HknokO6g7gIlbIAMBM8685gE4Xgb8lykC-gTF6SLEYM,149
 cog/server/helpers.py,sha256=Z0mRZJOonbqc7Kir3JiGSbg-0svmtJCVpp3IaET3MlM,5349
 cog/server/http.py,sha256=-xoaDzal7FV7_pAIATOM-TQZi90iEZeupw36MlPfjZY,16945
 cog/server/probes.py,sha256=QV_AaKzKM64euwiFuo0Fw8kjA6GYSzBkZ4kXy7QS7vE,971
 cog/server/response_throttler.py,sha256=sDjMj_hvJyiB4IywBB9zl-D_EcRKSK4SIT_mujORAXk,689
-cog/server/runner.py,sha256=-fXchhxcPeuXMWtKbgajuIyePSxEKF5r-pe7cNo84xQ,15515
+cog/server/runner.py,sha256=70blBq9ULdmVyb6bg_dbUWOWOMuyVaKNYnCDrj-NDt0,15648
 cog/server/webhook.py,sha256=alohqVPU8aOsPz10N77uv2eFlvGMk8RBUj37eWFzLjY,3326
 cog/server/worker.py,sha256=VybuJ3bAFdNsOcqAkhv8M2-FkSx7sr8atN_fFAx2yLc,8050
 tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/conftest.py,sha256=KbeqWWshZoqqT6aLcZGB3_zLMe1G0IQ61BhoKQU1Xro,536
 tests/test_json.py,sha256=fkrKcif7qoHoSoQNwK24267MWeO5Lwyz8EMRUUT122Q,1737
 tests/test_predictor.py,sha256=K6yc1Va8isKetQxMIyQJ6WG92HJHKI8vvxGj4sA3rDY,1154
 tests/test_types.py,sha256=yXePtMi7c1HIIpVzg8_qAIlqG4DqYDam3CToQ-a10WA,4895
+tests/cog/test_files.py,sha256=UY_rTFwKQe3JkIKZttUdHgUWI2aLw5fMjgJnYQu0tXM,2633
 tests/fixtures/argv_override.py,sha256=dGjPI-zOkXaA0PVG1n_uKTxGB7WlSuuoa8WxBz6ZGoo,113
 tests/server/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 tests/server/conftest.py,sha256=Njsjm2jgUf-4RaDMa3msxqgp0RMQIz0DZQtdP5i0sFQ,2800
 tests/server/test_code_xforms.py,sha256=3oBRcqz2UgzkBKvIIpicR0hWYpk5hTDHl6W9qVpCdYE,2564
 tests/server/test_helpers.py,sha256=XVpcv42AYwUmo1wAoR73FMdN4tOoRYkqaTjduKE_aDA,4692
 tests/server/test_http.py,sha256=3TqUNYjYkTktHE-8WskvTWQDRGWGFHSvqeuBgj6dr04,16956
 tests/server/test_http_input.py,sha256=qd9RVyj9G7EDpbYKBMMy-bXibO2k4mtzI9QcJumi0zk,9181
@@ -98,12 +99,12 @@
 tests/server/fixtures/slow_setup.py,sha256=vHIq6spLzpo-bLmgXlyazLWljQz53JamJDHcpTl_XJo,122
 tests/server/fixtures/steps.py,sha256=WbD27CUVQE8Zj_SVOtOqtleG3Y8meSJVAn-vkhpKst8,290
 tests/server/fixtures/train.py,sha256=5LmmIK9Cd7uSJIIjl-6zZkz4BRNbXCpMW5iBYRXLhKU,359
 tests/server/fixtures/yield_concatenate_iterator.py,sha256=2X582IGdiprIALwIs5e-EZO4i1eBUdM7CI4FCPf-CAo,263
 tests/server/fixtures/yield_files.py,sha256=QpIl1SOFsaakNZJlShl_XkjBGyB_MyuQgv5-J2Vm75U,506
 tests/server/fixtures/yield_strings.py,sha256=7Y9cTGZ7WE0iKlr-ZQmhkeg30mXt-fEpY9U0AQ0QMAQ,245
 tests/server/fixtures/yield_strings_file_input.py,sha256=rNxZHFXLhzqkNiG35JfcyihSA4Lx6s3bp86YRGPztX8,339
-cog-0.9.8a0.dist-info/LICENSE,sha256=DFJczlBRunZam8mzaMaTNN-4K9KyTIsXadU5_ijFpms,11347
-cog-0.9.8a0.dist-info/METADATA,sha256=wHFOKWLySzJCNDwVUE3QFVk5qrmawih_n59ELCD_glI,36706
-cog-0.9.8a0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-cog-0.9.8a0.dist-info/top_level.txt,sha256=gNf7F5ClydQZjQsWAVaX2nQwigQiONHlsrQGZrLOm5U,10
-cog-0.9.8a0.dist-info/RECORD,,
+cog-0.9.9a0.dist-info/LICENSE,sha256=DFJczlBRunZam8mzaMaTNN-4K9KyTIsXadU5_ijFpms,11347
+cog-0.9.9a0.dist-info/METADATA,sha256=zacJgvH2SIC9rLdGiPux2eUwTIRlUt4NGro7Kgwo1So,36706
+cog-0.9.9a0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+cog-0.9.9a0.dist-info/top_level.txt,sha256=gNf7F5ClydQZjQsWAVaX2nQwigQiONHlsrQGZrLOm5U,10
+cog-0.9.9a0.dist-info/RECORD,,
```

