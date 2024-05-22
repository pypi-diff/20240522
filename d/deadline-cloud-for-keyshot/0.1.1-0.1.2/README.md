# Comparing `tmp/deadline_cloud_for_keyshot-0.1.1.tar.gz` & `tmp/deadline_cloud_for_keyshot-0.1.2.tar.gz`

## Comparing `deadline_cloud_for_keyshot-0.1.1.tar` & `deadline_cloud_for_keyshot-0.1.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/_version.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/_version.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotAdaptor/KeyShotAdaptor.json
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotAdaptor/__init__.py
--rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotAdaptor/__main__.py
--rw-r--r--   0        0        0    19116 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotAdaptor/adaptor.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotAdaptor/schemas/init_data.schema.json
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotAdaptor/schemas/run_data.schema.json
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotClient/__init__.py
--rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotClient/keyshot_client.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotClient/keyshot_handler.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/__init__.py
--rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/__main__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/_version.py
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/adaptor_keyshot_job_template.yaml
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/data_classes.py
--rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/default_keyshot_job_template.yaml
--rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/keyshot_render_submitter.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/ui/__init__.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/ui/components/__init__.py
--rw-r--r--   0        0        0     7584 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/ui/components/scene_settings_tab.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/.gitignore
--rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/LICENSE
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/NOTICE
--rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/README.md
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/hatch.toml
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     7258 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/_version.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_adaptor/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_adaptor/_version.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_adaptor/KeyShotAdaptor/KeyShotAdaptor.json
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_adaptor/KeyShotAdaptor/__init__.py
+-rw-r--r--   0        0        0      819 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_adaptor/KeyShotAdaptor/__main__.py
+-rw-r--r--   0        0        0    19116 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_adaptor/KeyShotAdaptor/adaptor.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_adaptor/KeyShotAdaptor/schemas/init_data.schema.json
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_adaptor/KeyShotAdaptor/schemas/run_data.schema.json
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_adaptor/KeyShotClient/__init__.py
+-rw-r--r--   0        0        0     2464 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_adaptor/KeyShotClient/keyshot_client.py
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_adaptor/KeyShotClient/keyshot_handler.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_submitter/__init__.py
+-rw-r--r--   0        0        0      796 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_submitter/__main__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_submitter/_version.py
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_submitter/adaptor_keyshot_job_template.yaml
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_submitter/data_classes.py
+-rw-r--r--   0        0        0     2766 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_submitter/default_keyshot_job_template.yaml
+-rw-r--r--   0        0        0     7577 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_submitter/keyshot_render_submitter.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_submitter/ui/__init__.py
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_submitter/ui/components/__init__.py
+-rw-r--r--   0        0        0     7568 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_submitter/ui/components/scene_settings_tab.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/.gitignore
+-rw-r--r--   0        0        0    10142 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/LICENSE
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/NOTICE
+-rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/README.md
+-rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/hatch.toml
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     7291 2020-02-02 00:00:00.000000 deadline_cloud_for_keyshot-0.1.2/PKG-INFO
```

### Comparing `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotAdaptor/__main__.py` & `deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_adaptor/KeyShotAdaptor/__main__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotAdaptor/adaptor.py` & `deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_adaptor/KeyShotAdaptor/adaptor.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotAdaptor/schemas/init_data.schema.json` & `deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_adaptor/KeyShotAdaptor/schemas/init_data.schema.json`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotClient/keyshot_client.py` & `deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_adaptor/KeyShotClient/keyshot_client.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_adaptor/KeyShotClient/keyshot_handler.py` & `deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_adaptor/KeyShotClient/keyshot_handler.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/__main__.py` & `deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_submitter/__main__.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/adaptor_keyshot_job_template.yaml` & `deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_submitter/adaptor_keyshot_job_template.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/data_classes.py` & `deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_submitter/data_classes.py`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/default_keyshot_job_template.yaml` & `deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_submitter/default_keyshot_job_template.yaml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/keyshot_render_submitter.py` & `deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_submitter/keyshot_render_submitter.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import os
 import json
 from pathlib import Path
 from typing import Any, Optional
 import yaml  # type: ignore[import]
 from copy import deepcopy
 
-from PySide2 import QtWidgets
+from qtpy import QtWidgets
 
 from deadline.client import api
 from deadline.client.job_bundle.submission import AssetReferences
 from deadline.client.job_bundle._yaml import deadline_yaml_dump
 from deadline.client.ui.dialogs.submit_job_to_deadline_dialog import (  # pylint: disable=import-error
     SubmitJobToDeadlineDialog,
     JobBundlePurpose,
 )
 from deadline.client.exceptions import DeadlineOperationError
-from PySide2.QtCore import Qt  # pylint: disable=import-error
+from qtpy.QtCore import Qt  # type: ignore
 
 from .data_classes import (
     RenderSubmitterUISettings,
 )
 from .ui.components.scene_settings_tab import SceneSettingsWidget
 from ._version import version, version_tuple as adaptor_version_tuple
```

### Comparing `deadline_cloud_for_keyshot-0.1.1/src/deadline/keyshot_submitter/ui/components/scene_settings_tab.py` & `deadline_cloud_for_keyshot-0.1.2/src/deadline/keyshot_submitter/ui/components/scene_settings_tab.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright Amazon.com, Inc. or its affiliates. All Rights Reserved.
 import os
 from pathlib import Path
 
