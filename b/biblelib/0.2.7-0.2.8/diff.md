# Comparing `tmp/biblelib-0.2.7.tar.gz` & `tmp/biblelib-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biblelib-0.2.7.tar", max compression
+gzip compressed data, was "biblelib-0.2.8.tar", max compression
```

## Comparing `biblelib-0.2.7.tar` & `biblelib-0.2.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     3326 2023-05-12 17:59:15.958698 biblelib-0.2.7/LICENSE.md
--rw-r--r--   0        0        0     3337 2023-05-12 17:50:39.199097 biblelib-0.2.7/LICENSE.md~
--rw-r--r--   0        0        0     2048 2023-05-12 17:45:43.797503 biblelib-0.2.7/README.md
--rw-r--r--   0        0        0      207 2022-11-11 00:55:36.561996 biblelib-0.2.7/biblelib/__init__.py
--rw-r--r--   0        0        0      946 2023-05-12 17:25:25.324552 biblelib-0.2.7/biblelib/book/ReadMe.md
--rw-r--r--   0        0        0      350 2023-03-24 13:53:37.422750 biblelib-0.2.7/biblelib/book/__init__.py
--rw-r--r--   0        0        0    12780 2023-04-22 23:14:16.335752 biblelib-0.2.7/biblelib/book/book.py
--rw-r--r--   0        0        0     4755 2023-05-12 17:23:39.309175 biblelib-0.2.7/biblelib/book/books.tsv
--rw-r--r--   0        0        0      474 2023-04-09 04:44:24.570950 biblelib-0.2.7/biblelib/unit/__init__.py
--rw-r--r--   0        0        0     5788 2023-04-10 12:29:36.110427 biblelib-0.2.7/biblelib/unit/book.py
--rw-r--r--   0        0        0     1770 2023-03-30 03:30:47.201892 biblelib-0.2.7/biblelib/unit/bookchapters.tsv
--rw-r--r--   0        0        0     6972 2023-04-10 12:30:22.815665 biblelib-0.2.7/biblelib/unit/chapter.py
--rw-r--r--   0        0        0     1770 2023-03-24 23:24:06.076120 biblelib-0.2.7/biblelib/unit/chapters.tsv
--rw-r--r--   0        0        0    23363 2023-03-30 03:30:50.093429 biblelib-0.2.7/biblelib/unit/chapterverses.tsv
--rw-r--r--   0        0        0    29962 2023-03-30 03:30:33.249866 biblelib-0.2.7/biblelib/unit/tempchapter.py
--rw-r--r--   0        0        0     3332 2023-03-30 05:04:49.035453 biblelib-0.2.7/biblelib/unit/unit.py
--rw-r--r--   0        0        0     1240 2023-03-24 18:41:28.150962 biblelib-0.2.7/biblelib/unit/verse.py
--rw-r--r--   0        0        0     1348 2023-05-12 17:27:37.060726 biblelib-0.2.7/biblelib/versification/ReadMe.md
--rw-r--r--   0        0        0   431827 2021-10-25 18:19:51.303000 biblelib-0.2.7/biblelib/versification/vref-bcv.txt
--rw-r--r--   0        0        0   431827 2021-10-25 18:19:51.303000 biblelib-0.2.7/biblelib/versification/vref.txt
--rw-r--r--   0        0        0      199 2023-05-08 18:22:24.370434 biblelib-0.2.7/biblelib/versification/vrefmap.py
--rw-r--r--   0        0        0      786 2023-05-26 19:35:46.225675 biblelib-0.2.7/biblelib/word/__init__.py
--rw-r--r--   0        0        0    16067 2023-05-30 00:44:58.415393 biblelib-0.2.7/biblelib/word/bcvwpid.py
--rw-r--r--   0        0        0     4432 2022-11-17 00:30:21.039343 biblelib-0.2.7/biblelib/word/mappings.py
--rw-r--r--   0        0        0     1189 2023-05-30 00:57:11.215058 biblelib-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     2843 1970-01-01 00:00:00.000000 biblelib-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     3326 2023-05-12 17:59:15.958698 biblelib-0.2.8/LICENSE.md
+-rw-r--r--   0        0        0     3337 2023-05-12 17:50:39.199097 biblelib-0.2.8/LICENSE.md~
+-rw-r--r--   0        0        0     2048 2023-05-12 17:45:43.797503 biblelib-0.2.8/README.md
+-rw-r--r--   0        0        0      207 2022-11-11 00:55:36.561996 biblelib-0.2.8/biblelib/__init__.py
+-rw-r--r--   0        0        0      946 2023-05-12 17:25:25.324552 biblelib-0.2.8/biblelib/book/ReadMe.md
+-rw-r--r--   0        0        0      350 2023-03-24 13:53:37.422750 biblelib-0.2.8/biblelib/book/__init__.py
+-rw-r--r--   0        0        0    12780 2023-04-22 23:14:16.335752 biblelib-0.2.8/biblelib/book/book.py
+-rw-r--r--   0        0        0     4755 2023-05-30 01:05:17.747681 biblelib-0.2.8/biblelib/book/books.tsv
+-rw-r--r--   0        0        0      474 2023-04-09 04:44:24.570950 biblelib-0.2.8/biblelib/unit/__init__.py
+-rw-r--r--   0        0        0     5788 2023-04-10 12:29:36.110427 biblelib-0.2.8/biblelib/unit/book.py
+-rw-r--r--   0        0        0     1770 2023-03-30 03:30:47.201892 biblelib-0.2.8/biblelib/unit/bookchapters.tsv
+-rw-r--r--   0        0        0     6972 2023-04-10 12:30:22.815665 biblelib-0.2.8/biblelib/unit/chapter.py
+-rw-r--r--   0        0        0     1770 2023-03-24 23:24:06.076120 biblelib-0.2.8/biblelib/unit/chapters.tsv
+-rw-r--r--   0        0        0    23363 2023-03-30 03:30:50.093429 biblelib-0.2.8/biblelib/unit/chapterverses.tsv
+-rw-r--r--   0        0        0    29962 2023-03-30 03:30:33.249866 biblelib-0.2.8/biblelib/unit/tempchapter.py
+-rw-r--r--   0        0        0     3332 2023-03-30 05:04:49.035453 biblelib-0.2.8/biblelib/unit/unit.py
+-rw-r--r--   0        0        0     1240 2023-03-24 18:41:28.150962 biblelib-0.2.8/biblelib/unit/verse.py
+-rw-r--r--   0        0        0     1348 2023-05-12 17:27:37.060726 biblelib-0.2.8/biblelib/versification/ReadMe.md
+-rw-r--r--   0        0        0   431827 2021-10-25 18:19:51.303000 biblelib-0.2.8/biblelib/versification/vref-bcv.txt
+-rw-r--r--   0        0        0   431827 2021-10-25 18:19:51.303000 biblelib-0.2.8/biblelib/versification/vref.txt
+-rw-r--r--   0        0        0      199 2023-05-08 18:22:24.370434 biblelib-0.2.8/biblelib/versification/vrefmap.py
+-rw-r--r--   0        0        0      786 2023-05-26 19:35:46.225675 biblelib-0.2.8/biblelib/word/__init__.py
+-rw-r--r--   0        0        0    16067 2023-05-30 00:44:58.415393 biblelib-0.2.8/biblelib/word/bcvwpid.py
+-rw-r--r--   0        0        0     4432 2022-11-17 00:30:21.039343 biblelib-0.2.8/biblelib/word/mappings.py
+-rw-r--r--   0        0        0     1189 2023-05-30 01:06:40.167862 biblelib-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0     2843 1970-01-01 00:00:00.000000 biblelib-0.2.8/PKG-INFO
```

### Comparing `biblelib-0.2.7/LICENSE.md` & `biblelib-0.2.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.7/LICENSE.md~` & `biblelib-0.2.8/LICENSE.md~`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.7/README.md` & `biblelib-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.7/biblelib/book/ReadMe.md` & `biblelib-0.2.8/biblelib/book/ReadMe.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.7/biblelib/book/book.py` & `biblelib-0.2.8/biblelib/book/book.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.7/biblelib/book/books.tsv` & `biblelib-0.2.8/biblelib/book/books.tsv`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 61	40	MAT	Matt	Matthew	The Gospel according to Matthew
 62	41	MRK	Mark	Mark	The Gospel according to Mark
 63	42	LUK	Luke	Luke	The Gospel according to Luke
 64	43	JHN	John	John	The Gospel according to John
 65	44	ACT	Acts	Acts	The Acts of the Apostles
 66	45	ROM	Rom	Romans	The Letter of Paul to the Romans
 67	46	1CO	1Cor	1 Corinthians	The First Letter of Paul to the Corinthians
