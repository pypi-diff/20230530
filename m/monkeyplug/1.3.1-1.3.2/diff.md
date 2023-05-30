# Comparing `tmp/monkeyplug-1.3.1.tar.gz` & `tmp/monkeyplug-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monkeyplug-1.3.1.tar", last modified: Thu Nov 10 20:03:19 2022, max compression
+gzip compressed data, was "monkeyplug-1.3.2.tar", last modified: Tue May 30 03:54:26 2023, max compression
```

## Comparing `monkeyplug-1.3.1.tar` & `monkeyplug-1.3.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:03:19.074215 monkeyplug-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1510 2022-11-10 20:03:08.000000 monkeyplug-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     5059 2022-11-10 20:03:19.074215 monkeyplug-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4463 2022-11-10 20:03:08.000000 monkeyplug-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      103 2022-11-10 20:03:08.000000 monkeyplug-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      897 2022-11-10 20:03:19.074215 monkeyplug-1.3.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:03:19.070215 monkeyplug-1.3.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:03:19.070215 monkeyplug-1.3.1/src/monkeyplug/
--rw-r--r--   0 runner    (1001) docker     (121)      198 2022-11-10 20:03:08.000000 monkeyplug-1.3.1/src/monkeyplug/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    23882 2022-11-10 20:03:08.000000 monkeyplug-1.3.1/src/monkeyplug/monkeyplug.py
--rw-r--r--   0 runner    (1001) docker     (121)     7286 2022-11-10 20:03:08.000000 monkeyplug-1.3.1/src/monkeyplug/swears.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-10 20:03:19.074215 monkeyplug-1.3.1/src/monkeyplug.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5059 2022-11-10 20:03:19.000000 monkeyplug-1.3.1/src/monkeyplug.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-11-10 20:03:19.000000 monkeyplug-1.3.1/src/monkeyplug.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 20:03:19.000000 monkeyplug-1.3.1/src/monkeyplug.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-10 20:03:19.000000 monkeyplug-1.3.1/src/monkeyplug.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-10 20:03:18.000000 monkeyplug-1.3.1/src/monkeyplug.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-11-10 20:03:19.000000 monkeyplug-1.3.1/src/monkeyplug.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-11-10 20:03:19.000000 monkeyplug-1.3.1/src/monkeyplug.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:54:26.540839 monkeyplug-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-30 03:54:16.000000 monkeyplug-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-30 03:54:26.540839 monkeyplug-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-05-30 03:54:16.000000 monkeyplug-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-30 03:54:16.000000 monkeyplug-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-30 03:54:26.540839 monkeyplug-1.3.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:54:26.536839 monkeyplug-1.3.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:54:26.540839 monkeyplug-1.3.2/src/monkeyplug/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-30 03:54:16.000000 monkeyplug-1.3.2/src/monkeyplug/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24565 2023-05-30 03:54:16.000000 monkeyplug-1.3.2/src/monkeyplug/monkeyplug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-05-30 03:54:16.000000 monkeyplug-1.3.2/src/monkeyplug/swears.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 03:54:26.540839 monkeyplug-1.3.2/src/monkeyplug.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-30 03:54:26.000000 monkeyplug-1.3.2/src/monkeyplug.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-30 03:54:26.000000 monkeyplug-1.3.2/src/monkeyplug.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 03:54:26.000000 monkeyplug-1.3.2/src/monkeyplug.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-30 03:54:26.000000 monkeyplug-1.3.2/src/monkeyplug.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 03:54:26.000000 monkeyplug-1.3.2/src/monkeyplug.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-30 03:54:26.000000 monkeyplug-1.3.2/src/monkeyplug.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 03:54:26.000000 monkeyplug-1.3.2/src/monkeyplug.egg-info/top_level.txt
```

### Comparing `monkeyplug-1.3.1/LICENSE` & `monkeyplug-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `monkeyplug-1.3.1/PKG-INFO` & `monkeyplug-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monkeyplug
-Version: 1.3.1
+Version: 1.3.2
 Summary: monkeyplug is a little script to mute profanity in audio files.
 Home-page: https://github.com/mmguero/monkeyplug
 Author: Seth Grover
 Author-email: mero.mero.guero@gmail.com
 Project-URL: Bug Tracker, https://github.com/mmguero/monkeyplug/issues
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `monkeyplug-1.3.1/README.md` & `monkeyplug-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `monkeyplug-1.3.1/setup.cfg` & `monkeyplug-1.3.2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = monkeyplug
-version = 1.3.1
+version = 1.3.2
 author = Seth Grover
 author_email = mero.mero.guero@gmail.com
 description = monkeyplug is a little script to mute profanity in audio files.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/mmguero/monkeyplug
 project_urls =
```

