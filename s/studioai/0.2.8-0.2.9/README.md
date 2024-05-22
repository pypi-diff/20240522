# Comparing `tmp/studioai-0.2.8.tar.gz` & `tmp/studioai-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "studioai-0.2.8.tar", max compression
+gzip compressed data, was "studioai-0.2.9.tar", max compression
```

## Comparing `studioai-0.2.8.tar` & `studioai-0.2.9.tar`

### file list

```diff
@@ -1,34 +1,36 @@
--rw-r--r--   0        0        0     2701 2023-08-22 22:09:19.823223 studioai-0.2.8/README.md
--rw-r--r--   0        0        0     2383 2023-09-30 02:43:03.555928 studioai-0.2.8/pyproject.toml
--rw-r--r--   0        0        0     1822 2023-09-01 07:36:51.825301 studioai-0.2.8/studioai/__init__.py
--rw-r--r--   0        0        0     2290 2023-09-17 21:52:15.507020 studioai-0.2.8/studioai/container.py
--rw-r--r--   0        0        0     2538 2023-08-26 09:19:55.518354 studioai-0.2.8/studioai/data/__init__.py
--rw-r--r--   0        0        0     2205 2023-08-28 00:19:36.951588 studioai-0.2.8/studioai/data/credit.py
--rw-r--r--   0        0        0     3627 2023-08-22 22:30:38.893223 studioai-0.2.8/studioai/data/dataclass.py
--rw-r--r--   0        0        0    14340 2023-09-30 01:01:19.445928 studioai-0.2.8/studioai/data/dataset.py
--rw-r--r--   0        0        0    23824 2023-08-23 10:50:21.043223 studioai-0.2.8/studioai/data/distribution.py
--rw-r--r--   0        0        0     1662 2023-09-27 07:35:06.849551 studioai-0.2.8/studioai/data/prep/__init__.py
--rw-r--r--   0        0        0     2849 2023-09-28 07:15:10.743966 studioai-0.2.8/studioai/data/prep/base.py
--rw-r--r--   0        0        0     4544 2023-09-28 12:59:16.423966 studioai-0.2.8/studioai/data/prep/encode.py
--rw-r--r--   0        0        0        0 2023-08-22 21:55:50.003223 studioai-0.2.8/studioai/py.typed
--rw-r--r--   0        0        0     1662 2023-08-22 23:34:53.583223 studioai-0.2.8/studioai/service/__init__.py
--rw-r--r--   0        0        0    12080 2023-08-26 09:43:39.918354 studioai-0.2.8/studioai/service/io.py
--rw-r--r--   0        0        0     1662 2023-08-22 22:28:55.043223 studioai-0.2.8/studioai/stats/__init__.py
--rw-r--r--   0        0        0     1662 2023-08-22 23:30:50.003223 studioai-0.2.8/studioai/stats/descriptive/__init__.py
--rw-r--r--   0        0        0     4431 2023-08-23 09:25:01.963223 studioai-0.2.8/studioai/stats/descriptive/base.py
--rw-r--r--   0        0        0     2516 2023-08-26 15:04:10.518355 studioai-0.2.8/studioai/stats/descriptive/categorical.py
--rw-r--r--   0        0        0     3111 2023-08-26 15:03:56.888355 studioai-0.2.8/studioai/stats/descriptive/continuous.py
--rw-r--r--   0        0        0     8396 2023-08-28 10:28:40.811797 studioai-0.2.8/studioai/stats/descriptive/summary.py
--rw-r--r--   0        0        0     1662 2023-08-22 23:34:53.223223 studioai-0.2.8/studioai/stats/inferential/__init__.py
--rw-r--r--   0        0        0     9742 2023-09-30 06:22:05.855925 studioai-0.2.8/studioai/stats/inferential/association.py
--rw-r--r--   0        0        0     4445 2023-09-30 05:52:29.795929 studioai-0.2.8/studioai/stats/inferential/base.py
--rw-r--r--   0        0        0     6105 2023-09-30 05:52:44.765929 studioai-0.2.8/studioai/stats/inferential/centrality.py
--rw-r--r--   0        0        0    11519 2023-09-30 06:20:34.135926 studioai-0.2.8/studioai/stats/inferential/correlation.py
--rw-r--r--   0        0        0     6347 2023-09-30 05:58:05.765930 studioai-0.2.8/studioai/stats/inferential/gof.py
--rw-r--r--   0        0        0     5142 2023-09-30 05:52:09.495928 studioai-0.2.8/studioai/stats/inferential/independence.py
--rw-r--r--   0        0        0     3175 2023-08-22 23:49:09.503223 studioai-0.2.8/studioai/stats/inferential/profile.py
--rw-r--r--   0        0        0     5116 2023-09-30 04:56:57.355929 studioai-0.2.8/studioai/stats/inferential/test.py
--rw-r--r--   0        0        0     5502 2023-08-28 09:49:30.461795 studioai-0.2.8/studioai/visual/base.py
--rw-r--r--   0        0        0    45498 2023-09-30 05:35:46.545928 studioai-0.2.8/studioai/visual/visualizer.py
--rw-r--r--   0        0        0     3550 2023-09-30 06:29:19.293265 studioai-0.2.8/setup.py
--rw-r--r--   0        0        0     3730 2023-09-30 06:29:19.293850 studioai-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     2701 2023-08-22 22:09:19.823223 studioai-0.2.9/README.md
+-rw-r--r--   0        0        0     2383 2023-09-30 06:30:57.185928 studioai-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0     4482 2023-10-19 23:01:43.333299 studioai-0.2.9/studioai/__init__.py
+-rw-r--r--   0        0        0     1840 2023-10-19 23:34:07.013300 studioai-0.2.9/studioai/analysis/__init__.py
+-rw-r--r--   0        0        0     2302 2023-10-19 23:34:07.013300 studioai-0.2.9/studioai/analysis/container.py
+-rw-r--r--   0        0        0     1662 2023-10-19 23:24:36.953302 studioai-0.2.9/studioai/analysis/explore/__init__.py
+-rw-r--r--   0        0        0    14385 2023-10-19 23:23:02.793304 studioai-0.2.9/studioai/analysis/explore/eda.py
+-rw-r--r--   0        0        0     2216 2023-10-19 23:51:42.073299 studioai-0.2.9/studioai/analysis/explore/example.py
+-rw-r--r--   0        0        0     1662 2023-08-22 22:28:55.043223 studioai-0.2.9/studioai/analysis/stats/__init__.py
+-rw-r--r--   0        0        0     1662 2023-08-22 23:30:50.003223 studioai-0.2.9/studioai/analysis/stats/descriptive/__init__.py
+-rw-r--r--   0        0        0     4431 2023-08-23 09:25:01.963223 studioai-0.2.9/studioai/analysis/stats/descriptive/base.py
+-rw-r--r--   0        0        0     2501 2023-10-19 23:02:47.803300 studioai-0.2.9/studioai/analysis/stats/descriptive/categorical.py
+-rw-r--r--   0        0        0     3096 2023-10-19 23:02:47.873299 studioai-0.2.9/studioai/analysis/stats/descriptive/continuous.py
+-rw-r--r--   0        0        0     8400 2023-10-19 23:43:17.283300 studioai-0.2.9/studioai/analysis/stats/descriptive/summary.py
+-rw-r--r--   0        0        0     1662 2023-10-19 22:54:48.153299 studioai-0.2.9/studioai/analysis/stats/distribution/__init__.py
+-rw-r--r--   0        0        0    23809 2023-10-19 23:02:47.763300 studioai-0.2.9/studioai/analysis/stats/distribution/generate.py
+-rw-r--r--   0        0        0     1662 2023-08-22 23:34:53.223223 studioai-0.2.9/studioai/analysis/stats/inferential/__init__.py
+-rw-r--r--   0        0        0     9772 2023-10-19 23:34:07.013300 studioai-0.2.9/studioai/analysis/stats/inferential/association.py
+-rw-r--r--   0        0        0     4456 2023-10-20 00:01:04.313299 studioai-0.2.9/studioai/analysis/stats/inferential/base.py
+-rw-r--r--   0        0        0     6153 2023-10-19 23:34:07.013300 studioai-0.2.9/studioai/analysis/stats/inferential/centrality.py
+-rw-r--r--   0        0        0    11578 2023-10-20 00:01:25.163299 studioai-0.2.9/studioai/analysis/stats/inferential/correlation.py
+-rw-r--r--   0        0        0     6386 2023-10-19 23:34:07.013300 studioai-0.2.9/studioai/analysis/stats/inferential/gof.py
+-rw-r--r--   0        0        0     5181 2023-10-19 23:34:07.013300 studioai-0.2.9/studioai/analysis/stats/inferential/independence.py
+-rw-r--r--   0        0        0     3157 2023-10-19 23:02:48.063300 studioai-0.2.9/studioai/analysis/stats/inferential/profile.py
+-rw-r--r--   0        0        0     5082 2023-10-19 23:56:31.323300 studioai-0.2.9/studioai/analysis/stats/inferential/test.py
+-rw-r--r--   0        0        0     1662 2023-10-19 22:50:02.613300 studioai-0.2.9/studioai/analysis/visualize/__init__.py
+-rw-r--r--   0        0        0     5487 2023-10-19 23:02:47.293300 studioai-0.2.9/studioai/analysis/visualize/base.py
+-rw-r--r--   0        0        0    45507 2023-10-19 23:23:05.323304 studioai-0.2.9/studioai/analysis/visualize/visualizer.py
+-rw-r--r--   0        0        0     1662 2023-09-27 07:35:06.849551 studioai-0.2.9/studioai/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2849 2023-09-28 07:15:10.743966 studioai-0.2.9/studioai/preprocessing/base.py
+-rw-r--r--   0        0        0     4548 2023-10-19 23:44:29.423297 studioai-0.2.9/studioai/preprocessing/encode.py
+-rw-r--r--   0        0        0        0 2023-08-22 21:55:50.003223 studioai-0.2.9/studioai/py.typed
+-rw-r--r--   0        0        0     1662 2023-08-22 23:34:53.583223 studioai-0.2.9/studioai/util/__init__.py
+-rw-r--r--   0        0        0    12080 2023-08-26 09:43:39.918354 studioai-0.2.9/studioai/util/io.py
+-rw-r--r--   0        0        0     3665 2023-10-20 00:04:07.283046 studioai-0.2.9/setup.py
+-rw-r--r--   0        0        0     3730 2023-10-20 00:04:07.283429 studioai-0.2.9/PKG-INFO
```

### Comparing `studioai-0.2.8/README.md` & `studioai-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `studioai-0.2.8/pyproject.toml` & `studioai-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "studioai"
-version = "0.2.8"
+version = "0.2.9"
 description = "Atelier for Artificial Intelligence and Data Science"
 authors = [
     "John James <john.james.ai.studio@gmail.com>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `studioai-0.2.8/studioai/__init__.py` & `studioai-0.2.9/studioai/util/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
