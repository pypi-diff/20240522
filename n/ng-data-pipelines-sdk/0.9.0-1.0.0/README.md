# Comparing `tmp/ng_data_pipelines_sdk-0.9.0.tar.gz` & `tmp/ng_data_pipelines_sdk-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ng_data_pipelines_sdk-0.9.0.tar", max compression
+gzip compressed data, was "ng_data_pipelines_sdk-1.0.0.tar", max compression
```

## Comparing `ng_data_pipelines_sdk-0.9.0.tar` & `ng_data_pipelines_sdk-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      106 2024-05-21 19:44:39.302205 ng_data_pipelines_sdk-0.9.0/README.md
--rw-r--r--   0        0        0        0 2024-05-21 19:44:39.339205 ng_data_pipelines_sdk-0.9.0/ng_data_pipelines_sdk/__init__.py
--rw-r--r--   0        0        0     9155 2024-05-21 19:44:39.303205 ng_data_pipelines_sdk-0.9.0/ng_data_pipelines_sdk/aws_interface.py
--rw-r--r--   0        0        0      231 2024-05-21 19:44:39.303205 ng_data_pipelines_sdk-0.9.0/ng_data_pipelines_sdk/custom_logger.py
--rw-r--r--   0        0        0    28082 2024-05-21 19:44:39.303205 ng_data_pipelines_sdk-0.9.0/ng_data_pipelines_sdk/dataframe_manager.py
--rw-r--r--   0        0        0    16243 2024-05-21 19:44:39.303205 ng_data_pipelines_sdk-0.9.0/ng_data_pipelines_sdk/interfaces.py
--rw-r--r--   0        0        0     5093 2024-05-21 19:44:39.303205 ng_data_pipelines_sdk-0.9.0/ng_data_pipelines_sdk/spark_manager.py
--rw-r--r--   0        0        0     1453 2024-05-21 19:44:39.303205 ng_data_pipelines_sdk-0.9.0/ng_data_pipelines_sdk/utils.py
--rw-r--r--   0        0        0      695 2024-05-21 19:44:39.307205 ng_data_pipelines_sdk-0.9.0/pyproject.toml
--rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0      106 2024-05-22 20:58:59.906701 ng_data_pipelines_sdk-1.0.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-22 20:58:59.939702 ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/__init__.py
+-rw-r--r--   0        0        0     9155 2024-05-22 20:58:59.906701 ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/aws_interface.py
+-rw-r--r--   0        0        0      231 2024-05-22 20:58:59.906701 ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/custom_logger.py
+-rw-r--r--   0        0        0    26078 2024-05-22 20:58:59.906701 ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/dataframe_manager.py
+-rw-r--r--   0        0        0    19492 2024-05-22 20:58:59.906701 ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/interfaces.py
+-rw-r--r--   0        0        0     5406 2024-05-22 20:58:59.906701 ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/spark_manager.py
+-rw-r--r--   0        0        0     4780 2024-05-22 20:58:59.906701 ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/utils.py
+-rw-r--r--   0        0        0      838 2024-05-22 20:58:59.910702 ng_data_pipelines_sdk-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      884 1970-01-01 00:00:00.000000 ng_data_pipelines_sdk-1.0.0/PKG-INFO
```

### Comparing `ng_data_pipelines_sdk-0.9.0/ng_data_pipelines_sdk/aws_interface.py` & `ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/aws_interface.py`

 * *Files identical despite different names*

### Comparing `ng_data_pipelines_sdk-0.9.0/ng_data_pipelines_sdk/dataframe_manager.py` & `ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/dataframe_manager.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import json
 from datetime import datetime, timedelta
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, Optional, Union
 
 from pyspark.sql import DataFrame
 from pyspark.sql.functions import lit
 from pyspark.sql.types import StructType
 
 from ng_data_pipelines_sdk.aws_interface import AWSInterface
+from ng_data_pipelines_sdk.custom_logger import logger
 from ng_data_pipelines_sdk.interfaces import (
     DATE_FORMATTER,
-    DataFrameReadWriteParams,
+    DataFrameDict,
+    EmptyDataFrameException,
     FileType,
     FnKind,
     InputDataFrameParams,
     InputDataFrameParamsDict,
     OutputDataFrameParams,
     OutputDataFrameParamsDict,
-    ReadPreviousDayException,
     S3BucketParams,
-    S3ReadJsonParams,
+    S3ReadSchemaParams,
     StepParams,
     StepParamsDict,
     TransformParams,
     TransformParamsDict,
-    DataFrameDict,
 )
-from ng_data_pipelines_sdk.custom_logger import logger
 from ng_data_pipelines_sdk.spark_manager import SparkManager
 from ng_data_pipelines_sdk.utils import (
+    generate_date_paths,
     handle_pyspark_timestamp_in_schema,
 )
 
 logger.setLevel("INFO")
 
 
 class DataFrameManager:
@@ -57,77 +57,43 @@
         self.spark_manager = spark_manager
         self.completed_steps = []
         logger.info("DataFrameManager initialized.")
 
     def _get_bucket_url(self, bucket_params: S3BucketParams) -> str:
         return f"{self.file_system}://{bucket_params.bucket_name}"
 
-    def _get_processing_date_partition_path(
-        self, processing_date, processing_date_partitions
-    ) -> Union[str, List[str]]:
-        if processing_date_partitions is None:
-            return ""
-
-        if not isinstance(processing_date, datetime):
-            raise ValueError(
-                f"processing_date must be a datetime object to calculate partition path. Received: '{processing_date}'"
-            )
-
-        partition_path_segments = [
-            f"{date_part.value}={DATE_FORMATTER[date_part.value.replace('part_', '')](processing_date)}"
-            for date_part in processing_date_partitions
-        ]
-
-        processing_date_partition_path = "/".join(partition_path_segments)
-
-        return processing_date_partition_path
-
-    def _get_dataframe_path_with_date_partitions(
-        self, df_params: DataFrameReadWriteParams
-    ) -> Union[str, List[str]]:
-        if isinstance(df_params.processing_date, list):
-            return [
-                f"{df_params.path_to_dataframe_root}/{self._get_processing_date_partition_path(processing_date, df_params.processing_date_partitions)}"
-                for processing_date in df_params.processing_date
-            ]
-        else:
-            return f"{df_params.path_to_dataframe_root}/{self._get_processing_date_partition_path(df_params.processing_date, df_params.processing_date_partitions)}"
-
     def convert_schema_object_to_pyspark_schema(
         self, schema_object: Dict[str, Any]
     ) -> StructType:
         logger.debug("Converting schema object to PySpark StructType...")
         pyspark_schema = StructType.fromJson(schema_object)
         pyspark_schema = handle_pyspark_timestamp_in_schema(pyspark_schema)
         logger.debug(f"Schema converted sucessfully: {pyspark_schema}")
 
         return pyspark_schema
 
     def retrieve_schema_from_s3(
-        self, s3_read_schema_params: S3ReadJsonParams
+        self, s3_read_schema_params: S3ReadSchemaParams
     ) -> StructType:
         """
         Retrieve the schema for the data from an AWS S3 bucket.
 
         Returns:
             pyspark.sql.types.StructType: The retrieved schema.
 
         Raises:
             ValueError: If there is an issue retrieving or handling the schema.
         """
 
         if s3_read_schema_params is None:
