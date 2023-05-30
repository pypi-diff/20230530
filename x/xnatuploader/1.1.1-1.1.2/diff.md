# Comparing `tmp/xnatuploader-1.1.1.tar.gz` & `tmp/xnatuploader-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xnatuploader-1.1.1.tar", last modified: Wed Apr  5 03:19:49 2023, max compression
+gzip compressed data, was "xnatuploader-1.1.2.tar", last modified: Mon May 29 06:58:47 2023, max compression
```

## Comparing `xnatuploader-1.1.1.tar` & `xnatuploader-1.1.2.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-04-05 03:19:49.367302 xnatuploader-1.1.1/
--rw-r--r--   0 mike       (501) staff       (20)    14372 2023-04-05 03:19:49.367537 xnatuploader-1.1.1/PKG-INFO
--rw-r--r--   0 mike       (501) staff       (20)    13805 2023-02-16 03:37:24.000000 xnatuploader-1.1.1/README.md
--rw-r--r--   0 mike       (501) staff       (20)       93 2022-06-16 06:56:16.000000 xnatuploader-1.1.1/pyproject.toml
--rw-r--r--   0 mike       (501) staff       (20)     1076 2023-04-05 03:19:49.368943 xnatuploader-1.1.1/setup.cfg
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-04-05 03:19:49.353101 xnatuploader-1.1.1/src/
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-04-05 03:19:49.360386 xnatuploader-1.1.1/src/xnatuploader/
--rw-r--r--   0 mike       (501) staff       (20)       72 2022-06-16 06:56:16.000000 xnatuploader-1.1.1/src/xnatuploader/__init__.py
--rw-r--r--   0 mike       (501) staff       (20)     1242 2023-04-04 05:39:31.000000 xnatuploader-1.1.1/src/xnatuploader/dicoms.py
--rw-r--r--   0 mike       (501) staff       (20)    18502 2023-04-05 02:51:00.000000 xnatuploader-1.1.1/src/xnatuploader/matcher.py
--rw-r--r--   0 mike       (501) staff       (20)     8947 2023-03-15 03:09:46.000000 xnatuploader-1.1.1/src/xnatuploader/put.py
--rw-r--r--   0 mike       (501) staff       (20)     4892 2023-03-15 03:09:46.000000 xnatuploader-1.1.1/src/xnatuploader/upload.py
--rw-r--r--   0 mike       (501) staff       (20)     3631 2023-03-15 02:23:49.000000 xnatuploader-1.1.1/src/xnatuploader/workbook.py
--rwxr-xr-x   0 mike       (501) staff       (20)    16375 2023-04-04 23:13:30.000000 xnatuploader-1.1.1/src/xnatuploader/xnatuploader.py
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-04-05 03:19:49.363381 xnatuploader-1.1.1/src/xnatuploader.egg-info/
--rw-r--r--   0 mike       (501) staff       (20)    14372 2023-04-05 03:19:49.000000 xnatuploader-1.1.1/src/xnatuploader.egg-info/PKG-INFO
--rw-r--r--   0 mike       (501) staff       (20)      556 2023-04-05 03:19:49.000000 xnatuploader-1.1.1/src/xnatuploader.egg-info/SOURCES.txt
--rw-r--r--   0 mike       (501) staff       (20)        1 2023-04-05 03:19:49.000000 xnatuploader-1.1.1/src/xnatuploader.egg-info/dependency_links.txt
--rw-r--r--   0 mike       (501) staff       (20)       64 2023-04-05 03:19:49.000000 xnatuploader-1.1.1/src/xnatuploader.egg-info/entry_points.txt
--rw-r--r--   0 mike       (501) staff       (20)       98 2023-04-05 03:19:49.000000 xnatuploader-1.1.1/src/xnatuploader.egg-info/requires.txt
--rw-r--r--   0 mike       (501) staff       (20)       13 2023-04-05 03:19:49.000000 xnatuploader-1.1.1/src/xnatuploader.egg-info/top_level.txt
-drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-04-05 03:19:49.366545 xnatuploader-1.1.1/tests/
--rw-r--r--   0 mike       (501) staff       (20)      289 2022-11-17 02:49:16.000000 xnatuploader-1.1.1/tests/test_config.py
--rw-r--r--   0 mike       (501) staff       (20)     3117 2023-02-16 03:04:29.000000 xnatuploader-1.1.1/tests/test_matcher.py
--rw-r--r--   0 mike       (501) staff       (20)     4825 2023-04-05 02:51:00.000000 xnatuploader-1.1.1/tests/test_scan.py
--rw-r--r--   0 mike       (501) staff       (20)     4992 2023-03-14 05:26:10.000000 xnatuploader-1.1.1/tests/test_upload.py
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-05-29 06:58:47.590266 xnatuploader-1.1.2/
+-rw-r--r--   0 mike       (501) staff       (20)    14372 2023-05-29 06:58:47.590507 xnatuploader-1.1.2/PKG-INFO
+-rw-r--r--   0 mike       (501) staff       (20)    13805 2023-02-16 03:37:24.000000 xnatuploader-1.1.2/README.md
+-rw-r--r--   0 mike       (501) staff       (20)       93 2022-06-16 06:56:16.000000 xnatuploader-1.1.2/pyproject.toml
+-rw-r--r--   0 mike       (501) staff       (20)     1076 2023-05-29 06:58:47.591563 xnatuploader-1.1.2/setup.cfg
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-05-29 06:58:47.576581 xnatuploader-1.1.2/src/
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-05-29 06:58:47.583813 xnatuploader-1.1.2/src/xnatuploader/
+-rw-r--r--   0 mike       (501) staff       (20)       72 2022-06-16 06:56:16.000000 xnatuploader-1.1.2/src/xnatuploader/__init__.py
+-rw-r--r--   0 mike       (501) staff       (20)      283 2023-05-25 02:08:09.000000 xnatuploader-1.1.2/src/xnatuploader/dataclass.py
+-rw-r--r--   0 mike       (501) staff       (20)     3202 2023-05-29 06:43:19.000000 xnatuploader-1.1.2/src/xnatuploader/dicoms.py
+-rw-r--r--   0 mike       (501) staff       (20)    15000 2023-05-29 06:43:19.000000 xnatuploader-1.1.2/src/xnatuploader/matcher.py
+-rw-r--r--   0 mike       (501) staff       (20)     8947 2023-03-15 03:09:46.000000 xnatuploader-1.1.2/src/xnatuploader/put.py
+-rw-r--r--   0 mike       (501) staff       (20)     5358 2023-05-29 06:43:19.000000 xnatuploader-1.1.2/src/xnatuploader/upload.py
+-rw-r--r--   0 mike       (501) staff       (20)      203 2023-04-05 06:48:06.000000 xnatuploader-1.1.2/src/xnatuploader/userdict.py
+-rw-r--r--   0 mike       (501) staff       (20)     3898 2023-05-29 06:43:19.000000 xnatuploader-1.1.2/src/xnatuploader/workbook.py
+-rwxr-xr-x   0 mike       (501) staff       (20)    17102 2023-05-29 06:43:19.000000 xnatuploader-1.1.2/src/xnatuploader/xnatuploader.py
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-05-29 06:58:47.586319 xnatuploader-1.1.2/src/xnatuploader.egg-info/
+-rw-r--r--   0 mike       (501) staff       (20)    14372 2023-05-29 06:58:47.000000 xnatuploader-1.1.2/src/xnatuploader.egg-info/PKG-INFO
+-rw-r--r--   0 mike       (501) staff       (20)      615 2023-05-29 06:58:47.000000 xnatuploader-1.1.2/src/xnatuploader.egg-info/SOURCES.txt
+-rw-r--r--   0 mike       (501) staff       (20)        1 2023-05-29 06:58:47.000000 xnatuploader-1.1.2/src/xnatuploader.egg-info/dependency_links.txt
+-rw-r--r--   0 mike       (501) staff       (20)       64 2023-05-29 06:58:47.000000 xnatuploader-1.1.2/src/xnatuploader.egg-info/entry_points.txt
+-rw-r--r--   0 mike       (501) staff       (20)       98 2023-05-29 06:58:47.000000 xnatuploader-1.1.2/src/xnatuploader.egg-info/requires.txt
+-rw-r--r--   0 mike       (501) staff       (20)       13 2023-05-29 06:58:47.000000 xnatuploader-1.1.2/src/xnatuploader.egg-info/top_level.txt
+drwxr-xr-x   0 mike       (501) staff       (20)        0 2023-05-29 06:58:47.589486 xnatuploader-1.1.2/tests/
+-rw-r--r--   0 mike       (501) staff       (20)      289 2022-11-17 02:49:16.000000 xnatuploader-1.1.2/tests/test_config.py
+-rw-r--r--   0 mike       (501) staff       (20)     3117 2023-02-16 03:04:29.000000 xnatuploader-1.1.2/tests/test_matcher.py
+-rw-r--r--   0 mike       (501) staff       (20)     5387 2023-05-29 06:43:19.000000 xnatuploader-1.1.2/tests/test_scan.py
+-rw-r--r--   0 mike       (501) staff       (20)     5359 2023-05-29 06:43:19.000000 xnatuploader-1.1.2/tests/test_upload.py
```

### Comparing `xnatuploader-1.1.1/PKG-INFO` & `xnatuploader-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnatuploader
-Version: 1.1.1
+Version: 1.1.2
 Summary: CLI tool for uploading multiple files to XNAT
 Home-page: https://github.com/SydneyInformaticsHub/xnatuploader
 Author: Mike Lynch
 Author-email: m.lynch@sydney.edu.au
 Project-URL: Bug Tracker, https://github.com/SydneyInformaticsHub/xnatuploader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `xnatuploader-1.1.1/README.md` & `xnatuploader-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.1/setup.cfg` & `xnatuploader-1.1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xnatuploader
