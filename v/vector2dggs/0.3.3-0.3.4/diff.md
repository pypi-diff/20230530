# Comparing `tmp/vector2dggs-0.3.3.tar.gz` & `tmp/vector2dggs-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector2dggs-0.3.3.tar", max compression
+gzip compressed data, was "vector2dggs-0.3.4.tar", max compression
```

## Comparing `vector2dggs-0.3.3.tar` & `vector2dggs-0.3.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     8006 2023-05-30 03:13:02.078140 vector2dggs-0.3.3/README.md
--rw-r--r--   0        0        0     1092 2023-05-30 03:13:02.094141 vector2dggs-0.3.3/pyproject.toml
--rw-r--r--   0        0        0       27 2023-05-02 23:30:16.752288 vector2dggs-0.3.3/vector2dggs/__init__.py
--rw-r--r--   0        0        0      599 2023-05-02 23:30:16.752288 vector2dggs-0.3.3/vector2dggs/cli.py
--rw-r--r--   0        0        0    12638 2023-05-30 03:13:02.110141 vector2dggs-0.3.3/vector2dggs/h3.py
--rw-r--r--   0        0        0     3173 2023-05-22 02:20:32.367257 vector2dggs-0.3.3/vector2dggs/katana.py
--rw-r--r--   0        0        0     9440 1970-01-01 00:00:00.000000 vector2dggs-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     8208 2023-05-30 03:31:45.583819 vector2dggs-0.3.4/README.md
+-rw-r--r--   0        0        0     1092 2023-05-30 03:31:50.231842 vector2dggs-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-05-02 23:30:16.752288 vector2dggs-0.3.4/vector2dggs/__init__.py
+-rw-r--r--   0        0        0      599 2023-05-02 23:30:16.752288 vector2dggs-0.3.4/vector2dggs/cli.py
+-rw-r--r--   0        0        0    13018 2023-05-30 03:31:02.319601 vector2dggs-0.3.4/vector2dggs/h3.py
+-rw-r--r--   0        0        0     3173 2023-05-22 02:20:32.367257 vector2dggs-0.3.4/vector2dggs/katana.py
+-rw-r--r--   0        0        0     9642 1970-01-01 00:00:00.000000 vector2dggs-0.3.4/PKG-INFO
```

### Comparing `vector2dggs-0.3.3/README.md` & `vector2dggs-0.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,17 @@
   the write location for an Apache Parquet data store.
 
 Options:
   -v, --verbosity LVL             Either CRITICAL, ERROR, WARNING, INFO or
                                   DEBUG  [default: INFO]
   -r, --resolution [0|1|2|3|4|5|6|7|8|9|10|11|12|13|14|15]
                                   H3 resolution to index  [required]
+  -pr, --parent_res [0|1|2|3|4|5|6|7|8|9|10|11|12|13|14|15]
+                                  H3 Parent resolution for the output
+                                  partition. Defaults to resolution - 6
   -id, --id_field TEXT            Field to use as an ID; defaults to a
                                   constructed single 0...n index on the
                                   original feature order.
   -k, --keep_attributes           Retain attributes in output. The default is
                                   to create an output that only includes H3
                                   cell ID and the ID given by the -id field
                                   (or the default index ID).
@@ -148,17 +151,17 @@
 ## Citation
 
 ```bibtex
 @software{vector2dggs,
   title={{vector2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/vector2dggs},
-  version={0.3.3},
+  version={0.3.4},
   date={2023-04-20}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). vector2dggs (0.3.3) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
+> Ardo, J., & Law, R. (2023). vector2dggs (0.3.4) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/vector2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

### Comparing `vector2dggs-0.3.3/pyproject.toml` & `vector2dggs-0.3.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vector2dggs"
-version = "0.3.3"
+version = "0.3.4"
 description = "CLI DGGS indexer for vector geospatial data"
 authors = ["James Ardo <ardoj@landcareresearch.co.nz>"]
 maintainers = ["Richard Law <lawr@landcareresearch.co.nz>"]
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 repository = "https://github.com/manaakiwhenua/vector2dggs"
 keywords = ["dggs", "vector", "h3", "cli"]
```

### Comparing `vector2dggs-0.3.3/vector2dggs/cli.py` & `vector2dggs-0.3.4/vector2dggs/cli.py`

 * *Files identical despite different names*

### Comparing `vector2dggs-0.3.3/vector2dggs/h3.py` & `vector2dggs-0.3.4/vector2dggs/h3.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import errno
 import logging
 import os
 import multiprocessing
 from multiprocessing.dummy import Pool
 from pathlib import Path, PurePath
 import shutil
