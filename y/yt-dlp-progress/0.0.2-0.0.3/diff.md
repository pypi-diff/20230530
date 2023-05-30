# Comparing `tmp/yt_dlp_progress-0.0.2.tar.gz` & `tmp/yt_dlp_progress-0.0.3.tar.gz`

## Comparing `yt_dlp_progress-0.0.2.tar` & `yt_dlp_progress-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     2672 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.2/yt_dlp_progress/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.2/.gitignore
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.2/README.md
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.3/yt_dlp_progress/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.3/LICENSE
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.3/README.md
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.3/PKG-INFO
```

### Comparing `yt_dlp_progress-0.0.2/yt_dlp_progress/__init__.py` & `yt_dlp_progress-0.0.3/yt_dlp_progress/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import sys
 from typing import Any, Dict
 from unittest import mock
 
 import yt_dlp
 from yt_dlp import utils as ydl_utils
 
+__version__ = "0.0.3"
+
 original_parse_options = yt_dlp.parse_options
 original_popen = ydl_utils.Popen
 
 YDL_OPTIONS: Dict[str, Any] = {
     "buffersize": 16 * 1024,
     "retries": 5,
     "fragment_retries": 5,
```