-version = 1.1.1
+version = 1.1.2
 author = Mike Lynch
 author_email = m.lynch@sydney.edu.au
 description = CLI tool for uploading multiple files to XNAT
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/SydneyInformaticsHub/xnatuploader
 project_urls =
```

### Comparing `xnatuploader-1.1.1/src/xnatuploader/matcher.py` & `xnatuploader-1.1.2/src/xnatuploader/matcher.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,96 +1,211 @@
 import re
 import logging
-from pydicom import dcmread
-from pydicom.errors import InvalidDicomError
 
-XNAT_HIERARCHY = ["Subject", "Session", "Dataset"]
-DICOM_PARAMS = [
-    "Modality",
-    "StudyDescription",
-    "StudyDate",
-    "Manufacturer",
-    "ManufacturerModelName",
-    "StationName",
-]
 
 logger = logging.getLogger(__name__)
 
+# TODO- what to do about the DICOM:StudyDate v StudyDate stuff? I want to keep
+# the DICOM prefixes so that the user's spreadsheets still work - maybe handle
+# this in the subclass?
+
+
+class FileMatch(dict):
+    """
+    Represents a file, which may or may not have been successfully matched.
+    The values collected from paths and metadata extraction, and the metadata
+    parameters mapped form them, are available as dict lookups, like
+    filematch["Subject"].
+    """
+
+    def __init__(self, matcher, file=None, label=None, values=None):
+        self.matcher = matcher
+        self.label = label
+        self.file = str(file)
+        self.filename = None
+        if file is not None:
+            self.filename = file.name
+        self.error = None
+        self.success = False
+        self.status = None
+        self.selected = None
+        self._columns = None
+        if values is not None:
+            for field, value in values.items():
+                self[field] = value
+
+    @property
+    def columns(self):
+        """
+        Returns this file's representation in the spreadsheet, which may or
+        may not be a successful match.
+
+        fields: [ str ]
+        """
+        if self._columns is not None:
+            return self._columns
+        self._columns = [self.label, self.file, self.filename]
+        if self.selected:
+            self._columns += ["Y"]
+        else:
+            self._columns += ["N"]
+        if self.error is not None:
+            self._columns += [self.error]
+        else:
+            if self.status is None:
+                self._columns += [""]
+            else:
+                self._columns += [self.status]
+        self._columns += [self.get(v) for v in self.matcher.headers[5:]]
+        return self._columns
+
+    def from_row(self, row):
+        """
+        Read a row from a spreadsheet and populate the values required to
+        upload.
+        """
+        self.label = row[0]
+        self.file = row[1]
+        self.filename = row[2]
+        self.selected = row[3] == "Y"
+        self.status = row[4]
+        for field, value in zip(self.matcher.headers[5:], row[5:]):
+            self[field] = value
+
 
 class RecipeException(Exception):
     pass
 
 