### Comparing `monkeyplug-1.3.1/src/monkeyplug/monkeyplug.py` & `monkeyplug-1.3.2/src/monkeyplug/monkeyplug.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,47 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 
 import argparse
+import base64
 import errno
 import json
 import mmguero
 import mutagen
 import os
 import requests
 import shutil
 import sys
 import vosk
 import wave
 
 from urllib.parse import urlparse
 
 ###################################################################################################
+CHANNELS_REPLACER = 'CHANNELS'
 AUDIO_DEFAULT_PARAMS_BY_FORMAT = {
-    "flac": ["-c:a", "flac", "-ar", "44100", "-ac", "2"],
-    "m4a": ["-c:a", "aac", "-b:a", "128K", "-ar", "44100", "-ac", "2"],
-    "aac": ["-c:a", "aac", "-b:a", "128K", "-ar", "44100", "-ac", "2"],
-    "mp3": ["-c:a", "libmp3lame", "-b:a", "128K", "-ar", "44100", "-ac", "2"],
-    "ogg": ["-c:a", "libvorbis", "-qscale:a", "5", "-ar", "44100", "-ac", "2"],
-    "opus": ["-c:a", "libopus", "-b:a", "128K", "-ar", "48000", "-ac", "2"],
-    "ac3": ["-c:a", "ac3", "-b:a", "128K", "-ar", "44100", "-ac", "2"],
+    "flac": ["-c:a", "flac", "-ar", "44100", "-ac", CHANNELS_REPLACER],
+    "m4a": ["-c:a", "aac", "-b:a", "128K", "-ar", "44100", "-ac", CHANNELS_REPLACER],
+    "aac": ["-c:a", "aac", "-b:a", "128K", "-ar", "44100", "-ac", CHANNELS_REPLACER],
+    "mp3": ["-c:a", "libmp3lame", "-b:a", "128K", "-ar", "44100", "-ac", CHANNELS_REPLACER],
+    "ogg": ["-c:a", "libvorbis", "-qscale:a", "5", "-ar", "44100", "-ac", CHANNELS_REPLACER],
+    "opus": ["-c:a", "libopus", "-b:a", "128K", "-ar", "48000", "-ac", CHANNELS_REPLACER],
+    "ac3": ["-c:a", "ac3", "-b:a", "128K", "-ar", "44100", "-ac", CHANNELS_REPLACER],
 }
 AUDIO_CODEC_TO_FORMAT = {
     "aac": "m4a",
     "ac3": "ac3",
     "flac": "flac",
     "mp3": "mp3",
     "opus": "opus",
     "vorbis": "ogg",
 }
 
 AUDIO_DEFAULT_FORMAT = "mp3"
+AUDIO_DEFAULT_CHANNELS = 2
 AUDIO_MATCH_FORMAT = "MATCH"
 AUDIO_INTERMEDIATE_PARAMS = ["-c:a", "pcm_s16le", "-ac", "1", "-ar", "16000"]
 AUDIO_DEFAULT_WAV_FRAMES_CHUNK = 8000
 SWEARS_FILENAME_DEFAULT = 'swears.txt'
 MUTAGEN_METADATA_TAGS = ['encodedby', 'comment']
 MUTAGEN_METADATA_TAG_VALUE = u'monkeyplug'
 
@@ -190,14 +193,15 @@
         iFileSpec,
         oFileSpec,
         oAudioFileFormat,
         iSwearsFileSpec,
         mPath,
         outputJson,
         aParams=None,
+        aChannels=AUDIO_DEFAULT_CHANNELS,
         wChunk=AUDIO_DEFAULT_WAV_FRAMES_CHUNK,
         padMsecPre=0,
         padMsecPost=0,
         force=False,
         dbug=False,
     ):
         self.wavReadFramesChunk = wChunk
