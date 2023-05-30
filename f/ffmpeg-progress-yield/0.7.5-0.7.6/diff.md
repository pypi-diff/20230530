# Comparing `tmp/ffmpeg-progress-yield-0.7.5.tar.gz` & `tmp/ffmpeg-progress-yield-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ffmpeg-progress-yield-0.7.5.tar", last modified: Tue May 30 07:04:20 2023, max compression
+gzip compressed data, was "ffmpeg-progress-yield-0.7.6.tar", last modified: Tue May 30 07:05:57 2023, max compression
```

## Comparing `ffmpeg-progress-yield-0.7.5.tar` & `ffmpeg-progress-yield-0.7.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 07:04:20.511596 ffmpeg-progress-yield-0.7.5/
--rw-r--r--   0 werner     (501) staff       (20)     2404 2023-05-30 07:04:19.000000 ffmpeg-progress-yield-0.7.5/CHANGELOG.md
--rw-r--r--   0 werner     (501) staff       (20)     1086 2023-05-05 06:38:37.000000 ffmpeg-progress-yield-0.7.5/LICENSE
--rw-r--r--   0 werner     (501) staff       (20)     9953 2023-05-30 07:04:20.511740 ffmpeg-progress-yield-0.7.5/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)     6773 2023-05-05 06:38:38.000000 ffmpeg-progress-yield-0.7.5/README.md
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 07:04:20.509184 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield/
--rw-r--r--   0 werner     (501) staff       (20)      103 2023-05-30 07:04:18.000000 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield/__init__.py
--rw-r--r--   0 werner     (501) staff       (20)     1283 2023-05-30 06:56:19.000000 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield/__main__.py
--rw-r--r--   0 werner     (501) staff       (20)     7841 2023-05-30 07:03:47.000000 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield/ffmpeg_progress_yield.py
--rw-r--r--   0 werner     (501) staff       (20)        0 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield/py.typed
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 07:04:20.510296 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield.egg-info/
--rw-r--r--   0 werner     (501) staff       (20)     9953 2023-05-30 07:04:20.000000 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield.egg-info/PKG-INFO
--rw-r--r--   0 werner     (501) staff       (20)      494 2023-05-30 07:04:20.000000 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield.egg-info/SOURCES.txt
--rw-r--r--   0 werner     (501) staff       (20)        1 2023-05-30 07:04:20.000000 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield.egg-info/dependency_links.txt
--rw-r--r--   0 werner     (501) staff       (20)       78 2023-05-30 07:04:20.000000 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield.egg-info/entry_points.txt
--rw-r--r--   0 werner     (501) staff       (20)        1 2021-03-01 12:51:44.000000 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield.egg-info/not-zip-safe
--rw-r--r--   0 werner     (501) staff       (20)       22 2023-05-30 07:04:20.000000 ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield.egg-info/top_level.txt
--rw-r--r--   0 werner     (501) staff       (20)      279 2023-05-30 07:04:20.512089 ffmpeg-progress-yield-0.7.5/setup.cfg
--rw-r--r--   0 werner     (501) staff       (20)     1748 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.5/setup.py
-drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 07:04:20.511311 ffmpeg-progress-yield-0.7.5/test/
--rw-r--r--   0 werner     (501) staff       (20)    37351 2022-12-11 11:53:49.000000 ffmpeg-progress-yield-0.7.5/test/test.mp4
--rw-r--r--   0 werner     (501) staff       (20)     4235 2023-05-30 07:03:53.000000 ffmpeg-progress-yield-0.7.5/test/test.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 07:05:57.176997 ffmpeg-progress-yield-0.7.6/
+-rw-r--r--   0 werner     (501) staff       (20)     2473 2023-05-30 07:05:56.000000 ffmpeg-progress-yield-0.7.6/CHANGELOG.md
+-rw-r--r--   0 werner     (501) staff       (20)     1086 2023-05-05 06:38:37.000000 ffmpeg-progress-yield-0.7.6/LICENSE
+-rw-r--r--   0 werner     (501) staff       (20)    10022 2023-05-30 07:05:57.177096 ffmpeg-progress-yield-0.7.6/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)     6773 2023-05-05 06:38:38.000000 ffmpeg-progress-yield-0.7.6/README.md
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 07:05:57.175205 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield/
+-rw-r--r--   0 werner     (501) staff       (20)      103 2023-05-30 07:05:55.000000 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield/__init__.py
+-rw-r--r--   0 werner     (501) staff       (20)     1283 2023-05-30 06:56:19.000000 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield/__main__.py
+-rw-r--r--   0 werner     (501) staff       (20)     7903 2023-05-30 07:05:38.000000 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield/ffmpeg_progress_yield.py
+-rw-r--r--   0 werner     (501) staff       (20)        0 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield/py.typed
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 07:05:57.176051 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield.egg-info/
+-rw-r--r--   0 werner     (501) staff       (20)    10022 2023-05-30 07:05:57.000000 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield.egg-info/PKG-INFO
+-rw-r--r--   0 werner     (501) staff       (20)      494 2023-05-30 07:05:57.000000 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield.egg-info/SOURCES.txt
+-rw-r--r--   0 werner     (501) staff       (20)        1 2023-05-30 07:05:57.000000 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield.egg-info/dependency_links.txt
+-rw-r--r--   0 werner     (501) staff       (20)       78 2023-05-30 07:05:57.000000 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield.egg-info/entry_points.txt
+-rw-r--r--   0 werner     (501) staff       (20)        1 2021-03-01 12:51:44.000000 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield.egg-info/not-zip-safe
+-rw-r--r--   0 werner     (501) staff       (20)       22 2023-05-30 07:05:57.000000 ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield.egg-info/top_level.txt
+-rw-r--r--   0 werner     (501) staff       (20)      279 2023-05-30 07:05:57.177518 ffmpeg-progress-yield-0.7.6/setup.cfg
+-rw-r--r--   0 werner     (501) staff       (20)     1748 2022-12-18 19:28:54.000000 ffmpeg-progress-yield-0.7.6/setup.py
+drwxr-xr-x   0 werner     (501) staff       (20)        0 2023-05-30 07:05:57.176776 ffmpeg-progress-yield-0.7.6/test/
+-rw-r--r--   0 werner     (501) staff       (20)    37351 2022-12-11 11:53:49.000000 ffmpeg-progress-yield-0.7.6/test/test.mp4
+-rw-r--r--   0 werner     (501) staff       (20)     4235 2023-05-30 07:03:53.000000 ffmpeg-progress-yield-0.7.6/test/test.py
```

### Comparing `ffmpeg-progress-yield-0.7.5/CHANGELOG.md` & `ffmpeg-progress-yield-0.7.6/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # Changelog
 
 
+## v0.7.6 (2023-05-30)
+
+* Always use duration_override if present.
+
+
 ## v0.7.5 (2023-05-30)
 
 * Fix duration for multiple inputs, fixes #13.
 
 * Fix 'Test' string in tqdm.
