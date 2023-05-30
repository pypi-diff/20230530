# Comparing `tmp/citylex-0.1.8.tar.gz` & `tmp/citylex-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/citylex-0.1.8.tar", last modified: Wed Feb 10 23:25:04 2021, max compression
+gzip compressed data, was "citylex-0.1.9.tar", last modified: Sun Apr 25 22:39:21 2021, max compression
```

## Comparing `citylex-0.1.8.tar` & `citylex-0.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 kbg       (1000) kbg       (1000)        0 2021-02-10 23:25:04.099663 citylex-0.1.8/
--rw-r--r--   0 kbg       (1000) kbg       (1000)     5983 2021-02-10 23:25:04.099663 citylex-0.1.8/PKG-INFO
--rw-r--r--   0 kbg       (1000) kbg       (1000)     4222 2020-11-30 19:39:31.000000 citylex-0.1.8/README.md
-drwxr-xr-x   0 kbg       (1000) kbg       (1000)        0 2021-02-10 23:25:04.099663 citylex-0.1.8/citylex.egg-info/
--rw-rw-r--   0 kbg       (1000) kbg       (1000)     5983 2021-02-10 23:25:03.000000 citylex-0.1.8/citylex.egg-info/PKG-INFO
--rw-rw-r--   0 kbg       (1000) kbg       (1000)      262 2021-02-10 23:25:03.000000 citylex-0.1.8/citylex.egg-info/SOURCES.txt
--rw-rw-r--   0 kbg       (1000) kbg       (1000)        1 2021-02-10 23:25:03.000000 citylex-0.1.8/citylex.egg-info/dependency_links.txt
--rw-rw-r--   0 kbg       (1000) kbg       (1000)       42 2021-02-10 23:25:03.000000 citylex-0.1.8/citylex.egg-info/entry_points.txt
--rw-rw-r--   0 kbg       (1000) kbg       (1000)        1 2020-05-21 13:24:36.000000 citylex-0.1.8/citylex.egg-info/not-zip-safe
--rw-rw-r--   0 kbg       (1000) kbg       (1000)       25 2021-02-10 23:25:03.000000 citylex-0.1.8/citylex.egg-info/requires.txt
--rw-rw-r--   0 kbg       (1000) kbg       (1000)       20 2021-02-10 23:25:03.000000 citylex-0.1.8/citylex.egg-info/top_level.txt
--rw-r--r--   0 kbg       (1000) kbg       (1000)    18823 2021-02-10 23:04:37.000000 citylex-0.1.8/citylex.py
--rw-r--r--   0 kbg       (1000) kbg       (1000)    14887 2021-02-10 23:04:37.000000 citylex-0.1.8/citylex_pb2.py
--rw-r--r--   0 kbg       (1000) kbg       (1000)       38 2021-02-10 23:25:04.099663 citylex-0.1.8/setup.cfg
--rw-r--r--   0 kbg       (1000) kbg       (1000)     1910 2021-02-10 23:20:24.000000 citylex-0.1.8/setup.py
+drwxrwxr-x   0 kbg       (1000) kbg       (1000)        0 2021-04-25 22:39:21.963004 citylex-0.1.9/
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     6001 2021-04-25 22:39:21.963004 citylex-0.1.9/PKG-INFO
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     4240 2021-04-23 20:59:52.000000 citylex-0.1.9/README.md
+drwxrwxr-x   0 kbg       (1000) kbg       (1000)        0 2021-04-25 22:39:21.963004 citylex-0.1.9/citylex.egg-info/
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     6001 2021-04-25 22:39:21.000000 citylex-0.1.9/citylex.egg-info/PKG-INFO
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)      262 2021-04-25 22:39:21.000000 citylex-0.1.9/citylex.egg-info/SOURCES.txt
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)        1 2021-04-25 22:39:21.000000 citylex-0.1.9/citylex.egg-info/dependency_links.txt
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)       42 2021-04-25 22:39:21.000000 citylex-0.1.9/citylex.egg-info/entry_points.txt
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)        1 2021-04-25 22:39:21.000000 citylex-0.1.9/citylex.egg-info/not-zip-safe
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)       25 2021-04-25 22:39:21.000000 citylex-0.1.9/citylex.egg-info/requires.txt
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)       20 2021-04-25 22:39:21.000000 citylex-0.1.9/citylex.egg-info/top_level.txt
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)    18841 2021-04-23 21:04:26.000000 citylex-0.1.9/citylex.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)    14887 2021-04-23 20:59:52.000000 citylex-0.1.9/citylex_pb2.py
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)       38 2021-04-25 22:39:21.963004 citylex-0.1.9/setup.cfg
+-rw-rw-r--   0 kbg       (1000) kbg       (1000)     1910 2021-04-23 21:01:08.000000 citylex-0.1.9/setup.py
```

### Comparing `citylex-0.1.8/PKG-INFO` & `citylex-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citylex
-Version: 0.1.8
+Version: 0.1.9
 Summary: Builds a multisource English lexicon
 Home-page: https://github.com/kylebgorman/citylex
 Author: Kyle Gorman
 Author-email: kylebgorman@gmail.com
 License: Apache 2.0
 Description: 🗽 CityLex: a free multisource English lexical database
         ======================================================
