# Comparing `tmp/vector2dggs-0.3.2.tar.gz` & `tmp/vector2dggs-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector2dggs-0.3.2.tar", max compression
+gzip compressed data, was "vector2dggs-0.3.3.tar", max compression
```

## Comparing `vector2dggs-0.3.2.tar` & `vector2dggs-0.3.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     8006 2023-05-22 02:22:17.187783 vector2dggs-0.3.2/README.md
--rw-r--r--   0        0        0     1092 2023-05-22 02:20:46.867330 vector2dggs-0.3.2/pyproject.toml
--rw-r--r--   0        0        0       27 2023-05-02 23:30:16.752288 vector2dggs-0.3.2/vector2dggs/__init__.py
--rw-r--r--   0        0        0      599 2023-05-02 23:30:16.752288 vector2dggs-0.3.2/vector2dggs/cli.py
--rw-r--r--   0        0        0     9400 2023-05-22 02:22:11.423754 vector2dggs-0.3.2/vector2dggs/h3.py
--rw-r--r--   0        0        0     3173 2023-05-22 02:20:32.367257 vector2dggs-0.3.2/vector2dggs/katana.py
--rw-r--r--   0        0        0     9440 1970-01-01 00:00:00.000000 vector2dggs-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     8006 2023-05-30 03:13:02.078140 vector2dggs-0.3.3/README.md
+-rw-r--r--   0        0        0     1092 2023-05-30 03:13:02.094141 vector2dggs-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0       27 2023-05-02 23:30:16.752288 vector2dggs-0.3.3/vector2dggs/__init__.py
+-rw-r--r--   0        0        0      599 2023-05-02 23:30:16.752288 vector2dggs-0.3.3/vector2dggs/cli.py
+-rw-r--r--   0        0        0    12638 2023-05-30 03:13:02.110141 vector2dggs-0.3.3/vector2dggs/h3.py
+-rw-r--r--   0        0        0     3173 2023-05-22 02:20:32.367257 vector2dggs-0.3.3/vector2dggs/katana.py
+-rw-r--r--   0        0        0     9440 1970-01-01 00:00:00.000000 vector2dggs-0.3.3/PKG-INFO
```

### Comparing `vector2dggs-0.3.2/README.md` & `vector2dggs-0.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -148,17 +148,17 @@
 ## Citation
 
 ```bibtex
 @software{vector2dggs,
   title={{vector2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/vector2dggs},
-  version={0.3.2},
+  version={0.3.3},
   date={2023-04-20}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). vector2dggs (0.3.2) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
+> Ardo, J., & Law, R. (2023). vector2dggs (0.3.3) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/vector2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

### Comparing `vector2dggs-0.3.2/pyproject.toml` & `vector2dggs-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vector2dggs"
-version = "0.3.2"
+version = "0.3.3"
 description = "CLI DGGS indexer for vector geospatial data"
 authors = ["James Ardo <ardoj@landcareresearch.co.nz>"]
 maintainers = ["Richard Law <lawr@landcareresearch.co.nz>"]
 readme = "README.md"
 license = "LGPL-3.0-or-later"
 repository = "https://github.com/manaakiwhenua/vector2dggs"
 keywords = ["dggs", "vector", "h3", "cli"]
```

### Comparing `vector2dggs-0.3.2/vector2dggs/cli.py` & `vector2dggs-0.3.3/vector2dggs/cli.py`

 * *Files identical despite different names*

### Comparing `vector2dggs-0.3.2/vector2dggs/h3.py` & `vector2dggs-0.3.3/vector2dggs/h3.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,55 +33,130 @@
 MIN_H3, MAX_H3 = 0, 15
 
 warnings.filterwarnings(
     "ignore"
 )  # This is to filter out the polyfill warnings when rows failed to get indexed at a resolution, can be commented out to find missing rows
 
 
+DEFAULT_PARENT_OFFSET = 6
+
+
+class ParentResolutionException(Exception):
+    pass
+
+
+def _get_parent_res(parent_res: Union[None, int], resolution: int):
+    """
+    Uses a parent resolution,
+    OR,
+    Given a target resolution, returns our recommended parent resolution.
+
+    Used for intermediate re-partioning.
+    """
+    return (
+        int(parent_res)
+        if parent_res is not None
+        else max(MIN_H3, (resolution - DEFAULT_PARENT_OFFSET))
+    )
+
+
 def polyfill(
-    pq_in: Path, spatial_sort_col: str, resolution: int, output_directory: str
+    pq_in: Path,
+    spatial_sort_col: str,
+    resolution: int,
+    parent_res: Union[None, int],
+    output_directory: str,
 ) -> None:
     """
     Reads a geoparquet, performs H3 polyfilling,
     and writes out to parquet.
     """
     df = (
         gpd.read_parquet(pq_in)
         .reset_index()
         .drop(columns=[spatial_sort_col])
         .h3.polyfill_resample(resolution, return_geometry=False)
     )
     df = pd.DataFrame(df).drop(columns=["index", "geometry"])
     df.index.rename(f"h3_{resolution:02}", inplace=True)