```

### Comparing `ffmpeg-progress-yield-0.7.5/LICENSE` & `ffmpeg-progress-yield-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.5/PKG-INFO` & `ffmpeg-progress-yield-0.7.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg-progress-yield
-Version: 0.7.5
+Version: 0.7.6
 Summary: Run an ffmpeg command with progress
 Home-page: https://github.com/slhck/ffmpeg-progress-yield
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Keywords: ffmpeg
 Classifier: Development Status :: 4 - Beta
@@ -189,14 +189,19 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 
 # Changelog
 
 
+## v0.7.6 (2023-05-30)
+
+* Always use duration_override if present.
+
+
 ## v0.7.5 (2023-05-30)
 
 * Fix duration for multiple inputs, fixes #13.
 
 * Fix 'Test' string in tqdm.
```

### Comparing `ffmpeg-progress-yield-0.7.5/README.md` & `ffmpeg-progress-yield-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield/__main__.py` & `ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield/__main__.py`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield/ffmpeg_progress_yield.py` & `ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield/ffmpeg_progress_yield.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,17 @@
 
             stderr.append(stderr_line.strip())
 
             self.stderr = "\n".join(stderr)
 
             # assign the total duration if it was found. this can happen multiple times for multiple inputs,
             # in which case we have to determine the overall duration by taking the min/max (dependent on -shortest being present)
-            if total_dur_match := self.DUR_REGEX.search(stderr_line):
+            if (
+                total_dur_match := self.DUR_REGEX.search(stderr_line)
+            ) and duration_override is None:
                 total_dur_ms = to_ms(**total_dur_match.groupdict())
                 if total_dur is not None:
                     total_dur = (
                         min(total_dur, total_dur_ms)
                         if "-shortest" in self.cmd
                         else max(total_dur, total_dur_ms)
                     )
```

### Comparing `ffmpeg-progress-yield-0.7.5/ffmpeg_progress_yield.egg-info/PKG-INFO` & `ffmpeg-progress-yield-0.7.6/ffmpeg_progress_yield.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ffmpeg-progress-yield
-Version: 0.7.5
+Version: 0.7.6
 Summary: Run an ffmpeg command with progress
 Home-page: https://github.com/slhck/ffmpeg-progress-yield
 Author: Werner Robitza
 Author-email: werner.robitza@gmail.com
 License: MIT
 Keywords: ffmpeg
 Classifier: Development Status :: 4 - Beta
@@ -189,14 +189,19 @@
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 
 
 # Changelog
 
 
+## v0.7.6 (2023-05-30)
+
+* Always use duration_override if present.
+
+
 ## v0.7.5 (2023-05-30)
 
 * Fix duration for multiple inputs, fixes #13.
 
 * Fix 'Test' string in tqdm.
```

### Comparing `ffmpeg-progress-yield-0.7.5/setup.py` & `ffmpeg-progress-yield-0.7.6/setup.py`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.5/test/test.mp4` & `ffmpeg-progress-yield-0.7.6/test/test.mp4`

 * *Files identical despite different names*

### Comparing `ffmpeg-progress-yield-0.7.5/test/test.py` & `ffmpeg-progress-yield-0.7.6/test/test.py`

 * *Files identical despite different names*

