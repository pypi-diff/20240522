# Comparing `tmp/powerlift-0.1.3-py3-none-any.whl.zip` & `tmp/powerlift-0.1.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 27921 bytes, number of entries: 20
+Zip file size: 27832 bytes, number of entries: 20
 -rw-r--r--  2.0 unx      712 b- defN 24-May-17 18:23 powerlift/bench/__init__.py
 -rw-r--r--  2.0 unx     6431 b- defN 24-May-12 23:47 powerlift/bench/benchmark.py
 -rw-r--r--  2.0 unx     5888 b- defN 24-May-10 19:49 powerlift/bench/experiment.py
 -rw-r--r--  2.0 unx    36592 b- defN 24-May-21 06:32 powerlift/bench/store.py
 -rw-r--r--  2.0 unx      856 b- defN 24-May-07 19:14 powerlift/db/__init__.py
 -rw-r--r--  2.0 unx     1364 b- defN 24-May-10 18:52 powerlift/db/actions.py
 -rw-r--r--  2.0 unx     6971 b- defN 24-May-10 18:52 powerlift/db/schema.py
 -rw-r--r--  2.0 unx      233 b- defN 24-May-07 19:14 powerlift/executors/__init__.py
--rw-r--r--  2.0 unx     7639 b- defN 24-May-07 19:14 powerlift/executors/azure_ci.py
+-rw-r--r--  2.0 unx     7411 b- defN 24-May-22 18:09 powerlift/executors/azure_ci.py
 -rw-r--r--  2.0 unx     2275 b- defN 24-May-07 19:14 powerlift/executors/base.py
--rw-r--r--  2.0 unx     3041 b- defN 24-May-07 19:14 powerlift/executors/docker.py
+-rw-r--r--  2.0 unx     2886 b- defN 24-May-22 18:22 powerlift/executors/docker.py
 -rw-r--r--  2.0 unx     3069 b- defN 24-May-14 00:02 powerlift/executors/localmachine.py
 -rw-r--r--  2.0 unx      136 b- defN 24-May-07 19:14 powerlift/measures/__init__.py
 -rw-r--r--  2.0 unx     4500 b- defN 24-May-07 19:14 powerlift/measures/task_measures.py
 -rw-r--r--  2.0 unx     2639 b- defN 24-May-21 06:34 powerlift/run/__main__.py
--rw-r--r--  2.0 unx     1085 b- defN 24-May-21 06:36 powerlift-0.1.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     5740 b- defN 24-May-21 06:36 powerlift-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-21 06:36 powerlift-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 24-May-21 06:36 powerlift-0.1.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1668 b- defN 24-May-21 06:36 powerlift-0.1.3.dist-info/RECORD
-20 files, 90941 bytes uncompressed, 25201 bytes compressed:  72.3%
+-rw-r--r--  2.0 unx     1085 b- defN 24-May-22 20:28 powerlift-0.1.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5740 b- defN 24-May-22 20:28 powerlift-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-22 20:28 powerlift-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 24-May-22 20:28 powerlift-0.1.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1668 b- defN 24-May-22 20:28 powerlift-0.1.4.dist-info/RECORD
+20 files, 90558 bytes uncompressed, 25112 bytes compressed:  72.3%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: powerlift/measures/task_measures.py
 Comment: 
 
 Filename: powerlift/run/__main__.py
 Comment: 
 
-Filename: powerlift-0.1.3.dist-info/LICENSE
+Filename: powerlift-0.1.4.dist-info/LICENSE
 Comment: 
 
-Filename: powerlift-0.1.3.dist-info/METADATA
+Filename: powerlift-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: powerlift-0.1.3.dist-info/WHEEL
+Filename: powerlift-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: powerlift-0.1.3.dist-info/top_level.txt
+Filename: powerlift-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: powerlift-0.1.3.dist-info/RECORD
+Filename: powerlift-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## powerlift/executors/azure_ci.py

