# Comparing `tmp/neo4j_genai-0.1.4.tar.gz` & `tmp/neo4j_genai-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neo4j_genai-0.1.4.tar", max compression
+gzip compressed data, was "neo4j_genai-0.2.0a1.tar", max compression
```

## Comparing `neo4j_genai-0.1.4.tar` & `neo4j_genai-0.2.0a1.tar`

### file list

```diff
@@ -1,16 +1,21 @@
--rw-r--r--   0        0        0    11360 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/LICENSE.APACHE2.txt
--rw-r--r--   0        0        0     2774 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/LICENSE.PYTHON.txt
--rw-r--r--   0        0        0      423 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/LICENSE.txt
--rw-r--r--   0        0        0      160 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/NOTICE.txt
--rw-r--r--   0        0        0     5527 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/README.md
--rw-r--r--   0        0        0     1529 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      889 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/src/neo4j_genai/__init__.py
--rw-r--r--   0        0        0      984 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/src/neo4j_genai/embedder.py
--rw-r--r--   0        0        0     4276 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/src/neo4j_genai/indexes.py
--rw-r--r--   0        0        0     2496 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/src/neo4j_genai/neo4j_queries.py
--rw-r--r--   0        0        0        0 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/src/neo4j_genai/retrievers/__init__.py
--rw-r--r--   0        0        0     1969 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/src/neo4j_genai/retrievers/base.py
--rw-r--r--   0        0        0     7145 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/src/neo4j_genai/retrievers/hybrid.py
--rw-r--r--   0        0        0     7059 2024-05-03 13:42:59.611292 neo4j_genai-0.1.4/src/neo4j_genai/retrievers/vector.py
--rw-r--r--   0        0        0     2736 2024-05-03 13:42:59.615292 neo4j_genai-0.1.4/src/neo4j_genai/types.py
--rw-r--r--   0        0        0     6263 1970-01-01 00:00:00.000000 neo4j_genai-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11360 2024-05-22 13:05:48.449641 neo4j_genai-0.2.0a1/LICENSE.APACHE2.txt
+-rw-r--r--   0        0        0     2774 2024-05-22 13:05:48.449641 neo4j_genai-0.2.0a1/LICENSE.PYTHON.txt
+-rw-r--r--   0        0        0      423 2024-05-22 13:05:48.449641 neo4j_genai-0.2.0a1/LICENSE.txt
+-rw-r--r--   0        0        0      160 2024-05-22 13:05:48.449641 neo4j_genai-0.2.0a1/NOTICE.txt
+-rw-r--r--   0        0        0     6101 2024-05-22 13:05:48.449641 neo4j_genai-0.2.0a1/README.md
+-rw-r--r--   0        0        0     1760 2024-05-22 13:05:48.449641 neo4j_genai-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0      889 2024-05-22 13:05:48.449641 neo4j_genai-0.2.0a1/src/neo4j_genai/__init__.py
+-rw-r--r--   0        0        0      984 2024-05-22 13:05:48.449641 neo4j_genai-0.2.0a1/src/neo4j_genai/embedder.py
+-rw-r--r--   0        0        0    11975 2024-05-22 13:05:48.449641 neo4j_genai-0.2.0a1/src/neo4j_genai/filters.py
+-rw-r--r--   0        0        0     5597 2024-05-22 13:05:48.449641 neo4j_genai-0.2.0a1/src/neo4j_genai/indexes.py
+-rw-r--r--   0        0        0     6556 2024-05-22 13:05:48.449641 neo4j_genai-0.2.0a1/src/neo4j_genai/neo4j_queries.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:05:48.449641 neo4j_genai-0.2.0a1/src/neo4j_genai/retrievers/__init__.py
+-rw-r--r--   0        0        0     3396 2024-05-22 13:05:48.453641 neo4j_genai-0.2.0a1/src/neo4j_genai/retrievers/base.py
+-rw-r--r--   0        0        0      749 2024-05-22 13:05:48.453641 neo4j_genai-0.2.0a1/src/neo4j_genai/retrievers/external/weaviate/__init__.py
+-rw-r--r--   0        0        0     6219 2024-05-22 13:05:48.453641 neo4j_genai-0.2.0a1/src/neo4j_genai/retrievers/external/weaviate/weaviate.py
+-rw-r--r--   0        0        0     9185 2024-05-22 13:05:48.453641 neo4j_genai-0.2.0a1/src/neo4j_genai/retrievers/hybrid.py
+-rw-r--r--   0        0        0      917 2024-05-22 13:05:48.453641 neo4j_genai-0.2.0a1/src/neo4j_genai/retrievers/utils.py
+-rw-r--r--   0        0        0     9919 2024-05-22 13:05:48.453641 neo4j_genai-0.2.0a1/src/neo4j_genai/retrievers/vector.py
+-rw-r--r--   0        0        0     4335 2024-05-22 13:05:48.453641 neo4j_genai-0.2.0a1/src/neo4j_genai/schema.py
+-rw-r--r--   0        0        0     4352 2024-05-22 13:05:48.453641 neo4j_genai-0.2.0a1/src/neo4j_genai/types.py
+-rw-r--r--   0        0        0     6950 1970-01-01 00:00:00.000000 neo4j_genai-0.2.0a1/PKG-INFO
```

### Comparing `neo4j_genai-0.1.4/LICENSE.APACHE2.txt` & `neo4j_genai-0.2.0a1/LICENSE.APACHE2.txt`

 * *Files identical despite different names*

### Comparing `neo4j_genai-0.1.4/LICENSE.PYTHON.txt` & `neo4j_genai-0.2.0a1/LICENSE.PYTHON.txt`

 * *Files identical despite different names*

### Comparing `neo4j_genai-0.1.4/README.md` & `neo4j_genai-0.2.0a1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -157,18 +157,41 @@
     [suggested changes](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/incorporating-feedback-in-your-pull-request)
     or normal pull request comments. You can apply suggested changes directly through
     the UI, and any other changes can be made in your fork and committed to the PR branch.
 -   As you update your PR and apply changes, mark each conversation as [resolved](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/commenting-on-a-pull-request#resolving-conversations).
 
 ## Run tests
 
-Open a new virtual environment and then run the tests.
+### Unit tests
+
+This should run out of the box once the dependencies are installed.
+
+```bash
+poetry run pytest tests/unit
+```
+
+### E2E tests
+
+To run e2e tests you'd need to have some services running locally:
+
+-   neo4j
+-   weaviate
+-   weaviate-text2vec-transformers
+
+The easiest way to get it up and running is via Docker compose:
+
+```bash
+docker compose -f tests/e2e/docker-compose.yml up
+```
+
+_(pro tip: if you suspect something in the databases are cached, run `docker compose -f tests/e2e/docker-compose.yml down` to remove them completely)_
+
+Once the services are running, execute the following command to run the e2e tests.
 
 ```bash
-poetry shell
-pytest tests/unit
+poetry run pytest tests/e2e
 ```
 
 ## Further information
 
 -   [The official Neo4j Python driver](https://github.com/neo4j/neo4j-python-driver)
 -   [Neo4j GenAI integrations](https://neo4j.com/docs/cypher-manual/current/genai-integrations/)
```

### Comparing `neo4j_genai-0.1.4/pyproject.toml` & `neo4j_genai-0.2.0a1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -11,39 +11,47 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 [tool.poetry]
 name = "neo4j-genai"
-version = "0.1.4"
+version = "0.2.0a1"
 description = "Python package to allow easy integration to Neo4j's GenAI features"
 authors = ["Neo4j, Inc <team-gen-ai@neo4j.com>"]
 license = "Apache License, Version 2.0"
 readme = "README.md"
 
 [[tool.poetry.packages]]
 include = "neo4j_genai"
 from = "src"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 neo4j = "^5.17.0"
 types-requests = "^2.31.0.20240218"
 pydantic = "^2.6.3"
+weaviate-client = {version = "^4.6.1", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 pylint = "^3.1.0"
 mypy = "^1.8.0"
 pytest = "^8.0.2"
 pytest-mock = "^3.12.0"
 pre-commit = { version = "^3.6.2", python = "^3.9" }
 coverage = "^7.4.3"
 ruff = "^0.3.0"
 langchain-openai = "^0.1.1"
+weaviate-client = "^4.6.1"
+sentence-transformers = "^2.7.0"
+langchain-community = "^0.2.0"
+requests = "^2.32.0"
+
+[tool.poetry.extras]
+external_clients = ["weaviate-client"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 testpaths = ["tests"]
```

### Comparing `neo4j_genai-0.1.4/src/neo4j_genai/__init__.py` & `neo4j_genai-0.2.0a1/src/neo4j_genai/__init__.py`

 * *Files identical despite different names*

### Comparing `neo4j_genai-0.1.4/src/neo4j_genai/embedder.py` & `neo4j_genai-0.2.0a1/src/neo4j_genai/embedder.py`

 * *Files identical despite different names*

### Comparing `neo4j_genai-0.1.4/src/neo4j_genai/indexes.py` & `neo4j_genai-0.2.0a1/src/neo4j_genai/indexes.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,44 +9,52 @@
 #  #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from neo4j import Driver
+import neo4j
 from pydantic import ValidationError
 from .types import VectorIndexModel, FulltextIndexModel
+import logging
+
+
+logger = logging.getLogger(__name__)
 
 
 def create_vector_index(
-    driver: Driver,
+    driver: neo4j.Driver,
     name: str,
     label: str,
     property: str,
     dimensions: int,
     similarity_fn: str,
 ) -> None:
     """
     This method constructs a Cypher query and executes it
     to create a new vector index in Neo4j.
 
     See Cypher manual on [Create vector index](https://neo4j.com/docs/cypher-manual/current/indexes/semantic-indexes/vector-indexes/#indexes-vector-create)
 
+    Important: This operation will fail if an index with the same name already exists.
+    Ensure that the index name provided is unique within the database context.
+
     Args:
-        driver (Driver): Neo4j Python driver instance.
+        driver (neo4j.Driver): Neo4j Python driver instance.
         name (str): The unique name of the index.
         label (str): The node label to be indexed.
         property (str): The property key of a node which contains embedding values.
         dimensions (int): Vector embedding dimension
         similarity_fn (str): case-insensitive values for the vector similarity function:
             ``euclidean`` or ``cosine``.
 
     Raises:
         ValueError: If validation of the input arguments fail.
+        neo4j.exceptions.ClientError: If creation of vector index fails.
     """
     try:
         VectorIndexModel(
             **{
                 "driver": driver,
                 "name": name,
                 "label": label,
@@ -54,69 +62,92 @@
                 "dimensions": dimensions,
                 "similarity_fn": similarity_fn,
             }
         )
     except ValidationError as e:
         raise ValueError(f"Error for inputs to create_vector_index {str(e)}")
 
-    query = (
-        f"CREATE VECTOR INDEX $name FOR (n:{label}) ON n.{property} OPTIONS "
-        "{ indexConfig: { `vector.dimensions`: toInteger($dimensions), `vector.similarity_function`: $similarity_fn } }"
-    )
-    driver.execute_query(
-        query, {"name": name, "dimensions": dimensions, "similarity_fn": similarity_fn}
-    )
+    try:
+        query = (
+            f"CREATE VECTOR INDEX $name FOR (n:{label}) ON n.{property} OPTIONS "
+            "{ indexConfig: { `vector.dimensions`: toInteger($dimensions), `vector.similarity_function`: $similarity_fn } }"
+        )
+        logger.info(f"Creating vector index named '{name}'")
+        driver.execute_query(
+            query,
+            {"name": name, "dimensions": dimensions, "similarity_fn": similarity_fn},
+        )
+    except neo4j.exceptions.ClientError as e:
+        logger.error(f"Neo4j vector index creation failed {e}")
+        raise
 
 
 def create_fulltext_index(
-    driver: Driver, name: str, label: str, node_properties: list[str]
+    driver: neo4j.Driver, name: str, label: str, node_properties: list[str]
 ) -> None:
     """
     This method constructs a Cypher query and executes it
     to create a new fulltext index in Neo4j.
 
     See Cypher manual on [Create fulltext index](https://neo4j.com/docs/cypher-manual/current/indexes/semantic-indexes/full-text-indexes/#create-full-text-indexes)
 
+    Important: This operation will fail if an index with the same name already exists.
+    Ensure that the index name provided is unique within the database context.
+
     Args:
-        driver (Driver): Neo4j Python driver instance.
+        driver (neo4j.Driver): Neo4j Python driver instance.
         name (str): The unique name of the index.
         label (str): The node label to be indexed.
         node_properties (list[str]): The node properties to create the fulltext index on.
 
     Raises:
         ValueError: If validation of the input arguments fail.
+        neo4j.exceptions.ClientError: If creation of fulltext index fails.
     """
     try:
         FulltextIndexModel(
             **{
                 "driver": driver,
                 "name": name,
                 "label": label,
                 "node_properties": node_properties,
             }
         )
     except ValidationError as e:
         raise ValueError(f"Error for inputs to create_fulltext_index {str(e)}")
 
-    query = (
-        "CREATE FULLTEXT INDEX $name "
-        f"FOR (n:`{label}`) ON EACH "
-        f"[{', '.join(['n.`' + prop + '`' for prop in node_properties])}]"
-    )
-    driver.execute_query(query, {"name": name})
+    try:
+        query = (
+            "CREATE FULLTEXT INDEX $name "
+            f"FOR (n:`{label}`) ON EACH "
+            f"[{', '.join(['n.`' + prop + '`' for prop in node_properties])}]"
+        )
+        logger.info(f"Creating fulltext index named '{name}'")
+        driver.execute_query(query, {"name": name})
+    except neo4j.exceptions.ClientError as e:
+        logger.error(f"Neo4j fulltext index creation failed {e}")
+        raise
 
 
-def drop_index(driver: Driver, name: str) -> None:
+def drop_index_if_exists(driver: neo4j.Driver, name: str) -> None:
     """
     This method constructs a Cypher query and executes it
-    to drop a vector index in Neo4j.
+    to drop an index in Neo4j, if the index exists.
     See Cypher manual on [Drop vector indexes](https://neo4j.com/docs/cypher-manual/current/indexes-for-vector-search/#indexes-vector-drop)
 
     Args:
-        driver (Driver): Neo4j Python driver instance.
+        driver (neo4j.Driver): Neo4j Python driver instance.
         name (str): The name of the index to delete.
+
+    Raises:
+        neo4j.exceptions.ClientError: If dropping of index fails.
     """
-    query = "DROP INDEX $name IF EXISTS"
-    parameters = {
-        "name": name,
-    }
-    driver.execute_query(query, parameters)
+    try:
+        query = "DROP INDEX $name IF EXISTS"
+        parameters = {
+            "name": name,
+        }
+        logger.info(f"Dropping index named '{name}'")
+        driver.execute_query(query, parameters)
+    except neo4j.exceptions.ClientError as e:
+        logger.error(f"Dropping Neo4j index failed {e}")
+        raise
```

### Comparing `neo4j_genai-0.1.4/src/neo4j_genai/retrievers/hybrid.py` & `neo4j_genai-0.2.0a1/src/neo4j_genai/retrievers/hybrid.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,44 +10,72 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 from typing import Optional, Any
 
-from neo4j import Record, Driver
+import neo4j
 from pydantic import ValidationError
 
 from neo4j_genai.embedder import Embedder
 from neo4j_genai.retrievers.base import Retriever
-from neo4j_genai.types import HybridSearchModel, SearchType, HybridCypherSearchModel
+from neo4j_genai.types import (
+    HybridSearchModel,
+    SearchType,
+    HybridCypherSearchModel,
+    Neo4jDriverModel,
+    EmbedderModel,
+    HybridRetrieverModel,
+    HybridCypherRetrieverModel,
+)
 from neo4j_genai.neo4j_queries import get_search_query
+import logging
+
+logger = logging.getLogger(__name__)
 
 
 class HybridRetriever(Retriever):
     def __init__(
         self,
-        driver: Driver,
+        driver: neo4j.Driver,
         vector_index_name: str,
         fulltext_index_name: str,
         embedder: Optional[Embedder] = None,
         return_properties: Optional[list[str]] = None,
     ) -> None:
-        super().__init__(driver)
-        self.vector_index_name = vector_index_name
-        self.fulltext_index_name = fulltext_index_name
-        self.embedder = embedder
-        self.return_properties = return_properties
+        try:
+            driver_model = Neo4jDriverModel(driver=driver)
+            embedder_model = EmbedderModel(embedder=embedder) if embedder else None
+            validated_data = HybridRetrieverModel(
+                driver_model=driver_model,
+                vector_index_name=vector_index_name,
+                fulltext_index_name=fulltext_index_name,
+                embedder_model=embedder_model,
+                return_properties=return_properties,
+            )
+        except ValidationError as e:
+            raise ValueError(f"Validation failed: {e.errors()}")
+
+        super().__init__(validated_data.driver_model.driver)
+        self.vector_index_name = validated_data.vector_index_name
+        self.fulltext_index_name = validated_data.fulltext_index_name
+        self.return_properties = validated_data.return_properties
+        self.embedder = (
+            validated_data.embedder_model.embedder
+            if validated_data.embedder_model
+            else None
+        )
 
     def search(
         self,
         query_text: str,
         query_vector: Optional[list[float]] = None,
         top_k: int = 5,
-    ) -> list[Record]:
+    ) -> list[neo4j.Record]:
         """Get the top_k nearest neighbor embeddings for either provided query_vector or query_text.
         Both query_vector and query_text can be provided.
         If query_vector is provided, then it will be preferred over the embedded query_text
         for the vector search.
         See the following documentation for more details:
         - [Query a vector index](https://neo4j.com/docs/cypher-manual/current/indexes-for-vector-search/#indexes-vector-query)
         - [db.index.vector.queryNodes()](https://neo4j.com/docs/operations-manual/5/reference/procedures/#procedure_db_index_vector_queryNodes)
@@ -56,15 +84,15 @@
             query_text (str): The text to get the closest neighbors of.
             query_vector (Optional[list[float]], optional): The vector embeddings to get the closest neighbors of. Defaults to None.
             top_k (int, optional): The number of neighbors to return. Defaults to 5.
         Raises:
             ValueError: If validation of the input arguments fail.
             ValueError: If no embedder is provided.
         Returns:
-            list[Record]: The results of the search query
+            list[neo4j.Record]: The results of the search query
         """
         try:
             validated_data = HybridSearchModel(
                 vector_index_name=self.vector_index_name,
                 fulltext_index_name=self.fulltext_index_name,
                 top_k=top_k,
                 query_vector=query_vector,
@@ -77,42 +105,62 @@
 
         if query_text and not query_vector:
             if not self.embedder:
                 raise ValueError("Embedding method required for text query.")
             query_vector = self.embedder.embed_query(query_text)
             parameters["query_vector"] = query_vector
 
-        search_query = get_search_query(SearchType.HYBRID, self.return_properties)
+        search_query, _ = get_search_query(SearchType.HYBRID, self.return_properties)
+
+        logger.debug("HybridRetriever Cypher parameters: %s", parameters)
+        logger.debug("HybridRetriever Cypher query: %s", search_query)
 
         records, _, _ = self.driver.execute_query(search_query, parameters)
         return records
 
 
 class HybridCypherRetriever(Retriever):
     def __init__(
         self,
-        driver: Driver,
+        driver: neo4j.Driver,
         vector_index_name: str,
         fulltext_index_name: str,
         retrieval_query: str,
         embedder: Optional[Embedder] = None,
     ) -> None:
-        super().__init__(driver)
-        self.vector_index_name = vector_index_name
-        self.fulltext_index_name = fulltext_index_name
-        self.retrieval_query = retrieval_query
-        self.embedder = embedder
+        try:
+            driver_model = Neo4jDriverModel(driver=driver)
+            embedder_model = EmbedderModel(embedder=embedder) if embedder else None
+            validated_data = HybridCypherRetrieverModel(
+                driver_model=driver_model,
+                vector_index_name=vector_index_name,
+                fulltext_index_name=fulltext_index_name,
+                retrieval_query=retrieval_query,
+                embedder_model=embedder_model,
+            )
+        except ValidationError as e:
+            raise ValueError(f"Validation failed: {e.errors()}")
+
+        super().__init__(validated_data.driver_model.driver)
+        self.vector_index_name = validated_data.vector_index_name
+        self.fulltext_index_name = validated_data.fulltext_index_name
+        self.retrieval_query = validated_data.retrieval_query
+        self.embedder = (
+            validated_data.embedder_model.embedder
+            if validated_data.embedder_model
+            else None
+        )
 
     def search(
         self,
         query_text: str,
         query_vector: Optional[list[float]] = None,
         top_k: int = 5,
         query_params: Optional[dict[str, Any]] = None,
-    ) -> list[Record]:
+    ) -> list[neo4j.Record]:
         """Get the top_k nearest neighbor embeddings for either provided query_vector or query_text.
         Both query_vector and query_text can be provided.
         If query_vector is provided, then it will be preferred over the embedded query_text
         for the vector search.
         See the following documentation for more details:
         - [Query a vector index](https://neo4j.com/docs/cypher-manual/current/indexes-for-vector-search/#indexes-vector-query)
         - [db.index.vector.queryNodes()](https://neo4j.com/docs/operations-manual/5/reference/procedures/#procedure_db_index_vector_queryNodes)
@@ -122,15 +170,15 @@
             query_vector (Optional[list[float]], optional): The vector embeddings to get the closest neighbors of. Defaults to None.
             top_k (int, optional): The number of neighbors to return. Defaults to 5.
             query_params (Optional[dict[str, Any]], optional): Parameters for the Cypher query. Defaults to None.
         Raises:
             ValueError: If validation of the input arguments fail.
             ValueError: If no embedder is provided.
         Returns:
-            list[Record]: The results of the search query
+            list[neo4j.Record]: The results of the search query
         """
         try:
             validated_data = HybridCypherSearchModel(
                 vector_index_name=self.vector_index_name,
                 fulltext_index_name=self.fulltext_index_name,
                 top_k=top_k,
                 query_vector=query_vector,
@@ -150,12 +198,16 @@
 
         if query_params:
             for key, value in query_params.items():
                 if key not in parameters:
                     parameters[key] = value
             del parameters["query_params"]
 
-        search_query = get_search_query(
+        search_query, _ = get_search_query(
             SearchType.HYBRID, retrieval_query=self.retrieval_query
         )
+
+        logger.debug("HybridCypherRetriever Cypher parameters: %s", parameters)
+        logger.debug("HybridCypherRetriever Cypher query: %s", search_query)
+
         records, _, _ = self.driver.execute_query(search_query, parameters)
         return records
```

### Comparing `neo4j_genai-0.1.4/src/neo4j_genai/retrievers/vector.py` & `neo4j_genai-0.2.0a1/src/neo4j_genai/retrievers/external/weaviate/weaviate.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,175 +8,140 @@
 #      https://www.apache.org/licenses/LICENSE-2.0
 #  #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
-from typing import Optional, Any
-
-from neo4j import Driver, Record
-from neo4j_genai.retrievers.base import Retriever
-from pydantic import ValidationError
 
+from typing import Optional
+from neo4j_genai.retrievers.base import ExternalRetriever
 from neo4j_genai.embedder import Embedder
-from neo4j_genai.types import (
-    VectorSearchRecord,
-    VectorSearchModel,
-    VectorCypherSearchModel,
-    SearchType,
-)
-from neo4j_genai.neo4j_queries import get_search_query
+from neo4j_genai.retrievers.utils import validate_search_query_input
+import weaviate.classes as wvc
+from weaviate.client import WeaviateClient
+from weaviate.collections.classes.filters import _Filters
+import neo4j
+import logging
+from neo4j_genai.neo4j_queries import get_query_tail
 
+logger = logging.getLogger(__name__)
 
-class VectorRetriever(Retriever):
-    """
-    Provides retrieval method using vector search over embeddings.
-    If an embedder is provided, it needs to have the required Embedder type.
-    """
 
+class WeaviateNeo4jRetriever(ExternalRetriever):
     def __init__(
         self,
-        driver: Driver,
-        index_name: str,
+        driver: neo4j.Driver,
+        client: WeaviateClient,
+        collection: str,
+        id_property_external: str,
+        id_property_neo4j: str,
         embedder: Optional[Embedder] = None,
         return_properties: Optional[list[str]] = None,
-    ) -> None:
-        super().__init__(driver)
-        self.index_name = index_name
-        self.return_properties = return_properties
+        retrieval_query: Optional[str] = None,
+    ):
+        super().__init__(id_property_external, id_property_neo4j)
+        self.driver = driver
+        self.client = client
+        self.search_collection = client.collections.get(collection)
         self.embedder = embedder
+        self.return_properties = return_properties
+        self.retrieval_query = retrieval_query
 
     def search(
         self,
         query_vector: Optional[list[float]] = None,
         query_text: Optional[str] = None,
         top_k: int = 5,
-    ) -> list[VectorSearchRecord]:
-        """Get the top_k nearest neighbor embeddings for either provided query_vector or query_text.
-        See the following documentation for more details:
+        weaviate_filters: Optional[_Filters] = None,
+    ) -> list[neo4j.Record]:
+        """Get the top_k nearest neighbor embeddings using Weaviate for either provided query_vector or query_text.
+        Both query_vector and query_text can be provided.
+        If query_vector is provided, then it will be preferred over the embedded query_text
+        for the vector search.
+        If query_text is provided, then it will check if an embedder is provided and use it to generate the query_vector.
+        If no embedder is provided, then it will assume that the vectorizer is used in Weaviate.
 
+        See the following documentation for more details:
         - [Query a vector index](https://neo4j.com/docs/cypher-manual/current/indexes-for-vector-search/#indexes-vector-query)
         - [db.index.vector.queryNodes()](https://neo4j.com/docs/operations-manual/5/reference/procedures/#procedure_db_index_vector_queryNodes)
-
+        - [db.index.fulltext.queryNodes()](https://neo4j.com/docs/operations-manual/5/reference/procedures/#procedure_db_index_fulltext_querynodes)
         Args:
+            query_text (str): The text to get the closest neighbors of.
             query_vector (Optional[list[float]], optional): The vector embeddings to get the closest neighbors of. Defaults to None.
-            query_text (Optional[str], optional): The text to get the closest neighbors of. Defaults to None.
             top_k (int, optional): The number of neighbors to return. Defaults to 5.
-
+            weaviate_filters (Optional[_Filters], optional): The filters to apply to the search query in Weaviate. Defaults to None.
         Raises:
             ValueError: If validation of the input arguments fail.
-            ValueError: If no embedder is provided.
-
         Returns:
-            list[VectorSearchRecord]: The `top_k` neighbors found in vector search with their nodes and scores.
+            list[neo4j.Record]: The results of the search query
         """
-        try:
-            validated_data = VectorSearchModel(
-                index_name=self.index_name,
-                top_k=top_k,
-                query_vector=query_vector,
-                query_text=query_text,
-            )
-        except ValidationError as e:
-            error_details = e.errors()
-            raise ValueError(f"Validation failed: {error_details}")
 
-        parameters = validated_data.model_dump(exclude_none=True)
+        validate_search_query_input(query_text=query_text, query_vector=query_vector)
 
+        # If we want to use a local embedder, we still want to call the near_vector method
+        # so we want to create the vector as early as possible here
         if query_text:
-            if not self.embedder:
-                raise ValueError("Embedding method required for text query.")
-            query_vector = self.embedder.embed_query(query_text)
-            parameters["query_vector"] = query_vector
-            del parameters["query_text"]
-
-        search_query = get_search_query(SearchType.VECTOR, self.return_properties)
-
-        records, _, _ = self.driver.execute_query(search_query, parameters)
-
-        try:
-            return [
-                VectorSearchRecord(node=record["node"], score=record["score"])
-                for record in records
-            ]
-        except ValidationError as e:
-            error_details = e.errors()
-            raise ValueError(
-                f"Validation failed while constructing output: {error_details}"
+            if self.embedder:
+                query_vector = self.embedder.embed_query(query_text)
+                logger.debug("Locally generated query vector: %s", query_vector)
+            else:
+                logger.debug(
+                    "No embedder provided, assuming vectorizer is used in Weaviate."
+                )
+
+        if query_vector:
+            response = self.search_collection.query.near_vector(
+                near_vector=query_vector,
+                limit=top_k,
+                filters=weaviate_filters,
+                return_metadata=wvc.query.MetadataQuery(certainty=True),
             )
+            logger.debug("Weaviate query vector: %s", query_vector)
+            logger.debug("Response: %s", response)
+        else:
+            response = self.search_collection.query.near_text(
+                query=query_text,
+                limit=top_k,
+                filters=weaviate_filters,
+                return_metadata=wvc.query.MetadataQuery(certainty=True),
+            )
+            logger.debug("Query text: %s", query_text)
+            logger.debug("Response: %s", response)
 
+        result_tuples = [
+            [f"{o.properties[self.id_property_external]}", o.metadata.certainty or 0.0]
+            for o in response.objects
+        ]
+
+        search_query = get_match_query(
+            return_properties=self.return_properties,
+            retrieval_query=self.retrieval_query,
+        )
 
-class VectorCypherRetriever(Retriever):
-    """
-    Provides retrieval method using vector similarity and custom Cypher query.
-    If an embedder is provided, it needs to have the required Embedder type.
-    """
-
-    def __init__(
-        self,
-        driver: Driver,
-        index_name: str,
-        retrieval_query: str,
-        embedder: Optional[Embedder] = None,
-    ) -> None:
-        super().__init__(driver)
-        self.index_name = index_name
-        self.retrieval_query = retrieval_query
-        self.embedder = embedder
-
-    def search(
-        self,
-        query_vector: Optional[list[float]] = None,
-        query_text: Optional[str] = None,
-        top_k: int = 5,
-        query_params: Optional[dict[str, Any]] = None,
-    ) -> list[Record]:
-        """Get the top_k nearest neighbor embeddings for either provided query_vector or query_text.
-        See the following documentation for more details:
-
-        - [Query a vector index](https://neo4j.com/docs/cypher-manual/current/indexes-for-vector-search/#indexes-vector-query)
-        - [db.index.vector.queryNodes()](https://neo4j.com/docs/operations-manual/5/reference/procedures/#procedure_db_index_vector_queryNodes)
-
-        Args:
-            query_vector (Optional[list[float]], optional): The vector embeddings to get the closest neighbors of. Defaults to None.
-            query_text (Optional[str], optional): The text to get the closest neighbors of. Defaults to None.
-            top_k (int, optional): The number of neighbors to return. Defaults to 5.
-            query_params (Optional[dict[str, Any]], optional): Parameters for the Cypher query. Defaults to None.
+        parameters = {
+            "match_params": result_tuples,
+            "id_property": self.id_property_neo4j,
+        }
 
-        Raises:
-            ValueError: If validation of the input arguments fail.
-            ValueError: If no embedder is provided.
+        logger.debug("Weaviate Store Cypher parameters: %s", parameters)
+        logger.debug("Weaviate Store Cypher query: %s", search_query)
 
-        Returns:
-            list[Record]: The results of the search query
-        """
-        try:
-            validated_data = VectorCypherSearchModel(
-                index_name=self.index_name,
-                top_k=top_k,
-                query_vector=query_vector,
-                query_text=query_text,
-                query_params=query_params,
-            )
-        except ValidationError as e:
-            raise ValueError(f"Validation failed: {e.errors()}")
+        records, _, _ = self.driver.execute_query(search_query, parameters)
 
-        parameters = validated_data.model_dump(exclude_none=True)
+        return records
 
-        if query_text:
-            if not self.embedder:
-                raise ValueError("Embedding method required for text query.")
-            parameters["query_vector"] = self.embedder.embed_query(query_text)
-            del parameters["query_text"]
-
-        if query_params:
-            for key, value in query_params.items():
-                if key not in parameters:
-                    parameters[key] = value
-            del parameters["query_params"]
 
-        search_query = get_search_query(
-            SearchType.VECTOR, retrieval_query=self.retrieval_query
-        )
-        records, _, _ = self.driver.execute_query(search_query, parameters)
-        return records
+def get_match_query(
+    return_properties: Optional[str] = None, retrieval_query: Optional[str] = None
+):
+    match_query = (
+        "UNWIND $match_params AS match_param "
+        "WITH match_param[0] AS match_id_value, match_param[1] AS score "
+        "MATCH (node) "
+        "WHERE node[$id_property] = match_id_value "
+    )
+    return match_query + get_query_tail(
+        return_properties=return_properties,
+        retrieval_query=retrieval_query,
+        fallback_return="RETURN node, score",
+    )
```

### Comparing `neo4j_genai-0.1.4/PKG-INFO` & `neo4j_genai-0.2.0a1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: neo4j-genai
-Version: 0.1.4
+Version: 0.2.0a1
 Summary: Python package to allow easy integration to Neo4j's GenAI features
 License: Apache License, Version 2.0
 Author: Neo4j, Inc
 Author-email: team-gen-ai@neo4j.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Provides-Extra: external-clients
 Requires-Dist: neo4j (>=5.17.0,<6.0.0)
 Requires-Dist: pydantic (>=2.6.3,<3.0.0)
 Requires-Dist: types-requests (>=2.31.0.20240218,<3.0.0.0)
+Requires-Dist: weaviate-client (>=4.6.1,<5.0.0) ; extra == "external-clients"
 Description-Content-Type: text/markdown
 
 # Neo4j GenAI package for Python
 
 This repository contains the official Neo4j GenAI features for Python.
 
 The purpose of this package is to provide a first party package to developers,
@@ -176,19 +178,42 @@
     [suggested changes](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/incorporating-feedback-in-your-pull-request)
     or normal pull request comments. You can apply suggested changes directly through
     the UI, and any other changes can be made in your fork and committed to the PR branch.
 -   As you update your PR and apply changes, mark each conversation as [resolved](https://docs.github.com/en/github/collaborating-with-issues-and-pull-requests/commenting-on-a-pull-request#resolving-conversations).
 
 ## Run tests
 
-Open a new virtual environment and then run the tests.
+### Unit tests
+
+This should run out of the box once the dependencies are installed.
+
+```bash
+poetry run pytest tests/unit
+```
+
+### E2E tests
+
+To run e2e tests you'd need to have some services running locally:
+
+-   neo4j
+-   weaviate
+-   weaviate-text2vec-transformers
+
+The easiest way to get it up and running is via Docker compose:
+
+```bash
+docker compose -f tests/e2e/docker-compose.yml up
+```
+
+_(pro tip: if you suspect something in the databases are cached, run `docker compose -f tests/e2e/docker-compose.yml down` to remove them completely)_
+
+Once the services are running, execute the following command to run the e2e tests.
 
 ```bash
-poetry shell
-pytest tests/unit
+poetry run pytest tests/e2e
 ```
 
 ## Further information
 
 -   [The official Neo4j Python driver](https://github.com/neo4j/neo4j-python-driver)
 -   [Neo4j GenAI integrations](https://neo4j.com/docs/cypher-manual/current/genai-integrations/)
```

