# Comparing `tmp/dongraphio-0.3.5.tar.gz` & `tmp/dongraphio-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dongraphio-0.3.5.tar", max compression
+gzip compressed data, was "dongraphio-0.3.6.tar", max compression
```

## Comparing `dongraphio-0.3.5.tar` & `dongraphio-0.3.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0     1400 2024-05-19 14:37:01.616400 dongraphio-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     1384 2024-05-19 12:41:43.471387 dongraphio-0.3.5/README.md
--rw-r--r--   0        0        0      245 2024-05-19 14:37:01.619181 dongraphio-0.3.5/src/dongraphio/__init__.py
--rw-r--r--   0        0        0      133 2024-05-19 12:41:43.473390 dongraphio-0.3.5/src/dongraphio/base_models/__init__.py
--rw-r--r--   0        0        0    14979 2024-05-19 12:41:43.473390 dongraphio-0.3.5/src/dongraphio/base_models/grapher_logic.py
--rw-r--r--   0        0        0     4911 2024-05-19 14:07:12.233343 dongraphio-0.3.5/src/dongraphio/base_models/isochrones_logic.py
--rw-r--r--   0        0        0     2692 2024-05-19 14:23:12.859861 dongraphio-0.3.5/src/dongraphio/base_models/matrix_logic.py
--rw-r--r--   0        0        0     6194 2024-05-19 12:42:22.439889 dongraphio-0.3.5/src/dongraphio/dongraphio.py
--rw-r--r--   0        0        0     1056 2024-05-19 12:41:43.431091 dongraphio-0.3.5/src/dongraphio/enums.py
--rw-r--r--   0        0        0      523 2024-05-19 12:43:26.743296 dongraphio-0.3.5/src/dongraphio/utils/__init__.py
--rw-r--r--   0        0        0     1262 2024-05-19 12:41:43.475388 dongraphio-0.3.5/src/dongraphio/utils/geometry_utils.py
--rw-r--r--   0        0        0    19283 2024-05-19 12:41:43.476388 dongraphio-0.3.5/src/dongraphio/utils/graph_utils.py
--rw-r--r--   0        0        0     2602 2024-05-19 14:21:22.958792 dongraphio-0.3.5/src/dongraphio/utils/matrix_utils.py
--rw-r--r--   0        0        0     1713 2024-05-19 12:41:43.477391 dongraphio-0.3.5/src/dongraphio/utils/osm_worker.py
--rw-r--r--   0        0        0     1647 2024-03-31 14:31:51.764945 dongraphio-0.3.5/src/dongraphio/utils/tsp_solver.py
--rw-r--r--   0        0        0     2354 1970-01-01 00:00:00.000000 dongraphio-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1498 2024-05-22 18:54:48.578560 dongraphio-0.3.6/LICENSE.txt
+-rw-r--r--   0        0        0     1424 2024-05-22 18:59:54.009037 dongraphio-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     1461 2024-05-22 18:54:48.568815 dongraphio-0.3.6/README.md
+-rw-r--r--   0        0        0      211 2024-05-22 18:57:11.704747 dongraphio-0.3.6/src/dongraphio/__init__.py
+-rw-r--r--   0        0        0      133 2024-05-22 18:54:42.344284 dongraphio-0.3.6/src/dongraphio/base_models/__init__.py
+-rw-r--r--   0        0        0    14906 2024-05-22 18:54:42.351343 dongraphio-0.3.6/src/dongraphio/base_models/grapher_logic.py
+-rw-r--r--   0        0        0     5390 2024-05-22 19:01:15.437477 dongraphio-0.3.6/src/dongraphio/base_models/isochrones_logic.py
+-rw-r--r--   0        0        0     2750 2024-05-22 18:54:42.347119 dongraphio-0.3.6/src/dongraphio/base_models/matrix_logic.py
+-rw-r--r--   0        0        0     5628 2024-05-22 18:54:42.363628 dongraphio-0.3.6/src/dongraphio/dongraphio.py
+-rw-r--r--   0        0        0     1056 2024-05-22 18:54:42.337542 dongraphio-0.3.6/src/dongraphio/enums.py
+-rw-r--r--   0        0        0      466 2024-05-22 18:57:11.710084 dongraphio-0.3.6/src/dongraphio/utils/__init__.py
+-rw-r--r--   0        0        0     1262 2024-05-22 18:54:42.333656 dongraphio-0.3.6/src/dongraphio/utils/geometry_utils.py
+-rw-r--r--   0        0        0    19283 2024-05-22 18:54:42.325919 dongraphio-0.3.6/src/dongraphio/utils/graph_utils.py
+-rw-r--r--   0        0        0     2606 2024-05-22 18:54:42.327912 dongraphio-0.3.6/src/dongraphio/utils/matrix_utils.py
+-rw-r--r--   0        0        0     1713 2024-05-22 18:54:42.322735 dongraphio-0.3.6/src/dongraphio/utils/osm_worker.py
+-rw-r--r--   0        0        0     1738 2024-05-22 18:54:42.324415 dongraphio-0.3.6/src/dongraphio/utils/tsp_solver.py
+-rw-r--r--   0        0        0     2504 1970-01-01 00:00:00.000000 dongraphio-0.3.6/PKG-INFO
```

### Comparing `dongraphio-0.3.5/pyproject.toml` & `dongraphio-0.3.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [tool.poetry]
 name = "dongraphio"
