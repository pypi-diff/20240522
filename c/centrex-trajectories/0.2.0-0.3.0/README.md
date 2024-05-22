# Comparing `tmp/centrex-trajectories-0.2.0.tar.gz` & `tmp/centrex-trajectories-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "centrex-trajectories-0.2.0.tar", max compression
+gzip compressed data, was "centrex-trajectories-0.3.0.tar", max compression
```

## Comparing `centrex-trajectories-0.2.0.tar` & `centrex-trajectories-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      976 2024-04-04 16:37:01.257546 centrex-trajectories-0.2.0/centrex_trajectories/__init__.py
--rw-r--r--   0        0        0    25522 2024-04-04 16:37:01.262546 centrex-trajectories-0.2.0/centrex_trajectories/beamline_objects.py
--rw-r--r--   0        0        0      159 2024-04-04 16:37:01.262546 centrex-trajectories-0.2.0/centrex_trajectories/common_types.py
--rw-r--r--   0        0        0    19206 2024-04-04 16:37:01.267547 centrex-trajectories-0.2.0/centrex_trajectories/data_structures.py
--rw-r--r--   0        0        0      461 2024-02-05 02:37:13.221609 centrex-trajectories-0.2.0/centrex_trajectories/particles.py
--rw-r--r--   0        0        0    13965 2024-04-04 16:37:01.271548 centrex-trajectories-0.2.0/centrex_trajectories/propagation.py
--rw-r--r--   0        0        0     8066 2024-04-04 16:37:01.276547 centrex-trajectories-0.2.0/centrex_trajectories/propagation_ballistic.py
--rw-r--r--   0        0        0     5216 2024-04-04 16:37:01.280547 centrex-trajectories-0.2.0/centrex_trajectories/propagation_ode.py
--rw-r--r--   0        0        0      697 2024-02-05 02:37:13.230610 centrex-trajectories-0.2.0/centrex_trajectories/propagation_options.py
--rw-r--r--   0        0        0        0 2023-01-22 08:03:57.373693 centrex-trajectories-0.2.0/centrex_trajectories/py.typed
--rw-r--r--   0        0        0     3483 2023-01-22 21:19:08.413341 centrex-trajectories-0.2.0/centrex_trajectories/random_generation.py
--rw-r--r--   0        0        0      243 2024-04-04 16:37:01.288551 centrex-trajectories-0.2.0/centrex_trajectories/saved_data/stark_poly.pkl
--rw-r--r--   0        0        0      902 2024-04-04 16:37:01.289553 centrex-trajectories-0.2.0/centrex_trajectories/utils.py
--rw-r--r--   0        0        0     2009 2024-02-05 02:37:13.238609 centrex-trajectories-0.2.0/centrex_trajectories/visualization.py
--rw-r--r--   0        0        0     1086 2022-05-19 04:30:48.923066 centrex-trajectories-0.2.0/LICENSE
--rw-r--r--   0        0        0      735 2024-04-04 16:37:59.543350 centrex-trajectories-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     4180 2024-04-04 16:44:35.129831 centrex-trajectories-0.2.0/README.md
--rw-r--r--   0        0        0     4907 1970-01-01 00:00:00.000000 centrex-trajectories-0.2.0/setup.py
--rw-r--r--   0        0        0     4525 1970-01-01 00:00:00.000000 centrex-trajectories-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      976 2024-04-04 16:37:01.257546 centrex-trajectories-0.3.0/centrex_trajectories/__init__.py
+-rw-r--r--   0        0        0    26462 2024-05-21 23:47:17.678009 centrex-trajectories-0.3.0/centrex_trajectories/beamline_objects.py
+-rw-r--r--   0        0        0      159 2024-04-04 16:37:01.262546 centrex-trajectories-0.3.0/centrex_trajectories/common_types.py
+-rw-r--r--   0        0        0    19714 2024-05-21 23:39:01.326797 centrex-trajectories-0.3.0/centrex_trajectories/data_structures.py
+-rw-r--r--   0        0        0      461 2024-02-05 02:37:13.221609 centrex-trajectories-0.3.0/centrex_trajectories/particles.py
+-rw-r--r--   0        0        0    14392 2024-05-21 23:55:39.608754 centrex-trajectories-0.3.0/centrex_trajectories/propagation.py
+-rw-r--r--   0        0        0     8618 2024-05-21 23:53:02.390683 centrex-trajectories-0.3.0/centrex_trajectories/propagation_ballistic.py
+-rw-r--r--   0        0        0     5269 2024-05-21 23:56:01.855678 centrex-trajectories-0.3.0/centrex_trajectories/propagation_ode.py
+-rw-r--r--   0        0        0      697 2024-02-05 02:37:13.230610 centrex-trajectories-0.3.0/centrex_trajectories/propagation_options.py
+-rw-r--r--   0        0        0        0 2023-01-22 08:03:57.373693 centrex-trajectories-0.3.0/centrex_trajectories/py.typed
+-rw-r--r--   0        0        0     3474 2024-05-21 22:29:06.955771 centrex-trajectories-0.3.0/centrex_trajectories/random_generation.py
+-rw-r--r--   0        0        0      243 2024-04-04 16:37:01.288551 centrex-trajectories-0.3.0/centrex_trajectories/saved_data/stark_poly.pkl
+-rw-r--r--   0        0        0      902 2024-04-04 16:37:01.289553 centrex-trajectories-0.3.0/centrex_trajectories/utils.py
+-rw-r--r--   0        0        0     2909 2024-05-21 22:29:06.972643 centrex-trajectories-0.3.0/centrex_trajectories/visualization.py
+-rw-r--r--   0        0        0     1086 2022-05-19 04:30:48.923066 centrex-trajectories-0.3.0/LICENSE
+-rw-r--r--   0        0        0      735 2024-05-22 00:15:22.484103 centrex-trajectories-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     4194 2024-05-22 00:02:24.659607 centrex-trajectories-0.3.0/README.md
+-rw-r--r--   0        0        0     4921 1970-01-01 00:00:00.000000 centrex-trajectories-0.3.0/setup.py
+-rw-r--r--   0        0        0     4539 1970-01-01 00:00:00.000000 centrex-trajectories-0.3.0/PKG-INFO
```

### Comparing `centrex-trajectories-0.2.0/centrex_trajectories/__init__.py` & `centrex-trajectories-0.3.0/centrex_trajectories/__init__.py`

 * *Files identical despite different names*

### Comparing `centrex-trajectories-0.2.0/centrex_trajectories/beamline_objects.py` & `centrex-trajectories-0.3.0/centrex_trajectories/beamline_objects.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 from typing import Any, List, Optional, Tuple, overload
 
 import numpy as np
 import numpy.typing as npt
 
 from .common_types import NDArray_or_Float