+class ExtractException(Exception):
+    pass
+
+
 class Matcher:
     """
-    A Matcher is a set of recipes for matching against filepaths and mappings
-    which map the captured value to XNAT parameters. It's used to perform
-    the matching, returning FileMatch objects, and also has methods which are
-    used to get headers for the spreadsheets (since these will vary according
-    to the parameters captured in the recipes)
+    A Matcher is a set of patterns for matching against filepaths and mappings
+    which map the captured value to field values. It's used to perform
+    the matching, returning FileMatch objects.
+
+    file_extractor is a function which does application-specific metadata
+    extraction: it's up to the calling code to make sure that the values it
+    sets are coordinated with the values extracted by the patterns and mappings
     """
 
-    def __init__(self, config, loglevel="WARNING"):
-        """
-        config: dict with "paths" and "mappings"
+    def __init__(
+        self,
+        patterns,
+        mappings,
+        fields,
+        file_extractor=None,
+        match_class=FileMatch,
+        loglevel="WARNING",
+    ):
+        """
+        patterns: OrderedDict(str: str) of path patterns
+        mappings: OrderedDict(str: str) of metadata values to captured fields
+        fields: list of extra fields to include in the spreadsheet
+        file_extractor: fn or None
+        log_level: str
         """
         logger.setLevel(loglevel)
         logch = logging.StreamHandler()
         logch.setLevel(loglevel.upper())
         logger.addHandler(logch)
-        self.parse_recipes(config["paths"])
-        self.mappings = config["mappings"]
+        self.mappings = mappings
+        self.file_extractor = file_extractor
+        self.match_class = match_class
+        self.fields = fields
         self._headers = None
-        self._dicom_params = set(DICOM_PARAMS)
-        for k, vs in self.mappings.items():
-            for v in vs:
-                if v[:5] == "DICOM":
-                    self._dicom_params.add(v[6:])
-                elif v not in self.params:
-                    raise Exception(
-                        f"Value {v} in mapping for {k} not defined in a path"
-                    )
-        if set(self.mappings.keys()) != set(XNAT_HIERARCHY):
-            raise Exception(f"Must have mappings for each of {XNAT_HIERARCHY}")
+        self.path_values = []
+        self.parse_recipes(patterns)
 
     @property
     def headers(self):
         if self._headers is None:
             self._headers = [
                 "Pattern",
                 "File",
                 "Filename",
                 "Upload",
                 "Status",
-                "SessionLabel",
             ]
-            self._headers += XNAT_HIERARCHY + self.dicom_params + self.params
+            self._headers += list(self.mappings.keys())
+            self._headers += self.fields + self.path_values
         return self._headers
 
-    @property
-    def dicom_params(self):
-        return sorted(self._dicom_params)
+    def make_filematch(self, file, label=None, values=None):
+        """
+        Map a dict of values (which will be captured from the paths or by
+        specialised metadata extraction) to metadata paramers and use
+        those to populate a FileMatch object.
+        If the mapping was unsuccessful, the FileMatch will have its success
+        flag switched off.
+        """
+        match = self.match_class(self, file, label, values)
+        try:
+            for field, value in self.map_values(values).items():
+                match[field] = value
+            match.success = True
+        except ValueError as e:
+            logger.warning(f"Mapping error: {e}")
+            match.success = False
+            match.status = "unmatched"
+        match.selected = match.success
+        return match
+
+    def map_values(self, values):
+        """
+        Given a dict of values which has been captured from a filepath by a
+        pattern, returns the top-level metadata as defined by self.mappings
+
+        Raises: ValueError if any of the required values are missing
+
+        values: dict of { str: str }
+        --
+        returns: { str: str }
+        """
+        metadata = {}
+        for field, path_vars in self.mappings.items():
+            for v in path_vars:
+                if v not in values:
+                    raise ValueError(f"value {v} not found")
+                if values[v] is None:
+                    raise ValueError(f"value {v} is None")
+            metadata[field] = "".join([values[v] for v in path_vars])
+            metadata[field] = metadata[field].replace(" ", "_")
+        return metadata
+
+    def from_spreadsheet(self, row):
+        """
+        Build a FileMatch from a spreadsheet row, using the FileMatch.from_row
+        method
+        """
+        match = self.match_class(self)
+        match.from_row(row)
+        return match
 
     def parse_recipes(self, recipe_config):
         """
         Parses a set of recipes from the config, keyed by label. The value for
         each label should be a list of recipe strings. Builds the params
         variable, which is a list of all the params, and a list of compiled
         regular expressions.
         ---
         recipe_config: dict of { str: list of str  }
         """
-        self.params = []
         self.recipes = {}
         for label, patterns in recipe_config.items():
             self.recipes[label] = []
             for pattern in patterns:
-                params, regexp = self.parse_recipe(label, pattern)
+                path_values, regexp = self.parse_recipe(label, pattern)
                 self.recipes[label].append(regexp)
-                self.params += [p for p in params if p not in self.params]
+                self.path_values += [
+                    p for p in path_values if p not in self.path_values
+                ]
 
     def parse_recipe(self, label, recipe):
         """
         Parse a recipe string and add it to the recipes dict, and add its
         params to self.params
 
         A recipe is a string with one or more parameter names between {}
