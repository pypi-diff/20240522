# Comparing `tmp/pytest_qaseio-1.1.1.tar.gz` & `tmp/pytest_qaseio-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_qaseio-1.1.1.tar", max compression
+gzip compressed data, was "pytest_qaseio-1.2.0.tar", max compression
```

## Comparing `pytest_qaseio-1.1.1.tar` & `pytest_qaseio-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1092 2023-04-06 07:25:14.690639 pytest_qaseio-1.1.1/LICENSE
--rw-r--r--   0        0        0     5785 2023-05-11 09:07:18.681663 pytest_qaseio-1.1.1/README.md
--rw-r--r--   0        0        0     2818 2023-09-12 03:38:03.059725 pytest_qaseio-1.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-05 13:30:54.606605 pytest_qaseio-1.1.1/pytest_qaseio/__init__.py
--rw-r--r--   0        0        0     2387 2023-04-05 13:30:53.380549 pytest_qaseio-1.1.1/pytest_qaseio/api_client.py
--rw-r--r--   0        0        0      402 2023-04-05 13:30:52.095153 pytest_qaseio-1.1.1/pytest_qaseio/constants.py
--rw-r--r--   0        0        0     8055 2023-09-12 03:34:11.520126 pytest_qaseio-1.1.1/pytest_qaseio/converter.py
--rw-r--r--   0        0        0     3140 2023-09-12 03:34:03.631109 pytest_qaseio-1.1.1/pytest_qaseio/debug_info.py
--rw-r--r--   0        0        0      295 2023-04-05 14:41:26.341327 pytest_qaseio-1.1.1/pytest_qaseio/hooks.py
--rw-r--r--   0        0        0     8975 2023-09-12 03:38:04.753478 pytest_qaseio-1.1.1/pytest_qaseio/plugin.py
--rw-r--r--   0        0        0     1419 2023-04-05 14:02:37.660306 pytest_qaseio-1.1.1/pytest_qaseio/plugin_exceptions.py
--rw-r--r--   0        0        0        0 2023-04-05 13:31:00.616603 pytest_qaseio-1.1.1/pytest_qaseio/py.typed
--rw-r--r--   0        0        0     1156 2023-04-05 13:30:57.987221 pytest_qaseio-1.1.1/pytest_qaseio/storage.py
--rw-r--r--   0        0        0     6943 1970-01-01 00:00:00.000000 pytest_qaseio-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-06 07:25:14.690639 pytest_qaseio-1.2.0/LICENSE
+-rw-r--r--   0        0        0     5785 2023-05-11 09:07:18.681663 pytest_qaseio-1.2.0/README.md
+-rw-r--r--   0        0        0     2828 2024-05-22 08:01:02.025745 pytest_qaseio-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-05 13:30:54.606605 pytest_qaseio-1.2.0/pytest_qaseio/__init__.py
+-rw-r--r--   0        0        0     2387 2024-05-22 07:49:13.893891 pytest_qaseio-1.2.0/pytest_qaseio/api_client.py
+-rw-r--r--   0        0        0      402 2023-04-05 13:30:52.095153 pytest_qaseio-1.2.0/pytest_qaseio/constants.py
+-rw-r--r--   0        0        0     8055 2024-05-22 07:49:13.894504 pytest_qaseio-1.2.0/pytest_qaseio/converter.py
+-rw-r--r--   0        0        0     3128 2024-05-22 07:49:19.391090 pytest_qaseio-1.2.0/pytest_qaseio/debug_info.py
+-rw-r--r--   0        0        0      295 2024-04-22 09:59:50.443803 pytest_qaseio-1.2.0/pytest_qaseio/hooks.py
+-rw-r--r--   0        0        0     8936 2024-05-22 07:49:19.391628 pytest_qaseio-1.2.0/pytest_qaseio/plugin.py
+-rw-r--r--   0        0        0     1386 2024-05-22 07:49:19.391889 pytest_qaseio-1.2.0/pytest_qaseio/plugin_exceptions.py
+-rw-r--r--   0        0        0        0 2023-04-05 13:31:00.616603 pytest_qaseio-1.2.0/pytest_qaseio/py.typed
+-rw-r--r--   0        0        0     1156 2024-05-22 07:49:13.896526 pytest_qaseio-1.2.0/pytest_qaseio/storage.py
+-rw-r--r--   0        0        0     6995 1970-01-01 00:00:00.000000 pytest_qaseio-1.2.0/PKG-INFO
```

### Comparing `pytest_qaseio-1.1.1/LICENSE` & `pytest_qaseio-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_qaseio-1.1.1/README.md` & `pytest_qaseio-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_qaseio-1.1.1/pyproject.toml` & `pytest_qaseio-1.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pytest-qaseio"
 description = "Pytest plugin for Qase.io integration"