-from .data_structures import Coordinates, Force, Velocities
+from .data_structures import Acceleration, Coordinates, Force, Velocities
 from .particles import Particle
 from .propagation_ballistic import calculate_time_ballistic, propagate_ballistic
 from .propagation_options import PropagationType
 
 __all__ = [
     "Section",
     "ElectrostaticQuadrupoleLens",
@@ -124,14 +124,16 @@
         self,
         name: str,
         objects: List[Any],
         start: float,
         stop: float,
         V: float,
         R: float,
+        x: float = 0,
+        y: float = 0,
         save_collisions: bool = False,
         stark_potential: None | npt.NDArray[np.float64] = None,
     ) -> None:
         """
         Electrostatic Quadrupole Lens Section
 
         Args:
@@ -147,14 +149,16 @@
             stark_potential (Optional[np.ndarray]): polynomial coefficients of the stark
                                                     potential as a function of electric
                                                     field
         """
         super().__init__(name, objects, start, stop, save_collisions)
         self.V = V
         self.R = R
+        self.x0 = x
+        self.y0 = y
         self._stark_potential = np.polynomial.Polynomial([0])
         self._check_objects()
         self._initialize_potentials(stark_potential)
 
     def _initialize_potentials(
         self, stark_potential: None | npt.NDArray[np.float64] = None
     ) -> None:
@@ -164,14 +168,20 @@
         if stark_potential is None:
             self._stark_potential = stark_potential_default
         else:
             self._stark_potential = np.polynomial.Polynomial(stark_potential)
 
         self._stark_potential_derivative = self._stark_potential.deriv()
 
+    def x_transformed(self, x: NDArray_or_Float) -> NDArray_or_Float:
+        return x - self.x0
+
+    def y_transformed(self, y: NDArray_or_Float) -> NDArray_or_Float:
+        return y - self.y0
+
     def electric_field(
         self,
         x: NDArray_or_Float,
         y: NDArray_or_Float,
         z: NDArray_or_Float,
     ) -> NDArray_or_Float:
         """
@@ -181,15 +191,17 @@
             x (Union[NDArray[np.float64], float]): x coordinate(s) [m]
             y (Union[NDArray[np.float64], float]): y coordinate(s) [m]
             z (Union[NDArray[np.float64], float]): z coordinate(s) [m]
 
         Returns:
             Union[NDArray[np.float64], float]: electric field at x,y,z in V/m
         """
-        return 2 * self.V * np.sqrt(x**2 + y**2) / (self.R) ** 2
+        _x = self.x_transformed(x)
+        _y = self.y_transformed(y)
+        return 2 * self.V * np.sqrt(_x**2 + _y**2) / (self.R) ** 2
 
     def electric_field_derivative_r(
         self,
         x: NDArray_or_Float,
         y: NDArray_or_Float,
         z: NDArray_or_Float,
     ) -> NDArray_or_Float:
@@ -234,17 +246,23 @@
             x (Union[NDArray[np.float64], float]): x coordinate(s) [m]
             y (Union[NDArray[np.float64], float]): y coordinate(s) [m]
             z (Union[NDArray[np.float64], float]): z coordinate(s) [m]
 
         Returns:
             List: force in x, y and z
         """
-        r = np.sqrt(x**2 + y**2)
-        dx = x / r
-        dy = y / r
+        _x = self.x_transformed(x)
+        _y = self.y_transformed(y)
+        r = np.sqrt(_x**2 + _y**2)
+        if r == 0:
+            dx = 0.0
+            dy = 0.0
+        else:
+            dx = _x / r
+            dy = _y / r
         stark = -self.stark_potential_derivative(
             x, y, z
         ) * self.electric_field_derivative_r(x, y, z)
         return (stark * dx, stark * dy, 0)
 
     def stark_potential_derivative(
         self,
@@ -504,15 +522,19 @@
 
         Returns:
             bool: True if within bounds, else False
         """
         return (self.z >= start) & (self.z <= stop)
 
     def get_acceptance(
-        self, start: Coordinates, stop: Coordinates, vels: Velocities, force: Force
+        self,
+        start: Coordinates,
+        stop: Coordinates,
+        vels: Velocities,
+        acceleration: Acceleration,
     ) -> npt.NDArray[np.bool_]:
         raise NotImplementedError
 
     def collision_event_function(self, x: float, y: float, z: float) -> float:
         raise NotImplementedError
 
 
@@ -531,15 +553,19 @@
     r: float
 
     @property
     def z_stop(self):
         return self.z
 
     def get_acceptance(
-        self, start: Coordinates, stop: Coordinates, vels: Velocities, force: Force
+        self,
+        start: Coordinates,
+        stop: Coordinates,
+        vels: Velocities,
+        acceleration: Acceleration,
     ) -> npt.NDArray[np.bool_]:
         """
         check if the supplied coordinates are within the aperture
 
         Args:
             coords (Coordinates): coordinates to check
 
@@ -573,15 +599,19 @@
     wy: float
 
     @property
     def z_stop(self):
         return self.z
 
     def get_acceptance(
-        self, start: Coordinates, stop: Coordinates, vels: Velocities, force: Force
+        self,
+        start: Coordinates,
+        stop: Coordinates,
+        vels: Velocities,
+        acceleration: Acceleration,
     ) -> npt.NDArray[np.bool_]:
         """
         check if the supplied coordinates are within the aperture
 
         Args:
             coords (Coordinates): coordinates to check
 
