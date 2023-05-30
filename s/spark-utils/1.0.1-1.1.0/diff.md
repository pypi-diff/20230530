# Comparing `tmp/spark_utils-1.0.1.tar.gz` & `tmp/spark_utils-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_utils-1.0.1.tar", max compression
+gzip compressed data, was "spark_utils-1.1.0.tar", max compression
```

## Comparing `spark_utils-1.0.1.tar` & `spark_utils-1.1.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0     1075 2023-01-23 14:03:49.315519 spark_utils-1.0.1/LICENSE
--rw-r--r--   0        0        0     6653 2023-01-23 14:03:49.315519 spark_utils-1.0.1/README.md
--rw-r--r--   0        0        0      732 2023-01-23 14:04:06.399471 spark_utils-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1135 2023-01-23 14:03:49.319519 spark_utils-1.0.1/spark_utils/__init__.py
--rw-r--r--   0        0        0       22 2023-01-23 14:04:06.403471 spark_utils-1.0.1/spark_utils/_version.py
--rw-r--r--   0        0        0     1134 2023-01-23 14:03:49.319519 spark_utils-1.0.1/spark_utils/common/__init__.py
--rw-r--r--   0        0        0     4345 2023-01-23 14:03:49.319519 spark_utils-1.0.1/spark_utils/common/functions.py
--rw-r--r--   0        0        0     6082 2023-01-23 14:03:49.319519 spark_utils-1.0.1/spark_utils/common/spark_job_args.py
--rw-r--r--   0        0        0    10429 2023-01-23 14:03:49.319519 spark_utils-1.0.1/spark_utils/common/spark_session_provider.py
--rw-r--r--   0        0        0     3421 2023-01-23 14:03:49.319519 spark_utils-1.0.1/spark_utils/common/spark_sql_utils.py
--rw-r--r--   0        0        0     1450 2023-01-23 14:03:49.319519 spark_utils-1.0.1/spark_utils/common/spark_udf.py
--rw-r--r--   0        0        0     1135 2023-01-23 14:03:49.319519 spark_utils-1.0.1/spark_utils/dataframes/__init__.py
--rw-r--r--   0        0        0    10650 2023-01-23 14:03:49.319519 spark_utils-1.0.1/spark_utils/dataframes/functions.py
--rw-r--r--   0        0        0     2324 2023-01-23 14:03:49.319519 spark_utils-1.0.1/spark_utils/dataframes/models.py
--rw-r--r--   0        0        0     1135 2023-01-23 14:03:49.319519 spark_utils-1.0.1/spark_utils/dataframes/sets/__init__.py
--rw-r--r--   0        0        0     1631 2023-01-23 14:03:49.319519 spark_utils-1.0.1/spark_utils/dataframes/sets/functions.py
--rw-r--r--   0        0        0     1135 2023-01-23 14:03:49.319519 spark_utils-1.0.1/spark_utils/delta_lake/__init__.py
--rw-r--r--   0        0        0     1746 2023-01-23 14:03:49.319519 spark_utils-1.0.1/spark_utils/delta_lake/delta_log.py
--rw-r--r--   0        0        0     6209 2023-01-23 14:03:49.319519 spark_utils-1.0.1/spark_utils/delta_lake/functions.py
--rw-r--r--   0        0        0     1135 2023-01-23 14:03:49.319519 spark_utils-1.0.1/spark_utils/models/__init__.py
--rw-r--r--   0        0        0     1642 2023-01-23 14:03:49.319519 spark_utils-1.0.1/spark_utils/models/hive_metastore_config.py
--rw-r--r--   0        0        0     1317 2023-01-23 14:03:49.319519 spark_utils-1.0.1/spark_utils/models/hive_table.py
--rw-r--r--   0        0        0     1872 2023-01-23 14:03:49.319519 spark_utils-1.0.1/spark_utils/models/job_socket.py
--rw-r--r--   0        0        0     1131 2023-01-23 14:03:49.319519 spark_utils-1.0.1/spark_utils/models/k8s_config.py
--rw-r--r--   0        0        0     7808 1970-01-01 00:00:00.000000 spark_utils-1.0.1/setup.py
--rw-r--r--   0        0        0     7544 1970-01-01 00:00:00.000000 spark_utils-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-05-30 16:08:05.598116 spark_utils-1.1.0/LICENSE
+-rw-r--r--   0        0        0     6766 2023-05-30 16:08:05.598116 spark_utils-1.1.0/README.md
+-rw-r--r--   0        0        0      791 2023-05-30 16:08:21.997662 spark_utils-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1135 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-30 16:08:21.997662 spark_utils-1.1.0/spark_utils/_version.py
+-rw-r--r--   0        0        0     1134 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/common/__init__.py
+-rw-r--r--   0        0        0     4257 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/common/functions.py
+-rw-r--r--   0        0        0     5977 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/common/spark_job_args.py
+-rw-r--r--   0        0        0     9716 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/common/spark_session_provider.py
+-rw-r--r--   0        0        0     3381 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/common/spark_sql_utils.py
+-rw-r--r--   0        0        0     1449 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/common/spark_udf.py
+-rw-r--r--   0        0        0     1135 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/dataframes/__init__.py
+-rw-r--r--   0        0        0    10376 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/dataframes/functions.py
+-rw-r--r--   0        0        0     2325 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/dataframes/models.py
+-rw-r--r--   0        0        0     1135 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/dataframes/sets/__init__.py
+-rw-r--r--   0        0        0     1631 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/dataframes/sets/functions.py
+-rw-r--r--   0        0        0     1135 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/delta_lake/__init__.py
+-rw-r--r--   0        0        0     1691 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/delta_lake/delta_log.py
+-rw-r--r--   0        0        0     5982 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/delta_lake/functions.py
+-rw-r--r--   0        0        0     1135 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/models/__init__.py
+-rw-r--r--   0        0        0     1641 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/models/hive_metastore_config.py
+-rw-r--r--   0        0        0     1318 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/models/hive_table.py
+-rw-r--r--   0        0        0     1868 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/models/job_socket.py
+-rw-r--r--   0        0        0     1129 2023-05-30 16:08:05.598116 spark_utils-1.1.0/spark_utils/models/k8s_config.py
+-rw-r--r--   0        0        0     7658 1970-01-01 00:00:00.000000 spark_utils-1.1.0/PKG-INFO
```

### Comparing `spark_utils-1.0.1/LICENSE` & `spark_utils-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spark_utils-1.0.1/README.md` & `spark_utils-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Introduction
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 Utility functions and classes for working with Dataframes, provisioning SparkSession and much more.
 
 Core features:
 
 - Provisioning Spark session with some routine settings set in advance, including Delta Lake configuration. You must
   have delta-core jars in class path for this to work.
```

### Comparing `spark_utils-1.0.1/pyproject.toml` & `spark_utils-1.1.0/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 [tool.poetry]
 name = "spark-utils"
-version = "1.0.1"
+version = "1.1.0"
 description = "Utility classes for comfy Spark job authoriing."
 authors = ["ECCO Sneaks & Data <esdsupport@ecco.com>"]
 maintainers = ['GZU <gzu@ecco.com>', 'JRB <ext-jrb@ecco.com>']
 license = 'MIT'
 readme = "README.md"
 repository = 'https://github.com/SneaksAndData/spark-utils'
 
 [tool.poetry.dependencies]
-python = "^3.9"
-hadoop-fs-wrapper = "~0.5.2"
+python = ">=3.9, <3.12"
+hadoop-fs-wrapper = "~0.6.0"
 cryptography = "~36.0"
-delta-spark = "~2.1.1"
+delta-spark = "~2.4.0"
 
 kubernetes = { version = "24.2.0", optional = true }
 
 [tool.poetry.extras]
 k8s = [
     'kubernetes'
 ]
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0"
 pytest-cov = "^2.12"
 pylint = "^2.12"
+black = "~22.12.0"
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.black]
+line-length = 120
```

### Comparing `spark_utils-1.0.1/spark_utils/__init__.py` & `spark_utils-1.1.0/spark_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.0.1/spark_utils/common/__init__.py` & `spark_utils-1.1.0/spark_utils/common/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.0.1/spark_utils/common/functions.py` & `spark_utils-1.1.0/spark_utils/common/functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -46,22 +46,22 @@
 def decrypt_sensitive(sensitive_content: Optional[str]) -> Optional[str]:
     """
       Decrypts a provided string
 
     :param sensitive_content: payload to decrypt
     :return: Decrypted payload
     """
-    encryption_key = os.environ.get('RUNTIME_ENCRYPTION_KEY', '').encode('utf-8')
+    encryption_key = os.environ.get("RUNTIME_ENCRYPTION_KEY", "").encode("utf-8")
 
     if not encryption_key:
-        print('Encryption key not set - skipping operation.')
+        print("Encryption key not set - skipping operation.")
 
     if encryption_key and sensitive_content:
         fernet = Fernet(encryption_key)
