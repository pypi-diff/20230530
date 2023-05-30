# Comparing `tmp/googleapiutils2-0.5.8.tar.gz` & `tmp/googleapiutils2-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googleapiutils2-0.5.8.tar", max compression
+gzip compressed data, was "googleapiutils2-0.5.9.tar", max compression
```

## Comparing `googleapiutils2-0.5.8.tar` & `googleapiutils2-0.5.9.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.5.8/LICENSE
--rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.5.8/README.md
--rw-r--r--   0        0        0       96 2023-01-30 06:00:44.616601 googleapiutils2-0.5.8/googleapiutils2/__init__.py
--rw-r--r--   0        0        0       25 2023-01-15 05:10:18.196566 googleapiutils2-0.5.8/googleapiutils2/drive/__init__.py
--rw-r--r--   0        0        0    17597 2023-05-11 16:28:47.016478 googleapiutils2-0.5.8/googleapiutils2/drive/drive.py
--rw-r--r--   0        0        0      314 2023-05-11 16:28:47.016831 googleapiutils2-0.5.8/googleapiutils2/drive/misc.py
--rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.5.8/googleapiutils2/geocode/__init__.py
--rw-r--r--   0        0        0     1049 2022-12-30 01:32:12.342019 googleapiutils2-0.5.8/googleapiutils2/geocode/geocode.py
--rw-r--r--   0        0        0     1178 2022-12-30 01:32:12.342148 googleapiutils2-0.5.8/googleapiutils2/geocode/misc.py
--rw-r--r--   0        0        0      118 2023-01-30 06:00:44.617619 googleapiutils2-0.5.8/googleapiutils2/sheets/__init__.py
--rw-r--r--   0        0        0     6494 2023-05-09 18:46:09.012912 googleapiutils2-0.5.8/googleapiutils2/sheets/misc.py
--rw-r--r--   0        0        0    17179 2023-05-11 16:28:47.017272 googleapiutils2-0.5.8/googleapiutils2/sheets/sheets.py
--rw-r--r--   0        0        0     4925 2023-05-11 16:28:47.017646 googleapiutils2-0.5.8/googleapiutils2/sheets/sheets_value_range.py
--rw-r--r--   0        0        0     7387 2023-05-11 16:28:47.018058 googleapiutils2-0.5.8/googleapiutils2/utils.py
--rw-r--r--   0        0        0      817 2023-05-12 17:44:42.801832 googleapiutils2-0.5.8/pyproject.toml
--rw-r--r--   0        0        0     6375 1970-01-01 00:00:00.000000 googleapiutils2-0.5.8/setup.py
--rw-r--r--   0        0        0     6203 1970-01-01 00:00:00.000000 googleapiutils2-0.5.8/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-11 16:28:47.015700 googleapiutils2-0.5.9/LICENSE
+-rw-r--r--   0        0        0     5214 2023-05-11 16:28:47.015936 googleapiutils2-0.5.9/README.md
+-rw-r--r--   0        0        0       96 2023-01-30 06:00:44.616601 googleapiutils2-0.5.9/googleapiutils2/__init__.py
+-rw-r--r--   0        0        0       25 2023-01-15 05:10:18.196566 googleapiutils2-0.5.9/googleapiutils2/drive/__init__.py
+-rw-r--r--   0        0        0    20347 2023-05-23 20:00:42.933202 googleapiutils2-0.5.9/googleapiutils2/drive/drive.py
+-rw-r--r--   0        0        0      314 2023-05-11 16:28:47.016831 googleapiutils2-0.5.9/googleapiutils2/drive/misc.py
+-rw-r--r--   0        0        0       28 2022-12-30 01:32:12.341848 googleapiutils2-0.5.9/googleapiutils2/geocode/__init__.py
+-rw-r--r--   0        0        0     1040 2023-05-25 17:49:07.456779 googleapiutils2-0.5.9/googleapiutils2/geocode/geocode.py
+-rw-r--r--   0        0        0     1178 2022-12-30 01:32:12.342148 googleapiutils2-0.5.9/googleapiutils2/geocode/misc.py
+-rw-r--r--   0        0        0      118 2023-01-30 06:00:44.617619 googleapiutils2-0.5.9/googleapiutils2/sheets/__init__.py
+-rw-r--r--   0        0        0     6494 2023-05-09 18:46:09.012912 googleapiutils2-0.5.9/googleapiutils2/sheets/misc.py
+-rw-r--r--   0        0        0    17272 2023-05-25 18:19:15.621875 googleapiutils2-0.5.9/googleapiutils2/sheets/sheets.py
+-rw-r--r--   0        0        0     4966 2023-05-25 18:06:02.584876 googleapiutils2-0.5.9/googleapiutils2/sheets/sheets_value_range.py
+-rw-r--r--   0        0        0     7453 2023-05-30 14:27:56.280787 googleapiutils2-0.5.9/googleapiutils2/utils.py
+-rw-r--r--   0        0        0      846 2023-05-30 14:30:30.639371 googleapiutils2-0.5.9/pyproject.toml
+-rw-r--r--   0        0        0     6248 1970-01-01 00:00:00.000000 googleapiutils2-0.5.9/PKG-INFO
```

### Comparing `googleapiutils2-0.5.8/LICENSE` & `googleapiutils2-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.8/README.md` & `googleapiutils2-0.5.9/README.md`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.8/googleapiutils2/drive/drive.py` & `googleapiutils2-0.5.9/googleapiutils2/drive/drive.py`

 * *Files 9% similar despite different names*

