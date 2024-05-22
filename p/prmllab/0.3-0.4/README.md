# Comparing `tmp/prmllab-0.3.tar.gz` & `tmp/prmllab-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prmllab-0.3.tar", last modified: Thu May 16 01:04:53 2024, max compression
+gzip compressed data, was "prmllab-0.4.tar", last modified: Wed May 22 17:54:02 2024, max compression
```

## Comparing `prmllab-0.3.tar` & `prmllab-0.4.tar`

### file list

```diff
@@ -1,17 +1,29 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 01:04:53.114529 prmllab-0.3/
--rw-rw-rw-   0        0        0       52 2024-05-16 01:04:53.111527 prmllab-0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-16 01:04:53.055787 prmllab-0.3/prmllab/
--rw-rw-rw-   0        0        0   172797 2024-05-15 14:12:04.000000 prmllab-0.3/prmllab/Bagging.ipynb
--rw-rw-rw-   0        0        0    15193 2024-05-16 01:03:25.000000 prmllab-0.3/prmllab/Regression.ipynb
--rw-rw-rw-   0        0        0        0 2024-05-15 15:55:27.000000 prmllab-0.3/prmllab/__init__.py
--rw-rw-rw-   0        0        0      834 2024-05-15 15:57:22.000000 prmllab-0.3/prmllab/functions.py
--rw-rw-rw-   0        0        0     4282 2024-05-16 01:03:29.000000 prmllab-0.3/prmllab/kmeans.ipynb
--rw-rw-rw-   0        0        0     4012 2024-05-16 00:53:26.000000 prmllab-0.3/prmllab/mlp.ipynb
--rw-rw-rw-   0        0        0     2547 2024-05-15 14:37:28.000000 prmllab-0.3/prmllab/naive.ipynb
-drwxrwxrwx   0        0        0        0 2024-05-16 01:04:53.108493 prmllab-0.3/prmllab.egg-info/
--rw-rw-rw-   0        0        0       52 2024-05-16 01:04:52.000000 prmllab-0.3/prmllab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2024-05-16 01:04:52.000000 prmllab-0.3/prmllab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 01:04:52.000000 prmllab-0.3/prmllab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-16 01:04:52.000000 prmllab-0.3/prmllab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 01:04:53.116034 prmllab-0.3/setup.cfg
--rw-rw-rw-   0        0        0      216 2024-05-16 01:03:52.000000 prmllab-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:54:02.680595 prmllab-0.4/
+-rw-rw-rw-   0        0        0       52 2024-05-22 17:54:02.678130 prmllab-0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 17:54:02.497609 prmllab-0.4/prmllab/
+-rw-rw-rw-   0        0        0        0 2024-05-22 17:49:21.000000 prmllab-0.4/prmllab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:54:02.672411 prmllab-0.4/prmllab/files/
+-rw-rw-rw-   0        0        0   263203 2024-05-15 18:03:57.000000 prmllab-0.4/prmllab/files/Regression.ipynb
+-rw-rw-rw-   0        0        0    20653 2024-05-22 15:21:20.000000 prmllab-0.4/prmllab/files/abalone_regression.ipynb
+-rw-rw-rw-   0        0        0   172797 2024-05-15 16:32:54.000000 prmllab-0.4/prmllab/files/bagging.ipynb
+-rw-rw-rw-   0        0        0    19499 2024-05-22 16:21:40.000000 prmllab-0.4/prmllab/files/breast-cancer-detection-bagging.ipynb
+-rw-rw-rw-   0        0        0    34320 2024-05-22 17:33:19.000000 prmllab-0.4/prmllab/files/car-price-prediction.ipynb
+-rw-rw-rw-   0        0        0     7944 2024-05-22 15:35:46.000000 prmllab-0.4/prmllab/files/diabetes-detection-bagging.ipynb
+-rw-rw-rw-   0        0        0    80584 2024-05-22 16:55:25.000000 prmllab-0.4/prmllab/files/kmean.ipynb
+-rw-rw-rw-   0        0        0   198730 2024-05-15 16:32:55.000000 prmllab-0.4/prmllab/files/kmeans.ipynb
+-rw-rw-rw-   0        0        0    26066 2024-05-22 15:49:28.000000 prmllab-0.4/prmllab/files/linear-advertising.ipynb
+-rw-rw-rw-   0        0        0    31748 2024-05-22 16:00:22.000000 prmllab-0.4/prmllab/files/mlp-cardio.ipynb
+-rw-rw-rw-   0        0        0    36152 2024-05-22 16:06:46.000000 prmllab-0.4/prmllab/files/mlp-malware.ipynb
+-rw-rw-rw-   0        0        0   187692 2024-05-15 18:03:57.000000 prmllab-0.4/prmllab/files/mlp.ipynb
+-rw-rw-rw-   0        0        0     3191 2024-05-22 16:57:06.000000 prmllab-0.4/prmllab/files/naive.ipynb
+-rw-rw-rw-   0        0        0   106385 2024-05-22 15:09:39.000000 prmllab-0.4/prmllab/files/students.ipynb
+-rw-rw-rw-   0        0        0    23764 2024-05-22 16:44:54.000000 prmllab-0.4/prmllab/files/titanic-bagging.ipynb
+-rw-rw-rw-   0        0        0     2830 2024-05-22 17:43:03.000000 prmllab-0.4/prmllab/files/vehicle.ipynb
+-rw-rw-rw-   0        0        0      886 2024-05-22 17:50:21.000000 prmllab-0.4/prmllab/functions.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:54:02.675447 prmllab-0.4/prmllab.egg-info/
+-rw-rw-rw-   0        0        0       52 2024-05-22 17:54:02.000000 prmllab-0.4/prmllab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      709 2024-05-22 17:54:02.000000 prmllab-0.4/prmllab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 17:54:02.000000 prmllab-0.4/prmllab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-22 17:54:02.000000 prmllab-0.4/prmllab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 17:54:02.681608 prmllab-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      269 2024-05-22 17:51:07.000000 prmllab-0.4/setup.py
```

### Comparing `prmllab-0.3/prmllab/Bagging.ipynb` & `prmllab-0.4/prmllab/files/bagging.ipynb`

 * *Files identical despite different names*

### Comparing `prmllab-0.3/prmllab/functions.py` & `prmllab-0.4/prmllab/functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import os
 import shutil
 
 def display_files():