-        return fernet.decrypt(sensitive_content.encode('utf-8')).decode('utf-8')
+        return fernet.decrypt(sensitive_content.encode("utf-8")).decode("utf-8")
 
     return None
 
 
 def read_from_socket(
     socket: JobSocket,
     spark_session: SparkSession,
@@ -72,22 +72,18 @@
     :param socket: Socket
     :param spark_session: Spark session
     :param read_options: Read options passed to spark (e.g. Parquet options
     found here: https://spark.apache.org/docs/latest/sql-data-sources-parquet.html#data-source-option)
     :return: Spark dataframe
     """
     read_options = read_options or {}
-    if socket.data_format.startswith('hive'):
+    if socket.data_format.startswith("hive"):
         return spark_session.table(socket.data_path)
 
-    return spark_session \
-        .read \
-        .options(**read_options) \
-        .format(socket.data_format) \
-        .load(socket.data_path)
+    return spark_session.read.options(**read_options).format(socket.data_format).load(socket.data_path)
 
 
 def write_to_socket(
     data: DataFrame,
     socket: JobSocket,
     partition_by: Optional[List[str]] = None,
     partition_count: Optional[int] = None,
@@ -99,25 +95,20 @@
     :param socket: Socket to write to
     :param partition_by: List of column names to partition by
     :param partition_count: Number of partitions to split result into.
     :param write_options: Write options passed to spark (e.g. Parquet options
     found here: https://spark.apache.org/docs/latest/sql-data-sources-parquet.html#data-source-option)
     """
     write_options = write_options or {}
+    partition_by = partition_by or []
     if partition_count:
         data = data.repartition(partition_count, *partition_by)
 
-    writer = data.write \
-        .mode('overwrite') \
-        .options(**write_options)
+    writer = data.write.mode("overwrite").options(**write_options)
 
     if partition_by:
         writer = writer.partitionBy(*partition_by)
 
-    if socket.data_format.startswith('hive'):
-        writer \
-            .format(socket.data_format.split('_')[-1]) \
-            .saveAsTable(socket.data_path)
+    if socket.data_format.startswith("hive"):
+        writer.format(socket.data_format.split("_")[-1]).saveAsTable(socket.data_path)
     else:
-        writer \
-            .format(socket.data_format) \
-            .save(socket.data_path)
+        writer.format(socket.data_format).save(socket.data_path)
```

### Comparing `spark_utils-1.0.1/spark_utils/common/spark_job_args.py` & `spark_utils-1.1.0/spark_utils/common/spark_job_args.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,79 +29,78 @@
 
 from spark_utils.common.functions import decrypt_sensitive
 from spark_utils.models.job_socket import JobSocket
 
 
 class DecryptAction(argparse.Action):
     """
-      Action that performs decryption of a provided value using encryption key provided from the environment.
+    Action that performs decryption of a provided value using encryption key provided from the environment.
     """
 
-    def __init__(self,
-                 option_strings,
-                 dest,
-                 const=None,
-                 default=None,
-                 required=False,
-                 **kwargs):
+    def __init__(self, option_strings, dest, const=None, default=None, required=False, **kwargs):
         super().__init__(
-            option_strings=option_strings,
-            dest=dest,
-            nargs=1,
-            const=const,
-            default=default,
-            required=required,
-            **kwargs)
+            option_strings=option_strings, dest=dest, nargs=1, const=const, default=default, required=required, **kwargs
+        )
 
     def __call__(self, parser, namespace, values, option_string=None):
         arg_value = values[0]
         if arg_value.startswith("'"):
             arg_value = arg_value[1:]
         if arg_value.endswith("'"):
             arg_value = arg_value[:-1]
         setattr(namespace, self.dest, decrypt_sensitive(arg_value))
 
 
 class SparkJobArgs:
     """
-     Argsparse-based Spark job arguments provider
+    Argsparse-based Spark job arguments provider
 
-     This adds three default arguments to each job:
-      - --source a|b|c d|e|f ...
-      Describes inputs used by a job
-      Here `a` is a mapping key that a developer should use to extract path/format information for the source
-           `b` is a source path, in URI format: file:///, abfss:// etc.
-           'c' is a data format: json, csv, delta etc.
-      - --output a|b|c d|e|f...
-      Describes output locations used by a job
-      Same meanings as source attributes
-      - --overwrite
-      Controls overwrite behaviour. Will wipe the whole directory if set and honored by job developer.
+    This adds three default arguments to each job:
+     - --source a|b|c d|e|f ...
+     Describes inputs used by a job
+     Here `a` is a mapping key that a developer should use to extract path/format information for the source
+          `b` is a source path, in URI format: file:///, abfss:// etc.
+          'c' is a data format: json, csv, delta etc.
+     - --output a|b|c d|e|f...
+     Describes output locations used by a job
+     Same meanings as source attributes
+     - --overwrite
+     Controls overwrite behaviour. Will wipe the whole directory if set and honored by job developer.
     """
 
     def __init__(self):
         self._parser = argparse.ArgumentParser(description="Runtime arguments")
-        self._parser.add_argument("--source", type=str, nargs='+', default=[],
-                                  help='Sources to read data from, in a form of <source key>:<source path>')
-        self._parser.add_argument("--output", type=str, nargs='+', default=[],
-                                  help='Outputs to write data to, in a form of <output key>:<output path>')
-        self._parser.add_argument("--overwrite", dest='overwrite', action='store_true', help="Overwrite outputs")
+        self._parser.add_argument(
+            "--source",
+            type=str,
+            nargs="+",
+            default=[],
+            help="Sources to read data from, in a form of <source key>:<source path>",
+        )
+        self._parser.add_argument(
+            "--output",
+            type=str,
+            nargs="+",
+            default=[],
+            help="Outputs to write data to, in a form of <output key>:<output path>",
+        )
+        self._parser.add_argument("--overwrite", dest="overwrite", action="store_true", help="Overwrite outputs")
 
         self._parsed_args = None
         self._parsed_sources = None
         self._parsed_outputs = None
         self._overwrite = False
 
     def _sources(self) -> Iterable[JobSocket]:
         for source in self._parsed_args.source:
-            yield JobSocket(*source.split('|'))
+            yield JobSocket(*source.split("|"))
 
     def _outputs(self) -> Iterable[JobSocket]:
         for output in self._parsed_args.output:
-            yield JobSocket(*output.split('|'))
+            yield JobSocket(*output.split("|"))
 
     def new_arg(self, *args, **kwargs):
         """
         Adds one or more new arguments
         :param args: argsparse.add_argument(...)
         :return:
         """
@@ -112,18 +111,18 @@
     def new_encrypted_arg(self, *args, **kwargs):
         """
         Adds an argument that requires decryption before it can be used.
 
         :param args: argsparse.add_argument(...)
         :return:
         """
-        if 'action' not in kwargs:
-            kwargs.setdefault('action', DecryptAction)
+        if "action" not in kwargs:
+            kwargs.setdefault("action", DecryptAction)
         else:
-            kwargs['action'] = DecryptAction
+            kwargs["action"] = DecryptAction
 
         self._parser.add_argument(*args, **kwargs)
 
         return self
 
     def parse(self, arg_list=None):
         """
```

### Comparing `spark_utils-1.0.1/spark_utils/common/spark_session_provider.py` & `spark_utils-1.1.0/spark_utils/common/spark_session_provider.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,193 +26,197 @@
 import json
 import os
 import tempfile
 import uuid
 from typing import Optional, List, Dict
 
 try:
-    from kubernetes.client import V1Pod, V1ObjectMeta, V1PodSpec, V1Container, V1ContainerPort, V1EnvVar, \
-        V1ResourceRequirements, V1PodSecurityContext, V1NodeAffinity, V1NodeSelector, V1NodeSelectorTerm, \
-        V1NodeSelectorRequirement, V1Toleration
+    from kubernetes.client import (
+        V1Pod,
+        V1ObjectMeta,
+        V1PodSpec,
+        V1Container,
+        V1ContainerPort,
+        V1EnvVar,
+        V1PodSecurityContext,
+        V1NodeAffinity,
+        V1NodeSelector,
+        V1NodeSelectorTerm,
+        V1NodeSelectorRequirement,
+        V1Toleration,
+    )
 except ModuleNotFoundError:
     pass
 import pyspark
 from pyspark.sql import SparkSession
 
 from spark_utils.models.k8s_config import SparkKubernetesConfig
 from spark_utils.models.hive_metastore_config import HiveMetastoreConfig
 
 
 class SparkSessionProvider:
     """
-      Provider of a Spark session and related objects
+    Provider of a Spark session and related objects
     """
 
-    def __init__(self, *, delta_lake_version="2.12:2.1.0", hive_metastore_config: Optional[HiveMetastoreConfig] = None,
-                 additional_packages: Optional[List[str]] = None,
-                 additional_configs: Optional[Dict[str, str]] = None,
-                 run_local=False):
+    def __init__(
+        self,
+        *,
+        delta_lake_version="2.12:2.4.0",
+        hive_metastore_config: Optional[HiveMetastoreConfig] = None,
+        additional_packages: Optional[List[str]] = None,
+        additional_configs: Optional[Dict[str, str]] = None,
+        run_local=False,
+    ):
         """
         :param delta_lake_version: Delta lake package version.
         :param hive_metastore_config: Optional configuration of a hive metastore that should be connected to this Spark Session.
         :param additional_packages: Additional jars to download. Would not override jars installed or provided from spark-submit.
          This setting only works if a session is started from python and not spark-submit.
         :param additional_configs: Any additional spark configurations.
         :param run_local: Whether single-node local master should be used.
         """
 
         packages = [f"io.delta:delta-core_{delta_lake_version}"]
         if additional_packages:
             packages.extend(additional_packages)
 
-        self._spark_session_builder = SparkSession.builder \
-            .config("spark.jars.packages", ",".join(packages)) \
-            .config("spark.sql.extensions", "io.delta.sql.DeltaSparkSessionExtension") \
-            .config("spark.sql.catalog.spark_catalog", "org.apache.spark.sql.delta.catalog.DeltaCatalog") \
-            .config("spark.jars.ivy", os.path.join(tempfile.gettempdir(), ".ivy2")) \
-            .config("spark.sql.legacy.parquet.datetimeRebaseModeInWrite", "CORRECTED") \
-            .config("spark.sql.legacy.parquet.int96RebaseModeInWrite", "CORRECTED")
+        self._spark_session_builder = (
+            SparkSession.builder.config("spark.jars.packages", ",".join(packages))
+            .config("spark.sql.extensions", "io.delta.sql.DeltaSparkSessionExtension")
+            .config("spark.sql.catalog.spark_catalog", "org.apache.spark.sql.delta.catalog.DeltaCatalog")
+            .config("spark.jars.ivy", os.path.join(tempfile.gettempdir(), ".ivy2"))
+            .config("spark.sql.parquet.datetimeRebaseModeInWrite", "CORRECTED")
+            .config("spark.sql.parquet.int96RebaseModeInWrite", "CORRECTED")
+        )
 
         if hive_metastore_config:
             if hive_metastore_config.connection_driver_name:
-                self._spark_session_builder = self._spark_session_builder \
-                    .config("spark.hadoop.javax.jdo.option.ConnectionURL", hive_metastore_config.connection_url) \
-                    .config("spark.hadoop.javax.jdo.option.ConnectionUserName",
-                            hive_metastore_config.connection_username) \
-                    .config("spark.hadoop.javax.jdo.option.ConnectionPassword",
-                            hive_metastore_config.connection_password) \
-                    .config("spark.hadoop.javax.jdo.option.ConnectionDriverName",
-                            hive_metastore_config.connection_driver_name)
+                self._spark_session_builder = (
+                    self._spark_session_builder.config(
+                        "spark.hadoop.javax.jdo.option.ConnectionURL", hive_metastore_config.connection_url
+                    )
+                    .config(
+                        "spark.hadoop.javax.jdo.option.ConnectionUserName", hive_metastore_config.connection_username
+                    )
+                    .config(
+                        "spark.hadoop.javax.jdo.option.ConnectionPassword", hive_metastore_config.connection_password
+                    )
+                    .config(
+                        "spark.hadoop.javax.jdo.option.ConnectionDriverName",
+                        hive_metastore_config.connection_driver_name,
+                    )
+                )
             elif hive_metastore_config.metastore_uri:
-                self._spark_session_builder = self._spark_session_builder \
-                    .config("spark.hadoop.hive.metastore.uris", hive_metastore_config.metastore_uri)
+                self._spark_session_builder = self._spark_session_builder.config(
+                    "spark.hadoop.hive.metastore.uris", hive_metastore_config.metastore_uri
+                )
             else:
                 raise ValueError("Invalid Hive Metastore Configuration provided")
 
-            self._spark_session_builder = self._spark_session_builder \
-                .config("spark.sql.hive.metastore.version", hive_metastore_config.metastore_version) \
-                .config("spark.sql.hive.metastore.jars", hive_metastore_config.metastore_jars) \
+            self._spark_session_builder = (
+                self._spark_session_builder.config(
+                    "spark.sql.hive.metastore.version", hive_metastore_config.metastore_version
+                )
+                .config("spark.sql.hive.metastore.jars", hive_metastore_config.metastore_jars)
                 .config("spark.sql.catalogImplementation", "hive")
+            )
 
         if additional_configs:
             for config_key, config_value in additional_configs.items():
                 self._spark_session_builder = self._spark_session_builder.config(config_key, config_value)
 
         self._run_local = run_local
 
     @property
     def session_builder(self) -> pyspark.sql.session.SparkSession.Builder:
         """
-          Return a current session builder object.
+        Return a current session builder object.
         """
         return self._spark_session_builder
 
     def configure_for_k8s(
-            self,
-            master_url: str,
-            spark_config: SparkKubernetesConfig,
-            master_port: int = 443
-    ) -> 'SparkSessionProvider':
-        """
-         Configures spark session for using Kubernetes as a resource manager.
-
-         :param master_url: Kubernetes API URL, i.e. https://my-server-api.mydomain.com.
-         :param spark_config: Spark on K8S-specific configurations.
-         :param master_port: Connection port for the API server.
+        self, master_url: str, spark_config: SparkKubernetesConfig, master_port: int = 443
+    ) -> "SparkSessionProvider":
+        """
+        Configures spark session for using Kubernetes as a resource manager.
+
+        :param master_url: Kubernetes API URL, i.e. https://my-server-api.mydomain.com.
+        :param spark_config: Spark on K8S-specific configurations.
+        :param master_port: Connection port for the API server.
         """
         executor_name = spark_config.executor_name_prefix or str(uuid.uuid4())
         # base configuration
