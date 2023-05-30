# Comparing `tmp/popcast-1.0.1.tar.gz` & `tmp/popcast-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "popcast-1.0.1.tar", last modified: Thu Sep  1 19:45:51 2022, max compression
+gzip compressed data, was "popcast-1.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `popcast-1.0.1.tar` & `popcast-1.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1074 2022-08-02 04:18:03.259971 popcast-1.0.1/LICENSE
--rw-r--r--   0        0        0     1184 2022-09-01 18:55:56.434346 popcast-1.0.1/README.md
--rw-r--r--   0        0        0     1585 2022-09-01 19:44:11.067626 popcast-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      127 2022-08-31 22:46:23.326589 popcast-1.0.1/src/popcast/__init__.py
--rw-r--r--   0        0        0      959 2022-08-31 22:46:03.215894 popcast-1.0.1/src/popcast/cli.py
--rw-r--r--   0        0        0     4239 2022-08-02 06:24:02.937061 popcast-1.0.1/src/popcast/cross_immunity.py
--rw-r--r--   0        0        0    49134 2022-08-17 22:32:41.934350 popcast-1.0.1/src/popcast/fit.py
--rw-r--r--   0        0        0     6517 2022-08-02 22:03:44.302243 popcast-1.0.1/src/popcast/forecast.py
--rw-r--r--   0        0        0     5557 2022-08-02 06:24:02.939122 popcast-1.0.1/src/popcast/metrics.py
--rw-r--r--   0        0        0       19 2022-08-02 18:18:18.888013 popcast-1.0.1/src/popcast/nextcast.py
--rw-r--r--   0        0        0    10248 2022-08-02 06:24:02.940816 popcast-1.0.1/src/popcast/utils.py
--rw-r--r--   0        0        0     5791 2022-08-02 06:24:02.941362 popcast-1.0.1/src/popcast/weighted_distances.py
--rw-r--r--   0        0        0     2133 1970-01-01 00:00:00.000000 popcast-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-30 21:10:04.813148 popcast-1.0.2/LICENSE
+-rw-r--r--   0        0        0     1186 2023-05-30 21:35:27.567073 popcast-1.0.2/README.md
+-rw-r--r--   0        0        0     1585 2023-05-30 21:42:24.191854 popcast-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0      127 2023-05-30 21:42:47.088510 popcast-1.0.2/src/popcast/__init__.py
+-rw-r--r--   0        0        0      959 2023-05-30 21:10:04.813609 popcast-1.0.2/src/popcast/cli.py
+-rw-r--r--   0        0        0     4239 2023-05-30 21:10:04.813713 popcast-1.0.2/src/popcast/cross_immunity.py
+-rw-r--r--   0        0        0    49134 2023-05-30 21:10:04.813981 popcast-1.0.2/src/popcast/fit.py
+-rw-r--r--   0        0        0     6594 2023-05-30 21:35:27.567709 popcast-1.0.2/src/popcast/forecast.py
+-rw-r--r--   0        0        0     5557 2023-05-30 21:10:04.814204 popcast-1.0.2/src/popcast/metrics.py
+-rw-r--r--   0        0        0       19 2023-05-30 21:10:04.814295 popcast-1.0.2/src/popcast/nextcast.py
+-rw-r--r--   0        0        0    10248 2023-05-30 21:10:04.814419 popcast-1.0.2/src/popcast/utils.py
+-rw-r--r--   0        0        0     5791 2023-05-30 21:10:04.814523 popcast-1.0.2/src/popcast/weighted_distances.py
+-rw-r--r--   0        0        0     2135 1970-01-01 00:00:00.000000 popcast-1.0.2/PKG-INFO
```

### Comparing `popcast-1.0.1/LICENSE` & `popcast-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `popcast-1.0.1/README.md` & `popcast-1.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ```
 
 ## Development
 
 ### Install locally
 
 ``` bash
-python3 -m pip install .[test]
+python3 -m pip install ".[test]"
 ```
 
 ### Lint and run tests
 
 Lint code.
 
 ``` bash
```

### Comparing `popcast-1.0.1/pyproject.toml` & `popcast-1.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.2"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "popcast"
-version = "1.0.1"
+version = "1.0.2"
 authors = [
   { name="John Huddleston", email="huddlej@gmail.com" },
 ]
 description = "Long-term forecasts for pathogen populations"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.6"
```

### Comparing `popcast-1.0.1/src/popcast/cli.py` & `popcast-1.0.2/src/popcast/cli.py`

 * *Files identical despite different names*

### Comparing `popcast-1.0.1/src/popcast/cross_immunity.py` & `popcast-1.0.2/src/popcast/cross_immunity.py`

 * *Files identical despite different names*

### Comparing `popcast-1.0.1/src/popcast/fit.py` & `popcast-1.0.2/src/popcast/fit.py`

 * *Files identical despite different names*

### Comparing `popcast-1.0.1/src/popcast/forecast.py` & `popcast-1.0.2/src/popcast/forecast.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,19 +130,20 @@
         strain_to_projected_frequency = {}
         for index, row in forecasts_df.iterrows():
             strain_to_projected_frequency[row['strain']] = row['projected_frequency']
 
         if frequencies is not None:
             # extend frequencies
             for strain in frequencies.keys():
-                trajectory = frequencies[strain]['frequencies']
-                if strain in strain_to_projected_frequency:
-                    trajectory.append(strain_to_projected_frequency[strain])
-                else:
-                    trajectory.append(0.0)
+                if "frequencies" in frequencies[strain]:
+                    trajectory = frequencies[strain]['frequencies']
+                    if strain in strain_to_projected_frequency:
+                        trajectory.append(strain_to_projected_frequency[strain])
+                    else:
+                        trajectory.append(0.0)
 
             # extend pivots
             pivots.append(projection_pivot + delta_time)
 
         # Collect forecast data frames, if requested.
         if args.output_table:
             forecasts.append(forecasts_df)
```

### Comparing `popcast-1.0.1/src/popcast/metrics.py` & `popcast-1.0.2/src/popcast/metrics.py`

 * *Files identical despite different names*

### Comparing `popcast-1.0.1/src/popcast/utils.py` & `popcast-1.0.2/src/popcast/utils.py`

 * *Files identical despite different names*

### Comparing `popcast-1.0.1/src/popcast/weighted_distances.py` & `popcast-1.0.2/src/popcast/weighted_distances.py`

 * *Files identical despite different names*

### Comparing `popcast-1.0.1/PKG-INFO` & `popcast-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: popcast
-Version: 1.0.1
+Version: 1.0.2
 Summary: Long-term forecasts for pathogen populations
 Author-email: John Huddleston <huddlej@gmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -49,15 +49,15 @@
 ```
 
 ## Development
 
 ### Install locally
 
 ``` bash
-python3 -m pip install .[test]
+python3 -m pip install ".[test]"
 ```
 
 ### Lint and run tests
 
 Lint code.
 
 ``` bash
```