```diff
@@ -104,14 +104,23 @@
         file_id: str,
         mime_type: GoogleMimeTypes,
         recursive: bool = False,
         conversion_map: dict[
             GoogleMimeTypes, tuple[GoogleMimeTypes, str]
         ] = DEFAULT_DOWNLOAD_CONVERSION_MAP,
     ) -> Path:
+        """Download a file from Google Drive. If the file is larger than 10MB, it will be downloaded in chunks.
+
+        Args:
+            out_filepath (FilePath): The path to the file to download to.
+            file_id (str): The ID of the file to download.
+            mime_type (GoogleMimeTypes): The mime type of the file to download.
+            recursive (bool, optional): If the file is a folder, download its contents recursively. Defaults to False.
+            conversion_map (dict[GoogleMimeTypes, tuple[GoogleMimeTypes, str]], optional): A dictionary mapping mime types to their corresponding file extensions. Defaults to DEFAULT_DOWNLOAD_CONVERSION_MAP.
+        """
         file_id = parse_file_id(file_id)
         out_filepath = Path(out_filepath)
 
         if recursive and mime_type == GoogleMimeTypes.folder:
             return self._download_nested_filepath(out_filepath, file_id)
 
         mime_type, ext = conversion_map.get(mime_type, (mime_type, ""))
@@ -200,20 +209,36 @@
             response = list_func(page_token)
             yield response
             if (page_token := response.get("nextPageToken", None)) is None:
                 break
 
     def list(
         self,
-        query: str,
+        query: str = "",
         fields: str = "*",
         order_by: str = "modifiedTime desc",
         team_drives: bool = True,
         **kwargs: Any,
     ) -> Iterable[File]:
+        """List files in Google Drive.
+
+        Example:
+            query = "name contains 'hello'"
+            fields = "files(id, name, mimeType, size, modifiedTime)"
+            order_by = "modifiedTime desc"
+            team_drives = True
+
+            files = drive.list(query=query, fields=fields, order_by=order_by, team_drives=team_drives)
+
+        Args:
+            query (str): The query to use to filter files. For more information see https://developers.google.com/drive/api/v3/search-files.
+            fields (str, optional): The fields to return. Defaults to "*". For more information see https://developers.google.com/drive/api/v3/reference/files/list.
+            order_by (str, optional): The order to return files in. Defaults to "modifiedTime desc".
+            team_drives (bool, optional): Whether to include files from Team Drives. Defaults to True.
+        """
         if team_drives:
             kwargs.update(
                 {"includeItemsFromAllDrives": True, "supportsAllDrives": True}
             )
 
         list_func = lambda x: self.files.list(
             q=query,
@@ -225,14 +250,20 @@
 
         for response in self._list(list_func):
             yield from response.get("files", [])
 
     def list_children(
         self, parent_id: str, fields: str = "*", **kwargs: Any
     ) -> Iterable[File]:
+        """List files in a folder.
+
+        Args:
+            parent_id (str): The ID of the folder to list files in.
+            fields (str, optional): The fields to return. Defaults to "*". For more information see https://developers.google.com/drive/api/v3/reference/files/list.
+        """
         parent_id = parse_file_id(parent_id)
         return self.list(
             query=f"{q_escape(parent_id)} in parents", fields=fields, **kwargs
         )
 
     def _query_children(self, name: str, parents: List[str], q: str | None = None):
         filename = Path(name)
@@ -265,14 +296,22 @@
         for file in self._query_children(name=name, parents=parents):
             return self.update(file["id"], filepath, supportsAllDrives=team_drives)
         return None
 
     def _create_nested_folders(
         self, filepath: Path, parents: List[str], update: bool = True
     ) -> List[str]:
+        """Create nested folders in Google Drive. Walks up the filepath creating folders as it goes.
+
+        Args:
+            filepath (Path): The filepath to create folders for.
+            parents (List[str]): The parent folders to create the folders in.
+            update (bool, optional): Whether to update the folder if it already exists. Defaults to True.
+        """
+
         def create_or_get_if_exists(name: str, parents: List[str]):
             folders = self._query_children(
                 name=name,
                 parents=parents,
                 q=f"mimeType='{GoogleMimeTypes.folder.value}'",
             )
             if update and (folder := next(folders, None)) is not None:
@@ -385,15 +424,14 @@
         Args:
             filepath (FilePath): The path to the file to upload.
             name (str, optional): The name of the file. Defaults to None, which will use the name of the file at the filepath.
             mime_type (GoogleMimeTypes, optional): The mime type of the file. Defaults to None, which will use the mime type of the file at the filepath.
             parents (List[str], optional): The list of parent IDs. Defaults to None.
             body (File, optional): The body of the file. Defaults to None.
             update (bool, optional): Whether to update the file if it already exists. Defaults to True.
-            **kwargs: Additional keyword arguments to pass to the underlying Google Drive API call.
         """
         filepath = Path(filepath)
         mime_type = (
             mime_type
             if mime_type is not None
             else GoogleMimeTypes[filepath.suffix.lstrip(".")]
         )
@@ -488,14 +526,23 @@
         file_id: str,
         email_address: str,
         permission: Permission | None = None,
         sendNotificationEmail: bool = True,
         update: bool = False,
         **kwargs: Any,
     ) -> Permission:
+        """Creates a permission for a file. Defaults to a reader permission of type user.
+
+        Args:
+            file_id (str): The ID of the file.
+            email_address (str): The email address of the user to give permission to.
+            permission (Permission, optional): The permission to give. Defaults to None, which will give a reader permission of type user.
+            sendNotificationEmail (bool, optional): Whether to send a notification email. Defaults to True.
+            update (bool, optional): Whether to update the permission if it already exists. Defaults to False.
+        """
         file_id = parse_file_id(file_id)
 
         user_permission: Permission = {
             "type": "user",
             "role": "reader",
             "emailAddress": email_address.strip().lower(),
         }
```