```diff
@@ -124,15 +124,14 @@
         azure_client_secret: str,
         subscription_id: str,
         resource_group: str,
         image: str = "interpretml/powerlift:0.0.1",
         n_running_containers: int = 1,
         num_cores: int = 1,
         mem_size_gb: int = 2,
-        raise_exception: bool = False,
         wheel_filepaths: List[str] = None,
         docker_db_uri: str = None,
     ):
         """Runs remote execution of trials via Azure Container Instances.
 
         Args:
             store (Store): Store that houses trials.
@@ -141,15 +140,14 @@
             azure_client_secret (str): Azure client secret.
             subscription_id (str): Azure subscription ID.
             resource_group (str): Azure resource group.
             image (str, optional): Image to execute. Defaults to "interpretml/powerlift:0.0.1".
             n_running_containers (int, optional): Max number of containers to run simultaneously. Defaults to 1.
             num_cores (int, optional): Number of cores per container. Defaults to 1.
             mem_size_gb (int, optional): RAM size in GB per container. Defaults to 2.
-            raise_exception (bool, optional): Raise exception on failure. Defaults to False.
             wheel_filepaths (List[str], optional): List of wheel filepaths to install on ACI trial run. Defaults to None.
             docker_db_uri (str, optional): Database URI for container. Defaults to None.
         """
         from multiprocessing import Manager
 
         self._image = image
         self._n_running_containers = n_running_containers
@@ -160,15 +158,15 @@
         self._azure_json = {
             "tenant_id": azure_tenant_id,
             "client_id": azure_client_id,
             "client_secret": azure_client_secret,
             "subscription_id": subscription_id,
             "resource_group": resource_group,
         }
-        super().__init__(store, n_running_containers, raise_exception, wheel_filepaths)
+        super().__init__(store, n_running_containers, False, wheel_filepaths)
 
     def delete_credentials(self):
         """Deletes credentials in object for accessing Azure Resources."""
         del self._azure_json
 
     def submit(self, trial_run_fn, trials: Iterable, timeout=None):
         uri = (
@@ -179,15 +177,15 @@
             [x.id for x in trials], trial_run_fn, self._wheel_filepaths
         )
         for trial in trials:
             params = (
                 [trial.id],
                 uri,
                 timeout,
-                self._raise_exception,
+                False,
                 self._image,
             )
             tasks.append(params)
 
         params = (
             tasks,
             self._azure_json,
@@ -197,15 +195,13 @@
         )
         if self._pool is None:
             try:
                 res = _run(*params)
                 self._trial_id_to_result[0] = res
             except Exception as e:
                 self._trial_id_to_result[0] = e
-                if self._raise_exception:
-                    raise e
         else:
             self._trial_id_to_result[0] = self._pool.apply_async(
                 _run,
                 params,
                 error_callback=handle_err,
             )
```

## powerlift/executors/docker.py

```diff
@@ -40,45 +40,43 @@
     which means other users on the machine may be able to see it via enumerating
     the processes on the machine and their args.
     """
 
     def __init__(
         self,
         store: Store,
-        image: str = "interpretml/powerlift:0.0.1",
+        image: str = "interpretml/powerlift:0.1.4",
         n_running_containers: int = None,
-        raise_exception: bool = False,
         wheel_filepaths: List[str] = None,
         docker_db_uri: str = None,
     ):
         """Runs trials in local docker containers.
 
         Args:
             store (Store): Store that houses trials.
             image (str, optional): Image to execute in container. Defaults to "interpretml/powerlift:0.0.1".
             n_running_containers (int, optional): Max number of containers running simultaneously. Defaults to None.
-            raise_exception (bool, optional): Raise exception on failure. Defaults to False.
-            wheel_filepaths (List[str], optional): List of wheel filepaths to install on ACI trial run. Defaults to None.
+            wheel_filepaths (List[str], optional): List of wheel filepaths to install on docker trial run. Defaults to None.
             docker_db_uri (str, optional): Database URI for container. Defaults to None.
         """
         self._docker_db_uri = docker_db_uri
         self._image = image
-        super().__init__(store, n_running_containers, raise_exception, wheel_filepaths)
+        super().__init__(store, n_running_containers, False, wheel_filepaths)
 
     def submit(self, trial_run_fn, trials: Iterable, timeout=None):
         uri = (
             self._docker_db_uri if self._docker_db_uri is not None else self._store.uri
         )
         self._store.add_trial_run_fn(
             [x.id for x in trials], trial_run_fn, self._wheel_filepaths
         )
         for trial in trials:
             self._trial_id_to_result[trial.id] = self._pool.apply_async(
                 _run_docker,
-                ([trial.id], uri, timeout, self._raise_exception, self._image),
+                ([trial.id], uri, timeout, False, self._image),
                 error_callback=handle_err,
             )
 
     @property
     def docker_db_uri(self):
         return self._docker_db_uri
```

