# Comparing `tmp/glytrait-0.1.5.tar.gz` & `tmp/glytrait-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glytrait-0.1.5.tar", max compression
+gzip compressed data, was "glytrait-0.1.6.tar", max compression
```

## Comparing `glytrait-0.1.5.tar` & `glytrait-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1063 2023-06-01 11:46:23.327576 glytrait-0.1.5/LICENSE
--rw-r--r--   0        0        0    14774 2024-04-29 03:43:46.462080 glytrait-0.1.5/README.md
--rw-r--r--   0        0        0     1406 2024-05-14 11:24:08.310318 glytrait-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      118 2024-05-14 11:24:01.010739 glytrait-0.1.5/src/glytrait/__init__.py
--rw-r--r--   0        0        0    20638 2024-05-14 11:15:11.560250 glytrait-0.1.5/src/glytrait/api.py
--rw-r--r--   0        0        0     7998 2024-05-14 08:06:17.534042 glytrait-0.1.5/src/glytrait/cli.py
--rw-r--r--   0        0        0     2640 2024-04-20 16:02:21.883776 glytrait-0.1.5/src/glytrait/data_export.py
--rw-r--r--   0        0        0    12490 2024-04-24 12:35:20.623069 glytrait-0.1.5/src/glytrait/data_input.py
--rw-r--r--   0        0        0      923 2023-12-30 06:44:57.217908 glytrait-0.1.5/src/glytrait/data_type.py
--rw-r--r--   0        0        0      812 2024-04-14 11:59:08.463548 glytrait-0.1.5/src/glytrait/exception.py
--rw-r--r--   0        0        0    26273 2024-05-14 08:33:00.448535 glytrait-0.1.5/src/glytrait/formula.py
--rw-r--r--   0        0        0    13016 2024-04-24 12:35:20.622716 glytrait-0.1.5/src/glytrait/glycan.py
--rw-r--r--   0        0        0    18326 2024-04-24 12:35:20.623387 glytrait-0.1.5/src/glytrait/meta_property.py
--rw-r--r--   0        0        0     6664 2024-04-14 11:59:08.464921 glytrait-0.1.5/src/glytrait/post_filtering.py
--rw-r--r--   0        0        0     3687 2024-04-24 12:35:20.623765 glytrait-0.1.5/src/glytrait/preprocessing.py
--rw-r--r--   0        0        0     7931 2024-04-24 12:35:20.624129 glytrait-0.1.5/src/glytrait/resources/comp_formula.txt
--rw-r--r--   0        0        0    54374 2024-04-24 12:35:20.624453 glytrait-0.1.5/src/glytrait/resources/struc_formula.txt
--rw-r--r--   0        0        0     4834 2024-04-24 12:35:20.624749 glytrait-0.1.5/src/glytrait/stat.py
--rw-r--r--   0        0        0     1665 2023-12-30 06:44:57.220052 glytrait-0.1.5/src/glytrait/trait.py
--rw-r--r--   0        0        0    15396 1970-01-01 00:00:00.000000 glytrait-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-01 11:46:23.327576 glytrait-0.1.6/LICENSE
+-rw-r--r--   0        0        0    15381 2024-05-21 02:49:56.468224 glytrait-0.1.6/README.md
+-rw-r--r--   0        0        0     1406 2024-05-21 07:36:03.265250 glytrait-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      118 2024-05-21 07:36:09.106246 glytrait-0.1.6/src/glytrait/__init__.py
+-rw-r--r--   0        0        0    21864 2024-05-21 07:23:29.999855 glytrait-0.1.6/src/glytrait/api.py
+-rw-r--r--   0        0        0     7595 2024-05-21 07:23:30.000273 glytrait-0.1.6/src/glytrait/cli.py
+-rw-r--r--   0        0        0     2640 2024-04-20 16:02:21.883776 glytrait-0.1.6/src/glytrait/data_export.py
+-rw-r--r--   0        0        0    12490 2024-04-24 12:35:20.623069 glytrait-0.1.6/src/glytrait/data_input.py
+-rw-r--r--   0        0        0      923 2023-12-30 06:44:57.217908 glytrait-0.1.6/src/glytrait/data_type.py
+-rw-r--r--   0        0        0      812 2024-04-14 11:59:08.463548 glytrait-0.1.6/src/glytrait/exception.py
+-rw-r--r--   0        0        0    26273 2024-05-14 08:33:00.448535 glytrait-0.1.6/src/glytrait/formula.py
+-rw-r--r--   0        0        0    13016 2024-04-24 12:35:20.622716 glytrait-0.1.6/src/glytrait/glycan.py
+-rw-r--r--   0        0        0    18326 2024-04-24 12:35:20.623387 glytrait-0.1.6/src/glytrait/meta_property.py
+-rw-r--r--   0        0        0     6664 2024-04-14 11:59:08.464921 glytrait-0.1.6/src/glytrait/post_filtering.py
+-rw-r--r--   0        0        0     3687 2024-04-24 12:35:20.623765 glytrait-0.1.6/src/glytrait/preprocessing.py
+-rw-r--r--   0        0        0     7931 2024-04-24 12:35:20.624129 glytrait-0.1.6/src/glytrait/resources/comp_formula.txt
+-rw-r--r--   0        0        0    54374 2024-04-24 12:35:20.624453 glytrait-0.1.6/src/glytrait/resources/struc_formula.txt
+-rw-r--r--   0        0        0     4834 2024-04-24 12:35:20.624749 glytrait-0.1.6/src/glytrait/stat.py
+-rw-r--r--   0        0        0     1665 2023-12-30 06:44:57.220052 glytrait-0.1.6/src/glytrait/trait.py
+-rw-r--r--   0        0        0    15991 1970-01-01 00:00:00.000000 glytrait-0.1.6/PKG-INFO
```

### Comparing `glytrait-0.1.5/LICENSE` & `glytrait-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.5/README.md` & `glytrait-0.1.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -38,15 +38,16 @@
     - [Options](#options)
     - [Mode](#mode)
     - [Input file format](#input-file-format)
     - [Specify output path](#specify-the-output-path)
     - [Preprocessing](#preprocessing)
     - [Sialic-acid-linkage traits](#sialic-acid-linkage-traits)
     - [Post-filtering](#post-filtering)
-    - [Custom formulas](#custom-formula)
+    - [Custom formulas](#custom-formulas)
+- [Reproduction Instructions](#reproduction-instructions)
 - [License](#license)
 
 ## Web app
 
 > Let there be no code!
 > 
 > -- my colleagues
@@ -365,10 +366,21 @@
 ### Custom Formulas
 
 Coming soon...
 
 (The functionallity has been implemented, but the documentation is not ready yet.
 After publishing the GlyTrait paper, we will update the documentation.)
 
+## Reproduction Instructions
+
+To reproduce the results in our paper 
+"GlyTrait: A versatile bioinformatics tool for Glycomics Analysis",
+please download the Supplementary Data files.
+There are three such files, corresponding to different datasets mentioned in the paper.
+Each Supplementary Data file has several sheets with the prefix of "Input -".
+These are the input data for GlyTrait.
+Please reformat the data according to the [Input file format](#input-file-format) section,
+and run GlyTrait with the same options as in the paper.
+
 ## License
 
 [MIT License](LICENSE)
```

### Comparing `glytrait-0.1.5/pyproject.toml` & `glytrait-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glytrait"
-version = "0.1.5"
+version = "0.1.6"
 description = "A tool for calculating derived traits for N-glycome"
 authors = ["fubin1999 <65430559+fubin1999@users.noreply.github.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/fubin1999/glytrait"
 keywords = ["bioinformatics", "glycomics", "biology"]
```

### Comparing `glytrait-0.1.5/src/glytrait/api.py` & `glytrait-0.1.6/src/glytrait/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     MetaPropertyTable,
     DerivedTraitTable,
     GroupSeries,
     AbundanceTable,
 )
 from glytrait.exception import GlyTraitError
 from glytrait.formula import load_default_formulas, TraitFormula, parse_formulas
-from glytrait.data_input import GlyTraitInputData
+from glytrait.data_input import GlyTraitInputData, load_data
 from glytrait.meta_property import build_meta_property_table
 from glytrait.post_filtering import post_filter
 from glytrait.preprocessing import preprocess
 from glytrait.trait import calcu_derived_trait
 from glytrait.stat import auto_test
 from glytrait.glycan import Structure, Composition
 
@@ -183,22 +183,21 @@
 GlycanDict = dict[str, Structure] | dict[str, Composition]
 
 
 @define
 class Experiment(_Workflow):
     """GlyTrait experiment.
 
-    Create an instance of this class with an GlyTraitInputData instance
-    to perform all the steps in the GlyTrait workflow.
+    Create an instance of this class to perform all the steps in the GlyTrait workflow.
 
     Firstly, call the `preprocessed` method to filter glycans, impute missing values,
     and normalize the abundance.
     Calling this method makes the `processed_abundance_table` and
     `meta_property_table` attributes available.
-    The latter is a table of structural or compositional properties of glycans,
+    The latter is a table of structural or compositional properties,
     which is used to calculate derived traits.
 
     Secondly, call the `derive_traits` method to calculate all the derived traits.
     The result table is stored as the `derived_trait_table` attribute.
 
     Thirdly, call the `post_filter` method
     to remove invalid traits and highly correlated traits.
@@ -220,39 +219,37 @@
         post_filter: Post-filter the derived traits.
         diff_analysis: Perform differential analysis.
         derive_one_trait: Try a single trait formula.
         reset: Reset the workflow to the beginning (before `preprocess`).
         get_data: Get the data by name.
 
     Attributes:
+        abundance_file: The path to the abundance file.
+        glycan_file: The path to the glycan file.
+        group_file: The path to the group file.
         mode: "structure" or "composition".
         sia_linkage: Whether to consider the linkage of sialic acid.
         input_data: The input data (a `GlyTraitInputData` instance).
         abundance_table: The original abundance table.
         glycans: The glycans.
         groups: The groups.
         processed_abundance_table: The processed abundance table.
         meta_property_table: The meta property table.
         derived_trait_table: The derived trait table.
         filtered_derived_trait_table: The filtered derived trait table.
         diff_results: The differential analysis results.
 
     Examples:
         >>> from glytrait.api import Experiment
-        >>> from glytrait.data_input import load_data
-        # This is the safe way to load data.
-        # It ensures all data are in correct formats.
-        >>> input_data = load_data(
-        ...    abundance_df=pd.read_csv("glycan_abundance.csv"),
-        ...    glycan_df=pd.read_csv("glycan_structure.csv"),
-        ...    group_df=pd.read_csv("group.csv"),
+        >>> experiment = Experiment(
+        ...    abundance_file="glycan_abundance.csv",
+        ...    glycan_file="glycan_structure.csv",
+        ...    group_file="group.csv",
         ...    mode="structure",
-        )
-        # `input_data` is a GlyTraitInputData instance.
-        >>> experiment = Experiment(input_data)
+        ... )
         >>> experiment.preprocess(filter_max_na=0.5, impute_method="min")
         >>> experiment.derive_traits()  # with default formulas
         >>> experiment.post_filter(corr_threshold=0.9)
         >>> experiment.diff_analysis()
     """
 
     _all_steps = [
@@ -264,18 +261,45 @@
     _data_dict = {
         "preprocess": ["processed_abundance_table", "meta_property_table"],
         "derive_traits": ["derived_trait_table", "formulas"],
         "post_filter": ["filtered_derived_trait_table"],
         "diff_analysis": ["diff_results"],
     }
 
-    input_data: GlyTraitInputData
+    abundance_file: Optional[str] = field(default=None, kw_only=True, repr=False)
+    glycan_file: Optional[str] = field(default=None, kw_only=True, repr=False)
+    group_file: Optional[str] = field(default=None, kw_only=True, repr=False)
+    input_data: GlyTraitInputData = field(default=None, kw_only=True)
     mode: Literal["structure", "composition"] = field(default="structure", kw_only=True)
     sia_linkage: bool = field(default=False, kw_only=True)
 
+    def __attrs_post_init__(self):
+        if self.abundance_file is None and self.glycan_file is None:
+            if self.input_data is None:
+                msg = "Either `input_data` or `abundance_file` and `glycan_file` are required."
+                raise ValueError(msg)
+        if self.abundance_file and self.glycan_file is None:
+            raise ValueError(
+                "`glycan_file` is required if `abundance_file` is provided."
+            )
+        if self.abundance_file is None and self.glycan_file:
+            raise ValueError(
+                "`abundance_file` is required if `glycan_file` is provided."
+            )
+        if self.input_data and (self.abundance_file or self.glycan_file):
+            raise ValueError("Do not provide both `input_data` and files.")
+
+        if self.input_data is None:
+            self.input_data = load_data(
+                abundance_df=pd.read_csv(self.abundance_file),
+                glycan_df=pd.read_csv(self.glycan_file),
+                group_df=pd.read_csv(self.group_file) if self.group_file else None,
+                mode=self.mode,
+            )
+
     @property
     def abundance_table(self) -> pd.DataFrame:
         """The original abundance table."""
         return self.input_data.abundance_table
 
     @abundance_table.setter
     def abundance_table(self, value: pd.DataFrame) -> None:
```

### Comparing `glytrait-0.1.5/src/glytrait/cli.py` & `glytrait-0.1.6/src/glytrait/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 """Command line interface for glyTrait."""
 
 from pathlib import Path
 from typing import Literal, Any
 
 import click
 import emoji
-import pandas as pd
 from attrs import define
 
 from glytrait.exception import GlyTraitError
-from glytrait.data_input import load_data
 from glytrait.api import Experiment, MissingDataError
 from glytrait.formula import save_builtin_formula, load_formulas_from_file
 from glytrait.data_export import export_all
 
 UNDIFINED = "__UNDEFINED__"
 
 
@@ -213,26 +211,14 @@
     return str(output_dir_path)
 
 
 def _determine_mode(mode: str) -> Literal["structure", "composition"]:
     return "composition" if mode.lower() in ["c", "composition"] else "structure"
 
 
-def _make_input_data(
-    abundance_file: str,
-    glycan_file: str,
-    group_file: str | None,
-    mode: Literal["structure", "composition"],
-):
-    abundance_df = pd.read_csv(abundance_file)
-    glycan_df = pd.read_csv(glycan_file)
-    group_df = pd.read_csv(group_file) if group_file else None
-    return load_data(abundance_df, glycan_df, group_df, mode=mode)
-
-
 def _prepare_output(exp: Experiment) -> list[tuple[str, Any]]:
     result = {
         "derived_traits.csv": exp.derived_trait_table,
         "glycan_abundance_processed.csv": exp.processed_abundance_table,
         "meta_properties.csv": exp.meta_property_table,
     }
 
@@ -258,16 +244,21 @@
     abundance_file: str,
     glycan_file: str,
     group_file: str | None,
     formula_file: str | None,
     config: WorkflowConfig,
     output_dir: str,
 ):
-    input_data = _make_input_data(abundance_file, glycan_file, group_file, config.mode)
-    exp = Experiment(input_data, sia_linkage=config.sia_linkage, mode=config.mode)
+    exp = Experiment(
+        abundance_file=abundance_file,
+        glycan_file=glycan_file,
+        group_file=group_file,
+        sia_linkage=config.sia_linkage,
+        mode=config.mode,
+    )
     _process_exp(exp, formula_file, config)
     output_data = _prepare_output(exp)
     export_all(output_data, output_dir)
 
 
 def _process_exp(
     exp: Experiment,
```

### Comparing `glytrait-0.1.5/src/glytrait/data_export.py` & `glytrait-0.1.6/src/glytrait/data_export.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.5/src/glytrait/data_input.py` & `glytrait-0.1.6/src/glytrait/data_input.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.5/src/glytrait/data_type.py` & `glytrait-0.1.6/src/glytrait/data_type.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.5/src/glytrait/exception.py` & `glytrait-0.1.6/src/glytrait/exception.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.5/src/glytrait/formula.py` & `glytrait-0.1.6/src/glytrait/formula.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.5/src/glytrait/glycan.py` & `glytrait-0.1.6/src/glytrait/glycan.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.5/src/glytrait/meta_property.py` & `glytrait-0.1.6/src/glytrait/meta_property.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.5/src/glytrait/post_filtering.py` & `glytrait-0.1.6/src/glytrait/post_filtering.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.5/src/glytrait/preprocessing.py` & `glytrait-0.1.6/src/glytrait/preprocessing.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.5/src/glytrait/resources/comp_formula.txt` & `glytrait-0.1.6/src/glytrait/resources/comp_formula.txt`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.5/src/glytrait/resources/struc_formula.txt` & `glytrait-0.1.6/src/glytrait/resources/struc_formula.txt`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.5/src/glytrait/stat.py` & `glytrait-0.1.6/src/glytrait/stat.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.5/src/glytrait/trait.py` & `glytrait-0.1.6/src/glytrait/trait.py`

 * *Files identical despite different names*

### Comparing `glytrait-0.1.5/PKG-INFO` & `glytrait-0.1.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glytrait
-Version: 0.1.5
+Version: 0.1.6
 Summary: A tool for calculating derived traits for N-glycome
 Home-page: https://github.com/fubin1999/glytrait
 License: MIT
 Keywords: bioinformatics,glycomics,biology
 Author: fubin1999
 Author-email: 65430559+fubin1999@users.noreply.github.com
 Requires-Python: >=3.10,<3.13
@@ -64,15 +64,16 @@
     - [Options](#options)
     - [Mode](#mode)
     - [Input file format](#input-file-format)
     - [Specify output path](#specify-the-output-path)
     - [Preprocessing](#preprocessing)
     - [Sialic-acid-linkage traits](#sialic-acid-linkage-traits)
     - [Post-filtering](#post-filtering)
-    - [Custom formulas](#custom-formula)
+    - [Custom formulas](#custom-formulas)
+- [Reproduction Instructions](#reproduction-instructions)
 - [License](#license)
 
 ## Web app
 
 > Let there be no code!
 > 
 > -- my colleagues
@@ -391,11 +392,22 @@
 ### Custom Formulas
 
 Coming soon...
 
 (The functionallity has been implemented, but the documentation is not ready yet.
 After publishing the GlyTrait paper, we will update the documentation.)
 
+## Reproduction Instructions
+
+To reproduce the results in our paper 
+"GlyTrait: A versatile bioinformatics tool for Glycomics Analysis",
+please download the Supplementary Data files.
+There are three such files, corresponding to different datasets mentioned in the paper.
+Each Supplementary Data file has several sheets with the prefix of "Input -".
+These are the input data for GlyTrait.
+Please reformat the data according to the [Input file format](#input-file-format) section,
+and run GlyTrait with the same options as in the paper.
+
 ## License
 
 [MIT License](LICENSE)
```