@@ -277,15 +281,17 @@
         elif not aParams:
             # we're using ffmpeg encoding params based on output file format
             self.aParams = AUDIO_DEFAULT_PARAMS_BY_FORMAT[self.outputAudioFileFormat]
         else:
             # they specified custom ffmpeg encoding params
             self.aParams = aParams
             if self.aParams.startswith("base64:"):
-                self.aParams = base64.b64decode(self.aParams[7:]).decode("utf-8").split(' ')
+                self.aParams = base64.b64decode(self.aParams[7:]).decode("utf-8")
+            self.aParams = self.aParams.split(' ')
+        self.aParams = [str(aChannels) if aParam == CHANNELS_REPLACER else aParam for aParam in self.aParams]
 
         # if we're actually just replacing the audio stream(s) inside a video file, the actual output file is still a video file
         self.outputVideoFileFormat = (
             inParts[1]
             if (
                 (len(mmguero.GetIterable(self.inputCodecs.get('video', []))) > 0)
                 and (str(oAudioFileFormat).upper() == AUDIO_MATCH_FORMAT)
@@ -483,14 +489,15 @@
             shutil.copyfile(self.inputFileSpec, self.outputFileSpec)
 
         return self.outputFileSpec
 
 
 #################################################################################
 
+
 ###################################################################################################
 # RunMonkeyPlug
 def RunMonkeyPlug():
     parser = argparse.ArgumentParser(
         description=script_name,
         add_help=False,
         usage="{} <arguments>".format(script_name),
@@ -541,19 +548,28 @@
         help=f"text file containing profanity (default: \"{SWEARS_FILENAME_DEFAULT}\")",
         default=os.path.join(script_path, SWEARS_FILENAME_DEFAULT),
         metavar="<profanity file>",
     )
     parser.add_argument(
         "-a",
         "--audio-params",
-        help=f"Audio parameters for ffmpeg (default depends on output audio codec\")",
+        help=f"Audio parameters for ffmpeg (default depends on output audio codec)",
         dest="aParams",
         default=None,
     )
     parser.add_argument(
+        "-c",
+        "--channels",
+        dest="aChannels",
+        metavar="<int>",
+        type=int,
+        default=AUDIO_DEFAULT_CHANNELS,
+        help=f"Audio output channels (default: {AUDIO_DEFAULT_CHANNELS})",
+    )
+    parser.add_argument(
         "-f",
         "--format",
         dest="outputFormat",
         type=str,
         default=AUDIO_MATCH_FORMAT,
         required=False,
         metavar="<string>",
@@ -610,15 +626,16 @@
         metavar="true|false",
         help="Process file despite existence of embedded tag",
     )
 
     try:
         parser.error = parser.exit
         args = parser.parse_args()
-    except SystemExit:
+    except SystemExit as sy:
+        mmguero.eprint(sy)
         parser.print_help()
         exit(2)
 
     if args.debug:
         mmguero.eprint(os.path.join(script_path, script_name))
         mmguero.eprint("Arguments: {}".format(sys.argv[1:]))
         mmguero.eprint("Arguments: {}".format(args))
@@ -631,14 +648,15 @@
             args.input,
             args.output,
             args.outputFormat,
             args.swears,
             args.modelPath,
             args.outputJson,
             aParams=args.aParams,
+            aChannels=args.aChannels,
             wChunk=args.readFramesChunk,
             padMsecPre=args.padMsecPre if args.padMsecPre > 0 else args.padMsec,
             padMsecPost=args.padMsecPost if args.padMsecPost > 0 else args.padMsec,
             force=args.forceDespiteTag,
             dbug=args.debug,
         ).EncodeCleanAudio()
     )
```

### Comparing `monkeyplug-1.3.1/src/monkeyplug/swears.txt` & `monkeyplug-1.3.2/src/monkeyplug/swears.txt`

 * *Files identical despite different names*

### Comparing `monkeyplug-1.3.1/src/monkeyplug.egg-info/PKG-INFO` & `monkeyplug-1.3.2/src/monkeyplug.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monkeyplug
-Version: 1.3.1
+Version: 1.3.2
 Summary: monkeyplug is a little script to mute profanity in audio files.
 Home-page: https://github.com/mmguero/monkeyplug
 Author: Seth Grover
 Author-email: mero.mero.guero@gmail.com
 Project-URL: Bug Tracker, https://github.com/mmguero/monkeyplug/issues
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

