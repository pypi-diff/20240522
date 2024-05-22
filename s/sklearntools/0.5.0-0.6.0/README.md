# Comparing `tmp/sklearntools-0.5.0.tar.gz` & `tmp/sklearntools-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearntools-0.5.0.tar", last modified: Wed May 22 02:08:51 2024, max compression
+gzip compressed data, was "sklearntools-0.6.0.tar", last modified: Wed May 22 03:14:37 2024, max compression
```

## Comparing `sklearntools-0.5.0.tar` & `sklearntools-0.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-22 02:08:51.820881 sklearntools-0.5.0/
--rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-22 02:08:51.818421 sklearntools-0.5.0/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      761 2024-05-21 10:29:01.000000 sklearntools-0.5.0/README.rst
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-22 02:08:51.821253 sklearntools-0.5.0/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)      882 2024-05-22 02:08:45.000000 sklearntools-0.5.0/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-22 02:08:51.810938 sklearntools-0.5.0/sklearntools/
--rw-r--r--   0 summy      (501) staff       (20)     5973 2024-05-22 02:05:53.000000 sklearntools-0.5.0/sklearntools/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-22 02:08:51.815395 sklearntools-0.5.0/sklearntools.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-22 02:08:51.000000 sklearntools-0.5.0/sklearntools.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      258 2024-05-22 02:08:51.000000 sklearntools-0.5.0/sklearntools.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-22 02:08:51.000000 sklearntools-0.5.0/sklearntools.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-22 02:08:51.000000 sklearntools-0.5.0/sklearntools.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       32 2024-05-22 02:08:51.000000 sklearntools-0.5.0/sklearntools.egg-info/requires.txt
--rw-r--r--   0 summy      (501) staff       (20)       13 2024-05-22 02:08:51.000000 sklearntools-0.5.0/sklearntools.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-22 03:14:37.076444 sklearntools-0.6.0/
+-rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-22 03:14:37.075840 sklearntools-0.6.0/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      761 2024-05-21 10:29:01.000000 sklearntools-0.6.0/README.rst
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-22 03:14:37.076633 sklearntools-0.6.0/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)      882 2024-05-22 03:14:33.000000 sklearntools-0.6.0/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-22 03:14:37.071366 sklearntools-0.6.0/sklearntools/
+-rw-r--r--   0 summy      (501) staff       (20)     8744 2024-05-22 03:14:33.000000 sklearntools-0.6.0/sklearntools/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-22 03:14:37.075091 sklearntools-0.6.0/sklearntools.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-22 03:14:36.000000 sklearntools-0.6.0/sklearntools.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      258 2024-05-22 03:14:36.000000 sklearntools-0.6.0/sklearntools.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-22 03:14:36.000000 sklearntools-0.6.0/sklearntools.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-22 03:14:36.000000 sklearntools-0.6.0/sklearntools.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       32 2024-05-22 03:14:36.000000 sklearntools-0.6.0/sklearntools.egg-info/requires.txt
+-rw-r--r--   0 summy      (501) staff       (20)       13 2024-05-22 03:14:36.000000 sklearntools-0.6.0/sklearntools.egg-info/top_level.txt
```

### Comparing `sklearntools-0.5.0/PKG-INFO` & `sklearntools-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearntools
-Version: 0.5.0
+Version: 0.6.0
 Summary: Tools of sklearn.
 Home-page: https://gitee.com/summry/sklearntools
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sklearn
 Platform: UNKNOWN
```

### Comparing `sklearntools-0.5.0/README.rst` & `sklearntools-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `sklearntools-0.5.0/setup.py` & `sklearntools-0.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 setup(
     name='sklearntools',
     packages=['sklearntools'],
     description="Tools of sklearn.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.5.0',
+    version='0.6.0',
     install_requires=[
         'joblib>=1.1.0',
         'scikit-learn>=1.0',
     ],
     url='https://gitee.com/summry/sklearntools',
     author='summy',
     author_email='xiazhongbiao@126.com',
```

