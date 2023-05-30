# Comparing `tmp/google_speech-1.1.0.tar.gz` & `tmp/google_speech-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/google_speech-1.1.0.tar", last modified: Mon Dec 17 20:55:56 2018, max compression
+gzip compressed data, was "google_speech-1.2.0.tar", last modified: Tue May 30 08:53:00 2023, max compression
```

## Comparing `google_speech-1.1.0.tar` & `google_speech-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-17 20:55:56.000000 google_speech-1.1.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)       43 2018-12-17 20:55:15.000000 google_speech-1.1.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2018-12-17 20:55:15.000000 google_speech-1.1.0/requirements.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     6673 2018-12-17 20:55:56.000000 google_speech-1.1.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4619 2018-12-17 20:55:15.000000 google_speech-1.1.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-17 20:55:56.000000 google_speech-1.1.0/google_speech/
--rw-rw-r--   0 travis    (2000) travis    (2000)      950 2018-12-17 20:55:15.000000 google_speech-1.1.0/google_speech/colored_logging.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      100 2018-12-17 20:55:15.000000 google_speech-1.1.0/google_speech/__main__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    11536 2018-12-17 20:55:15.000000 google_speech-1.1.0/google_speech/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      168 2018-12-17 20:55:15.000000 google_speech-1.1.0/google_speech/bin_dep.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2018-12-17 20:55:56.000000 google_speech-1.1.0/google_speech.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6673 2018-12-17 20:55:56.000000 google_speech-1.1.0/google_speech.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2018-12-17 20:55:56.000000 google_speech-1.1.0/google_speech.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       14 2018-12-17 20:55:56.000000 google_speech-1.1.0/google_speech.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      389 2018-12-17 20:55:56.000000 google_speech-1.1.0/google_speech.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       48 2018-12-17 20:55:56.000000 google_speech-1.1.0/google_speech.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       57 2018-12-17 20:55:56.000000 google_speech-1.1.0/google_speech.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2018-12-17 20:55:56.000000 google_speech-1.1.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)    26530 2018-12-17 20:55:15.000000 google_speech-1.1.0/LICENSE
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2155 2018-12-17 20:55:15.000000 google_speech-1.1.0/setup.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-30 08:53:00.677473 google_speech-1.2.0/
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)    26521 2023-05-30 08:02:06.000000 google_speech-1.2.0/LICENSE
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       43 2014-11-30 01:23:29.000000 google_speech-1.2.0/MANIFEST.in
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     5715 2023-05-30 08:53:00.677473 google_speech-1.2.0/PKG-INFO
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     4475 2023-05-30 08:43:33.000000 google_speech-1.2.0/README.md
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-30 08:53:00.677473 google_speech-1.2.0/google_speech/
+-rwxr-xr-x   0 maxime    (1000) maxime    (1000)    12920 2023-05-30 08:52:40.000000 google_speech-1.2.0/google_speech/__init__.py
+-rwxrwxr-x   0 maxime    (1000) maxime    (1000)      162 2023-05-30 08:18:35.000000 google_speech-1.2.0/google_speech/__main__.py
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)     1040 2023-05-30 08:15:46.000000 google_speech-1.2.0/google_speech/colored_logging.py
+drwxr-xr-x   0 maxime    (1000) maxime    (1000)        0 2023-05-30 08:53:00.677473 google_speech-1.2.0/google_speech.egg-info/
+-rw-r--r--   0 maxime    (1000) maxime    (1000)     5715 2023-05-30 08:53:00.000000 google_speech-1.2.0/google_speech.egg-info/PKG-INFO
+-rw-r--r--   0 maxime    (1000) maxime    (1000)      364 2023-05-30 08:53:00.000000 google_speech-1.2.0/google_speech.egg-info/SOURCES.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)        1 2023-05-30 08:53:00.000000 google_speech-1.2.0/google_speech.egg-info/dependency_links.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       56 2023-05-30 08:53:00.000000 google_speech-1.2.0/google_speech.egg-info/entry_points.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       48 2023-05-30 08:53:00.000000 google_speech-1.2.0/google_speech.egg-info/requires.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       14 2023-05-30 08:53:00.000000 google_speech-1.2.0/google_speech.egg-info/top_level.txt
+-rw-rw-r--   0 maxime    (1000) maxime    (1000)       48 2018-11-04 15:09:55.000000 google_speech-1.2.0/requirements.txt
+-rw-r--r--   0 maxime    (1000) maxime    (1000)       38 2023-05-30 08:53:00.677473 google_speech-1.2.0/setup.cfg
+-rwxr-xr-x   0 maxime    (1000) maxime    (1000)     2114 2023-05-30 08:37:09.000000 google_speech-1.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `google_speech-1.1.0/README.md` & `google_speech-1.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,90 +1,84 @@
-Google Speech
-=============
+# Google Speech
 
 [![Latest version](https://img.shields.io/pypi/v/google_speech.svg?style=flat)](https://pypi.python.org/pypi/google_speech/)
-[![Tests status](https://img.shields.io/travis/desbma/GoogleSpeech/master.svg?label=tests&style=flat)](https://travis-ci.org/desbma/GoogleSpeech)
+[![Tests status](https://github.com/desbma/GoogleSpeech/actions/workflows/ci.yml/badge.svg)](https://github.com/desbma/GoogleSpeech/actions)
 [![Coverage](https://img.shields.io/coveralls/desbma/GoogleSpeech/master.svg?style=flat)](https://coveralls.io/github/desbma/GoogleSpeech?branch=master)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/google_speech.svg?style=flat)](https://pypi.python.org/pypi/google_speech/)
 [![License](https://img.shields.io/github/license/desbma/GoogleSpeech.svg?style=flat)](https://github.com/desbma/GoogleSpeech/blob/master/LICENSE)
 
 Google Speech is a simple multiplatform command line tool to read text using Google Translate TTS (Text To Speech) API.
 
-See also [gTTS](https://github.com/pndurette/gTTS), for a similar but probably more advanced, and actively maintained projet.
-
-
 ## Features
 
-* Support 64 different languages
-* Can read text without length limit
-* Can read text from standard input
-* Automatically pre download the next sentences while playing the current one to avoid long pauses between sentences
-* Automatically store downloaded data in a local cache
-* Can apply any [SoX effect](http://sox.sourceforge.net/sox.html#EFFECTS) to the audio while playing it
-
+- Support 64 different languages
+- Can read text without length limit
+- Can read text from standard input
+- Automatically pre download the next sentences while playing the current one to avoid long pauses between sentences
+- Automatically store downloaded data in a local cache
+- Can apply any [SoX effect](http://sox.sourceforge.net/sox.html#EFFECTS) to the audio while playing it
 
 ## Installation
 
-Google Speech requires [Python](https://www.python.org/downloads/) >= 3.4.
+Google Speech requires [Python](https://www.python.org/downloads/) >= 3.7.
 
 ### From PyPI (with PIP)
 
 1. If you don't already have it, [install pip](https://pip.pypa.io/en/stable/installing/) for Python 3
 2. Install Google Speech: `pip3 install google_speech`
 3. Install [SoX](http://sox.sourceforge.net/), with MP3 support.
-On Ubuntu and other Debian derivatives: `sudo apt-get install sox libsox-fmt-mp3`.
-Windows users can [download binaries on the SoX website](http://sourceforge.net/projects/sox/files/sox/), once installed you also need to copy [libmad DLL](http://ossbuild.googlecode.com/svn/trunk/Shared/Build/Windows/Win32/bin/libmad-0.dll) in the directory where you have installed SoX, and to add this directory to your PATH environment variable.
+   On Ubuntu and other Debian derivatives: `sudo apt-get install sox libsox-fmt-mp3`.
+   Windows users can [download binaries on the SoX website](http://sourceforge.net/projects/sox/files/sox/), once installed you also need to copy [libmad DLL](http://ossbuild.googlecode.com/svn/trunk/Shared/Build/Windows/Win32/bin/libmad-0.dll) in the directory where you have installed SoX, and to add this directory to your PATH environment variable.
 
 ### From source
 
 1. If you don't already have it, [install setuptools](https://pypi.python.org/pypi/setuptools#installation-instructions) for Python 3
 2. Clone this repository: `git clone https://github.com/desbma/GoogleSpeech`
 3. Install Google Speech: `python3 setup.py install`
 4. Install [SoX](http://sox.sourceforge.net/), with MP3 support.
-On Ubuntu and other Debian derivatives: `sudo apt-get install sox libsox-fmt-mp3`.
-Windows users can [download binaries on the SoX website](http://sourceforge.net/projects/sox/files/sox/), once installed you also need to copy [libmad DLL](http://ossbuild.googlecode.com/svn/trunk/Shared/Build/Windows/Win32/bin/libmad-0.dll) in the directory where you have installed SoX, and to add this directory to your PATH environment variable.
-
+   On Ubuntu and other Debian derivatives: `sudo apt-get install sox libsox-fmt-mp3`.
+   Windows users can [download binaries on the SoX website](http://sourceforge.net/projects/sox/files/sox/), once installed you also need to copy [libmad DLL](http://ossbuild.googlecode.com/svn/trunk/Shared/Build/Windows/Win32/bin/libmad-0.dll) in the directory where you have installed SoX, and to add this directory to your PATH environment variable.
 
 ## Command line usage
 
 Run `google_speech -h` to get full command line reference.
 
 ### Examples
 
-* Plane stall alarm:
+- Plane stall alarm:
 
-    `google_speech -l en stall -e delay 0.5 overdrive 20 repeat 5 speed 0.9 gain -5`
+  `google_speech -l en stall -e delay 0.5 overdrive 20 repeat 5 speed 0.9 gain -5`
 
-* Female robot voice (idea from [here](http://ubuntuforums.org/showthread.php?t=1813001&p=11090789#post11090789)):
+- Female robot voice (idea from [here](http://ubuntuforums.org/showthread.php?t=1813001&p=11090789#post11090789)):
 
-    `google_speech -l en "Hello, I am a stupid robot voice" -e speed 0.9 overdrive 10 echo 0.8 0.7 6 0.7 echo 0.8 0.7 10 0.7 echo 0.8 0.7 12 0.7 echo 0.8 0.88 12 0.7 echo 0.8 0.88 30 0.7 echo 0.6 0.6 60 0.7`
+  `google_speech -l en "Hello, I am a stupid robot voice" -e speed 0.9 overdrive 10 echo 0.8 0.7 6 0.7 echo 0.8 0.7 10 0.7 echo 0.8 0.7 12 0.7 echo 0.8 0.88 12 0.7 echo 0.8 0.88 30 0.7 echo 0.6 0.6 60 0.7`
 
-* Save to MP3 file :
-	`google_speech -l en -o hello.mp3 "Hello Google, greetings from France !"`
+- Save to MP3 file :
+  `google_speech -l en -o hello.mp3 "Hello Google, greetings from France !"`
 
 On Unix systems, with Bash and pipes, you can be creative:
 
-* Bash greetings:
-
-    `google_speech -l en "Hello $USER, it is $(date)"`
+- Bash greetings:
 
-* Countdown:
+  `google_speech -l en "Hello $USER, it is $(date)"`
 
-    `for i in {10..0}; do ( google_speech $i & ); sleep 1s; done`
+- Countdown:
 
-* Read a Chuck Norris joke:
+  `for i in {10..0}; do ( google_speech $i & ); sleep 1s; done`
 
-    `curl -s http://api.icndb.com/jokes/random/ | python3 -c 'import html.parser, json, sys; print(html.parser.HTMLParser().unescape(json.load(sys.stdin)["value"]["joke"]))' | google_speech -`
+- Read a Chuck Norris joke:
 
+  `curl -s http://api.icndb.com/jokes/random/ | python3 -c 'import html.parser, json, sys; print(html.parser.HTMLParser().unescape(json.load(sys.stdin)["value"]["joke"]))' | google_speech -`
 
 ## Python usage
 
 You can use `google_speech` from any Python script or module.
 
 Sample code:
+
 ```
 from google_speech import Speech
 
 # say "Hello World"
 text = "Hello World"
 lang = "en"
 speech = Speech(text, lang)
```

### Comparing `google_speech-1.1.0/google_speech/__init__.py` & `google_speech-1.2.0/google_speech/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,327 +1,417 @@
 #!/usr/bin/env python3
 
 """ Read a text using Google Translate TTS API. """
 
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 __author__ = "desbma"
 __license__ = "LGPLv2"
 
 import argparse
 import collections
-import itertools
 import logging
 import os
 import re
-import subprocess
 import string
+import subprocess
 import sys
 import threading
+import unicodedata
 import urllib.parse
 
 import appdirs
 import requests
 import web_cache
 
-from google_speech import bin_dep
 from google_speech import colored_logging
 
-
-SUPPORTED_LANGUAGES = ("af", "ar", "bn", "bs", "ca", "cs", "cy", "da", "de", "el", "en", "en-au", "en-ca", "en-gb",
-                       "en-gh", "en-ie", "en-in", "en-ng", "en-nz", "en-ph", "en-tz", "en-uk", "en-us", "en-za", "eo",
-                       "es", "es-es", "es-us", "et", "fi", "fr", "fr-ca", "fr-fr", "hi", "hr", "hu", "hy", "id", "is",
-                       "it", "ja", "jw", "km", "ko", "la", "lv", "mk", "ml", "mr", "my", "ne", "nl", "no", "pl", "pt",
-                       "pt-br", "pt-pt", "ro", "ru", "si", "sk", "sq", "sr", "su", "sv", "sw", "ta", "te", "th", "tl",
-                       "tr", "uk", "vi", "zh-cn", "zh-tw")
+SUPPORTED_LANGUAGES = (
+    "af",
+    "ar",
+    "bn",
+    "bs",
+    "ca",
+    "cs",
+    "cy",
+    "da",
+    "de",
+    "el",
+    "en",
+    "en-au",
+    "en-ca",
+    "en-gb",
+    "en-gh",
+    "en-ie",
+    "en-in",
+    "en-ng",
+    "en-nz",
+    "en-ph",
+    "en-tz",
+    "en-uk",
+    "en-us",
+    "en-za",
+    "eo",
+    "es",
+    "es-es",
+    "es-us",
+    "et",
+    "fi",
+    "fr",
+    "fr-ca",
+    "fr-fr",
+    "hi",
+    "hr",
+    "hu",
+    "hy",
+    "id",
+    "is",
+    "it",
+    "ja",
+    "jw",
+    "km",
+    "ko",
+    "la",
+    "lv",
+    "mk",
+    "ml",
+    "mr",
+    "my",
+    "ne",
+    "nl",
+    "no",
+    "pl",
+    "pt",
+    "pt-br",
+    "pt-pt",
+    "ro",
+    "ru",
+    "si",
+    "sk",
+    "sq",
+    "sr",
+    "su",
+    "sv",
+    "sw",
+    "ta",
+    "te",
+    "th",
+    "tl",
+    "tr",
+    "uk",
+    "vi",
+    "zh-cn",
+    "zh-tw",
+)
 
 PRELOADER_THREAD_COUNT = 1
 
 
 class PreloaderThread(threading.Thread):
 
-  """ Thread to pre load (download and store in cache) audio data of a segment. """
+    """Thread to pre load (download and store in cache) audio data of a segment."""
 
-  def run(self):
-    try:
-      for segment in self.segments:
-        acquired = segment.preload_mutex.acquire(blocking=False)
-        if acquired:
-          try:
-            if not segment.isInCache():
-              segment.preLoad()
-          finally:
-            segment.preload_mutex.release()
-    except Exception as e:
-      logging.getLogger().error("%s: %s" % (e.__class__.__qualname__, e))
+    def run(self):
+        """See threading.Thread.run."""
+        try:
+            for segment in self.segments:
+                acquired = segment.preload_mutex.acquire(blocking=False)
+                if acquired:
+                    try:
+                        if not segment.isInCache():
+                            segment.preLoad()
+                    finally:
+                        segment.preload_mutex.release()
+        except Exception as e:
+            logging.getLogger().error("%s: %s" % (e.__class__.__qualname__, e))
 
 
 class Speech:
 
-  """ Text to be read. """
+    """Text to be read."""
 
-  CLEAN_MULTIPLE_SPACES_REGEX = re.compile("\s{2,}")
-  MAX_SEGMENT_SIZE = 100
+    CLEAN_MULTIPLE_SPACES_REGEX = re.compile(r"\s{2,}")
+    MAX_SEGMENT_SIZE = 200
 
-  def __init__(self, text, lang):
-    self.text = self.cleanSpaces(text)
-    self.lang = lang
-
-  def __iter__(self):
-    """ Get an iterator over speech segments. """
-    return self.__next__()
-
-  def __next__(self):
-    """ Get a speech segment, splitting text by taking into account spaces, punctuation, and maximum segment size. """
-    if self.text == "-":
-      if sys.stdin.isatty():
-        logging.getLogger().error("Stdin is not a pipe")
-        return
-      while True:
-        new_line = sys.stdin.readline()
-        if not new_line:
-          return
-        segments = __class__.splitText(new_line)
-        for segment_num, segment in enumerate(segments):
-          yield SpeechSegment(segment, self.lang, segment_num, len(segments))
+    def __init__(self, text, lang):
+        self.text = self.cleanSpaces(text)
+        self.lang = lang
+
+    def __iter__(self):
+        """Get an iterator over speech segments."""
+        return self.__next__()
+
+    def __next__(self):
+        """Get a speech segment, splitting text by taking into account spaces, punctuation, and maximum segment size."""
+        if self.text == "-":
+            if sys.stdin.isatty():
+                logging.getLogger().error("Stdin is not a pipe")
+                return
+            while True:
+                new_line = sys.stdin.readline()
+                if not new_line:
+                    return
+                segments = __class__.splitText(new_line)
+                for segment_num, segment in enumerate(segments):
+                    yield SpeechSegment(segment, self.lang, segment_num, len(segments))
 
-    else:
-      segments = __class__.splitText(self.text)
-      for segment_num, segment in enumerate(segments):
-        yield SpeechSegment(segment, self.lang, segment_num, len(segments))
-
-  @staticmethod
-  def splitText(text):
-    useless_chars = frozenset(string.punctuation + string.whitespace)
-    segments = []
-    left = __class__.cleanSpaces(text)
-    previous_right = None
-    while True:
-      while len(left) > __class__.MAX_SEGMENT_SIZE:
-        lr = tuple(map(__class__.cleanSpaces, left.rsplit(" ", 1)))
-        if len(lr) == 2:
-          left, right = lr
         else:
-          left = lr[0][:__class__.MAX_SEGMENT_SIZE]
-          right = lr[0][__class__.MAX_SEGMENT_SIZE:]
-        if previous_right is not None:
-          previous_right = "%s %s" % (right, previous_right)
+            segments = __class__.splitText(self.text)
+            for segment_num, segment in enumerate(segments):
+                yield SpeechSegment(segment, self.lang, segment_num, len(segments))
+
+    @staticmethod
+    def findLastCharIndexMatching(text, func):
+        """Return index of last character in string for which func(char) evaluates to True."""
+        for i in range(len(text) - 1, -1, -1):
+            if func(text[i]):
+                return i
+
+    @staticmethod
+    def splitText(text):
+        """Split text into sub segments of size not bigger than MAX_SEGMENT_SIZE."""
+        segments = []
+        remaining_text = __class__.cleanSpaces(text)
+
+        while len(remaining_text) > __class__.MAX_SEGMENT_SIZE:
+            cur_text = remaining_text[: __class__.MAX_SEGMENT_SIZE]
+
+            # try to split at punctuation
+            split_idx = __class__.findLastCharIndexMatching(
+                cur_text,
+                # https://en.wikipedia.org/wiki/Unicode_character_property#General_Category
+                lambda x: unicodedata.category(x) in ("Ps", "Pe", "Pi", "Pf", "Po"),
+            )
+            if split_idx is None:
+                # try to split at whitespace
+                split_idx = __class__.findLastCharIndexMatching(
+                    cur_text, lambda x: unicodedata.category(x).startswith("Z")
+                )
+            if split_idx is None:
+                # try to split at anything not a letter or number
+                split_idx = __class__.findLastCharIndexMatching(
+                    cur_text, lambda x: not (unicodedata.category(x)[0] in ("L", "N"))
+                )
+            if split_idx is None:
+                # split at the last char
+                split_idx = __class__.MAX_SEGMENT_SIZE - 1
+
+            new_segment = cur_text[: split_idx + 1].rstrip()
+            segments.append(new_segment)
+            remaining_text = remaining_text[split_idx + 1 :].lstrip(string.whitespace + string.punctuation)
+
+        if remaining_text:
+            segments.append(remaining_text)
+
+        return segments
+
+    @staticmethod
+    def cleanSpaces(dirty_string):
+        """Remove consecutive spaces from a string."""
+        return __class__.CLEAN_MULTIPLE_SPACES_REGEX.sub(
+            " ", dirty_string.replace("\n", " ").replace("\t", " ").strip()
+        )
+
+    def play(self, sox_effects=()):
+        """Play a speech."""
+
+        # build the segments
+        preloader_threads = []
+        if self.text != "-":
+            segments = list(self)
+            # start preloader thread(s)
+            preloader_threads = [
+                PreloaderThread(name="PreloaderThread-%u" % (i)) for i in range(PRELOADER_THREAD_COUNT)
+            ]
+            for preloader_thread in preloader_threads:
+                preloader_thread.segments = segments
+                preloader_thread.start()
         else:
-          previous_right = right
-      if any(itertools.filterfalse(useless_chars.__contains__, left)):
-        segments.append(left)
-      if not previous_right:
-        break
-      left = previous_right
-      previous_right = None
-    return segments
-
-  @staticmethod
-  def cleanSpaces(dirty_string):
-    """ Remove consecutive spaces from a string. """
-    return __class__.CLEAN_MULTIPLE_SPACES_REGEX.sub(" ",
-                                                     dirty_string.replace("\n", " ").replace("\t", " ").strip())
-
-  def play(self, sox_effects=()):
-    """ Play a speech. """
-
-    # Build the segments
-    preloader_threads = []
-    if self.text != "-":
-      segments = list(self)
-      # start preloader thread(s)
-      preloader_threads = [PreloaderThread(name="PreloaderThread-%u" % (i)) for i in range(PRELOADER_THREAD_COUNT)]
-      for preloader_thread in preloader_threads:
-        preloader_thread.segments = segments
-        preloader_thread.start()
-    else:
-      segments = iter(self)
+            segments = iter(self)
 
-    # play segments
-    for segment in segments:
-      segment.play(sox_effects)
-
-    if self.text != "-":
-      # destroy preloader threads
-      for preloader_thread in preloader_threads:
-        preloader_thread.join()
-
-  def save(self, path):
-    """ Save audio data to an MP3 file. """
-    with open(path, "wb") as f:
-      for segment in self:
-        f.write(segment.getAudioData())
+        # play segments
+        for segment in segments:
+            segment.play(sox_effects)
+
+        if self.text != "-":
+            # destroy preloader threads
+            for preloader_thread in preloader_threads:
+                preloader_thread.join()
+
+    def save(self, path):
+        """Save audio data to an MP3 file."""
+        with open(path, "wb") as f:
+            self.savef(f)
+
+    def savef(self, file):
+        """Write audio data into a file object."""
+        for segment in self:
+            file.write(segment.getAudioData())
 
 
 class SpeechSegment:
 
-  """ Text segment to be read. """
+    """Text segment to be read."""
 
-  BASE_URL = "https://translate.google.com/translate_tts"
+    BASE_URL = "https://translate.google.com/translate_tts"
 
-  session = requests.Session()
+    session = requests.Session()
 
-  def __init__(self, text, lang, segment_num, segment_count=None):
-    self.text = text
-    self.lang = lang
-    self.segment_num = segment_num
-    self.segment_count = segment_count
-    self.preload_mutex = threading.Lock()
-    if not hasattr(__class__, "cache"):
-      db_filepath = os.path.join(appdirs.user_cache_dir(appname="google_speech",
-                                                        appauthor=False),
-                                 "google_speech-cache.sqlite")
-      os.makedirs(os.path.dirname(db_filepath), exist_ok=True)
-      cache_name = "sound_data"
-      __class__.cache = web_cache.ThreadedWebCache(db_filepath,
-                                                   cache_name,
-                                                   expiration=60 * 60 * 24 * 365,  # 1 year
-                                                   caching_strategy=web_cache.CachingStrategy.LRU)
-      logging.getLogger().debug("Total size of file '%s': %s" % (db_filepath,
-                                                                 __class__.cache.getDatabaseFileSize()))
-      purged_count = __class__.cache.purge()
-      logging.getLogger().debug("%u obsolete entries have been removed from cache '%s'" % (purged_count, cache_name))
-      row_count = len(__class__.cache)
-      logging.getLogger().debug("Cache '%s' contains %u entries" % (cache_name, row_count))
-
-  def __str__(self):
-    return self.text
-
-  def isInCache(self):
-    """ Return True if audio data for this segment is present in cache, False otherwise. """
-    url = self.buildUrl(cache_friendly=True)
-    return url in __class__.cache
-
-  def preLoad(self):
-    """ Store audio data in cache for fast playback. """
-    logging.getLogger().debug("Preloading segment '%s'" % (self))
-    real_url = self.buildUrl()
-    cache_url = self.buildUrl(cache_friendly=True)
-    audio_data = self.download(real_url)
-    assert(audio_data)
-    __class__.cache[cache_url] = audio_data
-
-  def getAudioData(self):
-    """ Fetch the audio data. """
-    with self.preload_mutex:
-      cache_url = self.buildUrl(cache_friendly=True)
-      if cache_url in __class__.cache:
-        logging.getLogger().debug("Got data for URL '%s' from cache" % (cache_url))
-        audio_data = __class__.cache[cache_url]
-        assert(audio_data)
-      else:
+    def __init__(self, text, lang, segment_num, segment_count=None):
+        self.text = text
+        self.lang = lang
+        self.segment_num = segment_num
+        self.segment_count = segment_count
+        self.preload_mutex = threading.Lock()
+        if not hasattr(__class__, "cache"):
+            db_filepath = os.path.join(
+                appdirs.user_cache_dir(appname="google_speech", appauthor=False), "google_speech-cache.sqlite"
+            )
+            os.makedirs(os.path.dirname(db_filepath), exist_ok=True)
+            cache_name = "sound_data"
+            __class__.cache = web_cache.ThreadedWebCache(
+                db_filepath,
+                cache_name,
+                expiration=60 * 60 * 24 * 365,  # 1 year
+                caching_strategy=web_cache.CachingStrategy.LRU,
+            )
+            logging.getLogger().debug(
+                "Total size of file '%s': %s" % (db_filepath, __class__.cache.getDatabaseFileSize())
+            )
+            purged_count = __class__.cache.purge()
+            logging.getLogger().debug(
+                "%u obsolete entries have been removed from cache '%s'" % (purged_count, cache_name)
+            )
+            row_count = len(__class__.cache)
+            logging.getLogger().debug("Cache '%s' contains %u entries" % (cache_name, row_count))
+
+    def __str__(self):
+        return self.text
+
+    def isInCache(self):
+        """Return True if audio data for this segment is present in cache, False otherwise."""
+        url = self.buildUrl(cache_friendly=True)
+        return url in __class__.cache
+
+    def preLoad(self):
+        """Store audio data in cache for fast playback."""
+        logging.getLogger().debug("Preloading segment '%s'" % (self))
         real_url = self.buildUrl()
+        cache_url = self.buildUrl(cache_friendly=True)
         audio_data = self.download(real_url)
-        assert(audio_data)
+        assert audio_data
         __class__.cache[cache_url] = audio_data
-    return audio_data
 
-  def play(self, sox_effects=()):
-    """ Play the segment. """
-    audio_data = self.getAudioData()
-    logging.getLogger().info("Playing speech segment (%s): '%s'" % (self.lang, self))
-    cmd = ["sox", "-q", "-t", "mp3", "-"]
-    if sys.platform.startswith("win32"):
-      cmd.extend(("-t", "waveaudio"))
-    cmd.extend(("-d", "trim", "0.1", "reverse", "trim", "0.07", "reverse"))  # "trim", "0.25", "-0.1"
-    cmd.extend(sox_effects)
-    logging.getLogger().debug("Start player process")
-    p = subprocess.Popen(cmd,
-                         stdin=subprocess.PIPE,
-                         stdout=subprocess.DEVNULL)
-    p.communicate(input=audio_data)
-    if p.returncode != 0:
-      raise RuntimeError()
-    logging.getLogger().debug("Done playing")
-
-  def buildUrl(self, cache_friendly=False):
-    """
-    Construct the URL to get the sound from Goggle API.
-
-    If cache_friendly is True, remove token from URL to use as a cache key.
-    """
-    params = collections.OrderedDict()
-    params["client"] = "tw-ob"
-    params["ie"] = "UTF-8"
-    params["idx"] = str(self.segment_num)
-    if self.segment_count is not None:
-      params["total"] = str(self.segment_count)
-    params["textlen"] = str(len(self.text))
-    params["tl"] = self.lang
-    lower_text = self.text.lower()
-    params["q"] = lower_text
-    return "%s?%s" % (__class__.BASE_URL, urllib.parse.urlencode(params))
-
-  def download(self, url):
-    """ Download a sound file. """
-    logging.getLogger().debug("Downloading '%s'..." % (url))
-    response = __class__.session.get(url,
-                                     headers={"User-Agent": "Mozilla/5.0"},
-                                     timeout=3.1)
-    response.raise_for_status()
-    return response.content
+    def getAudioData(self):
+        """Fetch the audio data."""
+        with self.preload_mutex:
+            cache_url = self.buildUrl(cache_friendly=True)
+            if cache_url in __class__.cache:
+                logging.getLogger().debug("Got data for URL '%s' from cache" % (cache_url))
+                audio_data = __class__.cache[cache_url]
+                assert audio_data
+            else:
+                real_url = self.buildUrl()
+                audio_data = self.download(real_url)
+                assert audio_data
+                __class__.cache[cache_url] = audio_data
+        return audio_data
+
+    def play(self, sox_effects=()):
+        """Play the segment."""
+        audio_data = self.getAudioData()
+        logging.getLogger().info("Playing speech segment (%s): '%s'" % (self.lang, self))
+        cmd = ["sox", "-q", "-t", "mp3", "-"]
+        if sys.platform.startswith("win32"):
+            cmd.extend(("-t", "waveaudio"))
+        cmd.extend(("-d", "trim", "0.1", "reverse", "trim", "0.07", "reverse"))  # "trim", "0.25", "-0.1"
+        cmd.extend(sox_effects)
+        logging.getLogger().debug("Start player process")
+        p = subprocess.Popen(cmd, stdin=subprocess.PIPE, stdout=subprocess.DEVNULL)
+        p.communicate(input=audio_data)
+        if p.returncode != 0:
+            raise RuntimeError()
+        logging.getLogger().debug("Done playing")
+
+    def buildUrl(self, cache_friendly=False):
+        """
+        Construct the URL to get the sound from Goggle API.
+
+        If cache_friendly is True, remove token from URL to use as a cache key.
+        """
+        params = collections.OrderedDict()
+        params["client"] = "tw-ob"
+        params["ie"] = "UTF-8"
+        params["idx"] = str(self.segment_num)
+        if self.segment_count is not None:
+            params["total"] = str(self.segment_count)
+        params["textlen"] = str(len(self.text))
+        params["tl"] = self.lang
+        lower_text = self.text.lower()
+        params["q"] = lower_text
+        return "%s?%s" % (__class__.BASE_URL, urllib.parse.urlencode(params))
+
+    def download(self, url):
+        """Download a sound file."""
+        logging.getLogger().debug("Downloading '%s'..." % (url))
+        response = __class__.session.get(url, headers={"User-Agent": "Mozilla/5.0"}, timeout=3.1)
+        response.raise_for_status()
+        return response.content
 
 
 def cl_main():
-  # parse args
-  arg_parser = argparse.ArgumentParser(description="Google Speech v%s.%s" % (__version__, __doc__),
-                                       formatter_class=argparse.ArgumentDefaultsHelpFormatter)
-  arg_parser.add_argument("speech",
-                          help="Text to play")
-  arg_parser.add_argument("-l",
-                          "--lang",
-                          choices=SUPPORTED_LANGUAGES,
-                          default="en",
-                          dest="lang",
-                          help="Language")
-  arg_parser.add_argument("-e",
-                          "--sox-effects",
-                          default=(),
-                          nargs="+",
-                          dest="sox_effects",
-                          help="SoX effect command to pass to SoX's play")
-  arg_parser.add_argument("-v",
-                          "--verbosity",
-                          choices=("warning", "normal", "debug"),
-                          default="normal",
-                          dest="verbosity",
-                          help="Level of logging output")
-  arg_parser.add_argument("-o",
-                          "--output",
-                          default=None,
-                          dest="output",
-                          help="Outputs audio data to this file instead of playing it")
-  args = arg_parser.parse_args()
-
-  # setup logger
-  logging_level = {"warning": logging.WARNING,
-                   "normal": logging.INFO,
-                   "debug": logging.DEBUG}
-  logging.getLogger().setLevel(logging_level[args.verbosity])
-  logging.getLogger("requests").setLevel(logging.ERROR)
-  logging.getLogger("urllib3").setLevel(logging.ERROR)
-  if logging_level[args.verbosity] == logging.DEBUG:
-    fmt = "%(asctime)s %(threadName)s: %(message)s"
-  else:
-    fmt = "%(message)s"
-  logging_formatter = colored_logging.ColoredFormatter(fmt=fmt)
-  logging_handler = logging.StreamHandler()
-  logging_handler.setFormatter(logging_formatter)
-  logging.getLogger().addHandler(logging_handler)
-
-  if (args.output is not None) and args.sox_effects:
-      logging.getLogger().debug("Effects are not supported when saving to a file")
-      exit(1)
-
-  # do the job
-  speech = Speech(args.speech, args.lang)
-  if args.output:
-    speech.save(args.output)
-  else:
-    speech.play(args.sox_effects)
-
-
-# check deps
-bin_dep.check_bin_dependency(("sox",))
+    """Command line entry point for google_speech."""
+    # parse args
+    arg_parser = argparse.ArgumentParser(
+        description="Google Speech v%s.%s" % (__version__, __doc__),
+        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    )
+    arg_parser.add_argument("speech", help="Text to play")
+    arg_parser.add_argument("-l", "--lang", choices=SUPPORTED_LANGUAGES, default="en", dest="lang", help="Language")
+    arg_parser.add_argument(
+        "-e",
+        "--sox-effects",
+        default=(),
+        nargs="+",
+        dest="sox_effects",
+        help="SoX effect command to pass to SoX's play",
+    )
+    arg_parser.add_argument(
+        "-v",
+        "--verbosity",
+        choices=("warning", "normal", "debug"),
+        default="normal",
+        dest="verbosity",
+        help="Level of logging output",
+    )
+    arg_parser.add_argument(
+        "-o", "--output", default=None, dest="output", help="Outputs audio data to this file instead of playing it"
+    )
+    args = arg_parser.parse_args()
+
+    # setup logger
+    logging_level = {"warning": logging.WARNING, "normal": logging.INFO, "debug": logging.DEBUG}
+    logging.getLogger().setLevel(logging_level[args.verbosity])
+    logging.getLogger("requests").setLevel(logging.ERROR)
+    logging.getLogger("urllib3").setLevel(logging.ERROR)
+    if logging_level[args.verbosity] == logging.DEBUG:
+        fmt = "%(asctime)s %(threadName)s: %(message)s"
+    else:
+        fmt = "%(message)s"
+    logging_formatter = colored_logging.ColoredFormatter(fmt=fmt)
+    logging_handler = logging.StreamHandler()
+    logging_handler.setFormatter(logging_formatter)
+    logging.getLogger().addHandler(logging_handler)
+
+    if (args.output is not None) and args.sox_effects:
+        logging.getLogger().debug("Effects are not supported when saving to a file")
+        exit(1)
+
+    # do the job
+    speech = Speech(args.speech, args.lang)
+    if args.output:
+        speech.save(args.output)
+    else:
+        speech.play(args.sox_effects)
 
 
 if __name__ == "__main__":
-  cl_main()
+    cl_main()
```

### Comparing `google_speech-1.1.0/LICENSE` & `google_speech-1.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 
   To protect each distributor, we want to make it very clear that
 there is no warranty for the free library.  Also, if the library is
 modified by someone else and passed on, the recipients should know
 that what they have is not the original version, so that the original
 author's reputation will not be affected by problems that might be
 introduced by others.
-
+
   Finally, software patents pose a constant threat to the existence of
 any free program.  We wish to make sure that a company cannot
 effectively restrict the users of a free program by obtaining a
 restrictive license from a patent holder.  Therefore, we insist that
 any patent license obtained for a version of the library must be
 consistent with the full freedom of use specified in this license.
 
@@ -107,15 +107,15 @@
 that program using a modified version of the Library.
 
   The precise terms and conditions for copying, distribution and
 modification follow.  Pay close attention to the difference between a
 "work based on the library" and a "work that uses the library".  The
 former contains code derived from the library, whereas the latter must
 be combined with the library in order to run.
-
+
                   GNU LESSER GENERAL PUBLIC LICENSE
    TERMS AND CONDITIONS FOR COPYING, DISTRIBUTION AND MODIFICATION
 
   0. This License Agreement applies to any software library or other
 program which contains a notice placed by the copyright holder or
 other authorized party saying it may be distributed under the terms of
 this Lesser General Public License (also called "this License").
@@ -154,15 +154,15 @@
 all the notices that refer to this License and to the absence of any
 warranty; and distribute a copy of this License along with the
 Library.
 
   You may charge a fee for the physical act of transferring a copy,
 and you may at your option offer warranty protection in exchange for a
 fee.
-
+
   2. You may modify your copy or copies of the Library or any portion
 of it, thus forming a work based on the Library, and copy and
 distribute such modifications or work under the terms of Section 1
 above, provided that you also meet all of these conditions:
 
     a) The modified work must itself be a software library.
 
@@ -212,15 +212,15 @@
 License instead of this License to a given copy of the Library.  To do
 this, you must alter all the notices that refer to this License, so
 that they refer to the ordinary GNU General Public License, version 2,
 instead of to this License.  (If a newer version than version 2 of the
 ordinary GNU General Public License has appeared, then you can specify
 that version instead if you wish.)  Do not make any other change in
 these notices.
-
+
   Once this change is made in a given copy, it is irreversible for
 that copy, so the ordinary GNU General Public License applies to all
 subsequent copies and derivative works made from that copy.
 
   This option is useful when you wish to copy part of the code of
 the Library into a program that is not a library.
 
@@ -263,15 +263,15 @@
 work.  (Executables containing this object code plus portions of the
 Library will still fall under Section 6.)
 
   Otherwise, if the work is a derivative of the Library, you may
 distribute the object code for the work under the terms of Section 6.
 Any executables containing that work also fall under Section 6,
 whether or not they are linked directly with the Library itself.
-
+
   6. As an exception to the Sections above, you may also combine or
 link a "work that uses the Library" with the Library to produce a
 work containing portions of the Library, and distribute that work
 under terms of your choice, provided that the terms permit
 modification of the work for the customer's own use and reverse
 engineering for debugging such modifications.
 
@@ -325,15 +325,15 @@
 the executable.
 
   It may happen that this requirement contradicts the license
 restrictions of other proprietary libraries that do not normally
 accompany the operating system.  Such a contradiction means you cannot
 use both them and the Library together in an executable that you
 distribute.
-
+
   7. You may place library facilities that are a work based on the
 Library side-by-side in a single library together with other library
 facilities not covered by this License, and distribute such a combined
 library, provided that the separate distribution of the work based on
 the Library and of the other library facilities is otherwise
 permitted, and provided that you do these two things:
 
@@ -366,15 +366,15 @@
   10. Each time you redistribute the Library (or any work based on the
 Library), the recipient automatically receives a license from the
 original licensor to copy, distribute, link with or modify the Library
 subject to these terms and conditions.  You may not impose any further
 restrictions on the recipients' exercise of the rights granted herein.
 You are not responsible for enforcing compliance by third parties with
 this License.
-
+
   11. If, as a consequence of a court judgment or allegation of patent
 infringement or for any other reason (not limited to patent issues),
 conditions are imposed on you (whether by court order, agreement or
 otherwise) that contradict the conditions of this License, they do not
 excuse you from the conditions of this License.  If you cannot
 distribute so as to satisfy simultaneously your obligations under this
 License and any other pertinent obligations, then as a consequence you
@@ -418,15 +418,15 @@
 Each version is given a distinguishing version number.  If the Library
 specifies a version number of this License which applies to it and
 "any later version", you have the option of following the terms and
 conditions either of that version or of any later version published by
 the Free Software Foundation.  If the Library does not specify a
 license version number, you may choose any version ever published by
 the Free Software Foundation.
-
+
   14. If you wish to incorporate parts of the Library into other free
 programs whose distribution conditions are incompatible with these,
 write to the author to ask for permission.  For software which is
 copyrighted by the Free Software Foundation, write to the Free
 Software Foundation; we sometimes make exceptions for this.  Our
 decision will be guided by the two goals of preserving the free status
 of all derivatives of our free software and of promoting the sharing
@@ -452,15 +452,15 @@
 LIBRARY (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING
 RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A
 FAILURE OF THE LIBRARY TO OPERATE WITH ANY OTHER SOFTWARE), EVEN IF
 SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH
 DAMAGES.
 
                      END OF TERMS AND CONDITIONS
-
+
            How to Apply These Terms to Your New Libraries
 
   If you develop a new library, and you want it to be of the greatest
 possible use to the public, we recommend making it free software that
 everyone can redistribute and change.  You can do so by permitting
 redistribution under these terms (or, alternatively, under the terms of the
 ordinary General Public License).
```

### Comparing `google_speech-1.1.0/setup.py` & `google_speech-1.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,51 +1,59 @@
 #!/usr/bin/env python3
 
+""" Package setup. """
+
 import os
 import re
 import sys
 
 from setuptools import find_packages, setup
 
-
-if sys.hexversion < 0x3040000:
-  print("Python version %s is unsupported, >= 3.4.0 is needed" % (".".join(map(str, sys.version_info[:3]))))
-  exit(1)
+if sys.hexversion < 0x3070000:
+    print("Python version %s is unsupported, >= 3.7.0 is needed" % (".".join(map(str, sys.version_info[:3]))))
+    exit(1)
 
 with open(os.path.join("google_speech", "__init__.py"), "rt") as f:
-  version = re.search("__version__ = \"([^\"]+)\"", f.read()).group(1)
+    match = re.search('__version__ = "([^"]+)"', f.read())
+    assert match is not None
+    version = match.group(1)
 
 with open("requirements.txt", "rt") as f:
-  requirements = f.read().splitlines()
+    requirements = f.read().splitlines()
 
 with open("README.md", "rt") as f:
-  readme = f.read()
+    readme = f.read()
 
-setup(name="google_speech",
-      version=version,
-      author="desbma",
-      packages=find_packages(exclude=("tests",)),
-      entry_points={"console_scripts": ["google_speech = google_speech:cl_main"]},
-      test_suite="tests",
-      install_requires=requirements,
-      description="Read text using Google Translate TTS API",
-      long_description=readme,
-      long_description_content_type="text/markdown",
-      url="https://github.com/desbma/GoogleSpeech",
-      download_url="https://github.com/desbma/GoogleSpeech/archive/%s.tar.gz" % (version),
-      keywords=["speech", "audio", "synthesis", "voice", "google", "tts"],
-      classifiers=["Development Status :: 5 - Production/Stable",
-                   "Environment :: Console",
-                   "Intended Audience :: Developers",
-                   "Intended Audience :: End Users/Desktop",
-                   "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
-                   "Operating System :: OS Independent",
-                   "Programming Language :: Python",
-                   "Programming Language :: Python :: 3",
-                   "Programming Language :: Python :: 3 :: Only",
-                   "Programming Language :: Python :: 3.4",
-                   "Programming Language :: Python :: 3.5",
-                   "Programming Language :: Python :: 3.6",
-                   "Programming Language :: Python :: 3.7",
-                   "Topic :: Multimedia :: Sound/Audio :: Sound Synthesis",
-                   "Topic :: Multimedia :: Sound/Audio :: Speech",
-                   "Topic :: Utilities"])
+setup(
+    name="google_speech",
+    version=version,
+    author="desbma",
+    packages=find_packages(exclude=("tests",)),
+    entry_points={"console_scripts": ["google_speech = google_speech:cl_main"]},
+    test_suite="tests",
+    install_requires=requirements,
+    description="Read text using Google Translate TTS API",
+    long_description=readme,
+    long_description_content_type="text/markdown",
+    url="https://github.com/desbma/GoogleSpeech",
+    download_url="https://github.com/desbma/GoogleSpeech/archive/%s.tar.gz" % (version),
+    keywords=["speech", "audio", "synthesis", "voice", "google", "tts"],
+    classifiers=[
+        "Development Status :: 5 - Production/Stable",
+        "Environment :: Console",
+        "Intended Audience :: Developers",
+        "Intended Audience :: End Users/Desktop",
+        "License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3 :: Only",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Topic :: Multimedia :: Sound/Audio :: Sound Synthesis",
+        "Topic :: Multimedia :: Sound/Audio :: Speech",
+        "Topic :: Utilities",
+    ],
+)
```