-        self._spark_session_builder = self._spark_session_builder \
-            .master(f"k8s://{master_url}:{master_port}") \
-            .config("spark.kubernetes.driver.pod.name", spark_config.driver_name or os.getenv('SPARK_DRIVER_NAME')) \
-            .config("spark.app.name", spark_config.application_name) \
-            .config("spark.kubernetes.executor.podNamePrefix", executor_name) \
-            .config('spark.kubernetes.executor.limit.cores', 1) \
-            .config('spark.driver.host', spark_config.driver_ip or os.getenv('SPARK_DRIVER_IP')) \
-            .config('spark.kubernetes.namespace', spark_config.k8s_namespace) \
-            .config('spark.kubernetes.container.image', spark_config.spark_image) \
-            .config('spark.shuffle.service.enabled', 'false')  # disable external shuffle service for now
+        self._spark_session_builder = (
+            self._spark_session_builder.master(f"k8s://{master_url}:{master_port}")
+            .config("spark.kubernetes.driver.pod.name", spark_config.driver_name or os.getenv("SPARK_DRIVER_NAME"))
+            .config("spark.app.name", spark_config.application_name)
+            .config("spark.kubernetes.executor.podNamePrefix", executor_name)
+            .config("spark.driver.host", spark_config.driver_ip or os.getenv("SPARK_DRIVER_IP"))
+            .config("spark.kubernetes.namespace", spark_config.k8s_namespace)
+            .config("spark.kubernetes.container.image", spark_config.spark_image)
+            .config("spark.shuffle.service.enabled", "false")
+        )  # disable external shuffle service for now
 
         # generate executor template
         executor_template = V1Pod(
-            api_version='v1',
-            kind='Pod',
-            metadata=V1ObjectMeta(name='spark-executor', namespace=spark_config.k8s_namespace),
+            api_version="v1",
+            kind="Pod",
+            metadata=V1ObjectMeta(name="spark-executor", namespace=spark_config.k8s_namespace),
             spec=V1PodSpec(
                 containers=[
                     V1Container(
-                        name='spark-executor',
+                        name="spark-executor",
                         image=spark_config.spark_image,
-                        ports=[
-                            V1ContainerPort(
-                                name='http',
-                                container_port=8080,
-                                protocol='TCP'
-                            )
-                        ],
-                        env=[
-                            V1EnvVar(
-                                name='SPARK_WORKER_WEBUI_PORT',
-                                value='8080'
-                            )
-                        ],
-                        resources=V1ResourceRequirements(
-                            limits={
-                                'cpu': 1,
-                                'memory': f'{spark_config.default_executor_memory}Mi'
-                            },
-                            requests={
-                                'cpu': 1,
-                                'memory': f'{spark_config.default_executor_memory}Mi'
-                            }
-                        )
+                        ports=[V1ContainerPort(name="http", container_port=8080, protocol="TCP")],
+                        env=[V1EnvVar(name="SPARK_WORKER_WEBUI_PORT", value="8080")],
                     )
                 ],
-                restart_policy='Never',
+                restart_policy="Never",
                 security_context=V1PodSecurityContext(
-                    run_as_user=spark_config.spark_uid,
-                    run_as_group=spark_config.spark_gid
+                    run_as_user=spark_config.spark_uid, run_as_group=spark_config.spark_gid
                 ),
                 affinity=V1NodeAffinity(
                     required_during_scheduling_ignored_during_execution=V1NodeSelector(
                         node_selector_terms=[
-                            V1NodeSelectorTerm(match_expressions=[
-                                V1NodeSelectorRequirement(
-                                    key=affinity_key,
-                                    values=[affinity_value], operator='In'
-                                ) for affinity_key, affinity_value in spark_config.executor_node_affinity.items()
-                            ])
+                            V1NodeSelectorTerm(
+                                match_expressions=[
+                                    V1NodeSelectorRequirement(key=affinity_key, values=[affinity_value], operator="In")
+                                    for affinity_key, affinity_value in spark_config.executor_node_affinity.items()
+                                ]
+                            )
                         ]
                     )
-                ) if spark_config.executor_node_affinity else None,
+                )
+                if spark_config.executor_node_affinity
+                else None,
                 tolerations=[
-                    V1Toleration(
-                        effect='NoSchedule',
-                        key=affinity_key,
-                        operator='Equal',
-                        value=affinity_value
-                    ) for affinity_key, affinity_value in spark_config.executor_node_affinity.items()
-                ] if spark_config.executor_node_affinity else None
-            )
+                    V1Toleration(effect="NoSchedule", key=affinity_key, operator="Equal", value=affinity_value)
+                    for affinity_key, affinity_value in spark_config.executor_node_affinity.items()
+                ]
+                if spark_config.executor_node_affinity
+                else None,
+            ),
         )
 
         template_path = os.path.join(tempfile.gettempdir(), executor_name)
         os.makedirs(template_path, exist_ok=True)
 