+import sys
 import tempfile
 from typing import Union
 from urllib.parse import urlparse
 import warnings
 
 os.environ["USE_PYGEOS"] = "0"
 
@@ -39,14 +40,16 @@
 
 DEFAULT_PARENT_OFFSET = 6
 
 
 class ParentResolutionException(Exception):
     pass
 
+class EmptyDataException(Exception):
+    pass
 
 def _get_parent_res(parent_res: Union[None, int], resolution: int):
     """
     Uses a parent resolution,
     OR,
     Given a target resolution, returns our recommended parent resolution.
 
@@ -106,14 +109,17 @@
         ddf = dd.read_parquet(input_dir, engine="pyarrow").set_index(
             f"h3_{parent_res:02}"
         )
     with TqdmCallback(desc="Counting parents"):
         # Count parents, to get target number of partitions
         uniqueh3 = sorted(list(ddf.index.unique().compute()))
 
+    if not len(uniqueh3):
+        raise EmptyDataException('No data to write; input data appears empty. Requested output "{output_dir}" will not be written.'.format(output_dir=output_dir))
+
     LOGGER.debug(
         "Repartitioning into %d partitions, based on parent cells",
         len(uniqueh3) + 1,
     )
 
     with TqdmCallback(desc="Repartitioning"):
         ddf = (
@@ -393,24 +399,29 @@
         LOGGER.info(f"Overwriting the contents of {output_directory}")
         shutil.rmtree(output_directory)
     output_directory.mkdir(parents=True, exist_ok=True)
 
     if cut_crs is not None:
         cut_crs = pyproj.CRS.from_user_input(cut_crs)
 
-    _index(
-        vector_input,
-        output_directory,
-        int(resolution),
-        parent_res,
-        keep_attributes,
-        partitions,
-        spatial_sorting,
-        cut_threshold,
-        threads,
-        cut_crs=cut_crs,
-        id_field=id_field,
-        con=con,
-        table=table,
-        geom_col=geom_col,
-        overwrite=overwrite,
-    )
+    try:
+        _index(
+            vector_input,
+            output_directory,
+            int(resolution),
+            parent_res,
+            keep_attributes,
+            partitions,
+            spatial_sorting,
+            cut_threshold,
+            threads,
+            cut_crs=cut_crs,
+            id_field=id_field,
+            con=con,
+            table=table,
+            geom_col=geom_col,
+            overwrite=overwrite,
+        )
+    except:
+        raise
+    else:
+        sys.exit(0)
```

### Comparing `vector2dggs-0.3.3/vector2dggs/katana.py` & `vector2dggs-0.3.4/vector2dggs/katana.py`

 * *Files identical despite different names*

### Comparing `vector2dggs-0.3.3/PKG-INFO` & `vector2dggs-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector2dggs
-Version: 0.3.3
+Version: 0.3.4
 Summary: CLI DGGS indexer for vector geospatial data
 Home-page: https://github.com/manaakiwhenua/vector2dggs
 License: LGPL-3.0-or-later
 Keywords: dggs,vector,h3,cli
 Author: James Ardo
 Author-email: ardoj@landcareresearch.co.nz
 Maintainer: Richard Law
@@ -66,14 +66,17 @@
   the write location for an Apache Parquet data store.
 
 Options:
   -v, --verbosity LVL             Either CRITICAL, ERROR, WARNING, INFO or
                                   DEBUG  [default: INFO]
   -r, --resolution [0|1|2|3|4|5|6|7|8|9|10|11|12|13|14|15]
                                   H3 resolution to index  [required]
+  -pr, --parent_res [0|1|2|3|4|5|6|7|8|9|10|11|12|13|14|15]
+                                  H3 Parent resolution for the output
+                                  partition. Defaults to resolution - 6
   -id, --id_field TEXT            Field to use as an ID; defaults to a
                                   constructed single 0...n index on the
                                   original feature order.
   -k, --keep_attributes           Retain attributes in output. The default is
                                   to create an output that only includes H3
                                   cell ID and the ID given by the -id field
                                   (or the default index ID).
@@ -183,18 +186,18 @@
 ## Citation
 
 ```bibtex
 @software{vector2dggs,
   title={{vector2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/vector2dggs},
-  version={0.3.3},
+  version={0.3.4},
   date={2023-04-20}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). vector2dggs (0.3.3) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
+> Ardo, J., & Law, R. (2023). vector2dggs (0.3.4) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/vector2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