@@ -623,15 +653,19 @@
     wyp: float
 
     @property
     def z_stop(self):
         return self.z
 
     def get_acceptance(
-        self, start: Coordinates, stop: Coordinates, vels: Velocities, force: Force
+        self,
+        start: Coordinates,
+        stop: Coordinates,
+        vels: Velocities,
+        acceleration: Acceleration,
     ) -> npt.NDArray[np.bool_]:
         """
         check if the supplied coordinates are within the aperture
 
         Args:
             start (Coordinates): start coordinates
             stop (Coordinates): stop coordinates
@@ -676,21 +710,29 @@
     def z_stop(self):
         return self.z + self.length
 
     def check_in_bounds(self, start: float, stop: float) -> bool:
         return self.z >= start and self.z + self.length <= stop
 
     def get_acceptance(
-        self, start: Coordinates, stop: Coordinates, vels: Velocities, force: Force
+        self,
+        start: Coordinates,
+        stop: Coordinates,
+        vels: Velocities,
+        acceleration: Acceleration,
     ) -> npt.NDArray[np.bool_]:
-        m, _, _ = self.get_collisions(start, stop, vels, force)
+        m, _, _ = self.get_collisions(start, stop, vels, acceleration)
         return ~m
 
     def get_collisions(
-        self, start: Coordinates, stop: Coordinates, vels: Velocities, force: Force
+        self,
+        start: Coordinates,
+        stop: Coordinates,
+        vels: Velocities,
+        acceleration: Acceleration,
     ) -> Tuple[npt.NDArray[np.bool_], Coordinates, Velocities]:
         t = np.zeros(start.x.shape)
 
         dx_upper = (self.x + self.separation / 2) - start.x
         dy_upper = (self.x - self.separation / 2) - start.x
 
         m_inside = (start.x > (self.x - self.separation / 2)) & (
@@ -698,26 +740,26 @@
         )
         m_below = start.x < (self.x - self.separation / 2)
         m_above = start.x > (self.x + self.separation / 2)
         m_vpos = vels.vx > 0
         m_vneg = vels.vx < 0
 
         m = m_inside & m_vpos
-        t[m] = calculate_time_ballistic(dx_upper[m], vels.vx[m], force.fx)
+        t[m] = calculate_time_ballistic(dx_upper[m], vels.vx[m], acceleration.ax)
 
         m = m_inside & m_vneg
-        t[m] = calculate_time_ballistic(dy_upper[m], vels.vx[m], force.fx)
+        t[m] = calculate_time_ballistic(dy_upper[m], vels.vx[m], acceleration.ax)
 
         m = m_below & m_vpos
-        t[m] = calculate_time_ballistic(dy_upper[m], vels.vx[m], force.fx)
+        t[m] = calculate_time_ballistic(dy_upper[m], vels.vx[m], acceleration.ax)
 
         m = m_above & m_vneg
-        t[m] = calculate_time_ballistic(dx_upper[m], vels.vx[m], force.fx)
+        t[m] = calculate_time_ballistic(dx_upper[m], vels.vx[m], acceleration.ax)
 
-        x, v = propagate_ballistic(t, start, vels, force)
+        x, v = propagate_ballistic(t, start, vels, acceleration)
         m = x.z <= (self.z + self.length)
         m &= x.z >= self.z
         m &= np.abs(x.y - self.y) <= self.width / 2
         return m, x.get_masked(m), v.get_masked(m)
 
     def collision_event_function(self, x: float, y: float, z: float) -> float:
         # for now assume electrode plates in y direction
@@ -742,15 +784,19 @@
     length: float
     radius: float
 
     def check_in_bounds(self, start: float, stop: float) -> bool:
         return self.z >= start and self.z + self.length <= stop
 
     def get_acceptance(
-        self, start: Coordinates, stop: Coordinates, vels: Velocities, force: Force
+        self,
+        start: Coordinates,
+        stop: Coordinates,
+        vels: Velocities,
+        acceleration: Acceleration,
     ) -> npt.NDArray[np.bool_]:
         mask_z = (stop.z >= self.z) & (stop.z <= self.z + self.length)
         mask_r = ((stop.x - self.x) ** 2 + (stop.y - self.y) ** 2) > self.radius**2
         accept_array = np.ones(stop.x.shape, dtype=np.bool_)
         accept_array[mask_z & mask_r] = False
         return accept_array
```

### Comparing `centrex-trajectories-0.2.0/centrex_trajectories/data_structures.py` & `centrex-trajectories-0.3.0/centrex_trajectories/data_structures.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,22 @@
 from dataclasses import dataclass, field
 from typing import Any, ItemsView, Iterator, List, Optional, Tuple, Union, ValuesView
 
 import numpy as np
 import numpy.typing as npt
 from scipy.optimize import OptimizeResult
 
-__all__: List[str] = ["Force", "Gravity", "Velocities", "Coordinates", "Trajectories"]
+__all__: List[str] = [
+    "Force",
+    "Acceleration",
+    "Gravity",
+    "Velocities",
+    "Coordinates",
+    "Trajectories",
+]
 
 
 @dataclass(frozen=True)
 class SectionData:
     """
     Specifies a section of the beamline
 
@@ -61,14 +68,31 @@
             raise TypeError(f"can only add Force (not {type(other)}) to Force")
 
 
 Gravity = Force
 
 
 @dataclass