-68	47	2CO	2cor	2 Corinthians	The Second Letter of Paul to the Corinthians
+68	47	2CO	2Cor	2 Corinthians	The Second Letter of Paul to the Corinthians
 69	48	GAL	Gal	Galatians	The Letter of Paul to the Galatians
 70	49	EPH	Eph	Ephesians	The Letter of Paul to the Ephesians
 71	50	PHP	Phil	Philippians	The Letter of Paul to the Philippians
 72	51	COL	Col	Colossians	The Letter of Paul to the Colossians
 73	52	1TH	1Thess	1 Thessalonians	The First Letter of Paul to the Thessalonians
 74	53	2TH	2Thess	2 Thessalonians	The Second Letter of Paul to the Thessalonians
 75	54	1TI	1Tim	1 Timothy	The First Letter of Paul to Timothy
```

### Comparing `biblelib-0.2.7/biblelib/unit/book.py` & `biblelib-0.2.8/biblelib/unit/book.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.7/biblelib/unit/bookchapters.tsv` & `biblelib-0.2.8/biblelib/unit/bookchapters.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.7/biblelib/unit/chapter.py` & `biblelib-0.2.8/biblelib/unit/chapter.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.7/biblelib/unit/chapters.tsv` & `biblelib-0.2.8/biblelib/unit/chapters.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.7/biblelib/unit/chapterverses.tsv` & `biblelib-0.2.8/biblelib/unit/chapterverses.tsv`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.7/biblelib/unit/tempchapter.py` & `biblelib-0.2.8/biblelib/unit/tempchapter.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.7/biblelib/unit/unit.py` & `biblelib-0.2.8/biblelib/unit/unit.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.7/biblelib/unit/verse.py` & `biblelib-0.2.8/biblelib/unit/verse.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.7/biblelib/versification/ReadMe.md` & `biblelib-0.2.8/biblelib/versification/ReadMe.md`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.7/biblelib/versification/vref-bcv.txt` & `biblelib-0.2.8/biblelib/versification/vref-bcv.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.7/biblelib/versification/vref.txt` & `biblelib-0.2.8/biblelib/versification/vref.txt`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.7/biblelib/word/__init__.py` & `biblelib-0.2.8/biblelib/word/__init__.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.7/biblelib/word/bcvwpid.py` & `biblelib-0.2.8/biblelib/word/bcvwpid.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.7/biblelib/word/mappings.py` & `biblelib-0.2.8/biblelib/word/mappings.py`

 * *Files identical despite different names*

### Comparing `biblelib-0.2.7/pyproject.toml` & `biblelib-0.2.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "biblelib"
-version = "0.2.7"
+version = "0.2.8"
 description = "Utilities for working with metadata for Bible books, references, pericopes, and other units."
 authors = ["Sean Boisen <sean.boisen@gmail.com>"]
 repository = "https://github.com/Clear-Bible/Biblelib/"
 # documentation = "https://sboisen.github.io/Biblelib/"
 readme = "README.md"
 packages = [
   {include = "biblelib"}
```

### Comparing `biblelib-0.2.7/PKG-INFO` & `biblelib-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: biblelib
-Version: 0.2.7
+Version: 0.2.8
 Summary: Utilities for working with metadata for Bible books, references, pericopes, and other units.
 Home-page: https://github.com/Clear-Bible/Biblelib/
 Author: Sean Boisen
 Author-email: sean.boisen@gmail.com
 Requires-Python: >=3.8,<=3.11
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