-# Python     : 3.10.12                                                                             #
-# Filename   : /studioai/__init__.py                                                               #
+# Python     : 3.10.10                                                                             #
+# Filename   : /studioai/service/__init__.py                                                       #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
-# Created    : Tuesday August 22nd 2023 05:55:50 pm                                                #
-# Modified   : Friday September 1st 2023 03:36:51 am                                               #
+# Created    : Friday May 26th 2023 11:59:46 pm                                                    #
+# Modified   : Tuesday August 22nd 2023 07:34:53 pm                                                #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
-from studioai.container import StudioAIContainer
-
-container = StudioAIContainer()
-container.init_resources()
-container.wire(packages=["studioai.data.dataset"])
```

### Comparing `studioai-0.2.8/studioai/container.py` & `studioai-0.2.9/studioai/analysis/container.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
 # Python     : 3.10.12                                                                             #
-# Filename   : /studioai/container.py                                                              #
+# Filename   : /studioai/analysis/container.py                                                     #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Saturday August 26th 2023 09:31:46 am                                               #
-# Modified   : Sunday September 17th 2023 05:52:15 pm                                              #
+# Modified   : Thursday October 19th 2023 07:34:06 pm                                              #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 """Framework Dependency Container"""
 from dependency_injector import containers, providers
 
-from studioai.visual.visualizer import SeabornCanvas, Visualizer
+from studioai.analysis.visualize.visualizer import SeabornCanvas, Visualizer
 
 
 # ------------------------------------------------------------------------------------------------ #
 #                                    VISUALIZER CONTAINER                                          #
 # ------------------------------------------------------------------------------------------------ #
