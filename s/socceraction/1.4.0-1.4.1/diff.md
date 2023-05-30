# Comparing `tmp/socceraction-1.4.0.tar.gz` & `tmp/socceraction-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socceraction-1.4.0.tar", max compression
+gzip compressed data, was "socceraction-1.4.1.tar", max compression
```

## Comparing `socceraction-1.4.0.tar` & `socceraction-1.4.1.tar`

### file list

```diff
@@ -1,53 +1,52 @@
--rw-r--r--   0        0        0     1114 2023-02-18 19:57:37.515886 socceraction-1.4.0/LICENSE.rst
--rw-r--r--   0        0        0     5271 2023-02-18 19:57:37.515886 socceraction-1.4.0/README.md
--rw-r--r--   0        0        0     2774 2023-02-18 19:58:07.577607 socceraction-1.4.0/pyproject.toml
--rw-r--r--   0        0        0      366 2023-02-18 19:58:07.577607 socceraction-1.4.0/socceraction/__init__.py
--rw-r--r--   0        0        0       61 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/atomic/__init__.py
--rw-r--r--   0        0        0      374 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/atomic/spadl/__init__.py
--rw-r--r--   0        0        0     8151 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/atomic/spadl/base.py
--rw-r--r--   0        0        0     1128 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/atomic/spadl/config.py
--rw-r--r--   0        0        0     1324 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/atomic/spadl/schema.py
--rw-r--r--   0        0        0     1897 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/atomic/spadl/utils.py
--rw-r--r--   0        0        0      172 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/atomic/vaep/__init__.py
--rw-r--r--   0        0        0     2327 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/atomic/vaep/base.py
--rw-r--r--   0        0        0     7724 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/atomic/vaep/features.py
--rw-r--r--   0        0        0     4677 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/atomic/vaep/formula.py
--rw-r--r--   0        0        0     3954 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/atomic/vaep/labels.py
--rw-r--r--   0        0        0      169 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/__init__.py
--rw-r--r--   0        0        0     5468 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/base.py
--rw-r--r--   0        0        0      361 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/opta/__init__.py
--rw-r--r--   0        0        0    15834 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/opta/loader.py
--rw-r--r--   0        0        0      557 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/opta/parsers/__init__.py
--rw-r--r--   0        0        0     4803 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/opta/parsers/base.py
--rw-r--r--   0        0        0     3882 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/opta/parsers/f1_json.py
--rw-r--r--   0        0        0     4463 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/opta/parsers/f24_json.py
--rw-r--r--   0        0        0     3971 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/opta/parsers/f24_xml.py
--rw-r--r--   0        0        0     9938 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/opta/parsers/f7_xml.py
--rw-r--r--   0        0        0    11898 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/opta/parsers/f9_json.py
--rw-r--r--   0        0        0    11432 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/opta/parsers/ma1_json.py
--rw-r--r--   0        0        0    14294 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/opta/parsers/ma3_json.py
--rw-r--r--   0        0        0    18167 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/opta/parsers/whoscored.py
--rw-r--r--   0        0        0     3302 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/opta/schema.py
--rw-r--r--   0        0        0     3920 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/schema.py
--rw-r--r--   0        0        0      476 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/statsbomb/__init__.py
--rw-r--r--   0        0        0    17692 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/statsbomb/loader.py
--rw-r--r--   0        0        0     4205 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/statsbomb/schema.py
--rw-r--r--   0        0        0      448 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/wyscout/__init__.py
--rw-r--r--   0        0        0    31818 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/wyscout/loader.py
--rw-r--r--   0        0        0     1246 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/data/wyscout/schema.py
--rw-r--r--   0        0        0      429 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/spadl/__init__.py
--rw-r--r--   0        0        0     2913 2023-02-18 19:57:37.575890 socceraction-1.4.0/socceraction/spadl/base.py
--rw-r--r--   0        0        0     2195 2023-02-18 19:57:37.579890 socceraction-1.4.0/socceraction/spadl/config.py
--rw-r--r--   0        0        0     5523 2023-02-18 19:57:37.579890 socceraction-1.4.0/socceraction/spadl/opta.py
--rw-r--r--   0        0        0     1446 2023-02-18 19:57:37.579890 socceraction-1.4.0/socceraction/spadl/schema.py
--rw-r--r--   0        0        0    10124 2023-02-18 19:57:37.579890 socceraction-1.4.0/socceraction/spadl/statsbomb.py
--rw-r--r--   0        0        0     1862 2023-02-18 19:57:37.579890 socceraction-1.4.0/socceraction/spadl/utils.py
--rw-r--r--   0        0        0    30351 2023-02-18 19:57:37.579890 socceraction-1.4.0/socceraction/spadl/wyscout.py
--rw-r--r--   0        0        0      153 2023-02-18 19:57:37.579890 socceraction-1.4.0/socceraction/vaep/__init__.py
--rw-r--r--   0        0        0    12922 2023-02-18 19:57:37.579890 socceraction-1.4.0/socceraction/vaep/base.py
--rw-r--r--   0        0        0    18789 2023-02-18 19:57:37.579890 socceraction-1.4.0/socceraction/vaep/features.py
--rw-r--r--   0        0        0     4882 2023-02-18 19:57:37.579890 socceraction-1.4.0/socceraction/vaep/formula.py
--rw-r--r--   0        0        0     4011 2023-02-18 19:57:37.579890 socceraction-1.4.0/socceraction/vaep/labels.py
--rw-r--r--   0        0        0    16919 2023-02-18 19:57:37.579890 socceraction-1.4.0/socceraction/xthreat.py
--rw-r--r--   0        0        0     6591 1970-01-01 00:00:00.000000 socceraction-1.4.0/setup.py
--rw-r--r--   0        0        0     6561 1970-01-01 00:00:00.000000 socceraction-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1114 2023-05-30 10:02:21.107882 socceraction-1.4.1/LICENSE.rst
+-rw-r--r--   0        0        0     5271 2023-05-30 10:02:21.107882 socceraction-1.4.1/README.md
+-rw-r--r--   0        0        0     2774 2023-05-30 10:02:36.352033 socceraction-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0      366 2023-05-30 10:02:36.352033 socceraction-1.4.1/socceraction/__init__.py
+-rw-r--r--   0        0        0       61 2023-05-30 10:02:21.159883 socceraction-1.4.1/socceraction/atomic/__init__.py
+-rw-r--r--   0        0        0      374 2023-05-30 10:02:21.159883 socceraction-1.4.1/socceraction/atomic/spadl/__init__.py
+-rw-r--r--   0        0        0     8151 2023-05-30 10:02:21.159883 socceraction-1.4.1/socceraction/atomic/spadl/base.py
+-rw-r--r--   0        0        0     1128 2023-05-30 10:02:21.159883 socceraction-1.4.1/socceraction/atomic/spadl/config.py
+-rw-r--r--   0        0        0     1324 2023-05-30 10:02:21.159883 socceraction-1.4.1/socceraction/atomic/spadl/schema.py
+-rw-r--r--   0        0        0     1897 2023-05-30 10:02:21.159883 socceraction-1.4.1/socceraction/atomic/spadl/utils.py
+-rw-r--r--   0        0        0      172 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/atomic/vaep/__init__.py
+-rw-r--r--   0        0        0     2327 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/atomic/vaep/base.py
+-rw-r--r--   0        0        0     7724 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/atomic/vaep/features.py
+-rw-r--r--   0        0        0     4677 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/atomic/vaep/formula.py
+-rw-r--r--   0        0        0     3954 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/atomic/vaep/labels.py
+-rw-r--r--   0        0        0      169 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/__init__.py
+-rw-r--r--   0        0        0     5468 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/base.py
+-rw-r--r--   0        0        0      361 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/opta/__init__.py
+-rw-r--r--   0        0        0    15797 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/opta/loader.py
+-rw-r--r--   0        0        0      557 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/opta/parsers/__init__.py
+-rw-r--r--   0        0        0     4803 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/opta/parsers/base.py
+-rw-r--r--   0        0        0     3882 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/opta/parsers/f1_json.py
+-rw-r--r--   0        0        0     4463 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/opta/parsers/f24_json.py
+-rw-r--r--   0        0        0     3971 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/opta/parsers/f24_xml.py
+-rw-r--r--   0        0        0     9938 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/opta/parsers/f7_xml.py
+-rw-r--r--   0        0        0    11898 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/opta/parsers/f9_json.py
+-rw-r--r--   0        0        0    11432 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/opta/parsers/ma1_json.py
+-rw-r--r--   0        0        0    14294 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/opta/parsers/ma3_json.py
+-rw-r--r--   0        0        0    18167 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/opta/parsers/whoscored.py
+-rw-r--r--   0        0        0     3302 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/opta/schema.py
+-rw-r--r--   0        0        0     3920 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/schema.py
+-rw-r--r--   0        0        0      476 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/statsbomb/__init__.py
+-rw-r--r--   0        0        0    17692 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/statsbomb/loader.py
+-rw-r--r--   0        0        0     4205 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/statsbomb/schema.py
+-rw-r--r--   0        0        0      448 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/wyscout/__init__.py
+-rw-r--r--   0        0        0    32143 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/wyscout/loader.py
+-rw-r--r--   0        0        0     1246 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/data/wyscout/schema.py
+-rw-r--r--   0        0        0      429 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/spadl/__init__.py
+-rw-r--r--   0        0        0     2913 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/spadl/base.py
+-rw-r--r--   0        0        0     2195 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/spadl/config.py
+-rw-r--r--   0        0        0     5523 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/spadl/opta.py
+-rw-r--r--   0        0        0     1446 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/spadl/schema.py
+-rw-r--r--   0        0        0    10124 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/spadl/statsbomb.py
+-rw-r--r--   0        0        0     1862 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/spadl/utils.py
+-rw-r--r--   0        0        0    30351 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/spadl/wyscout.py
+-rw-r--r--   0        0        0      153 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/vaep/__init__.py
+-rw-r--r--   0        0        0    12922 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/vaep/base.py
+-rw-r--r--   0        0        0    18789 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/vaep/features.py
+-rw-r--r--   0        0        0     4882 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/vaep/formula.py
+-rw-r--r--   0        0        0     4011 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/vaep/labels.py
+-rw-r--r--   0        0        0    16936 2023-05-30 10:02:21.163883 socceraction-1.4.1/socceraction/xthreat.py
+-rw-r--r--   0        0        0     6561 1970-01-01 00:00:00.000000 socceraction-1.4.1/PKG-INFO
```

### Comparing `socceraction-1.4.0/LICENSE.rst` & `socceraction-1.4.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/README.md` & `socceraction-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/pyproject.toml` & `socceraction-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "socceraction"
-version = "1.4.0"
+version = "1.4.1"
 description = "Convert soccer event stream data to the SPADL format and value on-the-ball player actions"
 authors = ["Tom Decroos <tom.decroos.be@gmail.com>", "Pieter Robberechts <pieter.robberechts@kuleuven.be>"]
 license = "MIT"
 readme = 'README.md'
 homepage = "https://github.com/ML-KULeuven/socceraction"
 repository = "https://github.com/ML-KULeuven/socceraction"
 documentation = "https://socceraction.readthedocs.io"