-version = "0.3.5"
+version = "0.3.6"
+license = "BSD-3-Clause"
 description = "Small utility library containing graph algorighms used in other projects"
 authors = ["Danila <63115678+DDonnyy@users.noreply.github.com>"]
 readme = "README.md"
 
 packages = [{ include = "dongraphio", from = "src" }]
 
 [tool.poetry.dependencies]
@@ -17,15 +18,14 @@
 momepy = "^0.6.0"
 networkit = "^11.0"
 numpy = "^1.23.5"
 pandas = "^2.2.0"
 networkx = "^3.2.1"
 loguru = "^0.7.2"
 
-
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 pylint = "^3.0.3"
 isort = "^5.13.2"
 jupyter = "^1.0.0"
 ortools = "^9.9.3963"
```

### Comparing `dongraphio-0.3.5/README.md` & `dongraphio-0.3.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 ## Base usage example
 ```pip install dongraphio```
 ```python
 import geopandas as gpd
 from dongraphio import DonGraphio
 from dongraphio import GraphType
 import networkx as nx
+from shapely import Point
 
 dongrph = DonGraphio(city_crs=32638)
     
 intermodal_graph = dongrph.get_intermodal_graph_from_osm(city_osm_id=3955288)
 nx.write_graphml(intermodal_graph,"city_intermodal.graphml")
 
 builds_from = gpd.read_file("test_data/buildings.geojson")
 services_to = gpd.read_file("test_data/services.geojson")
-adjacency_matrix = dongrph.get_adjacency_matrix(gdf_from=builds_from, gdf_to=services_to, weight="time_min")
+adjacency_matrix = dongrph.get_adjacency_matrix(gdf_from=builds_from, gdf_to=services_to, weight="time_min",graph_type=[GraphType.PUBLIC_TRANSPORT, GraphType.WALK])
 adjacency_matrix.to_csv("city_adjacency_matrix.csv")
 
 accessibility_isochrones, public_transport_routes, public_transport_stops = dongrph.get_accessibility_isochrones(
     graph_type=[GraphType.PUBLIC_TRANSPORT, GraphType.WALK],
-    x_from=571747,
-    y_from=5709639,
+    points=Point(571747,5709639),
     weight_value=15,
     weight_type="time_min",
 )
 accessibility_isochrones.to_file("city_accessibility_isochrones.geojson")
 public_transport_routes.to_file("city_public_transport.geojson")
 public_transport_stops.to_file("city_public_stops.geojson")
 ```