-class StudioAIContainer(containers.DeclarativeContainer):
+class AnalysisContainer(containers.DeclarativeContainer):
     canvas = providers.Factory(SeabornCanvas)
     visualizer = providers.Factory(Visualizer, canvas=canvas)
```

### Comparing `studioai-0.2.8/studioai/data/credit.py` & `studioai-0.2.9/studioai/analysis/explore/example.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
 # Python     : 3.10.12                                                                             #
-# Filename   : /studioai/data/credit.py                                                            #
+# Filename   : /studioai/analysis/explore/example.py                                               #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Wednesday August 23rd 2023 05:56:02 am                                              #
-# Modified   : Sunday August 27th 2023 08:19:36 pm                                                 #
+# Modified   : Thursday October 19th 2023 07:51:41 pm                                              #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 from __future__ import annotations
 
 import pandas as pd
 
-from studioai.data.dataset import Dataset
+from studioai.analysis.explore.eda import Explorer
 
 
 # ------------------------------------------------------------------------------------------------ #
-class CreditScoreDataset(Dataset):
+class CreditScoreExplorer(Explorer):
     def __init__(self, df: pd.DataFrame) -> None:
         super().__init__(df=df)
 
     @property
     def summary(self) -> pd.DataFrame:
         return (
             self._df[["Gender", "Education", "Marital Status", "Own", "Credit Rating"]]
```

### Comparing `studioai-0.2.8/studioai/data/dataclass.py` & `studioai-0.2.9/studioai/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,76 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
 # Python     : 3.10.12                                                                             #
-# Filename   : /studioai/data/dataclass.py                                                         #
+# Filename   : /studioai/__init__.py                                                               #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
-# Created    : Saturday August 19th 2023 05:28:25 pm                                               #
-# Modified   : Tuesday August 22nd 2023 06:30:38 pm                                                #
+# Created    : Tuesday August 22nd 2023 05:55:50 pm                                                #
+# Modified   : Thursday October 19th 2023 07:01:43 pm                                              #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
+"""Application-Wide Objects Module"""
 from abc import ABC
 from dataclasses import dataclass
 from datetime import datetime
 
 import pandas as pd
+import numpy as np
 
-from studioai.data import IMMUTABLE_TYPES, SEQUENCE_TYPES
+# ------------------------------------------------------------------------------------------------ #
+IMMUTABLE_TYPES: tuple = (
+    str,
+    int,
+    float,
+    bool,
+    np.int16,
+    np.int32,
+    np.int64,
+    np.int8,
+    np.float16,
+    np.float32,
+    np.float64,
+    np.float128,
+)
+SEQUENCE_TYPES: tuple = (
+    list,
+    tuple,
+)
+# ------------------------------------------------------------------------------------------------ #
+NUMERIC_TYPES = [
+    "int16",
+    "int32",
+    "int64",
+    "float16",
+    "float32",
+    "float64",
+    np.int16,
+    np.int32,
+    np.int64,
+    np.int8,
+    np.float16,
+    np.float32,
+    np.float64,
+    np.float128,
+    np.number,
+    int,
+    float,
+    complex,
+]
+
+# ------------------------------------------------------------------------------------------------ #
+NON_NUMERIC_TYPES = ["category", "object"]
 
 
 # ------------------------------------------------------------------------------------------------ #
 @dataclass
 class DataClass(ABC):
     def __repr__(self) -> str:  # pragma: no cover tested, but missing in coverage
         s = "{}({})".format(
```

### Comparing `studioai-0.2.8/studioai/data/dataset.py` & `studioai-0.2.9/studioai/analysis/explore/eda.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
 # Python     : 3.10.11                                                                             #
-# Filename   : /studioai/data/dataset.py                                                           #
+# Filename   : /studioai/data/eda.py                                                               #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Thursday August 10th 2023 08:29:08 pm                                               #
-# Modified   : Friday September 29th 2023 09:01:19 pm                                              #
+# Modified   : Thursday October 19th 2023 07:23:02 pm                                              #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 from __future__ import annotations
 from abc import ABC, abstractproperty
 import logging
 from typing import Callable, Union, List
 
 import pandas as pd
 
-from studioai.stats.descriptive.summary import SummaryStats
-from studioai.visual.visualizer import Visualizer, SeabornCanvas
-from studioai.stats.inferential.test import Inference
+from studioai.analysis.stats.descriptive.summary import SummaryStats
+from studioai.analysis.visualize.visualizer import Visualizer, SeabornCanvas
+from studioai.analysis.stats.inferential.test import Inference
 
 # ------------------------------------------------------------------------------------------------ #
 logger = logging.getLogger(__name__)
 
 
 # ------------------------------------------------------------------------------------------------ #
-#                                            DATASET                                               #
+#                                           EXPLORER                                               #
 # ------------------------------------------------------------------------------------------------ #
-class Dataset(ABC):
-    """Encapsulates numerical and categorical data comprising a set.
+class Explorer(ABC):
+    """Encapsulates the data and behaviors in support of Exploratory Data Analysis
 
     Args:
         df (pd.DataFrame): Pandas DataFrame object.
     """
 
     def __init__(self, df: pd.DataFrame) -> None:
         self._df = df
```

### Comparing `studioai-0.2.8/studioai/data/distribution.py` & `studioai-0.2.9/studioai/analysis/stats/distribution/generate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
 # Python     : 3.10.11                                                                             #
-# Filename   : /studioai/data/distribution.py                                                      #
+# Filename   : /studioai/explore/application/generate.py                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Saturday May 27th 2023 08:56:02 pm                                                  #
-# Modified   : Wednesday August 23rd 2023 06:50:21 am                                              #
+# Modified   : Thursday October 19th 2023 07:02:46 pm                                              #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 """Statistics Module"""
 from __future__ import annotations
 import logging
 from dataclasses import dataclass
 
 from scipy import stats
 import numpy as np
 
-from studioai.data.dataclass import DataClass
+from studioai import DataClass
 
 # ------------------------------------------------------------------------------------------------ #
 logger = logging.getLogger(__name__)
 # ------------------------------------------------------------------------------------------------ #
 NUM_POINTS = 5000
 # ------------------------------------------------------------------------------------------------ #
 #                                    SCIPY DISTRIBUTIONS                                           #
```

### Comparing `studioai-0.2.8/studioai/data/prep/__init__.py` & `studioai-0.2.9/studioai/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `studioai-0.2.8/studioai/data/prep/base.py` & `studioai-0.2.9/studioai/preprocessing/base.py`

 * *Files identical despite different names*

### Comparing `studioai-0.2.8/studioai/data/prep/encode.py` & `studioai-0.2.9/studioai/preprocessing/encode.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
 # Python     : 3.10.12                                                                             #
-# Filename   : /studioai/data/prep/encode.py                                                       #
+# Filename   : /studioai/preprocessing/encode.py                                                   #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Wednesday September 27th 2023 03:35:41 am                                           #
-# Modified   : Thursday September 28th 2023 08:59:16 am                                            #
+# Modified   : Thursday October 19th 2023 07:44:29 pm                                              #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 import pandas as pd
 import numpy as np
 
-from studioai.data.prep.base import Encoder
+from studioai.preprocessing.base import Encoder
 
 
 # ------------------------------------------------------------------------------------------------ #
 class RankFrequencyEncoder(Encoder):
     """Encodes and optionally standardizes data.
 
     This method uses both the value counts as well as the reverse rank of the value
```

### Comparing `studioai-0.2.8/studioai/service/__init__.py` & `studioai-0.2.9/studioai/analysis/stats/inferential/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
-# Python     : 3.10.10                                                                             #
-# Filename   : /studioai/service/__init__.py                                                       #
+# Python     : 3.10.11                                                                             #
+# Filename   : /studioai/stats/inferential/__init__.py                                             #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
-# Created    : Friday May 26th 2023 11:59:46 pm                                                    #
+# Created    : Sunday May 28th 2023 01:21:49 pm                                                    #
 # Modified   : Tuesday August 22nd 2023 07:34:53 pm                                                #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
```

### Comparing `studioai-0.2.8/studioai/service/io.py` & `studioai-0.2.9/studioai/util/io.py`

 * *Files identical despite different names*

### Comparing `studioai-0.2.8/studioai/stats/__init__.py` & `studioai-0.2.9/studioai/analysis/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `studioai-0.2.8/studioai/stats/descriptive/__init__.py` & `studioai-0.2.9/studioai/analysis/stats/descriptive/__init__.py`

 * *Files identical despite different names*

### Comparing `studioai-0.2.8/studioai/stats/descriptive/base.py` & `studioai-0.2.9/studioai/analysis/stats/descriptive/base.py`

 * *Files identical despite different names*

### Comparing `studioai-0.2.8/studioai/stats/descriptive/categorical.py` & `studioai-0.2.9/studioai/analysis/stats/descriptive/categorical.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
 # Python     : 3.10.10                                                                             #
-# Filename   : /studioai/stats/descriptive/categorical.py                                          #
+# Filename   : /studioai/explore/application/stats/descriptive/categorical.py                      #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Thursday June 8th 2023 02:56:56 am                                                  #
-# Modified   : Saturday August 26th 2023 11:04:10 am                                               #
+# Modified   : Thursday October 19th 2023 07:02:46 pm                                              #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 from dataclasses import dataclass
 
 import statistics
 from typing import Union
 
 import pandas as pd
 import numpy as np
 
-from studioai.data.dataclass import DataClass
+from studioai import DataClass
 
 
 # ------------------------------------------------------------------------------------------------ #
 @dataclass
 class CategoricalStats(DataClass):
     name: str  # Name of variable
     length: int  # total  length of variable
```

### Comparing `studioai-0.2.8/studioai/stats/descriptive/continuous.py` & `studioai-0.2.9/studioai/analysis/stats/descriptive/continuous.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
 # Python     : 3.10.10                                                                             #
-# Filename   : /studioai/stats/descriptive/continuous.py                                           #
+# Filename   : /studioai/explore/application/stats/descriptive/continuous.py                       #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Thursday June 8th 2023 02:56:56 am                                                  #
-# Modified   : Saturday August 26th 2023 11:03:56 am                                               #
+# Modified   : Thursday October 19th 2023 07:02:46 pm                                              #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 from dataclasses import dataclass
 from typing import Union
 import logging
 
 import pandas as pd
 import numpy as np
 from scipy import stats
 
-from studioai.data.dataclass import DataClass
+from studioai import DataClass
 
 # ------------------------------------------------------------------------------------------------ #
 logger = logging.getLogger(__name__)
 
 
 # ------------------------------------------------------------------------------------------------ #
 @dataclass
```

### Comparing `studioai-0.2.8/studioai/stats/descriptive/summary.py` & `studioai-0.2.9/studioai/analysis/stats/descriptive/summary.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
 # Python     : 3.10.12                                                                             #
-# Filename   : /studioai/stats/descriptive/summary.py                                              #
+# Filename   : /studioai/analysis/stats/descriptive/summary.py                                     #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Wednesday August 23rd 2023 12:15:10 am                                              #
-# Modified   : Monday August 28th 2023 06:28:40 am                                                 #
+# Modified   : Thursday October 19th 2023 07:43:17 pm                                              #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 """Summary Statistics Module"""
 from typing import Union
 import logging
 
 import pandas as pd
 import numpy as np
 
-from studioai.data import NUMERIC_TYPES, NON_NUMERIC_TYPES
-from studioai.stats.descriptive.base import DescriptiveStats
+from studioai import NUMERIC_TYPES, NON_NUMERIC_TYPES
+from studioai.analysis.stats.descriptive.base import DescriptiveStats
 
 # ------------------------------------------------------------------------------------------------ #
 logger = logging.getLogger(__name__)
 
 
 # ------------------------------------------------------------------------------------------------ #
 class SummaryStats(DescriptiveStats):
```

### Comparing `studioai-0.2.8/studioai/stats/inferential/__init__.py` & `studioai-0.2.9/studioai/analysis/explore/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
-# Python     : 3.10.11                                                                             #
-# Filename   : /studioai/stats/inferential/__init__.py                                             #
+# Python     : 3.10.12                                                                             #
+# Filename   : /studioai/analysis/explore/__init__.py                                              #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
-# Created    : Sunday May 28th 2023 01:21:49 pm                                                    #
-# Modified   : Tuesday August 22nd 2023 07:34:53 pm                                                #
+# Created    : Thursday October 19th 2023 07:24:32 pm                                              #
+# Modified   : Thursday October 19th 2023 07:24:36 pm                                              #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
```

### Comparing `studioai-0.2.8/studioai/stats/inferential/association.py` & `studioai-0.2.9/studioai/analysis/stats/inferential/association.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
 # Python     : 3.10.12                                                                             #
-# Filename   : /studioai/stats/inferential/association.py                                          #
+# Filename   : /studioai/analysis/stats/inferential/association.py                                 #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Friday September 29th 2023 11:52:02 pm                                              #
-# Modified   : Saturday September 30th 2023 02:22:05 am                                            #
+# Modified   : Thursday October 19th 2023 07:34:06 pm                                              #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 from __future__ import annotations
 from dataclasses import dataclass
 
 import pandas as pd
 import numpy as np
 from scipy import stats
 from dependency_injector.wiring import inject, Provide
 
-from studioai.container import StudioAIContainer
-from studioai.visual.visualizer import Visualizer
-from studioai.stats.inferential.base import (
+from studioai.analysis.container import AnalysisContainer
+from studioai.analysis.visualize.visualizer import Visualizer
+from studioai.analysis.stats.inferential.base import (
     StatTestResult,
     StatAnalysis,
 )
 
 
 # ================================================================================================ #
 #                                       KENDALL'S TAU                                              #
@@ -46,15 +46,15 @@
     b: str = None
     n: int = None
     strength: str = None
     pvalue: float = None
     visualizer: Visualizer = None
 
     @inject
-    def __post_init__(self, visualizer: Visualizer = Provide[StudioAIContainer.visualizer]) -> None:
+    def __post_init__(self, visualizer: Visualizer = Provide[AnalysisContainer.visualizer]) -> None:
         self.visualizer = visualizer
 
     def plot(self) -> None:  # pragma: no cover
         self.visualizer.kendallstau(
             data=self.data,
             a=self.a,
             b=self.b,
@@ -158,15 +158,15 @@
     x2dof: float = None
     pvalue: float = None
     expected_freq: np.array = None
     x2result: str = None
     visualizer: Visualizer = None
 
     @inject
-    def __post_init__(self, visualizer: Visualizer = Provide[StudioAIContainer.visualizer]) -> None:
+    def __post_init__(self, visualizer: Visualizer = Provide[AnalysisContainer.visualizer]) -> None:
         self.visualizer = visualizer
 
     def report(self) -> str:
         return f"(X\u00b2 ({self.dof}, n={self.data.shape[0]})={round(self.value,2)}, {self._report_pvalue(self.pvalue)}, phi={round(self.value,2)}."
 
 
 # ------------------------------------------------------------------------------------------------ #
```

### Comparing `studioai-0.2.8/studioai/stats/inferential/base.py` & `studioai-0.2.9/studioai/analysis/stats/inferential/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
 # Python     : 3.10.12                                                                             #
-# Filename   : /studioai/stats/inferential/base.py                                                 #
+# Filename   : /studioai/analysis/stats/inferential/base.py                                        #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Tuesday August 22nd 2023 07:44:59 pm                                                #
-# Modified   : Saturday September 30th 2023 01:52:29 am                                            #
+# Modified   : Thursday October 19th 2023 08:01:04 pm                                              #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 """Base classes used throughout the inferential package."""
 from __future__ import annotations
 from abc import ABC, abstractmethod
 import logging
 from dataclasses import dataclass
 
-from studioai.stats.inferential.profile import StatTestProfile
-from studioai.data.dataclass import DataClass
-from studioai.service.io import IOService
+from studioai.analysis.stats.inferential.profile import StatTestProfile
+from studioai import DataClass
+from studioai.util.io import IOService
 
 # ------------------------------------------------------------------------------------------------ #
 logger = logging.getLogger(__name__)
 # ------------------------------------------------------------------------------------------------ #
 ANALYSIS_TYPES = {
     "univariate": "Univariate",
     "bivariate": "Bivariate",
@@ -51,15 +51,15 @@
     def report(self) -> str:
         """Reports results in APA Style"""
 
     def _report_alpha(self) -> str:
         a = int(self.alpha * 100)
         return f"significant at {a}%."
 
-    def _report_pvalue(self, pvalue: float) -> str:
+    def _report_pvalue(self, pvalue: float) -> str:  # pragma: no cover
         """Rounds the pvalue in accordance with the APA Style Guide 7th Edition"""
         if pvalue < 0.001:
             return "p<.001"
         else:
             return "p=" + str(round(pvalue, 4))
```

### Comparing `studioai-0.2.8/studioai/stats/inferential/centrality.py` & `studioai-0.2.9/studioai/analysis/stats/inferential/centrality.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
 # Python     : 3.10.10                                                                             #
-# Filename   : /studioai/stats/inferential/centrality.py                                           #
+# Filename   : /studioai/analysis/stats/inferential/centrality.py                                  #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Wednesday June 7th 2023 11:41:00 pm                                                 #
-# Modified   : Saturday September 30th 2023 01:52:44 am                                            #
+# Modified   : Thursday October 19th 2023 07:34:06 pm                                              #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 from dataclasses import dataclass
 
 import numpy as np
 from scipy import stats
 from dependency_injector.wiring import inject, Provide
 
-from studioai.container import StudioAIContainer
-from studioai.visual.visualizer import Visualizer
-from studioai.stats.inferential.profile import StatTestProfile
-from studioai.stats.inferential.base import (
+from studioai.analysis.container import AnalysisContainer
+from studioai.analysis.visualize.visualizer import Visualizer
+from studioai.analysis.stats.inferential.profile import StatTestProfile
+from studioai.analysis.stats.inferential.base import (
     StatTestResult,
     StatisticalTest,
 )
 
-from studioai.stats.descriptive.continuous import ContinuousStats
+from studioai.analysis.stats.descriptive.continuous import ContinuousStats
 
 
 # ------------------------------------------------------------------------------------------------ #
 #                                     TEST RESULT                                                  #
 # ------------------------------------------------------------------------------------------------ #
 @dataclass
 class TTestResult(StatTestResult):
@@ -46,15 +46,15 @@
     b: np.ndarray = None
     b_name: str = None
     varname: str = None
     a_stats: ContinuousStats = None
     b_stats: ContinuousStats = None
 
     @inject
-    def __post_init__(self, visualizer: Visualizer = Provide[StudioAIContainer.visualizer]) -> None:
+    def __post_init__(self, visualizer: Visualizer = Provide[AnalysisContainer.visualizer]) -> None:
         self.visualizer = visualizer
 
     def plot(self) -> None:  # pragma: no cover
         title = self.result()
         self.visualizer.ttestplot(statistic=self.value, dof=self.dof, alpha=self.alpha, title=title)
 
     def report(self) -> str:
```

### Comparing `studioai-0.2.8/studioai/stats/inferential/correlation.py` & `studioai-0.2.9/studioai/analysis/stats/inferential/correlation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
 # Python     : 3.10.10                                                                             #
-# Filename   : /studioai/stats/inferential/correlation.py                                          #
+# Filename   : /studioai/analysis/stats/inferential/correlation.py                                 #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Wednesday June 7th 2023 08:15:08 pm                                                 #
-# Modified   : Saturday September 30th 2023 02:20:33 am                                            #
+# Modified   : Thursday October 19th 2023 08:01:24 pm                                              #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 from dataclasses import dataclass
 
 import pandas as pd
 from scipy import stats
 from dependency_injector.wiring import inject, Provide
 
-from studioai.visual.visualizer import Visualizer
-from studioai.container import StudioAIContainer
-from studioai.stats.inferential.profile import StatTestProfile
-from studioai.stats.inferential.base import (
+from studioai.analysis.visualize.visualizer import Visualizer
+from studioai.analysis.container import AnalysisContainer
+from studioai.analysis.stats.inferential.profile import StatTestProfile
+from studioai.analysis.stats.inferential.base import (
     StatTestResult,
     StatisticalTest,
 )
 
 
 # ================================================================================================ #
 #                                  PEARSON'S CORRELATION                                           #
@@ -47,15 +47,15 @@
     b: str = None
     dof: float = None
     strength: str = None
     low_ci: float = (None,)
     high_ci: float = (None,)
 
     @inject
-    def __post_init__(self, visualizer: Visualizer = Provide[StudioAIContainer.visualizer]) -> None:
+    def __post_init__(self, visualizer: Visualizer = Provide[AnalysisContainer.visualizer]) -> None:
         self.visualizer = visualizer
 
     def plot(self) -> None:  # pragma: no cover
         self.visualizer.regplot(data=self.data, x=self.a, y=self.b, title=self.result)
 
     def report(self) -> str:
         return f"Pearson Correlation Test\nr({self.dof})={round(self.value,2)}, {self._report_pvalue(self.pvalue)}"
@@ -117,15 +117,15 @@
     def run(self) -> None:
         """Performs the statistical test and creates a result object."""
 
         try:
             pearson_result = stats.pearsonr(
                 x=self._data[self._a].values, y=self._data[self._b].values, alternative="two-sided"
             )
-        except Exception as e:
+        except Exception as e:  # pragma: no cover
             msg = f"Unable to calculate pearson correlation.\n{e}"
             self._logger.exception(msg)
             raise
 
         r = pearson_result.statistic
         pvalue = pearson_result.pvalue
         confidence_interval = pearson_result.confidence_interval(0.05)
@@ -190,15 +190,15 @@
     data: pd.DataFrame = None
     a: str = None
     b: str = None
     dof: float = None
     n: int = None
 
     @inject
-    def __post_init__(self, visualizer: Visualizer = Provide[StudioAIContainer.visualizer]) -> None:
+    def __post_init__(self, visualizer: Visualizer = Provide[AnalysisContainer.visualizer]) -> None:
         self.visualizer = visualizer
 
     def plot(self) -> None:  # pragma: no cover
         self.visualizer.regplot(data=self.data, x=self.a, y=self.b, title=self.result)
 
     def report(self) -> str:
         return f"Spearman Correlation Test\nr({self.dof})={round(self.value,3)}, {self._report_pvalue(self.pvalue)}"
```

### Comparing `studioai-0.2.8/studioai/stats/inferential/gof.py` & `studioai-0.2.9/studioai/analysis/stats/inferential/gof.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
 # Python     : 3.10.10                                                                             #
-# Filename   : /studioai/stats/inferential/gof.py                                                  #
+# Filename   : /studioai/analysis/stats/inferential/gof.py                                         #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Tuesday June 6th 2023 01:45:05 am                                                   #
-# Modified   : Saturday September 30th 2023 01:58:05 am                                            #
+# Modified   : Thursday October 19th 2023 07:34:06 pm                                              #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 from dataclasses import dataclass
 from typing import Union
 
 import numpy as np
 from scipy import stats
 from dependency_injector.wiring import inject, Provide
 
-from studioai.container import StudioAIContainer
-from studioai.visual.visualizer import Visualizer
-from studioai.stats.inferential.profile import StatTestProfile
-from studioai.stats.inferential.base import (
+from studioai.analysis.container import AnalysisContainer
+from studioai.analysis.visualize.visualizer import Visualizer
+from studioai.analysis.stats.inferential.profile import StatTestProfile
+from studioai.analysis.stats.inferential.base import (
     StatTestResult,
     StatisticalTest,
 )
 
 
 # ------------------------------------------------------------------------------------------------ #
 #                                     TEST RESULT                                                  #
@@ -42,15 +42,15 @@
     name: str = "Kolmogorov-Smirnov Test"
     a: np.ndarray = None
     b: Union[np.ndarray, str] = None
     n: int = None
     advisory: str = None
 
     @inject
-    def __post_init__(self, visualizer: Visualizer = Provide[StudioAIContainer.visualizer]) -> None:
+    def __post_init__(self, visualizer: Visualizer = Provide[AnalysisContainer.visualizer]) -> None:
         self.visualizer = visualizer
 
     def plot(self) -> None:  # pragma: no cover
         self.visualizer.kstestplot(
             statistic=self.value, n=len(self.a), result=self.result, alpha=self.alpha
         )
```

### Comparing `studioai-0.2.8/studioai/stats/inferential/independence.py` & `studioai-0.2.9/studioai/analysis/stats/inferential/independence.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
 # Python     : 3.10.11                                                                             #
-# Filename   : /studioai/stats/inferential/independence.py                                         #
+# Filename   : /studioai/analysis/stats/inferential/independence.py                                #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Monday May 29th 2023 03:00:39 am                                                    #
-# Modified   : Saturday September 30th 2023 01:52:09 am                                            #
+# Modified   : Thursday October 19th 2023 07:34:06 pm                                              #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 from dataclasses import dataclass
 
 import pandas as pd
 from scipy import stats
 from dependency_injector.wiring import inject, Provide
 
-from studioai.container import StudioAIContainer
-from studioai.visual.visualizer import Visualizer
-from studioai.stats.inferential.profile import StatTestProfile
-from studioai.stats.inferential.base import (
+from studioai.analysis.container import AnalysisContainer
+from studioai.analysis.visualize.visualizer import Visualizer
+from studioai.analysis.stats.inferential.profile import StatTestProfile
+from studioai.analysis.stats.inferential.base import (
     StatTestResult,
     StatisticalTest,
 )
 
 
 # ------------------------------------------------------------------------------------------------ #
 #                                     TEST RESULT                                                  #
@@ -40,15 +40,15 @@
     dof: int = None
     data: pd.DataFrame = None
     a: str = None
     b: str = None
     visualizer: Visualizer = None
 
     @inject
-    def __post_init__(self, visualizer: Visualizer = Provide[StudioAIContainer.visualizer]) -> None:
+    def __post_init__(self, visualizer: Visualizer = Provide[AnalysisContainer.visualizer]) -> None:
         self.visualizer = visualizer
 
     def plot(self) -> None:  # pragma: no cover
         self.visualizer.x2testplot(
             statistic=self.value, dof=self.dof, result=self.result, alpha=self.alpha
         )
```

### Comparing `studioai-0.2.8/studioai/stats/inferential/profile.py` & `studioai-0.2.9/studioai/analysis/stats/inferential/profile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
 # Python     : 3.10.12                                                                             #
-# Filename   : /studioai/stats/inferential/profile.py                                              #
+# Filename   : /studioai/explore/application/stats/inferential/profile.py                          #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Tuesday August 22nd 2023 07:45:44 pm                                                #
-# Modified   : Tuesday August 22nd 2023 07:49:09 pm                                                #
+# Modified   : Thursday October 19th 2023 07:02:46 pm                                              #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 from __future__ import annotations
 from dataclasses import dataclass, fields
 
-from studioai.data.dataclass import DataClass
-from studioai.service.io import IOService
+from studioai import DataClass
+from studioai.util.io import IOService
 
 # ------------------------------------------------------------------------------------------------ #
 STAT_CONFIG = "config/stats.yml"
 
 
 # ------------------------------------------------------------------------------------------------ #
 @dataclass
```

### Comparing `studioai-0.2.8/studioai/stats/inferential/test.py` & `studioai-0.2.9/studioai/analysis/stats/inferential/test.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,45 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
 # Python     : 3.10.12                                                                             #
-# Filename   : /studioai/stats/inferential/test.py                                                 #
+# Filename   : /studioai/analysis/stats/inferential/test.py                                        #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Friday September 29th 2023 10:45:53 am                                              #
-# Modified   : Saturday September 30th 2023 12:56:57 am                                            #
+# Modified   : Thursday October 19th 2023 07:56:31 pm                                              #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 import pandas as pd
 import numpy as np
 from typing import Union
 
-from studioai.stats.inferential.independence import (
+from studioai.analysis.stats.inferential.independence import (
     ChiSquareIndependenceTest,
     ChiSquareIndependenceResult,
 )
-from studioai.stats.inferential.association import CramersVAnalysis, CramersV
-from studioai.stats.inferential.association import KendallsTauAnalysis, KendallsTau
-from studioai.stats.inferential.gof import KSTest, KSTestResult
-from studioai.stats.inferential.correlation import PearsonCorrelationTest, PearsonCorrelationResult
-from studioai.stats.inferential.correlation import (
+from studioai.analysis.stats.inferential.association import CramersVAnalysis, CramersV
+from studioai.analysis.stats.inferential.association import KendallsTauAnalysis, KendallsTau
+from studioai.analysis.stats.inferential.gof import KSTest, KSTestResult
+from studioai.analysis.stats.inferential.correlation import (
+    PearsonCorrelationTest,
+    PearsonCorrelationResult,
+)
+from studioai.analysis.stats.inferential.correlation import (
     SpearmanCorrelationTest,
     SpearmanCorrelationResult,
 )
-from studioai.stats.inferential.centrality import TTest, TTestResult
+from studioai.analysis.stats.inferential.centrality import TTest, TTestResult
 
 
 # ------------------------------------------------------------------------------------------------ #
 class Inference:
     """Bundles hypothesis testing into a single class."""
 
     def __init__(self) -> None:
@@ -107,23 +110,19 @@
         return test.result
 
     def ttest(
         self,
         a: np.ndarray,
         b: np.ndarray,
         varname: str = None,
-        a_name: str = None,
-        b_name: str = None,
         alpha: float = 0.05,
         homoscedastic: bool = True,
     ) -> TTestResult:
         test = TTest(
             a=a,
             b=b,
             varname=varname,
-            a_name=a_name,
-            b_name=b_name,
             alpha=alpha,
             homoscedastic=homoscedastic,
         )
         test.run()
         return test.result
```

### Comparing `studioai-0.2.8/studioai/visual/base.py` & `studioai-0.2.9/studioai/analysis/visualize/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
 # Python     : 3.10.12                                                                             #
-# Filename   : /studioai/visual/base.py                                                            #
+# Filename   : /studioai/explore/presentation/base.py                                              #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Saturday August 26th 2023 06:22:05 am                                               #
-# Modified   : Monday August 28th 2023 05:49:30 am                                                 #
+# Modified   : Thursday October 19th 2023 07:02:46 pm                                              #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 from dataclasses import dataclass
 from abc import ABC, abstractmethod
 
 import pandas as pd
 import seaborn as sns
 
-from studioai.data.dataclass import DataClass
+from studioai import DataClass
 
 
 # ------------------------------------------------------------------------------------------------ #
 #                                           COLORS                                                 #
 # ------------------------------------------------------------------------------------------------ #
 @dataclass
 class Colors(DataClass):
```

### Comparing `studioai-0.2.8/studioai/visual/visualizer.py` & `studioai-0.2.9/studioai/analysis/visualize/visualizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/usr/bin/env python3
 # -*- coding:utf-8 -*-
 # ================================================================================================ #
 # Project    : Artificial Intelligence & Data Science Studio                                       #
 # Version    : 0.1.0                                                                               #
 # Python     : 3.10.12                                                                             #
-# Filename   : /studioai/visual/visualizer.py                                                      #
+# Filename   : /studioai/analysis/visualize/visualizer.py                                          #
 # ------------------------------------------------------------------------------------------------ #
 # Author     : John James                                                                          #
 # Email      : john.james.ai.studio@gmail.com                                                      #
 # URL        : https://github.com/john-james-ai/studioai                                           #
 # ------------------------------------------------------------------------------------------------ #
 # Created    : Saturday August 26th 2023 06:25:27 am                                               #
-# Modified   : Saturday September 30th 2023 01:35:45 am                                            #
+# Modified   : Thursday October 19th 2023 07:23:04 pm                                              #
 # ------------------------------------------------------------------------------------------------ #
 # License    : MIT License                                                                         #
 # Copyright  : (c) 2023 John James                                                                 #
 # ================================================================================================ #
 """Wrapper for several Seaborn plotting functions."""
 from __future__ import annotations
 from dataclasses import dataclass
@@ -26,17 +26,17 @@
 import pandas as pd
 import numpy as np
 from scipy import stats
 import seaborn as sns
 import matplotlib.pyplot as plt
 from matplotlib.gridspec import GridSpec
 
-from studioai.visual.base import Canvas, Colors
-from studioai.visual.base import Visualizer as VisualizerABC
-from studioai.data.dataclass import DataClass
+from studioai.analysis.visualize.base import Canvas, Colors
+from studioai.analysis.visualize.base import Visualizer as VisualizerABC
+from studioai import DataClass
 
 # ------------------------------------------------------------------------------------------------ #
 logger = logging.getLogger(__name__)
 
 
 # ------------------------------------------------------------------------------------------------ #
 #                                            PALETTES                                              #
```

### Comparing `studioai-0.2.8/setup.py` & `studioai-0.2.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['studioai',
- 'studioai.data',
- 'studioai.data.prep',
- 'studioai.service',
- 'studioai.stats',
- 'studioai.stats.descriptive',
- 'studioai.stats.inferential',
- 'studioai.visual']
+ 'studioai.analysis',
+ 'studioai.analysis.explore',
+ 'studioai.analysis.stats',
+ 'studioai.analysis.stats.descriptive',
+ 'studioai.analysis.stats.distribution',
+ 'studioai.analysis.stats.inferential',
+ 'studioai.analysis.visualize',
+ 'studioai.preprocessing',
+ 'studioai.util']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'studioai',
-    'version': '0.2.8',
+    'version': '0.2.9',
     'description': 'Atelier for Artificial Intelligence and Data Science',
     'long_description': "# StudioAI\n\n[![PyPI](https://img.shields.io/pypi/v/studioai?style=flat-square)](https://pypi.python.org/pypi/studioai/)\n[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/studioai?style=flat-square)](https://pypi.python.org/pypi/studioai/)\n[![PyPI - License](https://img.shields.io/pypi/l/studioai?style=flat-square)](https://pypi.python.org/pypi/studioai/)\n![Code Coverage](https://img.shields.io/badge/Coverage-100%25-brightgreen.svg)\n\n---\n\n**Documentation**: [https://john-james-ai.github.io/studioai](https://john-james-ai.github.io/studioai)\n\n**Source Code**: [https://github.com/john-james-ai/studioai](https://github.com/john-james-ai/studioai)\n\n**PyPI**: [https://pypi.org/project/studioai/](https://pypi.org/project/studioai/)\n\n---\n\nAtelier for Artificial Intelligence and Data Science\n\n## Installation\n\n```sh\npip install studioai\n```\n\n## Development\n\n* Clone this repository\n* Requirements:\n  * [Poetry](https://python-poetry.org/)\n  * Python 3.7+\n* Create a virtual environment and install the dependencies\n\n```sh\npoetry install\n```\n\n* Activate the virtual environment\n\n```sh\npoetry shell\n```\n\n### Testing\n\n```sh\npytest\n```\n\n### Documentation\n\nThe documentation is automatically generated from the content of the [docs directory](./docs) and from the docstrings\n of the public signatures of the source code. The documentation is updated and published as a [Github project page\n ](https://pages.github.com/) automatically as part each release.\n\n### Releasing\n\nTrigger the [Draft release workflow](https://github.com/john-james-ai/studioai/actions/workflows/draft_release.yml)\n(press _Run workflow_). This will update the changelog & version and create a GitHub release which is in _Draft_ state.\n\nFind the draft release from the\n[GitHub releases](https://github.com/john-james-ai/studioai/releases) and publish it. When\n a release is published, it'll trigger [release](https://github.com/john-james-ai/studioai/blob/master/.github/workflows/release.yml) workflow which creates PyPI\n release and deploys updated documentation.\n\n### Pre-commit\n\nPre-commit hooks run all the auto-formatters (e.g. `black`, `isort`), linters (e.g. `mypy`, `flake8`), and other quality\n checks to make sure the changeset is in good shape before a commit/push happens.\n\nYou can install the hooks with (runs for each commit):\n\n```sh\npre-commit install\n```\n\nOr if you want them to run only for each push:\n\n```sh\npre-commit install -t pre-push\n```\n\nOr if you want e.g. want to run all checks manually for all files:\n\n```sh\npre-commit run --all-files\n```\n\n---\n\nThis project was generated using the [wolt-python-package-cookiecutter](https://github.com/woltapp/wolt-python-package-cookiecutter) template.\n",
     'author': 'John James',
     'author_email': 'john.james.ai.studio@gmail.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://john-james-ai.github.io/studioai',
```

### Comparing `studioai-0.2.8/PKG-INFO` & `studioai-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: studioai
-Version: 0.2.8
+Version: 0.2.9
 Summary: Atelier for Artificial Intelligence and Data Science
 Home-page: https://john-james-ai.github.io/studioai
 License: MIT
 Author: John James
 Author-email: john.james.ai.studio@gmail.com
 Requires-Python: >=3.7.1,<4.0
 Classifier: Development Status :: 4 - Beta
```

