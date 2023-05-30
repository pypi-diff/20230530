# Comparing `tmp/sym_metanet-1.0.5.tar.gz` & `tmp/sym_metanet-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sym_metanet-1.0.5.tar", last modified: Wed Apr  5 14:16:20 2023, max compression
+gzip compressed data, was "sym_metanet-1.0.6.tar", last modified: Tue May 30 13:45:57 2023, max compression
```

## Comparing `sym_metanet-1.0.5.tar` & `sym_metanet-1.0.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-05 14:16:20.548979 sym_metanet-1.0.5/
--rw-rw-rw-   0        0        0     1093 2022-10-27 09:27:26.000000 sym_metanet-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     5929 2023-04-05 14:16:20.547987 sym_metanet-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     5154 2023-02-24 10:16:30.000000 sym_metanet-1.0.5/README.md
--rw-rw-rw-   0        0        0     1058 2023-04-05 14:15:22.000000 sym_metanet-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-05 14:16:20.549977 sym_metanet-1.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-05 14:16:20.488748 sym_metanet-1.0.5/src/
-drwxrwxrwx   0        0        0        0 2023-04-05 14:16:20.507060 sym_metanet-1.0.5/src/sym_metanet/
--rw-rw-rw-   0        0        0     1084 2023-01-11 13:34:25.000000 sym_metanet-1.0.5/src/sym_metanet/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:16:20.526038 sym_metanet-1.0.5/src/sym_metanet/blocks/
--rw-rw-rw-   0        0        0     4463 2023-02-16 11:02:35.000000 sym_metanet-1.0.5/src/sym_metanet/blocks/base.py
--rw-rw-rw-   0        0        0     4105 2023-03-27 10:17:19.000000 sym_metanet-1.0.5/src/sym_metanet/blocks/destinations.py
--rw-rw-rw-   0        0        0     9951 2023-03-27 10:30:41.000000 sym_metanet-1.0.5/src/sym_metanet/blocks/links.py
--rw-rw-rw-   0        0        0     5000 2023-03-27 08:14:57.000000 sym_metanet-1.0.5/src/sym_metanet/blocks/nodes.py
--rw-rw-rw-   0        0        0    10768 2023-03-27 10:30:49.000000 sym_metanet-1.0.5/src/sym_metanet/blocks/origins.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:16:20.536334 sym_metanet-1.0.5/src/sym_metanet/engines/
--rw-rw-rw-   0        0        0      153 2022-11-28 11:51:22.000000 sym_metanet-1.0.5/src/sym_metanet/engines/__init__.py
--rw-rw-rw-   0        0        0    16202 2023-04-05 14:14:32.000000 sym_metanet-1.0.5/src/sym_metanet/engines/casadi.py
--rw-rw-rw-   0        0        0    17360 2023-03-27 09:50:26.000000 sym_metanet-1.0.5/src/sym_metanet/engines/core.py
--rw-rw-rw-   0        0        0     8414 2023-03-27 09:48:46.000000 sym_metanet-1.0.5/src/sym_metanet/engines/numpy.py
--rw-rw-rw-   0        0        0      557 2022-11-28 11:51:22.000000 sym_metanet-1.0.5/src/sym_metanet/errors.py
--rw-rw-rw-   0        0        0    20709 2023-03-27 10:20:52.000000 sym_metanet-1.0.5/src/sym_metanet/network.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:16:20.540316 sym_metanet-1.0.5/src/sym_metanet/util/
--rw-rw-rw-   0        0        0     3620 2022-12-29 23:12:08.000000 sym_metanet-1.0.5/src/sym_metanet/util/funcs.py
--rw-rw-rw-   0        0        0      909 2022-12-30 15:45:07.000000 sym_metanet-1.0.5/src/sym_metanet/util/types.py
--rw-rw-rw-   0        0        0     2066 2022-12-30 15:59:09.000000 sym_metanet-1.0.5/src/sym_metanet/views.py
-drwxrwxrwx   0        0        0        0 2023-04-05 14:16:20.515996 sym_metanet-1.0.5/src/sym_metanet.egg-info/
--rw-rw-rw-   0        0        0     5929 2023-04-05 14:16:20.000000 sym_metanet-1.0.5/src/sym_metanet.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      760 2023-04-05 14:16:20.000000 sym_metanet-1.0.5/src/sym_metanet.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-05 14:16:20.000000 sym_metanet-1.0.5/src/sym_metanet.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-04-05 14:16:20.000000 sym_metanet-1.0.5/src/sym_metanet.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-05 14:16:20.000000 sym_metanet-1.0.5/src/sym_metanet.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-05 14:16:20.545989 sym_metanet-1.0.5/tests/
--rw-rw-rw-   0        0        0     5220 2023-01-11 13:34:26.000000 sym_metanet-1.0.5/tests/test_blocks.py
--rw-rw-rw-   0        0        0    15027 2023-03-27 11:24:15.000000 sym_metanet-1.0.5/tests/test_engines.py
--rw-rw-rw-   0        0        0    11700 2022-12-01 08:54:08.000000 sym_metanet-1.0.5/tests/test_network.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:45:57.881509 sym_metanet-1.0.6/
+-rw-rw-rw-   0        0        0     1093 2022-10-27 09:27:26.000000 sym_metanet-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     6054 2023-05-30 13:45:57.831509 sym_metanet-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     5279 2023-05-25 11:27:33.000000 sym_metanet-1.0.6/README.md
+-rw-rw-rw-   0        0        0     1058 2023-05-25 11:30:18.000000 sym_metanet-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-30 13:45:57.882506 sym_metanet-1.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-30 13:45:57.650478 sym_metanet-1.0.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 13:45:57.698419 sym_metanet-1.0.6/src/sym_metanet/
+-rw-rw-rw-   0        0        0     1084 2023-01-11 13:34:25.000000 sym_metanet-1.0.6/src/sym_metanet/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:45:57.763407 sym_metanet-1.0.6/src/sym_metanet/blocks/
+-rw-rw-rw-   0        0        0     4463 2023-02-16 11:02:35.000000 sym_metanet-1.0.6/src/sym_metanet/blocks/base.py
+-rw-rw-rw-   0        0        0     4353 2023-05-25 09:49:21.000000 sym_metanet-1.0.6/src/sym_metanet/blocks/destinations.py
+-rw-rw-rw-   0        0        0     9951 2023-03-27 10:30:41.000000 sym_metanet-1.0.6/src/sym_metanet/blocks/links.py
+-rw-rw-rw-   0        0        0     5000 2023-03-27 08:14:57.000000 sym_metanet-1.0.6/src/sym_metanet/blocks/nodes.py
+-rw-rw-rw-   0        0        0    10768 2023-03-27 10:30:49.000000 sym_metanet-1.0.6/src/sym_metanet/blocks/origins.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:45:57.775575 sym_metanet-1.0.6/src/sym_metanet/engines/
+-rw-rw-rw-   0        0        0      153 2022-11-28 11:51:22.000000 sym_metanet-1.0.6/src/sym_metanet/engines/__init__.py
+-rw-rw-rw-   0        0        0    16381 2023-05-25 09:43:10.000000 sym_metanet-1.0.6/src/sym_metanet/engines/casadi.py
+-rw-rw-rw-   0        0        0    17963 2023-05-25 09:42:07.000000 sym_metanet-1.0.6/src/sym_metanet/engines/core.py
+-rw-rw-rw-   0        0        0     8605 2023-05-25 09:42:32.000000 sym_metanet-1.0.6/src/sym_metanet/engines/numpy.py
+-rw-rw-rw-   0        0        0      557 2022-11-28 11:51:22.000000 sym_metanet-1.0.6/src/sym_metanet/errors.py
+-rw-rw-rw-   0        0        0    20709 2023-03-27 10:20:52.000000 sym_metanet-1.0.6/src/sym_metanet/network.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:45:57.814518 sym_metanet-1.0.6/src/sym_metanet/util/
+-rw-rw-rw-   0        0        0     3620 2022-12-29 23:12:08.000000 sym_metanet-1.0.6/src/sym_metanet/util/funcs.py
+-rw-rw-rw-   0        0        0      909 2022-12-30 15:45:07.000000 sym_metanet-1.0.6/src/sym_metanet/util/types.py
+-rw-rw-rw-   0        0        0     2066 2022-12-30 15:59:09.000000 sym_metanet-1.0.6/src/sym_metanet/views.py
+drwxrwxrwx   0        0        0        0 2023-05-30 13:45:57.712431 sym_metanet-1.0.6/src/sym_metanet.egg-info/
+-rw-rw-rw-   0        0        0     6054 2023-05-30 13:45:57.000000 sym_metanet-1.0.6/src/sym_metanet.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      760 2023-05-30 13:45:57.000000 sym_metanet-1.0.6/src/sym_metanet.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 13:45:57.000000 sym_metanet-1.0.6/src/sym_metanet.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-30 13:45:57.000000 sym_metanet-1.0.6/src/sym_metanet.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-30 13:45:57.000000 sym_metanet-1.0.6/src/sym_metanet.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 13:45:57.821521 sym_metanet-1.0.6/tests/
+-rw-rw-rw-   0        0        0     5220 2023-01-11 13:34:26.000000 sym_metanet-1.0.6/tests/test_blocks.py
+-rw-rw-rw-   0        0        0    15027 2023-05-25 07:16:50.000000 sym_metanet-1.0.6/tests/test_engines.py
+-rw-rw-rw-   0        0        0    11700 2022-12-01 08:54:08.000000 sym_metanet-1.0.6/tests/test_network.py
```

### Comparing `sym_metanet-1.0.5/LICENSE` & `sym_metanet-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.5/PKG-INFO` & `sym_metanet-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sym_metanet
-Version: 1.0.5
+Version: 1.0.6
 Summary: Symbolic Modelling of Highway Traffic Networks with METANET
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/sym-metanet
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/sym-metanet/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,15 +15,17 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
 
 # Symbolic Modelling of Highway Traffic Networks with METANET
 