-            raise ValueError(
-                "s3_schema_path_params must be provided"
-            )
+            raise ValueError("s3_schema_path_params must be provided")
 
         if s3_read_schema_params.bucket_params.bucket_name is None:
             raise ValueError("bucket_name must be provided")
 
-
         bucket_name = s3_read_schema_params.bucket_params.bucket_name
         path_to_file = s3_read_schema_params.path
         full_s3_file_path = f"{self.file_system}://{bucket_name}/{path_to_file}"
 
         logger.debug(f"Retrieving schema from path '{full_s3_file_path}'...")
         try:
             # Retrieve the schema object from AWS S3
@@ -153,242 +119,254 @@
         except Exception as e:
             error_message = (
                 f"Error retrieving or handling schema from {full_s3_file_path}: {e}"
             )
             logger.error(error_message)
             raise ValueError(error_message)
 
-    def read_dataframe(self, df_params: InputDataFrameParams) -> DataFrame:
+    def read_dataframe(
+        self,
+        input_df_params: InputDataFrameParams,
+        cache: bool = False,
+        verbose: bool = True,
+    ) -> DataFrame:
         """
         Reads a DataFrame from a specified location.
 
         Args:
             df_params (InputDataFrameParams): The parameters for reading the DataFrame.
 
         Returns:
             DataFrame: The read DataFrame.
 
         """
