# Comparing `tmp/visier-connector-0.9.4.tar.gz` & `tmp/visier-connector-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "visier-connector-0.9.4.tar", last modified: Wed Apr 26 17:26:29 2023, max compression
+gzip compressed data, was "visier-connector-0.9.5.tar", last modified: Mon May 29 22:29:30 2023, max compression
```

## Comparing `visier-connector-0.9.4.tar` & `visier-connector-0.9.5.tar`

### file list

```diff
@@ -1,18 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:26:29.567140 visier-connector-0.9.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-26 17:26:06.000000 visier-connector-0.9.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18640 2023-04-26 17:26:29.567140 visier-connector-0.9.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-26 17:26:06.000000 visier-connector-0.9.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-26 17:26:06.000000 visier-connector-0.9.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 17:26:29.567140 visier-connector-0.9.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:26:29.563140 visier-connector-0.9.4/visier/
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-26 17:26:06.000000 visier-connector-0.9.4/visier/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:26:29.563140 visier-connector-0.9.4/visier/connector/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-04-26 17:26:06.000000 visier-connector-0.9.4/visier/connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-04-26 17:26:06.000000 visier-connector-0.9.4/visier/connector/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-26 17:26:06.000000 visier-connector-0.9.4/visier/connector/sessions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 17:26:29.563140 visier-connector-0.9.4/visier_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18640 2023-04-26 17:26:29.000000 visier-connector-0.9.4/visier_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-26 17:26:29.000000 visier-connector-0.9.4/visier_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 17:26:29.000000 visier-connector-0.9.4/visier_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-26 17:26:29.000000 visier-connector-0.9.4/visier_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-26 17:26:29.000000 visier-connector-0.9.4/visier_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:29:30.195076 visier-connector-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-29 22:29:19.000000 visier-connector-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    24749 2023-05-29 22:29:30.191076 visier-connector-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-05-29 22:29:19.000000 visier-connector-0.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-29 22:29:19.000000 visier-connector-0.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 22:29:30.195076 visier-connector-0.9.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:29:30.191076 visier-connector-0.9.5/visier/
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-29 22:29:19.000000 visier-connector-0.9.5/visier/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:29:30.191076 visier-connector-0.9.5/visier/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-29 22:29:19.000000 visier-connector-0.9.5/visier/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2315 2023-05-29 22:29:19.000000 visier-connector-0.9.5/visier/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-05-29 22:29:19.000000 visier-connector-0.9.5/visier/api/direct_intake.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3756 2023-05-29 22:29:19.000000 visier-connector-0.9.5/visier/api/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-05-29 22:29:19.000000 visier-connector-0.9.5/visier/api/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:29:30.191076 visier-connector-0.9.5/visier/connector/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-29 22:29:19.000000 visier-connector-0.9.5/visier/connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-29 22:29:19.000000 visier-connector-0.9.5/visier/connector/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5445 2023-05-29 22:29:19.000000 visier-connector-0.9.5/visier/connector/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-29 22:29:19.000000 visier-connector-0.9.5/visier/connector/table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 22:29:30.191076 visier-connector-0.9.5/visier_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24749 2023-05-29 22:29:30.000000 visier-connector-0.9.5/visier_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-29 22:29:30.000000 visier-connector-0.9.5/visier_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 22:29:30.000000 visier-connector-0.9.5/visier_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-29 22:29:30.000000 visier-connector-0.9.5/visier_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-29 22:29:30.000000 visier-connector-0.9.5/visier_connector.egg-info/top_level.txt
```

### Comparing `visier-connector-0.9.4/LICENSE` & `visier-connector-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.4/PKG-INFO` & `visier-connector-0.9.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visier-connector
-Version: 0.9.4
+Version: 0.9.5
 Summary: Visier People Data connector
 Author-email: Visier Research & Development <info@visier.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -219,89 +219,188 @@
 ## Prerequisites
 The connector acts as a bridge between your Python application, which is typically Pandas-enabled, and Visier's cloud-hosted service infrastructure. In order to successfully connect to your Visier People data, you need:
 * The URL domain name prefix. For example: `https://{vanity-name}.api.visier.io`.
 * An API key issued by Visier.
 * A username identifying a user within your organization's Visier tenant who has been granted API access capabilities.
 * That user's password
 