+class Acceleration:
+    ax: float
+    ay: float
+    az: float
+
+    def __add__(self, other) -> Acceleration:
+        if isinstance(other, Acceleration):
+            return Force(self.ax + other.ax, self.ay + other.ay, self.az + other.az)
+        elif other is None:
+            return self
+        else:
+            raise TypeError(
+                f"can only add Acceleration (not {type(other)}) to Acceleration"
+            )
+
+
+@dataclass
 class Velocity:
     """
     Velocity
 
     Attributes:
         vx (float): velocity in x [m/s]
         vy (float): velocity in y [m/s]
```

### Comparing `centrex-trajectories-0.2.0/centrex_trajectories/propagation.py` & `centrex-trajectories-0.3.0/centrex_trajectories/propagation.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,47 +3,55 @@
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import numpy.typing as npt
 
 from .beamline_objects import ODESection, Section
 from .data_structures import (
+    Acceleration,
     Coordinates,
     Force,
     SectionData,
     Trajectories,
     Trajectory,
     Velocities,
 )
-from .particles import Particle
+from .particles import Particle, TlF
 from .propagation_ballistic import propagate_ballistic_trajectories
 from .propagation_ode import propagate_ODE_trajectories
 from .propagation_options import PropagationOptions, PropagationType
 
 __all__: List[str] = ["PropagationType", "propagate_trajectories", "PropagationOptions"]
 
 
 def do_ballistic(
     indices: npt.NDArray[np.int_],
     timestamps_tracked: npt.NDArray[np.float_],
     coordinates_tracked: Coordinates,
     velocities_tracked: Velocities,
     trajectories: Trajectories,
     section: Union[Section, ODESection],
+    particle: Particle,
     force: Force,
     z_save_section: Union[List[float], npt.NDArray[np.float_], None],
     options: PropagationOptions,
 ) -> tuple[
     npt.NDArray[np.float_],
     Coordinates,
     Velocities,
     npt.NDArray[np.int_],
     Trajectories,
     SectionData,
 ]:
+    force_cst = force + section.force
+    acceleration = Acceleration(
+        force_cst.fx / particle.mass,
+        force_cst.fy / particle.mass,
+        force_cst.fz / particle.mass,
+    )
     (
         mask,
         timestamp_list,
         coord_list,
         velocities_list,
         nr_collisions,
         collisions,
@@ -51,15 +59,15 @@
         timestamps_tracked
         if timestamps_tracked.ndim == 1
         else timestamps_tracked[:, -1],
         coordinates_tracked.get_last(),
         velocities_tracked.get_last(),
         section.objects,
         section.stop,
-        force + section.force,
+        acceleration,
         z_save=z_save_section,
         save_collisions=section.save_collisions,
         options=options,
     )
 
     # only keep trajectories that made it through
     timestamps_tracked = timestamps_tracked[mask]
@@ -95,15 +103,15 @@
 
 def propagate_trajectories(
     sections: List[Union[Section, ODESection]],
     coordinates_init: Coordinates,
     velocities_init: Velocities,
     particle: Particle,
     t_start: Optional[npt.NDArray[np.float_]] = None,
-    force: Force = Force(0.0, -9.81, 0.0),
+    force: Force = Force(0.0, -9.81 * TlF().mass, 0.0),
     z_save: Optional[List] = None,
     options: PropagationOptions = PropagationOptions(),
 ) -> Tuple[List[SectionData], Trajectories]:
     """
     Propagate trajectories through sections starting at initial coordinates and initial
     velocities
 
@@ -173,22 +181,25 @@
             ) = do_ballistic(
                 indices=indices,
                 timestamps_tracked=timestamps_tracked,
                 coordinates_tracked=coordinates_tracked,
                 velocities_tracked=velocities_tracked,
                 trajectories=trajectories,
                 section=section,
+                particle=particle,
                 force=force,
                 z_save_section=z_save_section,
                 options=options,
             )
             section_data.append(sec_dat)
         # propagate ODE if section is ODE
         elif section.propagation_type == PropagationType.ode:
-            if np.any(coordinates_tracked.get_last().z < section.start):
+            if np.any(
+                coordinates_tracked.get_last().z < section.start
+            ) and not np.allclose(coordinates_tracked.get_last().z, section.start):
                 # do ballistic until ode section
                 (
                     timestamps_tracked,
                     coordinates_tracked,
                     velocities_tracked,
                     indices,
                     trajectories,
@@ -204,14 +215,15 @@
                         objects=[],
                         start=coordinates_tracked.get_last().z[
                             0
                         ],  # just give it one start coord, start is not used here
                         stop=section.start,
                         save_collisions=False,
                     ),
