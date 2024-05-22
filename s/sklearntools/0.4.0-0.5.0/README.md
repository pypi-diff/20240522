# Comparing `tmp/sklearntools-0.4.0.tar.gz` & `tmp/sklearntools-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearntools-0.4.0.tar", last modified: Tue May 21 15:34:04 2024, max compression
+gzip compressed data, was "sklearntools-0.5.0.tar", last modified: Wed May 22 02:08:51 2024, max compression
```

## Comparing `sklearntools-0.4.0.tar` & `sklearntools-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 15:34:04.042734 sklearntools-0.4.0/
--rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-21 15:34:04.041021 sklearntools-0.4.0/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      761 2024-05-21 10:29:01.000000 sklearntools-0.4.0/README.rst
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-21 15:34:04.042925 sklearntools-0.4.0/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)      882 2024-05-21 15:33:58.000000 sklearntools-0.4.0/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 15:34:04.030913 sklearntools-0.4.0/sklearntools/
--rw-r--r--   0 summy      (501) staff       (20)     6978 2024-05-21 15:31:57.000000 sklearntools-0.4.0/sklearntools/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 15:34:04.039939 sklearntools-0.4.0/sklearntools.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-21 15:34:03.000000 sklearntools-0.4.0/sklearntools.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      258 2024-05-21 15:34:03.000000 sklearntools-0.4.0/sklearntools.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-21 15:34:03.000000 sklearntools-0.4.0/sklearntools.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-21 10:55:39.000000 sklearntools-0.4.0/sklearntools.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       32 2024-05-21 15:34:03.000000 sklearntools-0.4.0/sklearntools.egg-info/requires.txt
--rw-r--r--   0 summy      (501) staff       (20)       13 2024-05-21 15:34:03.000000 sklearntools-0.4.0/sklearntools.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-22 02:08:51.820881 sklearntools-0.5.0/
+-rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-22 02:08:51.818421 sklearntools-0.5.0/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      761 2024-05-21 10:29:01.000000 sklearntools-0.5.0/README.rst
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-22 02:08:51.821253 sklearntools-0.5.0/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)      882 2024-05-22 02:08:45.000000 sklearntools-0.5.0/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-22 02:08:51.810938 sklearntools-0.5.0/sklearntools/
+-rw-r--r--   0 summy      (501) staff       (20)     5973 2024-05-22 02:05:53.000000 sklearntools-0.5.0/sklearntools/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-22 02:08:51.815395 sklearntools-0.5.0/sklearntools.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-22 02:08:51.000000 sklearntools-0.5.0/sklearntools.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      258 2024-05-22 02:08:51.000000 sklearntools-0.5.0/sklearntools.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-22 02:08:51.000000 sklearntools-0.5.0/sklearntools.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-22 02:08:51.000000 sklearntools-0.5.0/sklearntools.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       32 2024-05-22 02:08:51.000000 sklearntools-0.5.0/sklearntools.egg-info/requires.txt
+-rw-r--r--   0 summy      (501) staff       (20)       13 2024-05-22 02:08:51.000000 sklearntools-0.5.0/sklearntools.egg-info/top_level.txt
```

### Comparing `sklearntools-0.4.0/PKG-INFO` & `sklearntools-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearntools
-Version: 0.4.0
+Version: 0.5.0
 Summary: Tools of sklearn.
 Home-page: https://gitee.com/summry/sklearntools
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sklearn
 Platform: UNKNOWN
```

### Comparing `sklearntools-0.4.0/README.rst` & `sklearntools-0.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `sklearntools-0.4.0/setup.py` & `sklearntools-0.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 setup(
     name='sklearntools',
     packages=['sklearntools'],
     description="Tools of sklearn.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.4.0',
+    version='0.5.0',
     install_requires=[
         'joblib>=1.1.0',
         'scikit-learn>=1.0',
     ],
     url='https://gitee.com/summry/sklearntools',
     author='summy',
     author_email='xiazhongbiao@126.com',
```

### Comparing `sklearntools-0.4.0/sklearntools/__init__.py` & `sklearntools-0.5.0/sklearntools/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,31 @@
-from enum import Enum
-from typing import Union
 from collections import Counter
 from joblib import Parallel, delayed
 from sklearn.model_selection import ParameterGrid
 from sklearn.model_selection import train_test_split
