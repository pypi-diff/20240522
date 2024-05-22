# Comparing `tmp/sklearn_smithy-0.0.1.tar.gz` & `tmp/sklearn_smithy-0.0.2.tar.gz`

## Comparing `sklearn_smithy-0.0.1.tar` & `sklearn_smithy-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,15 @@
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.1/sksmithy/__init__.py
--rw-r--r--   0        0        0     4105 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.1/sksmithy/__main__.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.1/sksmithy/_arguments.py
--rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.1/sksmithy/_callbacks.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.1/sksmithy/_logger.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.1/sksmithy/_models.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.1/sksmithy/_prompts.py
--rw-r--r--   0        0        0     6303 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.1/sksmithy/template.py.jinja
--rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.1/.gitignore
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.1/LICENSE
--rw-r--r--   0        0        0     7032 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.1/README.md
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.2/sksmithy/__init__.py
+-rw-r--r--   0        0        0     3604 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.2/sksmithy/__main__.py
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.2/sksmithy/_arguments.py
+-rw-r--r--   0        0        0     1552 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.2/sksmithy/_callbacks.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.2/sksmithy/_logger.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.2/sksmithy/_models.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.2/sksmithy/_prompts.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.2/sksmithy/_utils.py
+-rw-r--r--   0        0        0     6542 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.2/sksmithy/app.py
+-rw-r--r--   0        0        0     6275 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.2/sksmithy/template.py.jinja
+-rw-r--r--   0        0        0     3084 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.2/LICENSE
+-rw-r--r--   0        0        0     7032 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.2/README.md
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     9060 2020-02-02 00:00:00.000000 sklearn_smithy-0.0.2/PKG-INFO
```

### Comparing `sklearn_smithy-0.0.1/sksmithy/__main__.py` & `sklearn_smithy-0.0.2/sksmithy/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,52 +1,46 @@
-import subprocess
-from importlib import resources
 from pathlib import Path
-from typing import Final
 
 import typer
-from jinja2 import Template
 
 from sksmithy._arguments import (
     estimator_type_arg,
     name_arg,
-    other_params_arg,
+    optional_params_arg,
     required_params_arg,
-    support_sample_weight_arg,
+    sample_weight_arg,
 )
 from sksmithy._callbacks import parse_tags
 from sksmithy._logger import console
 from sksmithy._models import EstimatorType
-from sksmithy._prompts import OUTPUT_PROMPT, PROMPT_DECISION_FUNCTION, PROMPT_LINEAR, PROMPT_PREDICT_PROBA, PROMPT_TAGS
+from sksmithy._prompts import PROMPT_DECISION_FUNCTION, PROMPT_LINEAR, PROMPT_OUTPUT, PROMPT_PREDICT_PROBA, PROMPT_TAGS
+from sksmithy._utils import render_template
 
 app = typer.Typer(
     help="Awesome CLI to generate scikit-learn estimator boilerplate code",
     rich_markup_mode="rich",
 )
 
 
