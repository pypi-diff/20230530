# Comparing `tmp/googleapiutils2-0.5.9.tar.gz` & `tmp/googleapiutils2-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googleapiutils2-0.5.9.tar", max compression
+gzip compressed data, was "googleapiutils2-0.6.0.tar", max compression
```

## Comparing `googleapiutils2-0.5.9.tar` & `googleapiutils2-0.6.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.5.9/LICENSE
--rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.5.9/README.md
--rw-r--r--   0        0        0       96 2023-01-30 06:00:44.616601 googleapiutils2-0.5.9/googleapiutils2/__init__.py
--rw-r--r--   0        0        0       25 2023-01-15 05:10:18.196566 googleapiutils2-0.5.9/googleapiutils2/drive/__init__.py
--rw-r--r--   0        0        0    20347 2023-05-23 20:00:42.933202 googleapiutils2-0.5.9/googleapiutils2/drive/drive.py
--rw-r--r--   0        0        0      314 2023-05-11 16:28:47.016831 googleapiutils2-0.5.9/googleapiutils2/drive/misc.py
--rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.5.9/googleapiutils2/geocode/__init__.py
--rw-r--r--   0        0        0     1040 2023-05-25 17:49:07.456779 googleapiutils2-0.5.9/googleapiutils2/geocode/geocode.py
--rw-r--r--   0        0        0     1178 2022-12-30 01:32:12.342148 googleapiutils2-0.5.9/googleapiutils2/geocode/misc.py
--rw-r--r--   0        0        0      118 2023-01-30 06:00:44.617619 googleapiutils2-0.5.9/googleapiutils2/sheets/__init__.py
--rw-r--r--   0        0        0     6494 2023-05-09 18:46:09.012912 googleapiutils2-0.5.9/googleapiutils2/sheets/misc.py
--rw-r--r--   0        0        0    17272 2023-05-25 18:19:15.621875 googleapiutils2-0.5.9/googleapiutils2/sheets/sheets.py
--rw-r--r--   0        0        0     4966 2023-05-25 18:06:02.584876 googleapiutils2-0.5.9/googleapiutils2/sheets/sheets_value_range.py
--rw-r--r--   0        0        0     7453 2023-05-30 14:27:56.280787 googleapiutils2-0.5.9/googleapiutils2/utils.py
--rw-r--r--   0        0        0      846 2023-05-30 14:30:30.639371 googleapiutils2-0.5.9/pyproject.toml
--rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.5.9/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.6.0/LICENSE
+-rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.6.0/README.md
+-rw-r--r--   0        0        0       96 2023-01-30 06:00:44.616601 googleapiutils2-0.6.0/googleapiutils2/__init__.py
+-rw-r--r--   0        0        0       25 2023-01-15 05:10:18.196566 googleapiutils2-0.6.0/googleapiutils2/drive/__init__.py
+-rw-r--r--   0        0        0    20347 2023-05-23 20:00:42.933202 googleapiutils2-0.6.0/googleapiutils2/drive/drive.py
+-rw-r--r--   0        0        0      314 2023-05-11 16:28:47.016831 googleapiutils2-0.6.0/googleapiutils2/drive/misc.py
+-rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.6.0/googleapiutils2/geocode/__init__.py
+-rw-r--r--   0        0        0     1040 2023-05-25 17:49:07.456779 googleapiutils2-0.6.0/googleapiutils2/geocode/geocode.py
+-rw-r--r--   0        0        0     1178 2022-12-30 01:32:12.342148 googleapiutils2-0.6.0/googleapiutils2/geocode/misc.py
+-rw-r--r--   0        0        0      118 2023-01-30 06:00:44.617619 googleapiutils2-0.6.0/googleapiutils2/sheets/__init__.py
+-rw-r--r--   0        0        0     6494 2023-05-09 18:46:09.012912 googleapiutils2-0.6.0/googleapiutils2/sheets/misc.py
+-rw-r--r--   0        0        0    20550 2023-05-30 20:16:51.953461 googleapiutils2-0.6.0/googleapiutils2/sheets/sheets.py
+-rw-r--r--   0        0        0     4966 2023-05-25 18:06:02.584876 googleapiutils2-0.6.0/googleapiutils2/sheets/sheets_value_range.py
+-rw-r--r--   0        0        0     7471 2023-05-30 19:56:34.731914 googleapiutils2-0.6.0/googleapiutils2/utils.py
+-rw-r--r--   0        0        0      846 2023-05-30 20:18:18.198374 googleapiutils2-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.6.0/PKG-INFO
```

### Comparing `googleapiutils2-0.5.9/LICENSE` & `googleapiutils2-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.9/README.md` & `googleapiutils2-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.9/googleapiutils2/drive/drive.py` & `googleapiutils2-0.6.0/googleapiutils2/drive/drive.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.9/googleapiutils2/geocode/geocode.py` & `googleapiutils2-0.6.0/googleapiutils2/geocode/geocode.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.9/googleapiutils2/geocode/misc.py` & `googleapiutils2-0.6.0/googleapiutils2/geocode/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.9/googleapiutils2/sheets/misc.py` & `googleapiutils2-0.6.0/googleapiutils2/sheets/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.9/googleapiutils2/sheets/sheets.py` & `googleapiutils2-0.6.0/googleapiutils2/sheets/sheets.py`

 * *Files 15% similar despite different names*

```diff
@@ -52,23 +52,24 @@
 
         self._cache: TTLCache = TTLCache(maxsize=128, ttl=80)
 
     def create(
         self,
         title: str,
         sheet_names: list[str] | None = None,
-        body: Spreadsheet | None = None,
+        body: Spreadsheet | None = None,  # type: ignore
     ):