-from sklearn.metrics import accuracy_score, mean_squared_error
+from sklearn.metrics import accuracy_score, mean_squared_error, root_mean_squared_error
 from logging import basicConfig, INFO, getLogger
 
 logger = getLogger(__name__)
 basicConfig(level=INFO, format='[%(asctime)s %(levelname)s] %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
 
 
-class ModelType(Enum):
-	CLASSIFY = 'classify'
-	REGRESS = 'regress'
-
-
-def train_evaluate(model, X_train, X_test, y_train, y_test, describe='准确率', return_predict=False,
-				   mode_type: Union[ModelType, str] = None):
+def train_evaluate(model, X_train, X_test, y_train, y_test, describe='准确率', return_predict=False, evaluate_func=None):
 	"""Train and evaluate a model
 
 	Parameters
     ----------
 	model: Model
 	X_train:
 	X_test:
 	y_train:
 	y_test:
 	describe:
 	return_predict: whether return predictions
-	mode_type:
+	evaluate_func: accuracy_score, mean_squared_error, root_mean_squared_error etc.
 
 	Returns
     -------
     score or (score, predictions)
 
     Examples
     --------
@@ -45,46 +37,44 @@
     >>> X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3)
     >>> model = RandomForestClassifier(n_estimators=837, bootstrap=False)
     >>> train_evaluate(model, X_train, X_test, y_train, y_test)
     0.88
 	"""
 
 	model.fit(X_train, y_train)
-	mode_type = mode_type or ModelType.CLASSIFY.value
-	mode_type = mode_type.value if isinstance(mode_type, ModelType) else mode_type
-
 	prediction = model.predict(X_test)
-	if mode_type.lower() == ModelType.CLASSIFY.value:
-		score = accuracy_score(y_test, prediction)
+	evaluate_func = evaluate_func or (accuracy_score if 'classifier' == model._estimator_type else mean_squared_error)
+	score = evaluate_func(y_test, prediction)
+	if evaluate_func == accuracy_score:
 		logger.info(f'{describe}: {score:.1%}')
-		if return_predict:
-			return score, prediction
-		return score
 	else:
-		mse = mean_squared_error(y_test, prediction)
-		logger.info(f'{"MSE" if "准确率" == describe else describe}: {mse:.2f}')
-		if return_predict:
-			return mse, prediction
-		return mse
+		if '准确率' == describe:
+			if evaluate_func == mean_squared_error:
+				describe = 'MSE'
+			elif evaluate_func == root_mean_squared_error:
+				describe = 'RMSE'
+		logger.info(f'{describe}: {score:.2f}')
+	if return_predict:
+		return score, prediction
+	return score
 
 
-def train_evaluate_split(model, X, y, test_size=0.2, describe='准确率', return_predict=False, random_state=42,
-						 mode_type: Union[ModelType, str] = None):
+def train_evaluate_split(model, X, y, test_size=0.2, describe='准确率', return_predict=False, random_state=42, evaluate_func=None):
 	"""Train and evaluate a model
 
 	Parameters
 	----------
 	model: Model
 	X:
 	y:
 	test_size:
 	describe:
 	return_predict: whether return predictions
 	random_state:
-	mode_type:
+	evaluate_func: accuracy_score, mean_squared_error, root_mean_squared_error etc.
 
 	Returns
 	-------
 	score or (score, predictions)
 
 	Examples
 	--------
@@ -93,115 +83,96 @@
 	>>> from sklearntools import train_evaluate_split
 	>>> X, y = np.arange(20).reshape((10, 2)), range(10)
 	>>> model = RandomForestClassifier(n_estimators=837, bootstrap=False)
 	>>> train_evaluate_split(model, X, y, test_size=0.2)
 	0.88
 	"""
 	X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=test_size, random_state=random_state)
-	return train_evaluate(model, X_train, X_test, y_train, y_test, describe, return_predict, mode_type)
+	return train_evaluate(model, X_train, X_test, y_train, y_test, describe, return_predict, evaluate_func)
 
 
-def search_model_params(model_name, X_train, X_test, y_train, y_test, param_grid, result_num=5, iter_num=8,
-						mode_type: Union[ModelType, str] = None):
-	"""Train and evaluate a model
+def search_model_params(model_name, X_train, X_test, y_train, y_test, param_grid, result_num=5, iter_num=8):
+	"""
+	Train and evaluate a model
 
 	Parameters
 	----------
 	model_name:
 	X_train:
 	X_test:
 	y_train:
 	y_test:
 	param_grid:
 	result_num:
 	iter_num:
-	mode_type:
 
 	Examples
 	--------
 	>>> import numpy as np
 	>>> from sklearn.ensemble import RandomForestClassifier
 	>>> from sklearn.model_selection import train_test_split
 	>>> from sklearntools import search_model_params
 	>>> X, y = np.arange(20).reshape((10, 2)), range(10)
 	>>> X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3)
 	>>> param_grid = {'n_estimators': np.arange(800, 820, 1), 'bootstrap': [False, True]}
 	>>> search_model_params(RandomForestClassifier, X_train, X_test, y_train, y_test, param_grid, result_num=3)
 	"""
-
-	mode_type = mode_type or ModelType.CLASSIFY.value
-	mode_type = mode_type.value if isinstance(mode_type, ModelType) else mode_type
-	if mode_type.lower() == ModelType.CLASSIFY.value:
-		results = Parallel(n_jobs=-1)(
-			delayed(_search_params)(model_name, X_train, X_test, y_train, y_test, params) for params in
-			ParameterGrid(param_grid))
-		results = sorted(results, key=lambda x: x[1], reverse=True)[:result_num]
-		for param, score in results:
-			logger.info(f'param: {param}\t准确率: {score:.1%}')
-			_evaluate_params(model_name, X_train, X_test, y_train, y_test, param, iter_num)
-	else:
-		results = Parallel(n_jobs=-1)(
-			delayed(_search_params_mse)(model_name, X_train, X_test, y_train, y_test, params) for params in
-			ParameterGrid(param_grid))
-		results = sorted(results, key=lambda x: x[1])[:result_num]
-		for param, mse in results:
-			logger.info(f'param: {param}\tMSE: {mse:.2f}')
-			_evaluate_params_mse(model_name, X_train, X_test, y_train, y_test, param, iter_num)
+	classifier = 'classifier' in model_name.__name__.lower()
+	results = Parallel(n_jobs=-1)(
+		delayed(_search_params)(model_name, classifier, X_train, X_test, y_train, y_test, params) for params in
+		ParameterGrid(param_grid)
+	)
+	results = sorted(results, key=lambda x: x[1], reverse=classifier)[:result_num]
+	for param, score in results:
+		if classifier:
+			logger.info(f'param: {param}\tscore: {score:.1%}')
+		else:
+			logger.info(f'param: {param}\tscore: {score:.4f}')
+		_evaluate_params(model_name, classifier, X_train, X_test, y_train, y_test, param, iter_num)
 
 
-def search_model_params_split(model_name, X, y, param_grid, test_size=0.2, result_num=5, iter_num=8, random_state=42,
-							  mode_type: Union[ModelType, str] = None):
+def search_model_params_split(model_name, X, y, param_grid, test_size=0.2, result_num=5, iter_num=8, random_state=42):
 	"""Train and evaluate a model
 
 	Parameters
 	----------
 	model_name:
 	X:
 	y:
 	test_size:
 	param_grid:
 	result_num:
 	iter_num:
 	random_state:
-	mode_type:
 
 	Examples
 	--------
 	>>> import numpy as np
 	>>> from sklearn.ensemble import RandomForestClassifier
 	>>> from sklearntools import search_model_params_split
 	>>> X, y = np.arange(20).reshape((10, 2)), range(10)
 	>>> param_grid = {'n_estimators': np.arange(800, 820, 1), 'bootstrap': [False, True]}
 	>>> search_model_params_split(RandomForestClassifier, X, y, param_grid, test_size=0.2, result_num=3)
 	"""
 	X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=test_size, random_state=random_state)
-	return search_model_params(model_name, X_train, X_test, y_train, y_test, param_grid, result_num, iter_num, mode_type)
+	return search_model_params(model_name, X_train, X_test, y_train, y_test, param_grid, result_num, iter_num)
 
 
-def _search_params(model_name, X_train, X_test, y_train, y_test, params):
+def _search_params(model_name, classifier, X_train, X_test, y_train, y_test, params):
 	model = model_name(**params)
 	model.fit(X_train, y_train)
 	score = model.score(X_test, y_test)
+	if not classifier:
+		score = round(score, 4)
 	return params, score
 
 
-def _search_params_mse(model_name, X_train, X_test, y_train, y_test, params):
-	model = model_name(**params)
-	model.fit(X_train, y_train)
-	mse = mean_squared_error(y_test, model.predict(X_test))
-	return params, mse
-
-
-def _evaluate_params(model_name, X_train, X_test, y_train, y_test, param, iter_num):
+def _evaluate_params(model_name, classifier, X_train, X_test, y_train, y_test, param, iter_num):
 	results = Parallel(n_jobs=-1)(
-		delayed(_search_params)(model_name, X_train, X_test, y_train, y_test, param) for _ in range(iter_num))
+		delayed(_search_params)(model_name, classifier, X_train, X_test, y_train, y_test, param) for _ in range(iter_num))
 	counter = Counter([result[1] for result in results])
-	for score, count in sorted(counter.items(), key=lambda x: x[0], reverse=True):
-		logger.info(f'\tscore: {score}\tcount: {count}')
+	for score, count in sorted(counter.items(), key=lambda x: x[0], reverse=classifier):
+		if classifier:
+			logger.info(f'\tscore: {score:.1%}\tcount: {count}')
+		else:
+			logger.info(f'\tscore: {score:.4f}\tcount: {count}')
 
-
-def _evaluate_params_mse(model_name, X_train, X_test, y_train, y_test, param, iter_num):
-	results = Parallel(n_jobs=-1)(
-		delayed(_search_params_mse)(model_name, X_train, X_test, y_train, y_test, param) for _ in range(iter_num))
-	counter = Counter([result[1] for result in results])
-	for mse, count in sorted(counter.items(), key=lambda x: x[0]):
-		logger.info(f'\tMSE: {mse}\tcount: {count}')
```

### Comparing `sklearntools-0.4.0/sklearntools.egg-info/PKG-INFO` & `sklearntools-0.5.0/sklearntools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearntools
-Version: 0.4.0
+Version: 0.5.0
 Summary: Tools of sklearn.
 Home-page: https://gitee.com/summry/sklearntools
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sklearn
 Platform: UNKNOWN
```