+                    particle=particle,
                     force=force,
                     z_save_section=z_save_section,
                     options=options,
                 )
             if len(trajectories) == 0:
                 for index, t, c, v in zip(
                     indices, timestamps_tracked, coordinates_tracked, velocities_tracked
```

### Comparing `centrex-trajectories-0.2.0/centrex_trajectories/propagation_ballistic.py` & `centrex-trajectories-0.3.0/centrex_trajectories/propagation_ballistic.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from collections.abc import Iterable
 from copy import deepcopy
 from typing import List, Optional, Tuple, Union
 
 import numpy as np
 import numpy.typing as npt
 
-from .data_structures import Coordinates, Force, Velocities
+from .data_structures import Acceleration, Coordinates, Velocities
 from .propagation_options import PropagationOptions
 
 __all__: List[str] = []
 
 
 def propagate_ballistic(
     t: npt.NDArray[np.float_],
     origin: Coordinates,
     velocities: Velocities,
-    force: Force,
+    acceleration: Acceleration,
 ) -> Tuple[Coordinates, Velocities]:
     """
     Propagate trajectories starting at `origin` with `velocities` for a time `t`
 
     Args:
         t (NDArray[np.float_]): time to propagate per particle
         origin (Coordinates): origin of each particle
@@ -28,22 +28,22 @@
 
     Returns:
         Tuple[Coordinates, Velocities]: coordinates and velocities after propagating for
                             time `t`
     """
     return (
         Coordinates(
-            origin.x + velocities.vx * t + 1 / 2 * force.fx * t**2,
-            origin.y + velocities.vy * t + 1 / 2 * force.fy * t**2,
-            origin.z + velocities.vz * t + 1 / 2 * force.fz * t**2,
+            origin.x + velocities.vx * t + 1 / 2 * acceleration.ax * t**2,
+            origin.y + velocities.vy * t + 1 / 2 * acceleration.ay * t**2,
+            origin.z + velocities.vz * t + 1 / 2 * acceleration.az * t**2,
         ),
         Velocities(
-            velocities.vx + force.fx * t,
-            velocities.vy + force.fy * t,
-            velocities.vz + force.fz * t,
+            velocities.vx + acceleration.ax * t,
+            velocities.vy + acceleration.ay * t,
+            velocities.vz + acceleration.az * t,
         ),
     )
 
 
 def calculate_time_ballistic(
     dx: npt.NDArray[np.float_], v: npt.NDArray[np.float_], a: float = 0.0
 ) -> npt.NDArray[np.float_]:
@@ -101,15 +101,15 @@
 
 def propagate_ballistic_trajectories(
     t_start: npt.NDArray[np.float_],
     origin: Coordinates,
     velocities: Velocities,
     objects: List,
     z_stop: float,
-    force: Force = Force(0.0, -9.81, 0.0),
+    acceleration: Acceleration = Acceleration(0.0, -9.81, 0.0),
     z_save: Optional[Union[List[float], npt.NDArray[np.float_]]] = None,
     save_collisions: bool = False,
     options: PropagationOptions = PropagationOptions(),
 ) -> Tuple[
     npt.NDArray[np.bool_],
     npt.NDArray[np.float_],
     Coordinates,
@@ -150,30 +150,43 @@
     t_accepted = deepcopy(t_start)
 
     # iterate through apertures, saving coordinates and velocities at each object and
     # saving collisions if save_collisions == True
     for obj in objects:
         # distance
         dz = obj.z_stop - accepted_coords.z
-        # velocity
-        vz = accepted_velocities.vz
-        # forward acceleration
-        fz = force.fz
-        t = calculate_time_ballistic(dz, vz, fz)
 
-        x, v = propagate_ballistic(t, accepted_coords, accepted_velocities, force)
-        acceptance = obj.get_acceptance(accepted_coords, x, accepted_velocities, force)
+        if not np.allclose(dz, 0):
+            # velocity
+            vz = accepted_velocities.vz
+            # forward acceleration
+            az = acceleration.az
+            t = calculate_time_ballistic(dz, vz, az)
+
+            x, v = propagate_ballistic(
+                t, accepted_coords, accepted_velocities, acceleration
+            )
+        else:
+            t = deepcopy(t_accepted)
+            x, v = deepcopy(accepted_coords), deepcopy(accepted_velocities)
+        try:
+            acceptance = obj.get_acceptance(
+                accepted_coords, x, accepted_velocities, acceleration
+            )
+        except AssertionError as error:
+            raise AssertionError(f"{obj} -> {error.args[0]}")
+        # why is this line here?
         acceptance &= ~np.isnan(t)
 
         if save_collisions:
             if hasattr(obj, "get_collisions"):
                 collisions.append(
-                    obj.get_collisions(accepted_coords, x, accepted_velocities, force)[
-                        1:
-                    ]
+                    obj.get_collisions(
+                        accepted_coords, x, accepted_velocities, acceleration
+                    )[1:]
                 )
             else:
                 collisions.append(
                     (x.get_masked(~acceptance), v.get_masked(~acceptance))
                 )
 
         accepted_coords = accepted_coords.get_masked(acceptance)
@@ -187,28 +200,28 @@
 
     # save coordinates and velocities at z positions z_save if supplied
     if z_save is not None:
         for idz, z in enumerate(z_save):
             coords = accepted_coords.get_last()
             vels = accepted_velocities.get_last()
             dz = z - coords.z
-            dt = calculate_time_ballistic(dz, vels.vz, force.fz)
-            x, v = propagate_ballistic(dt, coords, vels, force)
+            dt = calculate_time_ballistic(dz, vels.vz, acceleration.az)
+            x, v = propagate_ballistic(dt, coords, vels, acceleration)
             if idz != 0:
                 t_accepted = np.column_stack([t_accepted, t_accepted[:, -1] + dt])
             else:
                 t_accepted = np.column_stack([t_accepted, t_accepted + dt])
             accepted_coords.column_stack(x)
             accepted_velocities.column_stack(v)
 
     # timestamps, coordinates and velocities at the end of the section
     coords = accepted_coords.get_last()
     vels = accepted_velocities.get_last()
-    dt = calculate_time_ballistic(z_stop - coords.z, vels.vz, force.fz)
-    x, v = propagate_ballistic(dt, coords, vels, force)
+    dt = calculate_time_ballistic(z_stop - coords.z, vels.vz, acceleration.az)
+    x, v = propagate_ballistic(dt, coords, vels, acceleration)
 
     if z_save is not None and len(z_save) > 0:
         t_accepted = np.column_stack([t_accepted, t_accepted[:, -1] + dt])
     else:
         t_accepted = np.column_stack([t_accepted, t_accepted + dt])
     accepted_coords.column_stack(x)
     accepted_velocities.column_stack(v)
```

### Comparing `centrex-trajectories-0.2.0/centrex_trajectories/propagation_ode.py` & `centrex-trajectories-0.3.0/centrex_trajectories/propagation_ode.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import numpy as np
 import numpy.typing as npt
 from joblib import Parallel, delayed
 from scipy.integrate import solve_ivp
 from scipy.optimize import OptimizeResult
 
 from .data_structures import Coordinates, Force, Velocities
+from .particles import TlF
 from .propagation_options import PropagationOptions
 
 __all__: List[str] = []
 
 
 def z_stop_event_generator(
     z_stop: float,
@@ -58,20 +59,20 @@
 def solve_ode(*args) -> OptimizeResult:
     """
     Solve the trajectory propagation ODE for a single trajectory
 
     Returns:
         OptimizeResult: solution of the trajectory ODE
     """
-    t, x, v, z_stop, mass, force, gravity, events = args
+    t, x, v, z_stop, mass, force, force_cst, events = args
     t_span = [t, t + 2 * (z_stop - x.z) / v.vz]
     z_stop_event = z_stop_event_generator(z_stop)
     p = [x.x, x.y, x.z, v.vx, v.vy, v.vz]
     _ode_fun = partial(
-        ode_fun, **{"mass": mass, "force_fn": force, "force_cst": gravity}
+        ode_fun, **{"mass": mass, "force_fn": force, "force_cst": force_cst}
     )
     sol = solve_ivp(
         _ode_fun, t_span, p, events=events + [z_stop_event], rtol=1e-7, atol=1e-7
     )
     return sol
 
 
@@ -86,43 +87,43 @@
     General function describing the RHS of trajectory propagation
 
     Args:
         t (npt.NDArray[np.float64]): initial timestamps
         d (List[float]): list with x,y,z,vx,vy,vz
         mass (float): mass of particle
         force (Callable): function describing the force as a function of x,y,z
-        gravity (Gravity): gravitational accelleration
+        force_cst (Force): constant force
 
     Returns:
         Union[List[npt.NDArray[np.float64]], List[float]]: RHS of trajectory propagation
                                                             ODE
     """
     x, y, z, vx, vy, vz = d
     fx, fy, fz = force_fn(t, x, y, z)
     ax = fx / mass
     ay = fy / mass
     az = fz / mass
     return (
         vx,
         vy,
         vz,
-        ax + force_cst.fx,
-        ay + force_cst.fy,
-        az + force_cst.fz,
+        ax + force_cst.fx / mass,
+        ay + force_cst.fy / mass,
+        az + force_cst.fz / mass,
     )
 
 
 def propagate_ODE_trajectories(
     t_start: npt.NDArray[np.float_],
     origin: Coordinates,
     velocities: Velocities,
     z_stop: float,
     mass: float,
     force_fun: Callable[[float, float, float, float], Tuple[float, float, float]],
-    force_cst: Force = Force(0.0, -9.81, 0.0),
+    force_cst: Force = Force(0.0, -9.81 * TlF().mass, 0.0),
     events: Sequence[Callable[[float, float, float], float]] = [],
     z_save: Optional[
         Union[List[Union[float, int]], npt.NDArray[Union[np.float_, np.int_]]]
     ] = None,
     options: PropagationOptions = PropagationOptions(),
 ) -> List[OptimizeResult]:
     """
```

### Comparing `centrex-trajectories-0.2.0/centrex_trajectories/propagation_options.py` & `centrex-trajectories-0.3.0/centrex_trajectories/propagation_options.py`

 * *Files identical despite different names*

### Comparing `centrex-trajectories-0.2.0/centrex_trajectories/random_generation.py` & `centrex-trajectories-0.3.0/centrex_trajectories/random_generation.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 def generate_random_coordinates_normal_circle(
     sigma: float,
     number: int,
     *,
     x: float = 0,
     y: float = 0,
     z: float = 0,
-    rng: Optional[np.random.Generator] = None
+    rng: Optional[np.random.Generator] = None,
 ) -> Coordinates:
     """
     Generate normally distributed samples over a circle of radius `radius` in the xy
     plane
 
     Args:
         sigma (float): sigma of the circle
@@ -36,28 +36,28 @@
     Returns:
         Coordinates: randomly generated coordinates
     """
     if rng is None:
         rng = np.random.default_rng()
 
     return Coordinates(
-        x=x + rng.normal(0, sigma, number),
-        y=y + rng.normal(0, sigma, number),
+        x=rng.normal(x, sigma, number),
+        y=rng.normal(y, sigma, number),
         z=z * np.ones(number),
     )
 
 
 def generate_random_coordinates_uniform_circle(
     radius: float,
     number: int,
     *,
     x: float = 0,
     y: float = 0,
     z: float = 0,
-    rng: Optional[np.random.Generator] = None
+    rng: Optional[np.random.Generator] = None,
 ) -> Coordinates:
     """
     Generate random coordinates uniformly over a circle
 
     Args:
         radius (float): radius of cicle
         number (int): number of samples
@@ -70,32 +70,32 @@
     Returns:
         Coordinates: randomly generated coordinates
     """
     if rng is None:
         rng = np.random.default_rng()
 
     theta = rng.uniform(0, 2 * np.pi, number)
-    r = np.sqrt(rng.uniform(0, radius, number))
+    r = np.sqrt(rng.uniform(0, radius**2, number))
     return Coordinates(
-        x=r * np.cos(theta),
-        y=r * np.sin(theta),
+        x=r * np.cos(theta) + x,
+        y=r * np.sin(theta) + y,
         z=z * np.ones(number),
     )
 
 
 def generate_random_velocities_normal(
     vx: float,
     vy: float,
     vz: float,
     sigma_vx: float,
     sigma_vy: float,
     sigma_vz: float,
     number: int,
     *,
-    rng: Optional[np.random.Generator] = None
+    rng: Optional[np.random.Generator] = None,
 ) -> Velocities:
     """
     Generate normally distributed velocity samples
 
     Args:
         vx (float): mean vx
         vy (float): mean vy
@@ -109,11 +109,11 @@
 
     Returns:
         Velocities: generated samples
     """
     if rng is None:
         rng = np.random.default_rng()
     return Velocities(
-        vx=vx + rng.normal(vx, sigma_vx, number),
-        vy=vy + rng.normal(vy, sigma_vy, number),
-        vz=vz + rng.normal(vz, sigma_vz, number),
+        vx=rng.normal(vx, sigma_vx, number),
+        vy=rng.normal(vy, sigma_vy, number),
+        vz=rng.normal(vz, sigma_vz, number),
     )
```

### Comparing `centrex-trajectories-0.2.0/centrex_trajectories/utils.py` & `centrex-trajectories-0.3.0/centrex_trajectories/utils.py`

 * *Files identical despite different names*

### Comparing `centrex-trajectories-0.2.0/centrex_trajectories/visualization.py` & `centrex-trajectories-0.3.0/centrex_trajectories/visualization.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,54 +12,78 @@
 
 def plot_beamline(
     sections: List[Union[Section, ODESection]],
     ax: Optional[axes.Axes] = None,
     facecolor: str = "C0",
     edgecolor: str = "k",
     alpha: float = 0.5,
+    axis: str = "x",
 ):
     objects = []
     for section in sections:
         objects.extend(section.objects)
 
     height = 0.0
     for obj in objects:
         if isinstance(obj, CircularAperture):
-            if height <= (obj.y + obj.r) * 2:
-                height = (obj.y + obj.r) * 2
+            if axis == "x":
+                if height <= (obj.x + obj.r) * 2:
+                    height = (obj.x + obj.r) * 2
+            elif axis == "y":
+                if height <= (obj.y + obj.r) * 2:
+                    height = (obj.y + obj.r) * 2
         if isinstance(obj, RectangularAperture):
-            if height <= (obj.y + obj.wy / 2) * 2:
-                height = (obj.y + obj.wy / 2) * 2
+            if axis == "x":
+                if height <= (obj.x + obj.wx / 2) * 2:
+                    height = (obj.x + obj.wx / 2) * 2
+            elif axis == "y":
+                if height <= (obj.y + obj.wy / 2) * 2:
+                    height = (obj.y + obj.wy / 2) * 2
     patches = [
         Rectangle((section.start, -height), section.stop - section.start, 2 * height)
         for section in sections
     ]
 
     # Create patch collection with specified colour/alpha
     pc = PatchCollection(patches, facecolor=facecolor, alpha=alpha, edgecolor=edgecolor)
 
     if ax is None:
         fig, ax = plt.subplots(figsize=(8, 5))
 
     for obj in objects:
         if isinstance(obj, CircularAperture):
-            ax.plot([obj.z, obj.z], [obj.y - obj.r, obj.y + obj.r], lw=4, color="C3")
+            if axis == "x":
+                ax.plot(
+                    [obj.z, obj.z], [obj.x - obj.r, obj.x + obj.r], lw=4, color="C3"
+                )
+            elif axis == "y":
+                ax.plot(
+                    [obj.z, obj.z], [obj.y - obj.r, obj.y + obj.r], lw=4, color="C3"
+                )
         if isinstance(obj, RectangularAperture):
-            ax.plot(
-                [obj.z, obj.z],
-                [obj.y - obj.wy / 2, obj.y + obj.wy / 2],
-                lw=4,
-                color="C3",
-            )
+            if axis == "x":
+                ax.plot(
+                    [obj.z, obj.z],
+                    [obj.x - obj.wx / 2, obj.x + obj.wx / 2],
+                    lw=4,
+                    color="C3",
+                )
+            elif axis == "y":
+                ax.plot(
+                    [obj.z, obj.z],
+                    [obj.y - obj.wy / 2, obj.y + obj.wy / 2],
+                    lw=4,
+                    color="C3",
+                )
 
     # Add collection to axes
     ax.add_collection(pc)
 
     dx = sections[-1].stop - sections[0].start
     x0 = sections[0].start
     ax.set_xlim(x0 - 0.1 * dx, x0 + 1.1 * dx)
     ax.set_ylim(-height * 1.1, height * 1.1)
 
     ax.set_xlabel("z [m]")
-    ax.set_ylabel("y [m]")
+    ax.set_ylabel(f"{axis} [m]")
 
     return ax
```

### Comparing `centrex-trajectories-0.2.0/LICENSE` & `centrex-trajectories-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `centrex-trajectories-0.2.0/pyproject.toml` & `centrex-trajectories-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "centrex-trajectories"
-version = "0.2.0"
+version = "0.3.0"
 description = ""
 license = "MIT"
 authors = ["ograsdijk <o.grasdijk@gmail.com>"]
 readme = "README.md"
 packages = [{include = "centrex_trajectories"}]
 include = ["centrex_trajectories/saved_data/stark_poly.pkl"]
```

### Comparing `centrex-trajectories-0.2.0/README.md` & `centrex-trajectories-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -100,16 +100,16 @@
 velocities_init = Velocities(
     vx=np.random.randn(n_trajectories) * 39.4,
     vy=np.random.randn(n_trajectories) * 39.4,
     vz=np.random.randn(n_trajectories) * 16 + 184,
 )
 
 options = PropagationOptions(n_cores=6, verbose=False)
-gravity = Force(0, -9.81, 0)
 particle = TlF()
+gravity = Force(0, -9.81*particle.mass, 0)
 
 section_data, trajectories = propagate_trajectories(
     sections,
     coordinates_init,
     velocities_init,
     particle,
     force=gravity,
```

### Comparing `centrex-trajectories-0.2.0/setup.py` & `centrex-trajectories-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['joblib>=1.2.0,<2.0.0',
  'matplotlib>=3.6.2,<4.0.0',
  'numpy>=1.23.4,<2.0.0',
  'scipy>=1.9.3,<2.0.0']
 
 setup_kwargs = {
     'name': 'centrex-trajectories',
-    'version': '0.2.0',
+    'version': '0.3.0',
     'description': '',
-    'long_description': '[![Python versions on PyPI](https://img.shields.io/pypi/pyversions/centrex-trajectories.svg)](https://pypi.python.org/pypi/centrex-trajectories/)\n[![CeNTREX-TlF version on PyPI](https://img.shields.io/pypi/v/centrex-trajectories.svg "CeNTREX-TlF on PyPI")](https://pypi.python.org/pypi/centrex-trajectories/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n\n# CeNTREX-trajectories\nCode for simulating CeNTREX trajectories\n\n## Installation\nClone repo and install with `pip` or directly install from GitHub with:  \n```\npip install git+https://github.com/ograsdijk/CeNTREX-trajectories\n```\n\n## Sections\nThe beamline is split into sections specified with `Section`, which can be used as follows:\n```Python\nsections = [\n    fourK = Section(\n        name = "4K shield",\n        objects = [CircularAperture(x=0, y=0, z=5e-3)],\n        start = 0,\n        stop = 10e-2,\n        save_collisions = False,\n        propagation_type=PropagationType.ballistic,\n    )\n]\n```\nThis defines a section called `4K shield`, which runs from `z = 0 m -> 10e-2 m`. Collisions aren\'t\nsaved, the `propagation_type` is ballistic and it contains a single circular aperture centered around\nthe z axis with a radius of 5 mm.\n\n## Collision objects\nCurrently two type of apertures are defined for collisions:\n* `CircularAperture(x: float,y: float,r: float)`\n* `RectangularAperture(x: float,y: float,wx: float,wy: float)`\n\nCustom collision objects can be defined; apertures should inherit from `Aperture`, and each custom\ncollision object should have two functions:\n* `check_in_bounds(start: float, stop: float)` which returns a boolean specifying whether the object fully resides inside the section\n* `get_acceptance(coordinates: Coordinates)` which returns a boolean arrays specifiying which trajectories make it through the aperture\n\n## Propagation types\nThere is support for ballistic and ODE solver trajectories, which is specified on a per section basis through `Section.propagation_type`\n* `PropagationType.ballistic` assumes a constant velocity and constant gravitational acceleration\n* `PropagationType.ode` needs a defined force function in the section and uses `scipy.integrate.solve_ivp` to calculate the trajectory\n\n## Working example\n```Python\nimport numpy as np\nfrom centrex_trajectories import (\n    Coordinates,\n    Velocities,\n    Force,\n    PropagationType,\n    propagate_trajectories,\n    PropagationOptions,\n)\n\nfrom centrex_trajectories.beamline_objects import CircularAperture, Section\nfrom centrex_trajectories.particles import TlF\n\nin_to_m = 0.0254\n\nfourK = Section(\n    name="4K shield",\n    objects=[CircularAperture(x=0, y=0, z=1.75 * in_to_m, r=1 / 2 * in_to_m)],\n    start=0,\n    stop=2 * in_to_m,\n    save_collisions=False,\n    propagation_type=PropagationType.ballistic,\n)\nfourtyK = Section(\n    name="40K shield",\n    objects=[\n        CircularAperture(x=0, y=0, z=fourK.stop + 1.25 * in_to_m, r=1 / 2 * in_to_m)\n    ],\n    start=fourK.stop,\n    stop=fourK.stop + 1.5 * in_to_m,\n    save_collisions=False,\n    propagation_type=PropagationType.ballistic,\n)\nbbexit = Section(\n    name="Beamsource Exit",\n    objects=[CircularAperture(0, 0, fourtyK.stop + 2.5 * in_to_m, 2 * in_to_m)],\n    start=fourtyK.stop,\n    stop=fourtyK.stop + 3.25 * in_to_m,\n    save_collisions=False,\n    propagation_type=PropagationType.ballistic,\n)\n\nsections = [fourK, fourtyK, bbexit]\n\nn_trajectories = 100_000\ncoordinates_init = Coordinates(\n    x=np.random.randn(n_trajectories) * 1.5e-3,\n    y=np.random.randn(n_trajectories) * 1.5e-3,\n    z=np.zeros(n_trajectories),\n)\nvelocities_init = Velocities(\n    vx=np.random.randn(n_trajectories) * 39.4,\n    vy=np.random.randn(n_trajectories) * 39.4,\n    vz=np.random.randn(n_trajectories) * 16 + 184,\n)\n\noptions = PropagationOptions(n_cores=6, verbose=False)\ngravity = Force(0, -9.81, 0)\nparticle = TlF()\n\nsection_data, trajectories = propagate_trajectories(\n    sections,\n    coordinates_init,\n    velocities_init,\n    particle,\n    force=gravity,\n    options=options,\n)\n\n```',
+    'long_description': '[![Python versions on PyPI](https://img.shields.io/pypi/pyversions/centrex-trajectories.svg)](https://pypi.python.org/pypi/centrex-trajectories/)\n[![CeNTREX-TlF version on PyPI](https://img.shields.io/pypi/v/centrex-trajectories.svg "CeNTREX-TlF on PyPI")](https://pypi.python.org/pypi/centrex-trajectories/)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n\n\n# CeNTREX-trajectories\nCode for simulating CeNTREX trajectories\n\n## Installation\nClone repo and install with `pip` or directly install from GitHub with:  \n```\npip install git+https://github.com/ograsdijk/CeNTREX-trajectories\n```\n\n## Sections\nThe beamline is split into sections specified with `Section`, which can be used as follows:\n```Python\nsections = [\n    fourK = Section(\n        name = "4K shield",\n        objects = [CircularAperture(x=0, y=0, z=5e-3)],\n        start = 0,\n        stop = 10e-2,\n        save_collisions = False,\n        propagation_type=PropagationType.ballistic,\n    )\n]\n```\nThis defines a section called `4K shield`, which runs from `z = 0 m -> 10e-2 m`. Collisions aren\'t\nsaved, the `propagation_type` is ballistic and it contains a single circular aperture centered around\nthe z axis with a radius of 5 mm.\n\n## Collision objects\nCurrently two type of apertures are defined for collisions:\n* `CircularAperture(x: float,y: float,r: float)`\n* `RectangularAperture(x: float,y: float,wx: float,wy: float)`\n\nCustom collision objects can be defined; apertures should inherit from `Aperture`, and each custom\ncollision object should have two functions:\n* `check_in_bounds(start: float, stop: float)` which returns a boolean specifying whether the object fully resides inside the section\n* `get_acceptance(coordinates: Coordinates)` which returns a boolean arrays specifiying which trajectories make it through the aperture\n\n## Propagation types\nThere is support for ballistic and ODE solver trajectories, which is specified on a per section basis through `Section.propagation_type`\n* `PropagationType.ballistic` assumes a constant velocity and constant gravitational acceleration\n* `PropagationType.ode` needs a defined force function in the section and uses `scipy.integrate.solve_ivp` to calculate the trajectory\n\n## Working example\n```Python\nimport numpy as np\nfrom centrex_trajectories import (\n    Coordinates,\n    Velocities,\n    Force,\n    PropagationType,\n    propagate_trajectories,\n    PropagationOptions,\n)\n\nfrom centrex_trajectories.beamline_objects import CircularAperture, Section\nfrom centrex_trajectories.particles import TlF\n\nin_to_m = 0.0254\n\nfourK = Section(\n    name="4K shield",\n    objects=[CircularAperture(x=0, y=0, z=1.75 * in_to_m, r=1 / 2 * in_to_m)],\n    start=0,\n    stop=2 * in_to_m,\n    save_collisions=False,\n    propagation_type=PropagationType.ballistic,\n)\nfourtyK = Section(\n    name="40K shield",\n    objects=[\n        CircularAperture(x=0, y=0, z=fourK.stop + 1.25 * in_to_m, r=1 / 2 * in_to_m)\n    ],\n    start=fourK.stop,\n    stop=fourK.stop + 1.5 * in_to_m,\n    save_collisions=False,\n    propagation_type=PropagationType.ballistic,\n)\nbbexit = Section(\n    name="Beamsource Exit",\n    objects=[CircularAperture(0, 0, fourtyK.stop + 2.5 * in_to_m, 2 * in_to_m)],\n    start=fourtyK.stop,\n    stop=fourtyK.stop + 3.25 * in_to_m,\n    save_collisions=False,\n    propagation_type=PropagationType.ballistic,\n)\n\nsections = [fourK, fourtyK, bbexit]\n\nn_trajectories = 100_000\ncoordinates_init = Coordinates(\n    x=np.random.randn(n_trajectories) * 1.5e-3,\n    y=np.random.randn(n_trajectories) * 1.5e-3,\n    z=np.zeros(n_trajectories),\n)\nvelocities_init = Velocities(\n    vx=np.random.randn(n_trajectories) * 39.4,\n    vy=np.random.randn(n_trajectories) * 39.4,\n    vz=np.random.randn(n_trajectories) * 16 + 184,\n)\n\noptions = PropagationOptions(n_cores=6, verbose=False)\nparticle = TlF()\ngravity = Force(0, -9.81*particle.mass, 0)\n\nsection_data, trajectories = propagate_trajectories(\n    sections,\n    coordinates_init,\n    velocities_init,\n    particle,\n    force=gravity,\n    options=options,\n)\n\n```',
     'author': 'ograsdijk',
     'author_email': 'o.grasdijk@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `centrex-trajectories-0.2.0/PKG-INFO` & `centrex-trajectories-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: centrex-trajectories
-Version: 0.2.0
+Version: 0.3.0
 Summary: 
 License: MIT
 Author: ograsdijk
 Author-email: o.grasdijk@gmail.com
 Requires-Python: >3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -116,16 +116,16 @@
 velocities_init = Velocities(
     vx=np.random.randn(n_trajectories) * 39.4,
     vy=np.random.randn(n_trajectories) * 39.4,
     vz=np.random.randn(n_trajectories) * 16 + 184,
 )
 
 options = PropagationOptions(n_cores=6, verbose=False)
-gravity = Force(0, -9.81, 0)
 particle = TlF()
+gravity = Force(0, -9.81*particle.mass, 0)
 
 section_data, trajectories = propagate_trajectories(
     sections,
     coordinates_init,
     velocities_init,
     particle,
     force=gravity,
```