-TEMPLATE_PATH: Final[Path] = resources.files("sksmithy") / "template.py.jinja"  # type: ignore[assignment]
-
-
 @app.command()
 def version() -> None:
     """Display library version."""
     from importlib import metadata
 
     __version__ = metadata.version("sklearn-smithy")
     console.print(f"sklearn-smithy {__version__}", style="good")
 
 
 @app.command()
 def forge(
     name: name_arg,
     estimator_type: estimator_type_arg,
     required_params: required_params_arg = "",
-    other_params: other_params_arg = "",
-    support_sample_weight: support_sample_weight_arg = False,
+    optional_params: optional_params_arg = "",
+    sample_weight: sample_weight_arg = False,
 ) -> None:
     """Asks a list of questions to generate a shiny new estimator ✨
 
     Depending on the **estimator type** the additional information could be required:
 
     * if the estimator is linear (classifier or regression)
 
@@ -81,45 +75,37 @@
             decision_function = typer.confirm(PROMPT_DECISION_FUNCTION)
         case _:
             decision_function = False
 
     tags = typer.prompt(PROMPT_TAGS, default="")
     tags = parse_tags(tags)
 
-    output_file = typer.prompt(OUTPUT_PROMPT, default=f"{name.lower()}.py")
+    output_file = typer.prompt(PROMPT_OUTPUT, default=f"{name.lower()}.py")
 
     required = required_params.split(",") if required_params else []
-    other = other_params.split(",") if other_params else []
-    params = [*required, *other]
+    optional = optional_params.split(",") if optional_params else []
 
-    values = {
-        "name": name,
-        "estimator_type": estimator_type.value,
-        "mixin": estimator_type.name,
-        "linear": linear,
-        "support_sample_weight": support_sample_weight,
-        "required": required,
-        "others": other,
-        "parameters": params,
-        "decision_function": decision_function,
-        "predict_proba": predict_proba,
-        "tags": tags,
-    }
-
-    with TEMPLATE_PATH.open(mode="r") as stream:
-        template = Template(stream.read()).render(values)
+    forged_template = render_template(
+        name=name,
+        estimator_type=estimator_type,
+        required=required,
+        optional=optional,
+        linear=linear,
+        sample_weight=sample_weight,
+        predict_proba=predict_proba,
+        decision_function=decision_function,
+        tags=tags,
+    )
 
     try:
-        formatted = subprocess.check_output(["ruff", "format", "-"], input=template, encoding="utf-8")
-
         destination_file = Path(output_file)
         destination_file.parent.mkdir(parents=True, exist_ok=True)
 
         with destination_file.open(mode="w") as destination:
-            destination.write(formatted)
+            destination.write(forged_template)
 
         console.print(f"Template forged at {destination_file}", style="good")
 
     except Exception as e:  # noqa: BLE001
         console.print(f"Failed to forge template due to the following exception: {e}", style="bad")
```

### Comparing `sklearn_smithy-0.0.1/sksmithy/_arguments.py` & `sklearn_smithy-0.0.2/sksmithy/_arguments.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,23 @@
     str,
     Option(
         prompt=PROMPT_REQUIRED,
         help=("List of [bold green]required[/bold green] parameters (comma-separated)."),
         callback=args_callback,
     ),
 ]
-other_params_arg = Annotated[
+optional_params_arg = Annotated[
     str,
     Option(
         prompt=PROMPT_OPTIONAL,
         help=("List of [bold green]optional[/bold green] parameters (comma-separated)."),
         callback=args_callback,
     ),
 ]
 
-support_sample_weight_arg = Annotated[
+sample_weight_arg = Annotated[
     bool,
     Option(
         prompt=PROMPT_SAMPLE_WEIGHT,
         help="Whether or not `.fit()` does support [bold green]`sample_weight`[/bold green].",
     ),
 ]
```

### Comparing `sklearn_smithy-0.0.1/sksmithy/_callbacks.py` & `sklearn_smithy-0.0.2/sksmithy/_callbacks.py`

 * *Files identical despite different names*

### Comparing `sklearn_smithy-0.0.1/sksmithy/_models.py` & `sklearn_smithy-0.0.2/sksmithy/_models.py`

 * *Files identical despite different names*

### Comparing `sklearn_smithy-0.0.1/sksmithy/_prompts.py` & `sklearn_smithy-0.0.2/sksmithy/_prompts.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 PROMPT_DECISION_FUNCTION: Final[str] = "❓ Should the estimator have a `decision_function` method?"
 PROMPT_TAGS: Final[str] = (
     "🧪 We are almost there... Are there any tag you want to add? (comma or space separated)\n"
     "To know more about tags, check the documentation at:\n"
     "https://scikit-learn.org/dev/developers/develop.html#estimator-tags"
 )
 
-OUTPUT_PROMPT: Final[str] = "📂 Where would you like to save the class?"
+PROMPT_OUTPUT: Final[str] = "📂 Where would you like to save the class?"
```

### Comparing `sklearn_smithy-0.0.1/sksmithy/template.py.jinja` & `sklearn_smithy-0.0.2/sksmithy/template.py.jinja`

 * *Files 5% similar despite different names*

```diff
@@ -1,52 +1,47 @@
-import numpy as np
+{%- if estimator_type=='classifier' -%}import numpy as np {% endif %}
 
 from sklearn.base import {{ mixin }}
 {% if not linear %}from sklearn.base import BaseEstimator{% else %}from sklearn.linear_model._base import LinearModel{% endif %}
 from sklearn.utils import check_X_y
 from sklearn.utils.validation import check_is_fitted, check_array
 {% if support_sample_weight %}from sklearn.utils.validation import _check_sample_weight{% endif %}
 
 
 class {{ name }}({{ mixin }}, {% if not linear %}BaseEstimator{% else %}LinearModel{% endif %}):
-    """{name} estimator.
+    """{{ name }} estimator.
 
     ...
     {% if parameters %}
-
     Parameters
     ----------
     {% for param in parameters %}
-    param : ...
-    {% endfor %}
-    {% endif %}
+    {{- param }} : ...
+    {% endfor -%}
+    {% endif -%}
     """
     {% if required %}_required_parameters = {{ required }}{% endif -%}
 
     {% if parameters %}
     def __init__(
         self,
         {% for param in required %}
         {{- param }},
         {% endfor -%}
-        {%- if others -%}
+        {%- if optional -%}
         *,
         {% endif -%}
-        {% for param in others %}
+        {% for param in optional %}
         {{- param }}=...,
         {% endfor -%}
         ):
 
