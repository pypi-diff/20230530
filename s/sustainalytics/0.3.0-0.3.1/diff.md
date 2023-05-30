# Comparing `tmp/sustainalytics-0.3.0.tar.gz` & `tmp/sustainalytics-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sustainalytics-0.3.0.tar", max compression
+gzip compressed data, was "sustainalytics-0.3.1.tar", max compression
```

## Comparing `sustainalytics-0.3.0.tar` & `sustainalytics-0.3.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      777 2023-05-12 13:09:40.916939 sustainalytics-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     8007 2023-05-12 13:02:20.064810 sustainalytics-0.3.0/README.md
--rw-r--r--   0        0        0       23 2023-05-12 13:08:55.770785 sustainalytics-0.3.0/sustainalytics/__init__.py
--rw-r--r--   0        0        0    41747 2023-05-11 08:44:19.260290 sustainalytics-0.3.0/sustainalytics/api.py
--rw-r--r--   0        0        0     9139 1970-01-01 00:00:00.000000 sustainalytics-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      777 2023-05-30 12:41:48.948794 sustainalytics-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8007 2023-05-12 13:02:20.064810 sustainalytics-0.3.1/README.md
+-rw-r--r--   0        0        0       23 2023-05-30 12:34:40.467953 sustainalytics-0.3.1/sustainalytics/__init__.py
+-rw-r--r--   0        0        0    44341 2023-05-30 12:29:14.785687 sustainalytics-0.3.1/sustainalytics/api.py
+-rw-r--r--   0        0        0     9139 1970-01-01 00:00:00.000000 sustainalytics-0.3.1/PKG-INFO
```

### Comparing `sustainalytics-0.3.0/pyproject.toml` & `sustainalytics-0.3.1/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sustainalytics"
-version = "0.3.0"
+version = "0.3.1"
 description = "This is a package that helps clients access sustainalytics API"
 readme = "README.md"
 authors = ["Kienka Cromwell Kio <kienka.kio@morningstar.com>"]
 license = "MIT"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python :: 3",
```

### Comparing `sustainalytics-0.3.0/README.md` & `sustainalytics-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `sustainalytics-0.3.0/sustainalytics/api.py` & `sustainalytics-0.3.1/sustainalytics/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -554,14 +554,73 @@
         elif (parameter_values is not None) and (
                 isinstance(parameter_values, str) or isinstance(parameter_values, int)):
             all_parameters_values = all_parameters_values + ((str(parameter_name), parameter_values),)
             return all_parameters_values
         else:
             return all_parameters_values
 
+
+    def __get_endpoint_call_identifiers(self, params: tuple) -> list:
+        """Gets the identifiers used for the API call.
+
+        Args:
+            params: All the arguments used for in the API call.
+
+        Returns:
+            A list of identifiers.
+        """
+        identifiers_list = [args[1] for args in params if args[0] == 'identifiers']
+        identifiers_split = identifiers_list[0].split(",")
+        return identifiers_split
+
+    def __get_invalid_values_dataframe(self, params: tuple) -> pd.DataFrame:
+        """Creates a dataframe with the standard response for invalid identifiers passed in the API call.
+
+        Args:
+            params: All the arguments used for in the API call.
+
+        Returns:
+            Standard response for invalid identifiers in the API call.
+        """
+        identifiers_args = self.__get_endpoint_call_identifiers(params)
+        identifiers_args_unique = list(set(identifiers_args))
+        temp_data = pd.DataFrame(columns=['identifier', 'issuerId', 'issuerName', 'entityId',
+                                          'entityName', 'status'])
+        for row_number in range(len(identifiers_args_unique)):
+            temp_data.loc[row_number, 'identifier'] = identifiers_args_unique[row_number]
+            temp_data.loc[row_number, 'status'] = [{'matched': 'No', 'hasPermissions': False}]
+        return temp_data
+
+    def __endpoint_data_json_invalid_or_valid(self, request_response: list) -> list:
+        """Gets the right format of the endpoint response based on valid or invalid response (json format).
+
+        Args:
+            request_response: Response of the endpoint.
+
+        Returns:
+            The correct form to show the API response for json.
+        """
+        if "message" in request_response:
+            return [request_response]
+        return request_response
+
+    def __endpoint_data_df_invalid_or_valid(self, request_response: list, params: tuple) -> pd.DataFrame:
+        """Gets the right format of the endpoint response based on valid or invalid response (dataframe format).
+
+        Args:
+            request_response: Response of the endpoint.
+            params: All the arguments used for in the API call.
+
+        Returns:
+            The correct form to show the API response for dataframe.
+        """
+        if "message" in request_response:
+            return self.__get_invalid_values_dataframe(params)
+        return pd.DataFrame(request_response)
+
     def __get_endpoint_data(self, params: tuple, extracted_data: Union[list, pd.DataFrame], dtype: str,
                             endpoint: str) -> Union[list, pd.DataFrame]:
         """ Makes a GET request to the specified endpoint and returns it in the specified format.
 
         Args:
             params: Parameters for the request.
             extracted_data: Place where to store the data.
@@ -570,19 +629,19 @@
 
         Returns:
             A json or a dataframe with the extracted data.
         """
         requests_url = requests.get(f"https://api.sustainalytics.com/v2/{endpoint}",
                                     headers=self.access_headers, params=params, timeout=180).json()
         if dtype == 'json':
-            temp_data = requests_url
+            temp_data = self.__endpoint_data_json_invalid_or_valid(requests_url)
             extracted_data = extracted_data + temp_data
             return extracted_data
         else:
-            temp_data = pd.DataFrame(requests_url)
+            temp_data = self.__endpoint_data_df_invalid_or_valid(requests_url, params)
             extracted_data = pd.concat([extracted_data, temp_data], ignore_index=True)
             return extracted_data
 
     def __make_request_to_endpoint(self, all_parameter_values: tuple, extracted_data: Union[list, pd.DataFrame],
                                    endpoint: str, dtype: str) -> Union[list, pd.DataFrame]:
         """ Makes a request to a given V2 endpoint.
```

### Comparing `sustainalytics-0.3.0/PKG-INFO` & `sustainalytics-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sustainalytics
-Version: 0.3.0
+Version: 0.3.1
 Summary: This is a package that helps clients access sustainalytics API
 License: MIT
 Author: Kienka Cromwell Kio
 Author-email: kienka.kio@morningstar.com
 Requires-Python: >=3.6
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

