# Comparing `tmp/ontosample-0.2.2.tar.gz` & `tmp/ontosample-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontosample-0.2.2.tar", last modified: Sat Feb 17 15:02:38 2024, max compression
+gzip compressed data, was "ontosample-0.2.3.tar", last modified: Wed May 22 13:32:17 2024, max compression
```

## Comparing `ontosample-0.2.2.tar` & `ontosample-0.2.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2024-02-17 15:02:38.730554 ontosample-0.2.2/
--rw-rw-rw-   0        0        0    35184 2023-06-04 12:41:29.000000 ontosample-0.2.2/LICENSE
--rw-rw-rw-   0        0        0     7753 2024-02-17 15:02:38.729480 ontosample-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     6945 2024-02-15 21:59:40.000000 ontosample-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-02-17 15:02:38.708832 ontosample-0.2.2/ontolearn_light/
--rw-rw-rw-   0        0        0      668 2023-12-11 00:11:09.000000 ontosample-0.2.2/ontolearn_light/__init__.py
--rw-rw-rw-   0        0        0    20279 2024-02-15 21:59:40.000000 ontosample-0.2.2/ontolearn_light/abstracts.py
-drwxrwxrwx   0        0        0        0 2024-02-17 15:02:38.713690 ontosample-0.2.2/ontolearn_light/base/
--rw-rw-rw-   0        0        0      742 2024-02-15 21:59:40.000000 ontosample-0.2.2/ontolearn_light/base/__init__.py
--rw-rw-rw-   0        0        0    45983 2024-02-15 21:59:40.000000 ontosample-0.2.2/ontolearn_light/base/_base.py
--rw-rw-rw-   0        0        0    31749 2024-02-15 21:59:40.000000 ontosample-0.2.2/ontolearn_light/base/axioms.py
--rw-rw-rw-   0        0        0     5258 2024-02-15 21:59:40.000000 ontosample-0.2.2/ontolearn_light/base/complex_ce_instances.py
-drwxrwxrwx   0        0        0        0 2024-02-17 15:02:38.713690 ontosample-0.2.2/ontolearn_light/base/ext/
--rw-rw-rw-   0        0        0     4089 2023-11-21 14:06:28.000000 ontosample-0.2.2/ontolearn_light/base/ext/__init__.py
--rw-rw-rw-   0        0        0    27067 2024-02-15 21:59:40.000000 ontosample-0.2.2/ontolearn_light/base/fast_instance_checker.py
-drwxrwxrwx   0        0        0        0 2024-02-17 15:02:38.716985 ontosample-0.2.2/ontolearn_light/base/owl/
--rw-rw-rw-   0        0        0       20 2023-11-21 13:25:19.000000 ontosample-0.2.2/ontolearn_light/base/owl/__init__.py
--rw-rw-rw-   0        0        0    17414 2023-11-21 14:06:28.000000 ontosample-0.2.2/ontolearn_light/base/owl/hierarchy.py
--rw-rw-rw-   0        0        0    24746 2023-11-21 14:06:28.000000 ontosample-0.2.2/ontolearn_light/base/owl/utils.py
--rw-rw-rw-   0        0        0    15967 2023-11-21 14:06:28.000000 ontosample-0.2.2/ontolearn_light/base/utils.py
--rw-rw-rw-   0        0        0    10196 2024-02-15 21:59:40.000000 ontosample-0.2.2/ontolearn_light/concept_generator.py
--rw-rw-rw-   0        0        0     8566 2023-12-06 22:56:00.000000 ontosample-0.2.2/ontolearn_light/data_struct.py
--rw-rw-rw-   0        0        0      681 2024-02-15 21:59:40.000000 ontosample-0.2.2/ontolearn_light/fitness_functions.py
--rw-rw-rw-   0        0        0    51255 2024-02-15 21:59:40.000000 ontosample-0.2.2/ontolearn_light/knowledge_base.py
--rw-rw-rw-   0        0        0     2841 2024-02-17 12:16:28.000000 ontosample-0.2.2/ontolearn_light/learning_problem.py
--rw-rw-rw-   0        0        0     3192 2023-10-10 12:27:39.000000 ontosample-0.2.2/ontolearn_light/metrics.py
--rw-rw-rw-   0        0        0    27227 2023-12-03 21:04:04.000000 ontosample-0.2.2/ontolearn_light/search.py
-drwxrwxrwx   0        0        0        0 2024-02-17 15:02:38.720100 ontosample-0.2.2/ontolearn_light/utils/
--rw-rw-rw-   0        0        0     6640 2024-02-15 21:59:40.000000 ontosample-0.2.2/ontolearn_light/utils/__init__.py
--rw-rw-rw-   0        0        0     1208 2024-02-15 21:59:40.000000 ontosample-0.2.2/ontolearn_light/utils/log_config.py
--rw-rw-rw-   0        0        0      216 2023-10-12 13:01:03.000000 ontosample-0.2.2/ontolearn_light/utils/oplogging.py
--rw-rw-rw-   0        0        0     3650 2024-02-15 14:37:10.000000 ontosample-0.2.2/ontolearn_light/utils/static_funcs.py
-drwxrwxrwx   0        0        0        0 2024-02-17 15:02:38.723717 ontosample-0.2.2/ontosample/
--rw-rw-rw-   0        0        0        0 2023-11-22 19:49:53.000000 ontosample-0.2.2/ontosample/__init__.py
--rw-rw-rw-   0        0        0    12145 2024-02-17 15:01:54.000000 ontosample-0.2.2/ontosample/_base.py
--rw-rw-rw-   0        0        0    17341 2024-02-16 16:02:28.000000 ontosample-0.2.2/ontosample/classic_samplers.py
--rw-rw-rw-   0        0        0    14058 2024-02-16 16:02:28.000000 ontosample-0.2.2/ontosample/lpc_samplers.py
--rw-rw-rw-   0        0        0     6707 2024-02-16 16:02:28.000000 ontosample-0.2.2/ontosample/lpf_samplers.py
-drwxrwxrwx   0        0        0        0 2024-02-17 15:02:38.729480 ontosample-0.2.2/ontosample.egg-info/
--rw-rw-rw-   0        0        0     7753 2024-02-17 15:02:38.000000 ontosample-0.2.2/ontosample.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1127 2024-02-17 15:02:38.000000 ontosample-0.2.2/ontosample.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-17 15:02:38.000000 ontosample-0.2.2/ontosample.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2024-02-17 15:02:38.000000 ontosample-0.2.2/ontosample.egg-info/requires.txt
--rw-rw-rw-   0        0        0       27 2024-02-17 15:02:38.000000 ontosample-0.2.2/ontosample.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       93 2023-06-04 12:41:29.000000 ontosample-0.2.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-17 15:02:38.730554 ontosample-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1017 2024-02-17 15:01:54.000000 ontosample-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:32:17.365126 ontosample-0.2.3/
+-rw-rw-rw-   0        0        0    35184 2023-06-04 12:41:29.000000 ontosample-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     7753 2024-05-22 13:32:17.363878 ontosample-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6945 2024-02-15 21:59:40.000000 ontosample-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 13:32:17.340467 ontosample-0.2.3/ontolearn_light/
+-rw-rw-rw-   0        0        0       23 2024-05-21 12:09:14.000000 ontosample-0.2.3/ontolearn_light/__init__.py
+-rw-rw-rw-   0        0        0    20532 2024-05-21 14:46:58.000000 ontosample-0.2.3/ontolearn_light/abstracts.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:32:17.344906 ontosample-0.2.3/ontolearn_light/base/
+-rw-rw-rw-   0        0        0      740 2024-05-21 14:36:30.000000 ontosample-0.2.3/ontolearn_light/base/__init__.py
+-rw-rw-rw-   0        0        0    45660 2024-05-21 14:39:38.000000 ontosample-0.2.3/ontolearn_light/base/_base.py
+-rw-rw-rw-   0        0        0    32628 2024-05-21 14:39:38.000000 ontosample-0.2.3/ontolearn_light/base/axioms.py
+-rw-rw-rw-   0        0        0     5345 2024-05-21 14:39:38.000000 ontosample-0.2.3/ontolearn_light/base/complex_ce_instances.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:32:17.346419 ontosample-0.2.3/ontolearn_light/base/ext/
+-rw-rw-rw-   0        0        0     4219 2024-04-22 13:06:57.000000 ontosample-0.2.3/ontolearn_light/base/ext/__init__.py
+-rw-rw-rw-   0        0        0    27223 2024-05-21 14:46:58.000000 ontosample-0.2.3/ontolearn_light/base/fast_instance_checker.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:32:17.349567 ontosample-0.2.3/ontolearn_light/base/owl/
+-rw-rw-rw-   0        0        0       20 2023-11-21 13:25:19.000000 ontosample-0.2.3/ontolearn_light/base/owl/__init__.py
+-rw-rw-rw-   0        0        0    17545 2024-04-22 13:25:14.000000 ontosample-0.2.3/ontolearn_light/base/owl/hierarchy.py
+-rw-rw-rw-   0        0        0    24949 2024-04-22 13:25:14.000000 ontosample-0.2.3/ontolearn_light/base/owl/utils.py
+-rw-rw-rw-   0        0        0    16573 2024-04-23 12:09:16.000000 ontosample-0.2.3/ontolearn_light/base/utils.py
+-rw-rw-rw-   0        0        0    10334 2024-05-21 14:46:58.000000 ontosample-0.2.3/ontolearn_light/concept_generator.py
+-rw-rw-rw-   0        0        0    11689 2024-03-25 16:12:36.000000 ontosample-0.2.3/ontolearn_light/data_struct.py
+-rw-rw-rw-   0        0        0      681 2024-05-21 14:46:58.000000 ontosample-0.2.3/ontolearn_light/fitness_functions.py
+-rw-rw-rw-   0        0        0    55971 2024-05-21 14:46:58.000000 ontosample-0.2.3/ontolearn_light/knowledge_base.py
+-rw-rw-rw-   0        0        0     2850 2024-05-21 14:46:58.000000 ontosample-0.2.3/ontolearn_light/learning_problem.py
+-rw-rw-rw-   0        0        0     3192 2023-10-10 12:27:39.000000 ontosample-0.2.3/ontolearn_light/metrics.py
+-rw-rw-rw-   0        0        0    28669 2024-05-21 12:09:14.000000 ontosample-0.2.3/ontolearn_light/search.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:32:17.353064 ontosample-0.2.3/ontolearn_light/utils/
+-rw-rw-rw-   0        0        0     6780 2024-05-21 14:46:58.000000 ontosample-0.2.3/ontolearn_light/utils/__init__.py
+-rw-rw-rw-   0        0        0     1208 2024-05-21 14:46:58.000000 ontosample-0.2.3/ontolearn_light/utils/log_config.py
+-rw-rw-rw-   0        0        0      216 2023-10-12 13:01:03.000000 ontosample-0.2.3/ontolearn_light/utils/oplogging.py
+-rw-rw-rw-   0        0        0     6298 2024-05-22 13:25:05.000000 ontosample-0.2.3/ontolearn_light/utils/static_funcs.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:32:17.356841 ontosample-0.2.3/ontosample/
+-rw-rw-rw-   0        0        0        0 2023-11-22 19:49:53.000000 ontosample-0.2.3/ontosample/__init__.py
+-rw-rw-rw-   0        0        0    12200 2024-05-21 14:30:42.000000 ontosample-0.2.3/ontosample/_base.py
+-rw-rw-rw-   0        0        0    17350 2024-05-21 14:34:34.000000 ontosample-0.2.3/ontosample/classic_samplers.py
+-rw-rw-rw-   0        0        0    14067 2024-05-21 14:34:34.000000 ontosample-0.2.3/ontosample/lpc_samplers.py
+-rw-rw-rw-   0        0        0     6710 2024-05-21 14:34:34.000000 ontosample-0.2.3/ontosample/lpf_samplers.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:32:17.362607 ontosample-0.2.3/ontosample.egg-info/
+-rw-rw-rw-   0        0        0     7753 2024-05-22 13:32:17.000000 ontosample-0.2.3/ontosample.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1127 2024-05-22 13:32:17.000000 ontosample-0.2.3/ontosample.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 13:32:17.000000 ontosample-0.2.3/ontosample.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2024-05-22 13:32:17.000000 ontosample-0.2.3/ontosample.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       27 2024-05-22 13:32:17.000000 ontosample-0.2.3/ontosample.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       93 2023-06-04 12:41:29.000000 ontosample-0.2.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 13:32:17.365126 ontosample-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1017 2024-05-22 13:29:08.000000 ontosample-0.2.3/setup.py
```

### Comparing `ontosample-0.2.2/LICENSE` & `ontosample-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ontosample-0.2.2/PKG-INFO` & `ontosample-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontosample
-Version: 0.2.2
+Version: 0.2.3
 Summary: Ontosample is a package that offers different sampling techniques for OWL ontologies.
 Home-page: https://github.com/alkidbaci/OntoSample
 Author: Alkid Baci
 Author-email: alkid1baci@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.3.4
 Requires-Dist: owlready2>=0.40
 Requires-Dist: torch>=1.7.1
 Requires-Dist: pandas>=1.5.0
 Requires-Dist: sortedcontainers>=2.4.0
-Requires-Dist: owlapy>=0.1.1
+Requires-Dist: owlapy==1.0.2
 Requires-Dist: requests>=2.31.0
 
 # OntoSample
 
 OntoSample is a python package that offers classic sampling techniques for OWL ontologies/knowledge 
 bases. Furthermore, we have tailored the classic sampling techniques to the setting of concept 
 learning making use of learning problem.
```

### Comparing `ontosample-0.2.2/README.md` & `ontosample-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ontosample-0.2.2/ontolearn_light/abstracts.py` & `ontosample-0.2.3/ontolearn_light/abstracts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """The main abstract classes."""
 
 import logging
 from abc import ABCMeta, abstractmethod
 from typing import Set, List, Tuple, Iterable, TypeVar, Generic, ClassVar, Optional
-
-from owlapy.model import OWLClassExpression, OWLOntology
+from owlapy.class_expression import OWLClassExpression
+from owlapy.owl_ontology import OWLOntology
 from owlapy.util import iter_count
 from .data_struct import Experience
 from .utils import read_csv
 from collections import OrderedDict
+
 _N = TypeVar('_N')  #:
 _KB = TypeVar('_KB', bound='AbstractKnowledgeBase')  #:
 
 logger = logging.getLogger(__name__)
 
 # @TODO:CD: Each Class definiton in abstract.py should share a prefix, e.g., BaseX or AbstractX.
 # @TODO:CD: All imports must be located on top of the script
-
+from owlapy import owl_expression_to_dl
 class EncodedLearningProblem(metaclass=ABCMeta):
     """Encoded Abstract learning problem for use in Scorers."""
     __slots__ = ()
 
 
 class EncodedPosNegLPStandardKind(EncodedLearningProblem, metaclass=ABCMeta):
     """Encoded Abstract learning problem following pos-neg lp standard."""
@@ -324,14 +325,16 @@
         pass
 
 
 class AbstractKnowledgeBase(metaclass=ABCMeta):
     """Abstract knowledge base."""
     __slots__ = ()
 
