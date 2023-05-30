# Comparing `tmp/mathbib-0.4.0.tar.gz` & `tmp/mathbib-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mathbib-0.4.0.tar", max compression
+gzip compressed data, was "mathbib-0.5.0.tar", max compression
```

## Comparing `mathbib-0.4.0.tar` & `mathbib-0.5.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1070 2023-05-29 16:29:17.682650 mathbib-0.4.0/LICENSE
--rw-r--r--   0        0        0     5351 2023-05-29 16:41:55.640378 mathbib-0.4.0/README.md
--rw-r--r--   0        0        0      143 2023-05-29 16:27:47.709639 mathbib-0.4.0/mathbib/__init__.py
--rw-r--r--   0        0        0       63 2023-05-10 21:47:55.276481 mathbib-0.4.0/mathbib/__main__.py
--rw-r--r--   0        0        0     1402 2023-05-28 11:08:27.988644 mathbib-0.4.0/mathbib/bibtex.py
--rw-r--r--   0        0        0     2831 2023-05-28 15:54:03.882001 mathbib-0.4.0/mathbib/citegen.py
--rw-r--r--   0        0        0    10039 2023-05-30 14:37:18.467319 mathbib-0.4.0/mathbib/command.py
--rw-r--r--   0        0        0     2841 2023-05-28 16:33:13.843882 mathbib-0.4.0/mathbib/partition.py
--rw-r--r--   0        0        0     9459 2023-05-28 15:11:22.084659 mathbib-0.4.0/mathbib/record.py
--rw-r--r--   0        0        0     5481 2023-05-28 13:40:33.677396 mathbib-0.4.0/mathbib/remote/__init__.py
--rw-r--r--   0        0        0     3088 2023-05-28 12:38:27.635690 mathbib-0.4.0/mathbib/remote/arxiv.py
--rw-r--r--   0        0        0      923 2023-05-27 20:04:18.325197 mathbib-0.4.0/mathbib/remote/doi.py
--rw-r--r--   0        0        0      855 2023-05-28 09:33:03.953274 mathbib-0.4.0/mathbib/remote/error.py
--rw-r--r--   0        0        0     1475 2023-05-27 20:04:18.354984 mathbib-0.4.0/mathbib/remote/isbn.py
--rw-r--r--   0        0        0     1194 2023-05-27 18:35:57.528452 mathbib-0.4.0/mathbib/remote/ol.py
--rw-r--r--   0        0        0     4257 2023-05-28 15:10:12.248626 mathbib-0.4.0/mathbib/remote/utils.py
--rw-r--r--   0        0        0      597 2023-05-25 12:11:18.575783 mathbib-0.4.0/mathbib/remote/zbl.py
--rw-r--r--   0        0        0     1816 2023-05-28 12:19:04.718450 mathbib-0.4.0/mathbib/remote/zbmath.py
--rw-r--r--   0        0        0     5512 2023-05-29 16:27:20.815594 mathbib-0.4.0/mathbib/request.py
--rw-r--r--   0        0        0        0 2023-05-25 15:24:07.234292 mathbib-0.4.0/mathbib/resources/__init__.py
--rw-r--r--   0        0        0   270192 2023-05-25 15:19:42.503313 mathbib-0.4.0/mathbib/resources/journal_abbrevs.json
--rw-r--r--   0        0        0     2613 2023-05-28 12:14:16.785236 mathbib-0.4.0/mathbib/session.py
--rw-r--r--   0        0        0      705 2023-05-25 11:53:39.451875 mathbib-0.4.0/mathbib/term.py
--rw-r--r--   0        0        0      917 2023-05-30 14:39:27.955239 mathbib-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     6240 1970-01-01 00:00:00.000000 mathbib-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-29 16:29:17.682650 mathbib-0.5.0/LICENSE
+-rw-r--r--   0        0        0     5351 2023-05-29 16:41:55.640378 mathbib-0.5.0/README.md
+-rw-r--r--   0        0        0      143 2023-05-29 16:27:47.709639 mathbib-0.5.0/mathbib/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-10 21:47:55.276481 mathbib-0.5.0/mathbib/__main__.py
+-rw-r--r--   0        0        0     1402 2023-05-28 11:08:27.988644 mathbib-0.5.0/mathbib/bibtex.py
+-rw-r--r--   0        0        0     2831 2023-05-28 15:54:03.882001 mathbib-0.5.0/mathbib/citegen.py
+-rw-r--r--   0        0        0    10046 2023-05-30 15:28:52.311478 mathbib-0.5.0/mathbib/command.py
+-rw-r--r--   0        0        0     2841 2023-05-28 16:33:13.843882 mathbib-0.5.0/mathbib/partition.py
+-rw-r--r--   0        0        0     9459 2023-05-28 15:11:22.084659 mathbib-0.5.0/mathbib/record.py
+-rw-r--r--   0        0        0     5481 2023-05-28 13:40:33.677396 mathbib-0.5.0/mathbib/remote/__init__.py
+-rw-r--r--   0        0        0     3088 2023-05-28 12:38:27.635690 mathbib-0.5.0/mathbib/remote/arxiv.py
+-rw-r--r--   0        0        0      923 2023-05-27 20:04:18.325197 mathbib-0.5.0/mathbib/remote/doi.py
+-rw-r--r--   0        0        0      855 2023-05-28 09:33:03.953274 mathbib-0.5.0/mathbib/remote/error.py
+-rw-r--r--   0        0        0     1475 2023-05-27 20:04:18.354984 mathbib-0.5.0/mathbib/remote/isbn.py
+-rw-r--r--   0        0        0     1194 2023-05-27 18:35:57.528452 mathbib-0.5.0/mathbib/remote/ol.py
+-rw-r--r--   0        0        0     4257 2023-05-28 15:10:12.248626 mathbib-0.5.0/mathbib/remote/utils.py
+-rw-r--r--   0        0        0      597 2023-05-25 12:11:18.575783 mathbib-0.5.0/mathbib/remote/zbl.py
+-rw-r--r--   0        0        0     1816 2023-05-28 12:19:04.718450 mathbib-0.5.0/mathbib/remote/zbmath.py
+-rw-r--r--   0        0        0     5512 2023-05-29 16:27:20.815594 mathbib-0.5.0/mathbib/request.py
+-rw-r--r--   0        0        0        0 2023-05-25 15:24:07.234292 mathbib-0.5.0/mathbib/resources/__init__.py
+-rw-r--r--   0        0        0   270192 2023-05-25 15:19:42.503313 mathbib-0.5.0/mathbib/resources/journal_abbrevs.json
+-rw-r--r--   0        0        0     2613 2023-05-28 12:14:16.785236 mathbib-0.5.0/mathbib/session.py
+-rw-r--r--   0        0        0      705 2023-05-25 11:53:39.451875 mathbib-0.5.0/mathbib/term.py
+-rw-r--r--   0        0        0      917 2023-05-30 15:28:04.393078 mathbib-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     6240 1970-01-01 00:00:00.000000 mathbib-0.5.0/PKG-INFO
```

### Comparing `mathbib-0.4.0/LICENSE` & `mathbib-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mathbib-0.4.0/README.md` & `mathbib-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `mathbib-0.4.0/mathbib/bibtex.py` & `mathbib-0.5.0/mathbib/bibtex.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.4.0/mathbib/citegen.py` & `mathbib-0.5.0/mathbib/citegen.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.4.0/mathbib/command.py` & `mathbib-0.5.0/mathbib/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,15 @@
     toml_record = dumps(record.as_toml())
 
     while True:
         edited = click.edit(toml_record, extension=".toml")
         if edited is not None:
             try:
                 loads(edited)
-                record.keyid.toml_path().mkdir(parents=True, exist_ok=True)
+                record.keyid.toml_path().parent.mkdir(parents=True, exist_ok=True)
                 record.keyid.toml_path().write_text(edited)
                 return
 
             except TOMLDecodeError as e:
                 TermWrite.error(f"invalid TOML: {e}")
 
             if click.confirm("Edit again?"):
```

