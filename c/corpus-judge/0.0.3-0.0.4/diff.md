# Comparing `tmp/corpus_judge-0.0.3.tar.gz` & `tmp/corpus_judge-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corpus_judge-0.0.3.tar", max compression
+gzip compressed data, was "corpus_judge-0.0.4.tar", max compression
```

## Comparing `corpus_judge-0.0.3.tar` & `corpus_judge-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1491 2023-05-28 20:04:11.444523 corpus_judge-0.0.3/LICENSE
--rw-r--r--   0        0        0      250 2023-05-28 20:00:18.687607 corpus_judge-0.0.3/README.md
--rw-r--r--   0        0        0      153 2023-05-28 20:44:53.654068 corpus_judge-0.0.3/corpus_judge/__init__.py
--rw-r--r--   0        0        0     6750 2023-05-28 20:43:59.813913 corpus_judge-0.0.3/corpus_judge/justice_model.py
--rw-r--r--   0        0        0    14172 2023-05-30 00:36:45.835164 corpus_judge-0.0.3/corpus_judge/justice_name.py
--rw-r--r--   0        0        0     9709 2023-05-30 00:16:54.038433 corpus_judge-0.0.3/corpus_judge/justice_select.py
--rw-r--r--   0        0        0    45229 2023-05-28 19:46:46.811633 corpus_judge-0.0.3/corpus_judge/sc.yaml
--rw-r--r--   0        0        0     1227 2023-05-30 00:38:56.169412 corpus_judge-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 corpus_judge-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1491 2023-05-28 20:04:11.444523 corpus_judge-0.0.4/LICENSE
+-rw-r--r--   0        0        0      250 2023-05-28 20:00:18.687607 corpus_judge-0.0.4/README.md
+-rw-r--r--   0        0        0      153 2023-05-28 20:44:53.654068 corpus_judge-0.0.4/corpus_judge/__init__.py
+-rw-r--r--   0        0        0     6750 2023-05-28 20:43:59.813913 corpus_judge-0.0.4/corpus_judge/justice_model.py
+-rw-r--r--   0        0        0    14172 2023-05-30 00:36:45.835164 corpus_judge-0.0.4/corpus_judge/justice_name.py
+-rw-r--r--   0        0        0    10512 2023-05-30 02:53:09.075263 corpus_judge-0.0.4/corpus_judge/justice_select.py
+-rw-r--r--   0        0        0    45229 2023-05-28 19:46:46.811633 corpus_judge-0.0.4/corpus_judge/sc.yaml
+-rw-r--r--   0        0        0     1227 2023-05-30 02:55:54.446078 corpus_judge-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      954 1970-01-01 00:00:00.000000 corpus_judge-0.0.4/PKG-INFO
```

### Comparing `corpus_judge-0.0.3/LICENSE` & `corpus_judge-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `corpus_judge-0.0.3/corpus_judge/justice_model.py` & `corpus_judge-0.0.4/corpus_judge/justice_model.py`

 * *Files identical despite different names*

### Comparing `corpus_judge-0.0.3/corpus_judge/justice_name.py` & `corpus_judge-0.0.4/corpus_judge/justice_name.py`

 * *Files identical despite different names*

### Comparing `corpus_judge-0.0.3/corpus_judge/justice_select.py` & `corpus_judge-0.0.4/corpus_judge/justice_select.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+import logging
 from typing import Any, NamedTuple
 
 from dateutil.parser import parse
 from sqlite_utils.db import Database, Table
 
 from .justice_model import Justice
 from .justice_name import OpinionWriterName
@@ -27,15 +28,14 @@
         try:
             return parse(self.date_str).date()
         except Exception:
             return None
 
     @property
     def src(self):
-        """This may either be just the last name or the full name."""
         return OpinionWriterName.extract(self.text)
 
     @property
     def candidate(self) -> str | None:
         return self.src and self.src.writer
 
     @property
