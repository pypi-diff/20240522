# Comparing `tmp/phenotype2phenopacket-0.4.0.tar.gz` & `tmp/phenotype2phenopacket-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phenotype2phenopacket-0.4.0.tar", max compression
+gzip compressed data, was "phenotype2phenopacket-0.5.1.tar", max compression
```

## Comparing `phenotype2phenopacket-0.4.0.tar` & `phenotype2phenopacket-0.5.1.tar`

### file list

```diff
@@ -1,19 +1,18 @@
--rw-r--r--   0        0        0     1320 2024-01-03 16:39:55.742185 phenotype2phenopacket-0.4.0/README.md
--rw-r--r--   0        0        0      913 2024-01-03 16:39:55.742185 phenotype2phenopacket-0.4.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-03 16:39:55.742185 phenotype2phenopacket-0.4.0/src/phenotype2phenopacket/__init__.py
--rw-r--r--   0        0        0        0 2024-01-03 16:39:55.742185 phenotype2phenopacket-0.4.0/src/phenotype2phenopacket/add/__init__.py
--rw-r--r--   0        0        0     2361 2024-01-03 16:39:55.742185 phenotype2phenopacket-0.4.0/src/phenotype2phenopacket/add/add_genes.py
--rw-r--r--   0        0        0      478 2024-01-03 16:39:55.742185 phenotype2phenopacket-0.4.0/src/phenotype2phenopacket/cli.py
--rw-r--r--   0        0        0     1092 2024-01-03 16:39:55.742185 phenotype2phenopacket-0.4.0/src/phenotype2phenopacket/cli_add.py
--rw-r--r--   0        0        0      922 2024-01-03 16:39:55.742185 phenotype2phenopacket-0.4.0/src/phenotype2phenopacket/cli_convert.py
--rw-r--r--   0        0        0      924 2024-01-03 16:39:55.742185 phenotype2phenopacket-0.4.0/src/phenotype2phenopacket/cli_create.py
--rw-r--r--   0        0        0        0 2024-01-03 16:39:55.742185 phenotype2phenopacket-0.4.0/src/phenotype2phenopacket/convert/__init__.py
--rw-r--r--   0        0        0     1404 2024-01-03 16:39:55.742185 phenotype2phenopacket-0.4.0/src/phenotype2phenopacket/convert/convert.py
--rw-r--r--   0        0        0        0 2024-01-03 16:39:55.742185 phenotype2phenopacket-0.4.0/src/phenotype2phenopacket/create/__init__.py
--rw-r--r--   0        0        0     2275 2024-01-03 16:39:55.742185 phenotype2phenopacket-0.4.0/src/phenotype2phenopacket/create/create.py
--rw-r--r--   0        0        0 16425815 2024-01-03 16:39:55.814184 phenotype2phenopacket-0.4.0/src/phenotype2phenopacket/resources/hgnc_complete_set_2023-04-01.txt
--rw-r--r--   0        0        0        0 2024-01-03 16:39:55.814184 phenotype2phenopacket-0.4.0/src/phenotype2phenopacket/utils/__init__.py
--rw-r--r--   0        0        0     2405 2024-01-03 16:39:55.814184 phenotype2phenopacket-0.4.0/src/phenotype2phenopacket/utils/gene_map_utils.py
--rw-r--r--   0        0        0    23356 2024-01-03 16:39:55.814184 phenotype2phenopacket-0.4.0/src/phenotype2phenopacket/utils/phenopacket_utils.py
--rw-r--r--   0        0        0     2348 2024-01-03 16:39:55.814184 phenotype2phenopacket-0.4.0/src/phenotype2phenopacket/utils/utils.py
--rw-r--r--   0        0        0     2017 1970-01-01 00:00:00.000000 phenotype2phenopacket-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1721 2024-05-22 20:00:48.075733 phenotype2phenopacket-0.5.1/README.md
+-rw-r--r--   0        0        0      910 2024-05-22 20:00:48.075733 phenotype2phenopacket-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-22 20:00:48.075733 phenotype2phenopacket-0.5.1/src/phenotype2phenopacket/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 20:00:48.075733 phenotype2phenopacket-0.5.1/src/phenotype2phenopacket/add/__init__.py
+-rw-r--r--   0        0        0     3173 2024-05-22 20:00:48.075733 phenotype2phenopacket-0.5.1/src/phenotype2phenopacket/add/add_genes.py
+-rw-r--r--   0        0        0      478 2024-05-22 20:00:48.075733 phenotype2phenopacket-0.5.1/src/phenotype2phenopacket/cli.py
+-rw-r--r--   0        0        0     1175 2024-05-22 20:00:48.075733 phenotype2phenopacket-0.5.1/src/phenotype2phenopacket/cli_add.py
+-rw-r--r--   0        0        0     2108 2024-05-22 20:00:48.075733 phenotype2phenopacket-0.5.1/src/phenotype2phenopacket/cli_convert.py
+-rw-r--r--   0        0        0     2174 2024-05-22 20:00:48.075733 phenotype2phenopacket-0.5.1/src/phenotype2phenopacket/cli_create.py
+-rw-r--r--   0        0        0        0 2024-05-22 20:00:48.075733 phenotype2phenopacket-0.5.1/src/phenotype2phenopacket/convert/__init__.py
+-rw-r--r--   0        0        0     1642 2024-05-22 20:00:48.075733 phenotype2phenopacket-0.5.1/src/phenotype2phenopacket/convert/convert.py
+-rw-r--r--   0        0        0        0 2024-05-22 20:00:48.075733 phenotype2phenopacket-0.5.1/src/phenotype2phenopacket/create/__init__.py
+-rw-r--r--   0        0        0     2981 2024-05-22 20:00:48.075733 phenotype2phenopacket-0.5.1/src/phenotype2phenopacket/create/create.py
+-rw-r--r--   0        0        0 16425815 2024-05-22 20:00:48.147733 phenotype2phenopacket-0.5.1/src/phenotype2phenopacket/resources/hgnc_complete_set_2023-04-01.txt
+-rw-r--r--   0        0        0        0 2024-05-22 20:00:48.147733 phenotype2phenopacket-0.5.1/src/phenotype2phenopacket/utils/__init__.py
+-rw-r--r--   0        0        0    39629 2024-05-22 20:00:48.147733 phenotype2phenopacket-0.5.1/src/phenotype2phenopacket/utils/phenopacket_utils.py
+-rw-r--r--   0        0        0     7987 2024-05-22 20:00:48.147733 phenotype2phenopacket-0.5.1/src/phenotype2phenopacket/utils/utils.py
+-rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 phenotype2phenopacket-0.5.1/PKG-INFO
```

### Comparing `phenotype2phenopacket-0.4.0/README.md` & `phenotype2phenopacket-0.5.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -28,14 +28,26 @@
 
 You can also limit the number of disease phenopackets converted/created:
 
 ```shell
 p2p convert --phenotype-annotation /path/to/phenotype.hpoa --output-dir /path/to/output-dir --num-diseases 100
 ```
 
+Or limit for a specific OMIM disease:
+
+```shell
+p2p create --phenotype-annotation /path/to/phenotype.hpoa --output-dir /path/to/output-dir --omim-id OMIM:619340
+```
+
+Or limit for a list of OMIM IDs specified in a text file, with each ID separated by a new line:
+
+```shell
+p2p create --phenotype-annotation /path/to/phenotype.hpoa --output-dir /path/to/output-dir --omim-id-list /path/to/list.txt
+```
+
 To add known gene-to-phenotype relationships to phenopackets:
 
 ```shell
 p2p add-genes --phenopacket-dir /path/to/synthetic-phenopackets --disease-pg /path/to/disease.pg --hgnc-data /path/to/hgnc_complete_set.txt --output-dir /path/to/output-dir
 ```
 
 > **_NOTE:_** To add known gene-to-phenotype the Exomiser disease.pg file is expected