-        {%for param in required -%}
-        self.{{param}} = {{param}}
-        {% endfor -%}
-        {%for param in others -%}
+        {%for param in parameters -%}
         self.{{param}} = {{param}}
         {% endfor -%}
-    
         {% endif %}
 
     def fit(self, X, y{% if estimator_type == 'transformer' %}=None{% endif %}{% if support_sample_weight %}, sample_weight=None{% endif %}):
         """
         Fit {{name}} estimator.
 
         Parameters
@@ -62,15 +57,14 @@
             Target values.
         {% endif %}
             
         {%- if support_sample_weight -%}
         sample_weight : array-like of shape (n_samples,), default=None
             Individual weights for each sample.
         {% endif %}
-
         Returns
         -------
         self : {{name}}
             Fitted {{name}} estimator.
         """
 
         self.n_features_in_ = X.shape[1]
```

### Comparing `sklearn_smithy-0.0.1/.gitignore` & `sklearn_smithy-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `sklearn_smithy-0.0.1/LICENSE` & `sklearn_smithy-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn_smithy-0.0.1/README.md` & `sklearn_smithy-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sklearn_smithy-0.0.1/pyproject.toml` & `sklearn_smithy-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "sklearn-smithy"
-version = "0.0.1"
+version = "0.0.2"
 
 license = {file = "LICENSE"}
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [{name = "Francesco Bruzzesi"}]
 
 dependencies = [
@@ -25,14 +25,17 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Typing :: Typed",
 ]
 
+[project.optional-dependencies]
+streamlit = ["streamlit>=1.34.0"]
+
 [project.scripts]
 smith = "sksmithy.__main__:app"
 
 [tool.hatch.build.targets.sdist]
 only-include = ["sksmithy"]
 
 [tool.hatch.build.targets.wheel]
```

### Comparing `sklearn_smithy-0.0.1/PKG-INFO` & `sklearn_smithy-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: sklearn-smithy
-Version: 0.0.1
+Version: 0.0.2
 Author: Francesco Bruzzesi
 License: MIT License
         
         Copyright (c) 2024 Francesco Bruzzesi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -33,14 +33,16 @@
 Classifier: Typing :: Typed
 Requires-Python: >=3.10
 Requires-Dist: jinja2>=3.0.0
 Requires-Dist: rich>=13.0.0
 Requires-Dist: ruff>=0.4.0
 Requires-Dist: typer>=0.12.0
 Requires-Dist: typing-extensions>=4.4.0; python_version < '3.11'
+Provides-Extra: streamlit
+Requires-Dist: streamlit>=1.34.0; extra == 'streamlit'
 Description-Content-Type: text/markdown
 
 # Scikit-learn Smithy
 
 CLI to forge scikit-learn compatible estimator templates with ease.
 
 ## Why
```