### Comparing `sklearntools-0.5.0/sklearntools/__init__.py` & `sklearntools-0.6.0/sklearntools/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,30 @@
+import numpy as np
 from collections import Counter
 from joblib import Parallel, delayed
 from sklearn.model_selection import ParameterGrid
 from sklearn.model_selection import train_test_split
 from sklearn.metrics import accuracy_score, mean_squared_error, root_mean_squared_error
 from logging import basicConfig, INFO, getLogger
 
 logger = getLogger(__name__)
 basicConfig(level=INFO, format='[%(asctime)s %(levelname)s] %(message)s', datefmt='%Y-%m-%d %H:%M:%S')
 
 
-def train_evaluate(model, X_train, X_test, y_train, y_test, describe='准确率', return_predict=False, evaluate_func=None):
+def train_evaluate(model, X_train, X_test, y_train, y_test, print=True, describe='准确率', return_predict=False, evaluate_func=None):
 	"""Train and evaluate a model
 
 	Parameters
     ----------
 	model: Model
 	X_train:
 	X_test:
 	y_train:
 	y_test:
+	print:
 	describe:
 	return_predict: whether return predictions
 	evaluate_func: accuracy_score, mean_squared_error, root_mean_squared_error etc.
 
 	Returns
     -------
     score or (score, predictions)
@@ -40,37 +42,39 @@
     0.88
 	"""
 
 	model.fit(X_train, y_train)
 	prediction = model.predict(X_test)
 	evaluate_func = evaluate_func or (accuracy_score if 'classifier' == model._estimator_type else mean_squared_error)
 	score = evaluate_func(y_test, prediction)
-	if evaluate_func == accuracy_score:
-		logger.info(f'{describe}: {score:.1%}')
-	else:
-		if '准确率' == describe:
-			if evaluate_func == mean_squared_error:
-				describe = 'MSE'
-			elif evaluate_func == root_mean_squared_error:
-				describe = 'RMSE'
-		logger.info(f'{describe}: {score:.2f}')
+	if print:
+		if evaluate_func == accuracy_score:
+			logger.info(f'{describe}: {score:.1%}')
+		else:
+			if '准确率' == describe:
+				if evaluate_func == mean_squared_error:
+					describe = 'MSE'
+				elif evaluate_func == root_mean_squared_error:
+					describe = 'RMSE'
+			logger.info(f'{describe}: {score:.2f}')
 	if return_predict:
 		return score, prediction
 	return score
 
 
-def train_evaluate_split(model, X, y, test_size=0.2, describe='准确率', return_predict=False, random_state=42, evaluate_func=None):
+def train_evaluate_split(model, X, y, test_size=0.2, print=True, describe='准确率', return_predict=False, random_state=42, evaluate_func=None):
 	"""Train and evaluate a model
 
 	Parameters
 	----------
 	model: Model
 	X:
 	y:
 	test_size:
+	print:
 	describe:
 	return_predict: whether return predictions
 	random_state:
 	evaluate_func: accuracy_score, mean_squared_error, root_mean_squared_error etc.
 
 	Returns
 	-------
@@ -83,15 +87,15 @@
 	>>> from sklearntools import train_evaluate_split
 	>>> X, y = np.arange(20).reshape((10, 2)), range(10)
 	>>> model = RandomForestClassifier(n_estimators=837, bootstrap=False)
 	>>> train_evaluate_split(model, X, y, test_size=0.2)
 	0.88
 	"""
 	X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=test_size, random_state=random_state)
-	return train_evaluate(model, X_train, X_test, y_train, y_test, describe, return_predict, evaluate_func)
+	return train_evaluate(model, X_train, X_test, y_train, y_test, print, describe, return_predict, evaluate_func)
 
 
 def search_model_params(model_name, X_train, X_test, y_train, y_test, param_grid, result_num=5, iter_num=8):
 	"""
 	Train and evaluate a model
 
 	Parameters
@@ -153,14 +157,80 @@
 	>>> param_grid = {'n_estimators': np.arange(800, 820, 1), 'bootstrap': [False, True]}
 	>>> search_model_params_split(RandomForestClassifier, X, y, param_grid, test_size=0.2, result_num=3)
 	"""
 	X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=test_size, random_state=random_state)
 	return search_model_params(model_name, X_train, X_test, y_train, y_test, param_grid, result_num, iter_num)
 
 