-        read_params = df_params.df_params
-        bucket_url = self._get_bucket_url(read_params.bucket_params)
-        if read_params.specific_path:
-            if isinstance(read_params.specific_path, list):
-                path = [f"{bucket_url}/{path}" for path in read_params.specific_path]
-            else:
-                path = f"{bucket_url}/{read_params.specific_path}"
-        else:
-            if isinstance(read_params.processing_date, list):
-                path = [
-                    f"{bucket_url}/{path_with_date_partitions}"
-                    for path_with_date_partitions in self._get_dataframe_path_with_date_partitions(
-                        read_params
-                    )
+        bucket_url = self._get_bucket_url(input_df_params.dataframe_bucket_params)
+        if input_df_params.dataframe_specific_paths:
+            if isinstance(input_df_params.dataframe_specific_paths, list):
+                paths = [
+                    f"{bucket_url}/{path}"
+                    for path in input_df_params.dataframe_specific_paths
                 ]
             else:
-                path = f"{bucket_url}/{self._get_dataframe_path_with_date_partitions(read_params)}"
+                paths = f"{bucket_url}/{input_df_params.dataframe_specific_paths}"
+        elif input_df_params.read_date_params:
+            paths = generate_date_paths(
+                base_path=f"{bucket_url}/{input_df_params.dataframe_base_path}",
+                dates=input_df_params.read_date_params.read_dates,
+            )
+        else:
+            paths = f"{bucket_url}/{input_df_params.dataframe_base_path}"
 
-        if df_params.pyspark_schema_struct:
+        if input_df_params.pyspark_schema_struct:
             schema = self.convert_schema_object_to_pyspark_schema(
-                schema_object=df_params.pyspark_schema_struct
+                schema_object=input_df_params.pyspark_schema_struct
             )
-        elif df_params.s3_schema_path_params:
-            schema = self.retrieve_schema_from_s3(df_params.s3_schema_path_params)
+        elif input_df_params.s3_schema_path_params:
+            schema = self.retrieve_schema_from_s3(input_df_params.s3_schema_path_params)
         else:
             schema = None
 
-        logger.info(f"Reading DataFrame from {path}...")
+        if verbose:
+            logger.info("Starting read operation.")
 
-        if df_params.df_params.is_previous_date:
-            logger.info("Previous date flag is set. Attempting to read DataFrame from previous date.")
-            try:
-                df = self.spark_manager.read(
-                    env=read_params.bucket_params.env,
-                    path=path,
-                    file_type=df_params.df_params.file_type,
-                    schema=schema,
-                )
-            except Exception as e:
-                logger.error(f"Error reading DataFrame from previous date: {e}.")
-                raise ReadPreviousDayException
-        else:
-            df = self.spark_manager.read(
-                env=read_params.bucket_params.env,
-                path=path,
-                file_type=df_params.df_params.file_type,
-                schema=schema,
-            )
+        df = self.spark_manager.read(
+            env=input_df_params.dataframe_bucket_params.env,
+            paths=paths,
+            file_type=input_df_params.dataframe_file_type,
+            base_path=f"{bucket_url}/{input_df_params.dataframe_base_path}",
+            schema=schema,
+            cache=cache,
+        )
+
+        if verbose:
+            logger.info("Read operation completed successfully.\n")
+
+        if df is None:
+            raise EmptyDataFrameException
 
         return df
 
     def write_schema(
-        self, df: DataFrame, write_params: DataFrameReadWriteParams
+        self, df: DataFrame, output_df_params: OutputDataFrameParams
     ) -> None:
         """
         Write the schema of the DataFrame to the specified location.
 
         Parameters:
         - df (DataFrame): The DataFrame whose schema is to be written.
 
         Raises:
         - ValueError: If there is an issue with writing the schema object to AWS S3.
         """
         pyspark_schema_json = df.schema.jsonValue()
 
-        if write_params.bucket_params.bucket_name is None:
+        if output_df_params.dataframe_bucket_params.bucket_name is None:
             raise ValueError("bucket_name must be provided to write schema to S3")
 
-        if write_params.specific_path:
-            if isinstance(write_params.specific_path, list):
+        if output_df_params.dataframe_specific_path:
+            if isinstance(output_df_params.dataframe_specific_path, list):
                 raise ValueError(
                     "Specific path is set as a list. Only a single path is allowed for writing the schema."
                 )
             logger.warning(
                 "Specific path is set for writing the schema. Schema will be written to the same path."
             )
-            path_to_schema = write_params.specific_path
+            path_to_schema = output_df_params.dataframe_specific_path
         else:
-            if write_params.path_to_dataframe_root is None:
+            if output_df_params.dataframe_base_path is None:
                 raise ValueError(
-                    "Neither 'specific_path' nor 'path_to_dataframe_root' is set for writing the schema."
+                    "Neither 'specific_path' nor 'dataframe_base_path' is set for writing the schema."
                 )
 
-            parent_folder_of_dataframe_root = "/".join(
-                write_params.path_to_dataframe_root.split("/")[:-1]
+            parent_folder_of_dataframe_base_path = "/".join(
+                output_df_params.dataframe_base_path.split("/")[:-1]
             )
-            path_to_schema = f"{parent_folder_of_dataframe_root}/schema.json"
+            path_to_schema = f"{parent_folder_of_dataframe_base_path}/schema.json"
 
         try:
             self.aws_interface.put_object_aws(
-                env=write_params.bucket_params.env,
-                bucket_name=write_params.bucket_params.bucket_name,
+                env=output_df_params.dataframe_bucket_params.env,
+                bucket_name=output_df_params.dataframe_bucket_params.bucket_name,
                 object_name=path_to_schema,
                 object_data=pyspark_schema_json,
             )
         except Exception as e:
             raise ValueError(
-                f"Error writing schema to {write_params.bucket_params.bucket_name}/{path_to_schema}: {e}"
+                f"Error writing schema to {output_df_params.dataframe_bucket_params.bucket_name}/{path_to_schema}: {e}"
             )
 
-    def _get_partitions(self, write_params: DataFrameReadWriteParams) -> List[str]:
-        date_partition_columns: List[str] = []
-        if write_params.processing_date_partitions:
-            for date_partition in write_params.processing_date_partitions:
-                date_partition_columns.append(date_partition.value)
-
-        # Choose the order of adding partitions based on the `date_partition_first` flag
-        primary_partitions = (
-            date_partition_columns
-            if write_params.processing_date_partitions_first
-            else write_params.column_partitions
-        )
-        secondary_partitions = (
-            write_params.column_partitions
-            if write_params.processing_date_partitions_first
-            else date_partition_columns
-        )
-
-        partitions: List[str] = []
-        if primary_partitions:
-            partitions.extend(primary_partitions)
-        if secondary_partitions:
-            partitions.extend(secondary_partitions)
+    def _write_dataframe_specific_path(
+        self, df: DataFrame, output_df_params: OutputDataFrameParams
+    ) -> None:
+        bucket_url = self._get_bucket_url(output_df_params.dataframe_bucket_params)
+        write_path_url = f"{bucket_url}/{output_df_params.dataframe_specific_path}"
 
-        return partitions
+        if output_df_params.overwrite:
+            logger.info(
+                f"Overwrite is set to True. Deleting existing objects under path {write_path_url}"
+            )
+            try:
+                self.aws_interface.delete_objects_aws(
+                    env=output_df_params.dataframe_bucket_params.env,
+                    bucket_name=output_df_params.dataframe_bucket_params.bucket_name,
+                    path=output_df_params.dataframe_specific_path,
+                )
+            except Exception as e:
+                raise ValueError(f"Error deleting dataframe objects: {e}")
 
-    def write_dataframe_specific_path(
-        self, df: DataFrame, df_params: OutputDataFrameParams
-    ) -> None:
-        write_params = df_params.df_params
-        bucket_url = self._get_bucket_url(write_params.bucket_params)
-        write_path_url = f"{bucket_url}/{write_params.path_to_dataframe_root}"
+            logger.info("Objects deleted successfully.")
 
         logger.info(f"Writing DataFrame to path: {write_path_url}...")
         self.spark_manager.write(
-            env=write_params.bucket_params.env,
+            env=output_df_params.dataframe_bucket_params.env,
             df=df,
             path=write_path_url,
-            file_type=df_params.df_params.file_type,
+            file_type=output_df_params.dataframe_file_type,
             partitions=None,
         )
 
-        if (
-            df_params.write_schema_on_s3
-            or df_params.df_params.file_type != FileType.PARQUET
-        ):
-            self.write_schema(df, write_params)
-
-        logger.info("Dataframe written successfully.\n")
-
-    def write_dataframe(self, df: DataFrame, df_params: OutputDataFrameParams) -> None:
+    def _write_dataframe_base_path(
+        self,
+        df: DataFrame,
+        output_df_params: OutputDataFrameParams,
+    ) -> None:
         """
         Writes a DataFrame to a specified location with optional date partitions.
 
         Args:
             df (DataFrame): The DataFrame to be written.
             df_params (OutputDataFrameParams): The parameters for writing the DataFrame.
 
         Returns:
             None
         """
-        write_params = df_params.df_params
-
-        bucket_url = self._get_bucket_url(write_params.bucket_params)
-        write_path_url = f"{bucket_url}/{write_params.path_to_dataframe_root}"
-        logger.debug(f"Write root path: {write_path_url}")
-
-        partitions = self._get_partitions(write_params)
-        logger.debug(f"Using partitions: {partitions}")
-
-
-        path = f"{self._get_dataframe_path_with_date_partitions(write_params)}"
-        full_path = f"{bucket_url}/{path}"
+        bucket_url = self._get_bucket_url(output_df_params.dataframe_bucket_params)
+        write_base_path_url = f"{bucket_url}/{output_df_params.dataframe_base_path}"
+        logger.debug(f"Write base path: {write_base_path_url}")
+
+        df_to_write = df
+        if output_df_params.single_write_date:
+            # Add the date partitions columns to the DataFrame
+            date_partition_path = ""
+            for (
+                date_partition,
+                date_partition_name,
+            ) in (
+                output_df_params.single_write_date.single_write_date_partitions.items()
+            ):
+                date_partition_path += f"{date_partition_name}={date_partition.value}/"
 
-        # Add the date partitions columns to the DataFrame
-        df_with_date_partitions = df
-        if write_params.processing_date_partitions:
-            for date_partition in write_params.processing_date_partitions:
-                formatted_date_part_value = DATE_FORMATTER[
-                    date_partition.value.replace("part_", "")
-                ](write_params.processing_date)
+                formatted_date_part_value = DATE_FORMATTER[date_partition.value](
+                    output_df_params.single_write_date.single_write_date
+                )
 
-                df_with_date_partitions = df_with_date_partitions.withColumn(
-                    date_partition.value, lit(formatted_date_part_value)
+                df_to_write = df_to_write.withColumn(
+                    date_partition_name, lit(formatted_date_part_value)
                 )
 
-        if df_params.overwrite:
-            logger.info(
-                f"Overwrite is set to True. Deleting existing objects under path {full_path}"
-            )
-            try:
-                self.aws_interface.delete_objects_aws(
-                    write_params.bucket_params.env,
-                    write_params.bucket_params.bucket_name,
-                    path,
+            if output_df_params.overwrite:
+                full_path = f"{write_base_path_url}/{date_partition_path}"
+                logger.info(
+                    f"Overwrite is set to True. Deleting existing objects under path {full_path}"
                 )
-            except Exception as e:
-                raise ValueError(f"Error deleting dataframe objects: {e}")
+                try:
+                    self.aws_interface.delete_objects_aws(
+                        env=output_df_params.dataframe_bucket_params.env,
+                        bucket_name=output_df_params.dataframe_bucket_params.bucket_name,
+                        path=f"{output_df_params.dataframe_base_path}/{date_partition_path}",
+                    )
+                except Exception as e:
+                    raise ValueError(f"Error deleting dataframe objects: {e}")
 
-            logger.info("Objects deleted successfully.")
+                logger.info("Objects deleted successfully.")
 
         logger.info(
-            f"Writing DataFrame to {write_path_url} with partitions {partitions}..."
+            f"Writing DataFrame to base path {write_base_path_url} with partitions {output_df_params.partition_by}..."
         )
         self.spark_manager.write(
-            env=write_params.bucket_params.env,
-            df=df_with_date_partitions,
-            path=write_path_url,
-            file_type=df_params.df_params.file_type,
-            partitions=partitions if partitions else None,
+            env=output_df_params.dataframe_bucket_params.env,
+            df=df_to_write,
+            path=write_base_path_url,
+            file_type=output_df_params.dataframe_file_type,
+            partitions=output_df_params.partition_by,
         )
 
         if (
-            df_params.write_schema_on_s3
-            or df_params.df_params.file_type != FileType.PARQUET
+            output_df_params.write_schema_on_s3
+            or output_df_params.dataframe_file_type != FileType.PARQUET
         ):
-            self.write_schema(df, write_params)
+            self.write_schema(df, output_df_params)
+
+        logger.info("Dataframe written successfully.\n")
+
+    def write_dataframe(
+        self,
+        df: DataFrame,
+        output_df_params: OutputDataFrameParams,
+    ) -> None:
+        """
+        Writes a DataFrame to a specified location with optional date partitions.
+
+        Args:
+            df (DataFrame): The DataFrame to be written.
+            df_params (OutputDataFrameParams): The parameters for writing the DataFrame.
+
+        Returns:
+            None
+        """
+        if output_df_params.dataframe_base_path:
+            self._write_dataframe_base_path(df, output_df_params)
+        else:
+            self._write_dataframe_specific_path(df, output_df_params)
+
+        if (
+            output_df_params.write_schema_on_s3
+            or output_df_params.dataframe_file_type != FileType.PARQUET
+        ):
+            self.write_schema(df, output_df_params)
 
         logger.info("Dataframe written successfully.\n")
 
     @staticmethod
     def read_and_validate_step_json(step_params_json_file_path):
         """
         Reads and validates a JSON file containing step parameters.
@@ -416,22 +394,22 @@
         """Reads multiple input dataframes based on the provided configuration."""
         dfs: DataFrameDict = {}
 
         for df_name, input_df_params in input_df_params_dict.items():
             logger.info(f"Starting read operation for DataFrame '{df_name}'...")
 
             try:
-                dfs[df_name] = self.read_dataframe(df_params=input_df_params)
-            except ReadPreviousDayException:
+                dfs[df_name] = self.read_dataframe(
+                    input_df_params=input_df_params, verbose=False
+                )
+                logger.info(f"Dataframe '{df_name}' read successfully.\n")
+            except EmptyDataFrameException:
                 logger.warning(
-                    f"DataFrame '{df_name}' not found for previous date. Skipping..."
+                    f"DataFrame '{df_name}' is empty. No data could be found in the specified path(s). Skipping."
                 )
-                continue
-
-            logger.info(f"Dataframe '{df_name}' read successfully.\n")
 
         return dfs
 
     def _select_transformation_function(self, transform_params: TransformParams):
         """Select the transformation function based on direct or indirect reference."""
         if transform_params.transform_function:
             return transform_params.transform_function
@@ -497,69 +475,41 @@
             output_df_params = output_df_params_dict.get(df_name)
 
             if output_df_params is None:
                 raise ValueError(
                     f"No OutputDataFrameParams found for dataframe '{df_name}'"
                 )
 
-            if output_df_params.df_params.specific_path:
-                self.write_dataframe_specific_path(df=df, df_params=output_df_params)
-            else:
-                self.write_dataframe(df=df, df_params=output_df_params)
-
-    def inject_processing_date_into_dataframe_params(
-        self,
-        params: Union[DataFrameReadWriteParams, DataFrameReadWriteParams],
-        processing_date: datetime,
-    ) -> Union[DataFrameReadWriteParams, DataFrameReadWriteParams]:
-        modified_params = params
-        modified_params.is_previous_date = False
-
-        if params.processing_date == "{{processing_date}}":
-            modified_params.processing_date = processing_date
-        elif params.processing_date == "{{processing_date_previous}}":
-            modified_params.processing_date = processing_date - timedelta(days=1)
-            modified_params.is_previous_date = True
-
-        return modified_params
+            self.write_dataframe(df, output_df_params)
 
     def inject_processing_date_into_step_params(
         self, step_params: StepParams, processing_date: datetime
-    ) -> StepParams:
-        modified_step_params = step_params
-
-        for df_name, df_params in modified_step_params.input_dataframes_params.items():
-            new_read_params = self.inject_processing_date_into_dataframe_params(
-                df_params.df_params, processing_date
-            )
-            if not isinstance(new_read_params, DataFrameReadWriteParams):
-                raise ValueError(
-                    f"Expected DataFrameReadParams, but received: {new_read_params}"
-                )
-            modified_step_params.input_dataframes_params[
-                df_name
-            ].df_params = new_read_params
-
-        if modified_step_params.output_dataframes_params:
-            for (
-                df_name,
-                df_params,
-            ) in modified_step_params.output_dataframes_params.items():
-                new_write_params = self.inject_processing_date_into_dataframe_params(
-                    df_params.df_params, processing_date
-                )
-                if not isinstance(new_write_params, DataFrameReadWriteParams):
-                    raise ValueError(
-                        f"Expected DataFrameWriteParams, but received: {new_write_params}"
-                    )
-                modified_step_params.output_dataframes_params[
-                    df_name
-                ].df_params = new_write_params
-
-        return modified_step_params
+    ) -> None:
+        for _, df_params in step_params.input_dataframes_params.items():
+            if df_params.read_date_params:
+                df_params.read_date_params.was_offset_applied = False
+
+                if df_params.read_date_params.read_dates == "{{processing_date}}":
+                    df_params.read_date_params.read_dates = processing_date
+
+                    if df_params.read_date_params.processing_date_offset_days != 0:
+                        df_params.read_date_params.read_dates
+                        +timedelta(
+                            days=df_params.read_date_params.processing_date_offset_days
+                        )
+                        df_params.read_date_params.was_offset_applied = True
+
+        if step_params.output_dataframes_params:
+            for _, df_params in step_params.output_dataframes_params.items():
+                if (
+                    df_params.single_write_date
+                    and df_params.single_write_date.single_write_date
+                    == "{{processing_date}}"
+                ):
+                    df_params.single_write_date.single_write_date = processing_date
 
     def process_step(
         self,
         step_params_json_file_path: Optional[str] = None,
         step_params: Optional[StepParams] = None,
         processing_date: Optional[datetime] = None,
         write_output_dfs: bool = True,
@@ -600,15 +550,15 @@
 
         assert step_params is not None, "'step_params' was unexpectedly None"
 
         if processing_date is not None:
             logger.debug(
                 f"Injecting processing date '{processing_date}' into step parameters..."
             )
-            step_params = self.inject_processing_date_into_step_params(
+            self.inject_processing_date_into_step_params(
                 step_params=step_params,
                 processing_date=processing_date,
             )
             logger.debug("Processing date injected successfully.")
 
         try:
             print("\nPhase 1: Read Input DataFrames\n" + "-" * 80)
```

### Comparing `ng_data_pipelines_sdk-0.9.0/ng_data_pipelines_sdk/interfaces.py` & `ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/interfaces.py`

 * *Files 27% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import (
     Any,
     Callable,
     Dict,
     List,
     Literal,
     Optional,
+    Sequence,
     Union,
     get_args,
     get_origin,
 )
 
 from pydantic import BaseModel, field_validator, model_validator
 from pyspark.sql.dataframe import DataFrame
@@ -34,14 +35,23 @@
     """
 
     def __init__(self, message: str = "Dataframe from the previous day not found"):
         self.message = message
         super().__init__(self.message)
 
 
+class EmptyDataFrameException(Exception):
+    """
+    Exception raised when the dataframe is empty.
+    """
+
+    def __init__(self, message: str = "Dataframe is empty"):
+        self.message = message
+        super().__init__(self.message)
+
 
 class FileType(str, Enum):
     """
     Represents the type of file used in data pipelines.
 
     Attributes:
         CSV (str): Represents a CSV file.
@@ -85,25 +95,19 @@
 
 
 class DatePartition(str, Enum):
     """
     Enum representing different types of date partitions.
 
     Attributes:
-        PART_YEAR (str): Represents a partition by year, with name "part_year".
-        PART_MONTH (str): Represents a partition by month, with name "part_month".
-        PART_DAY (str): Represents a partition by day, with name "part_day".
         YEAR (str): Represents a partition by year, with name "year".
         MONTH (str): Represents a partition by month, with name "month".
         DAY (str): Represents a partition by day, with name "day".
     """
 
-    PART_YEAR = "part_year"
-    PART_MONTH = "part_month"
-    PART_DAY = "part_day"
     YEAR = "year"
     MONTH = "month"
     DAY = "day"
 
 
 class FnKind(str, Enum):
     """
@@ -178,29 +182,25 @@
                     "'layer' must be provided if 'bucket_name' is not provided"
                 )
             data["bucket_name"] = f"{ng_prefix}-datalake-{layer}-{env}"
 
         return data
 
 
-class S3ReadJsonParams(BaseModelJsonDumps):
+class S3ReadSchemaParams(BaseModelJsonDumps):
     """
-    Represents the parameters for reading a JSON file from an S3 bucket.
+    Represents the parameters for reading a schema from an S3 bucket.
 
     Attributes:
         bucket_params (S3BucketParams): The parameters for the S3 bucket.
-        path (str): The path to the JSON file in the S3 bucket.
+        path (str): The path to the schema file in the S3 bucket.
 
     Methods:
-        strip_slashes(cls, v: str) -> str: A class method that strips leading and trailing slashes from the path.
-        ensure_path_to_file_has_json_extension(cls, v: str) -> str: A class method that ensures the path has a '.json' extension.
-
-    Raises:
-        ValueError: If the path does not have a '.json' extension.
-
+        strip_slashes(v: str) -> str: A class method that strips leading and trailing slashes from the path.
+        ensure_path_to_file_has_json_extension(v: str) -> str: A class method that ensures the path has a '.json' extension.
     """
 
     bucket_params: S3BucketParams
     path: str
 
     @field_validator("path")
     @classmethod
@@ -214,165 +214,243 @@
             raise ValueError(
                 f"For S3 schema, 'path' must have a '.json' extension. Received path: '{v}'"
             )
 
         return v
 
 
-class DataFrameReadWriteParams(BaseModelJsonDumps):
+class DataFrameBaseParams(BaseModelJsonDumps):
     """
-    Represents the parameters for reading and writing a DataFrame.
+    Represents the base parameters for a DataFrame.
 
     Attributes:
-        bucket_params (S3BucketParams): The parameters for the S3 bucket.
-        specific_path (Optional[Union[List[str], str]]): The specific path to the data within the bucket.
-        path_to_dataframe_root (Optional[str]): The path to the root folder of the DataFrame within the bucket.
-        file_type (FileType): The type of file to read or write.
-        processing_date (Union[List[datetime], datetime, Literal["{{processing_date}}"], Literal["{{processing_date_previous}}"]]): The processing date or dates to use for partitioning.
-        processing_date_partitions (Optional[List[DatePartition]]): The list of date partitions to use for filtering.
-        processing_date_partitions_first (bool): Flag indicating whether to process date partitions first.
-        column_partitions (Optional[List[str]]): The list of column partitions to use for filtering.
+        dataframe_bucket_params (S3BucketParams): The bucket parameters for the DataFrame.
+        dataframe_specific_paths (Optional[Union[List[str], str]]): The specific path for the DataFrame. Defaults to None.
+        dataframe_base_path (Optional[str]): The base path for the DataFrame. Defaults to None.
+        dataframe_file_type (FileType): The file type of the DataFrame.
     """
 
-    bucket_params: S3BucketParams
-    specific_path: Optional[Union[List[str], str]] = None
-    path_to_dataframe_root: Optional[str] = None
-    file_type: FileType
-    processing_date: Union[
-        List[datetime],
+    dataframe_bucket_params: S3BucketParams
+    dataframe_base_path: Optional[str] = None
+    dataframe_file_type: FileType
+
+    @field_validator("dataframe_base_path")
+    def strip_and_ensure_dataframe_base_path_parent_folder(cls, v: str) -> str:
+        if v is not None:
+            v = v.strip("/")
+
+        if "/" not in v:
+            raise ValueError(
+                f"'dataframe_base_path' should have at least one parent folder inside the bucket. Ensure there is at least one slash ('/') in the path. Received path: '{v}'"
+            )
+
+        return v
+
+
+class ReadDateParams(BaseModelJsonDumps):
+    """
+    Represents the parameters for reading dates in a data pipeline.
+
+    Attributes:
+        read_dates (Union[List[datetime], datetime, Literal["{{processing_date}}"], Literal["{{processing_date_previous}}"]]):
+            The dates to be read. It can be a list of datetimes, a single datetime, or special placeholders for processing dates.
+            The default value is "{{processing_date}}".
+        processing_date_offset_days (int):
+            The offset to be applied to the processing date. It represents the number of days to add or subtract from the processing date.
+            The default value is 0.
+        date_partitions (List[str]):
+            The date partitions to be included in the read. It is a list of strings representing the desired partitions, such as "year", "month", "day".
+            The default value is ["year", "month", "day"].
+        date_partitions_first (bool):
+            Specifies whether the date partitions should be added as the first columns in the read data.
+            The default value is True.
+        add_all_date_columns (bool):
+            Specifies whether all date columns should be added to the read data.
+            The default value is True.
+    """
+
+    read_dates: Union[
+        Sequence[Union[Union[str, datetime], List[Union[str, datetime]]]],
         datetime,
         Literal["{{processing_date}}"],
-        Literal["{{processing_date_previous}}"],
     ] = "{{processing_date}}"
-    processing_date_partitions: Optional[List[DatePartition]] = None
-    processing_date_partitions_first: bool = True
+    processing_date_offset_days: int = 0
+    was_offset_applied: bool = False
+    date_partitions: List[str] = ["year", "month", "day"]
+    date_partitions_first: bool = True
+    add_all_date_columns: bool = True
+
+
+class InputDataFrameParams(DataFrameBaseParams):
+    """
+    Parameters for input data frames.
+
+    Attributes:
+        pyspark_schema_struct (Optional[Dict[str, Any]]): The schema of the input data frame in PySpark StructType format.
+        s3_schema_path_params (Optional[S3ReadSchemaParams]): The parameters for reading the schema from an S3 path.
+        read_date_params (Optional[ReadDateParams]): The parameters for reading the date from the input data frame.
+        column_partitions (Optional[List[str]]): The list of column names to be used for partitioning the input data frame.
+
+    Methods:
+        check_schema_mode(cls, data): Check the schema mode and validate the input data.
+
+    Raises:
+        ValueError: If 'pyspark_schema_struct' and 's3_schema_path_params' are passed together.
+    """
+
+    dataframe_specific_paths: Optional[Union[List[str], str]] = None
+    pyspark_schema_struct: Optional[Dict[str, Any]] = None
+    s3_schema_path_params: Optional[S3ReadSchemaParams] = None
+    read_date_params: Optional[ReadDateParams] = None
     column_partitions: Optional[List[str]] = None
-    is_previous_date: bool = False
 
     @model_validator(mode="before")
-    def xor_specific_path_and_path_to_dataframe_root(cls, data):
+    def check_schema_mode(cls, data):
         """
-        Validates that 'specific_path' and 'path_to_dataframe_root' are not passed together.
+        Check the schema mode and validate the input data.
 
         Args:
-            data (dict): The input data.
-
-        Raises:
-            ValueError: If 'specific_path' and 'path_to_dataframe_root' are passed together.
+            cls: The class object.
+            data: The input data dictionary.
 
         Returns:
-            dict: The validated data.
+            The validated input data dictionary.
+
+        Raises:
+            ValueError: If 'pyspark_schema_struct' and 's3_schema_path_params' are passed together.
         """
-        specific_path = data.get("specific_path")
-        path_to_dataframe_root = data.get("path_to_dataframe_root")
+        pyspark_schema_struct = data.get("pyspark_schema_struct")
+        s3_schema_path_params = data.get("s3_schema_path_params")
 
-        if specific_path is not None and path_to_dataframe_root is not None:
+        if pyspark_schema_struct is not None and s3_schema_path_params is not None:
             raise ValueError(
-                "'specific_path' and 'path_to_dataframe_root' cannot be passed together"
+                "'pyspark_schema_struct' and 's3_schema_path_params' cannot be passed together"
             )
 
-        if specific_path is None and path_to_dataframe_root is None:
+        return data
+
+    @model_validator(mode="before")
+    def xor_specific_path_and_dataframe_base_path(cls, data):
+        dataframe_specific_paths = data.get("dataframe_specific_paths")
+        dataframe_base_path = data.get("dataframe_base_path")
+
+        if dataframe_specific_paths is not None and dataframe_base_path is not None:
             raise ValueError(
-                "Either 'specific_path' or 'path_to_dataframe_root' should be passed"
+                "'dataframe_specific_paths' and 'dataframe_base_path' cannot be passed together"
+            )
+
+        if dataframe_specific_paths is None and dataframe_base_path is None:
+            raise ValueError(
+                "Either 'dataframe_specific_paths' or 'dataframe_base_path' should be passed"
             )
 
         return data
 
-    @field_validator("path_to_dataframe_root", "specific_path")
-    def strip_slashes(cls, v: Union[str, List[str]]) -> str:
-        """
-        Strips leading and trailing slashes from the input string.
+    @model_validator(mode="before")
+    def xor_specific_path_and_read_date_params(cls, data):
+        dataframe_specific_paths = data.get("dataframe_specific_paths")
+        read_date_params = data.get("read_date_params")
 
-        Args:
-            v (str): The input string.
+        if dataframe_specific_paths is not None and read_date_params is not None:
+            raise ValueError(
+                "'dataframe_specific_paths' and 'read_date_params' cannot be passed together"
+            )
 
-        Returns:
-            str: The input string with leading and trailing slashes stripped.
-        """
+        return data
+
+    @field_validator("dataframe_specific_paths")
+    def strip_dataframe_specific_paths(cls, v: str) -> str:
         if v is not None:
             if isinstance(v, list):
                 return [x.strip("/") for x in v]  # type: ignore
             else:
                 return v.strip("/")
 
-    @field_validator("path_to_dataframe_root")
-    def ensure_dataframe_root_parent_folder(cls, v: str) -> str:
-        """
-        Ensures that 'path_to_dataframe_root' has at least one parent folder inside the bucket.
-
-        Args:
-            v (str): The input string.
-
-        Raises:
-            ValueError: If 'path_to_dataframe_root' does not have at least one parent folder.
-
-        Returns:
-            str: The input string.
-        """
-        if v is not None and "/" not in v:
-            raise ValueError(
-                f"'path_to_dataframe_root' should have at least one parent folder inside the bucket. Ensure there is at least one slash ('/') in the path. Received path: '{v}'"
-            )
-
-        return v
-
 
-class InputDataFrameParams(BaseModelJsonDumps):
+class SingleWriteDateParams(BaseModelJsonDumps):
     """
-    Represents the parameters for an input DataFrame.
+    Represents the parameters for a single write date.
 
     Attributes:
-        pyspark_schema_struct (Optional[Dict[str, Any]]): The schema of the input DataFrame in PySpark struct format.
-        s3_schema_path_params (Optional[S3ReadJsonParams]): The parameters for reading the schema from an S3 path.
-        df_params (DataFrameReadWriteParams): The parameters for reading and writing the DataFrame.
-    """
-
-    pyspark_schema_struct: Optional[Dict[str, Any]] = None
-    s3_schema_path_params: Optional[S3ReadJsonParams] = None
-    df_params: DataFrameReadWriteParams
-
-    @model_validator(mode="before")
-    def check_schema_mode(cls, data):
+        single_write_date (Union[datetime, Literal["{{processing_date}}"]]):
+            The single write date. It can be either a datetime object or the string "{{processing_date}}".
+        single_write_date_partitions (List[str]):
+            The list of partitions to be used for the single write date. Defaults to ["year", "month", "day"].
+    """
+
+    single_write_date: Union[datetime, Literal["{{processing_date}}"]] = (
+        "{{processing_date}}"
+    )
+    single_write_date_partitions: dict[DatePartition, str] = {
+        DatePartition.YEAR: "year",
+        DatePartition.MONTH: "month",
+        DatePartition.DAY: "day",
+    }
+
+    @field_validator("single_write_date_partitions")
+    def ensure_all_date_partitions(
+        cls, v: dict[DatePartition, str]
+    ) -> dict[DatePartition, str]:
         """
-        Check the schema mode and validate the input data.
+        Ensures that all date partitions are present in the input dictionary.
 
         Args:
-            cls: The class object.
-            data: The input data dictionary.
+            v (dict[DatePartition, str]): The input dictionary.
 
         Returns:
-            The validated input data dictionary.
+            dict[DatePartition, str]: The input dictionary.
 
         Raises:
-            ValueError: If 'pyspark_schema_struct' and 's3_schema_path_params' are passed together.
+            ValueError: If any date partition is missing.
         """
-        pyspark_schema_struct = data.get("pyspark_schema_struct")
-        s3_schema_path_params = data.get("s3_schema_path_params")
+        date_partitions = [DatePartition.YEAR, DatePartition.MONTH, DatePartition.DAY]
 
-        if pyspark_schema_struct is not None and s3_schema_path_params is not None:
-            raise ValueError(
-                "'pyspark_schema_struct' and 's3_schema_path_params' cannot be passed together"
-            )
+        for date_partition in date_partitions:
+            if date_partition not in v:
+                raise ValueError(
+                    f"Missing date partition: '{date_partition}'. The dictionary must contain all date partitions: {date_partitions}"
+                )
 
-        return data
+        return v
 
 
-class OutputDataFrameParams(BaseModelJsonDumps):
+class OutputDataFrameParams(DataFrameBaseParams):
     """
-    Represents the parameters for writing an output DataFrame.
+    Parameters for writing output dataframes.
 
     Attributes:
         write_schema_on_s3 (bool): Whether to write the schema on S3.
         overwrite (bool): Whether to overwrite existing data.
-        df_params (DataFrameReadWriteParams): Parameters for reading and writing the DataFrame.
+        single_write_date (Optional[SingleWriteDateParams]): Parameters for single write date.
+        partition_by (List[str]): List of columns to partition the data by.
     """
 
+    dataframe_specific_path: Optional[str] = None
     write_schema_on_s3: bool = False
     overwrite: bool = False
-    df_params: DataFrameReadWriteParams
+    dataframe_file_type: FileType = FileType.PARQUET
+    single_write_date: Optional[SingleWriteDateParams] = None
+    partition_by: List[str] = ["year", "month", "day"]
+
+    @model_validator(mode="before")
+    def xor_specific_path_and_dataframe_base_path(cls, data):
+        dataframe_specific_path = data.get("dataframe_specific_path")
+        dataframe_base_path = data.get("dataframe_base_path")
+
+        if dataframe_specific_path is not None and dataframe_base_path is not None:
+            raise ValueError(
+                "'dataframe_specific_path' and 'dataframe_base_path' cannot be passed together"
+            )
+
+        if dataframe_specific_path is None and dataframe_base_path is None:
+            raise ValueError(
+                "Either 'dataframe_specific_path' or 'dataframe_base_path' should be passed"
+            )
+
+        return data
 
 
 class FnIndirect(BaseModelJsonDumps):
     fn_name: str
     fn_path: str
```

### Comparing `ng_data_pipelines_sdk-0.9.0/ng_data_pipelines_sdk/spark_manager.py` & `ng_data_pipelines_sdk-1.0.0/ng_data_pipelines_sdk/spark_manager.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Dict, List, Optional, Union
 
 from pyspark.conf import SparkConf
 from pyspark.sql import DataFrame, SparkSession
 from pyspark.sql.types import StructType
+from ng_data_pipelines_sdk.custom_logger import logger
 
 from ng_data_pipelines_sdk.interfaces import AWSCredentials, Env, FileType
 
 
 class SparkManager:
     """
     A class that manages the SparkSession and provides methods for reading and writing data.
@@ -77,47 +78,61 @@
             )
 
         return config
 
     def read(
         self,
         env: Env,
-        path: Union[str, List[str]],
+        paths: Union[str, List[str]],
         file_type: FileType,
+        base_path: Optional[str] = None,
         schema: Optional[StructType] = None,
-    ):
-        """
-        Reads data from a specified path using the specified file type and optional schema.
+        cache: bool = False,
+    ) -> Optional[DataFrame]:
+        def get_existing_paths(paths: List[str]) -> List[str]:
+            sc = self.spark.sparkContext
+            hadoop_conf = sc._jsc.hadoopConfiguration()
+            existing_paths = []
+            for path in paths:
+                fs_path = self.spark._jvm.org.apache.hadoop.fs.Path(path)
+                fs = fs_path.getFileSystem(hadoop_conf)
+                if fs.exists(fs_path):
+                    existing_paths.append(path)
+                else:
+                    logger.warning(f"Path does not exist (ignoring): {path}")
 
-        Args:
-            env (Env): The environment to use for setting AWS credentials.
-            path (Union[str, List[str]]): The path or list of paths to the data source.
-            file_type (FileType): The type of the data source.
-            schema (Optional[StructType], optional): The schema to use for reading the data. Defaults to None.
+            return existing_paths
 
-        Returns:
-            DataFrame: The loaded data as a DataFrame.
+        self._set_aws_credentials(env)
 
-        Raises:
-            None
+        if isinstance(paths, str):
+            paths = [paths]
 
-        Examples:
-            >>> env = Env()
-            >>> path = "/path/to/data"
-            >>> file_type = FileType.CSV
-            >>> schema = StructType([StructField("name", StringType()), StructField("age", IntegerType())])
-            >>> spark_manager = SparkManager()
-            >>> df = spark_manager.read(env, path, file_type, schema)
-        """
-        self._set_aws_credentials(env)
+        existing_paths = get_existing_paths(paths)
+
+        if existing_paths == []:
+            logger.warning("No existing paths found.")
+            return None
 
+        logger.info(f"Reading data from existing paths: {existing_paths}")
+
+        reader = self.spark.read.format(file_type)
         if schema:
-            return self.spark.read.format(file_type).schema(schema).load(path)
-        else:
-            return self.spark.read.format(file_type).load(path)
+            reader = reader.schema(schema)
+        if base_path:
+            reader = reader.option("basePath", base_path)
+
+        df = reader.load(existing_paths)
+
+        if cache:
+            logger.info("Caching DataFrame...")
+            df.cache()
+            df.count()  # Trigger caching
+
+        return df
 
     def write(
         self,
         env: Env,
         df: DataFrame,
         path: str,
         file_type: FileType,
```

### Comparing `ng_data_pipelines_sdk-0.9.0/pyproject.toml` & `ng_data_pipelines_sdk-1.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "ng-data-pipelines-sdk"
-version = "0.9.0"
-description = "A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airflow 2.8.1."
+version = "1.0.0"
+description = "A library for interacting with data from Amazon S3 through PySpark. Read, write and tranform data using a powerful and intuitive API with strong consistency and type checking, thanks to Pydantic. Compatible with Amazon MWAA running Airflow 2.7.2 and 2.8.1."
 authors = ["ng.cash"]
 readme = "README.md"
 exclude = [".git/", ".gitignore", "tests/", "docs/", "*.yml", "__pycache__/", "*.pyc", "*.ipynb", "playground/", "poetry.lock", "dist/", "build/"]
 
 [tool.poetry.dependencies]
 python = ">=3.9, <3.12"
 pyspark = "^3.2.0"
 pydantic = "^2.4.2"
 boto3 = "^1.28.17"
+pandas = "^2.1.1"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.29.4"
 ruff = "^0.3.7"
 load-dotenv = "^0.1.0"
 
 [build-system]
```

### Comparing `ng_data_pipelines_sdk-0.9.0/PKG-INFO` & `ng_data_pipelines_sdk-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: ng-data-pipelines-sdk
-Version: 0.9.0
-Summary: A library for facilitating the development of data engineering pipelines using pyspark. Compatible with MWAA running airflow 2.8.1.
+Version: 1.0.0
+Summary: A library for interacting with data from Amazon S3 through PySpark. Read, write and tranform data using a powerful and intuitive API with strong consistency and type checking, thanks to Pydantic. Compatible with Amazon MWAA running Airflow 2.7.2 and 2.8.1.
 Author: ng.cash
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.28.17,<2.0.0)
+Requires-Dist: pandas (>=2.1.1,<3.0.0)
 Requires-Dist: pydantic (>=2.4.2,<3.0.0)
 Requires-Dist: pyspark (>=3.2.0,<4.0.0)
 Description-Content-Type: text/markdown
 
 docker run --rm -it -d -e PYTHONPATH="/ng-data-pipelines-sdk" -v $pwd:/ng-data-pipelines-sdk pyspark-local
```

