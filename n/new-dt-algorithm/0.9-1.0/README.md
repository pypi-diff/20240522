# Comparing `tmp/new_dt_algorithm-0.9.tar.gz` & `tmp/new_dt_algorithm-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "new_dt_algorithm-0.9.tar", last modified: Wed May  8 10:02:51 2024, max compression
+gzip compressed data, was "new_dt_algorithm-1.0.tar", last modified: Wed May 22 11:08:52 2024, max compression
```

## Comparing `new_dt_algorithm-0.9.tar` & `new_dt_algorithm-1.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-08 10:02:51.058358 new_dt_algorithm-0.9/
--rw-rw-rw-   0        0        0      214 2024-05-08 10:02:51.057058 new_dt_algorithm-0.9/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-07 11:26:56.000000 new_dt_algorithm-0.9/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-08 10:02:51.057058 new_dt_algorithm-0.9/new_dt_algorithm.egg-info/
--rw-rw-rw-   0        0        0      214 2024-05-08 10:02:50.000000 new_dt_algorithm-0.9/new_dt_algorithm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      236 2024-05-08 10:02:50.000000 new_dt_algorithm-0.9/new_dt_algorithm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-08 10:02:50.000000 new_dt_algorithm-0.9/new_dt_algorithm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2024-05-08 10:02:50.000000 new_dt_algorithm-0.9/new_dt_algorithm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    56131 2024-05-08 10:02:10.000000 new_dt_algorithm-0.9/new_dt_algorithm.py
--rw-rw-rw-   0        0        0       42 2024-05-08 10:02:51.058534 new_dt_algorithm-0.9/setup.cfg
--rw-rw-rw-   0        0        0      443 2024-05-08 09:21:47.000000 new_dt_algorithm-0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:08:52.423163 new_dt_algorithm-1.0/
+-rw-rw-rw-   0        0        0      214 2024-05-22 11:08:52.423163 new_dt_algorithm-1.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2024-05-07 11:26:56.000000 new_dt_algorithm-1.0/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:08:52.423163 new_dt_algorithm-1.0/new_dt_algorithm.egg-info/
+-rw-rw-rw-   0        0        0      214 2024-05-22 11:08:52.000000 new_dt_algorithm-1.0/new_dt_algorithm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      236 2024-05-22 11:08:52.000000 new_dt_algorithm-1.0/new_dt_algorithm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 11:08:52.000000 new_dt_algorithm-1.0/new_dt_algorithm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2024-05-22 11:08:52.000000 new_dt_algorithm-1.0/new_dt_algorithm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    56525 2024-05-22 11:04:22.000000 new_dt_algorithm-1.0/new_dt_algorithm.py
+-rw-rw-rw-   0        0        0       42 2024-05-22 11:08:52.423163 new_dt_algorithm-1.0/setup.cfg
+-rw-rw-rw-   0        0        0      443 2024-05-08 10:08:52.000000 new_dt_algorithm-1.0/setup.py
```

### Comparing `new_dt_algorithm-0.9/new_dt_algorithm.py` & `new_dt_algorithm-1.0/new_dt_algorithm.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         Note:
         - Columns with 'unnamed' in their names are dropped from the dataset.
         """
         self.__init__()
         self.data = data
         self.Target = Target.lower()
         self.data.columns = self.data.columns.str.lower()
+        self.data  = self.data.loc[:, ~self.data.columns.duplicated()]
         self.data[self.Target] = pd.to_numeric(self.data[self.Target], errors='coerce')
         if self.data[self.Target].nunique()>2:
             self.data = self.data[self.data[self.Target]!=self.data[self.Target].min()]
         self.data = self.data.dropna(axis=1, how="all")
         self.data = self.data.dropna(axis=0, how="all")
         self.data = self.data.fillna(na_impute)
         self.data.reset_index(drop=True,inplace=True)
@@ -126,14 +127,21 @@
         
         for col in self.data.columns:
             self.data[col] = pd.to_numeric(self.data[col])
             if self.data[col].value_counts().reset_index().shape[0] == 2:
                 self.data[col] = self.data[col].astype(int)   
         
         self.data = self.data.drop([x for x in list(self.data.columns) if 'unnamed' in x], axis=1)
+        for col in self.data.drop([self.Target],axis=1).columns:
+            try:
+                self.data[col] = self.data[col].astype('float64')
+                self.data[col].replace(to_replace = {np.inf : -99999 , -np.inf : -99999}, inplace=True)
+
+            except Exception as e:
+                del self.data[col]
         self.data.reset_index(drop=True,inplace=True)
 
         
     def add_or_remove_feature(self, addition_feature_name=None, removing_feature_name=None):
         """
         Add or remove a feature from the dataset.
```