-![network-example](examples\example.jpg)
+<div align="center">
+  <img src="https://raw.githubusercontent.com/FilippoAiraldi/sym-metanet/dev/resources/example.jpg" alt="network-example" height="180">
+</div>
 
 **sym-metanet** is a Python package to model traffic networks with the METANET framework, a collection of tools to mathematically model the macroscopic behaviour of traffic in highway systems (see [[1]](#1) and [[2]](#2) for more details).
 
 [![PyPI version](https://badge.fury.io/py/sym-metanet.svg)](https://badge.fury.io/py/sym-metanet)
 [![Source Code License](https://img.shields.io/badge/license-MIT-blueviolet)](https://github.com/FilippoAiraldi/casadi-nlp/blob/release/LICENSE)
 ![Python 3.8](https://img.shields.io/badge/python->=3.8-green.svg)
```

### Comparing `sym_metanet-1.0.5/README.md` & `sym_metanet-1.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Symbolic Modelling of Highway Traffic Networks with METANET
 
-![network-example](examples\example.jpg)
+<div align="center">
+  <img src="https://raw.githubusercontent.com/FilippoAiraldi/sym-metanet/dev/resources/example.jpg" alt="network-example" height="180">
+</div>
 
 **sym-metanet** is a Python package to model traffic networks with the METANET framework, a collection of tools to mathematically model the macroscopic behaviour of traffic in highway systems (see [[1]](#1) and [[2]](#2) for more details).
 
 [![PyPI version](https://badge.fury.io/py/sym-metanet.svg)](https://badge.fury.io/py/sym-metanet)
 [![Source Code License](https://img.shields.io/badge/license-MIT-blueviolet)](https://github.com/FilippoAiraldi/casadi-nlp/blob/release/LICENSE)
 ![Python 3.8](https://img.shields.io/badge/python->=3.8-green.svg)
```

### Comparing `sym_metanet-1.0.5/pyproject.toml` & `sym_metanet-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sym_metanet"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Filippo Airaldi", email="filippoairaldi@gmail.com" },
 ]
 description = "Symbolic Modelling of Highway Traffic Networks with METANET"
 readme = "README.md"
 requires-python = ">=3.8"
 license = { text = "MIT" }
```

### Comparing `sym_metanet-1.0.5/src/sym_metanet/__init__.py` & `sym_metanet-1.0.6/src/sym_metanet/__init__.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.5/src/sym_metanet/blocks/base.py` & `sym_metanet-1.0.6/src/sym_metanet/blocks/base.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.5/src/sym_metanet/blocks/destinations.py` & `sym_metanet-1.0.6/src/sym_metanet/blocks/destinations.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,28 +18,35 @@
     def init_vars(self, *_, **__) -> None:
         """Initializes no variable in the ideal destination."""
 
     def step_dynamics(self, *_, **__) -> Dict[str, VarType]:
         """No dynamics to steps in the ideal destination."""
         return {}
 
-    def get_density(self, net: "Network", **_) -> VarType:
+    def get_density(
+        self, net: "Network", engine: Optional[EngineBase] = None, **_
+    ) -> VarType:
         """Computes the (downstream) density induced by the ideal destination.
 
         Parameters
         ----------
         net : Network
             The network this destination belongs to.
 
         Returns
         -------
         symbolic variable
             The destination's downstream density.
         """
-        return self._get_entering_link(net).states["rho"][-1]
+        if engine is None:
+            engine = get_current_engine()
+        link_up = self._get_entering_link(net)
+        return engine.destinations.get_congestion_free_downstream_density(
+            link_up.states["rho"][-1], link_up.rho_crit
+        )
 
     def _get_entering_link(self, net: "Network") -> "Link[VarType]":
         """Internal utility to fetch the link entering this destination (can only be
         one)."""
         links_up: Collection[Tuple["Node", "Node", "Link[VarType]"]] = net.in_links(
             net.destinations[self]  # type: ignore[index]
         )
@@ -82,15 +89,15 @@
         self.disturbances: Dict[str, VarType] = {
             "d": engine.var(f"d_{self.name}")
             if init_conditions is None or "d" not in init_conditions
             else init_conditions["d"]
         }
 
     def get_density(
-        self, net: "Network", engine: Optional[EngineBase] = None, **kwargs
+        self, net: "Network", engine: Optional[EngineBase] = None, **_
     ) -> VarType:
         """Computes the (downstream) density induced by the congested destination.
 
         Parameters
         ----------
         net : Network
             The network this destination belongs to.
```

### Comparing `sym_metanet-1.0.5/src/sym_metanet/blocks/links.py` & `sym_metanet-1.0.6/src/sym_metanet/blocks/links.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.5/src/sym_metanet/blocks/nodes.py` & `sym_metanet-1.0.6/src/sym_metanet/blocks/nodes.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.5/src/sym_metanet/blocks/origins.py` & `sym_metanet-1.0.6/src/sym_metanet/blocks/origins.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.5/src/sym_metanet/engines/casadi.py` & `sym_metanet-1.0.6/src/sym_metanet/engines/casadi.py`

 * *Files 0% similar despite different names*

```diff
@@ -149,14 +149,20 @@
         return cs.fmin(qdes, cs.fmin(term2, term3))
 
 
 class DestinationsEngine(DestinationsEngineBase, Generic[VarType]):
     """CasADi implementation of `sym_metanet.engines.core.DestinationsEngineBase`."""
 
     @staticmethod
+    def get_congestion_free_downstream_density(
+        rho_last: VarType, rho_crit: VarType
+    ) -> VarType:
+        return cs.fmin(rho_last, rho_crit)
+
+    @staticmethod
     def get_congested_downstream_density(
         rho_last: VarType, rho_destination: VarType, rho_crit: VarType
     ) -> VarType:
         return cs.fmax(cs.fmin(rho_last, rho_crit), rho_destination)
 
 
 class Engine(EngineBase, Generic[VarType]):
```

### Comparing `sym_metanet-1.0.5/src/sym_metanet/engines/core.py` & `sym_metanet-1.0.6/src/sym_metanet/engines/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -367,14 +367,34 @@
     ----------
     [1] Hegyi, A., 2004, "Model predictive control for integrating traffic control
         measures", Netherlands TRAIL Research School.
     """
 
     @staticmethod
     @abstractmethod
+    def get_congestion_free_downstream_density(rho_last, rho_crit):
+        """For a link with a downstream destination with no congestion, i.e., ideal,
+        returns the downstream density.
+
+        Parameters
+        ----------
+        rho_last
+            Density in the link's last segment.
+        rho_crit
+            Critical density of the link entering the destination.
+
+        Returns
+        -------
+        density
+            The downstream density for a link connected to a congestion-free
+            destination.
+        """
+
+    @staticmethod
+    @abstractmethod
     def get_congested_downstream_density(rho_last, rho_destination, rho_crit):
         """For a link with a downstream congested destination, returns the downstream
         density.
 
         Parameters
         ----------
         rho_last
```

### Comparing `sym_metanet-1.0.5/src/sym_metanet/engines/numpy.py` & `sym_metanet-1.0.6/src/sym_metanet/engines/numpy.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,20 @@
 
 class DestinationsEngine(DestinationsEngineBase):
     """
     NumPy implementation of `sym_metanet.engines.core.DestinationsEngineBase`.
     """
 
     @staticmethod
+    def get_congestion_free_downstream_density(
+        rho_last: np.ndarray, rho_crit: np.ndarray
+    ) -> np.ndarray:
+        return np.minimum(rho_last, rho_crit)
+
+    @staticmethod
     def get_congested_downstream_density(
         rho_last: np.ndarray, rho_destination: np.ndarray, rho_crit: np.ndarray
     ) -> np.ndarray:
         return np.maximum(np.minimum(rho_last, rho_crit), rho_destination)
 
 
 class Engine(EngineBase):
```

### Comparing `sym_metanet-1.0.5/src/sym_metanet/errors.py` & `sym_metanet-1.0.6/src/sym_metanet/errors.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.5/src/sym_metanet/network.py` & `sym_metanet-1.0.6/src/sym_metanet/network.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.5/src/sym_metanet/util/funcs.py` & `sym_metanet-1.0.6/src/sym_metanet/util/funcs.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.5/src/sym_metanet/util/types.py` & `sym_metanet-1.0.6/src/sym_metanet/util/types.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.5/src/sym_metanet/views.py` & `sym_metanet-1.0.6/src/sym_metanet/views.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.5/src/sym_metanet.egg-info/PKG-INFO` & `sym_metanet-1.0.6/src/sym_metanet.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sym-metanet
-Version: 1.0.5
+Version: 1.0.6
 Summary: Symbolic Modelling of Highway Traffic Networks with METANET
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/sym-metanet
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/sym-metanet/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -15,15 +15,17 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
 
 # Symbolic Modelling of Highway Traffic Networks with METANET
 
-![network-example](examples\example.jpg)
+<div align="center">
+  <img src="https://raw.githubusercontent.com/FilippoAiraldi/sym-metanet/dev/resources/example.jpg" alt="network-example" height="180">
+</div>
 
 **sym-metanet** is a Python package to model traffic networks with the METANET framework, a collection of tools to mathematically model the macroscopic behaviour of traffic in highway systems (see [[1]](#1) and [[2]](#2) for more details).
 
 [![PyPI version](https://badge.fury.io/py/sym-metanet.svg)](https://badge.fury.io/py/sym-metanet)
 [![Source Code License](https://img.shields.io/badge/license-MIT-blueviolet)](https://github.com/FilippoAiraldi/casadi-nlp/blob/release/LICENSE)
 ![Python 3.8](https://img.shields.io/badge/python->=3.8-green.svg)
```

### Comparing `sym_metanet-1.0.5/src/sym_metanet.egg-info/SOURCES.txt` & `sym_metanet-1.0.6/src/sym_metanet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.5/tests/test_blocks.py` & `sym_metanet-1.0.6/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.5/tests/test_engines.py` & `sym_metanet-1.0.6/tests/test_engines.py`

 * *Files identical despite different names*

### Comparing `sym_metanet-1.0.5/tests/test_network.py` & `sym_metanet-1.0.6/tests/test_network.py`

 * *Files identical despite different names*