+    # CD: This function is used as "a get method". Insteadf either access the atttribute directly
+    # or use it as a property @abstractmethod
     def ontology(self) -> OWLOntology:
         """The base ontology of this knowledge base."""
         pass
 
     def describe(self) -> None:
         """Print a short description of the Knowledge Base to the info logger output."""
         properties_count = iter_count(self.ontology.object_properties_in_signature()) + iter_count(
@@ -593,25 +596,27 @@
         self._nodes = OrderedDict(sorted_x)
 
     def best_hypotheses(self, n=10) -> List:
         assert self.search_tree is not None
         assert len(self.search_tree) > 1
         return [i for i in self.search_tree.get_top_n_nodes(n)]
 
-    def show_search_tree(self, th, top_n=10):
+    def show_search_tree(self, top_n=100):
         """
         Show search tree.
         """
-        print(f'######## {th}.step\t Top 10 nodes in Search Tree \t |Search Tree|={self.__len__()} ###########')
         predictions = list(self.get_top_n_nodes(top_n))
-        for ith, node in enumerate(predictions):
-            print(f'{ith + 1}-\t{node}')
         print('######## Search Tree ###########\n')
+        for ith, node in enumerate(predictions):
+            print(f"{ith + 1}-\t{owl_expression_to_dl(node.concept)} | Quality:{node.quality}| Heuristic:{node.heuristic}")
+        print('\n######## Search Tree ###########\n')
         return predictions
 
+
+
     def show_best_nodes(self, top_n, key=None):
         assert key
         self.sort_search_tree_by_decreasing_order(key=key)
         return self.show_search_tree('Final', top_n=top_n + 1)
 
     @staticmethod
     def save_current_top_n_nodes(key=None, n=10, path=None):
```

### Comparing `ontosample-0.2.2/ontolearn_light/base/__init__.py` & `ontosample-0.2.3/ontolearn_light/base/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """Implementations of owlapy abstract classes based on owlready2."""
-from owlapy._utils import MOVE
+from owlapy.util import move
 from ontolearn_light.base._base import OWLOntologyManager_Owlready2, OWLReasoner_Owlready2, \
     OWLOntology_Owlready2, BaseReasoner_Owlready2
 from ontolearn_light.base.complex_ce_instances import OWLReasoner_Owlready2_ComplexCEInstances
 from ontolearn_light.base.fast_instance_checker import OWLReasoner_FastInstanceChecker
-MOVE(OWLOntologyManager_Owlready2, OWLReasoner_Owlready2, OWLOntology_Owlready2, BaseReasoner_Owlready2)
+move(OWLOntologyManager_Owlready2, OWLReasoner_Owlready2, OWLOntology_Owlready2, BaseReasoner_Owlready2)
 __all__ = 'OWLOntologyManager_Owlready2', 'OWLReasoner_Owlready2', 'OWLOntology_Owlready2', 'BaseReasoner_Owlready2', \
     'OWLReasoner_Owlready2_ComplexCEInstances', 'OWLReasoner_FastInstanceChecker'
```

### Comparing `ontosample-0.2.2/ontolearn_light/base/_base.py` & `ontosample-0.2.3/ontolearn_light/base/_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,27 +2,31 @@
 from datetime import date, datetime
 from enum import Enum, auto
 from itertools import chain
 from types import MappingProxyType
 from typing import Iterable, Set, Final, List
 
 import owlready2
+from owlapy.class_expression import OWLClassExpression, OWLThing, OWLClass, OWLObjectSomeValuesFrom
+from owlapy.iri import IRI
+from owlapy.owl_axiom import OWLObjectPropertyRangeAxiom, OWLAxiom, OWLObjectPropertyDomainAxiom, \
+    OWLDataPropertyRangeAxiom, OWLDataPropertyDomainAxiom, OWLClassAxiom, OWLSubClassOfAxiom, OWLEquivalentClassesAxiom
+from owlapy.owl_individual import OWLNamedIndividual
+from owlapy.owl_literal import DoubleOWLDatatype, OWLLiteral, BooleanOWLDatatype, IntegerOWLDatatype, DateOWLDatatype, \
+    DateTimeOWLDatatype, DurationOWLDatatype, StringOWLDatatype
+from owlapy.owl_ontology import OWLOntologyID, OWLOntology
+from owlapy.owl_ontology_manager import OWLOntologyManager, OWLOntologyChange, AddImport
+from owlapy.owl_property import OWLDataProperty, OWLObjectPropertyExpression, OWLObjectInverseOf, OWLObjectProperty
 from owlready2 import declare_datatype
 from pandas import Timedelta
 
-from owlapy.owl2sparql.converter import Owl2SparqlConverter
+from owlapy.converter import Owl2SparqlConverter
 from ontolearn_light.base import axioms
 from owlapy import namespaces
 from ontolearn_light.base.ext import OWLReasonerEx
-from owlapy.model import OWLObjectPropertyRangeAxiom, OWLOntologyManager, OWLDataProperty, \
-    OWLNamedIndividual, OWLClassExpression, OWLObjectPropertyExpression, OWLOntologyID, OWLAxiom, OWLOntology, \
-    OWLOntologyChange, AddImport, OWLThing, DoubleOWLDatatype, OWLObjectPropertyDomainAxiom, OWLLiteral, \
-    OWLObjectInverseOf, BooleanOWLDatatype, IntegerOWLDatatype, DateOWLDatatype, DateTimeOWLDatatype, OWLClass, \
-    DurationOWLDatatype, StringOWLDatatype, IRI, OWLDataPropertyRangeAxiom, OWLDataPropertyDomainAxiom, OWLClassAxiom, \
-    OWLSubClassOfAxiom, OWLEquivalentClassesAxiom, OWLObjectSomeValuesFrom, OWLObjectProperty
 from ontolearn_light.base.utils import FromOwlready2
 
 logger = logging.getLogger(__name__)
 
 _Datatype_map: Final = MappingProxyType({
     int: IntegerOWLDatatype,
     float: DoubleOWLDatatype,
@@ -87,15 +91,15 @@
         return OWLOntology_Owlready2(self, iri, load=True)
 
     def apply_change(self, change: OWLOntologyChange):
         if isinstance(change, AddImport):
             ont_x: owlready2.namespace.Ontology = self._world.get_ontology(
                 change.get_ontology().get_ontology_id().get_ontology_iri().as_str())
             ont_x.imported_ontologies.append(
-                self._world.get_ontology(change.get_import_declaration().get_iri().as_str()))
+                self._world.get_ontology(change.get_import_declaration().str))
         else:
             # TODO XXX
             raise NotImplementedError
 
     def add_axiom(self, ontology: OWLOntology, axiom: OWLAxiom):
         axioms._add_axiom(axiom, ontology, self._world)
 
@@ -155,15 +159,15 @@
             yield OWLObjectProperty(IRI.create(op.iri))
 
     def individuals_in_signature(self) -> Iterable[OWLNamedIndividual]:
         for i in self._onto.individuals():
             yield OWLNamedIndividual(IRI.create(i.iri))
 
     def equivalent_classes_axioms(self, c: OWLClass) -> Iterable[OWLEquivalentClassesAxiom]:
-        c_x: owlready2.ThingClass = self._world[c.get_iri().as_str()]
+        c_x: owlready2.ThingClass = self._world[c.str]
         # TODO: Should this also return EquivalentClasses general class axioms? Compare to java owlapi
         for ec_x in c_x.equivalent_to:
             yield OWLEquivalentClassesAxiom([c, _parse_concept_to_owlapy(ec_x)])
 
     def general_class_axioms(self) -> Iterable[OWLClassAxiom]:
         # TODO: At the moment owlready2 only supports SubClassOf general class axioms. (18.02.2023)
         for ca in self._onto.general_class_axioms():
@@ -183,28 +187,28 @@
         else:
             version_iri = None
 
         return OWLOntologyID(IRI.create(onto_iri) if onto_iri is not None else None,
                              IRI.create(version_iri) if version_iri is not None else None)
 
     def data_property_domain_axioms(self, pe: OWLDataProperty) -> Iterable[OWLDataPropertyDomainAxiom]:
-        p_x: owlready2.DataPropertyClass = self._world[pe.get_iri().as_str()]
+        p_x: owlready2.DataPropertyClass = self._world[pe.str]
         domains = set(p_x.domains_indirect())
         if len(domains) == 0:
             yield OWLDataPropertyDomainAxiom(pe, OWLThing)
         else:
             for dom in domains:
                 if isinstance(dom, (owlready2.ThingClass, owlready2.ClassConstruct)):
                     yield OWLDataPropertyDomainAxiom(pe, _parse_concept_to_owlapy(dom))
                 else:
                     logger.warning("Construct %s not implemented at %s", dom, pe)
                     pass  # XXX TODO
 
     def data_property_range_axioms(self, pe: OWLDataProperty) -> Iterable[OWLDataPropertyRangeAxiom]:
-        p_x: owlready2.DataPropertyClass = self._world[pe.get_iri().as_str()]
+        p_x: owlready2.DataPropertyClass = self._world[pe.str]
         ranges = set(chain.from_iterable(super_prop.range for super_prop in p_x.ancestors()))
         if len(ranges) == 0:
             pass
             # TODO
         else:
             for rng in ranges:
                 if rng in _Datatype_map:
@@ -212,28 +216,28 @@
                 elif isinstance(rng, owlready2.ClassConstruct):
                     yield OWLDataPropertyRangeAxiom(pe, _parse_datarange_to_owlapy(rng))
                 else:
                     logger.warning("Datatype %s not implemented at %s", rng, pe)
                     pass  # XXX TODO
 
     def object_property_domain_axioms(self, pe: OWLObjectProperty) -> Iterable[OWLObjectPropertyDomainAxiom]:
-        p_x: owlready2.ObjectPropertyClass = self._world[pe.get_iri().as_str()]
+        p_x: owlready2.ObjectPropertyClass = self._world[pe.str]
         domains = set(p_x.domains_indirect())
         if len(domains) == 0:
             yield OWLObjectPropertyDomainAxiom(pe, OWLThing)
         else:
             for dom in domains:
                 if isinstance(dom, (owlready2.ThingClass, owlready2.ClassConstruct)):
                     yield OWLObjectPropertyDomainAxiom(pe, _parse_concept_to_owlapy(dom))
                 else:
                     logger.warning("Construct %s not implemented at %s", dom, pe)
                     pass  # XXX TODO
 
     def object_property_range_axioms(self, pe: OWLObjectProperty) -> Iterable[OWLObjectPropertyRangeAxiom]:
-        p_x: owlready2.ObjectPropertyClass = self._world[pe.get_iri().as_str()]
+        p_x: owlready2.ObjectPropertyClass = self._world[pe.str]
         ranges = set(chain.from_iterable(super_prop.range for super_prop in p_x.ancestors()))
         if len(ranges) == 0:
             yield OWLObjectPropertyRangeAxiom(pe, OWLThing)
         else:
             for rng in ranges:
                 if isinstance(rng, (owlready2.ThingClass, owlready2.ClassConstruct)):
                     yield OWLObjectPropertyRangeAxiom(pe, _parse_concept_to_owlapy(rng))
@@ -336,15 +340,15 @@
         yield from ranges - super_ranges
         if not direct:
             yield from super_ranges
 
     def equivalent_classes(self, ce: OWLClassExpression, only_named: bool = True) -> Iterable[OWLClassExpression]:
         seen_set = {ce}
         if isinstance(ce, OWLClass):
-            c_x: owlready2.ThingClass = self._world[ce.get_iri().as_str()]
+            c_x: owlready2.ThingClass = self._world[ce.str]
             for eq_x in c_x.INDIRECT_equivalent_to:
                 eq = _parse_concept_to_owlapy(eq_x)
                 if (isinstance(eq, OWLClass) or
                     (isinstance(eq, OWLClassExpression) and not only_named)) and eq not in seen_set:
                     seen_set.add(eq)
                     yield eq
                 # Workaround for problems in owlready2. It does not always recognize equivalent complex class
@@ -369,15 +373,15 @@
                             seen_set.add(e_c)
                             yield e_c
         else:
             raise ValueError(f'Equivalent classes not implemented for: {ce}')
 
     def _find_disjoint_classes(self, ce: OWLClassExpression, only_named: bool = True, seen_set=None):
         if isinstance(ce, OWLClass):
-            c_x: owlready2.ThingClass = self._world[ce.get_iri().as_str()]
+            c_x: owlready2.ThingClass = self._world[ce.str]
             for d_x in chain.from_iterable(map(lambda d: d.entities, c_x.disjoints())):
                 if d_x != c_x and (isinstance(d_x, owlready2.ThingClass) or
                                    (isinstance(d_x, owlready2.ClassConstruct) and not only_named)):
                     d_owlapy = _parse_concept_to_owlapy(d_x)
                     seen_set.add(d_owlapy)
                     yield d_owlapy
                     for c in self.equivalent_classes(d_owlapy, only_named=only_named):
@@ -400,94 +404,94 @@
         seen_set = set()
         yield from self._find_disjoint_classes(ce, only_named, seen_set)
         for c in self.super_classes(ce, only_named=only_named):
             if c != OWLClass(IRI('http://www.w3.org/2002/07/owl#', 'Thing')):
                 yield from self._find_disjoint_classes(c, only_named=only_named, seen_set=seen_set)
 
     def different_individuals(self, ind: OWLNamedIndividual) -> Iterable[OWLNamedIndividual]:
-        i: owlready2.Thing = self._world[ind.get_iri().as_str()]
+        i: owlready2.Thing = self._world[ind.str]
         yield from (OWLNamedIndividual(IRI.create(d_i.iri))
                     for d_i in chain.from_iterable(map(lambda x: x.entities, i.differents()))
                     if isinstance(d_i, owlready2.Thing) and i != d_i)
 
     def same_individuals(self, ind: OWLNamedIndividual) -> Iterable[OWLNamedIndividual]:
-        i: owlready2.Thing = self._world[ind.get_iri().as_str()]
+        i: owlready2.Thing = self._world[ind.str]
         yield from (OWLNamedIndividual(IRI.create(d_i.iri)) for d_i in i.equivalent_to
                     if isinstance(d_i, owlready2.Thing))
 
     def data_property_values(self, ind: OWLNamedIndividual, pe: OWLDataProperty, direct: bool = True) \
             -> Iterable[OWLLiteral]:
-        i: owlready2.Thing = self._world[ind.get_iri().as_str()]
-        p: owlready2.DataPropertyClass = self._world[pe.get_iri().as_str()]
+        i: owlready2.Thing = self._world[ind.str]
+        p: owlready2.DataPropertyClass = self._world[pe.str]
         retrieval_func = p._get_values_for_individual if direct else p._get_indirect_values_for_individual
         for val in retrieval_func(i):
             yield OWLLiteral(val)
 
     def all_data_property_values(self, pe: OWLDataProperty, direct: bool = True) -> Iterable[OWLLiteral]:
-        p: owlready2.DataPropertyClass = self._world[pe.get_iri().as_str()]
+        p: owlready2.DataPropertyClass = self._world[pe.str]
         relations = p.get_relations()
         if not direct:
             indirect_relations = chain.from_iterable(
-                map(lambda x: self._world[x.get_iri().as_str()].get_relations(),
+                map(lambda x: self._world[x.str].get_relations(),
                     self.sub_data_properties(pe, direct=False)))
             relations = chain(relations, indirect_relations)
         for _, val in relations:
             yield OWLLiteral(val)
 
     def object_property_values(self, ind: OWLNamedIndividual, pe: OWLObjectPropertyExpression, direct: bool = False) \
             -> Iterable[OWLNamedIndividual]:
         if isinstance(pe, OWLObjectProperty):
-            i: owlready2.Thing = self._world[ind.get_iri().as_str()]
-            p: owlready2.ObjectPropertyClass = self._world[pe.get_iri().as_str()]
+            i: owlready2.Thing = self._world[ind.str]
+            p: owlready2.ObjectPropertyClass = self._world[pe.str]
             # Recommended to use direct=False because _get_values_for_individual does not give consistent result
             # for the case when there are equivalent object properties. At least until this is fixed on owlready2.
             retieval_func = p._get_values_for_individual if direct else p._get_indirect_values_for_individual
             for val in retieval_func(i):
                 yield OWLNamedIndividual(IRI.create(val.iri))
         elif isinstance(pe, OWLObjectInverseOf):
-            p: owlready2.ObjectPropertyClass = self._world[pe.get_named_property().get_iri().as_str()]
+            p: owlready2.ObjectPropertyClass = self._world[pe.get_named_property().str]
             inverse_p = p.inverse_property
             # If the inverse property is explicitly defined we can take shortcut
             if inverse_p is not None:
                 yield from self.object_property_values(ind, OWLObjectProperty(IRI.create(inverse_p.iri)), direct)
             else:
                 if not direct:
                     raise NotImplementedError('Indirect values of inverse properties are only implemented if the '
                                               'inverse property is explicitly defined in the ontology.'
                                               f'Property: {pe}')
-                i: owlready2.Thing = self._world[ind.get_iri().as_str()]
+                i: owlready2.Thing = self._world[ind.str]
                 for val in p._get_inverse_values_for_individual(i):
                     yield OWLNamedIndividual(IRI.create(val.iri))
         else:
             raise NotImplementedError(pe)
 
     def flush(self) -> None:
         pass
 
     def instances(self, ce: OWLClassExpression, direct: bool = False) -> Iterable[OWLNamedIndividual]:
         if direct:
             if isinstance(ce, OWLClass):
-                c_x: owlready2.ThingClass = self._world[ce.get_iri().as_str()]
+                c_x: owlready2.ThingClass = self._world[ce.str]
                 for i in self._ontology._onto.get_instances_of(c_x):
                     if isinstance(i, owlready2.Thing):
                         yield OWLNamedIndividual(IRI.create(i.iri))
             else:
                 raise NotImplementedError("instances for complex class expressions not implemented", ce)
         else:
             if ce.is_owl_thing():
                 yield from self._ontology.individuals_in_signature()
             elif isinstance(ce, OWLClass):
-                c_x: owlready2.ThingClass = self._world[ce.get_iri().as_str()]
+                c_x: owlready2.ThingClass = self._world[ce.str]
                 for i in c_x.instances(world=self._world):
                     if isinstance(i, owlready2.Thing):
                         yield OWLNamedIndividual(IRI.create(i.iri))
             # elif isinstance(ce, OWLObjectSomeValuesFrom) and ce.get_filler().is_owl_thing()\
             #         and isinstance(ce.get_property(), OWLProperty):
             #     seen_set = set()
-            #     p_x: owlready2.ObjectProperty = self._world[ce.get_property().get_named_property().get_iri().as_str()]
+            #     p_x: owlready2.ObjectProperty = self._world[ce.get_property().get_named_property().str]
             #     for i, _ in p_x.get_relations():
             #         if isinstance(i, owlready2.Thing) and i not in seen_set:
             #             seen_set.add(i)
             #             yield OWLNamedIndividual(IRI.create(i.iri))
             else:
                 raise NotImplementedError("instances for complex class expressions not implemented", ce)
 
@@ -506,15 +510,15 @@
                         and axiom.get_sub_class() not in seen_set):
                     seen_set.add(axiom.get_sub_class())
                     if not only_named:
                         yield axiom.get_sub_class()
                     yield from self._sub_classes_recursive(axiom.get_sub_class(), seen_set, only_named)
 
             if isinstance(c, OWLClass):
-                c_x: owlready2.EntityClass = self._world[c.get_iri().as_str()]
+                c_x: owlready2.EntityClass = self._world[c.str]
                 # Subclasses will only return named classes
                 for sc_x in c_x.subclasses(world=self._world):
                     sc = _parse_concept_to_owlapy(sc_x)
                     if isinstance(sc, OWLClass) and sc not in seen_set:
                         seen_set.add(sc)
                         yield sc
                         yield from self._sub_classes_recursive(sc, seen_set, only_named=only_named)
@@ -545,15 +549,15 @@
             # First go through all general class axioms, they should only have complex classes as sub_classes.
             # Done for OWLClass and OWLClassExpression.
             if not only_named:
                 for axiom in self._ontology.general_class_axioms():
                     if isinstance(axiom, OWLSubClassOfAxiom) and axiom.get_super_class() == ce:
                         yield axiom.get_sub_class()
             if isinstance(ce, OWLClass):
-                c_x: owlready2.ThingClass = self._world[ce.get_iri().as_str()]
+                c_x: owlready2.ThingClass = self._world[ce.str]
                 # Subclasses will only return named classes
                 for sc in c_x.subclasses(world=self._world):
                     if isinstance(sc, owlready2.ThingClass):
                         yield OWLClass(IRI.create(sc.iri))
             elif isinstance(ce, OWLClassExpression):
                 # Slow but works. No better way to do this in owlready2 without using the reasoners at the moment.
                 for c in self._ontology.classes_in_signature():
@@ -566,15 +570,15 @@
             -> Iterable[OWLClassExpression]:
         # work around issue in class equivalence detection in Owlready2
         for c in [ce, *self.equivalent_classes(ce, only_named=False)]:
             if c not in seen_set:
                 seen_set.add(c)
                 yield c
             if isinstance(c, OWLClass):
-                c_x: owlready2.EntityClass = self._world[c.get_iri().as_str()]
+                c_x: owlready2.EntityClass = self._world[c.str]
                 for sc_x in c_x.is_a:
                     sc = _parse_concept_to_owlapy(sc_x)
                     if (isinstance(sc, OWLClass) or isinstance(sc, OWLClassExpression)) and sc not in seen_set:
                         seen_set.add(sc)
                         # Return class expression if it is a named class or complex class expressions should be
                         # included
                         if isinstance(sc, OWLClass) or not only_named:
@@ -604,15 +608,15 @@
     def super_classes(self, ce: OWLClassExpression, direct: bool = False, only_named: bool = True) \
             -> Iterable[OWLClassExpression]:
         if not direct:
             seen_set = {ce}
             yield from self._super_classes_recursive(ce, seen_set, only_named=only_named)
         else:
             if isinstance(ce, OWLClass):
-                c_x: owlready2.ThingClass = self._world[ce.get_iri().as_str()]
+                c_x: owlready2.ThingClass = self._world[ce.str]
                 for sc in c_x.is_a:
                     if (isinstance(sc, owlready2.ThingClass) or
                             (not only_named and isinstance(sc, owlready2.ClassConstruct))):
                         yield _parse_concept_to_owlapy(sc)
             elif isinstance(ce, OWLClassExpression):
                 seen_set = set()
                 for axiom in self._ontology.general_class_axioms():
@@ -628,29 +632,29 @@
                         seen_set.add(c)
                         yield c
             else:
                 raise ValueError(f'Super classes retrieval not supported for {ce}')
 
     def equivalent_object_properties(self, op: OWLObjectPropertyExpression) -> Iterable[OWLObjectPropertyExpression]:
         if isinstance(op, OWLObjectProperty):
-            p_x: owlready2.ObjectPropertyClass = self._world[op.get_iri().as_str()]
+            p_x: owlready2.ObjectPropertyClass = self._world[op.str]
             yield from (OWLObjectProperty(IRI.create(ep_x.iri)) for ep_x in p_x.INDIRECT_equivalent_to
                         if isinstance(ep_x, owlready2.ObjectPropertyClass))
         else:
             raise NotImplementedError("equivalent properties of inverse properties not yet implemented", op)
 
     def equivalent_data_properties(self, dp: OWLDataProperty) -> Iterable[OWLDataProperty]:
-        p_x: owlready2.DataPropertyClass = self._world[dp.get_iri().as_str()]
+        p_x: owlready2.DataPropertyClass = self._world[dp.str]
         yield from (OWLDataProperty(IRI.create(ep_x.iri)) for ep_x in p_x.INDIRECT_equivalent_to
                     if isinstance(ep_x, owlready2.DataPropertyClass))
 
     def _find_disjoint_object_properties(self, op: OWLObjectPropertyExpression, seen_set=None) \
             -> Iterable[OWLObjectPropertyExpression]:
         if isinstance(op, OWLObjectProperty):
-            p_x: owlready2.ObjectPropertyClass = self._world[op.get_iri().as_str()]
+            p_x: owlready2.ObjectPropertyClass = self._world[op.str]
             ont_x: owlready2.Ontology = self.get_root_ontology()._onto
             for disjoint in ont_x.disjoint_properties():
                 if p_x in disjoint.entities:
                     for o_p in disjoint.entities:
                         if isinstance(o_p, owlready2.ObjectPropertyClass) and o_p != p_x:
                             op_owlapy = OWLObjectProperty(IRI.create(o_p.iri))
                             seen_set.add(op_owlapy)
@@ -670,15 +674,15 @@
         seen_set = set()
         yield from self._find_disjoint_object_properties(op, seen_set)
         for o in self.super_object_properties(op):
             if o != OWLObjectProperty(IRI('http://www.w3.org/2002/07/owl#', 'ObjectProperty')):
                 yield from self._find_disjoint_object_properties(o, seen_set=seen_set)
 
     def _find_disjoint_data_properties(self, dp: OWLDataProperty, seen_set=None) -> Iterable[OWLDataProperty]:
-        p_x: owlready2.DataPropertyClass = self._world[dp.get_iri().as_str()]
+        p_x: owlready2.DataPropertyClass = self._world[dp.str]
         ont_x: owlready2.Ontology = self.get_root_ontology()._onto
         for disjoint in ont_x.disjoint_properties():
             if p_x in disjoint.entities:
                 for d_p in disjoint.entities:
                     if isinstance(d_p, owlready2.DataPropertyClass) and d_p != p_x:
                         dp_owlapy = OWLDataProperty(IRI.create(d_p.iri))
                         seen_set.add(dp_owlapy)
@@ -701,15 +705,15 @@
 
     def _sup_or_sub_data_properties_recursive(self, dp: OWLDataProperty, seen_set: Set, super_or_sub="") \
             -> Iterable[OWLDataProperty]:
         for d in self.equivalent_data_properties(dp):
             if d not in seen_set:
                 seen_set.add(d)
                 yield d
-        p_x: owlready2.DataPropertyClass = self._world[dp.get_iri().as_str()]
+        p_x: owlready2.DataPropertyClass = self._world[dp.str]
         assert isinstance(p_x, owlready2.DataPropertyClass)
         if super_or_sub == "super":
             dps = set(p_x.is_a)
         else:
             dps = set(p_x.subclasses(world=self._world))
         for sp_x in dps:
             if isinstance(sp_x, owlready2.DataPropertyClass):
@@ -718,15 +722,15 @@
                     seen_set.add(sp)
                     yield sp
                     yield from self._sup_or_sub_data_properties_recursive(sp, seen_set, super_or_sub)
 
     def _sup_or_sub_data_properties(self, dp: OWLDataProperty, direct: bool = False, super_or_sub=""):
         assert isinstance(dp, OWLDataProperty)
         if direct:
-            p_x: owlready2.DataPropertyClass = self._world[dp.get_iri().as_str()]
+            p_x: owlready2.DataPropertyClass = self._world[dp.str]
             if super_or_sub == "super":
                 dps = set(p_x.is_a)
             else:
                 dps = set(p_x.subclasses(world=self._world))
             for sp in dps:
                 if isinstance(sp, owlready2.DataPropertyClass):
                     yield OWLDataProperty(IRI.create(sp.iri))
@@ -752,15 +756,15 @@
         yield from self._sup_or_sub_data_properties(dp, direct, "sub")
 
     def _sup_or_sub_object_properties_recursive(self, op: OWLObjectProperty, seen_set: Set, super_or_sub=""):
         for o in self.equivalent_object_properties(op):
             if o not in seen_set:
                 seen_set.add(o)
                 yield o
-        p_x: owlready2.ObjectPropertyClass = self._world[op.get_iri().as_str()]
+        p_x: owlready2.ObjectPropertyClass = self._world[op.str]
         assert isinstance(p_x, owlready2.ObjectPropertyClass)
         if super_or_sub == "super":
             dps = set(p_x.is_a)
         else:
             dps = set(p_x.subclasses(world=self._world))
         for sp_x in dps:
             if isinstance(sp_x, owlready2.ObjectPropertyClass):
@@ -770,27 +774,27 @@
                     yield sp
                     yield from self._sup_or_sub_object_properties_recursive(sp, seen_set, super_or_sub)
 
     def _sup_or_sub_object_properties(self, op: OWLObjectPropertyExpression, direct: bool = False, super_or_sub="") \
             -> Iterable[OWLObjectPropertyExpression]:
         if isinstance(op, OWLObjectProperty):
             if direct:
-                p_x: owlready2.ObjectPropertyClass = self._world[op.get_iri().as_str()]
+                p_x: owlready2.ObjectPropertyClass = self._world[op.str]
                 if super_or_sub == "super":
                     dps = set(p_x.is_a)
                 else:
                     dps = set(p_x.subclasses(world=self._world))
                 for sp in dps:
                     if isinstance(sp, owlready2.ObjectPropertyClass):
                         yield OWLObjectProperty(IRI.create(sp.iri))
             else:
                 seen_set = set()
                 yield from self._sup_or_sub_object_properties_recursive(op, seen_set, super_or_sub)
         elif isinstance(op, OWLObjectInverseOf):
-            p: owlready2.ObjectPropertyClass = self._world[op.get_named_property().get_iri().as_str()]
+            p: owlready2.ObjectPropertyClass = self._world[op.get_named_property().str]
             inverse_p = p.inverse_property
             if inverse_p is not None:
                 yield from self._sup_or_sub_object_properties(OWLObjectProperty(IRI.create(inverse_p.iri)), direct,
                                                               super_or_sub)
             else:
                 raise NotImplementedError(f'{super_or_sub} properties of inverse properties are only implemented if the'
                                           ' inverse property is explicitly defined in the ontology. '
@@ -815,15 +819,15 @@
         yield from self._sup_or_sub_object_properties(op, direct, "super")
 
     def sub_object_properties(self, op: OWLObjectPropertyExpression, direct: bool = False) \
             -> Iterable[OWLObjectPropertyExpression]:
         yield from self._sup_or_sub_object_properties(op, direct, "sub")
 
     def types(self, ind: OWLNamedIndividual, direct: bool = False) -> Iterable[OWLClass]:
-        i: owlready2.Thing = self._world[ind.get_iri().as_str()]
+        i: owlready2.Thing = self._world[ind.str]
         if direct:
             for c in i.is_a:
                 if isinstance(c, owlready2.ThingClass):
                     yield OWLClass(IRI.create(c.iri))
                 # Anonymous classes are ignored
         else:
             for c in i.INDIRECT_is_a:
@@ -856,8 +860,8 @@
 
     def is_isolated(self):
         """Return True if this reasoner is using an isolated ontology."""
         return self._isolated
 
     def is_using_triplestore(self):
         # TODO: Deprecated! Remove after it is removed from OWLReasoner in owlapy
-        pass
+        pass
```

### Comparing `ontosample-0.2.2/ontolearn_light/base/axioms.py` & `ontosample-0.2.3/ontolearn_light/base/axioms.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 """Logic behind adding and removing axioms."""
 from functools import singledispatch
 from itertools import islice, combinations
 import types
 from typing import cast
 
 import owlready2
+from owlapy.owl_object import OWLObject
 from owlready2 import destroy_entity, AllDisjoint, AllDifferent, GeneralClassAxiom
-
-from owlapy.model import OWLDisjointUnionAxiom, OWLQuantifiedDataRestriction, \
-    OWLAnnotationAssertionAxiom, OWLClass, OWLClassAssertionAxiom, OWLEquivalentClassesAxiom, OWLObject, \
-    OWLAnnotationProperty, OWLDataHasValue, OWLDataProperty, OWLDeclarationAxiom, OWLIndividual, \
-    OWLNamedIndividual, OWLNaryBooleanClassExpression, OWLObjectComplementOf, OWLObjectHasValue, \
-    OWLObjectInverseOf, OWLObjectOneOf, OWLObjectProperty, OWLObjectPropertyAssertionAxiom,  OWLAxiom, \
-    OWLSubClassOfAxiom, OWLSubPropertyAxiom, OWLSymmetricObjectPropertyAxiom, OWLThing, OWLOntology, \
-    OWLPropertyDomainAxiom, OWLPropertyRangeAxiom, OWLObjectPropertyRangeAxiom, OWLTransitiveObjectPropertyAxiom, \
+from owlapy.class_expression import OWLThing, OWLClass, \
+    OWLQuantifiedDataRestriction, OWLDataHasValue, OWLNaryBooleanClassExpression, OWLObjectOneOf, OWLObjectComplementOf, \
+    OWLObjectHasValue, OWLQuantifiedObjectRestriction
+from owlapy.owl_axiom import OWLObjectPropertyRangeAxiom, OWLAxiom, OWLSubClassOfAxiom, OWLEquivalentClassesAxiom, \
+    OWLDisjointUnionAxiom, OWLAnnotationAssertionAxiom, OWLAnnotationProperty, OWLSubPropertyAxiom, \
+    OWLPropertyRangeAxiom, OWLClassAssertionAxiom, OWLDeclarationAxiom, OWLObjectPropertyAssertionAxiom, \
+    OWLSymmetricObjectPropertyAxiom, OWLTransitiveObjectPropertyAxiom, OWLPropertyDomainAxiom, \
     OWLAsymmetricObjectPropertyAxiom, OWLDataPropertyCharacteristicAxiom, OWLFunctionalDataPropertyAxiom, \
-    OWLDataPropertyAssertionAxiom,  OWLReflexiveObjectPropertyAxiom, OWLFunctionalObjectPropertyAxiom, \
-    OWLInverseFunctionalObjectPropertyAxiom, OWLIrreflexiveObjectPropertyAxiom, OWLObjectPropertyCharacteristicAxiom, \
+    OWLReflexiveObjectPropertyAxiom, OWLDataPropertyAssertionAxiom, OWLFunctionalObjectPropertyAxiom, \
+    OWLObjectPropertyCharacteristicAxiom, OWLIrreflexiveObjectPropertyAxiom, OWLInverseFunctionalObjectPropertyAxiom, \
     OWLDisjointDataPropertiesAxiom, OWLDisjointObjectPropertiesAxiom, OWLEquivalentDataPropertiesAxiom, \
     OWLEquivalentObjectPropertiesAxiom, OWLInverseObjectPropertiesAxiom, OWLNaryPropertyAxiom, OWLNaryIndividualAxiom, \
-    OWLDifferentIndividualsAxiom, OWLDisjointClassesAxiom, OWLSameIndividualAxiom, OWLProperty, \
-    OWLQuantifiedObjectRestriction
+    OWLDifferentIndividualsAxiom, OWLDisjointClassesAxiom, OWLSameIndividualAxiom
+from owlapy.owl_individual import OWLNamedIndividual, OWLIndividual
+from owlapy.owl_ontology import OWLOntology
+from owlapy.owl_property import OWLDataProperty, OWLObjectInverseOf, OWLObjectProperty, \
+    OWLProperty
 from ontolearn_light.base.utils import ToOwlready2
 
 
 @singledispatch
 def _add_axiom(axiom: OWLAxiom):
     raise NotImplementedError(f'Axiom type {axiom} is not implemented yet.')
 
@@ -41,26 +44,26 @@
         if entity_x is not None:
             return
 
         thing_x: owlready2.entity.ThingClass = conv.map_concept(OWLThing)
         if isinstance(entity, OWLClass):
             if entity.is_owl_thing() or entity.is_owl_nothing():
                 return
-            entity_x = types.new_class(name=entity.get_iri().get_remainder(), bases=(thing_x,))
+            entity_x = types.new_class(name=entity.iri.get_remainder(), bases=(thing_x,))
         elif isinstance(entity, OWLIndividual):
-            entity_x = thing_x(entity.get_iri().get_remainder())
+            entity_x = thing_x(entity.iri.get_remainder())
         elif isinstance(entity, OWLObjectProperty):
-            entity_x = types.new_class(name=entity.get_iri().get_remainder(), bases=(owlready2.ObjectProperty,))
+            entity_x = types.new_class(name=entity.iri.get_remainder(), bases=(owlready2.ObjectProperty,))
         elif isinstance(entity, OWLDataProperty):
-            entity_x = types.new_class(name=entity.get_iri().get_remainder(), bases=(owlready2.DatatypeProperty,))
+            entity_x = types.new_class(name=entity.iri.get_remainder(), bases=(owlready2.DatatypeProperty,))
         elif isinstance(entity, OWLAnnotationProperty):
-            entity_x = types.new_class(name=entity.get_iri().get_remainder(), bases=(owlready2.AnnotationProperty,))
+            entity_x = types.new_class(name=entity.iri.get_remainder(), bases=(owlready2.AnnotationProperty,))
         else:
             raise ValueError(f'Cannot add ({entity}). Not an atomic class, property, or individual.')
-        entity_x.namespace = ont_x.get_namespace(entity.get_iri().get_namespace())
+        entity_x.namespace = ont_x.get_namespace(entity.iri.get_namespace())
         entity_x.namespace.world._refactor(entity_x.storid, entity_x.iri)
 
 
 @_add_axiom.register
 def _(axiom: OWLClassAssertionAxiom, ontology: OWLOntology, world: owlready2.namespace.World):
     conv = ToOwlready2(world)
     ont_x: owlready2.namespace.Ontology = conv.map_object(ontology)
@@ -144,16 +147,30 @@
 
     assert axiom.contains_named_equivalent_class(), 'Owlready2 does not support general' \
                                                     'class axioms for equivalent classes.'
     for ce in axiom.class_expressions():
         _check_expression(ce, ontology, world)
     with ont_x:
         for ce_1, ce_2 in combinations(axiom.class_expressions(), 2):
+            assert ce_1 is not None, f"ce_1 cannot be None: {ce_1}, {type(ce_1)}"
+            assert ce_2 is not None, f"ce_2_x cannot be None: {ce_2}, {type(ce_2)}"
+
             ce_1_x = conv.map_concept(ce_1)
             ce_2_x = conv.map_concept(ce_2)
+            try:
+                assert ce_1_x is not None, f"ce_1_x cannot be None: {ce_1_x}, {type(ce_1_x)}"
+                assert ce_2_x is not None, f"ce_2_x cannot be None: {ce_2_x}, {type(ce_2_x)}"
+            except AssertionError:
+                print("function of ToOwlready2.map_concept() returns None")
+                print(ce_1, ce_1_x)
+                print(ce_2, ce_2_x)
+                print("Axiom:", axiom)
+                print("Temporary solution is reinitializing ce_1_x=ce_2_x\n\n")
+                ce_1_x=ce_2_x
+
             if isinstance(ce_1_x, owlready2.ThingClass):
                 ce_1_x.equivalent_to.append(ce_2_x)
             if isinstance(ce_2_x, owlready2.ThingClass):
                 ce_2_x.equivalent_to.append(ce_1_x)
 
 
 @_add_axiom.register
@@ -190,17 +207,17 @@
 
     prop_x = conv.map_object(axiom.get_property())
     if prop_x is None:
         with ont_x:
             prop_x: owlready2.annotation.AnnotationPropertyClass = cast(
                 owlready2.AnnotationProperty,
                 types.new_class(
-                    name=axiom.get_property().get_iri().get_remainder(),
+                    name=axiom.get_property().iri.get_remainder(),
                     bases=(owlready2.AnnotationProperty,)))
-            prop_x.namespace = ont_x.get_namespace(axiom.get_property().get_iri().get_namespace())
+            prop_x.namespace = ont_x.get_namespace(axiom.get_property().iri.get_namespace())
     sub_x = world[axiom.get_subject().as_iri().as_str()]
     assert sub_x is not None, f'{axiom.get_subject} not found in {ontology}'
     with ont_x:
         if axiom.get_value().is_literal():
             literal = axiom.get_value().as_literal()
             setattr(sub_x, prop_x.python_name, literal.to_python())
         else:
@@ -216,15 +233,15 @@
 
     for ind in axiom.individuals():
         _add_axiom(OWLDeclarationAxiom(ind), ontology, world)
     with ont_x:
         if isinstance(axiom, OWLSameIndividualAxiom):
             for idx, ind in enumerate(axiom.individuals()):
                 ind_x = conv._to_owlready2_individual(ind)
-                for ind_2 in islice(axiom.individuals(), idx+1, None):
+                for ind_2 in islice(axiom.individuals(), idx + 1, None):
                     ind_2_x = conv._to_owlready2_individual(ind_2)
                     ind_x.equivalent_to.append(ind_2_x)
         elif isinstance(axiom, OWLDifferentIndividualsAxiom):
             AllDifferent(list(map(conv._to_owlready2_individual, axiom.individuals())))
         else:
             raise ValueError(f'OWLNaryIndividualAxiom ({axiom}) is not defined.')
 
@@ -283,15 +300,15 @@
 
     for property_ in axiom.properties():
         _add_axiom(OWLDeclarationAxiom(property_), ontology, world)
     with ont_x:
         if isinstance(axiom, (OWLEquivalentObjectPropertiesAxiom, OWLEquivalentDataPropertiesAxiom,)):
             for idx, property_ in enumerate(axiom.properties()):
                 property_x = conv._to_owlready2_property(property_)
-                for property_2 in islice(axiom.properties(), idx+1, None):
+                for property_2 in islice(axiom.properties(), idx + 1, None):
                     property_2_x = conv._to_owlready2_property(property_2)
                     property_x.equivalent_to.append(property_2_x)
         elif isinstance(axiom, (OWLDisjointObjectPropertiesAxiom, OWLDisjointDataPropertiesAxiom,)):
             AllDisjoint(list(map(conv._to_owlready2_property, axiom.properties())))
         elif isinstance(axiom, OWLInverseObjectPropertiesAxiom):
             property_first_x = conv._to_owlready2_property(axiom.get_first_property())
             property_second_x = conv._to_owlready2_property(axiom.get_second_property())
@@ -482,15 +499,15 @@
 def _(axiom: OWLAnnotationAssertionAxiom, ontology: OWLOntology, world: owlready2.namespace.World):
     conv = ToOwlready2(world)
     ont_x: owlready2.Ontology = conv.map_object(ontology)
 
     sub_x = world[axiom.get_subject().as_iri().as_str()]
     if sub_x is None:
         return
-    name = axiom.get_property().get_iri().get_remainder()
+    name = axiom.get_property().iri.get_remainder()
     with ont_x:
         if axiom.get_value().is_literal():
             o_x = axiom.get_value().as_literal().to_python()
         else:
             o_x = world[axiom.get_value().as_iri().as_str()]
 
         value = getattr(sub_x, name, None)
@@ -636,17 +653,21 @@
     with ont_x:
         property_x = conv._to_owlready2_property(axiom.get_property())
         if property_x is not None and isinstance(axiom, OWLFunctionalDataPropertyAxiom) \
                 and owlready2.FunctionalProperty in property_x.is_a:
             property_x.is_a.remove(owlready2.FunctionalProperty)
 
 
-# Creates all entities (individuals, classes, properties) that appear in the given (complex) class expression
-# and do not exist in the given ontology yet
 def _check_expression(expr: OWLObject, ontology: OWLOntology, world: owlready2.namespace.World):
+    """
+    @TODO:CD: Documentation
+    Creates all entities (individuals, classes, properties) that appear in the given (complex) class expression
+    and do not exist in the given ontology yet
+
+    """
     if isinstance(expr, (OWLClass, OWLProperty, OWLNamedIndividual,)):
         _add_axiom(OWLDeclarationAxiom(expr), ontology, world)
     elif isinstance(expr, (OWLNaryBooleanClassExpression, OWLObjectComplementOf, OWLObjectOneOf,)):
         for op in expr.operands():
             _check_expression(op, ontology, world)
     elif isinstance(expr, (OWLQuantifiedObjectRestriction, OWLObjectHasValue,)):
         _check_expression(expr.get_property(), ontology, world)
```

### Comparing `ontosample-0.2.2/ontolearn_light/base/complex_ce_instances.py` & `ontosample-0.2.3/ontolearn_light/base/complex_ce_instances.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 """OWL Reasoner - Complex Class Expression Instances (CCEI)."""
 import logging
 import types
 from logging import warning
 from typing import Iterable, cast, Optional, List
 import os
 import owlready2
-
-from owlapy.model import OWLClass, OWLClassExpression, OWLNamedIndividual, IRI, OWLAxiom
+from owlapy.class_expression import OWLClassExpression
+from owlapy.iri import IRI
+from owlapy.owl_axiom import OWLAxiom
+from owlapy.owl_individual import OWLNamedIndividual
 from ontolearn_light.base import OWLReasoner_Owlready2, OWLOntology_Owlready2, BaseReasoner_Owlready2, \
     OWLOntologyManager_Owlready2
 from ontolearn_light.base.utils import ToOwlready2
 
 logger = logging.getLogger(__name__)
 
 
@@ -90,8 +92,8 @@
 
     def __del__(self):
         if self._isolated:
             file_path = f"isolated_ontology_{id(self.reference_ontology)}.owl"
             try:
                 os.remove(file_path)
             except OSError as e:
-                logger.warning(f"Error deleting {file_path}: {e}")
+                logger.warning(f"Error deleting {file_path}: {e}")
```

### Comparing `ontosample-0.2.2/ontolearn_light/base/ext/__init__.py` & `ontosample-0.2.3/ontolearn_light/base/ext/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 """Extra classes."""
 import logging
 from abc import ABCMeta
 from typing import Iterable
 
-from owlapy.model import OWLNamedIndividual, OWLObjectProperty, OWLReasoner, OWLDataProperty, OWLDataRange, \
-    OWLLiteral
-
+from owlapy.owl_data_ranges import OWLDataRange
+from owlapy.owl_individual import OWLNamedIndividual
+from owlapy.owl_literal import OWLLiteral
+from owlapy.owl_property import OWLObjectProperty, OWLDataProperty
+from owlapy.owl_reasoner import OWLReasoner
 
 logger = logging.getLogger(__name__)
 
 
 class OWLReasonerEx(OWLReasoner, metaclass=ABCMeta):
     """Extra convenience methods for OWL Reasoners
```

### Comparing `ontosample-0.2.2/ontolearn_light/base/fast_instance_checker.py` & `ontosample-0.2.3/ontolearn_light/base/fast_instance_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,23 +4,29 @@
 import operator
 import owlready2
 from functools import singledispatchmethod, reduce
 from itertools import repeat, chain
 from types import MappingProxyType, FunctionType
 from typing import DefaultDict, Iterable, Dict, Mapping, Set, Type, TypeVar, Optional, FrozenSet, cast
 
-from ontolearn_light.base import OWLReasoner_Owlready2
+from owlapy.class_expression import OWLObjectOneOf, OWLClass, OWLObjectUnionOf, OWLObjectIntersectionOf, \
+    OWLObjectSomeValuesFrom, OWLObjectComplementOf, OWLObjectAllValuesFrom, OWLDataSomeValuesFrom, \
+    OWLDatatypeRestriction, OWLClassExpression, OWLDataAllValuesFrom, OWLDataHasValue, OWLDataOneOf, \
+    OWLObjectCardinalityRestriction, OWLObjectMinCardinality, OWLObjectMaxCardinality, OWLObjectExactCardinality, \
+    OWLObjectHasValue, OWLFacetRestriction
+from owlapy.iri import IRI
+from owlapy.owl_data_ranges import OWLDataRange, OWLDataComplementOf, OWLDataIntersectionOf, OWLDataUnionOf
+from owlapy.owl_datatype import OWLDatatype
+from owlapy.owl_individual import OWLNamedIndividual
+from owlapy.owl_literal import OWLLiteral
+from owlapy.owl_ontology import OWLOntology
+from owlapy.owl_property import OWLObjectProperty, OWLDataProperty, OWLObjectPropertyExpression, OWLObjectInverseOf, \
+    OWLDataPropertyExpression, OWLPropertyExpression
+from owlapy.owl_reasoner import OWLReasoner
 from ontolearn_light.base.ext import OWLReasonerEx
-from owlapy.model import OWLDataRange, OWLObjectOneOf, OWLOntology, OWLNamedIndividual, OWLClass, \
-    OWLObjectProperty, OWLDataProperty, OWLObjectUnionOf, OWLObjectIntersectionOf, OWLObjectSomeValuesFrom, \
-    OWLObjectPropertyExpression, OWLObjectComplementOf, OWLObjectAllValuesFrom, IRI, OWLObjectInverseOf, \
-    OWLDataSomeValuesFrom, OWLDataPropertyExpression, OWLDatatypeRestriction, OWLLiteral, OWLClassExpression, \
-    OWLDataComplementOf, OWLDataAllValuesFrom, OWLDatatype, OWLDataHasValue, OWLDataOneOf, OWLReasoner, \
-    OWLDataIntersectionOf, OWLDataUnionOf, OWLObjectCardinalityRestriction, OWLObjectMinCardinality, \
-    OWLObjectMaxCardinality, OWLObjectExactCardinality, OWLObjectHasValue, OWLPropertyExpression, OWLFacetRestriction
 from owlapy.util import LRUCache
 
 logger = logging.getLogger(__name__)
 
 _P = TypeVar('_P', bound=OWLPropertyExpression)
 
 
@@ -580,23 +586,23 @@
         self._cls_to_ind[c] = frozenset(temp)
 
     def _retrieve_triples(self, pe: OWLPropertyExpression) -> Iterable:
         """Retrieve all subject/object pairs for the given property."""
 
         if isinstance(pe, OWLObjectPropertyExpression):
             retrieval_func = self.sub_object_properties
-            p_x: owlready2.ObjectProperty = self._ontology._world[pe.get_named_property().get_iri().as_str()]
+            p_x: owlready2.ObjectProperty = self._ontology._world[pe.get_named_property().str]
         else:
             retrieval_func = self.sub_data_properties
-            p_x: owlready2.DataProperty = self._ontology._world[pe.get_iri().as_str()]
+            p_x: owlready2.DataProperty = self._ontology._world[pe.str]
 
         relations = p_x.get_relations()
         if self._sub_properties:
             # Retrieve the subject/object pairs for all sub properties of pe
             indirect_relations = chain.from_iterable(
-                map(lambda x: self._ontology._world[x.get_iri().as_str()].get_relations(),
+                map(lambda x: self._ontology._world[x.str].get_relations(),
                     retrieval_func(pe, direct=False)))
             # If pe is an OWLObjectInverseOf we need to swap the pairs
             if isinstance(pe, OWLObjectInverseOf):
                 indirect_relations = ((r[1], r[0]) for r in indirect_relations)
             relations = chain(relations, indirect_relations)
-        yield from relations
+        yield from relations
```

### Comparing `ontosample-0.2.2/ontolearn_light/base/owl/hierarchy.py` & `ontosample-0.2.3/ontolearn_light/base/owl/hierarchy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Classes representing hierarchy in OWL."""
 
 import operator
 from abc import ABCMeta, abstractmethod
 from functools import reduce
 from typing import Dict, Iterable, Tuple, overload, TypeVar, Generic, Type, cast, Optional, FrozenSet, Set
 
-from owlapy.model import OWLClass, OWLReasoner, OWLObjectProperty, OWLDataProperty, OWLTopObjectProperty, \
-    OWLBottomObjectProperty, OWLTopDataProperty, OWLBottomDataProperty, OWLThing, OWLNothing, HasIRI
+from owlapy.class_expression import OWLClass, OWLThing, OWLNothing
+from owlapy.meta_classes import HasIRI
+from owlapy.owl_literal import OWLTopObjectProperty, OWLBottomObjectProperty, OWLTopDataProperty, OWLBottomDataProperty
+from owlapy.owl_property import OWLObjectProperty, OWLDataProperty
+from owlapy.owl_reasoner import OWLReasoner
 
 _S = TypeVar('_S', bound=HasIRI)  #:
 _U = TypeVar('_U', bound='AbstractHierarchy')  #:
 
 
 class AbstractHierarchy(Generic[_S], metaclass=ABCMeta):
     """Representation of an abstract hierarchy which can be used for classes or properties.
```

### Comparing `ontosample-0.2.2/ontolearn_light/base/owl/utils.py` & `ontosample-0.2.3/ontolearn_light/base/owl/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 from collections import Counter
 from functools import singledispatchmethod
 from typing import Iterable, Generic, TypeVar, Callable, List
-
-from owlapy.model import OWLDataRange, OWLLiteral, OWLObject, OWLClass, OWLObjectProperty, \
-    OWLObjectAllValuesFrom, OWLObjectUnionOf, OWLObjectIntersectionOf, OWLObjectComplementOf, OWLObjectInverseOf, \
-    OWLObjectCardinalityRestriction, OWLObjectHasSelf, OWLObjectHasValue, OWLObjectOneOf, OWLNamedIndividual, \
-    OWLObjectMinCardinality, OWLObjectExactCardinality, OWLObjectMaxCardinality, OWLClassExpression, OWLThing, \
-    OWLDataSomeValuesFrom, OWLDataOneOf, OWLDatatypeRestriction, OWLDataComplementOf, OWLDataAllValuesFrom, \
-    OWLDataCardinalityRestriction, OWLDatatype, OWLDataHasValue, OWLDataUnionOf, OWLDataIntersectionOf, \
-    OWLDataExactCardinality, OWLDataMaxCardinality, OWLDataMinCardinality, OWLDataProperty, OWLObjectSomeValuesFrom
+from owlapy.class_expression import OWLObjectOneOf, OWLClass, OWLObjectUnionOf, OWLObjectIntersectionOf, \
+    OWLObjectSomeValuesFrom, OWLObjectComplementOf, OWLObjectAllValuesFrom, OWLDataSomeValuesFrom, \
+    OWLDatatypeRestriction, OWLClassExpression, OWLDataAllValuesFrom, OWLDataHasValue, OWLDataOneOf, \
+    OWLObjectMinCardinality, OWLObjectMaxCardinality, OWLObjectExactCardinality, \
+    OWLObjectHasValue, OWLDataExactCardinality, OWLDataMaxCardinality, \
+    OWLDataMinCardinality, OWLObjectHasSelf, OWLObjectCardinalityRestriction, \
+    OWLDataCardinalityRestriction, OWLThing
+from owlapy.owl_data_ranges import OWLDataRange, OWLDataComplementOf, OWLDataIntersectionOf, OWLDataUnionOf
+from owlapy.owl_datatype import OWLDatatype
+from owlapy.owl_individual import OWLNamedIndividual
+from owlapy.owl_literal import OWLLiteral
+from owlapy.owl_object import OWLObject
+from owlapy.owl_property import OWLObjectProperty, OWLDataProperty, OWLObjectInverseOf
 
 from owlapy.util import OrderedOWLObject, iter_count
 from sortedcontainers import SortedSet
 
 
 class OWLClassExpressionLengthMetric:
     """Length calculation of OWLClassExpression
```

### Comparing `ontosample-0.2.2/ontolearn_light/base/utils.py` & `ontosample-0.2.3/ontolearn_light/base/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 """Utils for mapping to and from owlready2."""
 from datetime import date, datetime
 from functools import singledispatchmethod
 from types import MappingProxyType
 from typing import Union
 
 import owlready2
+from owlapy.class_expression import OWLObjectOneOf, OWLClass, OWLObjectUnionOf, OWLObjectIntersectionOf, \
+    OWLObjectSomeValuesFrom, OWLObjectComplementOf, OWLObjectAllValuesFrom, OWLDataSomeValuesFrom, \
+    OWLDatatypeRestriction, OWLClassExpression, OWLDataAllValuesFrom, OWLDataHasValue, OWLDataOneOf, \
+    OWLObjectMinCardinality, OWLObjectMaxCardinality, OWLObjectExactCardinality, \
+    OWLObjectHasValue, OWLFacetRestriction, OWLObjectRestriction, OWLDataExactCardinality, OWLDataMaxCardinality, \
+    OWLDataMinCardinality, OWLRestriction, OWLDataRestriction
+from owlapy.iri import IRI
+from owlapy.owl_axiom import OWLAnnotationProperty
+from owlapy.owl_data_ranges import OWLDataRange, OWLDataComplementOf, OWLDataIntersectionOf, OWLDataUnionOf
+from owlapy.owl_datatype import OWLDatatype
+from owlapy.owl_individual import OWLNamedIndividual, OWLIndividual
+from owlapy.owl_literal import OWLLiteral, IntegerOWLDatatype, DoubleOWLDatatype, BooleanOWLDatatype, DateOWLDatatype, \
+    DateTimeOWLDatatype, DurationOWLDatatype, StringOWLDatatype
+from owlapy.owl_object import OWLObject
+from owlapy.owl_ontology import OWLOntology
+from owlapy.owl_property import OWLObjectProperty, OWLDataProperty, OWLObjectPropertyExpression, OWLObjectInverseOf, \
+    OWLDataPropertyExpression, OWLPropertyExpression
+
 from pandas import Timedelta
 
-from owlapy.model import OWLObjectMinCardinality, OWLObjectOneOf, OWLObjectRestriction, \
-    OWLObjectComplementOf, OWLObjectUnionOf, OWLObjectIntersectionOf, OWLObjectSomeValuesFrom, OWLObjectAllValuesFrom, \
-    OWLObjectPropertyExpression, OWLObject, OWLOntology, OWLAnnotationProperty, IRI, OWLObjectInverseOf, \
-    DoubleOWLDatatype, IntegerOWLDatatype, OWLClassExpression, OWLDataAllValuesFrom, OWLDataComplementOf, \
-    OWLDataIntersectionOf, OWLDataProperty, OWLDataRange, OWLDataSomeValuesFrom, OWLDataUnionOf, OWLDatatype, \
-    BooleanOWLDatatype, OWLDataHasValue, OWLDataExactCardinality, OWLDataMaxCardinality, OWLDataMinCardinality, \
-    OWLDataPropertyExpression, OWLDatatypeRestriction, OWLFacetRestriction, OWLLiteral, OWLObjectHasValue, \
-    OWLNamedIndividual, OWLObjectExactCardinality, OWLObjectMaxCardinality, OWLObjectProperty, OWLClass, \
-    DateOWLDatatype, DateTimeOWLDatatype, DurationOWLDatatype, OWLRestriction, OWLDataOneOf, OWLDataRestriction, \
-    OWLIndividual, StringOWLDatatype, OWLPropertyExpression
 
 from owlapy.vocab import OWLFacet
 
-
 OWLREADY2_FACET_KEYS = MappingProxyType({
     OWLFacet.MIN_INCLUSIVE: "min_inclusive",
     OWLFacet.MIN_EXCLUSIVE: "min_exclusive",
     OWLFacet.MAX_INCLUSIVE: "max_inclusive",
     OWLFacet.MAX_EXCLUSIVE: "max_exclusive",
     OWLFacet.LENGTH: "length",
     OWLFacet.MIN_LENGTH: "min_length",
@@ -32,15 +39,14 @@
     OWLFacet.PATTERN: "pattern",
     OWLFacet.TOTAL_DIGITS: "total_digits",
     OWLFacet.FRACTION_DIGITS: "fraction_digits"
 })
 
 
 class ToOwlready2:
-
     __slots__ = '_world'
 
     _world: owlready2.World
 
     def __init__(self, world: owlready2.World):
         """Map owlapy model classes to owlready2.
 
@@ -57,21 +63,22 @@
     @map_object.register
     def _(self, ce: OWLClassExpression) -> Union[owlready2.ClassConstruct, owlready2.ThingClass]:
         return self.map_concept(ce)
 
     @map_object.register
     def _(self, ont: OWLOntology) -> owlready2.namespace.Ontology:
         return self._world.get_ontology(
-                ont.get_ontology_id().get_ontology_iri().as_str()
-            )
+            ont.get_ontology_id().get_ontology_iri().as_str()
+        )
 
     @map_object.register
     def _(self, ap: OWLAnnotationProperty) -> owlready2.annotation.AnnotationPropertyClass:
-        return self._world[ap.get_iri().as_str()]
+        return self._world[ap.str]
 
+    # @TODO CD: map_object is buggy. and it can return None
     # single dispatch is still not implemented in mypy, see https://github.com/python/mypy/issues/2904
     @singledispatchmethod
     def map_concept(self, o: OWLClassExpression) \
             -> Union[owlready2.ClassConstruct, owlready2.ThingClass]:
         """Map owlapy concept classes."""
         raise NotImplementedError(o)
 
@@ -82,31 +89,37 @@
     @_to_owlready2_property.register
     def _(self, p: OWLObjectInverseOf):
         p_x = self._to_owlready2_property(p.get_named_property())
         return owlready2.Inverse(p_x)
 
     @_to_owlready2_property.register
     def _(self, p: OWLObjectProperty) -> owlready2.prop.ObjectPropertyClass:
-        return self._world[p.get_iri().as_str()]
+        return self._world[p.str]
 
     @_to_owlready2_property.register
     def _(self, p: OWLDataProperty) -> owlready2.prop.DataPropertyClass:
-        return self._world[p.get_iri().as_str()]
+        return self._world[p.str]
 
     @singledispatchmethod
     def _to_owlready2_individual(self, i: OWLIndividual) -> owlready2.Thing:
         raise NotImplementedError(i)
 
     @_to_owlready2_individual.register
     def _(self, i: OWLNamedIndividual):
-        return self._world[i.get_iri().as_str()]
+        return self._world[i.str]
 
     @map_concept.register
     def _(self, c: OWLClass) -> owlready2.ThingClass:
-        return self._world[c.get_iri().as_str()]
+        x = self._world[c.str]
+        try:
+            assert x is not None
+        except AssertionError:
+            print(f"The world attribute{self._world} maps {c} into None")
+
+        return x
 
     @map_concept.register
     def _(self, c: OWLObjectComplementOf) -> owlready2.class_construct.Not:
         return owlready2.Not(self.map_concept(c.get_operand()))
 
     @map_concept.register
     def _(self, ce: OWLObjectUnionOf) -> owlready2.class_construct.Or:
@@ -115,14 +128,16 @@
     @map_concept.register
     def _(self, ce: OWLObjectIntersectionOf) -> owlready2.class_construct.And:
         return owlready2.And(map(self.map_concept, ce.operands()))
 
     @map_concept.register
     def _(self, ce: OWLObjectSomeValuesFrom) -> owlready2.class_construct.Restriction:
         prop = self._to_owlready2_property(ce.get_property())
+        assert isinstance(ce.get_filler(),
+                          OWLClassExpression), f"{ce.get_filler()} is not an OWL Class expression and cannot be serialized at the moment"
         return prop.some(self.map_concept(ce.get_filler()))
 
     @map_concept.register
     def _(self, ce: OWLObjectAllValuesFrom) -> owlready2.class_construct.Restriction:
         prop = self._to_owlready2_property(ce.get_property())
         return prop.only(self.map_concept(ce.get_filler()))
```

### Comparing `ontosample-0.2.2/ontolearn_light/concept_generator.py` & `ontosample-0.2.3/ontolearn_light/concept_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 """A module to generate concepts."""
 
 from typing import Iterable, List, Generator
 
+from owlapy.class_expression import OWLObjectMaxCardinality, OWLObjectMinCardinality, OWLObjectSomeValuesFrom, \
+    OWLObjectAllValuesFrom, OWLObjectIntersectionOf, OWLObjectUnionOf, OWLThing, OWLNothing, OWLClass, \
+    OWLClassExpression, OWLObjectComplementOf, OWLObjectExactCardinality, OWLDataAllValuesFrom, OWLDataSomeValuesFrom, \
+    OWLDataHasValue, OWLObjectHasValue
+from owlapy.owl_data_ranges import OWLDataRange
+from owlapy.owl_individual import OWLIndividual
+from owlapy.owl_literal import OWLLiteral
+from owlapy.owl_property import OWLObjectPropertyExpression, OWLDataPropertyExpression
+
 from ontolearn_light.utils import parametrized_performance_debugger
-from owlapy.model import OWLObjectMaxCardinality, OWLObjectMinCardinality, OWLObjectSomeValuesFrom, \
-    OWLObjectAllValuesFrom, OWLObjectIntersectionOf, OWLObjectUnionOf, OWLObjectPropertyExpression, OWLThing, \
-    OWLNothing, OWLClass, OWLClassExpression, OWLObjectComplementOf, \
-    OWLObjectExactCardinality, OWLDataAllValuesFrom, OWLDataPropertyExpression, OWLDataRange, OWLDataSomeValuesFrom, \
-    OWLDataHasValue, OWLIndividual, OWLLiteral, OWLObjectHasValue
 
 
 class ConceptGenerator:
     """A class that can generate some sorts of OWL Class Expressions."""
 
     @parametrized_performance_debugger()
     def negation_from_iterables(self, class_expressions: Iterable[OWLClassExpression]):
```

### Comparing `ontosample-0.2.2/ontolearn_light/data_struct.py` & `ontosample-0.2.3/ontolearn_light/data_struct.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Data structures."""
 
 import torch
 from collections import deque
 import pandas as pd
+import numpy as np
 import random
 
 
 class PrepareBatchOfPrediction(torch.utils.data.Dataset):
 
     def __init__(self, current_state: torch.FloatTensor, next_state_batch: torch.FloatTensor, p: torch.FloatTensor,
                  n: torch.FloatTensor):
@@ -118,15 +119,15 @@
 
     def clear(self):
         self.current_states.clear()
         self.next_states.clear()
         self.rewards.clear()
 
 
-class BaseDataLoader:
+class NCESBaseDataLoader:
 
     def __init__(self, vocab, inv_vocab):
 
         self.vocab = vocab
         self.inv_vocab = inv_vocab
         self.vocab_df = pd.DataFrame(self.vocab.values(), index=self.vocab.keys())
 
@@ -150,15 +151,15 @@
 
     def get_labels(self, target):
         target = self.decompose(target)
         labels = [self.vocab[atm] for atm in target]
         return labels, len(target)
 
 
-class NCESDataLoader(BaseDataLoader, torch.utils.data.Dataset):
+class NCESDataLoader(NCESBaseDataLoader, torch.utils.data.Dataset):
 
     def __init__(self, data: list, embeddings, vocab, inv_vocab, shuffle_examples, max_length, example_sizes=None,
                  sorted_examples=True):
         self.data_raw = data
         self.embeddings = embeddings
         self.max_length = max_length
         super().__init__(vocab, inv_vocab)
@@ -186,15 +187,15 @@
         datapoint_neg = torch.FloatTensor(self.embeddings.loc[selected_neg].values.squeeze())
         labels, length = self.get_labels(key)
         return datapoint_pos, datapoint_neg, torch.cat([torch.tensor(labels),
                                                         self.vocab['PAD'] * torch.ones(
                                                             self.max_length - length)]).long()
 
 
-class NCESDataLoaderInference(BaseDataLoader, torch.utils.data.Dataset):
+class NCESDataLoaderInference(NCESBaseDataLoader, torch.utils.data.Dataset):
 
     def __init__(self, data: list, embeddings, vocab, inv_vocab, shuffle_examples, sorted_examples=True):
         self.data_raw = data
         self.embeddings = embeddings
         super().__init__(vocab, inv_vocab)
         self.shuffle_examples = shuffle_examples
         self.sorted_examples = sorted_examples
@@ -205,10 +206,81 @@
     def __getitem__(self, idx):
         _, pos, neg = self.data_raw[idx]
         if self.sorted_examples:
             pos, neg = sorted(pos), sorted(neg)
         elif self.shuffle_examples:
             random.shuffle(pos)
             random.shuffle(neg)
-        datapoint_pos = torch.FloatTensor(self.embeddings.loc[pos].values)
-        datapoint_neg = torch.FloatTensor(self.embeddings.loc[neg].values)
+        datapoint_pos = torch.FloatTensor(self.embeddings.loc[pos].values.squeeze())
+        datapoint_neg = torch.FloatTensor(self.embeddings.loc[neg].values.squeeze())
         return datapoint_pos, datapoint_neg
+
+    
+class CLIPDataLoader(torch.utils.data.Dataset):
+
+    def __init__(self, data: list, embeddings, shuffle_examples, example_sizes: list=None,
+                 k=5, sorted_examples=True):
+        self.data_raw = data
+        self.embeddings = embeddings
+        super().__init__()
+        self.shuffle_examples = shuffle_examples
+        self.example_sizes = example_sizes
+        self.k = k
+        self.sorted_examples = sorted_examples
+
+    def __len__(self):
+        return len(self.data_raw)
+
+    def __getitem__(self, idx):
+        key, value = self.data_raw[idx]
+        pos = value['positive examples']
+        neg = value['negative examples']
+        length = value['length']
+        if self.example_sizes is not None:
+            k_pos, k_neg = random.choice(self.example_sizes)
+            k_pos = min(k_pos, len(pos))
+            k_neg = min(k_neg, len(neg))
+            selected_pos = random.sample(pos, k_pos)
+            selected_neg = random.sample(neg, k_neg)
+        elif self.k is not None:
+            prob_pos_set = 1.0/(1+np.array(range(min(self.k, len(pos)), len(pos)+1, self.k)))
+            prob_pos_set = prob_pos_set/prob_pos_set.sum()
+            prob_neg_set = 1.0/(1+np.array(range(min(self.k, len(neg)), len(neg)+1, self.k)))
+            prob_neg_set = prob_neg_set/prob_neg_set.sum()
+            k_pos = np.random.choice(range(min(self.k, len(pos)), len(pos)+1, self.k), replace=False, p=prob_pos_set)
+            k_neg = np.random.choice(range(min(self.k, len(neg)), len(neg)+1, self.k), replace=False, p=prob_neg_set)
+            selected_pos = random.sample(pos, k_pos)
+            selected_neg = random.sample(neg, k_neg)
+        else:
+            selected_pos = pos
+            selected_neg = neg
+        if self.shuffle_examples:
+            random.shuffle(selected_pos)
+            random.shuffle(selected_neg)
+        datapoint_pos = torch.FloatTensor(self.embeddings.loc[selected_pos].values.squeeze())
+        datapoint_neg = torch.FloatTensor(self.embeddings.loc[selected_neg].values.squeeze())
+        return datapoint_pos, datapoint_neg, torch.LongTensor([length])
+    
+    
+class CLIPDataLoaderInference(torch.utils.data.Dataset):
+
+    def __init__(self, data: list, embeddings, shuffle_examples,
+                 sorted_examples=True):
+        self.data_raw = data
+        self.embeddings = embeddings
+        super().__init__()
+        self.shuffle_examples = shuffle_examples
+        self.sorted_examples = sorted_examples
+
+    def __len__(self):
+        return len(self.data_raw)
+
+    def __getitem__(self, idx):
+        _, pos, neg = self.data_raw[idx]
+        if self.sorted_examples:
+            pos, neg = sorted(pos), sorted(neg)
+        elif self.shuffle_examples:
+            random.shuffle(pos)
+            random.shuffle(neg)
+        datapoint_pos = torch.FloatTensor(self.embeddings.loc[pos].values.squeeze())
+        datapoint_neg = torch.FloatTensor(self.embeddings.loc[pos].values.squeeze())
+        return datapoint_pos, datapoint_neg
```

### Comparing `ontosample-0.2.2/ontolearn_light/fitness_functions.py` & `ontosample-0.2.3/ontolearn_light/fitness_functions.py`

 * *Files identical despite different names*

### Comparing `ontosample-0.2.2/ontolearn_light/knowledge_base.py` & `ontosample-0.2.3/ontolearn_light/knowledge_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,50 @@
 """ Knowledge Base."""
 
 import logging
 import random
-from typing import Iterable, Optional, Callable, overload, Union, FrozenSet, Set, Dict, cast
+from collections import Counter
+from typing import Iterable, Optional, Callable, overload, Union, FrozenSet, Set, Dict, cast, Generator
 
 import owlapy
+from owlapy.class_expression import OWLClassExpression, OWLClass, OWLObjectSomeValuesFrom, OWLObjectAllValuesFrom, \
+    OWLThing, OWLObjectMinCardinality, OWLObjectOneOf
+from owlapy.iri import IRI
+from owlapy.owl_axiom import OWLClassAssertionAxiom, OWLObjectPropertyAssertionAxiom, OWLDataPropertyAssertionAxiom, \
+    OWLSubClassOfAxiom, OWLEquivalentClassesAxiom
+from owlapy.owl_data_ranges import OWLDataRange
+from owlapy.owl_datatype import OWLDatatype
+from owlapy.owl_individual import OWLNamedIndividual
+from owlapy.owl_literal import BooleanOWLDatatype, NUMERIC_DATATYPES, DoubleOWLDatatype, TIME_DATATYPES, OWLLiteral
+from owlapy.owl_ontology import OWLOntology
+from owlapy.owl_ontology_manager import OWLOntologyManager
+from owlapy.owl_property import OWLObjectProperty, OWLDataProperty, OWLObjectPropertyExpression, \
+    OWLDataPropertyExpression
+from owlapy.owl_reasoner import OWLReasoner
 
 from ontolearn_light.base import OWLOntology_Owlready2, OWLOntologyManager_Owlready2, OWLReasoner_Owlready2
 from ontolearn_light.base.fast_instance_checker import OWLReasoner_FastInstanceChecker
-from owlapy.model import OWLOntologyManager, OWLOntology, OWLReasoner, OWLClassExpression, \
-    OWLNamedIndividual, OWLObjectProperty, OWLClass, OWLDataProperty, IRI, OWLDataRange, OWLObjectSomeValuesFrom, \
-    OWLObjectAllValuesFrom, OWLDatatype, BooleanOWLDatatype, NUMERIC_DATATYPES, TIME_DATATYPES, OWLThing, \
-    OWLObjectPropertyExpression, OWLLiteral, OWLDataPropertyExpression, OWLClassAssertionAxiom, \
-    OWLObjectPropertyAssertionAxiom, OWLDataPropertyAssertionAxiom, OWLSubClassOfAxiom, OWLEquivalentClassesAxiom
+
 from owlapy.render import DLSyntaxObjectRenderer
 from ontolearn_light.search import EvaluatedConcept
 from owlapy.util import iter_count, LRUCache
 from .abstracts import AbstractKnowledgeBase, AbstractScorer, EncodedLearningProblem
 from .concept_generator import ConceptGenerator
 from ontolearn_light.base.owl.utils import OWLClassExpressionLengthMetric
 from .learning_problem import PosNegLPStandard, EncodedPosNegLPStandard
 from ontolearn_light.base.owl.hierarchy import ClassHierarchy, ObjectPropertyHierarchy, DatatypePropertyHierarchy
 
 from .utils.static_funcs import (init_length_metric, init_hierarchy_instances,
                                  init_named_individuals, init_individuals_from_concepts)
 
+from owlapy.class_expression import OWLDataMaxCardinality, OWLDataSomeValuesFrom
+from owlapy import owl_expression_to_sparql, owl_expression_to_dl
+from owlapy.owl_data_ranges import OWLDataRange
+from owlapy.class_expression import OWLDataOneOf
+
 logger = logging.getLogger(__name__)
 
 
 def depth_Default_ReasonerFactory(onto: OWLOntology) -> OWLReasoner:
     assert isinstance(onto, OWLOntology_Owlready2)
     base_reasoner = OWLReasoner_Owlready2(ontology=onto)
     return OWLReasoner_FastInstanceChecker(ontology=onto, base_reasoner=base_reasoner)
@@ -53,15 +69,14 @@
             Individuals (does not contain this type) as individuals.
 
     Attributes:
         generator (ConceptGenerator): Instance of concept generator.
         path (str): Path of the ontology file.
         use_individuals_cache (bool): Whether to use individuals cache to store individuals for method efficiency.
     """
-
     # __slots__ = '_manager', '_ontology', '_reasoner', '_length_metric', \
     #    '_ind_set', '_ind_cache', 'path', 'use_individuals_cache', 'generator', '_class_hierarchy', \
     #    '_object_property_hierarchy', '_data_property_hierarchy', '_op_domains', '_op_ranges', '_dp_domains', \
     #    '_dp_ranges'
 
     length_metric: OWLClassExpressionLengthMetric
 
@@ -85,14 +100,15 @@
                  include_implicit_individuals=False):
         ...
 
     @overload
     def __init__(self, *,
                  ontology: OWLOntology,
                  reasoner: OWLReasoner,
+                 load_class_hierarchy: bool = True,
                  length_metric: Optional[OWLClassExpressionLengthMetric] = None,
                  length_metric_factory: Optional[Callable[[], OWLClassExpressionLengthMetric]] = None,
                  individuals_cache_size=128):
         ...
 
     def __init__(self, *,
                  path: Optional[str] = None,
@@ -104,14 +120,15 @@
                  ontology: Optional[OWLOntology] = None,
                  reasoner: Optional[OWLReasoner] = None,
                  length_metric: Optional[OWLClassExpressionLengthMetric] = None,
 
                  individuals_cache_size=128,
                  backend_store: bool = False,
                  class_hierarchy: Optional[ClassHierarchy] = None,
+                 load_class_hierarchy: bool = True,
                  object_property_hierarchy: Optional[ObjectPropertyHierarchy] = None,
                  data_property_hierarchy: Optional[DatatypePropertyHierarchy] = None,
                  include_implicit_individuals=False
                  ):
         AbstractKnowledgeBase.__init__(self)
         self.path = path
 
@@ -144,23 +161,24 @@
         else:
             self.reasoner = OWLReasoner_FastInstanceChecker(ontology=self.ontology,
                                                             base_reasoner=OWLReasoner_Owlready2(
                                                                 ontology=self.ontology))
 
         self.length_metric = init_length_metric(length_metric, length_metric_factory)
 
-        self.class_hierarchy: ClassHierarchy
-        self.object_property_hierarchy: ObjectPropertyHierarchy
-        self.data_property_hierarchy: DatatypePropertyHierarchy
-        (self.class_hierarchy,
-         self.object_property_hierarchy,
-         self.data_property_hierarchy) = init_hierarchy_instances(self.reasoner,
-                                                                  class_hierarchy=class_hierarchy,
-                                                                  object_property_hierarchy=object_property_hierarchy,
-                                                                  data_property_hierarchy=data_property_hierarchy)
+        if load_class_hierarchy:
+            self.class_hierarchy: ClassHierarchy
+            self.object_property_hierarchy: ObjectPropertyHierarchy
+            self.data_property_hierarchy: DatatypePropertyHierarchy
+            (self.class_hierarchy,
+             self.object_property_hierarchy,
+             self.data_property_hierarchy) = init_hierarchy_instances(self.reasoner,
+                                                                      class_hierarchy=class_hierarchy,
+                                                                      object_property_hierarchy=object_property_hierarchy,
+                                                                      data_property_hierarchy=data_property_hierarchy)
         # Object property domain and range:
         self.op_domains: Dict[OWLObjectProperty, OWLClassExpression]
         self.op_domains = dict()
         self.op_ranges: Dict[OWLObjectProperty, OWLClassExpression]
         self.op_ranges = dict()
         # Data property domain and range:g
         self.dp_domains: Dict[OWLDataProperty, OWLClassExpression]
@@ -191,34 +209,35 @@
 
         if concept is None or concept.is_owl_thing():
             for i in self.ind_set:
                 yield i
         else:
             yield from self.maybe_cache_individuals(concept)
 
-    def abox(self, individuals: Union[OWLNamedIndividual, Iterable[OWLNamedIndividual]] = None, mode='native'):
+    def abox(self, individual: Union[OWLNamedIndividual, Iterable[OWLNamedIndividual]] = None, mode='native'):
         """
         Get all the abox axioms for a given individual. If no individual is given, get all abox axioms
 
         Args:
-            individuals (OWLNamedIndividual): Individual/s to get the abox axioms from.
+            individual (OWLNamedIndividual): Individual/s to get the abox axioms from.
             mode (str): The return format.
              1) 'native' -> returns triples as tuples of owlapy objects,
              2) 'iri' -> returns triples as tuples of IRIs as string,
              3) 'axiom' -> triples are represented by owlapy axioms.
 
         Returns: Iterable of tuples or owlapy axiom, depending on the mode.
         """
 
-        assert mode in ['native', 'iri', 'axiom'], "Valid modes are: 'native', 'iri' or 'axiom'"
+        assert mode in ['native', 'iri', 'axiom',
+                        "expression"], "Valid modes are: 'native', 'iri' ,'expression' or 'axiom'"
 
-        if isinstance(individuals, OWLNamedIndividual):
-            inds = [individuals]
-        elif isinstance(individuals, Iterable):
-            inds = individuals
+        if isinstance(individual, OWLNamedIndividual):
+            inds = [individual]
+        elif isinstance(individual, Iterable):
+            inds = individual
         else:
             inds = self.individuals()
 
         for i in inds:
             if mode == "native":
                 # Obtain all class assertion triples/axioms
                 # For now, 'rdfs:type' predicate will be represented as an IRI
@@ -229,36 +248,82 @@
                 for dp in self.get_data_properties_for_ind(ind=i):
                     yield from ((i, dp, literal) for literal in self.get_data_property_values(i, dp))
 
                 for op in self.get_object_properties_for_ind(ind=i):
                     yield from ((i, op, ind) for ind in self.get_object_property_values(i, op))
             elif mode == "iri":
                 yield from ((i.str, "http://www.w3.org/1999/02/22-rdf-syntax-ns#type",
-                             t.get_iri().as_str()) for t in self.get_types(ind=i, direct=True))
+                             t.str) for t in self.get_types(ind=i, direct=True))
                 for dp in self.get_data_properties_for_ind(ind=i):
-                    yield from ((i.str, dp.get_iri().as_str(), literal.get_literal()) for literal in
+                    yield from ((i.str, dp.str, literal.get_literal()) for literal in
                                 self.get_data_property_values(i, dp))
                 for op in self.get_object_properties_for_ind(ind=i):
-                    yield from ((i.str, op.get_iri().as_str(), ind.get_iri().as_str()) for ind in
+                    yield from ((i.str, op.str, ind.str) for ind in
                                 self.get_object_property_values(i, op))
             elif mode == "axiom":
                 yield from (OWLClassAssertionAxiom(i, t) for t in self.get_types(ind=i, direct=True))
                 for dp in self.get_data_properties_for_ind(ind=i):
                     yield from (OWLDataPropertyAssertionAxiom(i, dp, literal) for literal in
                                 self.get_data_property_values(i, dp))
                 for op in self.get_object_properties_for_ind(ind=i):
                     yield from (OWLObjectPropertyAssertionAxiom(i, op, ind) for ind in
                                 self.get_object_property_values(i, op))
+            elif mode == "expression":
+                object_restrictions_quantifiers = dict()
+                # To no return duplicate objects.
+                quantifier_gate = set()
+                # (1) Iterate over triples where individual is in the subject position. Recursion
+                for s, p, o in self.abox(individual=individual, mode="native"):
+                    if isinstance(p, IRI) and isinstance(o, OWLClass):
+                        """ Return OWLClass """
+                        yield o
+                    elif isinstance(p, OWLObjectProperty) and isinstance(o, OWLNamedIndividual):
+                        """ STORE: ObjectSomeValuesFrom with ObjectOneOf over OWLNamedIndividual"""
+                        object_restrictions_quantifiers.setdefault(p, []).append(o)
+                    elif isinstance(p, OWLDataProperty) and isinstance(o, OWLLiteral):
+                        """ RETURN: OWLDataSomeValuesFrom with OWLDataOneOf over OWLLiteral"""
+                        yield OWLDataSomeValuesFrom(property=p, filler=OWLDataOneOf(o))
+                    else:
+                        raise RuntimeError("Unrecognized triples to expression mappings")
+
+                for k, iter_inds in object_restrictions_quantifiers.items():
+                    # RETURN Existential Quantifiers over Nominals: \exists r. {x....y}
+                    for x in iter_inds:
+                        yield OWLObjectSomeValuesFrom(property=k, filler=OWLObjectOneOf(values=x))
+                    type_: OWLClass
+                    count: int
+                    for type_, count in Counter(
+                            [type_i for i in iter_inds for type_i in self.get_types(ind=i, direct=True)]).items():
+                        existential_quantifier = OWLObjectSomeValuesFrom(property=k, filler=type_)
+                        if existential_quantifier in quantifier_gate:
+                            continue
+                        else:
+                            # RETURN Existential Quantifiers over Concepts: \exists r. C
+                            quantifier_gate.add(existential_quantifier)
+                            yield existential_quantifier
+                        if count > 1:
+                            min_cardinality_item = OWLObjectMinCardinality(cardinality=count, property=k, filler=type_)
+                            if min_cardinality_item in quantifier_gate:
+                                continue
+                            else:
+                                quantifier_gate.add(min_cardinality_item)
+                                # RETURN \ge number r. C
+                                yield min_cardinality_item
+
+
+            else:
+                raise RuntimeError(f"Unrecognized mode:{mode}")
 
     def tbox(self, entities: Union[Iterable[OWLClass], Iterable[OWLDataProperty], Iterable[OWLObjectProperty], OWLClass,
-                                   OWLDataProperty, OWLObjectProperty, None] = None, mode='native'):
+    OWLDataProperty, OWLObjectProperty, None] = None, mode='native'):
         """Get all the tbox axioms for the given concept-s|propert-y/ies.
          If no concept-s|propert-y/ies are given, get all tbox axioms.
 
          Args:
+             @TODO: entities or namedindividuals ?!
              entities: Entities to obtain tbox axioms from. This can be a single
               OWLClass/OWLDataProperty/OWLObjectProperty object, a list of those objects or None. If you enter a list
               that combines classes and properties (which we don't recommend doing), only axioms for one type will be
               returned, whichever comes first (classes or props).
              mode (str): The return format.
               1) 'native' -> returns triples as tuples of owlapy objects,
               2) 'iri' -> returns triples as tuples of IRIs as string,
@@ -293,27 +358,29 @@
                     continue
                 if mode == 'native':
                     [results.add((j, IRI.create("http://www.w3.org/2000/01/rdf-schema#subClassOf"), concept)) for j in
                      self.get_direct_sub_concepts(concept)]
                     [results.add((concept, IRI.create("http://www.w3.org/2002/07/owl#equivalentClass"), j)) for j in
                      self.reasoner.equivalent_classes(concept, only_named=True)]
                     if not include_all:  # This kind of check is just for performance purposes
-                        [results.add((concept, IRI.create("http://www.w3.org/2000/01/rdf-schema#subClassOf"), j)) for j in
+                        [results.add((concept, IRI.create("http://www.w3.org/2000/01/rdf-schema#subClassOf"), j)) for j
+                         in
                          self.get_direct_parents(concept)]
                 elif mode == 'iri':
-                    [results.add((j.get_iri().as_str(), "http://www.w3.org/2000/01/rdf-schema#subClassOf",
-                                  concept.get_iri().as_str())) for j in self.get_direct_sub_concepts(concept)]
-                    [results.add((concept.get_iri().as_str(), "http://www.w3.org/2002/07/owl#equivalentClass",
-                                  cast(OWLClass, j).get_iri().as_str())) for j in
+                    [results.add((j.str, "http://www.w3.org/2000/01/rdf-schema#subClassOf",
+                                  concept.str)) for j in self.get_direct_sub_concepts(concept)]
+                    [results.add((concept.str, "http://www.w3.org/2002/07/owl#equivalentClass",
+                                  cast(OWLClass, j).str)) for j in
                      self.reasoner.equivalent_classes(concept, only_named=True)]
                     if not include_all:
-                        [results.add((concept.get_iri().as_str(), "http://www.w3.org/2000/01/rdf-schema#subClassOf",
-                                      j.get_iri().as_str())) for j in self.get_direct_parents(concept)]
+                        [results.add((concept.str, "http://www.w3.org/2000/01/rdf-schema#subClassOf",
+                                      j.str)) for j in self.get_direct_parents(concept)]
                 elif mode == "axiom":
-                    [results.add(OWLSubClassOfAxiom(super_class=concept, sub_class=j)) for j in self.get_direct_sub_concepts(concept)]
+                    [results.add(OWLSubClassOfAxiom(super_class=concept, sub_class=j)) for j in
+                     self.get_direct_sub_concepts(concept)]
                     [results.add(OWLEquivalentClassesAxiom([concept, j])) for j in
                      self.reasoner.equivalent_classes(concept, only_named=True)]
                     if not include_all:
                         [results.add(OWLSubClassOfAxiom(super_class=j, sub_class=concept)) for j in
                          self.get_direct_parents(concept)]
         if include_all or not classes:
             for prop in ens:
@@ -332,47 +399,49 @@
                      getattr(self.reasoner, prop_type.lower() + "_property_domains")(prop, direct=True)]
                     [results.add((prop, IRI.create("http://www.w3.org/2000/01/rdf-schema#range"), j)) for j in
                      getattr(self.reasoner, prop_type.lower() + "_property_ranges")(prop, direct=True)]
                     if not include_all:
                         [results.add((prop, IRI.create("http://www.w3.org/2000/01/rdf-schema#subPropertyOf"), j)) for j
                          in getattr(self.reasoner, "super_" + prop_type.lower() + "_properties")(prop, direct=True)]
                 elif mode == 'iri':
-                    [results.add((j.get_iri().as_str(), "http://www.w3.org/2000/01/rdf-schema#subPropertyOf",
-                                  prop.get_iri().as_str())) for j in
+                    [results.add((j.str, "http://www.w3.org/2000/01/rdf-schema#subPropertyOf",
+                                  prop.str)) for j in
                      getattr(self.reasoner, "sub_" + prop_type.lower() + "_properties")(prop, direct=True)]
-                    [results.add((prop.get_iri().as_str(), "http://www.w3.org/2002/07/owl#equivalentProperty",
-                                  j.get_iri().as_str())) for j in
+                    [results.add((prop.str, "http://www.w3.org/2002/07/owl#equivalentProperty",
+                                  j.str)) for j in
                      getattr(self.reasoner, "equivalent_" + prop_type.lower() + "_properties")(prop)]
-                    [results.add((prop.get_iri().as_str(), "http://www.w3.org/2000/01/rdf-schema#domain",
-                                  j.get_iri().as_str())) for j in
+                    [results.add((prop.str, "http://www.w3.org/2000/01/rdf-schema#domain",
+                                  j.str)) for j in
                      getattr(self.reasoner, prop_type.lower() + "_property_domains")(prop, direct=True)]
                     if prop_type == 'Object':
-                        [results.add((prop.get_iri().as_str(), "http://www.w3.org/2000/01/rdf-schema#range",
-                                      j.get_iri().as_str())) for j in
+                        [results.add((prop.str, "http://www.w3.org/2000/01/rdf-schema#range",
+                                      j.str)) for j in
                          self.reasoner.object_property_ranges(prop, direct=True)]
                     # # ranges of data properties not implemented for this mode
                     # else:
-                    #     [results.add((prop.get_iri().as_str(), "http://www.w3.org/2000/01/rdf-schema#range",
+                    #     [results.add((prop.str, "http://www.w3.org/2000/01/rdf-schema#range",
                     #                   str(j))) for j in self.reasoner.data_property_ranges(prop, direct=True)]
 
                     if not include_all:
-                        [results.add((prop.get_iri().as_str(), "http://www.w3.org/2000/01/rdf-schema#subPropertyOf",
-                                      j.get_iri().as_str())) for j
+                        [results.add((prop.str, "http://www.w3.org/2000/01/rdf-schema#subPropertyOf",
+                                      j.str)) for j
                          in getattr(self.reasoner, "super_" + prop_type.lower() + "_properties")(prop, direct=True)]
                 elif mode == 'axiom':
-                    [results.add(getattr(owlapy.model, "OWLSub" + prop_type + "PropertyOfAxiom")(j, prop)) for j in
+                    [results.add(getattr(owlapy.owl_axiom, "OWLSub" + prop_type + "PropertyOfAxiom")(j, prop)) for j in
                      getattr(self.reasoner, "sub_" + prop_type.lower() + "_properties")(prop, direct=True)]
-                    [results.add(getattr(owlapy.model, "OWLEquivalent" + prop_type + "PropertiesAxiom")([j, prop])) for j in
+                    [results.add(getattr(owlapy.owl_axiom, "OWLEquivalent" + prop_type + "PropertiesAxiom")([j, prop]))
+                     for
+                     j in
                      getattr(self.reasoner, "equivalent_" + prop_type.lower() + "_properties")(prop)]
-                    [results.add(getattr(owlapy.model, "OWL" + prop_type + "PropertyDomainAxiom")(prop, j)) for j in
+                    [results.add(getattr(owlapy.owl_axiom, "OWL" + prop_type + "PropertyDomainAxiom")(prop, j)) for j in
                      getattr(self.reasoner, prop_type.lower() + "_property_domains")(prop, direct=True)]
-                    [results.add(getattr(owlapy.model, "OWL" + prop_type + "PropertyRangeAxiom")(prop, j)) for j in
+                    [results.add(getattr(owlapy.owl_axiom, "OWL" + prop_type + "PropertyRangeAxiom")(prop, j)) for j in
                      getattr(self.reasoner, prop_type.lower() + "_property_ranges")(prop, direct=True)]
                     if not include_all:
-                        [results.add(getattr(owlapy.model, "OWLSub" + prop_type + "PropertyOfAxiom")(prop, j)) for j
+                        [results.add(getattr(owlapy.owl_axiom, "OWLSub" + prop_type + "PropertyOfAxiom")(prop, j)) for j
                          in getattr(self.reasoner, "super_" + prop_type.lower() + "_properties")(prop, direct=True)]
 
         return results
 
     def triples(self, mode="native"):
         """Get all tbox and abox axioms/triples.
 
@@ -383,15 +452,14 @@
               3) 'axiom' -> triples are represented by owlapy axioms.
 
         Returns: Iterable of tuples or owlapy axiom, depending on the mode.
         """
         yield from self.abox(mode=mode)
         yield from self.tbox(mode=mode)
 
-
     def ignore_and_copy(self, ignored_classes: Optional[Iterable[OWLClass]] = None,
                         ignored_object_properties: Optional[Iterable[OWLObjectProperty]] = None,
                         ignored_data_properties: Optional[Iterable[OWLDataProperty]] = None) -> 'KnowledgeBase':
         """Makes a copy of the knowledge base while ignoring specified concepts and properties.
 
         Args:
             ignored_classes: Classes to ignore.
@@ -455,14 +523,16 @@
         find the best results considering also the length of the concepts.
 
         Args:
             ce: The concept to be measured.
         Returns:
             Length of the concept.
         """
+        # @TODO: CD: Computing the length of a concept should be disantangled from KB
+        # @TODO: CD: Ideally, this should be a static function
 
         return self.length_metric.length(ce)
 
     def clean(self):
         """Clean all stored values (states and caches) if there is any.
 
         Note:
@@ -678,14 +748,34 @@
             concept: Atomic class for which to find leaf classes.
 
         Returns:
             Leaf classes { x \\| (x subClassOf concept) AND not exist y: y subClassOf x )}. """
         assert isinstance(concept, OWLClass)
         yield from self.class_hierarchy.leaves(of=concept)
 
+    def get_least_general_named_concepts(self) -> Generator[OWLClass, None, None]:
+        """Get leaf classes.
+        @TODO: Docstring needed
+        Returns:
+        """
+        yield from self.class_hierarchy.leaves()
+
+    def least_general_named_concepts(self) -> Generator[OWLClass, None, None]:
+        """Get leaf classes.
+        @TODO: Docstring needed
+        Returns:
+        """
+        yield from self.class_hierarchy.leaves()
+
+    def get_most_general_classes(self) -> Generator[OWLClass, None, None]:
+        """Get most general named concepts classes.
+        @TODO: Docstring needed
+        Returns:"""
+        yield from self.class_hierarchy.roots()
+
     def get_direct_sub_concepts(self, concept: OWLClass) -> Iterable[OWLClass]:
         """Direct sub-classes of atomic class.
 
         Args:
             concept: Atomic concept.
 
         Returns:
@@ -910,14 +1000,17 @@
         """Get all concepts of this concept generator.
 
         Returns:
             Concepts.
         """
         yield from self.class_hierarchy.items()
 
+    def get_classes_in_signature(self):
+        return self.get_concepts()
+
     @property
     def concepts(self) -> Iterable[OWLClass]:
         """Get all concepts of this concept generator.
 
         Returns:
             Concepts.
         """
@@ -979,14 +1072,22 @@
         """Get all numeric data properties of this concept generator.
 
         Returns:
             Numeric data properties.
         """
         yield from self.get_data_properties(NUMERIC_DATATYPES)
 
+    def get_double_data_properties(self) -> Iterable[OWLDataProperty]:
+        """Get all numeric data properties of this concept generator.
+
+        Returns:
+            Numeric data properties.
+        """
+        yield from self.get_data_properties(DoubleOWLDatatype)
+
     def get_time_data_properties(self) -> Iterable[OWLDataProperty]:
         """Get all time data properties of this concept generator.
 
         Returns:
             Time data properties.
         """
         yield from self.get_data_properties(TIME_DATATYPES)
@@ -1084,8 +1185,8 @@
     def __repr__(self):
         properties_count = iter_count(self.ontology.object_properties_in_signature()) + iter_count(
             self.ontology.data_properties_in_signature())
         class_count = iter_count(self.ontology.classes_in_signature())
         individuals_count = self.individuals_count()
 
         return f'KnowledgeBase(path={repr(self.path)} <{class_count} classes, {properties_count} properties, ' \
-               f'{individuals_count} individuals)'
+               f'{individuals_count} individuals)'
```

### Comparing `ontosample-0.2.2/ontolearn_light/learning_problem.py` & `ontosample-0.2.3/ontolearn_light/learning_problem.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Learning problem in Ontolearn."""
 import logging
 from typing import Set, Optional, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from ontolearn_light.knowledge_base import KnowledgeBase
 from ontolearn_light.abstracts import AbstractLearningProblem, EncodedLearningProblem, EncodedPosNegLPStandardKind
-from owlapy.model import OWLNamedIndividual
+from owlapy.owl_individual import OWLNamedIndividual
 
 logger = logging.getLogger(__name__)
 
 
 class EncodedPosNegLPStandard(EncodedPosNegLPStandardKind):
     """Encoded learning problem standard.
```

### Comparing `ontosample-0.2.2/ontolearn_light/metrics.py` & `ontosample-0.2.3/ontolearn_light/metrics.py`

 * *Files identical despite different names*

### Comparing `ontosample-0.2.2/ontolearn_light/search.py` & `ontosample-0.2.3/ontolearn_light/search.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """Node representation."""
 import weakref
 from _weakref import ReferenceType
 from abc import abstractmethod, ABCMeta
 from functools import total_ordering
 from queue import PriorityQueue
 from typing import List, Optional, ClassVar, Final, Iterable, TypeVar, Generic, Set, Tuple, Dict
-
-from owlapy.io import OWLObjectRenderer
-from owlapy.model import OWLClassExpression
+from owlapy.owl_object import OWLObjectRenderer
+from owlapy.class_expression import OWLClassExpression
 from owlapy.render import DLSyntaxObjectRenderer
 from owlapy.util import as_index, OrderedOWLObject
 from .abstracts import AbstractNode, AbstractHeuristic, AbstractScorer, AbstractOEHeuristicNode, LBLSearchTree, \
     AbstractConceptNode, EncodedLearningProblem, DRILLAbstractTree
 
 _N = TypeVar('_N')  #:
 
+from owlapy import owl_expression_to_dl
+
 
 # Due to a bug in Python, we cannot use the slots like we should be able to. Hence, the attribute access is also
 # invalid but there is nothing we can do. See https://mail.python.org/pipermail/python-list/2002-December/126637.html
 
 # noinspection PyUnresolvedReferences
 # noinspection PyDunderSlots
 class _NodeConcept(metaclass=ABCMeta):
@@ -195,16 +196,16 @@
         ))
 
 
 class OENode(_NodeConcept, _NodeLen, _NodeIndividualsCount, _NodeQuality, _NodeHeuristic,
              _NodeParentRef['OENode'], AbstractNode, AbstractConceptNode, AbstractOEHeuristicNode):
     """OENode search tree node."""
     __slots__ = '_concept', '_len', '_individuals_count', '_quality', '_heuristic', \
-                '_parent_ref', '_horizontal_expansion', \
-                '_refinement_count', '__weakref__'
+        '_parent_ref', '_horizontal_expansion', \
+        '_refinement_count', '__weakref__'
 
     renderer: ClassVar[OWLObjectRenderer] = DLSyntaxObjectRenderer()
 
     _horizontal_expansion: int
     _refinement_count: int
 
     def __init__(self, concept: OWLClassExpression, length: int, parent_node: Optional['OENode'] = None,
@@ -244,14 +245,15 @@
             _NodeHeuristic.__str__(self),
             _NodeParentRef.__str__(self),
             f'H_exp:{self.h_exp}',
             f'|RC|:{self.refinement_count}',
             _NodeIndividualsCount.__str__(self),
         ))
 
+
 class EvoLearnerNode(_NodeConcept, _NodeLen, _NodeIndividualsCount, _NodeQuality, AbstractNode, AbstractConceptNode):
     """
     EvoLearner search tree node.
     """
     __slots__ = '_concept', '_len', '_individuals_count', '_quality', '_tree_length', '_tree_depth'
 
     _tree_length: int
@@ -288,61 +290,80 @@
             f'Length:{self._len}',
             f'Tree Length:{self._tree_length}',
             f'Tree Depth:{self._tree_depth}',
             _NodeIndividualsCount.__str__(self),
         ))
 
 
+class NCESNode(_NodeConcept, _NodeLen, _NodeIndividualsCount, _NodeQuality, AbstractNode, AbstractConceptNode):
+    """
+    EvoLearner search tree node.
+    """
+    __slots__ = '_concept', '_len', '_individuals_count', '_quality'
+
+    def __init__(self,
+                 concept: OWLClassExpression,
+                 length: int,
+                 individuals_count: int,
+                 quality: float):
+        _NodeConcept.__init__(self, concept)
+        _NodeLen.__init__(self, length)
+        _NodeIndividualsCount.__init__(self, individuals_count)
+        _NodeQuality.__init__(self, quality)
+        AbstractNode.__init__(self)
+
+    def __str__(self):
+        return "\t".join((
+            AbstractNode.__str__(self),
+            _NodeConcept.__str__(self),
+            _NodeQuality.__str__(self),
+            f'Length:{self._len}',
+            _NodeIndividualsCount.__str__(self),
+        ))
+
 
 class RL_State(_NodeConcept, _NodeQuality, _NodeHeuristic, AbstractNode, _NodeParentRef['RL_State']):
     renderer: ClassVar[OWLObjectRenderer] = DLSyntaxObjectRenderer()
     """RL_State node."""
-    __slots__ = '_concept', '_quality', '_heuristic', \
-                'embeddings', 'individuals', \
-                'instances_bitset', 'length', 'instances', 'parent_node', 'is_root', '_parent_ref', '__weakref__'
+    __slots__ = '_concept', 'embeddings', '_quality', '_heuristic', 'length', 'parent_node', 'is_root', '_parent_ref', '__weakref__'
 
-    def __init__(self, concept: OWLClassExpression, parent_node: Optional['RL_State'] = None, is_root: bool = False,
-                 embeddings=None, instances=None, instances_set=None, length=None):
+    def __init__(self, concept: OWLClassExpression, parent_node: Optional['RL_State'] = None,
+                 embeddings=None, is_root: bool = False, length=None):
         _NodeConcept.__init__(self, concept)
         _NodeQuality.__init__(self)
         _NodeHeuristic.__init__(self)
         _NodeParentRef.__init__(self, parent_node=parent_node, is_root=is_root)
-        # TODO: CD _NodeParentRef causes unintended results:
-        #  Without using _NodeParentRef, one can reach the top class expression via recursive calling parent_node
-        #  However, if one uses _NodeParentRef amd comments self.parent_node and self.is_root, we can reach T.
         AbstractNode.__init__(self)
         self.parent_node = parent_node
         self.is_root = is_root
-
-        self.embeddings = embeddings  # tensor
-        self.instances = instances  # list
-        self.instances_bitset = instances_set  # bitset
         self.length = length
+        self.embeddings = embeddings
         self.__sanity_checking()
 
     def __sanity_checking(self):
         assert self.concept
         if self.is_root is False:
             assert self.parent_node
 
     def __str__(self):
-
-        if self.instances is None:
-            s = 'Not Init.'
+        if self.embeddings is None:
+            return "\t".join((
+                AbstractNode.__str__(self),
+                _NodeConcept.__str__(self),
+                _NodeQuality.__str__(self),
+                _NodeHeuristic.__str__(self),
+                f'Length:{self.length}'))
         else:
-            s = len(self.instances)
-
-        return "\t".join((
-            AbstractNode.__str__(self),
-            _NodeConcept.__str__(self),
-            _NodeQuality.__str__(self),
-            _NodeHeuristic.__str__(self),
-            f'|Instance|:{s}',
-            f'Length:{self.length}',
-        ))
+            return "\t".join((
+                AbstractNode.__str__(self),
+                _NodeConcept.__str__(self),
+                _NodeQuality.__str__(self),
+                _NodeHeuristic.__str__(self),
+                f'Length:{self.length}',
+                f'Embeddings:{self.embeddings.shape}',))
 
     def __lt__(self, other):
         return self.heuristic <= other.heuristic
 
     def __gt__(self, other):
         return self.heuristic > other.heuristic
 
@@ -659,14 +680,16 @@
             assert isinstance(parent_tree_node, TreeNode)
             parent_tree_node.children.add(self)
 
 
 class DRILLSearchTreePriorityQueue(DRILLAbstractTree):
     """
 
+    #@TODO Move to learners/drill.py
+
     Search tree based on priority queue.
 
     Parameters
     ----------
     quality_func : An instance of a subclass of AbstractScorer that measures the quality of a node.
     heuristic_func : An instance of a subclass of AbstractScorer that measures the promise of a node.
 
@@ -691,39 +714,51 @@
         Parameters
         ----------
         node : A RL_State object
         Returns
         -------
         None
         """
-        assert node.quality > 0
+        assert node.quality > 0, f"{RL_State.concept} cannot be added into the search tree"
         assert node.heuristic is not None
-        self.items_in_queue.put((-node.heuristic, node))  # gets the smallest one.
-        self.nodes[node] = node
+        dl_representation = owl_expression_to_dl(node.concept.get_nnf())
+        if dl_representation in self.nodes:
+            """Do nothing"""
+        else:
+            self.items_in_queue.put(
+                (-node.heuristic, len(owl_expression_to_dl(node.concept)), dl_representation))  # gets the smallest one.
+            self.nodes[dl_representation] = node
+
+    def show_current_search_tree(self, top_n=10):
+        """
+        Show search tree.
+        """
+        predictions = sorted(
+            [(neg_heuristic, length, self.nodes[dl_representation]) for neg_heuristic, length, dl_representation in
+             self.items_in_queue.queue])[:top_n]
+        print(f"\n######## Current Search Tree {len(self.items_in_queue.queue)} ###########\n")
+        for ith, (_, __, node) in enumerate(predictions):
+            print(
+                f"{ith + 1}-\t{owl_expression_to_dl(node.concept)} | Quality:{node.quality:.3f}| Heuristic:{node.heuristic:.3f}")
+        print('\n######## Current Search Tree ###########\n')
+        return predictions
 
-    def get_most_promising(self) -> Node:
+    def get_most_promising(self) -> RL_State:
         """
         Gets the current most promising node from Queue.
 
         Returns
         -------
         node: A node object
         """
-        _, most_promising_str = self.items_in_queue.get()  # get
-        try:
-            node = self.nodes[most_promising_str]
-            # We do not need to put the node again into the queue.
-            # self.items_in_queue.put((-node.heuristic, node.concept.name))
-            return node
-        except KeyError:
-            print(most_promising_str, 'is not found')
-            print('####')
-            for k, v in self.nodes.items():
-                print(k)
-            exit(1)
+        assert len(self.items_in_queue.queue) > 0
+        _, __, dl_representation = self.items_in_queue.get(timeout=1.0)
+        # R
+        node = self.nodes[dl_representation]
+        return node
 
     def get_top_n(self, n: int, key='quality') -> List[Node]:
         """
         Gets the top n nodes determined by key from the search tree.
 
         Returns
         -------
```

### Comparing `ontosample-0.2.2/ontolearn_light/utils/__init__.py` & `ontosample-0.2.3/ontolearn_light/utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 """Ontolearn utils."""
 import datetime
 import os
 import pickle
 import random
 import time
 from typing import Callable, Set, TypeVar, Tuple, Union
-
+from owlapy.class_expression import OWLClass
+from owlapy.iri import IRI
+from owlapy.meta_classes import HasIRI
+from owlapy.owl_individual import OWLNamedIndividual
 from ontolearn_light.utils.log_config import setup_logging  # noqa: F401
-from owlapy.model import OWLNamedIndividual, IRI, OWLClass, HasIRI
 import pandas as pd
-
+from .static_funcs import compute_f1_score
 Factory = Callable
 
 # DEFAULT_FMT = '[{elapsed:0.8f}s] {name}({args}) -> {result}'
 DEFAULT_FMT = 'Func:{name} took {elapsed:0.8f}s'
 flag_for_performance = False
```

### Comparing `ontosample-0.2.2/ontolearn_light/utils/log_config.py` & `ontosample-0.2.3/ontolearn_light/utils/log_config.py`

 * *Files identical despite different names*

### Comparing `ontosample-0.2.2/ontosample/_base.py` & `ontosample-0.2.3/ontosample/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 import random
 import logging
 from typing import Iterable
+
+from owlapy.iri import IRI
+from owlapy.owl_axiom import OWLObjectPropertyAssertionAxiom, OWLDeclarationAxiom, OWLDataPropertyAssertionAxiom
+from owlapy.owl_individual import OWLNamedIndividual
+
 try:
     from ontolearn.knowledge_base import KnowledgeBase
     from ontolearn.base import OWLReasoner_FastInstanceChecker, OWLReasoner_Owlready2, \
         OWLOntologyManager_Owlready2
 except ModuleNotFoundError:
     from ontolearn_light.knowledge_base import KnowledgeBase
     from ontolearn_light.base import OWLReasoner_FastInstanceChecker, OWLReasoner_Owlready2, OWLOntologyManager_Owlready2
-from owlapy.model import OWLNamedIndividual, OWLObjectPropertyAssertionAxiom, \
-    OWLDataPropertyAssertionAxiom, OWLDeclarationAxiom, IRI
 
 logger = logging.getLogger(__name__)
 
 
 class Neighbor:
     """
         Class structure to save a neighbor node in such a way that it also stores the edge type which make the
```

### Comparing `ontosample-0.2.2/ontosample/classic_samplers.py` & `ontosample-0.2.3/ontosample/classic_samplers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import random
 import logging
 import numpy as np
 from typing import List
 from collections import deque
-from owlapy.model import OWLNamedIndividual
+from owlapy.owl_individual import OWLNamedIndividual
 from ontosample._base import Sampler, Neighbor, Node
 try:
     from ontolearn.knowledge_base import KnowledgeBase
 except ModuleNotFoundError:
     from ontolearn_light.knowledge_base import KnowledgeBase
```

### Comparing `ontosample-0.2.2/ontosample/lpc_samplers.py` & `ontosample-0.2.3/ontosample/lpc_samplers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import random
 import logging
 from typing import Iterable
-from owlapy.model import OWLNamedIndividual
+from owlapy.owl_individual import OWLNamedIndividual
 from collections import deque
 from ontosample._base import Neighbor
 try:
     from ontolearn.knowledge_base import KnowledgeBase
 except ModuleNotFoundError:
     from ontolearn_light.knowledge_base import KnowledgeBase
 from ontosample.classic_samplers import RandomWalkerWithPrioritizationSampler, ForestFireSampler,\
```

### Comparing `ontosample-0.2.2/ontosample/lpf_samplers.py` & `ontosample-0.2.3/ontosample/lpf_samplers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import random
 import logging
-from typing import List, Iterable
-from owlapy.model import OWLNamedIndividual
+from typing import Iterable
+from owlapy.owl_individual import OWLNamedIndividual
 from ontosample._base import Neighbor
 try:
     from ontolearn.knowledge_base import KnowledgeBase
 except ModuleNotFoundError:
     from ontolearn_light.knowledge_base import KnowledgeBase
 from ontosample.classic_samplers import RandomWalkerWithPrioritizationSampler, RandomNodeSampler, \
     RandomEdgeSampler, RandomWalkSampler
```

### Comparing `ontosample-0.2.2/ontosample.egg-info/PKG-INFO` & `ontosample-0.2.3/ontosample.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontosample
-Version: 0.2.2
+Version: 0.2.3
 Summary: Ontosample is a package that offers different sampling techniques for OWL ontologies.
 Home-page: https://github.com/alkidbaci/OntoSample
 Author: Alkid Baci
 Author-email: alkid1baci@gmail.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
@@ -12,15 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.3.4
 Requires-Dist: owlready2>=0.40
 Requires-Dist: torch>=1.7.1
 Requires-Dist: pandas>=1.5.0
 Requires-Dist: sortedcontainers>=2.4.0
-Requires-Dist: owlapy>=0.1.1
+Requires-Dist: owlapy==1.0.2
 Requires-Dist: requests>=2.31.0
 
 # OntoSample
 
 OntoSample is a python package that offers classic sampling techniques for OWL ontologies/knowledge 
 bases. Furthermore, we have tailored the classic sampling techniques to the setting of concept 
 learning making use of learning problem.
```

### Comparing `ontosample-0.2.2/ontosample.egg-info/SOURCES.txt` & `ontosample-0.2.3/ontosample.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ontosample-0.2.2/setup.py` & `ontosample-0.2.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as fh:
     long_description = fh.read()
 setup(
     name="ontosample",
     description="Ontosample is a package that offers different sampling techniques for OWL ontologies.",
-    version="0.2.2",
+    version="0.2.3",
     packages=find_packages(),
     install_requires=[
         "matplotlib>=3.3.4",
         "owlready2>=0.40",
         "torch>=1.7.1",
         "pandas>=1.5.0",
         "sortedcontainers>=2.4.0",
-        "owlapy>=0.1.1",
+        "owlapy==1.0.2",
         "requests>=2.31.0"],
     author='Alkid Baci',
     author_email='alkid1baci@gmail.com',
     url='https://github.com/alkidbaci/OntoSample',
     classifiers=[
         "Programming Language :: Python :: 3.8",
         "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
```