-        body = nested_defaultdict(body if body else {})
+        body: Spreadsheet = nested_defaultdict(body if body else {})  # type: ignore
         sheet_names = sheet_names if sheet_names is not None else [DEFAULT_SHEET_NAME]
 
-        body["properties"]["title"] = title
+        body["properties"]["title"] = title  # type: ignore
         for n, sheet_name in enumerate(sheet_names):
-            body["sheets"][n]["properties"]["title"] = sheet_name
-        body["sheets"] = list(body["sheets"].values())
+            body["sheets"][n]["properties"]["title"] = sheet_name  # type: ignore
+
+        body["sheets"] = list(body["sheets"].values())  # type: ignore
 
         return self.sheets.create(body=body).execute()
 
     def copy_to(
         self,
         from_spreadsheet_id: str,
         from_sheet_id: int,
@@ -98,35 +99,150 @@
             )
             .execute()
         )
 
     def get(
         self,
         spreadsheet_id: str,
-    ):
+    ) -> Spreadsheet:
         spreadsheet_id = parse_file_id(spreadsheet_id)
         return self.sheets.get(spreadsheetId=spreadsheet_id).execute()
 
-    def get_by_sheet_name(
+    def get_sheet(
         self,
         spreadsheet_id: str,
         name: str | None = None,
         sheet_id: int | None = None,
-    ):
+    ) -> Sheet | None:
+        """Get a sheet from a spreadsheet. Either the name or the ID of the sheet must be provided.
+
+        Args:
+            spreadsheet_id (str): The ID of the spreadsheet containing the sheet to get.
+            name (str, optional): The name of the sheet to get. Defaults to None.
+            sheet_id (int, optional): The ID of the sheet to get. Defaults to None.
+        """
         spreadsheet_id = parse_file_id(spreadsheet_id)
         spreadsheet = self.get(spreadsheet_id)
 
         for sheet in spreadsheet["sheets"]:
             if sheet_id is not None and sheet["properties"]["sheetId"] == sheet_id:
                 return sheet
             if name is not None and sheet["properties"]["title"] == name:
                 return sheet
 
         return None
 
