# Comparing `tmp/dataramp-1.0.1.dev189.tar.gz` & `tmp/dataramp-1.0.1.dev190.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataramp-1.0.1.dev189.tar", last modified: Thu Feb 22 20:42:33 2024, max compression
+gzip compressed data, was "dataramp-1.0.1.dev190.tar", last modified: Fri Feb 23 14:06:04 2024, max compression
```

## Comparing `dataramp-1.0.1.dev189.tar` & `dataramp-1.0.1.dev190.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 shak      (1000) shak      (1000)        0 2024-02-22 20:42:33.192702 dataramp-1.0.1.dev189/
--rw-rw-r--   0 shak      (1000) shak      (1000)     1067 2024-02-19 09:37:12.000000 dataramp-1.0.1.dev189/LICENSE.txt
--rw-rw-r--   0 shak      (1000) shak      (1000)     1958 2024-02-22 20:42:33.192702 dataramp-1.0.1.dev189/PKG-INFO
--rw-rw-r--   0 shak      (1000) shak      (1000)     1211 2024-02-22 20:32:23.000000 dataramp-1.0.1.dev189/README.md
-drwxrwxr-x   0 shak      (1000) shak      (1000)        0 2024-02-22 20:42:33.192702 dataramp-1.0.1.dev189/dataramp/
--rw-rw-r--   0 shak      (1000) shak      (1000)        0 2024-02-22 20:34:20.000000 dataramp-1.0.1.dev189/dataramp/__init__.py
--rw-rw-r--   0 shak      (1000) shak      (1000)     5079 2024-02-22 20:34:20.000000 dataramp-1.0.1.dev189/dataramp/core.py
--rw-rw-r--   0 shak      (1000) shak      (1000)       74 2024-02-22 20:34:20.000000 dataramp-1.0.1.dev189/dataramp/eval.py
--rw-rw-r--   0 shak      (1000) shak      (1000)     3570 2024-02-22 20:34:20.000000 dataramp-1.0.1.dev189/dataramp/models.py
--rw-rw-r--   0 shak      (1000) shak      (1000)     3727 2024-02-22 20:34:20.000000 dataramp-1.0.1.dev189/dataramp/outlier.py
--rw-rw-r--   0 shak      (1000) shak      (1000)    16008 2024-02-22 20:34:20.000000 dataramp-1.0.1.dev189/dataramp/utils.py
--rw-rw-r--   0 shak      (1000) shak      (1000)       29 2024-02-22 20:42:33.000000 dataramp-1.0.1.dev189/dataramp/version.py
-drwxrwxr-x   0 shak      (1000) shak      (1000)        0 2024-02-22 20:42:33.192702 dataramp-1.0.1.dev189/dataramp.egg-info/
--rw-rw-r--   0 shak      (1000) shak      (1000)     1958 2024-02-22 20:42:33.000000 dataramp-1.0.1.dev189/dataramp.egg-info/PKG-INFO
--rw-rw-r--   0 shak      (1000) shak      (1000)      315 2024-02-22 20:42:33.000000 dataramp-1.0.1.dev189/dataramp.egg-info/SOURCES.txt
--rw-rw-r--   0 shak      (1000) shak      (1000)        1 2024-02-22 20:42:33.000000 dataramp-1.0.1.dev189/dataramp.egg-info/dependency_links.txt
--rw-rw-r--   0 shak      (1000) shak      (1000)        9 2024-02-22 20:42:33.000000 dataramp-1.0.1.dev189/dataramp.egg-info/top_level.txt
--rw-rw-r--   0 shak      (1000) shak      (1000)      811 2024-02-22 18:50:34.000000 dataramp-1.0.1.dev189/pyproject.toml
--rw-rw-r--   0 shak      (1000) shak      (1000)      236 2024-02-22 20:42:33.192702 dataramp-1.0.1.dev189/setup.cfg
--rw-rw-r--   0 shak      (1000) shak      (1000)     1814 2024-02-22 20:08:17.000000 dataramp-1.0.1.dev189/setup.py
+drwxrwxr-x   0 shak      (1000) shak      (1000)        0 2024-02-23 14:06:04.043730 dataramp-1.0.1.dev190/
+-rw-rw-r--   0 shak      (1000) shak      (1000)     1067 2024-02-19 09:37:12.000000 dataramp-1.0.1.dev190/LICENSE.txt
+-rw-rw-r--   0 shak      (1000) shak      (1000)     1958 2024-02-23 14:06:04.043730 dataramp-1.0.1.dev190/PKG-INFO
+-rw-rw-r--   0 shak      (1000) shak      (1000)     1211 2024-02-22 20:32:23.000000 dataramp-1.0.1.dev190/README.md
+drwxrwxr-x   0 shak      (1000) shak      (1000)        0 2024-02-23 14:06:04.043730 dataramp-1.0.1.dev190/dataramp/
+-rw-rw-r--   0 shak      (1000) shak      (1000)        0 2024-02-23 14:05:40.000000 dataramp-1.0.1.dev190/dataramp/__init__.py
+-rw-rw-r--   0 shak      (1000) shak      (1000)     5079 2024-02-23 14:05:40.000000 dataramp-1.0.1.dev190/dataramp/core.py
+-rw-rw-r--   0 shak      (1000) shak      (1000)       74 2024-02-23 14:05:40.000000 dataramp-1.0.1.dev190/dataramp/eval.py
+-rw-rw-r--   0 shak      (1000) shak      (1000)     3570 2024-02-23 14:05:40.000000 dataramp-1.0.1.dev190/dataramp/models.py
+-rw-rw-r--   0 shak      (1000) shak      (1000)     3727 2024-02-23 14:05:40.000000 dataramp-1.0.1.dev190/dataramp/outlier.py
+-rw-rw-r--   0 shak      (1000) shak      (1000)    15640 2024-02-23 14:05:40.000000 dataramp-1.0.1.dev190/dataramp/utils.py
+-rw-rw-r--   0 shak      (1000) shak      (1000)       29 2024-02-23 14:06:03.000000 dataramp-1.0.1.dev190/dataramp/version.py
+drwxrwxr-x   0 shak      (1000) shak      (1000)        0 2024-02-23 14:06:04.043730 dataramp-1.0.1.dev190/dataramp.egg-info/
+-rw-rw-r--   0 shak      (1000) shak      (1000)     1958 2024-02-23 14:06:03.000000 dataramp-1.0.1.dev190/dataramp.egg-info/PKG-INFO
+-rw-rw-r--   0 shak      (1000) shak      (1000)      315 2024-02-23 14:06:04.000000 dataramp-1.0.1.dev190/dataramp.egg-info/SOURCES.txt
+-rw-rw-r--   0 shak      (1000) shak      (1000)        1 2024-02-23 14:06:03.000000 dataramp-1.0.1.dev190/dataramp.egg-info/dependency_links.txt
+-rw-rw-r--   0 shak      (1000) shak      (1000)        9 2024-02-23 14:06:03.000000 dataramp-1.0.1.dev190/dataramp.egg-info/top_level.txt
+-rw-rw-r--   0 shak      (1000) shak      (1000)      811 2024-02-22 18:50:34.000000 dataramp-1.0.1.dev190/pyproject.toml
+-rw-rw-r--   0 shak      (1000) shak      (1000)      236 2024-02-23 14:06:04.043730 dataramp-1.0.1.dev190/setup.cfg
+-rw-rw-r--   0 shak      (1000) shak      (1000)     1814 2024-02-22 20:08:17.000000 dataramp-1.0.1.dev190/setup.py
```

### Comparing `dataramp-1.0.1.dev189/LICENSE.txt` & `dataramp-1.0.1.dev190/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dataramp-1.0.1.dev189/PKG-INFO` & `dataramp-1.0.1.dev190/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataramp
-Version: 1.0.1.dev189
+Version: 1.0.1.dev190
 Summary: A Data science library for data science / data analysis teams
 Home-page: 
 Author: Meshack Kitonga
 Author-email: kitongameshack9@gmail.com
 License: MIT
 Keywords: dataramp,Data Science,Data Analysis
 Classifier: Intended Audience :: Developers
