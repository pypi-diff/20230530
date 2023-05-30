# Comparing `tmp/ffmpeg-progress-yield-0.7.4.tar.gz` & `tmp/ffmpeg-progress-yield-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpeg-progress-yield-0.7.4.tar", last modified: Sat May  6 09:37:16 2023, max compression
+gzip compressed data, was "ffmpeg-progress-yield-0.7.5.tar", last modified: Tue May 30 07:04:20 2023, max compression
```

## Comparing `ffmpeg-progress-yield-0.7.4.tar` & `ffmpeg-progress-yield-0.7.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-06 09:37:16.416104 ffmpeg-progress-yield-0.7.4/
--rw-r--r--   0 werner     (501) staff       (20)     2301 2023-05-06 09:37:15.000000 ffmpeg-progress-yield-0.7.4/CHANGELOG.md
--rw-r--r--   0 werner     (501) staff       (20)     1086 2023-05-05 06:38:37.000000 ffmpeg-progress-yield-0.7.4/LICENSE
--rw-r--r--   0 werner     (501) staff       (20)     9850 2023-05-06 09:37:16.416243 ffmpeg-progress-yield-0.7.4/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)     6773 2023-05-05 06:38:38.000000 ffmpeg-progress-yield-0.7.4/README.md
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-06 09:37:16.413665 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield/
--rw-r--r--   0 werner     (501) staff       (20)      103 2023-05-06 09:37:14.000000 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield/__init__.py
--rw-r--r--   0 werner     (501) staff       (20)     1279 2023-03-04 16:13:54.000000 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield/__main__.py
--rw-r--r--   0 werner     (501) staff       (20)     7206 2023-05-06 09:36:51.000000 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield/ffmpeg_progress_yield.py
--rw-r--r--   0 werner     (501) staff       (20)        0 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield/py.typed
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-06 09:37:16.415040 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield.egg-info/
--rw-r--r--   0 werner     (501) staff       (20)     9850 2023-05-06 09:37:16.000000 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield.egg-info/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)      494 2023-05-06 09:37:16.000000 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield.egg-info/SOURCES.txt
--rw-r--r--   0 werner     (501) staff       (20)        1 2023-05-06 09:37:16.000000 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield.egg-info/dependency_links.txt
--rw-r--r--   0 werner     (501) staff       (20)       78 2023-05-06 09:37:16.000000 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield.egg-info/entry_points.txt
--rw-r--r--   0 werner     (501) staff       (20)        1 2021-03-01 12:51:44.000000 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield.egg-info/not-zip-safe
--rw-r--r--   0 werner     (501) staff       (20)       22 2023-05-06 09:37:16.000000 ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield.egg-info/top_level.txt
--rw-r--r--   0 werner     (501) staff       (20)      279 2023-05-06 09:37:16.416642 ffmpeg-progress-yield-0.7.4/setup.cfg
--rw-r--r--   0 werner     (501) staff       (20)     1748 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.4/setup.py
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-06 09:37:16.415940 ffmpeg-progress-yield-0.7.4/test/
--rw-r--r--   0 werner     (501) staff       (20)    37351 2022-12-11 11:53:49.000000 ffmpeg-progress-yield-0.7.4/test/test.mp4
--rw-r--r--   0 werner     (501) staff       (20)     4235 2023-05-05 06:37:46.000000 ffmpeg-progress-yield-0.7.4/test/test.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 07:04:20.511596 ffmpeg-progress-yield-0.7.5/
+-rw-r--r--   0 werner     (501) staff       (20)     2404 2023-05-30 07:04:19.000000 ffmpeg-progress-yield-0.7.5/CHANGELOG.md
+-rw-r--r--   0 werner     (501) staff       (20)     1086 2023-05-05 06:38:37.000000 ffmpeg-progress-yield-0.7.5/LICENSE
+-rw-r--r--   0 werner     (501) staff       (20)     9953 2023-05-30 07:04:20.511740 ffmpeg-progress-yield-0.7.5/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)     6773 2023-05-05 06:38:38.000000 ffmpeg-progress-yield-0.7.5/README.md
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 07:04:20.509184 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield/
+-rw-r--r--   0 werner     (501) staff       (20)      103 2023-05-30 07:04:18.000000 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield/__init__.py
+-rw-r--r--   0 werner     (501) staff       (20)     1283 2023-05-30 06:56:19.000000 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield/__main__.py
+-rw-r--r--   0 werner     (501) staff       (20)     7841 2023-05-30 07:03:47.000000 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield/ffmpeg_progress_yield.py
+-rw-r--r--   0 werner     (501) staff       (20)        0 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield/py.typed
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 07:04:20.510296 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield.egg-info/
+-rw-r--r--   0 werner     (501) staff       (20)     9953 2023-05-30 07:04:20.000000 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield.egg-info/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)      494 2023-05-30 07:04:20.000000 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield.egg-info/SOURCES.txt
+-rw-r--r--   0 werner     (501) staff       (20)        1 2023-05-30 07:04:20.000000 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield.egg-info/dependency_links.txt
+-rw-r--r--   0 werner     (501) staff       (20)       78 2023-05-30 07:04:20.000000 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield.egg-info/entry_points.txt
+-rw-r--r--   0 werner     (501) staff       (20)        1 2021-03-01 12:51:44.000000 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield.egg-info/not-zip-safe
+-rw-r--r--   0 werner     (501) staff       (20)       22 2023-05-30 07:04:20.000000 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield.egg-info/top_level.txt
+-rw-r--r--   0 werner     (501) staff       (20)      279 2023-05-30 07:04:20.512089 ffmpeg-progress-yield-0.7.5/setup.cfg
+-rw-r--r--   0 werner     (501) staff       (20)     1748 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.5/setup.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 07:04:20.511311 ffmpeg-progress-yield-0.7.5/test/
+-rw-r--r--   0 werner     (501) staff       (20)    37351 2022-12-11 11:53:49.000000 ffmpeg-progress-yield-0.7.5/test/test.mp4
+-rw-r--r--   0 werner     (501) staff       (20)     4235 2023-05-30 07:03:53.000000 ffmpeg-progress-yield-0.7.5/test/test.py
```

### Comparing `ffmpeg-progress-yield-0.7.4/CHANGELOG.md` & `ffmpeg-progress-yield-0.7.5/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 # Changelog
 
 
+## v0.7.5 (2023-05-30)
+
+* Fix duration for multiple inputs, fixes #13.
+
+* Fix 'Test' string in tqdm.
+
+
 ## v0.7.4 (2023-05-06)
 
 * Fix: round percentage numbers.
 
 
 ## v0.7.3 (2023-05-05)