```

### Comparing `dongraphio-0.3.5/src/dongraphio/base_models/grapher_logic.py` & `dongraphio-0.3.6/src/dongraphio/base_models/grapher_logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,21 +217,21 @@
         united_graph = self.join_graph(updated_G_base, G_to_project, points_df)
         return united_graph
 
     def get_public_trasport_graph(self) -> nx.MultiDiGraph:
         graph = nx.MultiDiGraph()
         edegs_different_types = []
         if not self.public_transport_speeds:
-            self.public_transport_speeds = {  # TODO add enum in future version
+            self.public_transport_speeds = {
                 "subway": 12 * 1000 / 60,
                 "tram": 15 * 1000 / 60,
                 "trolleybus": 12 * 1000 / 60,
                 "bus": 17 * 1000 / 60,
             }
-        from_file = False  # TODO REMAKE FILE MANAGEMENT SYSTEM
+        from_file = False
 
         # for transport in gdf_files.values():
         #     if transport.get("stops") or transport.get("routes"):
         #         from_file = True
 
         if not from_file:
             logger.warning(
```

### Comparing `dongraphio-0.3.5/src/dongraphio/base_models/isochrones_logic.py` & `dongraphio-0.3.6/src/dongraphio/base_models/isochrones_logic.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,98 +1,106 @@
 from typing import Literal, Optional, Tuple
 
 import geopandas as gpd
 import networkit as nk
 import networkx as nx
 import pandas as pd
-import shapely
 from loguru import logger
-from pydantic import BaseModel, InstanceOf
+from pydantic import BaseModel, InstanceOf, field_validator
+from shapely import Point, from_wkt
+from shapely.ops import unary_union
 from tqdm.auto import tqdm
 
 from ..enums import GraphType
 from ..utils import convert_multidigraph_to_digraph, get_nx2nk_idmap, matrix_utils, nx_to_gdf
 
 tqdm.pandas()
 
 
 class BuildsAvailabilitier(BaseModel):
     graph_type: list[GraphType]
     city_crs: int
-    x_from: float
-    y_from: float
+    points: InstanceOf[gpd.GeoSeries] | InstanceOf[Point]
     weight_value: int
     weight_type: Literal["time_min", "length_meter"]
     nx_intermodal_graph: InstanceOf[nx.DiGraph]
     _edge_types = None
 
+    @field_validator("points")
+    @classmethod
+    def ensure_points(cls, points):
+        if isinstance(points, gpd.GeoSeries):
+            assert points.apply(
+                lambda geom: isinstance(geom, Point)
+            ).all(), "Geometry type in provided points is not Point"
+        else:
+            points = gpd.GeoSeries([points])
+        return points
+
     def get_accessibility_isochrone(
         self,
     ) -> Tuple[gpd.GeoDataFrame, Optional[gpd.GeoDataFrame], Optional[gpd.GeoDataFrame]]:
 
-        source = gpd.GeoDataFrame(geometry=gpd.points_from_xy([self.x_from], [self.y_from], crs=self.city_crs))
-
         self._edge_types = [d.value for d in sum([t.edges for t in self.graph_type], [])]
 
         mobility_graph = matrix_utils.get_subgraph(self.nx_intermodal_graph, "type", self._edge_types)
         mobility_graph = nx.convert_node_labels_to_integers(mobility_graph)
 
         if mobility_graph.is_multigraph() & mobility_graph.is_directed():
             mobility_graph = convert_multidigraph_to_digraph(mobility_graph, self.weight_type)
         mobility_graph.graph["crs"] = self.city_crs
         graph_gdf = nx_to_gdf(nx.MultiDiGraph(mobility_graph), nodes=True)
 
-        from_sources = graph_gdf["geometry"].sindex.nearest(source["geometry"], return_distance=True, return_all=False)
+        from_sources = graph_gdf["geometry"].sindex.nearest(self.points, return_distance=True, return_all=False)
         source_index = from_sources[0][1]
         distances = pd.DataFrame(float(0), index=source_index, columns=list(mobility_graph.nodes()))
 
         logger.debug("Calculating distances from the specified point...")
 
         mapping = get_nx2nk_idmap(mobility_graph)
         nk_graph = nk.nxadapter.nx2nk(mobility_graph, self.weight_type)
         spsp = nk.distance.SPSP(G=nk_graph, sources=distances.index.values).run()
-        for index, row in distances.iterrows():
+        for index, _ in distances.iterrows():
             for column in distances.columns:
                 distances.loc[index, column] = spsp.getDistance(mapping.get(index), mapping.get(column))
         del spsp
 
         dist_nearest = pd.DataFrame(data=from_sources[1], index=from_sources[0][1], columns=["dist"])
         walk_speed = 4 * 1000 / 60
         dist_nearest = dist_nearest / walk_speed if self.weight_type == "time_min" else dist_nearest
         distances = distances.add(dist_nearest.dist, axis=0).transpose()
 
         distances = distances[distances[source_index[0]] <= self.weight_value]
-
+        results = []
+        point_num = 0
         logger.debug("Building isochrones geometry...")
-        distances["geometry"] = distances.apply(
-            lambda x: (
-                graph_gdf.loc[x.index].geometry.buffer(round(self.weight_value - x, 2) * walk_speed * 0.8)
-                if self.weight_type == "time_min"
-                else graph_gdf.loc[x.index].geometry.buffer(round(self.weight_value - x, 2) * 0.8)
-            )
-        )
-        isochrone_geometry = gpd.GeoDataFrame(data=distances, geometry="geometry").geometry.unary_union
-
-        isochrones = gpd.GeoDataFrame(
-            {
-                "travel_type": [str([d.russian_name for d in self.graph_type])],
-                "weight_type": [self.weight_type],
-                "weight_value": [self.weight_value],
-                "geometry": [isochrone_geometry],
-            },
-            geometry="geometry",
-            crs=self.city_crs,
-        )
+        for column_name in distances.columns:
+            geometry = []
+            for ind in distances.index:
+                value = distances.loc[ind, column_name]
+                geometry.append(
+                    graph_gdf.loc[ind].geometry.buffer(round(self.weight_value - value, 2) * walk_speed * 0.8)
+                    if self.weight_type == "time_min"
+                    else graph_gdf.loc[ind].geometry.buffer(round(self.weight_value - value, 2) * 0.8)
+                )
+            geometry = unary_union(geometry)
+            results.append({"geometry": geometry, "point": str(self.points.iloc[point_num])})
+            point_num += 1
+
+        isochrones = gpd.GeoDataFrame(data=results, geometry="geometry", crs=self.city_crs)
+        isochrones["travel_type"] = str([d.russian_name for d in self.graph_type])
+        isochrones["weight_type"] = self.weight_type
+        isochrones["weight_value"] = self.weight_value
 
         stops, routes = (None, None)
         if GraphType.PUBLIC_TRANSPORT in self.graph_type and self.weight_type == "time_min":
             if not (graph_gdf[graph_gdf["stop"] == "True"]).empty:
                 stops, routes = self._get_routes(graph_gdf, distances.index.values, mobility_graph)
             else:
-                logger.info('No public transport node in graph')
+                logger.info("No public transport node in graph")
         return isochrones, routes, stops
 
     def _get_routes(self, graph_gdf, selected_nodes, mobility_graph):
         stops = graph_gdf[graph_gdf["stop"] == "True"]
         stop_types = (
             stops["desc"]
             .astype(object)
@@ -101,11 +109,11 @@
             .fillna(False)
             .infer_objects(copy=False)
         )
         stops = stops.join(stop_types)
         selected_nodes = [node for node in selected_nodes if node in stops.index]
         subgraph = mobility_graph.subgraph(selected_nodes)
         routes = pd.DataFrame.from_records([e[-1] for e in subgraph.edges(data=True)])
-        routes['geometry'] = routes['geometry'].apply(shapely.from_wkt)
-        routes_result = gpd.GeoDataFrame(data=routes, geometry="geometry",crs=graph_gdf.crs)
-        stops_result = gpd.GeoDataFrame(data=stops.loc[selected_nodes], geometry="geometry",crs=graph_gdf.crs)
+        routes["geometry"] = routes["geometry"].apply(from_wkt)
+        routes_result = gpd.GeoDataFrame(data=routes, geometry="geometry", crs=graph_gdf.crs)
+        stops_result = gpd.GeoDataFrame(data=stops.loc[selected_nodes], geometry="geometry", crs=graph_gdf.crs)
         return stops_result, routes_result
```

### Comparing `dongraphio-0.3.5/src/dongraphio/base_models/matrix_logic.py` & `dongraphio-0.3.6/src/dongraphio/base_models/matrix_logic.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
             mobility_sub_graph = convert_multidigraph_to_digraph(mobility_sub_graph, self.weight)
 
         mobility_sub_graph.graph["crs"] = self.city_crs
 
         graph_gdf = nx_to_gdf(nx.MultiDiGraph(mobility_sub_graph), nodes=True)
 
         from_ = gpd.sjoin_nearest(self.gdf_from, graph_gdf)
-        from_ = from_.reset_index().drop_duplicates(subset="index", keep="first").set_index('index')
+        from_ = from_.reset_index().drop_duplicates(subset="index", keep="first").set_index("index")
 
         to_ = gpd.sjoin_nearest(self.gdf_to, graph_gdf)
         to_ = to_.reset_index().drop_duplicates(subset="index", keep="first").set_index("index")
 
         from_index = from_["index_right"]
         to_index = to_["index_right"]
         distance_matrix = pd.DataFrame(float(0), index=from_index, columns=to_index)
@@ -55,15 +55,19 @@
             mobility_sub_graph,
             from_index,
             to_index,
             weight=self.weight,
         )
 
         distance_matrix_result = distance_matrix_result.apply(pd.to_numeric, errors="coerce")
+
         def update_value(ind, col):
-            if ind in distance_matrix_result.index and col in distance_matrix_result.columns:
-                return distance_matrix_result.loc[ind, col]
+            return (
+                distance_matrix_result.loc[ind, col]
+                if ind in distance_matrix_result.index and col in distance_matrix_result.columns
+                else None
+            )
 
         distance_matrix = distance_matrix.apply(lambda x: x.index.map(lambda ind: update_value(ind, x.name)))
         distance_matrix.index = self.gdf_from.index
         distance_matrix.columns = self.gdf_to.index
         return distance_matrix
```

### Comparing `dongraphio-0.3.5/src/dongraphio/dongraphio.py` & `dongraphio-0.3.6/src/dongraphio/dongraphio.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,26 @@
 from typing import Optional, Tuple
 
 import geopandas as gpd
 import networkx as nx
 import pandas as pd
+import shapely
 from loguru import logger
 
 from .base_models import BuildsAvailabilitier, BuildsGrapher, BuildsMatrixer
 from .enums import GraphType
 
 
 class DonGraphio:
     def __init__(self, city_crs: int, intermodal_graph: nx.MultiDiGraph | None = None):
         self.city_crs = city_crs
-        # self.graphs: dict[GraphType, nx.Graph] = {} # TODO: add graphs to Invoker
+        # self.graphs: dict[GraphType, nx.Graph] = {}
 
         self._intermodal_graph = intermodal_graph
 
-    # TODO: replace non-alternative OSM integration with optional graphs build from OSM
-    # def try_build_graph_from_osm(self, graph_type: GraphType, osm_id: int) -> nx.Graph:
-    #     """Build a graph from OSM data and save it as the given graph type"""
-    #     raise NotImplementedError()
-
     def get_graph(self) -> Optional[nx.DiGraph]:
         """
         Return the intermodal graph.
 
         Returns:
             Optional[nx.DiGraph]: The intermodal graph if it exists, else None.
         Raises:
@@ -41,16 +37,14 @@
         Args:
             graph (nx.DiGraph): The graph to be set.
         Returns:
             None
         """
         self._intermodal_graph = graph
 
-    # TODO: update BuildsGrapher logic to construct from the graphs, fail if not all graphs are available
-
     def get_intermodal_graph_from_osm(self, city_osm_id: int, keep_city_boundary: bool = True) -> nx.MultiDiGraph:
         """
         Retrieves the intermodal graph for a given city from OpenStreetMap.
         Args:
             city_osm_id (int): The OpenStreetMap ID of the city.
             keep_city_boundary (bool, optional): Whether to keep the city boundary in the graph. Defaults to True.
         Returns:
@@ -96,24 +90,23 @@
             nx_intermodal_graph=self._intermodal_graph,
             graph_type=graph_type,
         ).get_adjacency_matrix()
         logger.info("Adjacency matrix done!")
         return to_return
 
     def get_accessibility_isochrones(
-        self, graph_type: list[GraphType], x_from: float, y_from: float, weight_value: int, weight_type: str
+        self, graph_type: list[GraphType], points: gpd.GeoSeries | shapely.Point, weight_value: int, weight_type: str
     ) -> Tuple[gpd.GeoDataFrame, Optional[gpd.GeoDataFrame], Optional[gpd.GeoDataFrame]]:
         """
         Get accessibility isochrones and return three GeoDataFrame objects with isochrones, and
         if graph_type contains GraphType.PUBLIC_TRANSPORT enum - routes and public transport stops.
 
         Args:
             graph_type (list[GraphType]): The List of Enum types of the graph to build isochrones.
-            x_from (float): The x-coordinate of the starting point in the corresponding coordinate system.
-            y_from (float): The y-coordinate of the starting point in the corresponding coordinate system.
+            points (gpd.GeoSeries | shapely.Point): The GeoSeries containing points.
             weight_value (int): The value of the weight.
             weight_type (str): The type of the weight, could be only "time_min" or "length_meter" .
 
         Returns:
             (gpd.GeoDataFrame, Optional[gpd.GeoDataFrame], Optional[gpd.GeoDataFrame]): Isochrones,routes,stops.
         Raises:
             RuntimeError: If no graph has been set, call get_intermodal_graph_from_osm() or set it by set_graph().
@@ -122,15 +115,14 @@
         if self._intermodal_graph is None:
             raise RuntimeError("No graph has set, call get_intermodal_graph_from_osm() or set it by set_graph()")
         # Build accessibility isochrones
         logger.info("Creating accessibility isochrones based on provided graph and point...")
         to_return = BuildsAvailabilitier(
             graph_type=graph_type,
             city_crs=self.city_crs,
-            x_from=x_from,
-            y_from=y_from,
+            points=points,
             weight_value=weight_value,
             weight_type=weight_type,
             nx_intermodal_graph=self._intermodal_graph,
         ).get_accessibility_isochrone()
         logger.info("Accessibility isochrones done!\n")
         return to_return
```

### Comparing `dongraphio-0.3.5/src/dongraphio/enums.py` & `dongraphio-0.3.6/src/dongraphio/enums.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.5/src/dongraphio/utils/geometry_utils.py` & `dongraphio-0.3.6/src/dongraphio/utils/geometry_utils.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.5/src/dongraphio/utils/graph_utils.py` & `dongraphio-0.3.6/src/dongraphio/utils/graph_utils.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.5/src/dongraphio/utils/matrix_utils.py` & `dongraphio-0.3.6/src/dongraphio/utils/matrix_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,9 +55,9 @@
     distance_matrix, route_matrix = get_dist_matrix(graph, route_nodes_ind, route_nodes_ind, True)
     mean_value = distance_matrix.values.mean()
     for i in route_nodes:
         node_1, n1_1, n2_1 = i
         for j in route_nodes:
             node_2, n1_2, n2_2 = j
             if (n1_1, n2_1) == (n2_2, n1_2):
-                distance_matrix.loc[node_1, node_2] = (mean_value+distance_matrix.loc[node_1, node_2])/3
+                distance_matrix.loc[node_1, node_2] = (mean_value + distance_matrix.loc[node_1, node_2]) / 3
     return distance_matrix, route_matrix
```

### Comparing `dongraphio-0.3.5/src/dongraphio/utils/osm_worker.py` & `dongraphio-0.3.6/src/dongraphio/utils/osm_worker.py`

 * *Files identical despite different names*

### Comparing `dongraphio-0.3.5/src/dongraphio/utils/tsp_solver.py` & `dongraphio-0.3.6/src/dongraphio/utils/tsp_solver.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,16 +23,21 @@
 
     routing = pywrapcp.RoutingModel(manager)
 
     transit_callback_index = routing.RegisterTransitCallback(distance_callback)
     routing.SetArcCostEvaluatorOfAllVehicles(transit_callback_index)
 
     search_parameters = pywrapcp.DefaultRoutingSearchParameters()
-    search_parameters.first_solution_strategy = routing_enums_pb2.FirstSolutionStrategy.PATH_CHEAPEST_ARC
-    search_parameters.local_search_metaheuristic = routing_enums_pb2.LocalSearchMetaheuristic.GUIDED_LOCAL_SEARCH
+
+    search_parameters.first_solution_strategy = (
+        routing_enums_pb2.FirstSolutionStrategy.PATH_CHEAPEST_ARC  # pylint: disable=no-member
+    )
+    search_parameters.local_search_metaheuristic = (
+        routing_enums_pb2.LocalSearchMetaheuristic.GUIDED_LOCAL_SEARCH  # pylint: disable=no-member
+    )
 
     search_parameters.time_limit.seconds = time_limit
 
     solution = routing.SolveWithParameters(search_parameters)
 
     result = get_solution(manager, routing, solution)
     mapping = dict(zip(range(distance_matrix.shape[0]), distance_matrix.index))
```

### Comparing `dongraphio-0.3.5/PKG-INFO` & `dongraphio-0.3.6/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: dongraphio
-Version: 0.3.5
+Version: 0.3.6
 Summary: Small utility library containing graph algorighms used in other projects
+License: BSD-3-Clause
 Author: Danila
 Author-email: 63115678+DDonnyy@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: geopandas (>=0.14.3,<0.15.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
@@ -30,29 +32,29 @@
 ## Base usage example
 ```pip install dongraphio```
 ```python
 import geopandas as gpd
 from dongraphio import DonGraphio
 from dongraphio import GraphType
 import networkx as nx
+from shapely import Point
 
 dongrph = DonGraphio(city_crs=32638)
     
 intermodal_graph = dongrph.get_intermodal_graph_from_osm(city_osm_id=3955288)
 nx.write_graphml(intermodal_graph,"city_intermodal.graphml")
 
 builds_from = gpd.read_file("test_data/buildings.geojson")
 services_to = gpd.read_file("test_data/services.geojson")
-adjacency_matrix = dongrph.get_adjacency_matrix(gdf_from=builds_from, gdf_to=services_to, weight="time_min")
+adjacency_matrix = dongrph.get_adjacency_matrix(gdf_from=builds_from, gdf_to=services_to, weight="time_min",graph_type=[GraphType.PUBLIC_TRANSPORT, GraphType.WALK])
 adjacency_matrix.to_csv("city_adjacency_matrix.csv")
 
 accessibility_isochrones, public_transport_routes, public_transport_stops = dongrph.get_accessibility_isochrones(
     graph_type=[GraphType.PUBLIC_TRANSPORT, GraphType.WALK],
-    x_from=571747,
-    y_from=5709639,
+    points=Point(571747,5709639),
     weight_value=15,
     weight_type="time_min",
 )
 accessibility_isochrones.to_file("city_accessibility_isochrones.geojson")
 public_transport_routes.to_file("city_public_transport.geojson")
 public_transport_stops.to_file("city_public_stops.geojson")
 ```
```

