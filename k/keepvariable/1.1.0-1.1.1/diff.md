# Comparing `tmp/keepvariable-1.1.0.tar.gz` & `tmp/keepvariable-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keepvariable-1.1.0.tar", last modified: Thu May 25 15:04:02 2023, max compression
+gzip compressed data, was "keepvariable-1.1.1.tar", last modified: Tue May 30 18:24:05 2023, max compression
```

## Comparing `keepvariable-1.1.0.tar` & `keepvariable-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 15:04:02.235746 keepvariable-1.1.0/
--rw-rw-rw-   0        0        0     1247 2021-03-10 00:11:59.000000 keepvariable-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     2146 2023-05-25 15:04:02.234749 keepvariable-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1593 2023-04-10 03:42:53.000000 keepvariable-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 15:04:02.211811 keepvariable-1.1.0/keepvariable/
--rw-rw-rw-   0        0        0        0 2021-03-10 00:11:59.000000 keepvariable-1.1.0/keepvariable/__init__.py
--rw-rw-rw-   0        0        0     9285 2023-05-25 15:03:40.000000 keepvariable-1.1.0/keepvariable/keepvariable_core.py
--rw-rw-rw-   0        0        0      295 2021-03-10 00:11:59.000000 keepvariable-1.1.0/keepvariable/keepvariable_model.py
--rw-rw-rw-   0        0        0     1684 2023-05-25 15:03:40.000000 keepvariable-1.1.0/keepvariable/kv_redis_example.py
-drwxrwxrwx   0        0        0        0 2023-05-25 15:04:02.233751 keepvariable-1.1.0/keepvariable.egg-info/
--rw-rw-rw-   0        0        0     2146 2023-05-25 15:04:01.000000 keepvariable-1.1.0/keepvariable.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      332 2023-05-25 15:04:02.000000 keepvariable-1.1.0/keepvariable.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 15:04:01.000000 keepvariable-1.1.0/keepvariable.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-25 15:04:01.000000 keepvariable-1.1.0/keepvariable.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-25 15:04:01.000000 keepvariable-1.1.0/keepvariable.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 15:04:02.235746 keepvariable-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      800 2023-05-25 15:03:58.000000 keepvariable-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:24:05.793237 keepvariable-1.1.1/
+-rw-rw-rw-   0        0        0     1247 2021-03-10 00:11:59.000000 keepvariable-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2146 2023-05-30 18:24:05.792240 keepvariable-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1593 2023-04-10 03:42:53.000000 keepvariable-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 18:24:05.774287 keepvariable-1.1.1/keepvariable/
+-rw-rw-rw-   0        0        0        0 2021-03-10 00:11:59.000000 keepvariable-1.1.1/keepvariable/__init__.py
+-rw-rw-rw-   0        0        0    10523 2023-05-30 18:23:43.000000 keepvariable-1.1.1/keepvariable/keepvariable_core.py
+-rw-rw-rw-   0        0        0      295 2021-03-10 00:11:59.000000 keepvariable-1.1.1/keepvariable/keepvariable_model.py
+-rw-rw-rw-   0        0        0     1684 2023-05-25 15:03:40.000000 keepvariable-1.1.1/keepvariable/kv_redis_example.py
+drwxrwxrwx   0        0        0        0 2023-05-30 18:24:05.791242 keepvariable-1.1.1/keepvariable.egg-info/
+-rw-rw-rw-   0        0        0     2146 2023-05-30 18:24:05.000000 keepvariable-1.1.1/keepvariable.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      332 2023-05-30 18:24:05.000000 keepvariable-1.1.1/keepvariable.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 18:24:05.000000 keepvariable-1.1.1/keepvariable.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-30 18:24:05.000000 keepvariable-1.1.1/keepvariable.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-30 18:24:05.000000 keepvariable-1.1.1/keepvariable.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-30 18:24:05.793237 keepvariable-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      800 2023-05-30 18:24:02.000000 keepvariable-1.1.1/setup.py
```

### Comparing `keepvariable-1.1.0/LICENSE` & `keepvariable-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `keepvariable-1.1.0/PKG-INFO` & `keepvariable-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keepvariable
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python package keeping the values of variables between separate runs in a seamless and effortless way.
 Home-page: https://github.com/DovaX/keepvariable
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keepvariable-1.1.0/README.md` & `keepvariable-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `keepvariable-1.1.0/keepvariable/keepvariable_core.py` & `keepvariable-1.1.1/keepvariable/keepvariable_core.py`

 * *Files 16% similar despite different names*

```diff
@@ -131,30 +131,55 @@
    
     
 class KeepVariableDummyRedisServer:
     def __init__(self,host="localhost"):
         self.host=host
         self.storage={}
         