+    parent_res: int = _get_parent_res(parent_res, resolution)
+    # Secondary (parent) H3 index, used later for partitioning
+    df = df.h3.h3_to_parent(parent_res).reset_index()
     df.to_parquet(
         PurePath(output_directory, pq_in.name),
         engine="auto",
         compression="ZSTD",
     )
     return None
 
 
-def polyfill_star(args):
+def polyfill_star(args) -> None:
     return polyfill(*args)
 
 
+def _parent_partitioning(
+    input_dir: Path,
+    output_dir: Path,
+    resolution,
+    parent_res: Union[None, int],
+    **kwargs,
+) -> Path:
+    parent_res: int = _get_parent_res(parent_res, resolution)
+    with TqdmCallback(desc="Reading spatial partitions"):
+        # Set index as parent cell
+        ddf = dd.read_parquet(input_dir, engine="pyarrow").set_index(
+            f"h3_{parent_res:02}"
+        )
+    with TqdmCallback(desc="Counting parents"):
+        # Count parents, to get target number of partitions
+        uniqueh3 = sorted(list(ddf.index.unique().compute()))
+
+    LOGGER.debug(
+        "Repartitioning into %d partitions, based on parent cells",
+        len(uniqueh3) + 1,
+    )
+
+    with TqdmCallback(desc="Repartitioning"):
+        ddf = (
+            ddf.repartition(  # See "notes" on why divisions expects repetition of the last item https://docs.dask.org/en/stable/generated/dask.dataframe.DataFrame.repartition.html
+                divisions=(uniqueh3 + [uniqueh3[-1]]), force=True
+            )
+            .reset_index()
+            .set_index(f"h3_{resolution:02}")
+            .drop(columns=[f"h3_{parent_res:02}"])
+            .to_parquet(
+                output_dir,
+                overwrite=kwargs.get("overwrite", False),
+                engine=kwargs.get("engine", "pyarrow"),
+                write_index=True,
+                # append=False,
+                name_function=lambda i: f"{uniqueh3[i]}.parquet",
+                compression=kwargs.get("compression", "ZSTD"),
+            )
+        )
+    LOGGER.debug("Parent cell repartitioning complete")
+    return output_dir
+
+
 def _index(
     input_file: Union[Path, str],
     output_directory: Union[Path, str],
     resolution: int,
+    parent_res: Union[None, int],
     keep_attributes: bool,
     npartitions: int,
     spatial_sorting: str,
     cut_threshold: int,
     processes: int,
     id_field: str = None,
     cut_crs: pyproj.CRS = None,
     con: Union[sqlalchemy.engine.Connection, sqlalchemy.engine.Engine] = None,
     table: str = None,
     geom_col: str = "geom",
+    overwrite: bool = False,
 ) -> Path:
     """
     Performs multi-threaded H3 polyfilling on (multi)polygons.
     """
 
     if table and con:
         # Database connection
@@ -134,31 +209,38 @@
     ddf = ddf.spatial_shuffle(by=spatial_sorting)
     spatial_sort_col = (
         spatial_sorting
         if spatial_sorting == "geohash"
         else f"{spatial_sorting}_distance"
     )
 
-    with tempfile.TemporaryDirectory() as tmpdir:
+    with tempfile.TemporaryDirectory(suffix=".parquet") as tmpdir:
         with TqdmCallback():
             ddf.to_parquet(tmpdir, overwrite=True)
 
         filepaths = list(map(lambda f: f.absolute(), Path(tmpdir).glob("*")))
 
         # Multithreaded polyfilling
         LOGGER.info(
             "H3 Indexing on spatial partitions by polyfill with H3 resolution: %d",
             resolution,
         )