```

### Comparing `socceraction-1.4.0/socceraction/atomic/spadl/base.py` & `socceraction-1.4.1/socceraction/atomic/spadl/base.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/atomic/spadl/config.py` & `socceraction-1.4.1/socceraction/atomic/spadl/config.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/atomic/spadl/schema.py` & `socceraction-1.4.1/socceraction/atomic/spadl/schema.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/atomic/spadl/utils.py` & `socceraction-1.4.1/socceraction/atomic/spadl/utils.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/atomic/vaep/base.py` & `socceraction-1.4.1/socceraction/atomic/vaep/base.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/atomic/vaep/features.py` & `socceraction-1.4.1/socceraction/atomic/vaep/features.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/atomic/vaep/formula.py` & `socceraction-1.4.1/socceraction/atomic/vaep/formula.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/atomic/vaep/labels.py` & `socceraction-1.4.1/socceraction/atomic/vaep/labels.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/data/base.py` & `socceraction-1.4.1/socceraction/data/base.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/data/opta/loader.py` & `socceraction-1.4.1/socceraction/data/opta/loader.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Implements serializers for Opta data."""
 import copy
 import datetime
 import glob
 import os
 import re
 import warnings
+from pathlib import Path
 from typing import Any, Dict, Mapping, Optional, Type, Union, cast
 
 import pandas as pd  # type: ignore
 from pandera.typing import DataFrame
 
 from socceraction.data.base import EventDataLoader
 
@@ -198,55 +199,50 @@
     if m is None:
         raise ValueError(f"The filepath {path} does not match the format {pattern}.")
     ids = m.groupdict()
     return {k: int(v) if v.isdigit() else v for k, v in ids.items()}
 
 
 class OptaLoader(EventDataLoader):
-    """Load Opta data from a local folder.
+    """Load Opta data feeds from a local folder.
 
     Parameters
     ----------
     root : str
         Root-path of the data.
     parser : str or dict
-        Either 'xml', 'json', 'statsperform', 'whoscored' or your custom
-        parser for each feed. The default xml parser supports F7 and F24
-        feeds; the default json parser supports F1, F9 and F24 feeds, the StatsPerform
-        parser supports MA1 and MA3 feeds. Custom parsers can be specified
-        as::
+        Either 'xml', 'json', 'statsperform', 'whoscored' or a dict with
+        a custom parser for each feed. The default xml parser supports F7 and
+        F24 feeds; the default json parser supports F1, F9 and F24 feeds, the
+        StatsPerform parser supports MA1 and MA3 feeds. Custom parsers can be
+        specified as::
 
             {
                 'feed1_name': Feed1Parser
                 'feed2_name': Feed2Parser
             }
 
         where Feed1Parser and Feed2Parser are classes implementing
         :class:`~socceraction.spadl.opta.OptaParser` and 'feed1_name' and
-        'feed2_name' correspond to the keys in 'feeds'.
+        'feed2_name' are a unique ID for each feed that matches to the keys in
+        `feeds`.
     feeds : dict
-        Glob pattern for each feed that should be parsed. For example, if
-        files are named::
+        Glob pattern describing from which files the data from a specific game
+        can be retrieved. For example, if files are named::
 
             f7-1-2021-17362.xml
             f24-1-2021-17362.xml
 
         use::
 
             feeds = {
                 'f7': "f7-{competition_id}-{season_id}-{game_id}.xml",
                 'f24': "f24-{competition_id}-{season_id}-{game_id}.xml"
             }
 
-        If you use JSON files obtained from `WhoScored <whoscored.com>`__ use::
-
-            feeds = {
-                'whoscored': "{competition_id}-{season_id}/{game_id}.json",
-            }
-
     Raises
     ------
     ValueError
         If an invalid parser is provided.
     """
 
     def __init__(  # noqa: C901
@@ -286,15 +282,15 @@
             self.parsers = self._get_parsers_for_feeds(_whoscoredparsers, feeds)
         elif isinstance(parser, dict):
             if feeds is None:
                 raise ValueError("You must specify a feed for each parser.")
             self.parsers = self._get_parsers_for_feeds(parser, feeds)
         else:
             raise ValueError("Invalid parser provided.")
-        self.feeds = feeds
+        self.feeds = {k: str(Path(v)) for k, v in feeds.items()}
 
     def _get_parsers_for_feeds(
         self, available_parsers: Mapping[str, Type[OptaParser]], feeds: Dict[str, str]
     ) -> Mapping[str, Type[OptaParser]]:
         """Select the appropriate parser for each feed.
 
         Parameters
```

### Comparing `socceraction-1.4.0/socceraction/data/opta/parsers/__init__.py` & `socceraction-1.4.1/socceraction/data/opta/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/data/opta/parsers/base.py` & `socceraction-1.4.1/socceraction/data/opta/parsers/base.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/data/opta/parsers/f1_json.py` & `socceraction-1.4.1/socceraction/data/opta/parsers/f1_json.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/data/opta/parsers/f24_json.py` & `socceraction-1.4.1/socceraction/data/opta/parsers/f24_json.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/data/opta/parsers/f24_xml.py` & `socceraction-1.4.1/socceraction/data/opta/parsers/f24_xml.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/data/opta/parsers/f7_xml.py` & `socceraction-1.4.1/socceraction/data/opta/parsers/f7_xml.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/data/opta/parsers/f9_json.py` & `socceraction-1.4.1/socceraction/data/opta/parsers/f9_json.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/data/opta/parsers/ma1_json.py` & `socceraction-1.4.1/socceraction/data/opta/parsers/ma1_json.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/data/opta/parsers/ma3_json.py` & `socceraction-1.4.1/socceraction/data/opta/parsers/ma3_json.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/data/opta/parsers/whoscored.py` & `socceraction-1.4.1/socceraction/data/opta/parsers/whoscored.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/data/opta/schema.py` & `socceraction-1.4.1/socceraction/data/opta/schema.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/data/schema.py` & `socceraction-1.4.1/socceraction/data/schema.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/data/statsbomb/loader.py` & `socceraction-1.4.1/socceraction/data/statsbomb/loader.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/data/statsbomb/schema.py` & `socceraction-1.4.1/socceraction/data/statsbomb/schema.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/data/wyscout/loader.py` & `socceraction-1.4.1/socceraction/data/wyscout/loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -298,19 +298,23 @@
             df_players_match[c] = df_players_match[c].apply(
                 lambda x: x.encode().decode("unicode-escape")
             )
         df_players_match = _convert_players(df_players_match)
 
         # get minutes played
         competition_id, season_id = self._match_index.loc[game_id, ["competition_id", "season_id"]]
-        path_events = os.path.join(
-            self.root, self._index.at[(competition_id, season_id), "db_events"]
-        )
-        events = cast(List[Dict[str, Any]], self.get(path_events))
-        match_events = [e for e in events if e["matchId"] == game_id]
+        path = os.path.join(self.root, self._index.at[(competition_id, season_id), "db_events"])
+        if self._cache is not None and self._cache["path"] == path:
+            df_events = self._cache["events"]
+        else:
+            df_events = pd.DataFrame(self.get(path)).set_index("matchId")
+            # avoid that this large json file has to be parsed again for
+            # each game when loading a batch of games from the same season
+            self._cache = {"path": path, "events": df_events}
+        match_events = df_events.loc[game_id].reset_index().to_dict("records")
         mp = _get_minutes_played(lineups, match_events)
         df_players_match = pd.merge(df_players_match, mp, on="player_id", how="right")
         df_players_match["minutes_played"] = df_players_match.minutes_played.fillna(0)
         df_players_match["game_id"] = game_id
         return cast(DataFrame[WyscoutPlayerSchema], df_players_match)
 
     def events(self, game_id: int) -> DataFrame[WyscoutEventSchema]:
```

### Comparing `socceraction-1.4.0/socceraction/data/wyscout/schema.py` & `socceraction-1.4.1/socceraction/data/wyscout/schema.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/spadl/base.py` & `socceraction-1.4.1/socceraction/spadl/base.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/spadl/config.py` & `socceraction-1.4.1/socceraction/spadl/config.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/spadl/opta.py` & `socceraction-1.4.1/socceraction/spadl/opta.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/spadl/schema.py` & `socceraction-1.4.1/socceraction/spadl/schema.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/spadl/statsbomb.py` & `socceraction-1.4.1/socceraction/spadl/statsbomb.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/spadl/utils.py` & `socceraction-1.4.1/socceraction/spadl/utils.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/spadl/wyscout.py` & `socceraction-1.4.1/socceraction/spadl/wyscout.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/vaep/base.py` & `socceraction-1.4.1/socceraction/vaep/base.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/vaep/features.py` & `socceraction-1.4.1/socceraction/vaep/features.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/vaep/formula.py` & `socceraction-1.4.1/socceraction/vaep/formula.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/vaep/labels.py` & `socceraction-1.4.1/socceraction/vaep/labels.py`

 * *Files identical despite different names*

### Comparing `socceraction-1.4.0/socceraction/xthreat.py` & `socceraction-1.4.1/socceraction/xthreat.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 
 def _get_cell_indexes(
     x: Series[float], y: Series[float], l: int = N, w: int = M
 ) -> Tuple[Series[int], Series[int]]:
     xi = x.divide(spadlconfig.field_length).multiply(l)
     yj = y.divide(spadlconfig.field_width).multiply(w)
-    xi = xi.astype('int64').clip(0, l - 1)
-    yj = yj.astype('int64').clip(0, w - 1)
+    xi = xi.astype("int64").clip(0, l - 1)
+    yj = yj.astype("int64").clip(0, w - 1)
     return xi, yj
 
 
 def _get_flat_indexes(x: Series[float], y: Series[float], l: int = N, w: int = M) -> Series[int]:
     xi, yj = _get_cell_indexes(x, y, l, w)
     return yj.rsub(w - 1).mul(l).add(xi)
 
@@ -63,15 +63,15 @@
     vc = flat_indexes.value_counts(sort=False)
     vector = np.zeros(w * l, dtype=int)
     vector[vc.index] = vc
     return vector.reshape((w, l))
 
 
 def _safe_divide(a: npt.ArrayLike, b: npt.ArrayLike) -> npt.NDArray[np.float64]:
-    return np.divide(a, b, out=np.zeros_like(a), where=b != 0, casting='unsafe')
+    return np.divide(a, b, out=np.zeros_like(a, dtype="float64"), where=b != 0, casting="unsafe")
 
 
 def scoring_prob(
     actions: DataFrame[SPADLSchema], l: int = N, w: int = M
 ) -> npt.NDArray[np.float64]:
     """Compute the probability of scoring when taking a shot for each cell.
 
@@ -85,16 +85,16 @@
         Amount of grid cells in the y-dimension of the grid.
 
     Returns
     -------
     np.ndarray
         A matrix, denoting the probability of scoring for each cell.
     """
-    shot_actions = actions[(actions.type_id == spadlconfig.actiontypes.index('shot'))]
-    goals = shot_actions[(shot_actions.result_id == spadlconfig.results.index('success'))]
+    shot_actions = actions[(actions.type_id == spadlconfig.actiontypes.index("shot"))]
+    goals = shot_actions[(shot_actions.result_id == spadlconfig.results.index("success"))]
 
     shotmatrix = _count(shot_actions.start_x, shot_actions.start_y, l, w)
     goalmatrix = _count(goals.start_x, goals.start_y, l, w)
     return _safe_divide(goalmatrix, shotmatrix)
 
 
 def get_move_actions(actions: DataFrame[SPADLSchema]) -> DataFrame[SPADLSchema]:
@@ -111,17 +111,17 @@
 
     Returns
     -------
     pd.DataFrame
         All ball-progressing actions in the input dataframe.
     """
     return actions[
-        (actions.type_id == spadlconfig.actiontypes.index('pass'))
-        | (actions.type_id == spadlconfig.actiontypes.index('dribble'))
-        | (actions.type_id == spadlconfig.actiontypes.index('cross'))
+        (actions.type_id == spadlconfig.actiontypes.index("pass"))
+        | (actions.type_id == spadlconfig.actiontypes.index("dribble"))
+        | (actions.type_id == spadlconfig.actiontypes.index("cross"))
     ]
 
 
 def get_successful_move_actions(actions: DataFrame[SPADLSchema]) -> DataFrame[SPADLSchema]:
     """Get all successful ball-progressing actions.
 
     These include successful passes, dribbles and crosses.
@@ -133,15 +133,15 @@
 
     Returns
     -------
     pd.DataFrame
         All ball-progressing actions in the input dataframe.
     """
     move_actions = get_move_actions(actions)
-    return move_actions[(move_actions.result_id == spadlconfig.results.index('success'))]
+    return move_actions[(move_actions.result_id == spadlconfig.results.index("success"))]
 
 
 def action_prob(
     actions: DataFrame[SPADLSchema], l: int = N, w: int = M
 ) -> Tuple[npt.NDArray[np.float64], npt.NDArray[np.float64]]:
     """Compute the probability of taking an action in each cell of the grid.
 
@@ -160,15 +160,15 @@
     -------
     shotmatrix : np.ndarray
         For each cell the probability of choosing to shoot.
     movematrix : np.ndarray
         For each cell the probability of choosing to move.
     """
     move_actions = get_move_actions(actions)
-    shot_actions = actions[(actions.type_id == spadlconfig.actiontypes.index('shot'))]
+    shot_actions = actions[(actions.type_id == spadlconfig.actiontypes.index("shot"))]
 
     movematrix = _count(move_actions.start_x, move_actions.start_y, l, w)
     shotmatrix = _count(shot_actions.start_x, shot_actions.start_y, l, w)
     totalmatrix = movematrix + shotmatrix
 
     return _safe_divide(shotmatrix, totalmatrix), _safe_divide(movematrix, totalmatrix)
 
@@ -194,27 +194,27 @@
     -------
     np.ndarray
         The transition matrix.
     """
     move_actions = get_move_actions(actions)
 
     X = pd.DataFrame()
-    X['start_cell'] = _get_flat_indexes(move_actions.start_x, move_actions.start_y, l, w)
-    X['end_cell'] = _get_flat_indexes(move_actions.end_x, move_actions.end_y, l, w)
-    X['result_id'] = move_actions.result_id
+    X["start_cell"] = _get_flat_indexes(move_actions.start_x, move_actions.start_y, l, w)
+    X["end_cell"] = _get_flat_indexes(move_actions.end_x, move_actions.end_y, l, w)
+    X["result_id"] = move_actions.result_id
 
     vc = X.start_cell.value_counts(sort=False)
     start_counts = np.zeros(w * l)
     start_counts[vc.index] = vc
 
     transition_matrix = np.zeros((w * l, w * l))
 
     for i in range(0, w * l):
         vc2 = X[
-            ((X.start_cell == i) & (X.result_id == spadlconfig.results.index('success')))
+            ((X.start_cell == i) & (X.result_id == spadlconfig.results.index("success")))
         ].end_cell.value_counts(sort=False)
         transition_matrix[i, vc2.index] = vc2 / start_counts[i]
 
     return transition_matrix
 
 
 class ExpectedThreat:
@@ -312,17 +312,17 @@
 
             newxT = gs + (p_move * total_payoff)
             diff = newxT - self.xT
             self.xT = newxT
             self.heatmaps.append(self.xT.copy())
             it += 1
 
-        print('# iterations: ', it)
+        print("# iterations: ", it)
 
-    def fit(self, actions: DataFrame[SPADLSchema]) -> 'ExpectedThreat':
+    def fit(self, actions: DataFrame[SPADLSchema]) -> "ExpectedThreat":
         """Fits the xT model with the given actions.
 
         Parameters
         ----------
         actions : pd.DataFrame
             Actions, in SPADL format.
 
@@ -340,15 +340,15 @@
             self.shot_prob_matrix,
             self.move_prob_matrix,
             self.transition_matrix,
         )
         return self
 
     def interpolator(
-        self, kind: str = 'linear'
+        self, kind: str = "linear"
     ) -> Callable[[npt.NDArray[np.float64], npt.NDArray[np.float64]], npt.NDArray[np.float64]]:
         """Interpolate over the pitch.
 
         This is a wrapper around :func:`scipy.interpolate.interp2d`.
 
         Parameters
         ----------
@@ -362,15 +362,15 @@
 
         Returns
         -------
         callable
             A function that interpolates xT values over the pitch.
         """
         if interp2d is None:
-            raise ImportError('Interpolation requires scipy to be installed.')
+            raise ImportError("Interpolation requires scipy to be installed.")
 
         cell_length = spadlconfig.field_length / self.l
         cell_width = spadlconfig.field_width / self.w
 
         x = np.arange(0.0, spadlconfig.field_length, cell_length) + 0.5 * cell_length
         y = np.arange(0.0, spadlconfig.field_width, cell_width) + 0.5 * cell_width
 
@@ -465,17 +465,17 @@
         if not np.any(self.xT):
             raise NotFittedError()
 
         # If file exists and should not be overwritten:
         if not overwrite and os.path.isfile(filepath):
             raise ValueError(
                 'save_xt got overwrite="False", but a file '
-                f'({filepath}) exists already. No data was saved.'
+                f"({filepath}) exists already. No data was saved."
             )
-        with open(filepath, 'w') as f:
+        with open(filepath, "w") as f:
             json.dump(self.xT.tolist(), f)
 
 
 def load_model(path: str) -> ExpectedThreat:
     """Create a model from a pre-computed xT value surface.
 
     The value surface should be provided as a JSON file containing a 2D
```

### Comparing `socceraction-1.4.0/setup.py` & `socceraction-1.4.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,97 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: socceraction
+Version: 1.4.1
+Summary: Convert soccer event stream data to the SPADL format and value on-the-ball player actions
+Home-page: https://github.com/ML-KULeuven/socceraction
+License: MIT
+Keywords: soccer,football,sports analytics
+Author: Tom Decroos
+Author-email: tom.decroos.be@gmail.com
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Provides-Extra: statsbomb
+Requires-Dist: lxml (>=4.6.3,<5.0.0)
+Requires-Dist: numpy (>=1.21.2,<2.0.0)
+Requires-Dist: pandas (>=1.3.3,<2.0.0)
+Requires-Dist: pandera (>=0.13.4,<0.14.0)
+Requires-Dist: requests-cache (>=0.9.1,<0.10.0) ; extra == "statsbomb"
+Requires-Dist: scikit-learn (>=1.2.1,<2.0.0)
+Requires-Dist: statsbombpy (>=1.3.0,<2.0.0) ; extra == "statsbomb"
+Project-URL: Documentation, https://socceraction.readthedocs.io
+Project-URL: Repository, https://github.com/ML-KULeuven/socceraction
+Description-Content-Type: text/markdown
+
+<div align="center">
+	<img src="https://socceraction.readthedocs.io/en/latest/_static/logo_white.png" height="200">
+	<p>
+	<b>Convert soccer event stream data to the SPADL format<br/>and value on-the-ball player actions</b>
+	</p>
+	<br/>
+
+[![PyPi](https://img.shields.io/pypi/v/socceraction.svg)](https://pypi.org/project/socceraction)
+[![Python Version: 3.7.1+](https://img.shields.io/badge/Python-3.7.1+-blue.svg)](https://pypi.org/project/socceraction)
+[![Downloads](https://img.shields.io/pypi/dm/socceraction.svg)](https://pypistats.org/packages/socceraction)
+[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://en.wikipedia.org/wiki/MIT_License)
+
+[![Build Status](https://github.com/ML-KULeuven/socceraction/workflows/CI/badge.svg)](https://github.com/ML-KULeuven/socceraction/actions?workflow=CI)
+[![Read the Docs](https://img.shields.io/readthedocs/socceraction/latest.svg?label=Read%20the%20Docs)](https://socceraction.readthedocs.io)
+[![Code coverage](https://codecov.io/gh/ML-KULeuven/socceraction/branch/master/graph/badge.svg)](https://codecov.io/gh/ML-KULeuven/socceraction)
+
+<br/>
+<br/>
+</div>
+
+Socceraction is a Python package for objectively quantifying the impact of the individual actions performed by soccer players using event stream data. The general idea is to assign a value to each on-the-ball action based on the action's impact on the game outcome, while accounting for the context in which the action happened. The video below gives a quick two-minute introduction to action values.
+
+<div align="center">
+
+https://user-images.githubusercontent.com/2175271/136857714-1d2c8706-7f2f-449d-818f-0e67fbb75400.mp4
+
+</div>
+
+## Features
+
+Socceraction contains the following components:
+
+- A set of API clients for **loading event stream data** from StatsBomb, Opta, Wyscout, Stats Perform and WhoScored as Pandas DataFrames using a unified data model. [Read more »](https://socceraction.readthedocs.io/en/latest/documentation/data/index.html)
+- Converters for each of these provider's proprietary data format to the **SPADL** and **atomic-SPADL** formats, which are unified and expressive languages for on-the-ball player actions. [Read more »](https://socceraction.readthedocs.io/en/latest/documentation/spadl/index.html)
+- An implementation of the **Expected Threat (xT)** possession value framework. [Read more »](https://socceraction.readthedocs.io/en/latest/documentation/valuing_actions/xT.html)
+- An implementation of the **VAEP** and **Atomic-VAEP** possession value frameworks. [Read more »](https://socceraction.readthedocs.io/en/latest/documentation/valuing_actions/vaep.html)
+
+## Installation / Getting started
+
+The recommended way to install `socceraction` is to simply use pip. The latest version officially supports Python 3.8 - 3.11.
+
+```sh
+$ pip install socceraction
+```
+
+The folder [`public-notebooks`](https://github.com/ML-KULeuven/socceraction/tree/master/public-notebooks) provides a demo of the full pipeline from raw StatsBomb event stream data to action values and player ratings. More detailed installation/usage instructions can be found in the [Documentation](https://socceraction.readthedocs.io/en/latest/).
+
+## Contributing
+
+All contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome. However, be aware that socceraction is not actively developed. It's primary use is to enable reproducibility of our research. If you believe there is a feature missing, feel free to raise a feature request, but please do be aware that the overwhelming likelihood is that your feature request will not be accepted.
+To learn more on how to contribute, see the [Contributor Guide](https://socceraction.readthedocs.io/en/latest/development/developer_guide.html).
+
+## Research
+
+If you make use of this package in your research, please consider citing the following papers:
+
+- Tom Decroos, Lotte Bransen, Jan Van Haaren, and Jesse Davis. **Actions speak louder than goals: Valuing player actions in soccer.** In Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining, pp. 1851-1861. 2019. <br/>[ [pdf](http://doi.acm.org/10.1145/3292500.3330758) | [bibtex](https://github.com/ML-KULeuven/socceraction/blob/master/docs/_static/decroos19.bibtex) ]
 
-packages = \
-['socceraction',
- 'socceraction.atomic',
- 'socceraction.atomic.spadl',
- 'socceraction.atomic.vaep',
- 'socceraction.data',
- 'socceraction.data.opta',
- 'socceraction.data.opta.parsers',
- 'socceraction.data.statsbomb',
- 'socceraction.data.wyscout',
- 'socceraction.spadl',
- 'socceraction.vaep']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['lxml>=4.6.3,<5.0.0',
- 'numpy>=1.21.2,<2.0.0',
- 'pandas>=1.3.3,<2.0.0',
- 'pandera>=0.13.4,<0.14.0',
- 'scikit-learn>=1.2.1,<2.0.0']
-
-extras_require = \
-{'statsbomb': ['statsbombpy>=1.3.0,<2.0.0', 'requests-cache>=0.9.1,<0.10.0']}
-
-setup_kwargs = {
-    'name': 'socceraction',
-    'version': '1.4.0',
-    'description': 'Convert soccer event stream data to the SPADL format and value on-the-ball player actions',
-    'long_description': '<div align="center">\n\t<img src="https://socceraction.readthedocs.io/en/latest/_static/logo_white.png" height="200">\n\t<p>\n\t<b>Convert soccer event stream data to the SPADL format<br/>and value on-the-ball player actions</b>\n\t</p>\n\t<br/>\n\n[![PyPi](https://img.shields.io/pypi/v/socceraction.svg)](https://pypi.org/project/socceraction)\n[![Python Version: 3.7.1+](https://img.shields.io/badge/Python-3.7.1+-blue.svg)](https://pypi.org/project/socceraction)\n[![Downloads](https://img.shields.io/pypi/dm/socceraction.svg)](https://pypistats.org/packages/socceraction)\n[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://en.wikipedia.org/wiki/MIT_License)\n\n[![Build Status](https://github.com/ML-KULeuven/socceraction/workflows/CI/badge.svg)](https://github.com/ML-KULeuven/socceraction/actions?workflow=CI)\n[![Read the Docs](https://img.shields.io/readthedocs/socceraction/latest.svg?label=Read%20the%20Docs)](https://socceraction.readthedocs.io)\n[![Code coverage](https://codecov.io/gh/ML-KULeuven/socceraction/branch/master/graph/badge.svg)](https://codecov.io/gh/ML-KULeuven/socceraction)\n\n<br/>\n<br/>\n</div>\n\nSocceraction is a Python package for objectively quantifying the impact of the individual actions performed by soccer players using event stream data. The general idea is to assign a value to each on-the-ball action based on the action\'s impact on the game outcome, while accounting for the context in which the action happened. The video below gives a quick two-minute introduction to action values.\n\n<div align="center">\n\nhttps://user-images.githubusercontent.com/2175271/136857714-1d2c8706-7f2f-449d-818f-0e67fbb75400.mp4\n\n</div>\n\n## Features\n\nSocceraction contains the following components:\n\n- A set of API clients for **loading event stream data** from StatsBomb, Opta, Wyscout, Stats Perform and WhoScored as Pandas DataFrames using a unified data model. [Read more »](https://socceraction.readthedocs.io/en/latest/documentation/data/index.html)\n- Converters for each of these provider\'s proprietary data format to the **SPADL** and **atomic-SPADL** formats, which are unified and expressive languages for on-the-ball player actions. [Read more »](https://socceraction.readthedocs.io/en/latest/documentation/spadl/index.html)\n- An implementation of the **Expected Threat (xT)** possession value framework. [Read more »](https://socceraction.readthedocs.io/en/latest/documentation/valuing_actions/xT.html)\n- An implementation of the **VAEP** and **Atomic-VAEP** possession value frameworks. [Read more »](https://socceraction.readthedocs.io/en/latest/documentation/valuing_actions/vaep.html)\n\n## Installation / Getting started\n\nThe recommended way to install `socceraction` is to simply use pip. The latest version officially supports Python 3.8 - 3.11.\n\n```sh\n$ pip install socceraction\n```\n\nThe folder [`public-notebooks`](https://github.com/ML-KULeuven/socceraction/tree/master/public-notebooks) provides a demo of the full pipeline from raw StatsBomb event stream data to action values and player ratings. More detailed installation/usage instructions can be found in the [Documentation](https://socceraction.readthedocs.io/en/latest/).\n\n## Contributing\n\nAll contributions, bug reports, bug fixes, documentation improvements, enhancements, and ideas are welcome. However, be aware that socceraction is not actively developed. It\'s primary use is to enable reproducibility of our research. If you believe there is a feature missing, feel free to raise a feature request, but please do be aware that the overwhelming likelihood is that your feature request will not be accepted.\nTo learn more on how to contribute, see the [Contributor Guide](https://socceraction.readthedocs.io/en/latest/development/developer_guide.html).\n\n## Research\n\nIf you make use of this package in your research, please consider citing the following papers:\n\n- Tom Decroos, Lotte Bransen, Jan Van Haaren, and Jesse Davis. **Actions speak louder than goals: Valuing player actions in soccer.** In Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining, pp. 1851-1861. 2019. <br/>[ [pdf](http://doi.acm.org/10.1145/3292500.3330758) | [bibtex](https://github.com/ML-KULeuven/socceraction/blob/master/docs/_static/decroos19.bibtex) ]\n\n- Maaike Van Roy, Pieter Robberechts, Tom Decroos, and Jesse Davis. **Valuing on-the-ball actions in soccer: a critical comparison of XT and VAEP.** In Proceedings of the AAAI-20 Workshop on Artifical Intelligence in Team Sports. AI in Team Sports Organising Committee, 2020. <br/>[ [pdf](https://limo.libis.be/primo-explore/fulldisplay?docid=LIRIAS2913207&context=L&vid=KULeuven&search_scope=ALL_CONTENT&tab=all_content_tab&lang=en_US) | [bibtex](https://github.com/ML-KULeuven/socceraction/blob/master/docs/_static/vanroy20.bibtex) ]\n\nThe Expected Threat (xT) framework was originally introduced by Karun Singh on his [blog](https://karun.in/blog/expected-threat.html) in 2019.\n\n## License\n\nDistributed under the terms of the [MIT license](https://opensource.org/licenses/MIT),\nsocceraction is free and open source software. Although not strictly required, we appreciate it if you include a link to this repo or cite our research in your work if you make use of socceraction.\n',
-    'author': 'Tom Decroos',
-    'author_email': 'tom.decroos.be@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/ML-KULeuven/socceraction',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
+- Maaike Van Roy, Pieter Robberechts, Tom Decroos, and Jesse Davis. **Valuing on-the-ball actions in soccer: a critical comparison of XT and VAEP.** In Proceedings of the AAAI-20 Workshop on Artifical Intelligence in Team Sports. AI in Team Sports Organising Committee, 2020. <br/>[ [pdf](https://limo.libis.be/primo-explore/fulldisplay?docid=LIRIAS2913207&context=L&vid=KULeuven&search_scope=ALL_CONTENT&tab=all_content_tab&lang=en_US) | [bibtex](https://github.com/ML-KULeuven/socceraction/blob/master/docs/_static/vanroy20.bibtex) ]
 
+The Expected Threat (xT) framework was originally introduced by Karun Singh on his [blog](https://karun.in/blog/expected-threat.html) in 2019.
+
+## License
+
+Distributed under the terms of the [MIT license](https://opensource.org/licenses/MIT),
+socceraction is free and open source software. Although not strictly required, we appreciate it if you include a link to this repo or cite our research in your work if you make use of socceraction.
 
-setup(**setup_kwargs)
```