```

### Comparing `dataramp-1.0.1.dev189/README.md` & `dataramp-1.0.1.dev190/README.md`

 * *Files identical despite different names*

### Comparing `dataramp-1.0.1.dev189/dataramp/core.py` & `dataramp-1.0.1.dev190/dataramp/core.py`

 * *Files identical despite different names*

### Comparing `dataramp-1.0.1.dev189/dataramp/models.py` & `dataramp-1.0.1.dev190/dataramp/models.py`

 * *Files identical despite different names*

### Comparing `dataramp-1.0.1.dev189/dataramp/outlier.py` & `dataramp-1.0.1.dev190/dataramp/outlier.py`

 * *Files identical despite different names*

### Comparing `dataramp-1.0.1.dev189/dataramp/utils.py` & `dataramp-1.0.1.dev190/dataramp/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,82 +15,60 @@
 """
 
 if platform.system() == "Darwin":
     plt.switch_backend("TkAgg")
 else:
     plt.switch_backend("Agg")
 
-
-def is_df(obj: Union[pd.DataFrame, pd.Series]) -> bool:
-    """
-    Returns True if `obj` is a pandas DataFrame.
-    Note that this function is simply doing `isinstance(obj, pd.DataFrame)`.
-    Using that `isinstance` check is better for typechecking with mypy,
-    and more explicit - so it's recommended to use that instead of `is_df`.
-
-    Args:
-        obj (Object): Object to test
-    Example::
-
-        >>> x = pd.DataFrame()
-        >>> is_df(x)
-        True
-    """
-    return isinstance(obj, pd.DataFrame)
-
-
 def get_num_vars(df: Union[pd.DataFrame, pd.Series]) -> list:
     """
     Returns the list of numerical features in a DataFrame or Series object.
 
     Parameters:
     -----------
     df : pandas DataFrame or Series object
         The input DataFrame or Series object to extract the numerical features from.
 
     Returns:
     --------
     list
         The list of numerical feature column names in the input DataFrame or Series object.
     """
-    if not is_df(df):
+    if not isinstance(df, (pd.DataFrame, pd.Series)):
         raise TypeError("df must be a pandas DataFrame or Series")
 
     num_vars = df.select_dtypes(include=np.number).columns.tolist()
 
     return num_vars
 
-
 def describe_df(df: Union[pd.DataFrame, pd.Series]) -> pd.DataFrame:
     """
     Describes a DataFrame or Series and returns a DataFrame with the descriptions.
 
     Parameters:
     -----------
     df : pandas DataFrame or Series object
         The input DataFrame or Series object to describe.
 
     Returns:
     --------
     pandas DataFrame
         A DataFrame containing the descriptions of the input DataFrame or Series.
     """
-    if not isinstance(df, pd.DataFrame):
+    if not isinstance(df, (pd.DataFrame, pd.Series)):
         raise TypeError("df must be a pandas DataFrame")
 
     if df.empty:
         raise ValueError("Input DataFrame is empty.")
 
     with tqdm(total=len(df.columns), desc="Describing DataFrame", unit="column") as pbar:
-        # Handle numerical features
         numeric_descr = [
             df[col].describe().apply("{0:.3f}".format)
             for col in df.select_dtypes(include=np.number).columns
         ]
-        # Handle categorical features
         non_numeric_descr = [
             df[col].describe().apply(str) for col in df.select_dtypes(exclude=np.number).columns
         ]
 
         descr = numeric_descr + non_numeric_descr
         pbar.update(len(df.columns))
 
@@ -109,15 +87,15 @@
         The input DataFrame or Series object to extract the categorical features from.
 
     Returns:
     --------
     list
         The list of categorical feature column names in the input DataFrame or Series object.
     """