@@ -102,18 +102,18 @@
         
         -   [`citylex.proto`](citylex.proto) for the protocol buffer data structure
         -   [`citylex.bib`](citylex.bib) for references to the data sources used
         
         For contributors
         ----------------
         
-        To regenerate `citylex_pb2.py` you will need to install the [Protocol Buffers
-        C++ runtime](https://github.com/protocolbuffers/protobuf) for your platform,
-        making sure the version number (e.g., the one returned by `protoc --version`
-        matches that of `protobuf` in `requirements.txt`. Then, run
+        To regenerate [`citylex_pb2.py`](citylex_pb2.py) you will need to install the
+        [Protocol Buffers C++ runtime](https://github.com/protocolbuffers/protobuf)
+        for your platform, making sure the version number (e.g., the one returned by
+        `protoc --version` matches that of `protobuf` in `requirements.txt`. Then, run
         `protoc --python_out=. citylex.proto`.
         
         License
         -------
         
         The CityLex codebase are distributed under the Apache 2.0 license. Please see
         [`License.txt`](LICENSE.txt) for details.
```

### Comparing `citylex-0.1.8/README.md` & `citylex-0.1.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -94,18 +94,18 @@
 
 -   [`citylex.proto`](citylex.proto) for the protocol buffer data structure
 -   [`citylex.bib`](citylex.bib) for references to the data sources used
 
 For contributors
 ----------------
 
-To regenerate `citylex_pb2.py` you will need to install the [Protocol Buffers
-C++ runtime](https://github.com/protocolbuffers/protobuf) for your platform,
-making sure the version number (e.g., the one returned by `protoc --version`
-matches that of `protobuf` in `requirements.txt`. Then, run
+To regenerate [`citylex_pb2.py`](citylex_pb2.py) you will need to install the
+[Protocol Buffers C++ runtime](https://github.com/protocolbuffers/protobuf)
+for your platform, making sure the version number (e.g., the one returned by
+`protoc --version` matches that of `protobuf` in `requirements.txt`. Then, run
 `protoc --python_out=. citylex.proto`.
 
 License
 -------
 
 The CityLex codebase are distributed under the Apache 2.0 license. Please see
 [`License.txt`](LICENSE.txt) for details.
```

### Comparing `citylex-0.1.8/citylex.egg-info/PKG-INFO` & `citylex-0.1.9/citylex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citylex
-Version: 0.1.8
+Version: 0.1.9
 Summary: Builds a multisource English lexicon
 Home-page: https://github.com/kylebgorman/citylex
 Author: Kyle Gorman
 Author-email: kylebgorman@gmail.com
 License: Apache 2.0
 Description: 🗽 CityLex: a free multisource English lexical database
         ======================================================
@@ -102,18 +102,18 @@
         
         -   [`citylex.proto`](citylex.proto) for the protocol buffer data structure
         -   [`citylex.bib`](citylex.bib) for references to the data sources used
         
         For contributors
         ----------------
         
-        To regenerate `citylex_pb2.py` you will need to install the [Protocol Buffers
-        C++ runtime](https://github.com/protocolbuffers/protobuf) for your platform,
-        making sure the version number (e.g., the one returned by `protoc --version`
-        matches that of `protobuf` in `requirements.txt`. Then, run
+        To regenerate [`citylex_pb2.py`](citylex_pb2.py) you will need to install the
+        [Protocol Buffers C++ runtime](https://github.com/protocolbuffers/protobuf)
+        for your platform, making sure the version number (e.g., the one returned by
+        `protoc --version` matches that of `protobuf` in `requirements.txt`. Then, run
         `protoc --python_out=. citylex.proto`.
         
         License
         -------
         
         The CityLex codebase are distributed under the Apache 2.0 license. Please see
         [`License.txt`](LICENSE.txt) for details.
```

### Comparing `citylex-0.1.8/citylex.py` & `citylex-0.1.9/citylex.py`

 * *Files 1% similar despite different names*

```diff
@@ -369,15 +369,15 @@
 
 
 def _wikipron_uk(lexicon: citylex_pb2.Lexicon) -> None:
     """Collects WikiPron US pronunciations."""
     counter = 0
     url = (
         "https://raw.githubusercontent.com/kylebgorman/"
-        "wikipron/master/data/tsv/eng_uk_phonemic_filtered.tsv"
+        "wikipron/master/data/scrape/tsv/eng_latn_us_broad_filtered.tsv"
     )
     for line in _request_url_resource(url):
         (wordform, pron, *_) = line.rstrip().split("\t")
         wordform = _normalize(wordform)
         lexicon.entry[wordform].wikipron_uk_pron.append(pron)
         counter += 1
     assert counter, "No data read"
@@ -388,15 +388,15 @@
 
 
 def _wikipron_us(lexicon: citylex_pb2.Lexicon) -> None:
     """Collects WikiPron US pronunciations."""
     counter = 0
     url = (
         "https://raw.githubusercontent.com/kylebgorman/"
-        "wikipron/master/data/tsv/eng_us_phonemic_filtered.tsv"
+        "wikipron/master/data/scrape/tsv/eng_latn_us_broad_filtered.tsv"
     )
     for line in _request_url_resource(url):
         (wordform, pron, *_) = line.rstrip().split("\t")
         wordform = _normalize(wordform)
         lexicon.entry[wordform].wikipron_us_pron.append(pron)
         counter += 1
     assert counter, "No data read"
@@ -417,15 +417,15 @@
         default="citylex.tsv",
         help="output TSV path (default: %(default)s)",
     )
     # Enables specific data sources.
     parser.add_argument(
         "--all-free",
         action="store_true",
-        help="extracts all free data sources"
+        help="extract all free data sources"
     )
     parser.add_argument(
         "--celex",
         action="store_true",
         help="extract CELEX data (proprietary use agreement): "
         "http://catalog.ldc.upenn.edu/license/celex-user-agreement.pdf",
     )
@@ -462,15 +462,15 @@
         action="store_true",
         help="extract Apertium UDLexicons data (GPL 3.0): "
         "https://opensource.org/licenses/GPL-3.0",
     )
     parser.add_argument(
         "--unimorph",
         action="store_true",
-        help="extract UniMorph data (C BY-SA 2.0): "
+        help="extract UniMorph data (CC BY-SA 2.0): "
         "http://creativecommons.org/licenses/by-sa/2.0/",
     )
     parser.add_argument(
         "--wikipron-uk",
         action="store_true",
         help="extract WikiPron UK data (CC BY-SA 3.0 Unported): "
         "http://creativecommons.org/licenses/by-sa/3.0/",
```

### Comparing `citylex-0.1.8/citylex_pb2.py` & `citylex-0.1.9/citylex_pb2.py`

 * *Files identical despite different names*

### Comparing `citylex-0.1.8/setup.py` & `citylex-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 _THIS_DIR = os.path.dirname(os.path.realpath(__file__))
 
 
 with open(os.path.join(_THIS_DIR, "README.md")) as f:
     _LONG_DESCRIPTION = f.read().strip()
 
 
-__version__ = "0.1.8"
+__version__ = "0.1.9"
 
 
 def main() -> None:
     setuptools.setup(
         name="citylex",
         version=__version__,
         author="Kyle Gorman",
```

