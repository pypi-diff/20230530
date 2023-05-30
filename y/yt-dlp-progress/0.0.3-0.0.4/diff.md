# Comparing `tmp/yt_dlp_progress-0.0.3.tar.gz` & `tmp/yt_dlp_progress-0.0.4.tar.gz`

## Comparing `yt_dlp_progress-0.0.3.tar` & `yt_dlp_progress-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     2695 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.3/yt_dlp_progress/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.3/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.3/LICENSE
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.3/README.md
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.4/yt_dlp_progress/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.4/LICENSE
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.4/README.md
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 yt_dlp_progress-0.0.4/PKG-INFO
```

### Comparing `yt_dlp_progress-0.0.3/yt_dlp_progress/__init__.py` & `yt_dlp_progress-0.0.4/yt_dlp_progress/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,41 +4,25 @@
 import sys
 from typing import Any, Dict
 from unittest import mock
 
 import yt_dlp
 from yt_dlp import utils as ydl_utils
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
 
 original_parse_options = yt_dlp.parse_options
-original_popen = ydl_utils.Popen
-
-YDL_OPTIONS: Dict[str, Any] = {
-    "buffersize": 16 * 1024,
-    "retries": 5,
-    "fragment_retries": 5,
-    "quiet": True,
-    "noprogress": True,
-    "no_color": True,
-    "call_home": False,
-    "ignoreerrors": False,
-    "geo_bypass": True,
-    "prefer_ffmpeg": True,
-    "noplaylist": True,
-}
 
 
 def get_logger() -> logging.Logger:
     logger = logging.getLogger("log")
     logger.setLevel(logging.DEBUG)
 
     if not logger.handlers:
         handler = logging.StreamHandler(sys.stdout)
-
         fmt = logging.Formatter("%(message)s")
         handler.setFormatter(fmt)
         handler.setLevel(logging.DEBUG)
 
         logger.addHandler(handler)
 
     return logger
@@ -52,43 +36,41 @@
         return super().run(*args, timeout=timeout, **kwargs)
 
 
 class YtDlpProgress:
     def __init__(self) -> None:
         self.logger = get_logger()
 
-        self.opts = copy.copy(YDL_OPTIONS)
-        self.opts.update(
-            {
-                "logger": self.logger,
-                "progress_hooks": [self._log_hook],
-                "postprocessor_args": ["-progress", "pipe:1"],
-            }
-        )
+        self.opts = {
+            "logger": self.logger,
+            "progress_hooks": [self._log_hook],
+            "noprogress": True,
+            "no_color": True,
+            "prefer_ffmpeg": True,
+            "postprocessor_args": ["-progress", "pipe:1"],
+        }
 
     def _log_hook(self, data: Dict[str, Any]) -> None:
         size_done = data.get("downloaded_bytes", None)
-        size_total = data.get("total_bytes", None)
+        size_total = data.get("total_bytes_estimate", None)
 
         report = {
             "finished": data.get("status") == "finished",
             "done": "unk",
         }
 
         if size_done is not None and size_total is not None:
-            report["downloaded"] = size_done
-            report["total"] = size_total
+            report["downloaded"] = int(size_done)
+            report["total"] = int(size_total)
             report["done"] = "%.2f%%" % (size_done * 100 / size_total)
 
         self.logger.info("progress %s", json.dumps(report))
 
     def _parse_options(self, argv=None):  # type: ignore
-        v = original_parse_options(argv=argv)
-        parser, opts, urls, ydl_opts = v
-        opts.update_self = False
+        parser, opts, urls, ydl_opts = original_parse_options(argv=argv)
         ydl_opts.update(self.opts)
         return parser, opts, urls, ydl_opts
 
     def execute(self) -> None:
         parse_options_mock = mock.patch("yt_dlp.parse_options", self._parse_options)
         popen_mock = mock.patch("yt_dlp.postprocessor.ffmpeg.Popen", Popen)
```

### Comparing `yt_dlp_progress-0.0.3/LICENSE` & `yt_dlp_progress-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yt_dlp_progress-0.0.3/pyproject.toml` & `yt_dlp_progress-0.0.4/pyproject.toml`

 * *Files identical despite different names*