-    if not isinstance(df, pd.DataFrame):
+    if not isinstance(df, (pd.DataFrame, pd.Series)):
         raise TypeError("df must be a pandas DataFrame or Series")
 
     cat_vars = df.select_dtypes(include="object").columns.tolist()
 
     return cat_vars
 
 
@@ -128,16 +106,15 @@
     Parameters:
         df: pandas DataFrame
             The input dataframe containing categorical features.
     Returns:
         pandas DataFrame
             Unique value counts of the categorical features in the dataframe.
     """
-
-    if not is_df(df):
+    if not isinstance(df, (pd.DataFrame, pd.Series)):
         raise TypeError("df must be a pandas DataFrame")
 
     cat_vars = get_cat_vars(df)
     counts = {var: df[var].value_counts().shape[0] for var in cat_vars}
     return pd.DataFrame({"Feature": list(counts.keys()), "Unique Count": list(counts.values())})
 
 
@@ -153,15 +130,15 @@
         The list of column names to perform one-hot encoding.
 
     Returns
     -------
     pandas DataFrame
         The DataFrame with one-hot encoded columns.
     """
-    if not is_df(df):
+    if not isinstance(df, (pd.DateOffset, pd.Series)):
         raise TypeError("df must be a pandas DataFrame")
 
     if not isinstance(cols, list):
         raise TypeError("columns must be a list of column names")
 
     df[cols] = df[cols].astype("category")
 