+    def rename_sheet(
+        self,
+        spreadsheet_id: str,
+        sheet_id: int,
+        new_name: str,
+    ):
+        """Rename a sheet in a spreadsheet.
+
+        Args:
+            spreadsheet_id (str): The ID of the spreadsheet containing the sheet to rename.
+            sheet_id (int): The ID of the sheet to rename.
+        """
+        spreadsheet_id = parse_file_id(spreadsheet_id)
+
+        body: BatchUpdateSpreadsheetRequest = {
+            "requests": [
+                {
+                    "updateSheetProperties": {
+                        "properties": {"sheetId": sheet_id, "title": new_name},
+                        "fields": "title",
+                    }
+                }
+            ]
+        }
+        return self.sheets.batchUpdate(
+            spreadsheetId=spreadsheet_id, body=body
+        ).execute()
+
+    def add_sheet(
+        self,
+        spreadsheet_id: str,
+        names: str | list[str],
+        rows: int = 1000,
+        cols: int = 26,
+        index: int | None = None,
+        **kwargs: Any,
+    ):
+        """Add one or more sheets to a spreadsheet.
+
+        Args:
+            spreadsheet_id (str): The ID of the spreadsheet to add sheets to.
+            names (str | list[str]): The name(s) of the sheet(s) to add.
+            rows (int, optional): The number of rows to add to each sheet. Defaults to 1000.
+            cols (int, optional): The number of columns to add to each sheet. Defaults to 26.
+            index (int, optional): The index at which to insert the sheet(s). Defaults to None.
+            **kwargs: Additional keyword arguments to pass to the API request."""
+        spreadsheet_id = parse_file_id(spreadsheet_id)
+        if isinstance(names, str):
+            names = [names]
+
+        def make_body(name: str) -> Sheet:
+            body: Sheet = {
+                "properties": {
+                    "title": name,
+                    "gridProperties": {
+                        "rowCount": rows,
+                        "columnCount": cols,
+                    },
+                },
+            }
+            if index is not None:
+                body["properties"]["index"] = index
+            return body
+
+        body: BatchUpdateSpreadsheetRequest = {
+            "requests": [
+                {
+                    "addSheet": make_body(name),
+                }
+                for name in names
+            ],
+        }
+
+        return self.sheets.batchUpdate(
+            spreadsheetId=spreadsheet_id,
+            body=body,
+            **kwargs,
+        ).execute()
+
+    def delete_sheet(
+        self,
+        spreadsheet_id: str,
+        sheet_id: int,
+        **kwargs: Any,
+    ):
+        """Deletes a sheet from a spreadsheet.
+
+        Args:
+            spreadsheet_id (str): The ID of the spreadsheet to delete the sheet from.
+            sheet_id (str): The ID of the sheet to delete.
+            **kwargs: Additional keyword arguments to pass to the API request.
+        """
+        spreadsheet_id = parse_file_id(spreadsheet_id)
+        body: BatchUpdateSpreadsheetRequest = {
+            "requests": [
+                {
+                    "deleteSheet": {
+                        "sheetId": sheet_id,
+                    },
+                },
+            ],
+        }
+        return self.sheets.batchUpdate(
+            spreadsheetId=spreadsheet_id,
+            body=body,
+            **kwargs,
+        ).execute()
+
     def values(
         self,
         spreadsheet_id: str,
         range_name: str | Any = DEFAULT_SHEET_NAME,
         value_render_option: ValueRenderOption = ValueRenderOption.unformatted,
         **kwargs: Any,
     ):
@@ -175,15 +291,15 @@
             frame = frame.reindex(
                 list(rows[0].keys()), axis=1
             )  # preserve the insertion order
             frame.index = frame.index.astype(str)
 
             if len(diff := frame.columns.difference(header)):
                 # only align columns if there are new columns
-                header: pd.Index = header.append(diff)
+                header = header.append(diff)
                 sheet_name, _ = reverse_sheet_range(range_name)
                 self.update(
                     spreadsheet_id,
                     SheetSlice[sheet_name, 1, ...],
                     [header.tolist()],
                 )
                 self._cache[(spreadsheet_id, sheet_name)] = list(header)
@@ -202,15 +318,15 @@
         values: list[list[Any]] | list[dict],
         align_columns: bool = True,
     ) -> list[list[Any]] | list[dict]:
         if all(isinstance(value, dict) for value in values):
             return self._dict_to_values_align_columns(
                 spreadsheet_id=spreadsheet_id,
                 range_name=range_name,
-                rows=values,
+                rows=values,  # type: ignore
                 align_columns=align_columns,
             )
         else:
             return values
 
     def update(
         self,
@@ -239,15 +355,15 @@
         values = self._process_values(spreadsheet_id, range_name, values, align_columns)
 
         return (
             self.sheets.values()
             .update(
                 spreadsheetId=spreadsheet_id,
                 range=range_name,
-                body={"values": values},
+                body={"values": values},  # type: ignore
                 valueInputOption=value_input_option.value,
             )
             .execute()
         )
 
     def batch_update(
         self,
@@ -275,15 +391,15 @@
                     spreadsheet_id=spreadsheet_id,
                     range_name=str_range_name,
                     values=values,
                     align_columns=align_columns,
                 ),
             }
             for range_name, values in data.items()