-        with open(os.path.join(template_path, "template.yml"), 'w', encoding='utf-8') as pod_template:
+        with open(os.path.join(template_path, "template.yml"), "w", encoding="utf-8") as pod_template:
             pod_template.write(json.dumps(executor_template.to_dict()))
 
-        self._spark_session_builder = self._spark_session_builder \
-            .config("spark.kubernetes.executor.podTemplateFile", os.path.join(template_path, "template.yml"))
+        self._spark_session_builder = self._spark_session_builder.config(
+            "spark.kubernetes.executor.podTemplateFile", os.path.join(template_path, "template.yml")
+        )
 
         return self
 
     def get_session(self):
         """
           Launch a configured Spark Session.
 
         :return: SparkSession
         """
-        if os.environ.get('PYTEST_CURRENT_TEST') or self._run_local:
-            return self._spark_session_builder.master('local[*]').getOrCreate()
+        if os.environ.get("PYTEST_CURRENT_TEST") or self._run_local:
+            return self._spark_session_builder.master("local[*]").getOrCreate()
 
         return self._spark_session_builder.getOrCreate()
```

### Comparing `spark_utils-1.0.1/spark_utils/common/spark_sql_utils.py` & `spark_utils-1.1.0/spark_utils/common/spark_sql_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,42 +30,46 @@
 from hadoop_fs_wrapper.wrappers.file_system import FileSystem
 
 from spark_utils.common.spark_job_args import SparkJobArgs
 from spark_utils.models.job_socket import JobSocket
 from spark_utils.dataframes.functions import union_dataframes
 
 
-def merge_or_create_table(spark_args: SparkJobArgs, spark_session: SparkSession, table_name: str,
-                          output_socket: JobSocket,
-                          merge_key_column="mergeKey"):
+def merge_or_create_table(
+    spark_args: SparkJobArgs,
+    spark_session: SparkSession,
+    table_name: str,
+    output_socket: JobSocket,
+    merge_key_column="mergeKey",
+):
     """
      Writes a specified SQL table or view to the provided output
 
     :param spark_args: Parent job runtime arguments
     :param spark_session: Spark Session to use when writing
     :param table_name: Table to write
     :param output_socket: JobSocket definition for the output
     :param merge_key_column: Table column to use when merging data
     :return:
     """
     output_file_system = FileSystem.from_spark_session(spark_session)
 
     if spark_args.overwrite():
         output_file_system.delete(path=output_socket.data_path, recursive=True)
-        spark_session.table(table_name).write.format(output_socket.data_format).mode('overwrite').save(
-            output_socket.data_path)
+        spark_session.table(table_name).write.format(output_socket.data_format).mode("overwrite").save(
+            output_socket.data_path
+        )
     else:
         delta_table = DeltaTable.forPath(spark_session, output_socket.data_path)
         delta_table.alias("target").merge(
             spark_session.table(table_name).alias("stagingData"),
             f"""
             stagingData.{merge_key_column} <=> target.{merge_key_column}
-            """) \
-            .whenNotMatchedInsertAll() \
-            .execute()
+            """,
+        ).whenNotMatchedInsertAll().execute()
 
 
 def union_views_to_schema(spark_session: SparkSession, schema: List[StructField], views: List[str]) -> DataFrame:
     """
       Combines all views and forces them into provided schema by adding missing columns filled with nulls
     :param spark_session: Spark Session to run the statement
     :param schema: Schema to enforce
```

### Comparing `spark_utils-1.0.1/spark_utils/common/spark_udf.py` & `spark_utils-1.1.0/spark_utils/common/spark_udf.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,9 +29,9 @@
 
 def getfromstr_uuid(input_str):
     """
       Generates UUID seeded by input
     :param input_str: Any string value
     :return: UUID that only matches provided input
     """
-    null_namespace = type('', (), dict(bytes=b''))()
+    null_namespace = type("", (), {"bytes": b""})()
     return str(uuid.uuid3(null_namespace, input_str))
```

### Comparing `spark_utils-1.0.1/spark_utils/dataframes/__init__.py` & `spark_utils-1.1.0/spark_utils/dataframes/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.0.1/spark_utils/dataframes/functions.py` & `spark_utils-1.1.0/spark_utils/dataframes/functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,17 +44,18 @@
       Returns an empty (null values) column
     :param col_name: Column name
     :return: Spark SQL column
     """
     return lit(None).alias(col_name)
 
 
-def order_df_and_add_missing_cols(source_df: DataFrame, columns_order_list: List[str],
-                                  df_missing_fields: List[str]) -> DataFrame:
-    """ return ordered dataFrame by the columns order list with null in missing columns """
+def order_df_and_add_missing_cols(
+    source_df: DataFrame, columns_order_list: List[str], df_missing_fields: List[str]
+) -> DataFrame:
+    """return ordered dataFrame by the columns order list with null in missing columns"""
     if not df_missing_fields:  # no missing fields for the df
         return source_df.select(columns_order_list)
 
     columns = []
     missing_lower = list(map(lambda x: x.lower(), df_missing_fields))
     for col_name in columns_order_list:
         if col_name.lower() not in missing_lower:
@@ -73,84 +74,82 @@
     :return: Dataframe with new columns from missing_column_names, initialized with nulls
     """
     for missing_col in missing_column_names:
         source_df = source_df.withColumn(missing_col, empty_column(missing_col))
     return source_df
 
 
-def order_and_union_dataframes(left_df: DataFrame, right_df: DataFrame, left_list_miss_cols: List[str],
-                               right_list_miss_cols: List[str]) -> DataFrame:
+def order_and_union_dataframes(
+    left_df: DataFrame, right_df: DataFrame, left_list_miss_cols: List[str], right_list_miss_cols: List[str]
+) -> DataFrame:
     """
       Union data frames and order columns by left_df.
 
     :param left_df: Left dataframe
     :param right_df: Right dataframe
     :param left_list_miss_cols: Columns to add to the left df
     :param right_list_miss_cols: Columns to add to the right df
     :return:
     """
     left_df_all_cols = add_missing_columns(left_df, left_list_miss_cols)
-    right_df_all_cols = order_df_and_add_missing_cols(right_df, left_df_all_cols.schema.names,
-                                                      right_list_miss_cols)
+    right_df_all_cols = order_df_and_add_missing_cols(right_df, left_df_all_cols.schema.names, right_list_miss_cols)
     return left_df_all_cols.union(right_df_all_cols)
 
 
 def union_dataframes(left_df: DataFrame, right_df: DataFrame) -> DataFrame:
     """
       Union between two dataFrames, if there is a gap of column fields,
       it will append all missing columns as nulls
 
     :param left_df: Left dataframe
     :param right_df: Right dataframe
     :return: A new dataframe, union of left and right
     """
     # Check for None input
-    assert left_df, 'left_df parameter should not be None'
-    assert right_df, 'right_df parameter should not be None'
+    assert left_df, "left_df parameter should not be None"
+    assert right_df, "right_df parameter should not be None"
 
     # For data frames with equal columns and order - regular union
     if left_df.schema.names == right_df.schema.names:
         return left_df.union(right_df)
 
     # Different columns
     # Save dataFrame columns name list as set
     left_df_col_list = set(left_df.schema.names)
     right_df_col_list = set(right_df.schema.names)
     # Diff columns between left_df and right_df