+    def _json_serialize_dataframe(self, df:pd.DataFrame) -> str:
+        """Takes a pandas DataFrame and serialized it to a json-like string.
+        The function uses pd.DataFrame().to_json() approach so as to handle various variable types with ease (pd.NA, pd.NaT, datetime etc.)
+
+        Example:
+            input: df2 = pd.DataFrame([[1,datetime.datetime.now(),3],[4,5,pd.NA],[pd.NaT,8,None]])
+            output: {"columns": [0, 1, 2], "data": [[1, 1685402664424, 3], [4, 5, null], [null, 8, null]], "object_type": "pd.DataFrame", "attrs": {}}'
+
+        Args:
+            df (pd.DataFrame): DataFrame to be serialized
+
+        Returns:
+            str: DataFrame serialized into json-like string
+        """        
+        df_json = df.to_json(orient='split')
+        df_as_dict = json.loads(df_json)
+        df_as_dict["object_type"] = 'pd.DataFrame'
+        df_as_dict["attrs"] = df.attrs
+        df_json = json.dumps(df_as_dict)
+        
+        return df_json
+        
     def parse_saved_value(self, value, additional_params: dict = {}):
         """Parses enterted value to json format. Certain special type values are serialized (DFs, datetimes, functions, classes).
 
         Args:
             value (Any): Entered value of any type (not all types can get serialized and stored however!)
             additional_params (dict, optional): Additional parameters used for serialization, e.g. for a function variable it's 
             code must be passed somehow --> additional_params = {'code': <function_code>}. Defaults to {}.
         """        
         if isinstance(value,list) or isinstance(value,bool) or isinstance(value,dict):
             value=json.dumps(value)
         elif isinstance(value,pd.DataFrame):
-            data=value.values.tolist()
-            columns=list(value.columns)
-            final_data={"columns":columns,"data":data,"object_type":"pd.DataFrame"}
-            print(final_data)
-            value=json.dumps(final_data)
+            value = self._json_serialize_dataframe(value)
+            #* Old implementation
+            # TODO: Keep for now, delete in following commits
+            # data=value.values.tolist()
+            # columns=list(value.columns)
+            # final_data={"columns":columns,"data":data,"object_type":"pd.DataFrame", "attrs": value.attrs}
+            # print(final_data)
+            # value=json.dumps(final_data)
         elif isinstance(value,np.ndarray):
             data=value.tolist()
             final_data={"data":data,"object_type":"np.ndarray"}
             value=json.dumps(final_data)
         elif isinstance(value, datetime.datetime):
             data=value.strftime("%Y-%m-%d %H:%M:%S")
             final_data = {"data": data, "object_type": "datetime.datetime"}
@@ -181,14 +206,15 @@
             Any: Parsed variable value
         """        
         try:
             value=json.loads(value)
             if "object_type" in value and isinstance(value,dict):
                 if value["object_type"]=="pd.DataFrame":
                     df=pd.DataFrame(value["data"],columns=value["columns"])
+                    df.attrs = value["attrs"]
                     return(df)
                 elif value["object_type"]=="np.ndarray":
                     array=pd.DataFrame(value["data"]).values #to ensure 64bit values in array
                     return(array)
                 elif value["object_type"] == "datetime.datetime":
                     datetime_value = datetime.datetime.strptime(value["data"],"%Y-%m-%d %H:%M:%S")
                     return datetime_value
```

### Comparing `keepvariable-1.1.0/keepvariable/kv_redis_example.py` & `keepvariable-1.1.1/keepvariable/kv_redis_example.py`

 * *Files identical despite different names*

### Comparing `keepvariable-1.1.0/keepvariable.egg-info/PKG-INFO` & `keepvariable-1.1.1/keepvariable.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keepvariable
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Python package keeping the values of variables between separate runs in a seamless and effortless way.
 Home-page: https://github.com/DovaX/keepvariable
 Author: DovaX
 Author-email: dovax.ai@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `keepvariable-1.1.0/setup.py` & `keepvariable-1.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
     
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setuptools.setup(
     name='keepvariable',
-    version='1.1.0',
+    version='1.1.1',
     author='DovaX',
     author_email='dovax.ai@gmail.com',
     description='A Python package keeping the values of variables between separate runs in a seamless and effortless way.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/DovaX/keepvariable',
     packages=setuptools.find_packages(),
```