### Comparing `mathbib-0.4.0/mathbib/partition.py` & `mathbib-0.5.0/mathbib/partition.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.4.0/mathbib/record.py` & `mathbib-0.5.0/mathbib/record.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.4.0/mathbib/remote/__init__.py` & `mathbib-0.5.0/mathbib/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.4.0/mathbib/remote/arxiv.py` & `mathbib-0.5.0/mathbib/remote/arxiv.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.4.0/mathbib/remote/doi.py` & `mathbib-0.5.0/mathbib/remote/doi.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.4.0/mathbib/remote/error.py` & `mathbib-0.5.0/mathbib/remote/error.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.4.0/mathbib/remote/isbn.py` & `mathbib-0.5.0/mathbib/remote/isbn.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.4.0/mathbib/remote/ol.py` & `mathbib-0.5.0/mathbib/remote/ol.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.4.0/mathbib/remote/utils.py` & `mathbib-0.5.0/mathbib/remote/utils.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.4.0/mathbib/remote/zbl.py` & `mathbib-0.5.0/mathbib/remote/zbl.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.4.0/mathbib/remote/zbmath.py` & `mathbib-0.5.0/mathbib/remote/zbmath.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.4.0/mathbib/request.py` & `mathbib-0.5.0/mathbib/request.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.4.0/mathbib/resources/journal_abbrevs.json` & `mathbib-0.5.0/mathbib/resources/journal_abbrevs.json`

 * *Files identical despite different names*

### Comparing `mathbib-0.4.0/mathbib/session.py` & `mathbib-0.5.0/mathbib/session.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.4.0/mathbib/term.py` & `mathbib-0.5.0/mathbib/term.py`

 * *Files identical despite different names*

### Comparing `mathbib-0.4.0/pyproject.toml` & `mathbib-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "mathbib"
-version = "0.4.0"
+version = "0.5.0"
 description = "A mathematics BibLaTeX bibliography manager."
 authors = ["Alex Rutar <alex@rutar.org>"]
 readme = "README.md"
 packages = [{include = "mathbib"}]
 license = "MIT"
 repository = "https://github.com/alexrutar/mathbib-py"
 include = ["mathbib/resources/journal_abbrevs.json"]
```

### Comparing `mathbib-0.4.0/PKG-INFO` & `mathbib-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mathbib
-Version: 0.4.0
+Version: 0.5.0
 Summary: A mathematics BibLaTeX bibliography manager.
 Home-page: https://github.com/alexrutar/mathbib-py
 License: MIT
 Author: Alex Rutar
 Author-email: alex@rutar.org
 Requires-Python: >=3.11.0,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