@@ -174,65 +289,29 @@
         ---
         file: pathlib.Path
 
         returns: a FileMatch
         """
         label, values = self.match_path(filepath.relative_to(root))
         if label:
-            logger.debug(f"> reading DICOM metadata {filepath}")
-            dicom_values = self.read_dicom(filepath)
-            if dicom_values is None:
-                logger.debug(f"> DICOM read failed {filepath}")
-                match = FileMatch(self, filepath, None)
-                match.status = "No DICOM metadata"
-                return match
-            if "EncapsulatedDocument" in dicom_values:
-                logger.debug(f"> DICOM is an encapsulated report {filepath}")
-                match = FileMatch(self, filepath, None)
-                match.status = "DICOM is an encapsulated report"
-                return match
-            if dicom_values["Modality"] == "SR":
-                logger.debug(f"> DICOM is a structured report {filepath}")
-                match = FileMatch(self, filepath, None)
-                match.status = "DICOM is an SR (structured report)"
-                return match
-            return self.make_filematch(filepath, label, values, dicom_values)
-        match = FileMatch(self, filepath, None)
+            if self.file_extractor is not None:
+                try:
+                    file_values = self.file_extractor(filepath)
+                except ExtractException as e:
+                    match = self.match_class(self, filepath)
+                    match.status = "unmatched"
+                    match.error = str(e)
+                    return match
+                for field, value in file_values.items():
+                    values[field] = value  # file metadata can overwrite path
+            return self.make_filematch(filepath, label, values)
+        match = self.match_class(self, filepath)
         match.status = "unmatched"
         return match
 
-    def make_filematch(self, file, label, path_values, dicom_values):
-        """
-        Map the values captured to XNAT hierarchy values and return an
-        FileMatch object. If the mapping was unsuccessful, the FileMatch will
-        have its success flag switched off
-        """
-        match = FileMatch(self, file, label)
-        match.values = path_values
-        match.dicom_values = dicom_values
-        try:
-            logger.debug("> mapping DICOM and path values to XNAT params")
-            match.xnat_params = self.map_values(path_values, dicom_values)
-            match.success = True
-        except ValueError as e:
-            logger.warning(f"> xnat params error: {e}")
-            match.success = False
-            match.status = "unmatched"
-        match.selected = match.success
-        return match
-
-    def from_spreadsheet(self, row):
-        """
-        Build a FileMatch from a spreadsheet row, using the FileMatch.from_row
-        method
-        """
-        match = FileMatch(self, None, None)
-        match.from_row(row)
-        return match
-
     def match_path(self, filepath):
         """
         Try to match a filepath against each of the recipes and return the label
         and values for the first one which matches.
         ---
         file: pathlib.Path
 
@@ -337,194 +416,7 @@
         m = patterns[0].match(dirs[0])
         if m is not None:
             if len(patterns) > 1:
                 return m
             if len(dirs) == 1:
                 return m
         return None