@@ -103,41 +103,59 @@
             >>> # Note that the raw information above contains 'Acting Cj' and thus the designation is only 'J.' At present we only track 'C.J.' and 'J.' titles.
             >>> # With a different date, we can get the 'C.J.' designation.:
             >>> search_cj = CandidateJustice(db=c.db, text='Panganiban', date_str='2006-03-30')
             >>> print(search_cj.choice) # note variance in text designation as acting CJ. vs. J.
             {'id': 137, 'surname': 'Panganiban', 'start_term': '1995-10-05', 'inactive_date': '2006-12-06', 'chief_date': '2005-12-20', 'designation': 'C.J.'}
             >>> c.path_to_db.unlink() # tear down
         """  # noqa: E501
-        opts = []
+        candidate_options = []
         if not self.valid_date:
             return None
-        if not self.candidate:
-            return None
 
-        for candidate in self.rows:
-            if candidate["alias"] and candidate["alias"] == self.candidate:
-                opts.append(candidate)
-                continue
-            elif candidate["surname"] == self.candidate:
-                opts.append(candidate)
-                continue
-        if opts:
-            if len(opts) == 1:
-                res = opts[0]
+        if self.text:
+            # Special rule for duplicate names
+            if "Lopez" in self.text:
+                if "jhosep" in self.text.lower():
+                    for candidate in self.rows:
+                        if int(candidate["id"]) == 190:
+                            candidate_options.append(candidate)
+                elif "mario" in self.text.lower():
+                    for candidate in self.rows:
+                        if int(candidate["id"]) == 185:
+                            candidate_options.append(candidate)
+
+        # only proceed to add more options if special rule not met
+        if not candidate_options:
+            if not self.candidate:
+                return None
+
+            for candidate in self.rows:
+                if candidate["alias"] and candidate["alias"] == self.candidate:
+                    candidate_options.append(candidate)
+                    continue
+                elif candidate["surname"] == self.candidate:
+                    candidate_options.append(candidate)
+                    continue
+
+        if candidate_options:
+            if len(candidate_options) == 1:
+                res = candidate_options[0]
                 res.pop("alias")
                 res["surname"] = res["surname"].title()
                 res["designation"] = "J."
                 if chief_date := res.get("chief_date"):
                     s = parse(chief_date).date()
                     e = parse(res["inactive_date"]).date()
                     if s < self.valid_date < e:
                         res["designation"] = "C.J."
                 return res
             else:
-                print(f"Many {opts=} for {self.candidate=} on {self.valid_date=}")
+                msg = f"Too many {candidate_options=} for {self.candidate=} on {self.valid_date=}. Consider manual intervention."  # noqa: E501
+                logging.error(msg)
+
         return None
 
     @property
     def detail(self) -> JusticeDetail | None:
         """Get object to match fields directly
 
         Examples:
```

### Comparing `corpus_judge-0.0.3/corpus_judge/sc.yaml` & `corpus_judge-0.0.4/corpus_judge/sc.yaml`

 * *Files identical despite different names*

### Comparing `corpus_judge-0.0.3/pyproject.toml` & `corpus_judge-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "corpus-judge"
 description = "Cleaning, setting Justices"
-version = "0.0.3"
+version = "0.0.4"
 authors = ["Marcelino G. Veloso III <mars@veloso.one>"]
 readme = "README.md"
 homepage = "https://mv3.dev"
 repository = "https://github.com/justmars/corpus-judge"
 documentation = "https://justmars.github.io/corpus-judge"
 classifiers = [
   "Programming Language :: Python :: 3.11",
```

### Comparing `corpus_judge-0.0.3/PKG-INFO` & `corpus_judge-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: corpus-judge
-Version: 0.0.3
+Version: 0.0.4
 Summary: Cleaning, setting Justices
 Home-page: https://mv3.dev
 Author: Marcelino G. Veloso III
 Author-email: mars@veloso.one
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
```