-        with Pool(processes=processes) as pool:
-            args = [
-                (filepath, spatial_sort_col, resolution, output_directory)
-                for filepath in filepaths
-            ]
-            list(tqdm(pool.imap(polyfill_star, args), total=len(args)))
+        with tempfile.TemporaryDirectory(suffix=".parquet") as tmpdir2:
+            with Pool(processes=processes) as pool:
+                args = [
+                    (filepath, spatial_sort_col, resolution, parent_res, tmpdir2)
+                    for filepath in filepaths
+                ]
+                list(tqdm(pool.imap(polyfill_star, args), total=len(args)))
+
+            output_directory = _parent_partitioning(
+                tmpdir2, output_directory, resolution, parent_res, overwrite=overwrite
+            )
+
+    return output_directory
 
 
 @click.command(context_settings={"show_default": True})
 @click_log.simple_verbosity_option(LOGGER)
 @click.argument("vector_input", required=True, type=click.Path(), nargs=1)
 @click.argument("output_directory", required=True, type=click.Path(), nargs=1)
 @click.option(
@@ -166,14 +248,21 @@
     "--resolution",
     required=True,
     type=click.Choice(list(map(str, range(MIN_H3, MAX_H3 + 1)))),
     help="H3 resolution to index",
     nargs=1,
 )
 @click.option(
+    "-pr",
+    "--parent_res",
+    required=False,
+    type=click.Choice(list(map(str, range(MIN_H3, MAX_H3 + 1)))),
+    help="H3 Parent resolution for the output partition. Defaults to resolution - 6",
+)
+@click.option(
     "-id",
     "--id_field",
     required=False,
     default=None,
     type=str,
     help="Field to use as an ID; defaults to a constructed single 0...n index on the original feature order.",
     nargs=1,
@@ -249,14 +338,15 @@
 )
 @click.option("-o", "--overwrite", is_flag=True)
 @click.version_option(version=__version__)
 def h3(
     vector_input: Union[str, Path],
     output_directory: Union[str, Path],
     resolution: str,
+    parent_res: str,
     id_field: str,
     keep_attributes: bool,
     partitions: int,
     spatial_sorting: str,
     cut_crs: int,
     cut_threshold: int,
     threads: int,
@@ -266,14 +356,20 @@
 ):
     """
     Ingest a vector dataset and index it to the H3 DGGS.
 
     VECTOR_INPUT is the path to input vector geospatial data.
     OUTPUT_DIRECTORY should be a directory, not a file or database table, as it will instead be the write location for an Apache Parquet data store.
     """
+    if parent_res is not None and not int(parent_res) < int(resolution):
+        raise ParentResolutionException(
+            "Parent resolution ({pr}) must be less than target resolution ({r})".format(
+                pr=parent_res, r=resolution
+            )
+        )
     con: sqlalchemy.engine.Connection = None
     scheme: str = urlparse(vector_input).scheme
     if bool(scheme) and scheme != "file":
         # Assume database connection
         con = sqlalchemy.create_engine(vector_input)
     elif not Path(vector_input).exists():
         if not scheme:
@@ -301,18 +397,20 @@
     if cut_crs is not None:
         cut_crs = pyproj.CRS.from_user_input(cut_crs)
 
     _index(
         vector_input,
         output_directory,
         int(resolution),
+        parent_res,
         keep_attributes,
         partitions,
         spatial_sorting,
         cut_threshold,
         threads,
         cut_crs=cut_crs,
         id_field=id_field,
         con=con,
         table=table,
         geom_col=geom_col,
+        overwrite=overwrite,
     )
```

### Comparing `vector2dggs-0.3.2/vector2dggs/katana.py` & `vector2dggs-0.3.3/vector2dggs/katana.py`

 * *Files identical despite different names*

### Comparing `vector2dggs-0.3.2/PKG-INFO` & `vector2dggs-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector2dggs
-Version: 0.3.2
+Version: 0.3.3
 Summary: CLI DGGS indexer for vector geospatial data
 Home-page: https://github.com/manaakiwhenua/vector2dggs
 License: LGPL-3.0-or-later
 Keywords: dggs,vector,h3,cli
 Author: James Ardo
 Author-email: ardoj@landcareresearch.co.nz
 Maintainer: Richard Law
@@ -183,18 +183,18 @@
 ## Citation
 
 ```bibtex
 @software{vector2dggs,
   title={{vector2dggs}},
   author={Ardo, James and Law, Richard},
   url={https://github.com/manaakiwhenua/vector2dggs},
-  version={0.3.2},
+  version={0.3.3},
   date={2023-04-20}
 }
 ```
 
 APA/Harvard
 
-> Ardo, J., & Law, R. (2023). vector2dggs (0.3.2) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
+> Ardo, J., & Law, R. (2023). vector2dggs (0.3.3) [Computer software]. https://github.com/manaakiwhenua/vector2dggs
 
 [![manaakiwhenua-standards](https://github.com/manaakiwhenua/vector2dggs/workflows/manaakiwhenua-standards/badge.svg)](https://github.com/manaakiwhenua/manaakiwhenua-standards)
```

