# Comparing `tmp/fgo_api_types-2024.5.2.2.18.47.tar.gz` & `tmp/fgo_api_types-2024.5.22.15.26.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgo_api_types-2024.5.2.2.18.47.tar", max compression
+gzip compressed data, was "fgo_api_types-2024.5.22.15.26.16.tar", max compression
```

## Comparing `fgo_api_types-2024.5.2.2.18.47.tar` & `fgo_api_types-2024.5.22.15.26.16.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    34523 2024-05-02 02:18:30.563126 fgo_api_types-2024.5.2.2.18.47/LICENSE
--rw-r--r--   0        0        0      449 2024-05-02 02:18:30.563126 fgo_api_types-2024.5.2.2.18.47/README.md
--rw-r--r--   0        0        0        0 2024-05-02 02:18:47.351299 fgo_api_types-2024.5.2.2.18.47/fgo_api_types/__init__.py
--rw-r--r--   0        0        0      434 2024-05-02 02:18:47.351299 fgo_api_types-2024.5.2.2.18.47/fgo_api_types/base.py
--rw-r--r--   0        0        0     4511 2024-05-02 02:18:47.351299 fgo_api_types-2024.5.2.2.18.47/fgo_api_types/basic.py
--rw-r--r--   0        0        0     3843 2024-05-02 02:18:47.351299 fgo_api_types-2024.5.2.2.18.47/fgo_api_types/common.py
--rw-r--r--   0        0        0    41947 2024-05-02 02:18:47.351299 fgo_api_types-2024.5.2.2.18.47/fgo_api_types/enums.py
--rw-r--r--   0        0        0   183237 2024-05-02 02:18:47.351299 fgo_api_types-2024.5.2.2.18.47/fgo_api_types/gameenums.py
--rw-r--r--   0        0        0    86981 2024-05-02 02:18:47.351299 fgo_api_types-2024.5.2.2.18.47/fgo_api_types/nice.py
--rw-r--r--   0        0        0    59573 2024-05-02 02:18:47.351299 fgo_api_types-2024.5.2.2.18.47/fgo_api_types/raw.py
--rw-r--r--   0        0        0     4518 2024-05-02 02:18:47.351299 fgo_api_types-2024.5.2.2.18.47/fgo_api_types/rayshift.py
--rw-r--r--   0        0        0    19445 2024-05-02 02:18:47.351299 fgo_api_types-2024.5.2.2.18.47/fgo_api_types/search.py
--rw-r--r--   0        0        0      520 2024-05-02 02:18:47.667302 fgo_api_types-2024.5.2.2.18.47/pyproject.toml
--rw-r--r--   0        0        0     1272 1970-01-01 00:00:00.000000 fgo_api_types-2024.5.2.2.18.47/PKG-INFO
+-rw-r--r--   0        0        0    34523 2024-05-22 15:26:00.800917 fgo_api_types-2024.5.22.15.26.16/LICENSE
+-rw-r--r--   0        0        0      449 2024-05-22 15:26:00.800917 fgo_api_types-2024.5.22.15.26.16/README.md
+-rw-r--r--   0        0        0        0 2024-05-22 15:26:16.417020 fgo_api_types-2024.5.22.15.26.16/fgo_api_types/__init__.py
+-rw-r--r--   0        0        0      434 2024-05-22 15:26:16.417020 fgo_api_types-2024.5.22.15.26.16/fgo_api_types/base.py
+-rw-r--r--   0        0        0     4511 2024-05-22 15:26:16.417020 fgo_api_types-2024.5.22.15.26.16/fgo_api_types/basic.py
+-rw-r--r--   0        0        0     3893 2024-05-22 15:26:16.417020 fgo_api_types-2024.5.22.15.26.16/fgo_api_types/common.py
+-rw-r--r--   0        0        0    41947 2024-05-22 15:26:16.417020 fgo_api_types-2024.5.22.15.26.16/fgo_api_types/enums.py
+-rw-r--r--   0        0        0   183237 2024-05-22 15:26:16.421020 fgo_api_types-2024.5.22.15.26.16/fgo_api_types/gameenums.py
+-rw-r--r--   0        0        0    87076 2024-05-22 15:26:16.421020 fgo_api_types-2024.5.22.15.26.16/fgo_api_types/nice.py
+-rw-r--r--   0        0        0    59573 2024-05-22 15:26:16.421020 fgo_api_types-2024.5.22.15.26.16/fgo_api_types/raw.py
+-rw-r--r--   0        0        0     4518 2024-05-22 15:26:16.421020 fgo_api_types-2024.5.22.15.26.16/fgo_api_types/rayshift.py
+-rw-r--r--   0        0        0    19445 2024-05-22 15:26:16.421020 fgo_api_types-2024.5.22.15.26.16/fgo_api_types/search.py
+-rw-r--r--   0        0        0      520 2024-05-22 15:26:16.765022 fgo_api_types-2024.5.22.15.26.16/pyproject.toml
+-rw-r--r--   0        0        0     1274 1970-01-01 00:00:00.000000 fgo_api_types-2024.5.22.15.26.16/PKG-INFO
```

### Comparing `fgo_api_types-2024.5.2.2.18.47/LICENSE` & `fgo_api_types-2024.5.22.15.26.16/LICENSE`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.5.2.2.18.47/fgo_api_types/basic.py` & `fgo_api_types-2024.5.22.15.26.16/fgo_api_types/basic.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.5.2.2.18.47/fgo_api_types/common.py` & `fgo_api_types-2024.5.22.15.26.16/fgo_api_types/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,14 +114,15 @@
     checkIndvType: Optional[int] = None
     CheckOpponentBuffTypes: Optional[list[NiceBuffType]] = None
     relationId: Optional[NiceBuffRelationOverwrite] = None
     ReleaseText: Optional[str] = None
     DamageRelease: Optional[int] = None
     INDIVIDUALITIE: Optional[NiceTrait] = None
     INDIVIDUALITIE_COUNT_ABOVE: int | None = None
+    INDIVIDUALITIE_COUNT_BELOW: int | None = None
     INDIVIDUALITIE_AND: list[NiceTrait] | None = None
     INDIVIDUALITIE_OR: list[NiceTrait] | None = None
     UpBuffRateBuffIndiv: Optional[list[NiceTrait]] = None
     HP_LOWER: Optional[int] = None
     HP_HIGHER: int | None = None
     CounterMessage: str | None = None
     avoidanceText: str | None = None
```