-
-    def read_dicom(self, file):
-        """
-        Try to parse the dicom metadata from the file and returns a dict
-        of all the values extracted for this Matcher's dicom_params
-        ---
-        file: a pathlib.Path
-
-        returns: { str: str }
-        """
-        try:
-            dc_meta = dcmread(file)
-            if "EncapsulatedDocument" in dc_meta:
-                return {"EncapsulatedDocument": True}
-            values = {p: dc_meta.get(p) for p in self._dicom_params}
-            return values
-        except InvalidDicomError:
-            return None
-
-    def map_values(self, path_values, dicom_values):
-        """
-        Given a dict of values which has been captured from a filepath by a recipe,
-        try to map it to the XNAT hierarchy.
-
-        Raises: ValueError if any of the required values are missing
-
-        values: dict of { str: str }
-        """
-        for k, v in dicom_values.items():
-            path_values["DICOM:" + k] = v
-        xnat_params = {}
-        for xnat_cat, path_vars in self.mappings.items():
-            for v in path_vars:
-                if v not in path_values:
-                    raise ValueError(f"value {v} not found")
-                if path_values[v] is None:
-                    raise ValueError(f"value {v} is None")
-            xnat_params[xnat_cat] = "".join([path_values[v] for v in path_vars])
-            xnat_params[xnat_cat] = xnat_params[xnat_cat].replace(" ", "_")
-        return xnat_params
-
-
-class FileMatch:
-    """
-    Represents a file, which may or may not have been successfully matched.
-    Used as the return value from Matcher.match and as the result of loading
-    the log spreadsheet.
-    """
-
-    def __init__(self, matcher, file, label):
-        self.matcher = matcher
-        self.label = label
-        self.file = str(file)
-        self.filename = None
-        if file is not None:
-            self.filename = file.name
-        self.values = None
-        self.dicom_values = None
-        self.xnat_params = None
-        self.session_label = None
-        self.error = None
-        self.success = False
-        self.status = None
-        self.selected = None
-        self._columns = None
-        self._status = None
-        self._selected = None
-
-    @property
-    def columns(self, refresh=False):
-        """
-        Returns this file's representation in the spreadsheet, which may or
-        may not be a successful match
-        """
-        if self._columns is not None:
-            return self._columns
-        self._columns = [self.label, self.file, self.filename]
-        if self.selected:
-            self._columns += ["Y"]
-        else:
-            self._columns += ["N"]
-        if self.error is not None:
-            self._columns += [self.error]
-        else:
-            if self.status is None:
-                self._columns += [""]
-            else:
-                self._columns += [self.status]
-        self._columns += [self.session_label]
-        self._columns += self.dict_to_columns(XNAT_HIERARCHY, self.xnat_params)
-        self._columns += self.dict_to_columns(
-            self.matcher.dicom_params, self.dicom_values
-        )
-        self._columns += self.dict_to_columns(self.matcher.params, self.values)
-        return self._columns
-
-    def dict_to_columns(self, columns, values):
-        if values is None:
-            return ["" for _ in columns]
-        else:
-            return [values.get(c, "") for c in columns]
-
-    def from_row(self, row):
-        """
-        Read a row from the spreadsheet and populate the values required to
-        upload.
-        """
-        self.label = row[0]
-        self.file = row[1]
-        self.filename = row[2]
-        self.selected = row[3] == "Y"
-        self.status = row[4]
-        self.session_label = row[5]
-        self.xnat_params = {
-            "Subject": row[6],
-            "Session": row[7],
-            "Dataset": row[8],
-        }
-        self.dicom_values = {}
-        c = 9
-        for p in self.matcher.dicom_params:
-            self.dicom_values[p] = row[c]
-            c += 1
-        self.values = {}
-        for p in self.matcher.params:
-            self.values[p] = row[c]
-            c += 1
-
-    def load_dicom(self):
-        """
-        Utility method used to load the dicom metadata for an umatched file
-        when debugging
-        """
-        dicom_values = self.matcher.read_dicom(self.file)
-        if dicom_values is not None:
-            self.dicom_values = dicom_values
-            self._columns = None
-
-    @property
-    def subject(self):
-        if self.xnat_params is not None:
-            return self.xnat_params["Subject"]
-        else:
-            return None
-
-    @property
-    def session(self):
-        if self.xnat_params is not None:
-            return self.xnat_params["Session"]
-        else:
-            return None
-
-    @property
-    def dataset(self):
-        if self.xnat_params is not None:
-            return self.xnat_params["Dataset"]
-        else:
-            return None
-
-    @property
-    def study_date(self):
-        if self.session is not None:
-            return self.session
-        if self.dicom_values is not None:
-            return self.dicom_values["StudyDate"]
-        return ""
-
-    @property
-    def modality(self):
-        if self.dicom_values is not None:
-            return self.dicom_values["Modality"]
-        else:
-            return "OT"  # DICOM code for "Other"
-
-    @property
-    def manufacturer(self):
-        if self.dicom_values is not None:
-            return self.dicom_values["Manufacturer"]
-        else:
-            return None
-
-    @property
-    def model(self):
-        if self.dicom_values is not None:
-            return self.dicom_values["ManufacturerModelName"]
-        else:
-            return None
```

### Comparing `xnatuploader-1.1.1/src/xnatuploader/put.py` & `xnatuploader-1.1.2/src/xnatuploader/put.py`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.1/src/xnatuploader/upload.py` & `xnatuploader-1.1.2/src/xnatuploader/upload.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,70 @@
-# import xnatutils
 import xnatuploader.put
 import os.path
 import logging
+from dataclasses import dataclass
 
 logger = logging.getLogger(__name__)
 
 
+@dataclass
 class Upload:
     """
     An Upload represents a session for a single patient and visit, which may
     have more than one file.
+
     """
 
-    def __init__(
-        self, session_label, subject, date, modality, scan_type, manufacturer, model
-    ):
-        self.session_label = session_label
-        self.subject = subject
-        self.modality = modality
-        self.date = date
-        self.scan_type = scan_type
-        self.manufacturer = manufacturer
-        self.model = model
+    session_label: str
+    subject: str
+    date: str
+    modality: str
+    series_number: str
+    scan_type: str
+    manufacturer: str
+    model: str
+
+    def __post_init__(self):
         self.new_session = True
         self.xnat_session = None
         self.files = []
 
     @property
     def label(self):
         """A value which can identify this upload in XNAT - scan_type
         corresponds to dataset. Used for logging upload errors which are
         triggered by start_upload below."""
         return f"{self.session_label}/{self.scan_type}"
 
     def add_file(self, file):
-        self.files.append(file)
+        """Add a file to this upload's file list. If the series number on the
+        file doesn't match the upload series number, doesn't add it and
+        logs an error"""
+        if file.series_number == self.series_number:
+            self.files.append(file)
+            return True
+        else:
+            logger.error(
+                f"""
+{self.session_label} {file.filename} series number {file.series_number} does
+not match series number in scan ({self.series_number})
+"""
+            )
+            return False
 
     def start_upload(self, xnat_session, project):
         """Create a resource in the session for this scan"""
         self.xnat_session = xnat_session
         self.resource = xnatuploader.put.resource(
             self.session_label,
             self.scan_type,
             resource_name="DICOM",
             project_id=project,
             subject_id=self.subject,
+            scan_id=self.series_number,
             #            date=self.date,
             modality=self.modality,
             create_session=self.new_session,
             connection=xnat_session,
         )
 
     def upload(self, files, overwrite=False):
@@ -97,14 +113,15 @@
             else:
                 remote_digest = digests[xnat_filename]
                 local_digest = xnatuploader.put.calculate_checksum(file.file)
                 if local_digest != remote_digest:
                     status[
                         file.file
                     ] = f"Digest mismatch {local_digest} {remote_digest}"
+                    logger.error(file.file + ": " + status[file.file])
                 else:
                     status[file.file] = "success"
         return status
 
     def log(self, logger):
         """
         Write an upload batch to logger for debugging
```

### Comparing `xnatuploader-1.1.1/src/xnatuploader/workbook.py` & `xnatuploader-1.1.2/src/xnatuploader/workbook.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from collections import OrderedDict
 from openpyxl import Workbook, load_workbook
 from openpyxl.styles.alignment import Alignment
 
 FILE_COLUMN_WIDTH = 50
 HELP_COLUMN_WIDTH = 25
 HELP_ROW_HEIGHT = 90
 
@@ -91,28 +92,33 @@
     ws = wb.create_sheet("Files")
     ws.column_dimensions["B"].width = FILE_COLUMN_WIDTH
     ws.append(matcher.headers)
     return ws
 
 
 def load_config(excelfile):
+    """
+    Load config from the Configuration worksheet of the spreadsheet.
+    Each section is loaded into an OrderedDict - this is because order is
+    significant for building the columns in the spreadsheet.
+    """
     wb = load_workbook(excelfile)
     if "Configuration" not in wb:
         raise WorkbookError(f"No worksheet named 'Configuration' in {excelfile}")
     ws = wb["Configuration"]
     config = {}
     section = None
     sections = ["paths", "mappings", "xnat"]
     for row in ws:
         if row[0].value is not None:
             section = row[0].value.lower()
         var = row[1].value
         if var is not None and section is not None:
             if section not in config:
-                config[section] = {}
+                config[section] = OrderedDict()
             cells = [cell.value for cell in row[2:] if cell.value is not None]
             if section == "xnat":
                 config[section][var] = cells[0]
             else:
                 config[section][var] = cells
     missing = [s for s in sections if s not in config]
     if len(missing) > 0:
```

### Comparing `xnatuploader-1.1.1/src/xnatuploader/xnatuploader.py` & `xnatuploader-1.1.2/src/xnatuploader/xnatuploader.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from importlib.metadata import version
 
 __version__ = version("xnatuploader")
 
 from openpyxl import load_workbook
 
 from xnatuploader.matcher import Matcher
+from xnatuploader.dicoms import dicom_extractor, XNATFileMatch, SPREADSHEET_FIELDS
 from xnatuploader.workbook import new_workbook, add_filesheet, load_config
 from xnatuploader.upload import Upload, trigger_pipelines
 
 from xnatutils.base import sanitize_re
 
 FILE_COLUMN_WIDTH = 50
 
@@ -42,51 +43,65 @@
 def scan(matcher, root, spreadsheet, include_unmatched=True, debug=False):
     """
     Scan the filesystem under root for files which match recipes and write
     out the resulting values to a new worksheet in the spreadsheet.
 
     If the debug flag is true, only try to match DEBUG_MAX files
     ---
-    matcher: a PathMatcher
+    matcher: a Matcher
     root: pathlib.Path
     spreadsheet: pathlib.Path
     include_unmatched: boolean
     debug: boolean
     """
     logger.info(f"Loading {spreadsheet}")
     wb = load_workbook(spreadsheet)
     ws = add_filesheet(wb, matcher, debug)  # keeps old sheets if debug=True
-    matched = 0
-    unmatched = 0
     logger.info("Preparing file list")