-    right_list_miss_cols = case_insensitive_diff(
-        left_df_col_list, right_df_col_list)
-    left_list_miss_cols = case_insensitive_diff(
-        right_df_col_list, left_df_col_list)
+    right_list_miss_cols = case_insensitive_diff(left_df_col_list, right_df_col_list)
+    left_list_miss_cols = case_insensitive_diff(right_df_col_list, left_df_col_list)
     return order_and_union_dataframes(left_df, right_df, list(left_list_miss_cols), list(right_list_miss_cols))
 
 
 def rename_column(name: str) -> str:
     """
       Removes illegal column characters from a string
 
     :param name: String to format
     :return:
     """
 
     illegals = [
-        ' ',
-        ',',
-        ';',
-        '{',
-        '}',
-        '(',
-        ')',
-        '\t',
-        '=',
-        '/',
-        '\\',
+        " ",
+        ",",
+        ";",
+        "{",
+        "}",
+        "(",
+        ")",
+        "\t",
+        "=",
+        "/",
+        "\\",
     ]
 
     for illegal in illegals:
-        name = name.replace(illegal, '')
+        name = name.replace(illegal, "")
 
     return name
 
 
 def rename_columns(dataframe: DataFrame) -> DataFrame:
     """
       Removes illegal characters from all columns
@@ -165,108 +164,101 @@
     """
       Returns max of a provided timestamp column, using provided format.
     :param dataframe: Dataframe to perform computation on.
     :param timestamp_column: Timestamp column to max.
     :param timestamp_column_format: Timestamp column format.
     :return: max timestamp.
     """
-    return dataframe.select(
-        to_timestamp(col(timestamp_column), timestamp_column_format).alias(timestamp_column)).agg(
-        df_max(col(timestamp_column)).alias(timestamp_column)).head(1)[0][0]
+    return (
+        dataframe.select(to_timestamp(col(timestamp_column), timestamp_column_format).alias(timestamp_column))
+        .agg(df_max(col(timestamp_column)).alias(timestamp_column))
+        .head(1)[0][0]
+    )
 
 
-def copy_dataframe_to_socket(spark_session: SparkSession,
-                             copy_options: CopyDataOptions) -> dict:
+def copy_dataframe_to_socket(spark_session: SparkSession, copy_options: CopyDataOptions) -> dict:
     """
       Copies data from src to dest JobSocket via a SparkSession
 
     :param spark_session: Spark Session to use for copying
     :param copy_options: Copy options.
     :return: dict of (original_row_count, original_content_age, row_count, content_age)
     """
 
     print(f"Running data copy using options: {copy_options}")
 
     copy_options.read_options = copy_options.read_options or {}
     copy_options.write_options = copy_options.write_options or {}
 
     if copy_options.timestamp_column:
-        assert copy_options.timestamp_column_format, \
-            'When specifying timestamp_column, you must provide timestamp_column_format as well.'
+        assert (
+            copy_options.timestamp_column_format
+        ), "When specifying timestamp_column, you must provide timestamp_column_format as well."
 
     output_file_system = FileSystem.from_spark_session(spark_session)
 
     if copy_options.clean_destination:
         output_file_system.delete(path=copy_options.dest.data_path, recursive=True)
 
-    copy_stats = {
-        'original_row_count': 0,
-        'original_content_age': 0,
-        'row_count': 0,
-        'content_age': 0
-    }
-
-    if is_valid_source_path(
-            file_system=output_file_system,
-            path=copy_options.dest.data_path
-    ):
+    copy_stats = {"original_row_count": 0, "original_content_age": 0, "row_count": 0, "content_age": 0}
+
+    if is_valid_source_path(file_system=output_file_system, path=copy_options.dest.data_path):
         original_df = spark_session.read.format(copy_options.dest.data_format).load(copy_options.dest.data_path)
-        copy_stats['original_row_count'] = original_df.count()
+        copy_stats["original_row_count"] = original_df.count()
         if copy_options.timestamp_column:
-            original_max_ts = _max_timestamp(original_df, copy_options.timestamp_column,
-                                             copy_options.timestamp_column_format)
-            copy_stats['original_content_age'] = int((datetime.utcnow() - original_max_ts).total_seconds())
+            original_max_ts = _max_timestamp(
+                original_df, copy_options.timestamp_column, copy_options.timestamp_column_format
+            )
+            copy_stats["original_content_age"] = int((datetime.utcnow() - original_max_ts).total_seconds())
 
-    source_df = spark_session.read.format(copy_options.src.data_format).options(**copy_options.read_options).load(
-        copy_options.src.data_path)
+    source_df = (
+        spark_session.read.format(copy_options.src.data_format)
+        .options(**copy_options.read_options)
+        .load(copy_options.src.data_path)
+    )
 
     if copy_options.clean_column_names:
         source_df = rename_columns(source_df)
 
     if copy_options.include_filename:
-        source_df = source_df \
-            .withColumn("filename", input_file_name())
+        source_df = source_df.withColumn("filename", input_file_name())
 
     if copy_options.include_row_sequence:
-        source_df = source_df \
-            .rdd.zipWithIndex() \
-            .map(lambda x: list(x[0]) + [x[1]]) \
-            .toDF(source_df.withColumn('row_sequence', lit(0)).schema)
+        source_df = (
+            source_df.rdd.zipWithIndex()
+            .map(lambda x: list(x[0]) + [x[1]])
+            .toDF(source_df.withColumn("row_sequence", lit(0)).schema)
+        )
 
-    copy_stats['row_count'] = source_df.count()
+    copy_stats["row_count"] = source_df.count()
 
     if copy_options.timestamp_column:
         max_ts = _max_timestamp(source_df, copy_options.timestamp_column, copy_options.timestamp_column_format)
-        copy_stats['content_age'] = int((datetime.utcnow() - max_ts).total_seconds())
+        copy_stats["content_age"] = int((datetime.utcnow() - max_ts).total_seconds())
 
     if copy_options.output_file_count:
         source_df = source_df.repartition(copy_options.output_file_count)
 
-    source_df \
-        .write \
-        .format(copy_options.dest.data_format) \
-        .options(**copy_options.write_options) \
-        .save(path=copy_options.dest.data_path, mode='errorifexists' if copy_options.clean_destination else 'append')
+    source_df.write.format(copy_options.dest.data_format).options(**copy_options.write_options).save(
+        path=copy_options.dest.data_path, mode="errorifexists" if copy_options.clean_destination else "append"
+    )
 
     return copy_stats
 
 
 def get_dataframe_columns(rows: Iterator[Row]) -> Iterator[HiveTableColumn]:
     """
      Reads columns from extended dataframe definition
 
     :param rows: Dataframe rows produced by describe table extended (df.toLocalIterator())
     :return:
     """
     for t_row in rows:
-        if t_row['col_name']:
-            yield HiveTableColumn(
-                name=rename_column(t_row['col_name']),
-                type=t_row['data_type']
-            )
+        if t_row["col_name"]:
+            yield HiveTableColumn(name=rename_column(t_row["col_name"]), type=t_row["data_type"])
         else:
             break
 
 
 def get_dataframe_partitions(rows: Iterator[Row]) -> Iterator[Tuple[int, str]]:
     """
       Reads Partitioning section from extended table description
@@ -276,14 +268,14 @@
     skip = True
     for t_row in rows:
         # catch when partitioning section starts
         if t_row["col_name"] == "# Partitioning":
             skip = False
             continue
         if not skip and t_row["col_name"]:
-            part_index_str = str(t_row['col_name']).replace("Part ", "")
+            part_index_str = str(t_row["col_name"]).replace("Part ", "")
             if part_index_str.isdigit():
-                yield int(part_index_str), rename_column(t_row['data_type'])
+                yield int(part_index_str), rename_column(t_row["data_type"])
             else:
                 break
         elif not skip and not t_row["col_name"]:
             break
```

### Comparing `spark_utils-1.0.1/spark_utils/dataframes/models.py` & `spark_utils-1.1.0/spark_utils/dataframes/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     :arg write_options: Spark session options to set when writing
     :arg include_filename: Adds "filename" column to the destination output.
     :arg include_row_sequence: Adds "sequence_number" column to the destination output.
     :arg clean_destination: Wipe destination path before starting a copy.
     :arg timestamp_column: Column name to use for evaluating data age.
     :arg timestamp_column_format: Format for the timestamp
     """
+
     src: JobSocket
     dest: JobSocket
     include_filename: bool = False
     include_row_sequence: bool = False
     clean_destination: bool = False
     clean_column_names: bool = False
     read_options: Optional[dict] = None
```

### Comparing `spark_utils-1.0.1/spark_utils/dataframes/sets/__init__.py` & `spark_utils-1.1.0/spark_utils/dataframes/sets/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.0.1/spark_utils/dataframes/sets/functions.py` & `spark_utils-1.1.0/spark_utils/dataframes/sets/functions.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.0.1/spark_utils/delta_lake/__init__.py` & `spark_utils-1.1.0/spark_utils/delta_lake/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.0.1/spark_utils/delta_lake/delta_log.py` & `spark_utils-1.1.0/spark_utils/delta_lake/delta_log.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,52 +4,54 @@
 from pyspark.sql import SparkSession
 from hadoop_fs_wrapper.models.hadoop_fs_path import HadoopFsPath
 
 
 # pylint: disable=W0212
 class DeltaLog:
     """