### Comparing `fgo_api_types-2024.5.2.2.18.47/fgo_api_types/enums.py` & `fgo_api_types-2024.5.22.15.26.16/fgo_api_types/enums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.5.2.2.18.47/fgo_api_types/gameenums.py` & `fgo_api_types-2024.5.22.15.26.16/fgo_api_types/gameenums.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.5.2.2.18.47/fgo_api_types/nice.py` & `fgo_api_types-2024.5.22.15.26.16/fgo_api_types/nice.py`

 * *Files 0% similar despite different names*

```diff
@@ -1030,14 +1030,17 @@
 class NiceServantTrait(BaseModel):
     idx: int
     trait: list[NiceTrait]
     limitCount: int
     condType: Optional[NiceCondType] = None
     condId: Optional[int] = None
     condNum: Optional[int] = None
+    eventId: int | None = None
+    startedAt: int | None = None
+    endedAt: int | None = None
 
 
 class NiceLoreCommentAdd(BaseModel):
     idx: int
     condType: NiceCondType
     condValues: list[int]
     condValue2: int = Field(
```

### Comparing `fgo_api_types-2024.5.2.2.18.47/fgo_api_types/raw.py` & `fgo_api_types-2024.5.22.15.26.16/fgo_api_types/raw.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.5.2.2.18.47/fgo_api_types/rayshift.py` & `fgo_api_types-2024.5.22.15.26.16/fgo_api_types/rayshift.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.5.2.2.18.47/fgo_api_types/search.py` & `fgo_api_types-2024.5.22.15.26.16/fgo_api_types/search.py`

 * *Files identical despite different names*

### Comparing `fgo_api_types-2024.5.2.2.18.47/pyproject.toml` & `fgo_api_types-2024.5.22.15.26.16/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgo-api-types"
-version = "2024.05.02.02.18.47"
+version = "2024.05.22.15.26.16"
 description = "Provide Pydantic types from FGO API"
 authors = ["squaresmile <squaresmile@protonmail.com>"]
 readme = "README.md"
 homepage = "https://api.atlasacademy.io"
 repository = "https://github.com/atlasacademy/fgo-game-data-api"
 
 [tool.poetry.dependencies]
```

### Comparing `fgo_api_types-2024.5.2.2.18.47/PKG-INFO` & `fgo_api_types-2024.5.22.15.26.16/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fgo-api-types
-Version: 2024.5.2.2.18.47
+Version: 2024.5.22.15.26.16
 Summary: Provide Pydantic types from FGO API
 Home-page: https://api.atlasacademy.io
 Author: squaresmile
 Author-email: squaresmile@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