```

### Comparing `ffmpeg-progress-yield-0.7.4/LICENSE` & `ffmpeg-progress-yield-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.4/PKG-INFO` & `ffmpeg-progress-yield-0.7.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg-progress-yield
-Version: 0.7.4
+Version: 0.7.5
 Summary: Run an ffmpeg command with progress
 Home-page: https://github.com/slhck/ffmpeg-progress-yield
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Keywords: ffmpeg
 Classifier: Development Status :: 4 - Beta
@@ -189,14 +189,21 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 
 # Changelog
 
 
+## v0.7.5 (2023-05-30)
+
+* Fix duration for multiple inputs, fixes #13.
+
+* Fix 'Test' string in tqdm.
+
+
 ## v0.7.4 (2023-05-06)
 
 * Fix: round percentage numbers.
 
 
 ## v0.7.3 (2023-05-05)
```

### Comparing `ffmpeg-progress-yield-0.7.4/README.md` & `ffmpeg-progress-yield-0.7.5/README.md`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield/__main__.py` & `ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     args = parser.parse_args()
 
     ff = FfmpegProgress(args.ffmpeg_command, dry_run=args.dry_run)
 
     try:
         from tqdm import tqdm
 
-        with tqdm(total=100, position=1, desc="Test") as pbar:
+        with tqdm(total=100, position=1, desc="Progress") as pbar:
             for progress in ff.run_command_with_progress(
                 duration_override=args.duration
             ):
                 pbar.update(progress - pbar.n)
     except ImportError:
         for progress in ff.run_command_with_progress():
             print(f"{progress}/100")
```

### Comparing `ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield/ffmpeg_progress_yield.py` & `ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield/ffmpeg_progress_yield.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os
 import re
 import subprocess
 from typing import Any, Callable, Iterator, List, Optional, Union
 
 
 def to_ms(**kwargs: Union[float, int, str]) -> int:
     hour = int(kwargs.get("hour", 0))