-     Wrapper for org.apache.spark.sql.delta.DeltaLog
+    Wrapper for org.apache.spark.sql.delta.DeltaLog
     """
 
     def __init__(self, underlying):
         """
-         Class init
+        Class init
         """
         self.underlying = underlying
 
     @classmethod
-    def for_table(cls, spark_session: SparkSession, data_path: str) -> 'DeltaLog':
+    def for_table(cls, spark_session: SparkSession, data_path: str) -> "DeltaLog":
         """
          Wraps constructor: def forTable(spark: SparkSession, dataPath: String): DeltaLog
 
          Helper for creating a log when it stored at the root of the data
 
         :param data_path: Path to delta table.
         :return: DeltaLog.
         """
         return cls(
-            spark_session._jvm.org.apache.spark.sql.delta.DeltaLog.forTable(spark_session._jsparkSession, data_path))
+            spark_session._jvm.org.apache.spark.sql.delta.DeltaLog.forTable(spark_session._jsparkSession, data_path)
+        )
 
     @staticmethod
     def invalidate_cache(spark_session: SparkSession, data_path: str) -> None:
         """
-          Invalidate the cached DeltaLog object for the given data_path.
+        Invalidate the cached DeltaLog object for the given data_path.
         """
 
         hadoop_path = HadoopFsPath.from_string(spark_session._jvm, data_path)
 
-        spark_session._jvm.org.apache.spark.sql.delta.DeltaLog.invalidateCache(spark_session._jsparkSession,
-                                                                               hadoop_path.underlying)
+        spark_session._jvm.org.apache.spark.sql.delta.DeltaLog.invalidateCache(
+            spark_session._jsparkSession, hadoop_path.underlying
+        )
 
     @staticmethod
     def clear_cache(spark_session: SparkSession):
         """
-         Clears all delta log caches associated with this Spark session.
+        Clears all delta log caches associated with this Spark session.
         """
         spark_session._jvm.org.apache.spark.sql.delta.DeltaLog.clearCache()
 
     def table_id(self) -> str:
         """
-          The unique identifier for this table.
+        The unique identifier for this table.
         """
         return self.underlying.tableId()
```

### Comparing `spark_utils-1.0.1/spark_utils/delta_lake/functions.py` & `spark_utils-1.1.0/spark_utils/delta_lake/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,21 +29,23 @@
 from delta import DeltaTable
 from pyspark.sql import SparkSession
 
 from spark_utils.dataframes.functions import get_dataframe_columns, get_dataframe_partitions
 from spark_utils.models.hive_table import HiveTableColumn
 
 
-def _generate_table_ddl(*,
-                        publish_as_symlink: bool,
-                        publish_schema_name: str,
-                        publish_table_name: str,
-                        column_str: str,
-                        partition_str: str,
-                        location: str) -> str:
+def _generate_table_ddl(
+    *,
+    publish_as_symlink: bool,
+    publish_schema_name: str,
+    publish_table_name: str,
+    column_str: str,
+    partition_str: str,
+    location: str,
+) -> str:
     """
       Generates CREATE ... TABLE  statement for Spark SQL.
 
     :param publish_as_symlink: Generate CREATE EXTERNAL TABLE with SymlinkTextInputFormat input format
     :param publish_schema_name: Hive schema to publish to.
     :param publish_table_name: Hive table.
     :param column_str: Column list, <col> <type>, comma-separated
@@ -64,20 +66,22 @@
     return f"""
         CREATE TABLE {publish_schema_name}.{publish_table_name}
         USING delta 
         LOCATION '{location}' 
         """
 
 
-def publish_delta_to_hive(spark_session: SparkSession,
-                          publish_table_name: str,
-                          publish_schema_name: str,
-                          data_path: str,
-                          refresh: bool = False,
-                          publish_as_symlink=True):
+def publish_delta_to_hive(
+    spark_session: SparkSession,
+    publish_table_name: str,
+    publish_schema_name: str,
+    data_path: str,
+    refresh: bool = False,
+    publish_as_symlink=True,
+):
     """
       Generate symlink manifest and create an external table in a Hive Metastore used by a SparkSession provided
 
       OR
 
       Generate simple Hive table linked to abfss path
 
@@ -96,47 +100,47 @@
     if refresh:
         spark_session.sql(f"DROP TABLE IF EXISTS {publish_schema_name}.{publish_table_name}")
 
     delta_table = DeltaTable.forPath(spark_session, data_path)
 
     (columns, partitions, location) = get_table_info(spark_session, data_path)
 
-    column_str = ','.join(map(lambda t_col: f"{t_col.name} {t_col.type}", columns))
-    partition_str = ','.join(map(lambda t_col: f"{t_col.name} {t_col.type}", partitions))
-    partition_str = '' if not partition_str else f"PARTITIONED BY ({partition_str})"
+    column_str = ",".join(map(lambda t_col: f"{t_col.name} {t_col.type}", columns))
+    partition_str = ",".join(map(lambda t_col: f"{t_col.name} {t_col.type}", partitions))
+    partition_str = "" if not partition_str else f"PARTITIONED BY ({partition_str})"
 
     if publish_as_symlink:
         delta_table.generate("symlink_format_manifest")
 
     create_table_sql = _generate_table_ddl(
         publish_as_symlink=publish_as_symlink,
         publish_schema_name=publish_schema_name,
         publish_table_name=publish_table_name,
         column_str=column_str,
         partition_str=partition_str,
-        location=location
+        location=location,
     )
 
     spark_session.sql(create_table_sql)
 
     if partition_str and publish_as_symlink:
         spark_session.sql(f"""MSCK REPAIR TABLE {publish_schema_name}.{publish_table_name}""")
 
 
-def get_table_info(spark_session: SparkSession, table_path: str) -> (
-        Iterator[HiveTableColumn], Iterator[HiveTableColumn], str):
+def get_table_info(
+    spark_session: SparkSession, table_path: str
+) -> (Iterator[HiveTableColumn], Iterator[HiveTableColumn], str):
     """
       Reads columns, partitions and table data location
 
     :param spark_session: SparkSession
     :param table_path: path to a Delta table
     :return:
     """
-    definition_table = spark_session.sql(
-        f"describe table extended delta.`{table_path}/`")
+    definition_table = spark_session.sql(f"describe table extended delta.`{table_path}/`")
 
     definition_table_rows = list(definition_table.toLocalIterator())
 
     cols = list(get_dataframe_columns(definition_table_rows))
 
     parts_names_with_index = list(get_dataframe_partitions(definition_table_rows))
     if parts_names_with_index:
```

### Comparing `spark_utils-1.0.1/spark_utils/models/__init__.py` & `spark_utils-1.1.0/spark_utils/models/__init__.py`

 * *Files identical despite different names*

### Comparing `spark_utils-1.0.1/spark_utils/models/hive_metastore_config.py` & `spark_utils-1.1.0/spark_utils/models/hive_metastore_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,17 @@
 from dataclasses import dataclass
 from typing import Optional
 
 
 @dataclass
 class HiveMetastoreConfig:
     """
-      Parameters required by Spark when connecting to an external Hive Metastore
+    Parameters required by Spark when connecting to an external Hive Metastore
     """
+
     metastore_version: str
     metastore_jars: str
     connection_url: Optional[str] = None
     connection_username: Optional[str] = None
     connection_password: Optional[str] = None
     connection_driver_name: Optional[str] = None
     metastore_uri: Optional[str] = None
```

### Comparing `spark_utils-1.0.1/spark_utils/models/hive_table.py` & `spark_utils-1.1.0/spark_utils/models/hive_table.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,9 +26,10 @@
 
 from dataclasses import dataclass
 
 
 @dataclass
 class HiveTableColumn:
     """Describes a Hive Metastore table column"""
+
     name: str
     type: str
```

### Comparing `spark_utils-1.0.1/spark_utils/models/job_socket.py` & `spark_utils-1.1.0/spark_utils/models/job_socket.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,25 +26,26 @@
 
 from dataclasses import dataclass
 
 
 @dataclass
 class JobSocket:
     """
-     Input/Output data map
+    Input/Output data map
 
-     Attributes:
-         alias: mapping key to be used by a consumer
-         data_path: fully qualified path to actual data, i.e. abfss://..., s3://... etc.
-         data_format: data format, i.e. csv, json, delta etc.
+    Attributes:
+        alias: mapping key to be used by a consumer
+        data_path: fully qualified path to actual data, i.e. abfss://..., s3://... etc.
+        data_format: data format, i.e. csv, json, delta etc.
     """
+
     alias: str
     data_path: str
     data_format: str
 
-    def serialize(self, separator: str = '|') -> str:
+    def serialize(self, separator: str = "|") -> str:
         """Serializes job socket to the format used by SparkJobArgs when reading from command line.
 
         Attributes:
             separator: Separator to use for serialization
         """
         return separator.join([self.alias, self.data_path, self.data_format])
```

### Comparing `spark_utils-1.0.1/spark_utils/models/k8s_config.py` & `spark_utils-1.1.0/spark_utils/models/k8s_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 from dataclasses import dataclass
 from typing import Optional, Dict
 
 
 @dataclass
 class SparkKubernetesConfig:
     """