-## Example
-This connector was authored with [Pandas](https://pandas.pydata.org/) in mind.
+## Connector Separation
+As of version `0.9.5`, the Python connector has separated the API calls from the `VisierSession` object. As a result of this change, the query execution methods on the `VisierSession` have been deprecated and will be subject to removal in a future release.
 
+The new way of invoking Visier public APIs through the Visier Python connector requires instantiating the appropriate API client and calling the methods defined on the client object. The following example, invokes the `analytic-objects` Model API to obtain the metadata for two analytic objects:
+```python
+    with VisierSession(auth) as session:
+        model_client = ModelApiClient(session)
+
+        objs = model_client.get_analytic_objects(["Requisition", "Employee_Exit"])
+        print(objs.text)
+```
+### Error handling
+By default, a failed API call will return `None` and information about the error is available on the client object. Using the example above, the last error in the event `objs` was `None` would be `model_client.last_error()`.
+
+It is however possible to force the API client to instead raise a `QueryExecutionException`. This is accomplished when instantiating the API client with the following parameter value `raise_on_error=True`. Using the example above, the `model_client` instantiation would look like this: `model_client = ModelApiClient(session, raise_on_error=True)`.
+
+# Examples
+## Query API
+The Query API Client is used to make calls to Visier's Query APIs. 
+
+**Note that the `examples` in this repository are not included in the `visier-connector` package** Instead, these `examples` should be copied into a sample application or the example queries can be run with a test script in this repository as per the snippets below.
+
+The Query API examples use [Pandas](https://pandas.pydata.org/) to illustrate a common data engineering and data science workflow using Visier data.
+ 
 A small set of example queries have been provided. Generally, Visier Query API queries fall into one of two categories:
 1. **Detail query** - These queries produce tabular results from underlying individual analytic objects. The shape of the result is inherently tabular with each table attribute represented as a column in the result set. Detail queries are often referred to as `list` or even `drill-through` queries. This query provides a detailed, non-aggregated view of the underlying analytical objects.
 1. **Aggregate query** - These queries aggregate metric values. They do so along the axes defined for the query and they produce multi-dimensional cell sets by default However, by providing an `Accept` header whose first value is either `application/jsonlines` or `text/csv`, the server will flatten the cell set into a tabular format when building the response.
 
 Visier also offers an experimental alternative to the JSON-based query definitions: SQL-like. This allows you to make queries using a language that comes close to SQL, which is generally more compact and intuitive. SQL-like allows definition of both aggregate and detail queries.
 
 :warning: **SQL-like is in alpha stage and not yet suitable for production use**.
 
 Example queries are provided through individual _files_. This is merely for convenience. SQL-like, being simple strings, can easily be provided to the call itself.
 
 In order to reduce duplication, each provided sample below should be preceded by the necessary `import` statements as well as authentication credential definition:
 ```python
 import os
 from visier.connector import Authentication, VisierSession
+from visier.api import QueryApiClient
 from examples import load_json, load_str
 import pandas as pd
 
 auth = Authentication(
     username = os.getenv("SOME_USERNAME"),
     password = os.getenv("SOME_PASSWORD"),
     host = os.getenv("SOME_HOST"),
     api_key = os.getenv("SOME_APIKEY"))
 ```
 
 ### Detail Query
 This is an example of a snippet that may be added to something that loads detailed data such as a Jupyter Notebook. Detailed data is essentially granular, non-aggregated data from Visier entities. For example, subjects such as `Employee` or events such as `Compensation_Payout`.
 ```python
-# List query from JSON query definition
-list_query = load_json("detail/employee-pay_level.json")
-list_result = s.executeList(list_query)
-df_list = pd.DataFrame.from_records(data=list_result.rows(), columns=list_result.header)
+with VisierSession(auth) as s:
+    client = QueryApiClient(s)
+    # List query from JSON query definition
+    list_query = load_json("detail/employee-pay_level.json")
+    list_result = client.list(list_query)
+    df_list = pd.DataFrame.from_records(data=list_result.rows(), columns=list_result.header)
 
-# ...
-print(df_list.head)
+    # ...
+    print(df_list.head)
 ```
 
 ### Aggregate Query
 Aggregate queries execute queries around Visier's predefined metrics. A metric is a calculation that targets a specific quantifiable question or scenario. They range from very simple like `employeeCount` to more complex ones like `hrRecruitingBudgetedLaborCostPerFTE`. 
 
 With a `VisierSession` available, an aggregate query is executed functionally identically:
 ```python
-# Aggregate query from JSON query definition
-aggregate_query = load_json("aggregate/applicants-source.json")
-aggregate_result = s.executeAggregate(aggregate_query)
-df_aggregate = pd.DataFrame.from_records(data=aggregate_result.rows(), columns=aggregate_result.header)
+with VisierSession(auth) as s:
+    client = QueryApiClient(s)
+    # Aggregate query from JSON query definition
+    aggregate_query = load_json("aggregate/applicants-source.json")
+    aggregate_result = client.aggregate(aggregate_query)
+    df_aggregate = pd.DataFrame.from_records(data=aggregate_result.rows(), columns=aggregate_result.header)
 
-# Now that the data is in a Pandas Data Frame, do something with it, or just...
-print(df_aggregate.head)
+    # Now that the data is in a Pandas Data Frame, do something with it, or just...
+    print(df_aggregate.head)
 ```
 
 ### SQL-like Queries
 SQL-like allows definition of both aggregate as well as detail queries:
 
 #### Detail Query
 ```python
-# SQL-like detail query
-sql_detail_query = load_str("sql-like/detail/employee-demo.sql")
-list_result = s.executeSqlLike(sql_detail_query)
-df_list = pd.DataFrame.from_records(data=list_result.rows(), columns=list_result.header)
+with VisierSession(auth) as s:
+    client = QueryApiClient(s)
+    # SQL-like detail query
+    sql_detail_query = load_str("sql-like/detail/employee-demo.sql")
+    list_result = client.sqllike(sql_detail_query)
+    df_list = pd.DataFrame.from_records(data=list_result.rows(), columns=list_result.header)
 
-# ...
-print(df_list.head)
+    # ...
+    print(df_list.head)
 ```
 
 #### Aggregate Query
 This example shows the query definition. Notice how the options object can be used to aggressively eliminate zero and null-valued cells for the purpose of reducing the size of the overall result set to only include rows whose metric value > 0.
 ```python
-# SQL-like aggregate query
-sql_aggregate_query = load_str("sql-like/aggregate/employee-count.sql")
-sparse_options = load_json("sql-like/options/sparse.json")
-aggregate_result = s.executeSqlLike(sql_aggregate_query, sparse_options)
-df_aggregate = pd.DataFrame.from_records(data=aggregate_result.rows(), columns=aggregate_result.header)
+with VisierSession(auth) as s:
+    client = QueryApiClient(s)
+    # SQL-like aggregate query
+    sql_aggregate_query = load_str("sql-like/aggregate/employee-count.sql")
+    sparse_options = load_json("sql-like/options/sparse.json")
+    aggregate_result = client.sqllike(sql_aggregate_query, sparse_options)
+    df_aggregate = pd.DataFrame.from_records(data=aggregate_result.rows(), columns=aggregate_result.header)
+
+    # ...
+    print(df_aggregate.head)
+```
+
+## Model API
+The Model API Client is used to make calls to the Visier Model API.
+In order to run the example below, ensure you add the following import statement to your program:
+```python
+from visier.api import ModelApiClient
+```
+
+In the example below, we query for the metadata for two named selection concepts on the `Requisition` analytic object:
+```python
+    with VisierSession(auth) as session:
+        model_client = ModelApiClient(session)
+
+        concepts = model_client.get_selection_concepts("Requisition", ["isRequisitionbyOtherIncomingReasons", "isActiveRequisition"])
+        print(concepts)
+```
+
+## Direct Intake API
+The Direct Intake API enable clients to load data whose structure already matches the target analytic object.
+Be sure to import the appropriate API client: `from visier.api import DirectIntakeApiClient`
+
+The instantiation of the API client follows the same pattern as both Query and Model. Regarding the semantics of the API, there are two points to be mindful of:
+1. The Direct Intake API is so called because this method of loading data into the Visier system relies on the source data already having been cleansed, deduplicated and transformed. Should these criteria not be met, then these APIs are not suitable for loading data, and alternative methods that leverage Visier's Data Provisioning data transformation mechanisms should be used instead.
+1. The call sequence follows a transactional pattern. A transaction is started, followed by a number of uploads after which the transaction is either committed or, in cases where the load should be aborted, rolled-back.
 
-# ...
-print(df_aggregate.head)
+:warning: Please be sure to read the product documentation to ensure the API calling principal has sufficient capabiltities to successfully make these calls.
+
+### Schema determination
+As this load mechanism is strictly dependent on the structure of the source files matching the schema of the target objects, a `schemas` API is available to query for the so called 'staging' schema of the target object:
+```python
+schema = intake_client.get_object_schema("Employee_Exit")
+```
+It's important to note that this schema is distinct from the so called 'analytic' schema obtained through the Model API. The 'analytic' schema will include elements that are used during query composition and will include artifacts whose values are derived from others. The 'staging' schema on the other hand, contains only key fields, simple properties, dimension and reference keys.
+
+### Load example
+Below is a simple example that shows loading data for Employee and Employee_Exit:
+```python
+    with VisierSession(auth) as session:
+        intake_client = DirectIntakeApiClient(session, raise_on_error=True)
+
+        try:
+            response = intake_client.start_transaction()
+            tx_id = response.json()["transactionId"]
+            print(f"Transaction ID: {tx_id}")
+
+            response = intake_client.upload_file(tx_id, "Employee", "/tmp/data/employee-data.zip")
+            print(response)
+
+            response = intake_client.upload_file(tx_id, "Employee_Exit", "/tmp/data/exits.csv")
+            print(response)
+            
+            response = intake_client.commit_transaction(tx_id)
+            print(response)
+        except:
+            print(f"Intake failed. Rolling back {tx_id}")
+            intake_client.rollback_transaction(tx_id)
+```
+
+### Any Visier public API
+While connector provides specific functions for querying data, it also provides a lower level, generic function for executing other public Visier APIs. Below is a simple example for determining which Plans have been defined for a given model:
+```python
+def get_location_levels(context: SessionContext) -> Response:
+    path = "/v1/data/model/plan-models/WorkforcePlanModel/plans"
+    return context.session().get(url=context.mk_url(path))
+
+with VisierSession(auth) as s:
+    levels = s.execute(get_location_levels)
+    print(levels.json())
 ```
 
 ## Installation
 Add `visier-connector` as a dependency to your module or install directly: `pip install -U visier-connector`
```

### Comparing `visier-connector-0.9.4/pyproject.toml` & `visier-connector-0.9.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["visier", "data", "query", "connector", "api"]
 license = {file = "LICENSE"}
 dynamic = ["version"]
 dependencies = [
     "requests >= 2.28",
+    "deprecated",
 ]
 
 [tool.poetry]
 readme = "README.md"
 
 [tool.setuptools.dynamic]
 version = {attr = "visier.__version__"}
```

### Comparing `visier-connector-0.9.4/visier/__init__.py` & `visier-connector-0.9.5/visier/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # You should have received a copy of the Apache License, Version 2.0
 # along with visier-connector-python. If not, see <https://www.apache.org/licenses/LICENSE-2.0>.
 
 """
 Visier Public Python Connector
 """
 
-__version__ = "0.9.4"
+__version__ = "0.9.5"
```

### Comparing `visier-connector-0.9.4/visier/connector/__init__.py` & `visier-connector-0.9.5/visier/connector/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 # along with visier-connector-python. If not, see <https://www.apache.org/licenses/LICENSE-2.0>.
 
 """
 Visier Public Python Connector
 """
 
 from .authentication import Authentication
-from .sessions import VisierSession, ResultTable, SessionContext, QueryExecutionError
+from .sessions import VisierSession, SessionContext, QueryExecutionError
+from .table import ResultTable
```

### Comparing `visier-connector-0.9.4/visier/connector/authentication.py` & `visier-connector-0.9.5/visier/connector/authentication.py`

 * *Files identical despite different names*

### Comparing `visier-connector-0.9.4/visier/connector/sessions.py` & `visier-connector-0.9.5/visier/connector/sessions.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,57 +11,38 @@
 # You should have received a copy of the Apache License, Version 2.0
 # along with visier-connector-python. If not, see <https://www.apache.org/licenses/LICENSE-2.0>.
 
 """
 Visier Session object through which JSON as well as SQL-like queries are executed.
 """
 
-import json
-import dataclasses
 from typing import Callable
 import requests
 from requests import Session, Response
-from visier.connector.authentication import Authentication
+from deprecated import deprecated
+from .table import ResultTable
+from .authentication import Authentication
 
-
-@dataclasses.dataclass
 class QueryExecutionError(Exception):
     """Description of error from executing a query"""
     def __init__(self, status_code, message) -> None:
         self.args = (f"""The query execution failed with the following
         HTTP status code: {status_code}
         The server returned the following description of the error:
         {message}""", )
+        self._status_code = status_code
+        self._message = message
 
-
-@dataclasses.dataclass
-class ResultTable:
-    """Tabular result set
-
-    Keyword args:
-    jsonlines -- JSON Lines representation of the entire result set.
-                 This is an array of strings, where each line will be
-                 parsed independently.
-
-    Class members:
-    header -- Array of column header strings.
-    rows() -- Row tuple generator
-    """
-    header = []
-
-    def __init__(self, gen_f) -> None:
-        self.header = json.loads(next(gen_f))
-        self._generator = gen_f
-
-
-    def rows(self):
-        """Returns a row tuple generator"""
-        for line in self._generator:
-            yield json.loads(line)
-
+    def status_code(self) -> int:
+        """Returns the HTTP status code"""
+        return self._status_code
+
+    def message(self) -> str:
+        """Returns the error message"""
+        return self._message
 
 class SessionContext:
     """
     Context object passed to the user-defined function in the execute() method.
     """
     def __init__(self, session: Session, host: str) -> None:
         self._session = session
@@ -83,22 +64,25 @@
     """
     HEADER = {"Accept": "application/jsonlines, application/json"}
 
     def __init__(self, auth: Authentication) -> None:
         self._auth = auth
         self._session = None
 
+    @deprecated(version="0.9.5", reason="Use visier.api.QueryApiClient instead")
     def execute_aggregate(self, query_def: object):
         """Execute a Visier aggregate query and return a tabular result."""
         return self._execute_query_api("/v1/data/query/aggregate", query_def)
 
+    @deprecated(version="0.9.5", reason="Use visier.api.QueryApiClient instead")
     def execute_list(self, query_def: object):
         """Execute a Visier list query and return a tabular result."""
         return self._execute_query_api("/v1/data/query/list", query_def)
 
+    @deprecated(version="0.9.5", reason="Use visier.api.QueryApiClient instead")
     def execute_sqllike(self, sql_query: str, options = None):
         """Execute a Visier SQL-like query statement and return a tabular result."""
         body = {"query" : sql_query}
         if options:
             body["options"] = options
         return self._execute_query_api("/v1/data/query/sql", body)
 
@@ -124,15 +108,15 @@
         return result
 
     def __enter__(self):
         self._connect()
         return self
 
     def __exit__(self, ex_type, ex_value, trace_back):
-        self._close()
+        self.close()
 
     def _execute_query_api(self, path: str, body: object):
         """Helper method for executing a query API with flattened result."""
         result = self.execute(lambda s: s.session().post(url=s.mk_url(path),
                                                          json=body,
                                                          headers=self.HEADER))
         return ResultTable(result.iter_lines())
@@ -147,9 +131,10 @@
 
         # Only create a requests.Session once we have a Visier ASID Token
         asid_token = result.text
         self._session = Session()
         self._session.cookies["VisierASIDToken"] = asid_token
         self._session.headers.update({"apikey": self._auth.api_key})
 
-    def _close(self):
+    def close(self):
+        """Close the session."""
         self._session.close()
```

### Comparing `visier-connector-0.9.4/visier_connector.egg-info/PKG-INFO` & `visier-connector-0.9.5/visier_connector.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: visier-connector
-Version: 0.9.4
+Version: 0.9.5
 Summary: Visier People Data connector
 Author-email: Visier Research & Development <info@visier.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -219,89 +219,188 @@
 ## Prerequisites
 The connector acts as a bridge between your Python application, which is typically Pandas-enabled, and Visier's cloud-hosted service infrastructure. In order to successfully connect to your Visier People data, you need:
 * The URL domain name prefix. For example: `https://{vanity-name}.api.visier.io`.
 * An API key issued by Visier.
 * A username identifying a user within your organization's Visier tenant who has been granted API access capabilities.
 * That user's password
 
-## Example
-This connector was authored with [Pandas](https://pandas.pydata.org/) in mind.
+## Connector Separation
+As of version `0.9.5`, the Python connector has separated the API calls from the `VisierSession` object. As a result of this change, the query execution methods on the `VisierSession` have been deprecated and will be subject to removal in a future release.
 
+The new way of invoking Visier public APIs through the Visier Python connector requires instantiating the appropriate API client and calling the methods defined on the client object. The following example, invokes the `analytic-objects` Model API to obtain the metadata for two analytic objects:
+```python
+    with VisierSession(auth) as session:
+        model_client = ModelApiClient(session)
+
+        objs = model_client.get_analytic_objects(["Requisition", "Employee_Exit"])
+        print(objs.text)
+```
+### Error handling
+By default, a failed API call will return `None` and information about the error is available on the client object. Using the example above, the last error in the event `objs` was `None` would be `model_client.last_error()`.
+
+It is however possible to force the API client to instead raise a `QueryExecutionException`. This is accomplished when instantiating the API client with the following parameter value `raise_on_error=True`. Using the example above, the `model_client` instantiation would look like this: `model_client = ModelApiClient(session, raise_on_error=True)`.
+
+# Examples
+## Query API
+The Query API Client is used to make calls to Visier's Query APIs. 
+
+**Note that the `examples` in this repository are not included in the `visier-connector` package** Instead, these `examples` should be copied into a sample application or the example queries can be run with a test script in this repository as per the snippets below.
+
+The Query API examples use [Pandas](https://pandas.pydata.org/) to illustrate a common data engineering and data science workflow using Visier data.
+ 
 A small set of example queries have been provided. Generally, Visier Query API queries fall into one of two categories:
 1. **Detail query** - These queries produce tabular results from underlying individual analytic objects. The shape of the result is inherently tabular with each table attribute represented as a column in the result set. Detail queries are often referred to as `list` or even `drill-through` queries. This query provides a detailed, non-aggregated view of the underlying analytical objects.
 1. **Aggregate query** - These queries aggregate metric values. They do so along the axes defined for the query and they produce multi-dimensional cell sets by default However, by providing an `Accept` header whose first value is either `application/jsonlines` or `text/csv`, the server will flatten the cell set into a tabular format when building the response.
 
 Visier also offers an experimental alternative to the JSON-based query definitions: SQL-like. This allows you to make queries using a language that comes close to SQL, which is generally more compact and intuitive. SQL-like allows definition of both aggregate and detail queries.
 
 :warning: **SQL-like is in alpha stage and not yet suitable for production use**.
 
 Example queries are provided through individual _files_. This is merely for convenience. SQL-like, being simple strings, can easily be provided to the call itself.
 
 In order to reduce duplication, each provided sample below should be preceded by the necessary `import` statements as well as authentication credential definition:
 ```python
 import os
 from visier.connector import Authentication, VisierSession
+from visier.api import QueryApiClient
 from examples import load_json, load_str
 import pandas as pd
 
 auth = Authentication(
     username = os.getenv("SOME_USERNAME"),
     password = os.getenv("SOME_PASSWORD"),
     host = os.getenv("SOME_HOST"),
     api_key = os.getenv("SOME_APIKEY"))
 ```
 
 ### Detail Query
 This is an example of a snippet that may be added to something that loads detailed data such as a Jupyter Notebook. Detailed data is essentially granular, non-aggregated data from Visier entities. For example, subjects such as `Employee` or events such as `Compensation_Payout`.
 ```python
-# List query from JSON query definition
-list_query = load_json("detail/employee-pay_level.json")
-list_result = s.executeList(list_query)
-df_list = pd.DataFrame.from_records(data=list_result.rows(), columns=list_result.header)
+with VisierSession(auth) as s:
+    client = QueryApiClient(s)
+    # List query from JSON query definition
+    list_query = load_json("detail/employee-pay_level.json")
+    list_result = client.list(list_query)
+    df_list = pd.DataFrame.from_records(data=list_result.rows(), columns=list_result.header)
 
-# ...
-print(df_list.head)
+    # ...
+    print(df_list.head)
 ```
 
 ### Aggregate Query
 Aggregate queries execute queries around Visier's predefined metrics. A metric is a calculation that targets a specific quantifiable question or scenario. They range from very simple like `employeeCount` to more complex ones like `hrRecruitingBudgetedLaborCostPerFTE`. 
 
 With a `VisierSession` available, an aggregate query is executed functionally identically:
 ```python
-# Aggregate query from JSON query definition
-aggregate_query = load_json("aggregate/applicants-source.json")
-aggregate_result = s.executeAggregate(aggregate_query)
-df_aggregate = pd.DataFrame.from_records(data=aggregate_result.rows(), columns=aggregate_result.header)
+with VisierSession(auth) as s:
+    client = QueryApiClient(s)
+    # Aggregate query from JSON query definition
+    aggregate_query = load_json("aggregate/applicants-source.json")
+    aggregate_result = client.aggregate(aggregate_query)
+    df_aggregate = pd.DataFrame.from_records(data=aggregate_result.rows(), columns=aggregate_result.header)
 
-# Now that the data is in a Pandas Data Frame, do something with it, or just...
-print(df_aggregate.head)
+    # Now that the data is in a Pandas Data Frame, do something with it, or just...
+    print(df_aggregate.head)
 ```
 
 ### SQL-like Queries
 SQL-like allows definition of both aggregate as well as detail queries:
 
 #### Detail Query
 ```python
-# SQL-like detail query
-sql_detail_query = load_str("sql-like/detail/employee-demo.sql")
-list_result = s.executeSqlLike(sql_detail_query)
-df_list = pd.DataFrame.from_records(data=list_result.rows(), columns=list_result.header)
+with VisierSession(auth) as s:
+    client = QueryApiClient(s)
+    # SQL-like detail query
+    sql_detail_query = load_str("sql-like/detail/employee-demo.sql")
+    list_result = client.sqllike(sql_detail_query)
+    df_list = pd.DataFrame.from_records(data=list_result.rows(), columns=list_result.header)
 
-# ...
-print(df_list.head)
+    # ...
+    print(df_list.head)
 ```
 
 #### Aggregate Query
 This example shows the query definition. Notice how the options object can be used to aggressively eliminate zero and null-valued cells for the purpose of reducing the size of the overall result set to only include rows whose metric value > 0.
 ```python
-# SQL-like aggregate query
-sql_aggregate_query = load_str("sql-like/aggregate/employee-count.sql")
-sparse_options = load_json("sql-like/options/sparse.json")
-aggregate_result = s.executeSqlLike(sql_aggregate_query, sparse_options)
-df_aggregate = pd.DataFrame.from_records(data=aggregate_result.rows(), columns=aggregate_result.header)
+with VisierSession(auth) as s:
+    client = QueryApiClient(s)
+    # SQL-like aggregate query
+    sql_aggregate_query = load_str("sql-like/aggregate/employee-count.sql")
+    sparse_options = load_json("sql-like/options/sparse.json")
+    aggregate_result = client.sqllike(sql_aggregate_query, sparse_options)
+    df_aggregate = pd.DataFrame.from_records(data=aggregate_result.rows(), columns=aggregate_result.header)
+
+    # ...
+    print(df_aggregate.head)
+```
+
+## Model API
+The Model API Client is used to make calls to the Visier Model API.
+In order to run the example below, ensure you add the following import statement to your program:
+```python
+from visier.api import ModelApiClient
+```
+
+In the example below, we query for the metadata for two named selection concepts on the `Requisition` analytic object:
+```python
+    with VisierSession(auth) as session:
+        model_client = ModelApiClient(session)
+
+        concepts = model_client.get_selection_concepts("Requisition", ["isRequisitionbyOtherIncomingReasons", "isActiveRequisition"])
+        print(concepts)
+```
+
+## Direct Intake API
+The Direct Intake API enable clients to load data whose structure already matches the target analytic object.
+Be sure to import the appropriate API client: `from visier.api import DirectIntakeApiClient`
+
+The instantiation of the API client follows the same pattern as both Query and Model. Regarding the semantics of the API, there are two points to be mindful of:
+1. The Direct Intake API is so called because this method of loading data into the Visier system relies on the source data already having been cleansed, deduplicated and transformed. Should these criteria not be met, then these APIs are not suitable for loading data, and alternative methods that leverage Visier's Data Provisioning data transformation mechanisms should be used instead.
+1. The call sequence follows a transactional pattern. A transaction is started, followed by a number of uploads after which the transaction is either committed or, in cases where the load should be aborted, rolled-back.
 
-# ...
-print(df_aggregate.head)
+:warning: Please be sure to read the product documentation to ensure the API calling principal has sufficient capabiltities to successfully make these calls.
+
+### Schema determination
+As this load mechanism is strictly dependent on the structure of the source files matching the schema of the target objects, a `schemas` API is available to query for the so called 'staging' schema of the target object:
+```python
+schema = intake_client.get_object_schema("Employee_Exit")
+```
+It's important to note that this schema is distinct from the so called 'analytic' schema obtained through the Model API. The 'analytic' schema will include elements that are used during query composition and will include artifacts whose values are derived from others. The 'staging' schema on the other hand, contains only key fields, simple properties, dimension and reference keys.
+
+### Load example
+Below is a simple example that shows loading data for Employee and Employee_Exit:
+```python
+    with VisierSession(auth) as session:
+        intake_client = DirectIntakeApiClient(session, raise_on_error=True)
+
+        try:
+            response = intake_client.start_transaction()
+            tx_id = response.json()["transactionId"]
+            print(f"Transaction ID: {tx_id}")
+
+            response = intake_client.upload_file(tx_id, "Employee", "/tmp/data/employee-data.zip")
+            print(response)
+
+            response = intake_client.upload_file(tx_id, "Employee_Exit", "/tmp/data/exits.csv")
+            print(response)
+            
+            response = intake_client.commit_transaction(tx_id)
+            print(response)
+        except:
+            print(f"Intake failed. Rolling back {tx_id}")
+            intake_client.rollback_transaction(tx_id)
+```
+
+### Any Visier public API
+While connector provides specific functions for querying data, it also provides a lower level, generic function for executing other public Visier APIs. Below is a simple example for determining which Plans have been defined for a given model:
+```python
+def get_location_levels(context: SessionContext) -> Response:
+    path = "/v1/data/model/plan-models/WorkforcePlanModel/plans"
+    return context.session().get(url=context.mk_url(path))
+
+with VisierSession(auth) as s:
+    levels = s.execute(get_location_levels)
+    print(levels.json())
 ```
 
 ## Installation
 Add `visier-connector` as a dependency to your module or install directly: `pip install -U visier-connector`
```