-version = "1.1.1"
+version = "1.2.0"
 license = "MIT"
 
 authors = [
   "Saritasa <pypi@saritasa.com>",
 ]
 
 readme = "README.md"
@@ -32,22 +32,22 @@
 ]
 
 [tool.poetry.plugins."pytest11"]
 pytest_qaseio = "pytest_qaseio.plugin"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-qaseio = "^3.2.1"
-selenium = "^4.8.3"
-arrow = "^1.2.3"
-filelock = "^3.10.7"
-pytest = "^7.2.2"
+qaseio = "^3.4.1"
+selenium = "^4.21.0"
+arrow = "^1.3.0"
+filelock = "^3.14.0"
+pytest = ">=7.2.2,<9.0.0"
 
 [tool.poetry.group.test.dependencies]
-mypy = "^1.1.1"
+mypy = "^1.10.0"
 safety = "^2.3.5"
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
```

### Comparing `pytest_qaseio-1.1.1/pytest_qaseio/api_client.py` & `pytest_qaseio-1.2.0/pytest_qaseio/api_client.py`

 * *Files identical despite different names*

### Comparing `pytest_qaseio-1.1.1/pytest_qaseio/converter.py` & `pytest_qaseio-1.2.0/pytest_qaseio/converter.py`

 * *Files identical despite different names*

### Comparing `pytest_qaseio-1.1.1/pytest_qaseio/debug_info.py` & `pytest_qaseio-1.2.0/pytest_qaseio/debug_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,32 +61,32 @@
         file_storage: storage.FileStorage,
         folder: str,
     ) -> str:
         try:
             screenshot_url = file_storage.save_file_obj(
                 content=self.screenshot, filename=f"{folder}/screenshot.png",
             )
-        except BaseException:
+        except Exception:
             self.logger.error(msg="Can't save screenshot to storage", exc_info=True)
             screenshot_url = ""
 
         try:
             html_url = file_storage.save_file_obj(
                 content=self.html, filename=f"{folder}/html.html",
             )
-        except BaseException:
+        except Exception:
             self.logger.error(msg="Can't save HTML to storage", exc_info=True)
             html_url = ""
 
         try:
             browser_log_url = file_storage.save_file_obj(
                 content=self.browser_log.encode("utf-8"),
                 filename=f"{folder}/browser_log.txt",
             )