-      Configuration parameters required to launch a k8s driver in client mode.
+    Configuration parameters required to launch a k8s driver in client mode.
     """
 
     # Spark Application name for this session.
     application_name: str
 
     # Kubernetes namespace where to launch executors.
     k8s_namespace: str
 
     # Image to use for executors.
     spark_image: str
 
     # Group for the Spark UID.
-    spark_gid: Optional[str] = '0'
+    spark_gid: Optional[str] = "0"
 
     # Spark UID.
-    spark_uid: Optional[str] = '1001'
+    spark_uid: Optional[str] = "1001"
 
     # Default memory to assign to executors if spark.executor.memory is not provided.
     default_executor_memory: Optional[int] = 2000
 
     # Name of a driver host.
     driver_name: Optional[str] = socket.gethostname()
```

### Comparing `spark_utils-1.0.1/setup.py` & `spark_utils-1.1.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,41 +1,152 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['spark_utils',
- 'spark_utils.common',
- 'spark_utils.dataframes',
- 'spark_utils.dataframes.sets',
- 'spark_utils.delta_lake',
- 'spark_utils.models']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['cryptography>=36.0,<36.1',
- 'delta-spark>=2.1.1,<2.2.0',
- 'hadoop-fs-wrapper>=0.5.2,<0.6.0']
-
-extras_require = \
-{'k8s': ['kubernetes==24.2.0']}
-
-setup_kwargs = {
-    'name': 'spark-utils',
-    'version': '1.0.1',
-    'description': 'Utility classes for comfy Spark job authoriing.',
-    'long_description': '# Introduction\n\nUtility functions and classes for working with Dataframes, provisioning SparkSession and much more.\n\nCore features:\n\n- Provisioning Spark session with some routine settings set in advance, including Delta Lake configuration. You must\n  have delta-core jars in class path for this to work.\n- Spark job argument wrappers, allowing to specify job inputs for `spark.read.format(...).options(...).load(...)` and\n  outputs for `spark.write.format(...).save(...)` in a generic way. Those are exposed as `source` and `target` built-in\n  arguments (see example below).\n\nConsider a simple Spark Job that reads `json` data from `source` and stores it as `parquet` in `target`. This job can be\ndefined using `spark-utils` as below:\n\n```python\nfrom spark_utils.common.spark_job_args import SparkJobArgs\nfrom spark_utils.common.spark_session_provider import SparkSessionProvider\n\n\ndef main(args=None):\n    """\n     Job entrypoint\n    :param args:\n    :return:\n    """\n    spark_args = SparkJobArgs().parse(args)\n\n    source_table = spark_args.source(\'json_source\')\n    target_table = spark_args.output(\'parquet_target\')\n\n    # Spark session and hadoop FS\n    spark_session = SparkSessionProvider().get_session()\n    df = spark_session.read.format(source_table.data_format).load(source_table.data_path)\n    df.write.format(target_table.data_format).save(target_table.data_path)\n```\n\nYou can also provision Spark Session using Kubernetes API server as a resource manager. Use Java options from the\nexample below for Java 17 installations:\n\n```python\nfrom spark_utils.common.spark_session_provider import SparkSessionProvider\nfrom spark_utils.models.k8s_config import SparkKubernetesConfig\n\nconfig = {\n    \'spark.local.dir\': \'/tmp\',\n    \'spark.driver.extraJavaOptions\': "-XX:+UseG1GC -XX:+UnlockDiagnosticVMOptions -XX:InitiatingHeapOccupancyPercent=35 -XX:OnOutOfMemoryError=\'kill -9 %p\' -XX:+IgnoreUnrecognizedVMOptions --add-opens=java.base/java.lang=ALL-UNNAMED --add-opens=java.base/java.lang.invoke=ALL-UNNAMED --add-opens=java.base/java.lang.reflect=ALL-UNNAMED --add-opens=java.base/java.io=ALL-UNNAMED --add-opens=java.base/java.net=ALL-UNNAMED --add-opens=java.base/java.nio=ALL-UNNAMED --add-opens=java.base/java.util=ALL-UNNAMED --add-opens=java.base/java.util.concurrent=ALL-UNNAMED --add-opens=java.base/java.util.concurrent.atomic=ALL-UNNAMED --add-opens=java.base/sun.nio.ch=ALL-UNNAMED --add-opens=java.base/sun.nio.cs=ALL-UNNAMED --add-opens=java.base/sun.security.action=ALL-UNNAMED --add-opens=java.base/sun.util.calendar=ALL-UNNAMED --add-opens=java.security.jgss/sun.security.krb5=ALL-UNNAMED --add-opens=java.base/java.util.stream=ALL-UNNAMED",\n    \'spark.executor.extraJavaOptions\': "-XX:+UseG1GC -XX:+UnlockDiagnosticVMOptions -XX:InitiatingHeapOccupancyPercent=35 -XX:OnOutOfMemoryError=\'kill -9 %p\' -XX:+IgnoreUnrecognizedVMOptions --add-opens=java.base/java.lang=ALL-UNNAMED --add-opens=java.base/java.lang.invoke=ALL-UNNAMED --add-opens=java.base/java.lang.reflect=ALL-UNNAMED --add-opens=java.base/java.io=ALL-UNNAMED --add-opens=java.base/java.net=ALL-UNNAMED --add-opens=java.base/java.nio=ALL-UNNAMED --add-opens=java.base/java.util=ALL-UNNAMED --add-opens=java.base/java.util.concurrent=ALL-UNNAMED --add-opens=java.base/java.util.concurrent.atomic=ALL-UNNAMED --add-opens=java.base/sun.nio.ch=ALL-UNNAMED --add-opens=java.base/sun.nio.cs=ALL-UNNAMED --add-opens=java.base/sun.security.action=ALL-UNNAMED --add-opens=java.base/sun.util.calendar=ALL-UNNAMED --add-opens=java.security.jgss/sun.security.krb5=ALL-UNNAMED --add-opens=java.base/java.util.stream=ALL-UNNAMED",\n    \'spark.executor.instances\': \'5\'\n}\n\nspc = SparkKubernetesConfig(\n  application_name=\'test\',\n  k8s_namespace=\'my-spark-namespace\',\n  spark_image=\'myregistry.io/spark:v3.3.1\',\n  executor_node_affinity={\n    \'kubernetes.mycompany.com/sparknodetype\': \'worker\', \n    \'kubernetes.azure.com/scalesetpriority\': \'spot\'\n  },\n  executor_name_prefix=\'spark-k8s-test\'\n)\nssp = SparkSessionProvider(additional_configs=config).configure_for_k8s(\n  master_url=\'https://my-k8s-cluster.mydomain.io\',\n  spark_config=spc\n)\n\nspark_session = ssp.get_session()\n```\n\nNow we can call this job directly or with `spark-submit`. Note that you must have `spark-utils` in PYTHONPATH before\nrunning the script:\n\n```commandline\nspark-submit --master local[*] --deploy-mode client --name simpleJob ~/path/to/main.py --source \'json_source|file://tmp/test_json/*|json\' --output \'parquet_target|file://tmp/test_parquet/*|parquet\'\n```\n\n- Job argument encryption is supported. This functionality requires an encryption key to be present in a cluster\n  environment variable `RUNTIME_ENCRYPTION_KEY`. The only supported algorithm now is `fernet`. You can declare an\n  argument as encrypted using `new_encrypted_arg` function. You then must pass an encrypted value to the declared\n  argument, which will be decrypted by `spark-utils` when a job is executed and passed to the consumer.\n\nFor example, you can pass sensitive spark configuration (storage access keys, hive database passwords etc.) encrypted:\n\n```python\nimport json\n\nfrom spark_utils.common.spark_job_args import SparkJobArgs\nfrom spark_utils.common.spark_session_provider import SparkSessionProvider\n\n\ndef main(args=None):\n    spark_args = SparkJobArgs()\n        .new_encrypted_arg("--custom-config", type=str, default=None,\n                           help="Optional spark configuration flags to pass. Will be treated as an encrypted value.")\n        .parse(args)\n\n    spark_session = SparkSessionProvider(\n        additional_configs=json.loads(\n            spark_args.parsed_args.custom_config) if spark_args.parsed_args.custom_config else None).get_session()\n\n    ...\n```\n\n- Delta Lake utilities\n    - Table publishing to Hive Metastore.\n    - Delta OSS compaction with row count / file optimization target.\n- Models for common data operations like data copying etc. Note that actual code for those operations will be migrated\n  to this repo a bit later.\n- Utility functions for common data operations, for example, flattening parent-child hierarchy, view concatenation,\n  column name clear etc.\n\nThere are so many possibilities with this project - please feel free to open an issue / PR adding new capabilities or\nfixing those nasty bugs!\n\n# Getting Started\n\nSpark Utils must be installed on your cluster or virtual env that Spark is using Python interpreter from:\n\n```commandline\npip install spark-utils\n```\n\n# Build and Test\n\nTest pipeline runs Spark in local mode, so everything can be tested against our current runtime. Update the image used\nin `build.yaml` if you require a test against a different runtime version.\n',
-    'author': 'ECCO Sneaks & Data',
-    'author_email': 'esdsupport@ecco.com',
-    'maintainer': 'GZU',
-    'maintainer_email': 'gzu@ecco.com',
-    'url': 'https://github.com/SneaksAndData/spark-utils',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.9,<4.0',
+Metadata-Version: 2.1
+Name: spark-utils
+Version: 1.1.0
+Summary: Utility classes for comfy Spark job authoriing.
+Home-page: https://github.com/SneaksAndData/spark-utils
+License: MIT
+Author: ECCO Sneaks & Data
+Author-email: esdsupport@ecco.com
+Maintainer: GZU
+Maintainer-email: gzu@ecco.com
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: k8s
+Requires-Dist: cryptography (>=36.0,<36.1)
+Requires-Dist: delta-spark (>=2.4.0,<2.5.0)
+Requires-Dist: hadoop-fs-wrapper (>=0.6.0,<0.7.0)
+Requires-Dist: kubernetes (==24.2.0) ; extra == "k8s"
+Project-URL: Repository, https://github.com/SneaksAndData/spark-utils
+Description-Content-Type: text/markdown
+
+# Introduction
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+Utility functions and classes for working with Dataframes, provisioning SparkSession and much more.
+
+Core features:
+
+- Provisioning Spark session with some routine settings set in advance, including Delta Lake configuration. You must
+  have delta-core jars in class path for this to work.
+- Spark job argument wrappers, allowing to specify job inputs for `spark.read.format(...).options(...).load(...)` and
+  outputs for `spark.write.format(...).save(...)` in a generic way. Those are exposed as `source` and `target` built-in
+  arguments (see example below).
+
+Consider a simple Spark Job that reads `json` data from `source` and stores it as `parquet` in `target`. This job can be
+defined using `spark-utils` as below:
+
+```python
+from spark_utils.common.spark_job_args import SparkJobArgs
+from spark_utils.common.spark_session_provider import SparkSessionProvider
+
+
+def main(args=None):
+    """
+     Job entrypoint
+    :param args:
+    :return:
+    """
+    spark_args = SparkJobArgs().parse(args)
+
+    source_table = spark_args.source('json_source')
+    target_table = spark_args.output('parquet_target')
+
+    # Spark session and hadoop FS
+    spark_session = SparkSessionProvider().get_session()
+    df = spark_session.read.format(source_table.data_format).load(source_table.data_path)
+    df.write.format(target_table.data_format).save(target_table.data_path)
+```
+
+You can also provision Spark Session using Kubernetes API server as a resource manager. Use Java options from the
+example below for Java 17 installations:
+
+```python
+from spark_utils.common.spark_session_provider import SparkSessionProvider
+from spark_utils.models.k8s_config import SparkKubernetesConfig
+
+config = {
+    'spark.local.dir': '/tmp',
+    'spark.driver.extraJavaOptions': "-XX:+UseG1GC -XX:+UnlockDiagnosticVMOptions -XX:InitiatingHeapOccupancyPercent=35 -XX:OnOutOfMemoryError='kill -9 %p' -XX:+IgnoreUnrecognizedVMOptions --add-opens=java.base/java.lang=ALL-UNNAMED --add-opens=java.base/java.lang.invoke=ALL-UNNAMED --add-opens=java.base/java.lang.reflect=ALL-UNNAMED --add-opens=java.base/java.io=ALL-UNNAMED --add-opens=java.base/java.net=ALL-UNNAMED --add-opens=java.base/java.nio=ALL-UNNAMED --add-opens=java.base/java.util=ALL-UNNAMED --add-opens=java.base/java.util.concurrent=ALL-UNNAMED --add-opens=java.base/java.util.concurrent.atomic=ALL-UNNAMED --add-opens=java.base/sun.nio.ch=ALL-UNNAMED --add-opens=java.base/sun.nio.cs=ALL-UNNAMED --add-opens=java.base/sun.security.action=ALL-UNNAMED --add-opens=java.base/sun.util.calendar=ALL-UNNAMED --add-opens=java.security.jgss/sun.security.krb5=ALL-UNNAMED --add-opens=java.base/java.util.stream=ALL-UNNAMED",
+    'spark.executor.extraJavaOptions': "-XX:+UseG1GC -XX:+UnlockDiagnosticVMOptions -XX:InitiatingHeapOccupancyPercent=35 -XX:OnOutOfMemoryError='kill -9 %p' -XX:+IgnoreUnrecognizedVMOptions --add-opens=java.base/java.lang=ALL-UNNAMED --add-opens=java.base/java.lang.invoke=ALL-UNNAMED --add-opens=java.base/java.lang.reflect=ALL-UNNAMED --add-opens=java.base/java.io=ALL-UNNAMED --add-opens=java.base/java.net=ALL-UNNAMED --add-opens=java.base/java.nio=ALL-UNNAMED --add-opens=java.base/java.util=ALL-UNNAMED --add-opens=java.base/java.util.concurrent=ALL-UNNAMED --add-opens=java.base/java.util.concurrent.atomic=ALL-UNNAMED --add-opens=java.base/sun.nio.ch=ALL-UNNAMED --add-opens=java.base/sun.nio.cs=ALL-UNNAMED --add-opens=java.base/sun.security.action=ALL-UNNAMED --add-opens=java.base/sun.util.calendar=ALL-UNNAMED --add-opens=java.security.jgss/sun.security.krb5=ALL-UNNAMED --add-opens=java.base/java.util.stream=ALL-UNNAMED",
+    'spark.executor.instances': '5'
 }
 
+spc = SparkKubernetesConfig(
+  application_name='test',
+  k8s_namespace='my-spark-namespace',
+  spark_image='myregistry.io/spark:v3.3.1',
+  executor_node_affinity={
+    'kubernetes.mycompany.com/sparknodetype': 'worker', 
+    'kubernetes.azure.com/scalesetpriority': 'spot'
+  },
+  executor_name_prefix='spark-k8s-test'
+)
+ssp = SparkSessionProvider(additional_configs=config).configure_for_k8s(
+  master_url='https://my-k8s-cluster.mydomain.io',
+  spark_config=spc
+)
+
+spark_session = ssp.get_session()
+```
+
+Now we can call this job directly or with `spark-submit`. Note that you must have `spark-utils` in PYTHONPATH before
+running the script:
+
+```commandline
+spark-submit --master local[*] --deploy-mode client --name simpleJob ~/path/to/main.py --source 'json_source|file://tmp/test_json/*|json' --output 'parquet_target|file://tmp/test_parquet/*|parquet'
+```
+
+- Job argument encryption is supported. This functionality requires an encryption key to be present in a cluster
+  environment variable `RUNTIME_ENCRYPTION_KEY`. The only supported algorithm now is `fernet`. You can declare an
+  argument as encrypted using `new_encrypted_arg` function. You then must pass an encrypted value to the declared
+  argument, which will be decrypted by `spark-utils` when a job is executed and passed to the consumer.
+
+For example, you can pass sensitive spark configuration (storage access keys, hive database passwords etc.) encrypted:
+
+```python
+import json
+
+from spark_utils.common.spark_job_args import SparkJobArgs
+from spark_utils.common.spark_session_provider import SparkSessionProvider
+
+
+def main(args=None):
+    spark_args = SparkJobArgs()
+        .new_encrypted_arg("--custom-config", type=str, default=None,
+                           help="Optional spark configuration flags to pass. Will be treated as an encrypted value.")
+        .parse(args)
+
+    spark_session = SparkSessionProvider(
+        additional_configs=json.loads(
+            spark_args.parsed_args.custom_config) if spark_args.parsed_args.custom_config else None).get_session()
+
+    ...
+```
+
+- Delta Lake utilities
+    - Table publishing to Hive Metastore.
+    - Delta OSS compaction with row count / file optimization target.
+- Models for common data operations like data copying etc. Note that actual code for those operations will be migrated
+  to this repo a bit later.
+- Utility functions for common data operations, for example, flattening parent-child hierarchy, view concatenation,
+  column name clear etc.
+
+There are so many possibilities with this project - please feel free to open an issue / PR adding new capabilities or
+fixing those nasty bugs!
+
+# Getting Started
+
+Spark Utils must be installed on your cluster or virtual env that Spark is using Python interpreter from:
+
+```commandline
+pip install spark-utils
+```
+
+# Build and Test
+
+Test pipeline runs Spark in local mode, so everything can be tested against our current runtime. Update the image used
+in `build.yaml` if you require a test against a different runtime version.
 
-setup(**setup_kwargs)
```