+def search_test_size(model, X, y, test_sizes=np.arange(0.15, 0.36, 0.01), random_state=42, evaluate_func=None):
+	"""
+	Examples
+	--------
+	>>> from sklearntools import search_test_size
+	>>> search_test_size(model, X, y, random_state=42, evaluate_func=accuracy_score)
+	"""
+	classifier = 'classifier' == model._estimator_type
+	results = Parallel(n_jobs=-1)(
+		delayed(_search_test_size)(model, X, y, test_size, random_state, evaluate_func) for test_size in test_sizes
+	)
+	for test_size, score in results:
+		if classifier:
+			logger.info(f'test_size: {test_size:.0%} \t score: {score:.2%}')
+		else:
+			logger.info(f'test_size: {test_size:.0%} \t score: {score}:4f')
+
+
+def search_random_state(model, X, y, random_states=np.arange(0, 20, 1), test_size=0.2, evaluate_func=None):
+	"""
+	Examples
+	--------
+	>>> from sklearntools import search_random_state
+	>>> search_random_state(model, X, y, test_size=0.2, evaluate_func=accuracy_score)
+	"""
+	classifier = 'classifier' == model._estimator_type
+	results = Parallel(n_jobs=-1)(
+		delayed(_search_random_state)(model, X, y, test_size, random_state, evaluate_func) for random_state in random_states
+	)
+	for random_state, score in results:
+		if classifier:
+			logger.info(f'random_state: {random_state} \t score: {score:.2%}')
+		else:
+			logger.info(f'random_state: {random_state} \t score: {score}:4f')
+
+
+def search_random_state2(model, X_train, X_test, y_train, y_test, random_states=np.arange(0, 20, 1), evaluate_func=None):
+	"""
+	Examples
+	--------
+	>>> from sklearntools import search_random_state2
+	>>> search_test_size2(model, X_train, X_test, y_train, y_test, random_state=42, evaluate_func=accuracy_score)
+	"""
+	classifier = 'classifier' == model._estimator_type
+	results = Parallel(n_jobs=-1)(
+		delayed(_search_random_state2)(model, X_train, X_test, y_train, y_test, random_state, evaluate_func) for random_state in random_states
+	)
+	for random_state, score in results:
+		if classifier:
+			logger.info(f'random_state: {random_state} \t score: {score:.2%}')
+		else:
+			logger.info(f'random_state: {random_state} \t score: {score}:4f')
+
+
+def _search_test_size(model, X, y, test_size, random_state, evaluate_func):
+	return test_size, train_evaluate_split(model, X, y, test_size, False, None, False, random_state, evaluate_func)
+
+
+def _search_random_state(model, X, y, test_size, random_state, evaluate_func):
+	return random_state, train_evaluate_split(model, X, y, test_size, False, None, False, random_state, evaluate_func)
+
+
+def _search_random_state2(model, X_train, X_test, y_train, y_test, random_state, evaluate_func):
+	return random_state, train_evaluate(model, X_train, X_test, y_train, y_test, False, None, False, evaluate_func)
+
+
 def _search_params(model_name, classifier, X_train, X_test, y_train, y_test, params):
 	model = model_name(**params)
 	model.fit(X_train, y_train)
 	score = model.score(X_test, y_test)
 	if not classifier:
 		score = round(score, 4)
 	return params, score
```

### Comparing `sklearntools-0.5.0/sklearntools.egg-info/PKG-INFO` & `sklearntools-0.6.0/sklearntools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearntools
-Version: 0.5.0
+Version: 0.6.0
 Summary: Tools of sklearn.
 Home-page: https://gitee.com/summry/sklearntools
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sklearn
 Platform: UNKNOWN
```

