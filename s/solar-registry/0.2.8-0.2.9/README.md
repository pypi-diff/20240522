# Comparing `tmp/solar_registry-0.2.8.tar.gz` & `tmp/solar_registry-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solar_registry-0.2.8.tar", last modified: Wed May 15 07:31:32 2024, max compression
+gzip compressed data, was "solar_registry-0.2.9.tar", last modified: Thu May 16 02:30:58 2024, max compression
```

## Comparing `solar_registry-0.2.8.tar` & `solar_registry-0.2.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0    11357 2024-05-15 07:31:06.782474 solar_registry-0.2.8/LICENSE
--rw-r--r--   0        0        0      682 2024-05-15 07:31:06.782474 solar_registry-0.2.8/README.md
--rw-r--r--   0        0        0     1240 2024-05-15 07:31:32.686683 solar_registry-0.2.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/__init__.py
--rw-r--r--   0        0        0     2150 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/cli.py
--rw-r--r--   0        0        0        0 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/commands/__init__.py
--rw-r--r--   0        0        0     4959 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/commands/meta_merger.py
--rw-r--r--   0        0        0        0 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/model/__init__.py
--rw-r--r--   0        0        0     2117 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/model/test_tool.py
--rw-r--r--   0        0        0        0 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/service/__init__.py
--rw-r--r--   0        0        0     3993 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/service/cos_sync.py
--rw-r--r--   0        0        0     2517 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/service/generator.py
--rw-r--r--   0        0        0     2628 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/service/pr_generator.py
--rw-r--r--   0        0        0      505 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/service/testtool.py
--rw-r--r--   0        0        0     2068 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/service/validator.py
--rw-r--r--   0        0        0        0 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/util/__init__.py
--rw-r--r--   0        0        0      600 2024-05-15 07:31:06.782474 solar_registry-0.2.8/src/solar_registry/util/file.py
--rw-r--r--   0        0        0        0 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/__init__.py
--rw-r--r--   0        0        0      364 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/test_cos_sync.py
--rw-r--r--   0        0        0      680 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/test_merger.py
--rw-r--r--   0        0        0      495 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/test_pr_generator.py
--rw-r--r--   0        0        0      928 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/test_testtool.py
--rw-r--r--   0        0        0      291 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/test_validator.py
--rw-r--r--   0        0        0      731 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/testdata/error_meta_file/pytest/testtool.yaml
--rw-r--r--   0        0        0      736 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/testdata/error_version_file/pytest/testtool.yaml
--rw-r--r--   0        0        0     2778 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/testdata/pytest/testtool.yaml
--rw-r--r--   0        0        0     3607 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json
--rw-r--r--   0        0        0     2942 2024-05-15 07:31:06.782474 solar_registry-0.2.8/tests/testdata/stable_index_file_check/testtools/stable.index.json
--rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 solar_registry-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-16 02:30:35.744616 solar_registry-0.2.9/LICENSE
+-rw-r--r--   0        0        0      682 2024-05-16 02:30:35.744616 solar_registry-0.2.9/README.md
+-rw-r--r--   0        0        0     1240 2024-05-16 02:30:58.312821 solar_registry-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/__init__.py
+-rw-r--r--   0        0        0     2228 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/cli.py
+-rw-r--r--   0        0        0        0 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/commands/__init__.py
+-rw-r--r--   0        0        0     4959 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/commands/meta_merger.py
+-rw-r--r--   0        0        0        0 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/model/__init__.py
+-rw-r--r--   0        0        0     2117 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/model/test_tool.py
+-rw-r--r--   0        0        0        0 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/service/__init__.py
+-rw-r--r--   0        0        0     4161 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/service/cos_sync.py
+-rw-r--r--   0        0        0     2517 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/service/generator.py
+-rw-r--r--   0        0        0     2628 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/service/pr_generator.py
+-rw-r--r--   0        0        0      505 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/service/testtool.py
+-rw-r--r--   0        0        0     2068 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/service/validator.py
+-rw-r--r--   0        0        0        0 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/util/__init__.py
+-rw-r--r--   0        0        0      600 2024-05-16 02:30:35.744616 solar_registry-0.2.9/src/solar_registry/util/file.py
+-rw-r--r--   0        0        0        0 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/__init__.py
+-rw-r--r--   0        0        0      364 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/test_cos_sync.py
+-rw-r--r--   0        0        0      680 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/test_merger.py
+-rw-r--r--   0        0        0      495 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/test_pr_generator.py
+-rw-r--r--   0        0        0      928 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/test_testtool.py
+-rw-r--r--   0        0        0      291 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/test_validator.py
+-rw-r--r--   0        0        0      731 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/testdata/error_meta_file/pytest/testtool.yaml
+-rw-r--r--   0        0        0      736 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/testdata/error_version_file/pytest/testtool.yaml
+-rw-r--r--   0        0        0     2778 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/testdata/pytest/testtool.yaml
+-rw-r--r--   0        0        0     3607 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json
+-rw-r--r--   0        0        0     2942 2024-05-16 02:30:35.744616 solar_registry-0.2.9/tests/testdata/stable_index_file_check/testtools/stable.index.json
+-rw-r--r--   0        0        0     1503 1970-01-01 00:00:00.000000 solar_registry-0.2.9/PKG-INFO
```

### Comparing `solar_registry-0.2.8/LICENSE` & `solar_registry-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.8/README.md` & `solar_registry-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.8/pyproject.toml` & `solar_registry-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "solar-registry"
-version = "0.2.8"
+version = "0.2.9"
 description = "Generate and merge meta data for testsolar test tools"
 authors = [
     { name = "asiazhang", email = "asiazhang2002@gmail.com" },
 ]
 dependencies = [
     "requests>=2.31.0",
     "pydantic>=2.7.1",
```

### Comparing `solar_registry-0.2.8/src/solar_registry/cli.py` & `solar_registry-0.2.9/src/solar_registry/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,22 +61,23 @@
     :param working_dir: 可选工作目录
     """
     validator = ToolValidator(working_dir)
     validator.validate()
 
 
 @app.command()
-def sync_cos(working_dir: Optional[str] = None) -> None:
+def sync_cos(working_dir: Optional[str] = None, force: bool = False) -> None:
     """
     同步数据到COS上
 
     :param working_dir: 可选工作目录
+    :param force: 是否强制更新COS上的文件
     """
     sync = CosSyncService(working_dir)
-    sync.sync_meta_data()
+    sync.sync_meta_data(force)
 
 
 def cli_entry() -> None:
     app()
 
 
 if __name__ == "__main__":
```

### Comparing `solar_registry-0.2.8/src/solar_registry/commands/meta_merger.py` & `solar_registry-0.2.9/src/solar_registry/commands/meta_merger.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.8/src/solar_registry/model/test_tool.py` & `solar_registry-0.2.9/src/solar_registry/model/test_tool.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.8/src/solar_registry/service/cos_sync.py` & `solar_registry-0.2.9/src/solar_registry/service/cos_sync.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,69 +27,76 @@
             CosConfig(
                 Region=os.environ["COS_REGION"],
                 SecretId=os.environ["COS_SECRET_ID"],
                 SecretKey=os.environ["COS_SECRET_KEY"],
             )
         )
 
-    def sync_meta_data(self) -> None:
+    def sync_meta_data(self, force: bool) -> None:
         for dir_path, _, filenames in os.walk(Path(self.workdir) / "testtools"):
             for filename in filenames:
                 full_path = Path(dir_path, filename)
                 logger.info(f"Syncing {full_path}")
                 relative_path = os.path.relpath(full_path, self.workdir)
                 logger.info(f"Relative path = {relative_path}")
 
                 # 上传本地文件，相同文件跳过不上传
-                self.upload_relative_file(relative_path)
+                self.upload_relative_file(relative_path, force)
 
-    def upload_relative_file(self, relative_file: str) -> None:
+    def upload_relative_file(self, relative_file: str, force: bool) -> None:
         full_path = Path(self.workdir, relative_file)
 
-        if self.cos_client.object_exists(Bucket=self.cos_bucket, Key=relative_file):
-            with tempfile.TemporaryDirectory() as temp:
-                output_path = Path(temp) / relative_file
-                output_path.parent.mkdir(parents=True, exist_ok=True)
-
-                logger.info(f"Download {relative_file} to {output_path}...")
-                self.cos_client.download_file(
-                    Bucket=self.cos_bucket,
-                    Key=relative_file,
-                    DestFilePath=str(output_path),
-                )
+        if force:
+            logger.info(f"Overwriting {relative_file}...")
+            self.upload_file_to_cos(
+                relative_file=relative_file, full_path=str(full_path)
+            )
+        else:
+            if self.cos_client.object_exists(Bucket=self.cos_bucket, Key=relative_file):
+                with tempfile.TemporaryDirectory() as temp:
+                    output_path = Path(temp) / relative_file
+                    output_path.parent.mkdir(parents=True, exist_ok=True)
 
-                logger.info("Compare MD5...")
-                if calculate_md5(full_path) == calculate_md5(output_path):
-                    logger.info(
-                        f"✨ relative_file {relative_file} not changed, skip upload"
-                    )
-                else:
-                    response = self.cos_client.upload_file(
+                    logger.info(f"Download {relative_file} to {output_path}...")
+                    self.cos_client.download_file(
                         Bucket=self.cos_bucket,
                         Key=relative_file,
-                        LocalFilePath=str(full_path),
-                        EnableMD5=True,
-                        ACL="public-read",  # 必须设置为公有读取
-                        progress_callback=None,
-                    )
-                    logger.info(
-                        f"✅ relative_file {relative_file} uploaded, ETag: {response['ETag']}"
+                        DestFilePath=str(output_path),
                     )
 
-        else:
-            logger.info(f"File {relative_file} does not exist on cos, start upload...")
-            # 文件不存在直接上传
-            with open(Path(self.workdir, relative_file), "rb") as fp:
-                response = self.cos_client.put_object(
-                    Bucket=self.cos_bucket, Key=relative_file, Body=fp
-                )
+                    logger.info("Compare MD5...")
+                    if calculate_md5(full_path) == calculate_md5(output_path):
+                        logger.info(
+                            f"✨ relative_file {relative_file} not changed, skip upload"
+                        )
+                    else:
+                        self.upload_file_to_cos(
+                            relative_file=relative_file, full_path=str(full_path)
+                        )
+            else:
                 logger.info(
-                    f'✅ File {relative_file} uploaded, ETag: {response["ETag"]}!'
+                    f"File {relative_file} does not exist on cos, start upload..."
+                )
+                self.upload_file_to_cos(
+                    relative_file=relative_file, full_path=str(full_path)
                 )
 
+    def upload_file_to_cos(self, relative_file: str, full_path: str) -> None:
+        response = self.cos_client.upload_file(
+            Bucket=self.cos_bucket,
+            Key=relative_file,
+            LocalFilePath=full_path,
+            EnableMD5=True,
+            ACL="public-read",
+            progress_callback=None,
+        )
+        logger.info(
+            f"✅ relative_file {relative_file} uploaded, ETag: {response['ETag']}"
+        )
+
 
 def calculate_md5(file_path: Path) -> str:
     """
     计算文件的 MD5 码。
 
     Args:
         file_path: 文件路径。
```

### Comparing `solar_registry-0.2.8/src/solar_registry/service/generator.py` & `solar_registry-0.2.9/src/solar_registry/service/generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.8/src/solar_registry/service/pr_generator.py` & `solar_registry-0.2.9/src/solar_registry/service/pr_generator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.8/src/solar_registry/service/validator.py` & `solar_registry-0.2.9/src/solar_registry/service/validator.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.8/src/solar_registry/util/file.py` & `solar_registry-0.2.9/src/solar_registry/util/file.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.8/tests/test_merger.py` & `solar_registry-0.2.9/tests/test_merger.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.8/tests/test_testtool.py` & `solar_registry-0.2.9/tests/test_testtool.py`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.8/tests/testdata/error_meta_file/pytest/testtool.yaml` & `solar_registry-0.2.9/tests/testdata/error_meta_file/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.8/tests/testdata/error_version_file/pytest/testtool.yaml` & `solar_registry-0.2.9/tests/testdata/error_version_file/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.8/tests/testdata/pytest/testtool.yaml` & `solar_registry-0.2.9/tests/testdata/pytest/testtool.yaml`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.8/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json` & `solar_registry-0.2.9/tests/testdata/stable_index_file_check/testtools/python/pytest/metadata.json`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.8/tests/testdata/stable_index_file_check/testtools/stable.index.json` & `solar_registry-0.2.9/tests/testdata/stable_index_file_check/testtools/stable.index.json`

 * *Files identical despite different names*

### Comparing `solar_registry-0.2.8/PKG-INFO` & `solar_registry-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: solar-registry
-Version: 0.2.8
+Version: 0.2.9
 Summary: Generate and merge meta data for testsolar test tools
 Author-Email: asiazhang <asiazhang2002@gmail.com>
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