-        except BaseException:
+        except Exception:
             self.logger.error(msg="Can't save browser log to storage", exc_info=True)
             browser_log_url = ""
 
         return constants.FAILED_TEST_REPORT_TEMPLATE.format(
             url=self.url,
             screenshot_url=screenshot_url,
             html_url=html_url,
```

### Comparing `pytest_qaseio-1.1.1/pytest_qaseio/plugin.py` & `pytest_qaseio-1.2.0/pytest_qaseio/plugin.py`

 * *Files 9% similar despite different names*

```diff
@@ -135,20 +135,20 @@
 
         # Mapping of pytest items ids and case id
         self._tests: dict[str, int | None] = dict()
         # Mapping of case ids and result hash from qase with status
         self._qase_results: dict[str, tuple[str, models.ResultCreate]] = dict()
 
     def pytest_sessionstart(self, session: pytest.Session):
-        """Remove lock files."""
+        """Clear previously saved run, prepare lock file."""
         if hasattr(session.config, "workerinput"):
             # Do nothing if it is not master thread
             return
         self.__run_file.unlink(missing_ok=True)
-        self.__run_file_lock.unlink(missing_ok=True)
+        self.__run_file_lock.touch(exist_ok=True)
 
     @pytest.hookimpl(trylast=True)
     def pytest_collection_modifyitems(
         self,
         items: list[pytest.Function],
     ):
         """Create test run in qase."""
@@ -179,15 +179,15 @@
                 self._current_run = self._load_run_from_file()
                 if self._current_run:
                     return
 
                 self._current_run = self._client.create_run(
                     run_data=run_data,
                 )
-                with open(self.__run_file, "w") as lock_file:
+                with pathlib.Path(self.__run_file).open(mode="w") as lock_file:
                     lock_file.write(str(self._current_run.id))
             except plugin_exceptions.BaseQasePluginException as e:
                 pytest.exit(e.message)
 
     @pytest.hookimpl(tryfirst=True, hookwrapper=True)
     def pytest_runtest_makereport(self, item: pytest.Function):
         """Represent standard pytest hook on test completion.
@@ -238,15 +238,12 @@
 
     def _load_run_from_file(
         self,
     ) -> models.Run | None:
         """Load run id and then load it from qase."""
         if not self.__run_file.exists():
             return None
-        with open(self.__run_file, "r") as lock_file:
-            try:
-                run_id = int(lock_file.read())
-                return self._client.get_run(
-                    run_id=run_id,
-                )
-            except ValueError:
-                return None
+        with pathlib.Path(self.__run_file).open() as lock_file:
+            run_id = int(lock_file.read())
+            return self._client.get_run(
+                run_id=run_id,
+            )
```

### Comparing `pytest_qaseio-1.1.1/pytest_qaseio/plugin_exceptions.py` & `pytest_qaseio-1.2.0/pytest_qaseio/plugin_exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 class BaseQasePluginException(Exception):
     """Represent BaseQasePlugin exception."""
 
     message: str = ""
 
-    def __init__(self, message: str = "", *args: object) -> None:
+    def __init__(self, *args, message: str = "") -> None:
         super().__init__(*args)
         if message:
             self.message = message
 
 
 class InvalidCaseId(BaseQasePluginException):
     """Exception that signifies that incorrect case was set for test."""
 
     message = "Tests have incorrect cases ids. Please check logs"
 
 
 class DuplicatingCaseId(BaseQasePluginException):
     """Exception that signifies that incorrect case was set for test."""
 
-    def __init__(self, duplicating_ids: list[int], *args: object) -> None:
+    def __init__(self, duplicating_ids: list[int], *args) -> None:
         ids = ", ".join(str(i) for i in duplicating_ids)
         super().__init__(
+            *args,
             message=f"Duplicating qase IDs found: {ids}",
-            *args,   # type: ignore
         )
 
 
 class MultipleIDsForTest(BaseQasePluginException):
     """Exception that signifies that single test marked with multiple IDs.
 
     Each test should be associated with exactly 1 case from qase.io for
```

### Comparing `pytest_qaseio-1.1.1/pytest_qaseio/storage.py` & `pytest_qaseio-1.2.0/pytest_qaseio/storage.py`

 * *Files identical despite different names*

### Comparing `pytest_qaseio-1.1.1/PKG-INFO` & `pytest_qaseio-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-qaseio
-Version: 1.1.1
+Version: 1.2.0
 Summary: Pytest plugin for Qase.io integration
 Home-page: https://pypi.org/project/pytest-qaseio/
 License: MIT
 Keywords: pytest,qase,qaseio,selenium,autotests
 Author: Saritasa
 Author-email: pypi@saritasa.com
 Requires-Python: >=3.10,<4.0
@@ -12,22 +12,23 @@
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Bug Tracking
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: arrow (>=1.2.3,<2.0.0)
-Requires-Dist: filelock (>=3.10.7,<4.0.0)
-Requires-Dist: pytest (>=7.2.2,<8.0.0)
-Requires-Dist: qaseio (>=3.2.1,<4.0.0)
-Requires-Dist: selenium (>=4.8.3,<5.0.0)
+Requires-Dist: arrow (>=1.3.0,<2.0.0)
+Requires-Dist: filelock (>=3.14.0,<4.0.0)
+Requires-Dist: pytest (>=7.2.2,<9.0.0)
+Requires-Dist: qaseio (>=3.4.1,<4.0.0)
+Requires-Dist: selenium (>=4.21.0,<5.0.0)
 Project-URL: Repository, https://github.com/saritasa-nest/pytest-qaseio
 Description-Content-Type: text/markdown
 
 # pytest-qaseio
 
 [![Build Status](https://github.com/saritasa-nest/pytest-qaseio/workflows/checks/badge.svg?branch=main&event=push)](https://github.com/saritasa-nest/pytest-qaseio/actions?query=workflow%3Achecks)
 [![Python Version](https://img.shields.io/pypi/pyversions/pytest-qaseio.svg)](https://pypi.org/project/pytest-qaseio/)
```