## Comparing `powerlift-0.1.3.dist-info/LICENSE` & `powerlift-0.1.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `powerlift-0.1.3.dist-info/METADATA` & `powerlift-0.1.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: powerlift
-Version: 0.1.3
+Version: 0.1.4
 Summary: Interactive Benchmarking for Machine Learning.
 Home-page: https://github.com/interpretml/interpret
 Author: The InterpretML Contributors
 Author-email: interpret@microsoft.com
 Project-URL: Bug Tracker, https://github.com/interpretml/interpret/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `powerlift-0.1.3.dist-info/RECORD` & `powerlift-0.1.4.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 powerlift/bench/benchmark.py,sha256=QHNyfwsOCAac9pXrXSq2O3GI2VB20Rs6i3_3DDH240I,6431
 powerlift/bench/experiment.py,sha256=LCjzoJVSBa96XvFbwYvk1obMbKJHal2NU4fzL0r64PI,5888
 powerlift/bench/store.py,sha256=9ZrAyF7L-ABNLsnE3eZREMsi87cOgg8v2ahL9Z_-Pao,36592
 powerlift/db/__init__.py,sha256=f0S6DsKHCEB8iZ6cVh7MX-1kl4KHtgVsmJcbtfEknEU,856
 powerlift/db/actions.py,sha256=qc9NxS9TLNfx9qYaPlpS4KpJhuGfSoKe3andHYJI32g,1364
 powerlift/db/schema.py,sha256=T1pCXaiLew_04Oadpg5IE6aYmwRokh-kU5m68lutMKI,6971
 powerlift/executors/__init__.py,sha256=Xxy4Qzjfe-hFY1ZarMYBEjH076CKHuHOTxqszoPYvuw,233
-powerlift/executors/azure_ci.py,sha256=hpjuyDlNFBFHwqiaVR6ZzHn7upN0NI7xJUHkJiFJN3A,7639
+powerlift/executors/azure_ci.py,sha256=ncSEPHTt-Zu3BUyFDRaITDT83MeFhTe-c1imdUz8Ceo,7411
 powerlift/executors/base.py,sha256=Blhm0ZiF6u0_wqw8NjYKmF70fdkZsyL61zX5DfBdZoY,2275
-powerlift/executors/docker.py,sha256=1g-hphvh-g5-QuG_xyo7bhBp0SMdYIzY8EHz0D27Ixc,3041
+powerlift/executors/docker.py,sha256=3LzgMsuvKkM3aZE3GX1sUA6l8H1MxATkV7N2uHaYrYg,2886
 powerlift/executors/localmachine.py,sha256=8dYImIq5cQPVk0H4B_AiPpVGZKIhdbB05s46f717TOA,3069
 powerlift/measures/__init__.py,sha256=br7A9iJgQl7cPcPFnnJkRGEDRn_IBJMj24rVZFaSF44,136
 powerlift/measures/task_measures.py,sha256=23zwd25L_KB9Xe6LuWtBS4QBuv1F0mKnCR4HAKjsmg0,4500
 powerlift/run/__main__.py,sha256=YbXDeF33dehQgEEEFfuCctGlr2dTmNNhKjCibEg-EuE,2639
-powerlift-0.1.3.dist-info/LICENSE,sha256=7vlTCQ2WSK8wDjuX9Rv36FpE_bEP1FkMVxceVw-VTGs,1085
-powerlift-0.1.3.dist-info/METADATA,sha256=MLy6mXrb4T6HTT0xu7GA_xaldcJIVeupSzT4q2ikAA4,5740
-powerlift-0.1.3.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-powerlift-0.1.3.dist-info/top_level.txt,sha256=PqZeILUPLCstbaDfaAG14A4rCLPYynR_EKCJjGGW88s,10
-powerlift-0.1.3.dist-info/RECORD,,
+powerlift-0.1.4.dist-info/LICENSE,sha256=7vlTCQ2WSK8wDjuX9Rv36FpE_bEP1FkMVxceVw-VTGs,1085
+powerlift-0.1.4.dist-info/METADATA,sha256=xpR30KcM41rm453hr7XmPmQbT8bSflA8F8KsL4dVNYs,5740
+powerlift-0.1.4.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+powerlift-0.1.4.dist-info/top_level.txt,sha256=PqZeILUPLCstbaDfaAG14A4rCLPYynR_EKCJjGGW88s,10
+powerlift-0.1.4.dist-info/RECORD,,
```