-    file_list = [file for file in os.listdir(os.path.dirname(__file__)) if os.path.isfile(os.path.join(os.path.dirname(__file__), file))]
+    files_dir = os.path.join(os.path.dirname(__file__), 'files')
+    file_list = [file for file in os.listdir(files_dir) if os.path.isfile(os.path.join(files_dir, file))]
     print("Available files:")
     for i, file in enumerate(file_list, start=1):
         print(f"{i}. {file}")
 
 def copy_file(file_index):
-    file_list = [file for file in os.listdir(os.path.dirname(__file__)) if os.path.isfile(os.path.join(os.path.dirname(__file__), file))]
+    files_dir = os.path.join(os.path.dirname(__file__), 'files')
+    file_list = [file for file in os.listdir(files_dir) if os.path.isfile(os.path.join(files_dir, file))]
     if file_index < 1 or file_index > len(file_list):
         print("Invalid selection.")
         return
     file_to_copy = file_list[file_index - 1]
-    src = os.path.join(os.path.dirname(__file__), file_to_copy)
+    src = os.path.join(files_dir, file_to_copy)
     dst = os.path.join(os.getcwd(), file_to_copy)
     shutil.copy(src, dst)
     print(f"File '{file_to_copy}' copied to current directory.")
```

### Comparing `prmllab-0.3/prmllab/mlp.ipynb` & `prmllab-0.4/prmllab/files/vehicle.ipynb`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9029134199134199%*

 * *Differences: {"'cells'": "{0: {'execution_count': 2, 'source': {insert: [(0, 'import pandas as pd\\n'), (1, "*

 * *            "'from sklearn.model_selection import train_test_split\\n'), (2, 'from "*

 * *            "sklearn.preprocessing import StandardScaler\\n'), (3, 'from sklearn.linear_model "*

 * *            'import LinearRegression\\n\'), (4, \'from sklearn import metrics\\n\'), (8, "data = '*

 * *            'pd.read_csv(\'car_data.csv\')\\n"), (10, "data = pd.get_dummies(data, '*

 * *            'columns=[\'Fuel_Type\',\'Seller_Type\ […]*

```diff
@@ -1,146 +1,91 @@
 {
     "cells": [
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
-                "import numpy as np\n",
                 "import pandas as pd\n",
-                "data=pd.read_csv(r'cardio.csv',delimiter=\";\")\n",
-                "data.head()"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "#data.columns\n",
-                "print(data.dtypes)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "import pandas as pd\n",
-                "from sklearn.preprocessing import LabelEncoder\n",
-                "\n",
-                "# Initialize LabelEncoder\n",
-                "label_encoder = LabelEncoder()\n",
-                "\n",
-                "# Loop through each column except the first one (assuming it's an identifier column)\n",
-                "for column in data.columns[1:]:\n",
-                "    # Apply label encoding to object-type columns\n",
-                "    if data[column].dtype == 'object':\n",
-                "        data[column] = label_encoder.fit_transform(data[column])\n",
-                "\n",
-                "# Print the updated DataFrame\n",
-                "print(data.head())\n"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
+                "from sklearn.model_selection import train_test_split\n",
+                "from sklearn.preprocessing import StandardScaler\n",
+                "from sklearn.linear_model import LinearRegression\n",
+                "from sklearn import metrics\n",
                 "import seaborn as sns\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
-                "# Calculate the correlation matrix\n",
-                "corr = data.corr()\n",
+                "data = pd.read_csv('car_data.csv')\n",
                 "\n",
-                "# Create a heatmap\n",
-                "plt.figure(figsize=(10, 8))\n",
-                "sns.heatmap(corr, annot=True, fmt=\".2f\")\n",
-                "plt.title('Correlation Heatmap of Cardio Dataset')\n",
-                "plt.show()"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "X = data.drop(columns=['cardio','height','weight','id','active','ap_hi','ap_lo'])  # Features (independent variables)\n",
-                "y = data['cardio']  # Target variable\n",
+                "data = pd.get_dummies(data, columns=['Fuel_Type','Seller_Type','Transmission'], drop_first=True)\n",
+                "X = data.drop(['Car_Name','Selling_Price'], axis=1)\n",
+                "y = data['Selling_Price']\n",
+                "X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=42)\n",
+                "scaler = StandardScaler()\n",
+                "X_train = scaler.fit_transform(X_train)\n",
+                "X_test = scaler.fit_transform(X_test)\n",
                 "\n",
-                "# Print the independent variables (features) and target variable\n",
-                "print(\"Independent variables (features):\\n\", X)\n",
-                "print(\"\\nTarget variable:\\n\", y)"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "from sklearn.model_selection import train_test_split\n",
+                "model = LinearRegression()\n",
+                "model.fit(X_train, y_train)\n",
                 "\n",
-                "# Split dataset into training set and test set\n",
-                "X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.3, random_state=42)  # 70% training and 30% test"
-            ]
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "# Import MLPClassifer \n",
-                "from sklearn.neural_network import MLPClassifier\n",
                 "\n",
-                "# Create model object\n",
-                "clf = MLPClassifier(hidden_layer_sizes=(6,5),\n",
-                "                    random_state=5,\n",
-                "                    verbose=True,\n",
-                "                    learning_rate_init=0.01)\n",
+                "input_data = X_test[0:1]  # Selecting the first row from the test set for prediction\n",
+                "predicted_price = model.predict(input_data)\n",
                 "\n",
-                "# Fit data onto the model\n",
-                "clf.fit(X_train,y_train)"
+                "\n"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 3,
             "metadata": {},
-            "outputs": [],
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Mean Absolute Error (MAE): 1.2401911938820376\n",
+                        "Mean Squared Error (MSE): 3.4868775495557136\n",
+                        "R^2 Score: 0.850413419632344\n"
+                    ]
+                }
+            ],
             "source": [
-                "# Make prediction on test dataset\n",
-                "ypred=clf.predict(X_test)\n",
-                "\n",
-                "# Import accuracy score \n",
-                "from sklearn.metrics import accuracy_score\n",
+                "# Evaluate the model\n",
+                "pred = model.predict(X_test)\n",
+                "mae = metrics.mean_absolute_error(pred, y_test)\n",
+                "mse = metrics.mean_squared_error(pred, y_test)\n",
+                "r2 = metrics.r2_score(pred, y_test)\n",
                 "\n",
-                "# Calcuate accuracy\n",
-                "print(\"Accuracy: \",accuracy_score(y_test,ypred))"
+                "# evaluation metrics\n",
+                "print(\"Mean Absolute Error (MAE):\", mae)\n",
+                "print(\"Mean Squared Error (MSE):\", mse)\n",
+                "print(\"R^2 Score:\", r2)"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": null,
-            "metadata": {},
-            "outputs": [],
-            "source": []
-        },
-        {
-            "cell_type": "code",
-            "execution_count": null,
+            "execution_count": 4,
             "metadata": {},
-            "outputs": [],
-            "source": []
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Actual Price: 0.35\n",
+                        "Predicted Price: 1.8560422012802351\n"
+                    ]
+                }
+            ],
+            "source": [
+                "# actual vs predicted\n",
+                "print(\"Actual Price:\", y_test.iloc[0])  \n",
+                "print(\"Predicted Price:\", predicted_price[0]) \n",
+                "\n"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

### Comparing `prmllab-0.3/prmllab/naive.ipynb` & `prmllab-0.4/prmllab/files/naive.ipynb`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'cells'": "{insert: [(1, OrderedDict([('cell_type', 'code'), ('execution_count', 2), "*

 * *            "('metadata', OrderedDict()), ('outputs', [OrderedDict([('name', 'stdout'), "*

 * *            "('output_type', 'stream'), ('text', ['Actual Label: 0\\n', 'Predicted Label: "*

 * *            "0\\n'])])]), ('source', ['row_index = 10\\n', 'input_text = "*

 * *            "X_test.iloc[row_index]\\n', '\\n', 'input_text_counts = "*

 * *            "vectorizer.transform([input_text])\\n', '\\n', '\\n', 'predicted_label = "*

 * *        […]*

```diff
@@ -55,14 +55,42 @@
                 "# Calculate accuracy\n",
                 "accuracy = accuracy_score(y_test, y_pred)\n",
                 "print(\"Accuracy:\", accuracy)\n",
                 "\n",
                 "print(\"\\nClassification Report:\")\n",
                 "print(classification_report(y_test, y_pred))\n"
             ]
+        },
+        {
+            "cell_type": "code",
+            "execution_count": 2,
+            "metadata": {},
+            "outputs": [
+                {
+                    "name": "stdout",
+                    "output_type": "stream",
+                    "text": [
+                        "Actual Label: 0\n",
+                        "Predicted Label: 0\n"
+                    ]
+                }
+            ],
+            "source": [
+                "row_index = 10\n",
+                "input_text = X_test.iloc[row_index]\n",
+                "\n",
+                "input_text_counts = vectorizer.transform([input_text])\n",
+                "\n",
+                "\n",
+                "predicted_label = clf.predict(input_text_counts)[0]\n",
+                "actual_label = y_test.iloc[row_index]\n",
+                "\n",
+                "print(\"Actual Label:\", actual_label)\n",
+                "print(\"Predicted Label:\", predicted_label)\n"
+            ]
         }
     ],
     "metadata": {
         "kernelspec": {
             "display_name": "Python 3",
             "language": "python",
             "name": "python3"
```