@@ -19,45 +20,50 @@
 
     Args:
         cmd (List[str]): A list of command line elements, e.g. ["ffmpeg", "-i", ...]
 
     Returns:
         Optional[int]: The duration in milliseconds.
     """
+    file_names = []
+    for i, arg in enumerate(cmd):
+        if arg == "-i":
+            file_name = cmd[i + 1]
+
+            # filter for filenames that we can probe, i.e. regular files
+            if os.path.isfile(file_name):
+                file_names.append(file_name)
 
-    def _get_file_name(cmd: List[str]) -> Optional[str]:
+    if len(file_names) == 0:
+        return None
+
+    durations = []
+
+    for file_name in file_names:
         try:
-            idx = cmd.index("-i")
-            return cmd[idx + 1]
-        except ValueError:
+            output = subprocess.check_output(
+                [
+                    "ffprobe",
+                    "-loglevel",
+                    "error",
+                    "-hide_banner",
+                    "-show_entries",
+                    "format=duration",
+                    "-of",
+                    "default=noprint_wrappers=1:nokey=1",
+                    file_name,
+                ],
+                universal_newlines=True,
+            )
+            durations.append(int(float(output.strip()) * 1000))
+        except Exception:
+            # TODO: add logging
             return None
 
-    file_name = _get_file_name(cmd)
-    if file_name is None:
-        return None
-
-    try:
-        output = subprocess.check_output(
-            [
-                "ffprobe",
-                "-loglevel",
-                "error",
-                "-hide_banner",
-                "-show_entries",
-                "format=duration",
-                "-of",
-                "default=noprint_wrappers=1:nokey=1",
-                file_name,
-            ],
-            universal_newlines=True,
-        )
-        return int(float(output.strip()) * 1000)
-    except Exception:
-        # TODO: add logging
-        return None
+    return max(durations) if "-shortest" not in cmd else min(durations)
 
 
 def _uses_error_loglevel(cmd: List[str]) -> bool:
     try:
         idx = cmd.index("-loglevel")
         if cmd[idx + 1] == "error":
             return True
@@ -132,14 +138,17 @@
         if self.dry_run:
             return self.cmd
 
         total_dur: Union[None, int] = None
         if _uses_error_loglevel(self.cmd):
             total_dur = _probe_duration(self.cmd)
 
+        if duration_override is not None:
+            total_dur = int(duration_override * 1000)
+
         cmd_with_progress = (
             [self.cmd[0]] + ["-progress", "-", "-nostats"] + self.cmd[1:]
         )
 
         stderr = []
         base_popen_kwargs = self.base_popen_kwargs.copy()
         if popen_kwargs is not None:
@@ -166,29 +175,32 @@
             if stderr_line == "" and self.process.poll() is not None:
                 break
 
             stderr.append(stderr_line.strip())
 
             self.stderr = "\n".join(stderr)
 
-            if total_dur is None:
-                total_dur_match = self.DUR_REGEX.search(stderr_line)
-                if total_dur_match:
-                    total_dur = to_ms(**total_dur_match.groupdict())
-                    continue
-                elif duration_override is not None:
-                    # use the override (should apply in the first loop)
-                    total_dur = int(duration_override * 1000)
-                    continue
-
-            if total_dur:
-                progress_time = FfmpegProgress.TIME_REGEX.search(stderr_line)
-                if progress_time:
-                    elapsed_time = to_ms(**progress_time.groupdict())
-                    yield round(elapsed_time / total_dur * 100, 2)
+            # assign the total duration if it was found. this can happen multiple times for multiple inputs,
+            # in which case we have to determine the overall duration by taking the min/max (dependent on -shortest being present)
+            if total_dur_match := self.DUR_REGEX.search(stderr_line):
+                total_dur_ms = to_ms(**total_dur_match.groupdict())
+                if total_dur is not None:
+                    total_dur = (
+                        min(total_dur, total_dur_ms)
+                        if "-shortest" in self.cmd
+                        else max(total_dur, total_dur_ms)
+                    )
+                else:
+                    total_dur = total_dur_ms
+
+            if (
+                progress_time := FfmpegProgress.TIME_REGEX.search(stderr_line)
+            ) and total_dur is not None:
+                elapsed_time = to_ms(**progress_time.groupdict())
+                yield min(max(round(elapsed_time / total_dur * 100, 2), 0), 100)
 
         if self.process is None or self.process.returncode != 0:
             _pretty_stderr = "\n".join(stderr)
             raise RuntimeError(f"Error running command {self.cmd}: {_pretty_stderr}")
 
         yield 100
         self.process = None
```

### Comparing `ffmpeg-progress-yield-0.7.4/ffmpeg_progress_yield.egg-info/PKG-INFO` & `ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg-progress-yield
-Version: 0.7.4
+Version: 0.7.5
 Summary: Run an ffmpeg command with progress
 Home-page: https://github.com/slhck/ffmpeg-progress-yield
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Keywords: ffmpeg
 Classifier: Development Status :: 4 - Beta
@@ -189,14 +189,21 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 
 # Changelog
 
 
+## v0.7.5 (2023-05-30)
+
+* Fix duration for multiple inputs, fixes #13.
+
+* Fix 'Test' string in tqdm.
+
+
 ## v0.7.4 (2023-05-06)
 
 * Fix: round percentage numbers.
 
 
 ## v0.7.3 (2023-05-05)
```

### Comparing `ffmpeg-progress-yield-0.7.4/setup.py` & `ffmpeg-progress-yield-0.7.5/setup.py`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.4/test/test.mp4` & `ffmpeg-progress-yield-0.7.5/test/test.mp4`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.4/test/test.py` & `ffmpeg-progress-yield-0.7.5/test/test.py`

 * *Files identical despite different names*