-        ]
+        ]  # type: ignore
 
         body: BatchUpdateValuesRequest = {
             "valueInputOption": value_input_option.value,
             "data": batch,
         }
         return (
             self.sheets.values()
@@ -313,19 +429,20 @@
             values (list[list[Any]]): The values to append.
             insert_data_option (InsertDataOption, optional): How the input data should be inserted. Defaults to InsertDataOption.overwrite.
             value_input_option (ValueInputOption, optional): How the input data should be interpreted. Defaults to ValueInputOption.user_entered.
             align_columns (bool, optional): Whether to align the columns of the spreadsheet with the keys of the first row of the values. Defaults to True.
         """
         spreadsheet_id = parse_file_id(spreadsheet_id)
         range_name = str(range_name)
-        body = {
+        body: ValueRange = {
             "values": self._process_values(
                 spreadsheet_id, range_name, values, align_columns
-            )
+            )  # type: ignore
         }
+
         return (
             self.sheets.values()
             .append(
                 spreadsheetId=spreadsheet_id,
                 range=range_name,
                 body=body,
                 insertDataOption=insert_data_option.value,
@@ -346,37 +463,14 @@
 
         return (
             self.sheets.values()
             .clear(spreadsheetId=spreadsheet_id, range=range_name)
             .execute()
         )
 
-    def rename_sheet(
-        self,
-        spreadsheet_id: str,
-        curr_name: str,
-        new_name: str,
-    ):
-        spreadsheet_id = parse_file_id(spreadsheet_id)
-        sheet = self.get(spreadsheet_id, curr_name)
-        sheet_id = sheet["properties"]["sheetId"]
-        body = {
-            "requests": [
-                {
-                    "updateSheetProperties": {
-                        "properties": {"sheetId": sheet_id, "title": new_name},
-                        "fields": "title",
-                    }
-                }
-            ]
-        }
-        return self.sheets.batchUpdate(
-            spreadsheetId=spreadsheet_id, body=body
-        ).execute()
-
     @staticmethod
     def to_frame(values: ValueRange, **kwargs: Any) -> pd.DataFrame | None:
         """Converts a ValueRange to a DataFrame.
         Useful for working with the data in Pandas after a call to sheets.values().
         If one of the keyword arguments to the dataframe is "columns",
         the first row of the values will be used as the column names, aligned to the data.
 
@@ -468,15 +562,15 @@
 
         Args:
             spreadsheet_id (str): The spreadsheet to update.
             sheet_name (str): The name of the sheet to update.
             width (int, optional): The width to set the columns to. Defaults to 100. If None, will auto-resize.
         """
         spreadsheet_id = parse_file_id(spreadsheet_id)
-        sheet = self.get_by_sheet_name(spreadsheet_id, name=sheet_name)
+        sheet = self.get_sheet(spreadsheet_id, name=sheet_name)
         if not sheet:
             raise ValueError(f"Sheet '{sheet_name}' not found in the given spreadsheet")
 
         body: BatchUpdateSpreadsheetRequest = {
             "requests": self._resize_columns(sheet, width)
         }
         return (
```

### Comparing `googleapiutils2-0.5.9/googleapiutils2/sheets/sheets_value_range.py` & `googleapiutils2-0.6.0/googleapiutils2/sheets/sheets_value_range.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.9/googleapiutils2/utils.py` & `googleapiutils2-0.6.0/googleapiutils2/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -232,15 +232,15 @@
         y.append(x % base)
         if (x := (x // base) - 1) < 0:
             break
 
     return y[::-1]
 
 
-def nested_defaultdict(existing: dict | Any | None = None, **kwargs: Any):
+def nested_defaultdict(existing: dict | Any | None = None, **kwargs: Any) -> dict[Any, Any]:
     if existing is None:
         existing = {}
     elif not isinstance(existing, dict):
         return existing
     existing = {key: nested_defaultdict(val) for key, val in existing.items()}
     return defaultdict(nested_defaultdict, existing, **kwargs)
```

### Comparing `googleapiutils2-0.5.9/pyproject.toml` & `googleapiutils2-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "googleapiutils2"
-version = "0.5.9"
+version = "0.6.0"
 description = "Wrapper for Google's Python API."
 authors = ["Mike Babb <mike7400@gmail.com>"]
 
 readme = "README.md"
 keywords = ["google", "googleapi", "googleapiutils2"]
 license = "MIT"
 repository = "https://github.com/mkbabb/googleapiutils2"
```

### Comparing `googleapiutils2-0.5.9/PKG-INFO` & `googleapiutils2-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googleapiutils2
-Version: 0.5.9
+Version: 0.6.0
 Summary: Wrapper for Google's Python API.
 Home-page: https://github.com/mkbabb/googleapiutils2
 License: MIT
 Keywords: google,googleapi,googleapiutils2
 Author: Mike Babb
 Author-email: mike7400@gmail.com
 Requires-Python: >=3.10,<4.0
```