-from PySide2.QtCore import QSize, Qt  # type: ignore
-from PySide2.QtWidgets import (  # type: ignore
+from qtpy.QtCore import QSize, Qt  # type: ignore
+from qtpy.QtWidgets import (  # type: ignore
     QComboBox,
     QCheckBox,
     QFileDialog,
     QGridLayout,
     QHBoxLayout,
     QLabel,
     QLineEdit,
@@ -49,15 +49,14 @@
             raise ValueError("")
 
         self.file_format = file_format
         self.directory_only = directory_only
 
         lyt = QHBoxLayout(self)
         lyt.setContentsMargins(0, 0, 0, 0)
-        lyt.setMargin(0)
 
         self.edit = QLineEdit(self)
         self.btn = QPushButton("...", parent=self)
         self.btn.setMaximumSize(QSize(100, 40))
         self.btn.clicked.connect(self.get_file)
 
         lyt.addWidget(self.edit)
@@ -182,15 +181,15 @@
         else:
             settings.include_adaptor_wheels = False
 
     def activate_frame_override_changed(self, state):
         """
         Set the activated/deactivated status of the Frame override text box
         """
-        self.frame_override_txt.setEnabled(state == Qt.Checked)
+        self.frame_override_txt.setEnabled(Qt.CheckState(state) == Qt.Checked)
 
     def output_file_path_changed(self):
         """
         Update the output file path display if any of the name, folder or
         extension are changed in the UI.
         """
         folder = self.output_folder_text.text()
```

### Comparing `deadline_cloud_for_keyshot-0.1.1/LICENSE` & `deadline_cloud_for_keyshot-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.1/README.md` & `deadline_cloud_for_keyshot-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 
 ## Submitter
 
 This package provides a KeyShot plugin script that creates jobs for AWS Deadline Cloud using the [AWS Deadline Cloud client library][deadline-cloud-client]. Based on the loaded scene it determines the files required, allows the user to specify render options with KeyShot's render interface, and builds an [OpenJD template][openjd] that defines the workflow.
 
 ### Using the KeyShot Submitter
 
-1. Install deadline-cloud and PySide2
+1. Install deadline and Pyside6
+    - e.g. `pip install deadline[gui]`
 2. Copy or link the file `deadline-cloud-for-keyshot/keyshot_script/Submit to AWS Deadline Cloud.py` to the KeyShot scripts folder.
     - e.g. On Windows `C:/Users/<USER>/Documents/KeyShot 12/Scripts`
 3. Set the following environment variables
     - Set the environment variable `DEADLINE_PYTHON` as the path to the Python installation where deadline-cloud and PySide2 were installed in step 1.
       - e.g. On Windows if using Python 3.10 it might be `set DEADLINE_PYTHON=C:/Users/<USER>/AppData/Local/Programs/Python/Python310/python`
     - Set the environment variable `DEADLINE_KEYSHOT` as the path to the `<PATH TO>/deadline-cloud-for-keyshot/src/deadline/keyshot_submitter` folder
       - e.g. On Windows if the source was on the user's desktop it might be  `set DEADLINE_KEYSHOT=C:/Users/<USER>/Desktop/deadline-cloud-for-keyshot/src/deadline/keyshot_submitter`
```

### Comparing `deadline_cloud_for_keyshot-0.1.1/hatch.toml` & `deadline_cloud_for_keyshot-0.1.2/hatch.toml`

 * *Files identical despite different names*

### Comparing `deadline_cloud_for_keyshot-0.1.1/pyproject.toml` & `deadline_cloud_for_keyshot-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 pretty = true
 # Tell mypy that there's a namspace package src/deadline
 namespace_packages = true
 explicit_package_bases = true
 mypy_path = "src"
 
 [[tool.mypy.overrides]]
-module = ["lux.*", "PySide2.*"]
+module = ["lux.*", "qtpy.*"]
 ignore_missing_imports = true
 
 [tool.ruff]
 ignore = [
   "E501",
 ]
 line-length = 100
```

### Comparing `deadline_cloud_for_keyshot-0.1.1/PKG-INFO` & `deadline_cloud_for_keyshot-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: deadline-cloud-for-keyshot
-Version: 0.1.1
+Version: 0.1.2
 Summary: AWS Deadline Cloud for KeyShot
 Project-URL: Homepage, https://github.com/aws-deadline/deadline-cloud-for-keyshot
 Project-URL: Source, https://github.com/aws-deadline/deadline-cloud-for-keyshot
 Author: Amazon Web Services
 License-Expression: Apache-2.0
 License-File: LICENSE
 License-File: NOTICE
@@ -48,15 +48,16 @@
 
 ## Submitter
 
 This package provides a KeyShot plugin script that creates jobs for AWS Deadline Cloud using the [AWS Deadline Cloud client library][deadline-cloud-client]. Based on the loaded scene it determines the files required, allows the user to specify render options with KeyShot's render interface, and builds an [OpenJD template][openjd] that defines the workflow.
 
 ### Using the KeyShot Submitter
 
-1. Install deadline-cloud and PySide2
+1. Install deadline and Pyside6
+    - e.g. `pip install deadline[gui]`
 2. Copy or link the file `deadline-cloud-for-keyshot/keyshot_script/Submit to AWS Deadline Cloud.py` to the KeyShot scripts folder.
     - e.g. On Windows `C:/Users/<USER>/Documents/KeyShot 12/Scripts`
 3. Set the following environment variables
     - Set the environment variable `DEADLINE_PYTHON` as the path to the Python installation where deadline-cloud and PySide2 were installed in step 1.
       - e.g. On Windows if using Python 3.10 it might be `set DEADLINE_PYTHON=C:/Users/<USER>/AppData/Local/Programs/Python/Python310/python`
     - Set the environment variable `DEADLINE_KEYSHOT` as the path to the `<PATH TO>/deadline-cloud-for-keyshot/src/deadline/keyshot_submitter` folder
       - e.g. On Windows if the source was on the user's desktop it might be  `set DEADLINE_KEYSHOT=C:/Users/<USER>/Desktop/deadline-cloud-for-keyshot/src/deadline/keyshot_submitter`
```