-    files = sorted(
+    filepaths = sorted(
         [f for f in root.glob("**/*") if f.is_file() and f.name not in IGNORE_FILES]
     )
+    files = []
+    unmatched = []
     if debug:
-        files = files[:DEBUG_MAX]
+        filepaths = filepaths[:DEBUG_MAX]
     logger.info(f"Scanning directory {root}")
-    for file in tqdm(files):
-        if file.is_file():
-            logger.debug(f"Scanning {file}")
-            filematch = matcher.match(root, file)
-            if filematch.success:
-                matched += 1
-                logger.debug(f"Matched {filematch.file}")
-                ws.append(filematch.columns)
+    for filepath in tqdm(filepaths):
+        if filepath.is_file():
+            logger.debug(f"Scanning {filepath}")
+            file = matcher.match(root, filepath)
+            if file.success:
+                logger.debug(f"Matched {file.file}")
+                files.append(file)
             else:
                 if include_unmatched:
-                    unmatched += 1
-                    filematch.load_dicom()
-                    ws.append(filematch.columns)
+                    file.load_dicom()
+                    unmatched.append(file)
+
+    skips, uploads = collate_uploads(files)
+
+    ns = len(uploads)
+    nm = len(files)
+    num = len(unmatched)
+
     if include_unmatched:
         logger.info(
-            f"Saved {matched} matching files and {unmatched} non-matching files to {spreadsheet}"
+            f"Saving {ns} scans with {nm} matching files and {num} non-matching files to {spreadsheet}"
         )
     else:
-        logger.info(f"Saved {matched} matching files to {spreadsheet}")
+        logger.info(f"Saving {ns} scans with {nm} matching files to {spreadsheet}")
+
+    for session_scan, upload in tqdm(uploads.items(), desc="Scans"):
+        for file in upload.files:
+            ws.append(file.columns)
+
+    if include_unmatched:
+        for file in unmatched:
+            ws.append(file.columns)
+
     wb.save(spreadsheet)
 
 
 def upload(
     xnat_session,
     matcher,
     project,
@@ -122,15 +137,15 @@
     files = []
     for row in ws.values:
         if header:
             header = False
         else:
             matchfile = matcher.from_spreadsheet(row)
             files.append(matchfile)
-    skip, uploads = collate_uploads(project, files)
+    skip, uploads = collate_uploads(files)
     csvout = get_csv_filename(spreadsheet)
     if test:
         dry_run(uploads)
         return
     written = {}
     abandoned = False
     with open(csvout, "w", newline="") as cfh:
@@ -237,22 +252,22 @@
 the spreadsheet open in Excel.
 
 The results are available as a CSV file: {csvout}
 """
         )
 
 
-def collate_uploads(project_id, files):
+def collate_uploads(files):
     """
     Takes a list of files and collates them by subject (patient), visit
-    index (starting from the earliest) and scan type, returning a list of
-    files which have skipped or already uploaded and a dictionary
-    of Uploads keyed by {session_label}_{scan}
+    index (starting from the earliest), scan type, and (optionally) scan_id,
+    returning a list of files which have skipped or already uploaded and a dictionary
+    of Uploads keyed by {session_label}_{scan}_{scan_id}
+
     ---
-    project_id: str
     files: list of FileMatch
 
     returns: tuple of ( list of FileMatch, dict of str: Upload )
     """
 
     subjects = {}
     skip = []
@@ -260,38 +275,40 @@
         if not file.selected:
             skip.append(file)
         else:
             if file.status == "success":
                 logger.debug(f"skipping file already uploaded {file.file}")
                 skip.append(file)
             else:
-                if file.subject not in subjects:
-                    subjects[file.subject] = []
-                subjects[file.subject].append(file)
+                if file["Subject"] not in subjects:
+                    subjects[file["Subject"]] = []
+                subjects[file["Subject"]].append(file)
     uploads = {}
     for subject_id, files in subjects.items():
         dates = sorted(set([file.study_date for file in files]))
         visits = {dates[i]: i + 1 for i in range(len(dates))}
         clean_datasets = sanitise_dataset_names(files)
         for file in files:
             visit = visits[file.study_date]
             modality = file.modality
-            session_label = f"{subject_id}_{modality}{visit}"
+            scan_id = file.series_number
+            session_label = f"{subject_id}_{modality}{visit}_{scan_id}"
             file.session_label = session_label
             scan_type = clean_datasets[file.dataset]
             session_scan = f"{session_label}:{scan_type}"
             if session_scan not in uploads:
                 uploads[session_scan] = Upload(
-                    session_label,
-                    subject_id,
-                    file.study_date,
-                    modality,
-                    scan_type,
-                    file.manufacturer,
-                    file.model,
+                    session_label=session_label,
+                    subject=subject_id,
+                    date=file.study_date,
+                    modality=modality,
+                    series_number=scan_id,
+                    scan_type=scan_type,
+                    manufacturer=file.manufacturer,
+                    model=file.model,
                 )
             uploads[session_scan].add_file(file)
     return skip, uploads
 
 
 def sanitise_dataset_names(files):
     """
@@ -462,15 +479,22 @@
     if args.operation == "init":
         new_workbook(args.spreadsheet)
         logger.info(f"Initialised spreadsheet at {args.spreadsheet}")
         exit()
 
     config = load_config(args.spreadsheet)
 
-    matcher = Matcher(config, loglevel=loglevel)
+    matcher = Matcher(
+        patterns=config["paths"],
+        mappings=config["mappings"],
+        fields=SPREADSHEET_FIELDS,
+        file_extractor=dicom_extractor,
+        match_class=XNATFileMatch,
+        loglevel=loglevel,
+    )
 
     if args.operation == "scan":
         scan(
             matcher,
             args.dir,
             args.spreadsheet,
             include_unmatched=args.unmatched,
```

### Comparing `xnatuploader-1.1.1/src/xnatuploader.egg-info/PKG-INFO` & `xnatuploader-1.1.2/src/xnatuploader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xnatuploader
-Version: 1.1.1
+Version: 1.1.2
 Summary: CLI tool for uploading multiple files to XNAT
 Home-page: https://github.com/SydneyInformaticsHub/xnatuploader
 Author: Mike Lynch
 Author-email: m.lynch@sydney.edu.au
 Project-URL: Bug Tracker, https://github.com/SydneyInformaticsHub/xnatuploader/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `xnatuploader-1.1.1/src/xnatuploader.egg-info/SOURCES.txt` & `xnatuploader-1.1.2/src/xnatuploader.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 README.md
 pyproject.toml
 setup.cfg
 src/xnatuploader/__init__.py
+src/xnatuploader/dataclass.py
 src/xnatuploader/dicoms.py
 src/xnatuploader/matcher.py
 src/xnatuploader/put.py
 src/xnatuploader/upload.py
+src/xnatuploader/userdict.py
 src/xnatuploader/workbook.py
 src/xnatuploader/xnatuploader.py
 src/xnatuploader.egg-info/PKG-INFO
 src/xnatuploader.egg-info/SOURCES.txt
 src/xnatuploader.egg-info/dependency_links.txt
 src/xnatuploader.egg-info/entry_points.txt
 src/xnatuploader.egg-info/requires.txt
```

### Comparing `xnatuploader-1.1.1/tests/test_matcher.py` & `xnatuploader-1.1.2/tests/test_matcher.py`

 * *Files identical despite different names*

### Comparing `xnatuploader-1.1.1/tests/test_scan.py` & `xnatuploader-1.1.2/tests/test_scan.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import json
 from openpyxl import load_workbook
 from pathlib import Path
 
 from xnatuploader.matcher import Matcher
+from xnatuploader.dicoms import dicom_extractor, XNATFileMatch, SPREADSHEET_FIELDS
 from xnatuploader.xnatuploader import scan, collate_uploads
 from xnatuploader.workbook import load_config, new_workbook
 
 logger = logging.getLogger(__name__)
 
 
 def assert_worksheets_equal(expect, got):
@@ -17,86 +18,107 @@
         grows = grows[1:]
     assert len(grows) == 0
 
 
 def test_scan(tmp_path, test_files):
     fileset = test_files["basic"]
     config = load_config(fileset["config_excel"])
-    matcher = Matcher(config)
+    matcher = Matcher(
+        config["paths"],
+        config["mappings"],
+        SPREADSHEET_FIELDS,
+        dicom_extractor,
+        XNATFileMatch,
+    )
     scanned = tmp_path / "scanned.xlsx"
     new_workbook(scanned)
     scan(matcher, Path(fileset["dir"]), scanned, include_unmatched=True)
     expect_wb = load_workbook(fileset["scanned_excel"])
     got_wb = load_workbook(scanned)
     assert "Files" in got_wb
     assert_worksheets_equal(expect_wb["Files"], got_wb["Files"])
 
 
 def test_collation(tmp_path, test_files, uploads_dict):
     fileset = test_files["basic"]
     config = load_config(fileset["config_excel"])
-    matcher = Matcher(config)
+    matcher = Matcher(
+        config["paths"],
+        config["mappings"],
+        SPREADSHEET_FIELDS,
+        dicom_extractor,
+        XNATFileMatch,
+    )
     log = tmp_path / "log.xlsx"
     new_workbook(log)
     scan(matcher, Path(fileset["dir"]), log)
-    project_id = uploads_dict["project"]
     wb = load_workbook(log)
     ws = wb["Files"]
     header = True
     files = []
     for row in ws.values:
         if header:
             header = False
         else:
             matchfile = matcher.from_spreadsheet(row)
             files.append(matchfile)
-    skipped, uploads = collate_uploads(project_id, files)
+    skipped, uploads = collate_uploads(files)
     for session_scan, upload in uploads.items():
         uploads[session_scan] = [f.file for f in uploads[session_scan].files]
     assert uploads == uploads_dict["uploads"]
     assert len(skipped) == uploads_dict["skipped"]
 
 
 def test_sanitisation_collisions(tmp_path, test_files, sanitised_dict):
     fileset = test_files["sanitisation"]
     config_file = fileset["config"]
     with open(config_file, "r") as fh:
         config = json.load(fh)
-    matcher = Matcher(config)
+    matcher = Matcher(
+        config["paths"],
+        config["mappings"],
+        SPREADSHEET_FIELDS,
+        dicom_extractor,
+        XNATFileMatch,
+    )
     logger.warning(f"Testing santisation in {fileset}")
     log = tmp_path / "log.xlsx"
     new_workbook(log)
     scan(matcher, Path(fileset["dir"]), log)
-    project_id = sanitised_dict["project"]
     wb = load_workbook(log)
     ws = wb["Files"]
     header = True
     files = []
     for row in ws.values:
         if header:
             header = False
         else:
             matchfile = matcher.from_spreadsheet(row)
             files.append(matchfile)
     logger.warning(f"File list = {files}")
-    skipped, uploads = collate_uploads(project_id, files)
+    skipped, uploads = collate_uploads(files)
     for session_scan, upload in uploads.items():
         uploads[session_scan] = [f.file for f in uploads[session_scan].files]
     assert uploads == sanitised_dict["uploads"]
     assert len(skipped) == sanitised_dict["skipped"]
 
 
 def test_collation_skips(tmp_path, test_files, uploads_dict):
     fileset = test_files["basic"]
     config = load_config(fileset["config_excel"])
-    matcher = Matcher(config)
+    matcher = Matcher(
+        config["paths"],
+        config["mappings"],
+        SPREADSHEET_FIELDS,
+        dicom_extractor,
+        XNATFileMatch,
+    )
     log = tmp_path / "log.xlsx"
     new_workbook(log)
     scan(matcher, Path(fileset["dir"]), log)
-    project_id = uploads_dict["project"]
     wb = load_workbook(log)
     ws = wb["Files"]
     header = True
     files = []
     skip_n = 4  # mark the first four files as "success"
     n = 0
     for row in ws.values:
@@ -106,15 +128,15 @@
             matchfile = matcher.from_spreadsheet(row)
             if n < skip_n:
                 if matchfile.selected:
                     matchfile.status = "success"
                     logger.warning(f"Skipping {matchfile.file}")
                     n += 1
             files.append(matchfile)
-    skip, uploads = collate_uploads(project_id, files)
+    skip, uploads = collate_uploads(files)
     assert len(skip) == uploads_dict["skipped"] + skip_n
     for session_scan, upload in uploads.items():
         uploads[session_scan] = [f.file for f in uploads[session_scan].files]
     # remove skipped files from the fixture dictionary
     upload_skipped = {}
     skipstr = [f.file for f in skip]
     for subject_id, files in uploads_dict["uploads"].items():
@@ -124,15 +146,21 @@
             upload_skipped[subject_id] = upload_files
     assert uploads == upload_skipped
 
 
 def test_secret_pdfs(tmp_path, test_files):
     fileset = test_files["secret_pdf"]
     config = load_config(fileset["config_excel"])
-    matcher = Matcher(config)
+    matcher = Matcher(
+        config["paths"],
+        config["mappings"],
+        SPREADSHEET_FIELDS,
+        dicom_extractor,
+        XNATFileMatch,
+    )
     scanned = tmp_path / "scanned.xlsx"
     new_workbook(scanned)
     scan(matcher, Path(fileset["dir"]), scanned, include_unmatched=True)
     expect_wb = load_workbook(fileset["scanned_excel"])
     got_wb = load_workbook(scanned)
     assert "Files" in got_wb
     assert_worksheets_equal(expect_wb["Files"], got_wb["Files"])
```

### Comparing `xnatuploader-1.1.1/tests/test_upload.py` & `xnatuploader-1.1.2/tests/test_upload.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,24 +5,31 @@
 
 from openpyxl import load_workbook
 
 from pathlib import Path
 
 from xnatuploader.xnatuploader import scan, upload
 from xnatuploader.matcher import Matcher
+from xnatuploader.dicoms import dicom_extractor, XNATFileMatch, SPREADSHEET_FIELDS
 from xnatuploader.workbook import new_workbook
 
 
 @pytest.mark.parametrize("source_dir", ["basic", "bad_paths"])
 def test_upload_from_spreadsheet(source_dir, xnat_connection, tmp_path, test_files):
     test_config = test_files[source_dir]["config"]
     test_dir = test_files[source_dir]["dir"]
     with open(test_config, "r") as fh:
-        config_json = json.load(fh)
-        matcher = Matcher(config_json)
+        config = json.load(fh)
+        matcher = Matcher(
+            config["paths"],
+            config["mappings"],
+            SPREADSHEET_FIELDS,
+            dicom_extractor,
+            XNATFileMatch,
+        )
     project = xnat_connection.classes.ProjectData(
         parent=xnat_connection,
         name="Test_" + source_dir,
     )
     log_scanned = tmp_path / "log_scanned.xlsx"
     log_uploaded = tmp_path / "log_uploaded.xlsx"
     downloads = tmp_path / "downloads"
@@ -92,16 +99,22 @@
 def test_missing_file(xnat_connection, tmp_path, test_files):
     project = xnat_connection.classes.ProjectData(
         parent=xnat_connection,
         name="Test_missing",
     )
     basic = test_files["basic"]
     with open(basic["config"], "r") as fh:
-        config_json = json.load(fh)
-        matcher = Matcher(config_json)
+        config = json.load(fh)
+        matcher = Matcher(
+            config["paths"],
+            config["mappings"],
+            SPREADSHEET_FIELDS,
+            dicom_extractor,
+            XNATFileMatch,
+        )
     log_scanned = tmp_path / "log_scanned.xlsx"
     log_uploaded = tmp_path / "log_uploaded.xlsx"
     new_workbook(log_scanned)
     scan(matcher, Path(basic["dir"]), log_scanned)
     scanned_wb = load_workbook(log_scanned)
     ws = scanned_wb["Files"]
     # change the third filename to trigger an error
```