### Comparing `googleapiutils2-0.5.8/googleapiutils2/geocode/geocode.py` & `googleapiutils2-0.5.9/googleapiutils2/geocode/geocode.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
-from typing import *
 
 import requests
 from requests.exceptions import JSONDecodeError
 
 from ..utils import update_url_params
-from .misc import *
+from .misc import GeocodeResult
 
 
 class Geocode:
     URL = "https://maps.googleapis.com/maps/api/geocode/json"
 
     def __init__(self, api_key: str):
         self.api_key = api_key
```

### Comparing `googleapiutils2-0.5.8/googleapiutils2/geocode/misc.py` & `googleapiutils2-0.5.9/googleapiutils2/geocode/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.8/googleapiutils2/sheets/misc.py` & `googleapiutils2-0.5.9/googleapiutils2/sheets/misc.py`

 * *Files identical despite different names*

### Comparing `googleapiutils2-0.5.8/googleapiutils2/sheets/sheets.py` & `googleapiutils2-0.5.9/googleapiutils2/sheets/sheets.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     reverse_sheet_range,
 )
 
 if TYPE_CHECKING:
     from googleapiclient._apis.drive.v3.resources import File
     from googleapiclient._apis.sheets.v4.resources import (
         AppendValuesResponse,
+        BatchUpdateSpreadsheetRequest,
         BatchUpdateValuesRequest,
         BatchUpdateValuesResponse,
         ClearValuesResponse,
         CopySheetToAnotherSpreadsheetRequest,
         Sheet,
         SheetProperties,
         SheetsResource,
@@ -211,22 +212,22 @@
         else:
             return values
 
     def update(
         self,
         spreadsheet_id: str,
         range_name: str | Any,
-        values: list[list[Any]] | list[dict],
+        values: list[list[Any]] | list[dict] | list[Any],
         value_input_option: ValueInputOption = ValueInputOption.user_entered,
         align_columns: bool = True,
     ):
         """Updates a range of values in a spreadsheet.
 
-        If values is a list of dicts, the keys of the first dict will be used as the header row.
-        Further, if the input is a list of dicts and align_columns is True, the columns of the spreadsheet
+        If `values` is a list of dicts, the keys of the first dict will be used as the header row.
+        Further, if the input is a list of dicts and `align_columns` is True, the columns of the spreadsheet
         will be aligned with the keys of the first dict.
 
         Args:
             spreadsheet_id (str): The spreadsheet to update.
             range_name (str | Any): The range to update. Can be a string or a SheetSlice.
             values (list[list[Any]] | list[dict]): The values to update.
             value_input_option (ValueInputOption, optional): How the input data should be interpreted. Defaults to ValueInputOption.user_entered.
@@ -251,15 +252,15 @@
     def batch_update(
         self,
         spreadsheet_id: str,
         data: dict[str | Any, list[list[Any]] | list[dict]],
         value_input_option: ValueInputOption = ValueInputOption.user_entered,
         align_columns: bool = True,
     ):
-        """Updates a range of values in a spreadsheet. Much faster version of calling `update` multiple times.
+        """Updates a series of range values in a spreadsheet. Much faster version of calling `update` multiple times.
         See `update` for more details.
 
         Args:
             spreadsheet_id (str): The spreadsheet to update.
             data (dict): A dict of {range_name: values} to update;
                         values: list[list[Any]] | list[dict].
             value_input_option (ValueInputOption, optional): How the input data should be interpreted. Defaults to ValueInputOption.user_entered.
@@ -299,15 +300,16 @@
         range_name: str | Any,
         values: list[list[Any]],
         insert_data_option: InsertDataOption = InsertDataOption.overwrite,
         value_input_option: ValueInputOption = ValueInputOption.user_entered,
         align_columns: bool = True,
     ):
         """Appends values to a spreadsheet. Like `update`, but appends instead of overwrites.
-        This means rows will be added to the spreadsheet if the input values are longer than the existing rows.
+        This means rows will be added to the spreadsheet if the input values are longer than the
+        number of existing rows.
 
         Args:
             spreadsheet_id (str): The spreadsheet to update.
             range_name (str | Any): The range to update. Can be a string or a SheetSlice.
             values (list[list[Any]]): The values to append.
             insert_data_option (InsertDataOption, optional): How the input data should be inserted. Defaults to InsertDataOption.overwrite.
             value_input_option (ValueInputOption, optional): How the input data should be interpreted. Defaults to ValueInputOption.user_entered.
@@ -420,15 +422,15 @@
         df = df.astype(str)
 
         data: list = df.values.tolist()
         data.insert(0, list(df.columns))
         return data
 
     @staticmethod
-    def _resize_columns(sheet: Sheet, widths: int | list[int] | None = None):
+    def _resize_columns(sheet: Sheet, widths: int | list[int] | None = None) -> list:
         sheet_id = sheet["properties"]["sheetId"]
         num_columns = sheet["properties"]["gridProperties"]["columnCount"]
 
         make_range = lambda i: {
             "sheetId": sheet_id,
             "dimension": "COLUMNS",
             "startIndex": i,
@@ -470,15 +472,15 @@
             width (int, optional): The width to set the columns to. Defaults to 100. If None, will auto-resize.
         """
         spreadsheet_id = parse_file_id(spreadsheet_id)
         sheet = self.get_by_sheet_name(spreadsheet_id, name=sheet_name)
         if not sheet:
             raise ValueError(f"Sheet '{sheet_name}' not found in the given spreadsheet")
 
-        body: BatchUpdateValuesRequest = {
+        body: BatchUpdateSpreadsheetRequest = {
             "requests": self._resize_columns(sheet, width)
         }
         return (
             self.service.spreadsheets()
             .batchUpdate(spreadsheetId=spreadsheet_id, body=body)
             .execute()
         )
```

### Comparing `googleapiutils2-0.5.8/googleapiutils2/sheets/sheets_value_range.py` & `googleapiutils2-0.5.9/googleapiutils2/sheets/sheets_value_range.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,22 +68,21 @@
     def header(self) -> list[str]:
         return self.sheets._header(
             spreadsheet_id=self.spreadsheet_id, sheet_name=self.sheet_name
         )
 
     @cachedmethod(operator.attrgetter("_cache"))
     def shape(self) -> tuple[int, int]:
-        for sheet in self.sheets.get(self.spreadsheet_id)["sheets"]:
-            properties = sheet["properties"]
-
-            if properties["title"] == self.sheet_name:
-                grid_properties = properties["gridProperties"]
+        for sheet in self.sheets.get(self.spreadsheet_id).get("sheets", []):
+            properties = sheet.get("properties", {})
+            if properties.get("title") == self.sheet_name:
+                grid_properties = properties.get("gridProperties", {})
                 return (
-                    grid_properties["rowCount"],
-                    grid_properties["columnCount"],
+                    grid_properties.get("rowCount", 0),
+                    grid_properties.get("columnCount", 0),
                 )
         return DEFAULT_SHEET_SHAPE
 
     def values(
         self,
         value_render_option: ValueRenderOption = ValueRenderOption.unformatted,
     ):
@@ -106,16 +105,16 @@
             value_input_option=value_input_option,
             align_columns=align_columns,
         )
 
     def rename(self, new_sheet_name: str):
         return self.sheets.rename_sheet(
             spreadsheet_id=self.spreadsheet_id,
-            sheet_name=self.sheet_name,
-            new_sheet_name=new_sheet_name,
+            curr_name=self.sheet_name,
+            new_name=new_sheet_name,
         )
 
     def append(
         self,
         values: list[list[Any]],
         insert_data_option: InsertDataOption = InsertDataOption.overwrite,
         value_input_option: ValueInputOption = ValueInputOption.user_entered,
@@ -131,15 +130,15 @@
         )
 
     def clear(self):
         return self.sheets.clear(
             spreadsheet_id=self.spreadsheet_id, range_name=str(self)
         )
 
-    def to_frame(self, **kwargs) -> pd.DataFrame:
+    def to_frame(self, **kwargs) -> pd.DataFrame | None:
         return self.sheets.to_frame(self.values(), **kwargs)
 
     def __getitem__(self, ixs: Any) -> SheetsValueRange:
         slc = SheetSliceT(
             sheet_name=self.sheet_name, range_name=self.range_name, shape=self.shape()
         )[ixs]
         return self.__class__(
```

### Comparing `googleapiutils2-0.5.8/googleapiutils2/utils.py` & `googleapiutils2-0.5.9/googleapiutils2/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     return f"'{s}'"
 
 
 def get_oauth2_creds(
     client_config: FilePath | dict = CONFIG_PATH,
     token_path: FilePath = TOKEN_PATH,
     scopes: List[str] = SCOPES,
-) -> Optional[Credentials]:
+) -> Credentials:
     """Get OAuth2 credentials for Google API.
 
     This will automatically detect if the credentials are for a service account.
     If it's not, it will try to load the token from the token path (defaults to TOKEN_PATH)
     and refresh it. The token will be saved to the token path.
 
     Args:
@@ -135,36 +135,36 @@
 
     token_path = Path(token_path)
 
     if not isinstance(client_config, dict):
         path = Path(client_config)
         client_config = json.loads(path.read_bytes())
 
-    is_service_account = client_config.get("type", "") == "service_account"
+    is_service_account = client_config.get("type", "") == "service_account"  # type: ignore
 
-    if not is_service_account:
-        creds: Credentials = None
+    if is_service_account:
+        return service_account.Credentials.from_service_account_info(
+            client_config, scopes=scopes
+        )  # type: ignore
+    else:
+        creds: Credentials = None  # type: ignore
 
         if token_path.exists():
             creds = pickle.loads(token_path.read_bytes())
 
         if creds is not None and not creds.valid:
             if creds.expired and creds.refresh_token:
                 creds.refresh(Request())
 
         elif creds is None:
             flow = InstalledAppFlow.from_client_config(client_config, scopes)
-            creds = flow.run_local_server(port=0)
+            creds = flow.run_local_server(port=0)  # type: ignore
             token_path.write_bytes(pickle.dumps(creds))
 
-        return creds
-    else:
-        return service_account.Credentials.from_service_account_info(
-            client_config, scopes=scopes
-        )
+        return creds  # type: ignore
 
 
 def download_large_file(
     url: str, filepath: FilePath, chunk_size=googleapiclient.http.DEFAULT_CHUNK_SIZE
 ) -> Path:
     filepath = Path(filepath)
```

### Comparing `googleapiutils2-0.5.8/pyproject.toml` & `googleapiutils2-0.5.9/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 [tool.poetry]
 name = "googleapiutils2"
-version = "0.5.8"
+version = "0.5.9"
 description = "Wrapper for Google's Python API."
 authors = ["Mike Babb <mike7400@gmail.com>"]
+
 readme = "README.md"
 keywords = ["google", "googleapi", "googleapiutils2"]
 license = "MIT"
 repository = "https://github.com/mkbabb/googleapiutils2"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-pandas = "^2.0.1"
+pandas = "^2.0.2"
 mypy = "^1.3.0"
-google-api-python-client-stubs = "^1.16.0"
-google-api-python-client = "^2.86.0"
+google-api-python-client-stubs = "^1.17.0"
+google-api-python-client = "^2.88.0"
 google-auth-oauthlib = "^1.0.0"
-requests = "^2.30.0"
-cachetools = "^5.3.0"
+requests = "^2.31.0"
+cachetools = "^5.3.1"
 google-auth-httplib2 = "^0.1.0"
+google-auth = "^2.19.0"
 
 [tool.poetry.group.dev.dependencies]
-types-requests = "^2.30.0"
-types-cachetools = "^5.3.0"
-pytest = "^7.2.0"
+types-requests = "^2.31.0.1"
+types-cachetools = "^5.3.0.5"
+pytest = "^7.3.1"
 pandas-stubs = "^2.0.1.230501"
 black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `googleapiutils2-0.5.8/setup.py` & `googleapiutils2-0.5.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,180 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: googleapiutils2
+Version: 0.5.9
+Summary: Wrapper for Google's Python API.
+Home-page: https://github.com/mkbabb/googleapiutils2
+License: MIT
+Keywords: google,googleapi,googleapiutils2
+Author: Mike Babb
+Author-email: mike7400@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: cachetools (>=5.3.1,<6.0.0)
+Requires-Dist: google-api-python-client (>=2.88.0,<3.0.0)
+Requires-Dist: google-api-python-client-stubs (>=1.17.0,<2.0.0)
+Requires-Dist: google-auth (>=2.19.0,<3.0.0)
+Requires-Dist: google-auth-httplib2 (>=0.1.0,<0.2.0)
+Requires-Dist: google-auth-oauthlib (>=1.0.0,<2.0.0)
+Requires-Dist: mypy (>=1.3.0,<2.0.0)
+Requires-Dist: pandas (>=2.0.2,<3.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
+Project-URL: Repository, https://github.com/mkbabb/googleapiutils2
+Description-Content-Type: text/markdown
 
-packages = \
-['googleapiutils2',
- 'googleapiutils2.drive',
- 'googleapiutils2.geocode',
- 'googleapiutils2.sheets']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['cachetools>=5.3.0,<6.0.0',
- 'google-api-python-client-stubs>=1.16.0,<2.0.0',
- 'google-api-python-client>=2.86.0,<3.0.0',
- 'google-auth-httplib2>=0.1.0,<0.2.0',
- 'google-auth-oauthlib>=1.0.0,<2.0.0',
- 'mypy>=1.3.0,<2.0.0',
- 'pandas>=2.0.1,<3.0.0',
- 'requests>=2.30.0,<3.0.0']
-
-setup_kwargs = {
-    'name': 'googleapiutils2',
-    'version': '0.5.8',
-    'description': "Wrapper for Google's Python API.",
-    'long_description': '# googleapiutils2\n\nUtilities for\n[Google\'s v2 Python API](https://github.com/googleapis/google-api-python-client).\nCurrently supports sections of the following resources:\n\n-   [Drive](https://developers.google.com/drive/api/reference/rest/v3): `DriveResource`,\n    `FilesResource`, `PermissionsResource`, `RepliesResource`, `...`\n-   [Sheets](https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets):\n    `SpreadsheetsResource`, `ValuesResource`, `...`\n-   [Geocoding](https://developers.google.com/maps/documentation/geocoding/overview)\n\n## Quickstart\n\nThis project requires Python `^3.10` to run.\n\nSeveral dependencies are needed, namely the aforesaid Google Python API, but also\nGoogle\'s oauth library, and `requests`. Pre-bundled for ease of use are the fairly\nmonolithic `google-api-stubs`, which greatly improves the usage experience.\n\n### via [`poetry`](https://python-poetry.org/docs/)\n\nInstall poetry, then run\n\n> poetry install\n\nAnd you\'re done.\n\n## Overview\n\nThe library was written to be consistent with Google\'s own Python API - just a little\neasier to use. Most `Drive` and `Sheets` operations are supported using explicit\nparameters. But most functions thereof take a `**kwargs` parameter (used for parameter\nforwarding) to allow for the more granular usage of the underlying API.\n\nA note on IDs: anytime a resource ID is needed, one can be provide the actual resource\nID, or the URL to the resource. If a URL is provided, this mapping is cached for future\nuse.\n\n## Authentication\n\nBefore using a `Drive` or `Sheets` object, one must first authenticate. This is done via\nthe `google.oauth2` library, creating a `Credentials` object.\n\nThe library supports two methods of authentication:\n\n-   via a Google service account (recommended, see more\n    [here](https://cloud.google.com/iam/docs/creating-managing-service-accounts))\n-   via OAuth2 (see more\n    [here](https://developers.google.com/identity/protocols/oauth2/native-app))\n\nWith a service account, one can programmatically access resources without user input.\nThis is by far the easiest route, but requires a bit of setup.\n\nIf not using a service account, the library will attempt to open a browser window to\nauthenticate using the provided credentials. This authentication is cached for future\nusage (though it does expire on some interval) - so an valid token path is required.\n\nSee the [`get_oauth2_creds`](googleapiutils2/utils.py) function for more information.\n\n## Drive\n\nExample: copy a file to a folder.\n\n```python\ncreds = get_oauth2_creds(config_obj)\ndrive = Drive(creds)\n\nfilename = "Heyy"\n\nfile = drive.get_name(filename, parents=[FOLDER_URL])\nif file is not None:\n    drive.delete(file["id"])\n\nfile = drive.copy(file_id=FILE_ID, to_filename=filename, to_folder_id=FOLDER_URL)\n```\n\nWhat the above does is:\n\n-   Get the OAuth2 credentials from the `config_obj` object (JSON object representing\n    the requisite credentials, see\n    [here](https://developers.google.com/identity/protocols/oauth2/native-app#step-2:-send-a-request-to-googles-oauth-2.0-server)\n    for more information).\n-   create a `Drive` object thereupon.\n-   Get the file with the given name, and delete it if it exists.\n-   Copy the file with the given ID to the given folder, and return the new file.\n\n## Sheets\n\nExample: update a range of cells in a sheet.\n\n```python\ncreds = get_oauth2_creds(config_path)\nsheets = Sheets(creds)\n\nSheet1 = SheetsValueRange(sheets, SHEET_ID, sheet_name="Sheet1")\n\nrows = [\n    {\n        "Heyy": "99",\n    }\n]\nSheet1[2:3, ...].update(rows)\n```\n\nWhat the above does is:\n\n-   Get the OAuth2 credentials from the `config_path` file (see\n    [here](https://developers.google.com/identity/protocols/oauth2/native-app#step-2:-send-a-request-to-googles-oauth-2.0-server)\n    for more information).\n-   create a `Sheets` object thereupon.\n-   Create a `SheetsValueRange` object, which is a wrapper around the\n    `spreadsheets.values` API.\n-   Update the range `Sheet1!A2:B3` with the given rows.\n\nNote the slicing syntax, which will feel quite familiar for any user of Numpy or Pandas.\n\n### SheetSlice\n\nA `SheetsValueRange` object can be sliced in a similar manner to that of a Numpy array.\nThe syntax is as follows:\n\n    slc = Sheet[rows, cols]\n\nWherein `rows` and `cols` are either integers, slices of integers (stride is not\nsupported), strings (in A1 notation), or ellipses (`...`).\n\nNote that Google\'s implementation of A1 notation is 1-indexed; 0 is invalid (e.g., 1\nmaps to `A`, 2 to `B`, etc.)\n\n```py\nix = SheetSlice["Sheet1", 1:3, 2:4] #  "Sheet1!B2:D4"\nix = SheetSlice["Sheet1", "A1:B2"]  #  "Sheet1!A1:B2"\nix = SheetSlice[1:3, 2:4]           #  "Sheet1!B2:D4"\nix = SheetSlice["A1:B2"]            #  "Sheet1!A1:B2"\nix = SheetSlice[..., 1:3]           #  "Sheet1!A1:Z3"\n\nvalues = {\n    SheetSlice["A1:B2"]: [\n        ["Heyy", "99"],\n        ["Heyy", "99"],\n    ],\n} # "Sheet1!A1:B2" = [["Heyy", "99"], ["Heyy", "99"]]\n```\n\nA `SheetSlice` can also be used as a key into a `SheetsValueRange`, or a dictionary (to\nuse in updating a sheet\'s range via `.update()`, for example). Further, a\n`SheetsValueRange` can be sliced in a similar manner to that of a `SheetSlice`.\n\n```py\nSheet1[2:3, ...].update(rows)\n...\n```\n',
-    'author': 'Mike Babb',
-    'author_email': 'mike7400@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/mkbabb/googleapiutils2',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
+# googleapiutils2
 
+Utilities for
+[Google's v2 Python API](https://github.com/googleapis/google-api-python-client).
+Currently supports sections of the following resources:
+
+-   [Drive](https://developers.google.com/drive/api/reference/rest/v3): `DriveResource`,
+    `FilesResource`, `PermissionsResource`, `RepliesResource`, `...`
+-   [Sheets](https://developers.google.com/sheets/api/reference/rest/v4/spreadsheets):
+    `SpreadsheetsResource`, `ValuesResource`, `...`
+-   [Geocoding](https://developers.google.com/maps/documentation/geocoding/overview)
+
+## Quickstart
+
+This project requires Python `^3.10` to run.
+
+Several dependencies are needed, namely the aforesaid Google Python API, but also
+Google's oauth library, and `requests`. Pre-bundled for ease of use are the fairly
+monolithic `google-api-stubs`, which greatly improves the usage experience.
+
+### via [`poetry`](https://python-poetry.org/docs/)
+
+Install poetry, then run
+
+> poetry install
+
+And you're done.
+
+## Overview
+
+The library was written to be consistent with Google's own Python API - just a little
+easier to use. Most `Drive` and `Sheets` operations are supported using explicit
+parameters. But most functions thereof take a `**kwargs` parameter (used for parameter
+forwarding) to allow for the more granular usage of the underlying API.
+
+A note on IDs: anytime a resource ID is needed, one can be provide the actual resource
+ID, or the URL to the resource. If a URL is provided, this mapping is cached for future
+use.
+
+## Authentication
+
+Before using a `Drive` or `Sheets` object, one must first authenticate. This is done via
+the `google.oauth2` library, creating a `Credentials` object.
+
+The library supports two methods of authentication:
+
+-   via a Google service account (recommended, see more
+    [here](https://cloud.google.com/iam/docs/creating-managing-service-accounts))
+-   via OAuth2 (see more
+    [here](https://developers.google.com/identity/protocols/oauth2/native-app))
+
+With a service account, one can programmatically access resources without user input.
+This is by far the easiest route, but requires a bit of setup.
+
+If not using a service account, the library will attempt to open a browser window to
+authenticate using the provided credentials. This authentication is cached for future
+usage (though it does expire on some interval) - so an valid token path is required.
+
+See the [`get_oauth2_creds`](googleapiutils2/utils.py) function for more information.
+
+## Drive
+
+Example: copy a file to a folder.
+
+```python
+creds = get_oauth2_creds(config_obj)
+drive = Drive(creds)
+
+filename = "Heyy"
+
+file = drive.get_name(filename, parents=[FOLDER_URL])
+if file is not None:
+    drive.delete(file["id"])
+
+file = drive.copy(file_id=FILE_ID, to_filename=filename, to_folder_id=FOLDER_URL)
+```
+
+What the above does is:
+
+-   Get the OAuth2 credentials from the `config_obj` object (JSON object representing
+    the requisite credentials, see
+    [here](https://developers.google.com/identity/protocols/oauth2/native-app#step-2:-send-a-request-to-googles-oauth-2.0-server)
+    for more information).
+-   create a `Drive` object thereupon.
+-   Get the file with the given name, and delete it if it exists.
+-   Copy the file with the given ID to the given folder, and return the new file.
+
+## Sheets
+
+Example: update a range of cells in a sheet.
+
+```python
+creds = get_oauth2_creds(config_path)
+sheets = Sheets(creds)
+
+Sheet1 = SheetsValueRange(sheets, SHEET_ID, sheet_name="Sheet1")
+
+rows = [
+    {
+        "Heyy": "99",
+    }
+]
+Sheet1[2:3, ...].update(rows)
+```
+
+What the above does is:
+
+-   Get the OAuth2 credentials from the `config_path` file (see
+    [here](https://developers.google.com/identity/protocols/oauth2/native-app#step-2:-send-a-request-to-googles-oauth-2.0-server)
+    for more information).
+-   create a `Sheets` object thereupon.
+-   Create a `SheetsValueRange` object, which is a wrapper around the
+    `spreadsheets.values` API.
+-   Update the range `Sheet1!A2:B3` with the given rows.
+
+Note the slicing syntax, which will feel quite familiar for any user of Numpy or Pandas.
+
+### SheetSlice
+
+A `SheetsValueRange` object can be sliced in a similar manner to that of a Numpy array.
+The syntax is as follows:
+
+    slc = Sheet[rows, cols]
+
+Wherein `rows` and `cols` are either integers, slices of integers (stride is not
+supported), strings (in A1 notation), or ellipses (`...`).
+
+Note that Google's implementation of A1 notation is 1-indexed; 0 is invalid (e.g., 1
+maps to `A`, 2 to `B`, etc.)
+
+```py
+ix = SheetSlice["Sheet1", 1:3, 2:4] #  "Sheet1!B2:D4"
+ix = SheetSlice["Sheet1", "A1:B2"]  #  "Sheet1!A1:B2"
+ix = SheetSlice[1:3, 2:4]           #  "Sheet1!B2:D4"
+ix = SheetSlice["A1:B2"]            #  "Sheet1!A1:B2"
+ix = SheetSlice[..., 1:3]           #  "Sheet1!A1:Z3"
+
+values = {
+    SheetSlice["A1:B2"]: [
+        ["Heyy", "99"],
+        ["Heyy", "99"],
+    ],
+} # "Sheet1!A1:B2" = [["Heyy", "99"], ["Heyy", "99"]]
+```
+
+A `SheetSlice` can also be used as a key into a `SheetsValueRange`, or a dictionary (to
+use in updating a sheet's range via `.update()`, for example). Further, a
+`SheetsValueRange` can be sliced in a similar manner to that of a `SheetSlice`.
+
+```py
+Sheet1[2:3, ...].update(rows)
+...
+```
 
-setup(**setup_kwargs)
```

