# Comparing `tmp/argilla_llama_index-1.0.0.tar.gz` & `tmp/argilla_llama_index-1.0.1.tar.gz`

## Comparing `argilla_llama_index-1.0.0.tar` & `argilla_llama_index-1.0.1.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/.github/workflows/integration-tests.yml
--rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/.github/workflows/release.yml
--rw-r--r--   0        0        0    75041 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/data/paul_graham_essay.txt
--rw-r--r--   0        0        0   102735 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/docs/assets/argilla-ui-dataset.png
--rw-r--r--   0        0        0    52647 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/docs/examples/usage_example.ipynb
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/src/argilla_llama_index/__init__.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/src/argilla_llama_index/helpers.py
--rw-r--r--   0        0        0    30479 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/src/argilla_llama_index/llama_index_handler.py
--rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/tests/test_llama_index_callback.py
--rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/.gitignore
--rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/LICENSE
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/LICENSE_HEADER
--rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/README.md
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     5342 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1863 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.1/.github/workflows/integration-tests.yml
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0    75041 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.1/data/paul_graham_essay.txt
+-rw-r--r--   0        0        0   102735 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.1/docs/assets/argilla-ui-dataset.png
+-rw-r--r--   0        0        0   106518 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.1/docs/assets/rag_example_1.png
+-rw-r--r--   0        0        0    52647 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.1/docs/examples/usage_example.ipynb
+-rw-r--r--   0        0        0    13632 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.1/docs/tutorials/github_rag_llamaindex_argilla.ipynb
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.1/src/argilla_llama_index/__init__.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.1/src/argilla_llama_index/helpers.py
+-rw-r--r--   0        0        0    30479 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.1/src/argilla_llama_index/llama_index_handler.py
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.1/tests/test_llama_index_callback.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.1/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.1/LICENSE
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.1/LICENSE_HEADER
+-rw-r--r--   0        0        0     4186 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.1/README.md
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     5394 2020-02-02 00:00:00.000000 argilla_llama_index-1.0.1/PKG-INFO
```

### Comparing `argilla_llama_index-1.0.0/.github/workflows/integration-tests.yml` & `argilla_llama_index-1.0.1/.github/workflows/integration-tests.yml`

 * *Files identical despite different names*

### Comparing `argilla_llama_index-1.0.0/.github/workflows/release.yml` & `argilla_llama_index-1.0.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `argilla_llama_index-1.0.0/data/paul_graham_essay.txt` & `argilla_llama_index-1.0.1/data/paul_graham_essay.txt`

 * *Files identical despite different names*

### Comparing `argilla_llama_index-1.0.0/docs/assets/argilla-ui-dataset.png` & `argilla_llama_index-1.0.1/docs/assets/argilla-ui-dataset.png`

 * *Files identical despite different names*

### Comparing `argilla_llama_index-1.0.0/docs/examples/usage_example.ipynb` & `argilla_llama_index-1.0.1/docs/examples/usage_example.ipynb`

 * *Files identical despite different names*

### Comparing `argilla_llama_index-1.0.0/src/argilla_llama_index/__init__.py` & `argilla_llama_index-1.0.1/src/argilla_llama_index/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,12 +8,12 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.0.0"
+__version__ = "1.0.1"
 
 from argilla_llama_index.llama_index_handler import ArgillaCallbackHandler
 
 __all__ = ["ArgillaCallbackHandler"]
```

### Comparing `argilla_llama_index-1.0.0/src/argilla_llama_index/helpers.py` & `argilla_llama_index-1.0.1/src/argilla_llama_index/helpers.py`

 * *Files identical despite different names*

### Comparing `argilla_llama_index-1.0.0/src/argilla_llama_index/llama_index_handler.py` & `argilla_llama_index-1.0.1/src/argilla_llama_index/llama_index_handler.py`

 * *Files identical despite different names*

### Comparing `argilla_llama_index-1.0.0/tests/test_llama_index_callback.py` & `argilla_llama_index-1.0.1/tests/test_llama_index_callback.py`

 * *Files identical despite different names*

### Comparing `argilla_llama_index-1.0.0/.gitignore` & `argilla_llama_index-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `argilla_llama_index-1.0.0/LICENSE` & `argilla_llama_index-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `argilla_llama_index-1.0.0/LICENSE_HEADER` & `argilla_llama_index-1.0.1/LICENSE_HEADER`

 * *Files identical despite different names*

### Comparing `argilla_llama_index-1.0.0/README.md` & `argilla_llama_index-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `argilla_llama_index-1.0.0/pyproject.toml` & `argilla_llama_index-1.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,16 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "argilla >= 1.22.0",
     "llama-index >= 0.10.0",
     "packaging >= 23.2",
-    "typing-extensions >= 4.3.0"
+    "typing-extensions >= 4.3.0",
+    "llama-index-callbacks-argilla >= 0.1.4",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["black == 23.10.0", "ruff == 0.1.0", "pre-commit >= 3.5.0"]
 tests = ["pytest >= 7.4.0"]
```

### Comparing `argilla_llama_index-1.0.0/PKG-INFO` & `argilla_llama_index-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: argilla-llama-index
-Version: 1.0.0
+Version: 1.0.1
 Summary: Argilla-Llama Index Integration
 Project-URL: Documentation, https://github.com/argilla-io/argilla-llama-index
 Project-URL: Issues, https://github.com/argilla-io/argilla-llama-index/issues
 Project-URL: Source, https://github.com/argilla-io/argilla-llama-index
 Author-email: Argilla <admin@argilla.io>
 License-Expression: MIT
 License-File: LICENSE
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Requires-Dist: argilla>=1.22.0
+Requires-Dist: llama-index-callbacks-argilla>=0.1.4
 Requires-Dist: llama-index>=0.10.0
 Requires-Dist: packaging>=23.2
 Requires-Dist: typing-extensions>=4.3.0
 Provides-Extra: dev
 Requires-Dist: black==23.10.0; extra == 'dev'
 Requires-Dist: pre-commit>=3.5.0; extra == 'dev'
 Requires-Dist: ruff==0.1.0; extra == 'dev'
```