```

### Comparing `phenotype2phenopacket-0.4.0/pyproject.toml` & `phenotype2phenopacket-0.5.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "phenotype2phenopacket"
-version = "0.4.0"
+version = "0.5.1"
 description = ""
 authors = ["Yasemin Bridges <y.bridges@qmul.ac.uk>"]
 readme = "README.md"
 packages = [{ include = "phenotype2phenopacket", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 pandas = ">=1.5.1,<2.0.0"
 phenopackets = "^2.0.2"
-polars = "^0.17.5"
+polars = "^0.19"
 oaklib = "^0.5.1"
 click = "^8.1.3"
-ontobio = "^2.8.5"
+pheval = "^0.3.6"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 coverage = "^6.5.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.12.0"
```

### Comparing `phenotype2phenopacket-0.4.0/src/phenotype2phenopacket/add/add_genes.py` & `phenotype2phenopacket-0.5.1/src/phenotype2phenopacket/add/add_genes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,86 @@
 from pathlib import Path
 
 import polars as pl
 from phenopackets import Disease
-
-from phenotype2phenopacket.utils.gene_map_utils import (
+from pheval.utils.file_utils import all_files
+from pheval.utils.phenopacket_utils import (
     GeneIdentifierUpdater,
     create_gene_identifier_map,
     create_hgnc_dict,
+    phenopacket_reader,
 )
+
 from phenotype2phenopacket.utils.phenopacket_utils import (
     PhenopacketInterpretationExtender,
     PhenopacketUtil,
-    phenopacket_reader,
     write_phenopacket,
 )
-from phenotype2phenopacket.utils.utils import all_files
 
 
 def get_phenotype_to_disease_entries(
     omim_disease_pg: pl.DataFrame, disease: Disease
 ) -> pl.DataFrame:
-    """Return disease.pg entries that match the OMIM disease ID."""
+    """
+    Return disease.pg entries that match the provided OMIM disease ID.
+
+    Args:
+        omim_disease_pg (pl.DataFrame): DataFrame containing disease.pg entries.
+        disease (Disease): Disease object containing the OMIM disease ID.
+
+    Returns:
+        pl.DataFrame: Filtered DataFrame containing entries matching the OMIM disease ID.
+    """
     return omim_disease_pg.filter(pl.col("database_id") == disease.term.id)
 
 
 def add_genes(
     phenopacket_path: Path,
     disease_pg: pl.DataFrame,
     gene_identifier_updater: GeneIdentifierUpdater,
     output_dir: Path,
 ):
-    """Add known gene to phenotype relationships to the interpretations of a phenopacket."""
+    """
+    Add known gene-to-phenotype relationships to the interpretations of a phenopacket.
+
+    Args:
+        phenopacket_path (Path): Path to the phenopacket file.
+        disease_pg (pl.DataFrame): DataFrame containing disease.pg entries.
+        gene_identifier_updater (GeneIdentifierUpdater): Object for updating gene identifiers.
+        output_dir (Path): Directory to write the updated phenopacket.
+
+    """
     phenopacket = phenopacket_reader(phenopacket_path)
     disease = PhenopacketUtil(phenopacket).return_phenopacket_disease()
     filtered_disease_pg = get_phenotype_to_disease_entries(disease_pg, disease)
     if len(filtered_disease_pg) == 0:
         print(f"No gene-to-phenotype matches: {disease.term.id}, {disease.term.label}")
     else:
         phenopacket_with_genes = PhenopacketInterpretationExtender(
             phenopacket
         ).add_gene_interpretation_to_phenopacket(
             omim_disease_phenotype_gene_map=filtered_disease_pg,
             gene_identifier_updater=gene_identifier_updater,
         )
-        write_phenopacket(
-            phenopacket_with_genes, output_dir.joinpath(phenopacket_path.name)
-        ) if phenopacket_with_genes is not None else None
+        (
+            write_phenopacket(phenopacket_with_genes, output_dir.joinpath(phenopacket_path.name))
+            if phenopacket_with_genes is not None
+            else None
+        )
 
 
-def add_genes_to_directory(
-    phenopacket_dir: Path, disease_pg: pl.DataFrame, hgnc_data_file: Path, output_dir: Path
-):
-    """Add known gene to phenotype relationships to the interpretations of a directory phenopackets."""
-    hgnc_dict = create_hgnc_dict(hgnc_data_file)
-    identifier_map = create_gene_identifier_map(hgnc_data_file)
+def add_genes_to_directory(phenopacket_dir: Path, disease_pg: pl.DataFrame, output_dir: Path):
+    """
+    Add known gene-to-phenotype relationships to the interpretations of a directory of phenopackets.
+
+    Args:
+        phenopacket_dir (Path): Directory containing the phenopacket files.
+        disease_pg (pl.DataFrame): DataFrame containing disease.pg entries.
+        output_dir (Path): Directory to store the updated phenopackets.
+    """
+    hgnc_dict = create_hgnc_dict()
+    identifier_map = create_gene_identifier_map()
     gene_identifier_updater = GeneIdentifierUpdater(
         gene_identifier="ensembl_id", hgnc_data=hgnc_dict, identifier_map=identifier_map
     )
     for phenopacket_path in all_files(phenopacket_dir):
         add_genes(phenopacket_path, disease_pg, gene_identifier_updater, output_dir)
```

### Comparing `phenotype2phenopacket-0.4.0/src/phenotype2phenopacket/cli_add.py` & `phenotype2phenopacket-0.5.1/src/phenotype2phenopacket/cli_add.py`

 * *Files 22% similar despite different names*

```diff
@@ -18,35 +18,33 @@
     "--disease-pg",
     "-d",
     required=True,
     help="Path to disease.pg data file.",
     type=Path,
 )
 @click.option(
-    "--hgnc-data",
-    "-h",
-    required=True,
-    help="Path to hgnc_full_set data file.",
-    type=Path,
-)
-@click.option(
     "--output-dir",
     "-o",
     required=True,
     help="Path to output directory.",
     type=Path,
 )
 def add_genes_command(
     phenopacket_dir: Path,
     disease_pg: Path,
-    hgnc_data: Path,
     output_dir: Path,
 ):
-    """Add known gene-to-phenotype relationships to a phenopacket."""
+    """
+    Add known gene-to-phenotype relationships to a set of phenopackets in a directory.
+
+    Args:
+        phenopacket_dir (Path): Directory containing the phenopacket files.
+        disease_pg (Path): Path to the disease.pg file.
+        output_dir (Path): Directory to store the updated phenopackets.
+    """
     output_dir.mkdir(exist_ok=True)
     disease_pg_df = read_disease_pg(disease_pg)
     add_genes_to_directory(
         phenopacket_dir,
         disease_pg_df,
-        hgnc_data,
         output_dir,
     )
```

### Comparing `phenotype2phenopacket-0.4.0/src/phenotype2phenopacket/create/create.py` & `phenotype2phenopacket-0.5.1/src/phenotype2phenopacket/convert/convert.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,58 +1,39 @@
-import random
 from pathlib import Path
 
-import polars as pl
-
 from phenotype2phenopacket.utils.phenopacket_utils import (
     PhenotypeAnnotationToPhenopacketConverter,
-    SyntheticPatientGenerator,
     write_phenopacket,
 )
 from phenotype2phenopacket.utils.utils import (
-    get_phenotype_annotation_version,
+    filter_diseases,
     load_ontology,
-    load_ontology_factory,
-    read_phenotype_annotation_file,
+    return_phenotype_annotation_data,
 )
 
 
-def create_synthetic_patient_phenopacket(
-    human_phenotype_ontology,
-    omim_disease: pl.DataFrame,
-    ontology_factory,
-    output_dir: Path,
-    hpoa_version: str,
+def convert_to_phenopackets(
+    phenotype_annotation: Path, num_disease: int, omim_id: str, omim_id_list: Path, output_dir: Path
 ):
-    """Create a synthetic patient phenopacket from a set of phenotype entries for a specific OMIM disease."""
-    synthetic_patient_generator = SyntheticPatientGenerator(
-        omim_disease, human_phenotype_ontology, ontology_factory
-    )
-    patient_terms = synthetic_patient_generator.patient_term_annotation_set()
-    phenopacket_file = PhenotypeAnnotationToPhenopacketConverter(
-        human_phenotype_ontology
-    ).create_phenopacket(patient_terms, hpoa_version, synthetic_patient_generator.get_onset_range())
-    write_phenopacket(
-        phenopacket_file.phenopacket, output_dir.joinpath(phenopacket_file.phenopacket_path)
-    )
+    """
+    Convert a phenotype annotation file to a set of disease-specific phenopackets.
 
-
-def create_synthetic_patients(phenotype_annotation: Path, num_disease: int, output_dir: Path):
-    """Create a set of synthetic patient phenopackets from a phenotype annotation file."""
-    phenotype_annotation_df = read_phenotype_annotation_file(phenotype_annotation)
-    phenotype_annotation_version = get_phenotype_annotation_version(phenotype_annotation)
+    Args:
+        phenotype_annotation (Path): Path to the phenotype annotation file.
+        num_disease (int): Number of diseases to convert to phenopackets.
+                           If set to 0, processes all available diseases.
+        omim_id (str) : OMIM ID to generate synthetic patient phenopackets for.
+        omim_id_list (Path) : Path to the list of OMIM IDs to generate synthetic patient phenopackets for.
+        output_dir (Path): Directory path to write the generated phenopackets.
+    """
     human_phenotype_ontology = load_ontology()
-    ontology_factory = load_ontology_factory()
-    omim_diseases = phenotype_annotation_df.filter(
-        pl.col("database_id").str.starts_with("OMIM")
-    ).filter(pl.col("aspect") == "P")
-    grouped_omim_diseases = omim_diseases.partition_by(by="database_id", maintain_order=True)
-    if num_disease != 0:
-        grouped_omim_diseases = random.sample(grouped_omim_diseases, num_disease)
+    phenotype_annotation_data = return_phenotype_annotation_data(phenotype_annotation)
+    grouped_omim_diseases = filter_diseases(
+        num_disease, omim_id, omim_id_list, phenotype_annotation_data
+    )
     for omim_disease in grouped_omim_diseases:
-        create_synthetic_patient_phenopacket(
-            human_phenotype_ontology,
-            omim_disease,
-            ontology_factory,
-            output_dir,
-            phenotype_annotation_version,
+        phenopacket_file = PhenotypeAnnotationToPhenopacketConverter(
+            human_phenotype_ontology
+        ).create_phenopacket(omim_disease, phenotype_annotation_data.version)
+        write_phenopacket(
+            phenopacket_file.phenopacket, output_dir.joinpath(phenopacket_file.phenopacket_path)
         )
```

### Comparing `phenotype2phenopacket-0.4.0/src/phenotype2phenopacket/resources/hgnc_complete_set_2023-04-01.txt` & `phenotype2phenopacket-0.5.1/src/phenotype2phenopacket/resources/hgnc_complete_set_2023-04-01.txt`

 * *Files identical despite different names*

### Comparing `phenotype2phenopacket-0.4.0/src/phenotype2phenopacket/utils/phenopacket_utils.py` & `phenotype2phenopacket-0.5.1/src/phenotype2phenopacket/utils/phenopacket_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,52 @@
-import json
 import re
 import secrets
-import signal
+import threading
+import warnings
 from copy import copy
 from dataclasses import dataclass
 from fractions import Fraction
 from pathlib import Path
-from typing import Union
+from typing import List, Union
 
 import polars as pl
-from google.protobuf.json_format import MessageToJson, Parse
 from google.protobuf.timestamp_pb2 import Timestamp
+from oaklib.implementations import ProntoImplementation
 from phenopackets import (
     Age,
     Diagnosis,
     Disease,
-    Family,
     GeneDescriptor,
     GenomicInterpretation,
     Individual,
     Interpretation,
     MetaData,
     OntologyClass,
     Phenopacket,
     PhenotypicFeature,
     Resource,
     TimeElement,
 )
+from pheval.utils.phenopacket_utils import GeneIdentifierUpdater, create_json_message
 
-from phenotype2phenopacket.utils.gene_map_utils import GeneIdentifierUpdater
 from phenotype2phenopacket.utils.utils import is_float
 
 
 @dataclass
 class FrequencyTerm:
+    """
+    Represents a frequency range with upper and lower values.
+
+    Attributes:
+        lower (Union[int, str]): The lower bound of the frequency range.
+            Can be an integer or a string representing the lower frequency value.
+        upper (Union[int, str]): The upper bound of the frequency range.
+            Can be an integer or a string representing the upper frequency value.
+    """
+
     lower: Union[int, str]
     upper: Union[int, str]
 
 
 frequency_hpo = {
     "HP:0040281": FrequencyTerm(0, 0),
     "HP:0040282": FrequencyTerm(1, 4),
@@ -47,14 +56,24 @@
     "HP:0040286": FrequencyTerm(100, 100),
     "HP:0040280": FrequencyTerm(100, 100),
 }
 
 
 @dataclass
 class OnsetTerm:
+    """
+    Represents a range of onset ages with the lowest and highest values.
+
+    Attributes:
+        lower_age (Union[int, str]): The lowest age of onset.
+            Can be an integer or a string representing the lowest age value.
+        upper_age (Union[int, str]): The highest age of onset.
+            Can be an integer or a string representing the highest age value.
+    """
+
     lower_age: Union[int, str]
     upper_age: Union[int, str]
 
 
 onset_hpo = {
     "HP:0011462": OnsetTerm(16, 40),
     "HP:0011460": OnsetTerm(0, 0),
@@ -75,106 +94,151 @@
     "HP:0003623": OnsetTerm(0, 0),
     "HP:0034199": OnsetTerm(0, 0),
     "HP:0003581": OnsetTerm(16, 80),
     "HP:0025710": OnsetTerm(25, 40),
 }
 
 
-def handler(signum, frame):
-    raise TimeoutError("Took too long to filter terms.")
-
-
 @dataclass
 class PhenopacketFile:
-    phenopacket: Phenopacket
-    phenopacket_path: Path
+    """
+    Represents a proband presented as a Phenopacket object and the corresponding phenopacket file name.
 
+    Attributes:
+        phenopacket: Phenopacket object of the proband.
+        phenopacket_path: Path to the phenopacket file.
+    """
 
-def phenopacket_reader(file: Path):
-    """Reads a phenopacket file, returning its contents."""
-    file = open(file, "r")
-    phenopacket = json.load(file)
-    file.close()
-    if "proband" in phenopacket:
-        return Parse(json.dumps(phenopacket), Family())
-    else:
-        return Parse(json.dumps(phenopacket), Phenopacket())
+    phenopacket: Phenopacket
+    phenopacket_path: Path
 
 
 def create_phenopacket_file_name_from_disease(disease_name: str) -> Path:
+    """
+    Create a Phenopacket file name from the disease.
+
+    Args:
+        disease_name (str): The name of the disease.
+    """
     normalised_string = re.sub(r"\W+", "_", disease_name)
     return Path(normalised_string.replace(" ", "_") + ".json")
 
 
-def create_json_message(phenopacket: Phenopacket) -> str:
-    """Create json message for writing to file."""
-    return MessageToJson(phenopacket)
-
-
-def write_phenopacket(phenopacket: Phenopacket, output_file: Path) -> Path:
-    """Write a phenopacket."""
+def write_phenopacket(phenopacket: Phenopacket, output_file: Path) -> None:
+    """
+    Write a Phenopacket object to a file in JSON format.
+
+    Args:
+        phenopacket (Phenopacket): The Phenopacket object to be written.
+        output_file (Path): The Path object representing the file to write the Phenopacket data.
+    """
     phenopacket_json = create_json_message(phenopacket)
     suffix = 1
-    while Path(
-        output_file.parents[0].joinpath(f"{output_file.stem}_patient_{suffix}.json")
-    ).is_file():
-        suffix += 1
-    output_file = output_file.parents[0].joinpath(f"{output_file.stem}_patient_{suffix}.json")
+    if "_patient_" not in output_file.stem:
+        while Path(
+            output_file.parents[0].joinpath(f"{output_file.stem}_patient_{suffix}.json")
+        ).is_file():
+            suffix += 1
+        output_file = output_file.parents[0].joinpath(f"{output_file.stem}_patient_{suffix}.json")
+    else:
+        pass
     with open(output_file, "w") as file:
         file.write(phenopacket_json)
     file.close()
 
 
 class SyntheticPatientGenerator:
-    def __init__(self, disease_df: pl.DataFrame, ontology, ontology_factory):
+    """Class for generating synthetic patients."""
+
+    def __init__(self, disease_df: pl.DataFrame, ontology: ProntoImplementation):
+        """
+        Initialise the SyntheticPatientGenerator class
+
+        Args:
+            disease_df (pl.DataFrame): The dataframe containing the annotation data for a specific disease.
+            ontology (ProntoImplementation): An instance of ProntoImplementation containing the loaded HPO.
+
+        """
         self.disease_df = disease_df
         self.ontology = ontology
-        self.ontology_factory = ontology_factory
         self.lower_age = 0
         self.upper_age = 0
         self.filtered_df = []
         self.secret_rand = secrets.SystemRandom()
 
-    def get_number_of_terms(self):
-        """Get number of terms to ascribe from full set."""
+    def get_number_of_terms(self) -> int:
+        """
+        Get the number of terms to ascribe from the full set.
+
+        Returns:
+            int: Number of terms to ascribe from the full set.
+        """
         if len(self.disease_df) == 1:
             return 1
         number_of_terms = 0
         while number_of_terms == 0:
             number_of_terms = int(len(self.disease_df) * (self.secret_rand.uniform(0.2, 0.75)))
         return number_of_terms
 
     @staticmethod
-    def shuffle_dataframe(disease_df: pl.DataFrame):
-        """Shuffle dataframe."""
+    def shuffle_dataframe(disease_df: pl.DataFrame) -> pl.DataFrame:
+        """
+        Shuffle the rows of a dataframe.
+
+        Args:
+            disease_df (pl.DataFrame): The dataframe containing the annotation data for a specific disease
+
+        Returns:
+            pl.DataFrame: The shuffled dataframe
+        """
         return disease_df.sample(fraction=1, shuffle=True)
 
-    def add_frequency(self):
-        """Add random frequency to annotations without one defined."""
+    def add_frequency(self) -> pl.DataFrame:
+        """
+        Add random frequency to annotations without one defined.
+
+        Returns:
+            pl.DataFrame: DataFrame with random frequency added to annotations without one defined.
+        """
         return self.disease_df.with_columns(
             [
                 pl.when(self.disease_df["frequency"].is_null())
                 .then(pl.lit(self.secret_rand.uniform(0, 1)))
                 .otherwise(self.disease_df["frequency"])
                 .alias("frequency")
             ]
         )
 
-    def get_onset_range(self):
-        """Get the onset range from a set of annotations for a disease."""
+    def get_onset_range(self) -> OnsetTerm:
+        """
+        Get the onset range from a set of annotations for a disease.
+
+        Returns:
+            OnsetTerm: An instance of OnsetTerm representing the onset range from the annotations.
+        """
         for phenotype_entry in self.disease_df.rows(named=True):
             if phenotype_entry["onset"] is not None:
-                if self.lower_age < float(onset_hpo[phenotype_entry["onset"]].lower_age):
-                    self.lower_age = float(onset_hpo[phenotype_entry["onset"]].lower_age)
-                if self.upper_age < float(onset_hpo[phenotype_entry["onset"]].upper_age):
-                    self.upper_age = float(onset_hpo[phenotype_entry["onset"]].upper_age)
+                if self.lower_age < int(onset_hpo[phenotype_entry["onset"]].lower_age):
+                    self.lower_age = int(onset_hpo[phenotype_entry["onset"]].lower_age)
+                if self.upper_age < int(onset_hpo[phenotype_entry["onset"]].upper_age):
+                    self.upper_age = int(onset_hpo[phenotype_entry["onset"]].upper_age)
         return OnsetTerm(lower_age=self.lower_age, upper_age=self.upper_age)
 
-    def check_hpo_frequency(self, phenotype_entry: dict):
-        """Filter with HPO defined frequencies."""
+    def check_hpo_frequency(self, phenotype_entry: dict) -> None:
+        """
+        Filter annotations based on HPO-defined frequencies.
+
+        Args:
+            phenotype_entry (dict): A dictionary representing an HPO phenotype entry.
+
+        Notes:
+            This method filters phenotype entries based on their defined frequencies from the HPO database.
+            If the frequency is 100-100 or if a random frequency falls within the defined limits,
+            the phenotype_entry will be appended to the filtered list.
+        """
         frequency_limits = frequency_hpo[phenotype_entry["frequency"]]
         if (
             frequency_limits.lower == 100
             and frequency_limits.upper == 100
             and phenotype_entry not in self.filtered_df
         ):
             self.filtered_df.append(phenotype_entry)
@@ -185,112 +249,242 @@
                 and phenotype_entry not in self.filtered_df
             ):
                 self.filtered_df.append(phenotype_entry)
 
     def check_frequency_threshold(
         self, frequency: float, phenotype_entry: dict, random_frequency: float
     ):
-        """Check if patient frequency meets the filter for the disease frequency."""
+        """
+        Check if patient frequency meets the filter for the disease frequency.
+
+        Args:
+            frequency (float): The disease frequency threshold.
+            phenotype_entry (dict): A dictionary representing an HPO phenotype entry.
+            random_frequency (float): The random frequency of the patient.
+
+        Notes:
+            This method compares the patient's random frequency against the disease frequency threshold.
+            If the patient's random frequency is less than or equal to the disease frequency and
+            the phenotype_entry is not already in the filtered list, it will be appended.
+        """
         if random_frequency <= float(frequency) and phenotype_entry not in self.filtered_df:
             self.filtered_df.append(phenotype_entry)
         else:
             pass
 
     def check_percentage_frequency(self, phenotype_entry: dict):
-        """Filter with percentage frequency."""
+        """
+        Filter annotations with percentage-based frequency.
+
+        Args:
+            phenotype_entry (dict): A dictionary representing an HPO phenotype entry.
+        """
         frequency = phenotype_entry["frequency"].strip("%")
         random_frequency = self.secret_rand.uniform(0, 100)
         self.check_frequency_threshold(frequency, phenotype_entry, random_frequency)
 
     def check_fraction_frequency(self, phenotype_entry: dict):
-        """Filter with fraction frequency."""
+        """
+        Filter annotations with fraction-based frequency.
+
+        Args:
+            phenotype_entry (dict): A dictionary representing an HPO phenotype entry.
+        """
         random_frequency = self.secret_rand.uniform(0, 1)
         frequency = float(Fraction(phenotype_entry["frequency"]))
         self.check_frequency_threshold(frequency, phenotype_entry, random_frequency)
 
     def check_float_frequency(self, phenotype_entry: dict):
-        """Filter with float threshold."""
+        """
+        Filter annotations with float-based frequency.
+
+        Args:
+            phenotype_entry (dict): A dictionary representing an HPO phenotype entry.
+        """
         random_frequency = self.secret_rand.uniform(0, 1)
         frequency = float((phenotype_entry["frequency"]))
         self.check_frequency_threshold(frequency, phenotype_entry, random_frequency)
 
     def check_frequency(self, phenotype_entry: dict):
-        """Filter for frequency."""
+        """
+        Filter phenotype entries based on different types of frequency representations.
+
+        Args:
+            phenotype_entry (dict): A dictionary representing an HPO phenotype entry.
+
+        Notes:
+            This method categorises and filters phenotype entries based on different types of frequency representations:
+            HPO-defined frequencies starting with "HP:",
+            percentage-based frequencies ending with "%",
+            frequencies represented as fractions (containing "/"),
+            and frequencies represented as floating-point numbers.
+        """
         if str(phenotype_entry["frequency"]).startswith("HP:"):
             self.check_hpo_frequency(phenotype_entry)
         elif str(phenotype_entry["frequency"]).endswith("%"):
             self.check_percentage_frequency(phenotype_entry)
         elif "/" in str(phenotype_entry["frequency"]):
             self.check_fraction_frequency(phenotype_entry)
         elif is_float(phenotype_entry["frequency"]) is True:
             self.check_float_frequency(phenotype_entry)
 
     def filter_phenotype_entries(self, frequency_df: pl.DataFrame, max_number: int):
-        """Filter annotations based on frequency."""
+        """
+        Filter annotations based on frequency.
+
+        Args:
+            frequency_df (pl.DataFrame): DataFrame containing phenotype frequency data.
+            max_number (int): Maximum number of phenotype entries to filter.
+
+        Returns:
+            pl.DataFrame: Filtered phenotype entries DataFrame.
+
+        Notes:
+            This method filters phenotype entries based on frequency constraints until the maximum number is reached.
+            It sets a time limit for execution and handles timeouts by returning filtered results or sampled data.
+        """
         time_limit = 15
-        signal.signal(signal.SIGALRM, handler)
-        signal.alarm(time_limit)
-        try:
-            while len(self.filtered_df) < max_number:
-                for phenotype_entry in frequency_df.rows(named=True):
-                    if len(self.filtered_df) >= max_number:
-                        break
-                    self.check_frequency(phenotype_entry)
-            return pl.from_dicts(self.filtered_df)
-        except TimeoutError:
+
+        def worker():
+            try:
+                while len(self.filtered_df) < max_number:
+                    for phenotype_entry in frequency_df.rows(named=True):
+                        if len(self.filtered_df) >= max_number:
+                            break
+                        self.check_frequency(phenotype_entry)
+            except Exception as e:
+                print("Error in worker thread:", e)
+
+        thread = threading.Thread(target=worker)
+        thread.daemon = True
+        stop_event = threading.Event()
+        thread.start()
+        thread.join(timeout=time_limit)
+
+        if thread.is_alive():
+            stop_event.set()
+            print("Timed out!")
             if len(self.filtered_df) == 0:
                 return frequency_df.sample(n=max_number)
             else:
                 return pl.from_dicts(self.filtered_df)
-        finally:
-            signal.alarm(0)
+        else:
+            return pl.from_dicts(self.filtered_df)
 
-    def get_patient_terms(self):
-        """Get patient terms, filtered on frequency thresholds."""
+    def get_patient_terms(self) -> pl.DataFrame:
+        """
+        Get patient terms filtered on frequency thresholds.
+
+        Returns:
+            pl.DataFrame: DataFrame containing patient terms filtered on frequency thresholds.
+
+        Notes:
+            This method retrieves patient terms by applying various filters based on frequency thresholds.
+            It shuffles the dataframe, adds frequency information, and filters phenotype entries
+            based on frequency constraints to obtain patient terms.
+        """
         return self.filter_phenotype_entries(
             self.shuffle_dataframe(self.add_frequency()), self.get_number_of_terms()
         )
 
-    def get_number_of_terms_to_randomise(self, patient_terms: pl.DataFrame):
-        """Get number of terms to randomise from filtered frequency set."""
+    def get_number_of_terms_to_randomise(self, patient_terms: pl.DataFrame) -> int:
+        """
+        Get the number of terms to randomise from the filtered frequency set.
+
+        Args:
+            patient_terms (pl.DataFrame): DataFrame containing the filtered frequency set of patient terms.
+
+        Returns:
+            int: Number of terms to be randomly selected from the filtered frequency set.
+        """
         return self.secret_rand.randint(0, int(len(patient_terms)))
 
-    def get_number_of_steps_for_randomisation(self):
-        """Get the number of steps to take in range 1-5 for making a term more/less specific."""
+    def get_number_of_steps_for_randomisation(self) -> int:
+        """
+        Get the number of steps to take in the range of 1-5 for making a term more or less specific.
+
+        Returns:
+            int: Number of steps to adjust a term's specificity during randomization (1 to 5).
+        """
         return self.secret_rand.randint(1, 5)
 
-    def return_less_or_more_specific(self):
-        """Generate a float between 0-1."""
+    def return_less_or_more_specific(self) -> float:
+        """
+        Generate a random float between 0 and 1.
+
+        Returns:
+            float: A random float value between 0 and 1.
+        """
         return self.secret_rand.random()
 
-    def subsample_patient_terms(self, patient_terms: pl.dataframe):
-        """Get a subsample of patient terms to make more/less specific."""
+    def subsample_patient_terms(self, patient_terms: pl.dataframe) -> pl.dataframe:
+        """
+        Get a subsample of patient terms to make more or less specific.
+
+
+        Args:
+            patient_terms (pl.DataFrame): DataFrame containing patient terms.
+
+        Returns:
+            pl.DataFrame: Subsample of patient terms for making more or less specific.
+        """
         return patient_terms.sample(self.get_number_of_terms_to_randomise(patient_terms))
 
-    def get_children_of_term(self, phenotype_entry: dict, steps: int):
-        """Get a child term of a hpo id from the number of steps specified."""
+    def get_children_of_term(self, phenotype_entry: dict, steps: int) -> dict:
+        """
+        Get a child term of an HPO ID from the specified number of steps.
+
+        Args:
+            phenotype_entry (dict): A dictionary representing an HPO phenotype entry.
+            steps (int): The number of steps to search for child terms.
+
+        Returns:
+            dict: A dictionary representing the updated phenotype entry with a new HPO ID.
+
+        Notes:
+            This method retrieves a child term of an HPO ID based on the specified number of steps.
+            It iterates through the ontology to find descendants of the given HPO ID
+            and selects a child term randomly if available within the specified steps.
+        """
         term_id = phenotype_entry["hpo_id"]
         for _i in range(steps):
-            descendants = self.ontology_factory.children(term_id)
+            descendants = list(self.ontology.incoming_relationships(term_id))
             if descendants:
-                term_id = self.secret_rand.choice(descendants)
+                term_id = self.secret_rand.choice(descendants)[1]
             else:
                 break
         phenotype_entry["hpo_id"] = term_id
         return phenotype_entry
 
-    def get_parents_of_terms(self, phenotype_entry: dict, steps: int):
-        """Get a parent term of a hpo id from the number of steps specified."""
+    def get_parents_of_terms(self, phenotype_entry: dict, steps: int) -> dict:
+        """
+        Get a parent term of an HPO ID from the specified number of steps.
+
+        Args:
+            phenotype_entry (dict): A dictionary representing an HPO phenotype entry.
+            steps (int): The number of steps to search for parent terms.
+
+        Returns:
+            dict: A dictionary representing the updated phenotype entry with a new HPO ID.
+
+        Notes:
+            This method retrieves a parent term of an HPO ID based on the specified number of steps.
+            It iterates through the ontology to find hierarchical parents of the given HPO ID
+            and selects a parent term randomly if available within the specified steps.
+        """
         term_id = phenotype_entry["hpo_id"]
         rels = self.ontology.entity_alias_map(term_id)
         term = "".join(rels[(list(rels.keys())[0])])
         if term.startswith("Abnormality of"):
             return phenotype_entry
         for _i in range(steps):
             parents = self.ontology.hierarchical_parents(term_id)
+            if not parents:
+                warnings.warn(f"No parents found for term {term}", stacklevel=2)
+                return phenotype_entry
             parent = self.secret_rand.choice(parents)
             rels = self.ontology.entity_alias_map(parent)
             term = "".join(rels[(list(rels.keys())[0])])
             if (
                 term.startswith("Abnormality of")
                 or term_id == "HP:0000118"
                 or term_id == "HP:0032443"
@@ -298,40 +492,77 @@
                 break
             else:
                 term_id = parent
         phenotype_entry["hpo_id"] = term_id
         return phenotype_entry
 
     @staticmethod
-    def remove_terms_to_be_randomised(patient_terms: pl.DataFrame, subset: pl.DataFrame):
-        """Remove terms selected to be randomised from patient terms."""
+    def remove_terms_to_be_randomised(
+        patient_terms: pl.DataFrame, subset: pl.DataFrame
+    ) -> pl.DataFrame:
+        """
+        Remove terms selected for randomisation from patient terms.
+
+        Args:
+            patient_terms (pl.DataFrame): DataFrame containing patient terms.
+            subset (pl.DataFrame): DataFrame representing terms selected for randomisation.
+
+        Returns:
+            pl.DataFrame: DataFrame with selected terms removed for randomisation.
+        """
         subset_list = subset.to_dicts()
         for phenotype_entry in subset_list:
             patient_terms = patient_terms.filter(pl.col("hpo_id") != phenotype_entry["hpo_id"])
         return patient_terms
 
-    def alter_term_specificity(self, new_phenotype_terms: [dict], phenotype_entry: dict):
-        """Alter the hpo id specificity - making less specific if the float is less than 0.5,
-        otherwise the term is made more specific."""
+    def alter_term_specificity(
+        self, new_phenotype_terms: List[dict], phenotype_entry: dict
+    ) -> List[dict]:
+        """
+        Alter the specificity of the HPO ID.
+
+        Args:
+            new_phenotype_terms (List[dict]): List containing updated phenotype terms.
+            phenotype_entry (dict): A dictionary representing an HPO phenotype entry.
+
+        Returns:
+            List[dict]: Updated list of phenotype terms with altered specificity.
+
+        Notes:
+            This method adjusts the specificity of the HPO ID by making it less specific
+            if a randomly generated float is less than 0.5; otherwise, it makes the term more specific.
+        """
         if self.return_less_or_more_specific() < 0.5:
             new_phenotype_terms.append(
                 self.get_parents_of_terms(
                     phenotype_entry, self.get_number_of_steps_for_randomisation()
                 )
             )
         else:
             new_phenotype_terms.append(
                 self.get_children_of_term(
                     phenotype_entry, self.get_number_of_steps_for_randomisation()
                 )
             )
         return new_phenotype_terms
 
-    def patient_term_annotation_set(self):
-        """Get the final patient term annotation set."""
+    def patient_term_annotation_set(self) -> pl.DataFrame:
+        """
+        Get the final patient term annotation set.
+
+        This method generates the final set of patient term annotations by performing the following steps:
+        1. Retrieves patient terms and returns them if only one term is present.
+        2. Sub-samples patient terms to create a smaller subset.
+        3. Alters the specificity of each phenotype entry in the subset.
+        4. Removes terms selected for randomisation from the full patient terms.
+        5. Combines the altered terms with the filtered terms to form the final patient term set.
+
+        Returns:
+            pl.DataFrame: DataFrame containing the final patient term annotation set.
+        """
         patient_terms = self.get_patient_terms()
         if len(patient_terms) == 1:
             return patient_terms
         patient_terms_sub_sample = self.subsample_patient_terms(patient_terms)
         new_phenotype_terms = []
         for phenotype_entry in patient_terms_sub_sample.rows(named=True):
             new_phenotype_terms = self.alter_term_specificity(new_phenotype_terms, phenotype_entry)
@@ -339,122 +570,214 @@
             patient_terms, patient_terms_sub_sample
         )
         final_patient_terms = patient_terms_filtered.to_dicts() + new_phenotype_terms
         return pl.from_dicts(final_patient_terms)
 
 
 class PhenotypeAnnotationToPhenopacketConverter:
-    def __init__(self, human_phenotype_ontology):
+    """Class for converting a set of phenotype annotations to a phenopacket format."""
+
+    def __init__(self, human_phenotype_ontology: ProntoImplementation):
+        """
+        Initialise the PhenotypeAnnotationToPhenopacketConverter class.
+
+        Args:
+            human_phenotype_ontology (ProntoImplementation): An instance of ProntoImplementation
+            containing the loaded HPO.
+        """
+
         self.human_phenotype_ontology = human_phenotype_ontology
         self.secrets_random_num = secrets.SystemRandom()
 
-    def create_individual(self, onset_range: OnsetTerm = None) -> Individual:
-        """Create an Individual object."""
+    def create_individual(
+        self, onset_range: OnsetTerm = None, pt_id: str = "patient1"
+    ) -> Individual:
+        """
+        Create an Individual object.
+
+        Args:
+            onset_range (OnsetTerm, optional): An OnsetTerm object representing the age range of onset.
+            Defaults to None.
+            pt_id (str, optional): An identifier for the patient.
+
+        Returns:
+            Individual: An instance of the Individual class.
+        """
         age = (
             self.secrets_random_num.randint(onset_range.lower_age, onset_range.upper_age)
             if onset_range is not None
             else None
         )
         if onset_range is None or onset_range.upper_age == 0 and onset_range.lower_age == 0:
             age = None
         return Individual(
-            id="patient1",
-            time_at_last_encounter=TimeElement(age=Age(iso8601duration=f"P{age}Y"))
-            if age is not None
-            else None,
+            id="patient1" if pt_id is None else pt_id,
+            time_at_last_encounter=(
+                TimeElement(age=Age(iso8601duration=f"P{age}Y")) if age is not None else None
+            ),
         )
 
     def create_onset(self, phenotype_annotation_entry: dict) -> TimeElement:
-        """Create an Onset object."""
+        """
+        Create an Onset object.
+
+        This method creates a TimeElement representing the onset information for a phenotype annotation entry.
+
+        Args:
+            phenotype_annotation_entry (dict): A dictionary representing a phenotype annotation entry.
+
+        Returns:
+            TimeElement or None: An instance of TimeElement if onset information is available, else None.
+        """
         if phenotype_annotation_entry["onset"] is not None:
             rels = self.human_phenotype_ontology.entity_alias_map(
                 phenotype_annotation_entry["onset"]
             )
             term = "".join(rels[(list(rels.keys())[0])])
             return TimeElement(
                 ontology_class=OntologyClass(id=phenotype_annotation_entry["onset"], label=term)
             )
         else:
             return None
 
-    def create_modifier(self, phenotype_annotation_entry: dict) -> [OntologyClass]:
-        """Create a Modifier."""
+    def create_modifier(self, phenotype_annotation_entry: dict) -> List[OntologyClass]:
+        """
+        Create a Modifier.
+
+        This method creates an OntologyClass representing the modifier information for a phenotype annotation entry.
+
+        Args:
+            phenotype_annotation_entry (dict): A dictionary representing a phenotype annotation entry.
+
+        Returns:
+            list[OntologyClass] or None: A list containing an OntologyClass if modifier information exists,
+                                          otherwise returns None.
+        """
         if phenotype_annotation_entry["modifier"] is not None:
             try:
                 rels = self.human_phenotype_ontology.entity_alias_map(
                     phenotype_annotation_entry["modifier"]
                 )
                 term = "".join(rels[(list(rels.keys())[0])])
                 return [OntologyClass(id=phenotype_annotation_entry["modifier"], label=term)]
             except IndexError:
                 return [OntologyClass(id=phenotype_annotation_entry["modifier"])]
         else:
             return None
 
     def create_phenotypic_feature(self, phenotype_annotation_entry: dict) -> PhenotypicFeature:
-        """Create a PhenotypicFeature object."""
+        """
+        Create a PhenotypicFeature object.
+
+        This method generates a PhenotypicFeature object based on a phenotype annotation entry.
+
+        Args:
+            phenotype_annotation_entry (dict): A dictionary representing a phenotype annotation entry.
+
+        Returns:
+            PhenotypicFeature or None: An instance of PhenotypicFeature if the aspect is 'P' (phenotypic),
+            otherwise None.
+        """
         if phenotype_annotation_entry["aspect"] == "P":
             rels = self.human_phenotype_ontology.entity_alias_map(
                 phenotype_annotation_entry["hpo_id"]
             )
             hpo_term = "".join(rels[(list(rels.keys())[0])])
             return PhenotypicFeature(
                 type=OntologyClass(id=phenotype_annotation_entry["hpo_id"], label=hpo_term),
                 onset=self.create_onset(phenotype_annotation_entry),
                 modifiers=self.create_modifier(phenotype_annotation_entry),
                 excluded=True if phenotype_annotation_entry["qualifier"] == "NOT" else False,
             )
         else:
             return None
 
-    def create_phenotypic_features(self, omim_disease_df: pl.DataFrame):
-        """Create a list of phenotypic features."""
+    def create_phenotypic_features(self, omim_disease_df: pl.DataFrame) -> List[PhenotypicFeature]:
+        """
+        Create a list of phenotypic features.
+
+        This method generates a list of PhenotypicFeature objects based on a DataFrame of OMIM disease entries.
+
+        Args:
+            omim_disease_df (pl.DataFrame): DataFrame containing OMIM disease entries.
+
+        Returns:
+            List[PhenotypicFeature]: A list of PhenotypicFeature objects derived from the provided DataFrame.
+        """
         phenotypic_features = []
         for phenotype_annotation_entry in omim_disease_df.rows(named=True):
             phenotypic_feature = self.create_phenotypic_feature(phenotype_annotation_entry)
             if phenotypic_feature is not None:
                 phenotypic_features.append(phenotypic_feature)
         return phenotypic_features
 
     @staticmethod
     def create_disease(phenotype_annotation_entry: dict) -> Disease:
-        """Create a Disease object."""
+        """
+        Create a Disease object.
+        Args:
+            phenotype_annotation_entry (dict): A dictionary representing a phenotype annotation entry.
+
+        Returns:
+            Disease: An instance of Disease representing the disease information.
+        """
         return Disease(
             term=OntologyClass(
                 id=phenotype_annotation_entry["database_id"],
                 label=phenotype_annotation_entry["disease_name"],
             )
         )
 
     @staticmethod
     def create_omim_resource() -> Resource:
-        """Create OMIM resource."""
+        """
+        Create OMIM resource.
+
+        Returns:
+            Resource: An instance of Resource representing the OMIM database resource.
+        """
         return Resource(
             id="omim",
             name="Online Mendelian Inheritance in Man",
             url="https://www.omim.org",
             version="hp/releases/2023-04-18",
             namespace_prefix="OMIM",
             iri_prefix="https://omim.org/entry/",
         )
 
     @staticmethod
     def create_human_phenotype_ontology_resource(hpoa_version: str) -> Resource:
-        """Create human phenotype ontology resource."""
+        """
+        Create human phenotype ontology resource.
+
+        Returns:
+            Resource: An instance of Resource representing the human phenotype ontology resource.
+        """
         return Resource(
             id="hp",
             name="human phenotype ontology",
             url="http://purl.obolibrary.org/obo/hp.owl",
             version="hp/releases/" + hpoa_version,
             namespace_prefix="HP",
             iri_prefix="http://purl.obolibrary.org/obo/HP_",
         )
 
     def create_metadata(self, hpoa_version: str) -> MetaData:
-        """Create metadata"""
+        """
+        Create metadata.
+
+        This method generates metadata for a Phenopacket including timestamp, creator information,
+        associated resources, and Phenopacket schema version.
+
+        Args:
+            hpoa_version (str): Version of the Human Phenotype Ontology Annotation.
+
+        Returns:
+            MetaData: Metadata information for the Phenopacket.
+        """
         timestamp = Timestamp()
         timestamp.GetCurrentTime()
         return MetaData(
             created=timestamp,
             created_by="phenotype2phenopacket",
             resources=[
                 self.create_human_phenotype_ontology_resource(hpoa_version),
@@ -463,60 +786,109 @@
             phenopacket_schema_version="2.0",
         )
 
     def create_phenopacket(
         self,
         omim_disease_df: pl.DataFrame,
         hpoa_version: str,
+        pt_id: str,
         onset: OnsetTerm = None,
     ) -> PhenopacketFile:
-        """Create a Phenopacket object."""
+        """
+        Create a Phenopacket object.
+
+        This method generates a PhenopacketFile containing a Phenopacket object with information
+        from OMIM disease DataFrame, Human Phenotype Ontology Annotation version, and onset term (if available).
+
+        Args:
+            omim_disease_df (pl.DataFrame): DataFrame containing phenotype annotation disease entries.
+            hpoa_version (str): Version of the Human Phenotype Ontology Annotation.
+            pt_id (str): The patient ID. If not given, defaults to "patient1" in create_individual()
+            onset (OnsetTerm, optional): An OnsetTerm object representing the age range of onset. Defaults to None.
+
+        Returns:
+            PhenopacketFile: A class instance containing the phenopacket file name and
+            the generated Phenopacket.
+        """
         phenotypic_features = self.create_phenotypic_features(omim_disease_df)
         phenotype_annotation_entry = omim_disease_df.to_dicts()[0]
         return PhenopacketFile(
             phenopacket=Phenopacket(
                 id=phenotype_annotation_entry["disease_name"].lower().replace(" ", "_"),
-                subject=self.create_individual(onset),
+                subject=self.create_individual(onset, pt_id),
                 phenotypic_features=phenotypic_features,
                 diseases=[self.create_disease(phenotype_annotation_entry)],
                 meta_data=self.create_metadata(hpoa_version),
             ),
             phenopacket_path=create_phenopacket_file_name_from_disease(
                 phenotype_annotation_entry["disease_name"]
             ),
         )
 
 
 class PhenopacketUtil:
+    """Phenopacket utility class."""
+
     def __init__(self, phenopacket: Phenopacket):
+        """
+        Initialise the PhenopacketUtil class.
+
+        Args:
+            phenopacket(Phenopacket): The phenopacket object.
+        """
         self.phenopacket = phenopacket
 
-    def return_phenopacket_disease(self) -> [str]:
-        """Return the disease object from a phenopacket."""
+    def return_phenopacket_disease(self) -> Disease:
+        """
+        Return the disease object from a phenopacket.
+
+        Returns:
+            Disease: The proband disease.
+        """
         return self.phenopacket.diseases[0]
 
 
 class PhenopacketInterpretationExtender:
+    """Class for extending the phenopacket interpretations field."""
+
     def __init__(self, phenopacket: Phenopacket):
+        """
+        Initialise the PhenopacketInterpretationExtender class.
+
+        Args:
+            phenopacket(Phenopacket): The phenopacket object.
+        """
         self.phenopacket = phenopacket
 
     @staticmethod
     def create_gene_genomic_interpretation(
         gene_to_phenotype_entry: dict, gene_identifier_updater: GeneIdentifierUpdater
-    ):
-        """Create genomic interpretation for a gene-to-phenotype relationship."""
+    ) -> GenomicInterpretation:
+        """
+        Create genomic interpretation for a gene-to-phenotype relationship.
+
+        This method generates a GenomicInterpretation object based on a gene-to-phenotype relationship entry.
+
+        Args:
+            gene_to_phenotype_entry (dict): A dictionary representing a gene-to-phenotype relationship.
+            gene_identifier_updater (GeneIdentifierUpdater): An instance of GeneIdentifierUpdater.
+
+        Returns:
+            GenomicInterpretation or None: An instance of GenomicInterpretation representing the interpretation
+                                           of the gene-to-phenotype relationship or None if unsuccessful.
+        """
         try:
             gene_symbol = gene_identifier_updater.obtain_gene_symbol_from_identifier(
                 str(gene_to_phenotype_entry["entrez_id"])
             )
             return GenomicInterpretation(
                 subject_or_biosample_id="patient1",
-                interpretation_status=4
-                if gene_to_phenotype_entry["disease_name"].startswith("?") is False
-                else 0,
+                interpretation_status=(
+                    4 if gene_to_phenotype_entry["disease_name"].startswith("?") is False else 0
+                ),
                 gene=GeneDescriptor(
                     value_id=gene_identifier_updater.find_identifier(gene_symbol),
                     symbol=gene_symbol,
                 ),
             )
         except KeyError:
             print(f"Unable to find gene_symbol for {gene_to_phenotype_entry['entrez_id']}")
@@ -525,32 +897,59 @@
             print("N/A value", gene_to_phenotype_entry)
             return None
 
     def create_gene_genomic_interpretations(
         self,
         omim_disease_phenotype_gene_map: pl.DataFrame,
         gene_identifier_updater: GeneIdentifierUpdater,
-    ):
-        """Create list of genomic interpretations for known gene-to-phenotype relationships."""
+    ) -> List[GenomicInterpretation]:
+        """
+        Create a list of genomic interpretations for known gene-to-phenotype relationships.
+
+        This method generates a list of GenomicInterpretation objects based on a DataFrame
+        containing known gene-to-phenotype relationships.
+
+        Args:
+            omim_disease_phenotype_gene_map (pl.DataFrame): DataFrame containing gene-to-phenotype mappings.
+            gene_identifier_updater (GeneIdentifierUpdater): An instance of GeneIdentifierUpdater.
+
+        Returns:
+            List[GenomicInterpretation]: A list of GenomicInterpretation objects representing the interpretations
+                  of gene-to-phenotype relationships.
+        """
         genomic_interpretations = []
         for phenotype_entry in omim_disease_phenotype_gene_map.rows(named=True):
             genomic_interpretation = self.create_gene_genomic_interpretation(
                 phenotype_entry, gene_identifier_updater
             )
             if genomic_interpretation is not None:
                 genomic_interpretations.append(genomic_interpretation)
         return genomic_interpretations
 
     def create_gene_diagnosis(
         self,
         omim_disease_phenotype_gene_map: pl.DataFrame,
         gene_identifier_updater: GeneIdentifierUpdater,
         disease: Disease,
-    ):
-        """Create a diagnosis object for known gene-to-phenotype relationships."""
+    ) -> Diagnosis:
+        """
+        Create a diagnosis object for known gene-to-phenotype relationships.
+
+        This method generates a Diagnosis object based on known gene-to-phenotype relationships
+        provided in a DataFrame and a Disease object.
+
+        Args:
+            omim_disease_phenotype_gene_map (pl.DataFrame): DataFrame containing gene-to-phenotype mappings.
+            gene_identifier_updater (GeneIdentifierUpdater): An instance of GeneIdentifierUpdater.
+            disease (Disease): An instance of Disease representing the disease information.
+
+        Returns:
+            Diagnosis or None: A Diagnosis object representing the diagnosis based on gene-to-phenotype relationships,
+                               or None if no genomic interpretations were found.
+        """
         genomic_interpretations = self.create_gene_genomic_interpretations(
             omim_disease_phenotype_gene_map, gene_identifier_updater
         )
         return (
             Diagnosis(
                 disease=OntologyClass(
                     id=disease.term.id,
@@ -562,16 +961,29 @@
             else None
         )
 
     def create_gene_interpretation(
         self,
         omim_disease_phenotype_gene_map: pl.DataFrame,
         gene_identifier_updater: GeneIdentifierUpdater,
-    ):
-        """Create an interpretation object for known gene-to-phenotype relationships."""
+    ) -> Interpretation:
+        """
+        Create an interpretation object for known gene-to-phenotype relationships.
+
+        This method generates an Interpretation object based on known gene-to-phenotype relationships
+        provided in a DataFrame and a GeneIdentifierUpdater instance.
+
+        Args:
+            omim_disease_phenotype_gene_map (pl.DataFrame): DataFrame containing gene-to-phenotype mappings.
+            gene_identifier_updater (GeneIdentifierUpdater): An instance of GeneIdentifierUpdater.
+
+        Returns:
+            Interpretation or None: An Interpretation object representing the interpretation based on gene-to-phenotype
+                                    relationships, or None if no diagnosis was created.
+        """
         phenopacket_util = PhenopacketUtil(self.phenopacket)
         disease = phenopacket_util.return_phenopacket_disease()
         diagnosis = self.create_gene_diagnosis(
             omim_disease_phenotype_gene_map, gene_identifier_updater, disease
         )
         return (
             Interpretation(
@@ -583,16 +995,28 @@
             else None
         )
 
     def add_gene_interpretation_to_phenopacket(
         self,
         omim_disease_phenotype_gene_map: pl.DataFrame,
         gene_identifier_updater: GeneIdentifierUpdater,
-    ):
-        """Add interpretations to phenopacket."""
+    ) -> Phenopacket:
+        """
+        Add interpretations to a Phenopacket.
+
+        This method adds gene-based interpretations to a copy of the Phenopacket.
+
+        Args:
+            omim_disease_phenotype_gene_map (pl.DataFrame): DataFrame containing gene-to-phenotype mappings.
+            gene_identifier_updater (GeneIdentifierUpdater): An instance of GeneIdentifierUpdater.
+
+        Returns:
+            Phenopacket or None: A copy of the Phenopacket with added gene-based interpretations,
+            or None if interpretations were not created.
+        """
         phenopacket_copy = copy(self.phenopacket)
         interpretations = [
             self.create_gene_interpretation(
                 omim_disease_phenotype_gene_map, gene_identifier_updater
             )
         ]
         if interpretations is not None:
```

### Comparing `phenotype2phenopacket-0.4.0/PKG-INFO` & `phenotype2phenopacket-0.5.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: phenotype2phenopacket
-Version: 0.4.0
+Version: 0.5.1
 Summary: 
 Author: Yasemin Bridges
 Author-email: y.bridges@qmul.ac.uk
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: oaklib (>=0.5.1,<0.6.0)
-Requires-Dist: ontobio (>=2.8.5,<3.0.0)
 Requires-Dist: pandas (>=1.5.1,<2.0.0)
 Requires-Dist: phenopackets (>=2.0.2,<3.0.0)
-Requires-Dist: polars (>=0.17.5,<0.18.0)
+Requires-Dist: pheval (>=0.3.6,<0.4.0)
+Requires-Dist: polars (>=0.19,<0.20)
 Description-Content-Type: text/markdown
 
 # Phenotype2Phenopacket
 
 _Phenotype2Phenopacket_ is a command-line interface (CLI) application for the construction of phenopackets
 from a phenotype annotation file.
 
@@ -48,14 +48,26 @@
 
 You can also limit the number of disease phenopackets converted/created:
 
 ```shell
 p2p convert --phenotype-annotation /path/to/phenotype.hpoa --output-dir /path/to/output-dir --num-diseases 100
 ```
 
+Or limit for a specific OMIM disease:
+
+```shell
+p2p create --phenotype-annotation /path/to/phenotype.hpoa --output-dir /path/to/output-dir --omim-id OMIM:619340
+```
+
+Or limit for a list of OMIM IDs specified in a text file, with each ID separated by a new line:
+
+```shell
+p2p create --phenotype-annotation /path/to/phenotype.hpoa --output-dir /path/to/output-dir --omim-id-list /path/to/list.txt
+```
+
 To add known gene-to-phenotype relationships to phenopackets:
 
 ```shell
 p2p add-genes --phenopacket-dir /path/to/synthetic-phenopackets --disease-pg /path/to/disease.pg --hgnc-data /path/to/hgnc_complete_set.txt --output-dir /path/to/output-dir
 ```
 
 > **_NOTE:_** To add known gene-to-phenotype the Exomiser disease.pg file is expected
```