@@ -190,15 +167,15 @@
 
     Returns
     -------
     pandas DataFrame
         The DataFrame with the categorical column replaced by target encoding.
     """
 
-    if not is_df(df):
+    if not isinstance(df, (pd.DataFrame, pd.DataFrame)):
         raise TypeError("df must be a pandas DataFrame")
 
     if not isinstance(col, str) or not isinstance(target_column, str):
         raise TypeError("col and target_column must be strings")
 
     target_mean = df.groupby(col)[target_column].mean()
     df[col + "_encoded"] = df[col].map(target_mean)
@@ -268,15 +245,15 @@
     pandas DataFrame
         The summary DataFrame with columns for the number of null values, unique value counts, data types,
         maximum and minimum values, mean, standard deviation, and skewness.
     """
     if df is None:
         raise ValueError("Expected a pandas dataframe, but got None")
 
-    if not isinstance(df, pd.DataFrame):
+    if not isinstance(df, (pd.DataFrame, pd.Series)):
         raise TypeError("df must be a pandas DataFrame")
 
     summary_df = pd.DataFrame(
         index=df.columns,
         columns=[
             "Null",
             "Unique_Count",
@@ -360,15 +337,15 @@
         If plot=False, returns a DataFrame with the missing counts and percentages for each feature.
         If plot=True, returns None and displays a heatmap of the missing values.
 
     """
     if df is None:
         raise ValueError("Expected a pandas DataFrame, but got None")
 
-    if not isinstance(df, pd.DataFrame):
+    if not isinstance(df, (pd.DataFrame, pd.Series)):
         raise TypeError("df must be a pandas DataFrame")
 
     dfs = (
         df.isna()
         .sum()
         .to_frame(name="missing_count")
         .reset_index()
@@ -410,15 +387,15 @@
     -------
     DataFrame
         Unique value counts of the features in the dataset.
     """
     if data is None:
         raise ValueError("data: Expecting a DataFrame or Series, got 'None'")
 
-    if not is_df(data):
+    if not isinstance(data, (pd.DataFrame, pd.Series)):
         raise TypeError("data: Expecting a DataFrame or Series, got '{}'".format(type(data)))
 
     if isinstance(data, pd.Series):
         data = data.to_frame()
 
     features = data.select_dtypes(include="object").columns.tolist()
     unique_counts = data[features].nunique().reset_index()
@@ -451,15 +428,15 @@
     int
         Number of rows in the test set.
     """
 
     if data_train is None or data_test is None:
         raise ValueError("Both 'data_train' and 'data_test' must be provided.")
 
-    if not is_df(data_train) or not is_df(data_test):
+    if not isinstance(data_train) or not isinstance(data_test):
         raise TypeError("Both 'data_train' and 'data_test' should be DataFrames.")
 
     n_train = data_train.shape[0]
     n_test = data_test.shape[0]
     all_data = pd.concat([data_train, data_test], ignore_index=True, sort=False)
 
     return all_data, n_train, n_test
```

### Comparing `dataramp-1.0.1.dev189/dataramp.egg-info/PKG-INFO` & `dataramp-1.0.1.dev190/dataramp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataramp
-Version: 1.0.1.dev189
+Version: 1.0.1.dev190
 Summary: A Data science library for data science / data analysis teams
 Home-page: 
 Author: Meshack Kitonga
 Author-email: kitongameshack9@gmail.com
 License: MIT
 Keywords: dataramp,Data Science,Data Analysis
 Classifier: Intended Audience :: Developers
```

### Comparing `dataramp-1.0.1.dev189/pyproject.toml` & `dataramp-1.0.1.dev190/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dataramp-1.0.1.dev189/setup.py` & `dataramp-1.0.1.dev190/setup.py`

 * *Files identical despite different names*

