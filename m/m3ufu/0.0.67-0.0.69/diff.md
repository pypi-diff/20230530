# Comparing `tmp/m3ufu-0.0.67.tar.gz` & `tmp/m3ufu-0.0.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m3ufu-0.0.67.tar", last modified: Mon Apr 10 22:45:50 2023, max compression
+gzip compressed data, was "m3ufu-0.0.69.tar", last modified: Tue May 30 18:12:58 2023, max compression
```

## Comparing `m3ufu-0.0.67.tar` & `m3ufu-0.0.69.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-04-10 22:45:50.315814 m3ufu-0.0.67/
--rw-r--r--   0 a         (1000) a         (1000)    10183 2023-04-10 22:45:50.315814 m3ufu-0.0.67/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)     9649 2023-04-03 22:14:37.000000 m3ufu-0.0.67/README.md
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-04-10 22:45:50.315814 m3ufu-0.0.67/bin/
--rw-r--r--   0 a         (1000) a         (1000)       54 2023-04-03 22:14:37.000000 m3ufu-0.0.67/bin/m3ufu
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-04-10 22:45:50.315814 m3ufu-0.0.67/m3ufu.egg-info/
--rw-r--r--   0 a         (1000) a         (1000)    10183 2023-04-10 22:45:50.000000 m3ufu-0.0.67/m3ufu.egg-info/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)      181 2023-04-10 22:45:50.000000 m3ufu-0.0.67/m3ufu.egg-info/SOURCES.txt
--rw-r--r--   0 a         (1000) a         (1000)        1 2023-04-10 22:45:50.000000 m3ufu-0.0.67/m3ufu.egg-info/dependency_links.txt
--rw-r--r--   0 a         (1000) a         (1000)       42 2023-04-10 22:45:50.000000 m3ufu-0.0.67/m3ufu.egg-info/requires.txt
--rw-r--r--   0 a         (1000) a         (1000)        6 2023-04-10 22:45:50.000000 m3ufu-0.0.67/m3ufu.egg-info/top_level.txt
--rw-r--r--   0 a         (1000) a         (1000)    17744 2023-04-10 22:45:39.000000 m3ufu-0.0.67/m3ufu.py
--rw-r--r--   0 a         (1000) a         (1000)       38 2023-04-10 22:45:50.315814 m3ufu-0.0.67/setup.cfg
--rw-r--r--   0 a         (1000) a         (1000)      956 2023-04-03 22:14:37.000000 m3ufu-0.0.67/setup.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-30 18:12:58.601889 m3ufu-0.0.69/
+-rw-r--r--   0 a         (1000) a         (1000)     9683 2023-05-30 18:12:58.601889 m3ufu-0.0.69/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)     9149 2023-05-30 18:12:14.000000 m3ufu-0.0.69/README.md
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-30 18:12:58.601889 m3ufu-0.0.69/bin/
+-rw-r--r--   0 a         (1000) a         (1000)       54 2023-05-30 18:06:16.000000 m3ufu-0.0.69/bin/m3ufu
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-05-30 18:12:58.601889 m3ufu-0.0.69/m3ufu.egg-info/
+-rw-r--r--   0 a         (1000) a         (1000)     9683 2023-05-30 18:12:58.000000 m3ufu-0.0.69/m3ufu.egg-info/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)      181 2023-05-30 18:12:58.000000 m3ufu-0.0.69/m3ufu.egg-info/SOURCES.txt
+-rw-r--r--   0 a         (1000) a         (1000)        1 2023-05-30 18:12:58.000000 m3ufu-0.0.69/m3ufu.egg-info/dependency_links.txt
+-rw-r--r--   0 a         (1000) a         (1000)       42 2023-05-30 18:12:58.000000 m3ufu-0.0.69/m3ufu.egg-info/requires.txt
+-rw-r--r--   0 a         (1000) a         (1000)        6 2023-05-30 18:12:58.000000 m3ufu-0.0.69/m3ufu.egg-info/top_level.txt
+-rw-r--r--   0 a         (1000) a         (1000)    17844 2023-05-30 18:12:14.000000 m3ufu-0.0.69/m3ufu.py
+-rw-r--r--   0 a         (1000) a         (1000)       38 2023-05-30 18:12:58.601889 m3ufu-0.0.69/setup.cfg
+-rw-r--r--   0 a         (1000) a         (1000)      956 2023-05-30 18:06:16.000000 m3ufu-0.0.69/setup.py
```

### Comparing `m3ufu-0.0.67/PKG-INFO` & `m3ufu-0.0.69/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,13 @@
-Metadata-Version: 2.1
-Name: m3ufu
-Version: 0.0.67
-Summary: M3U8 Parser with SCTE-35 Support
-Home-page: https://github.com/futzu/m3u8fu
-Author: Adrian
-Author-email: spam@iodisco.com
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
 [Requires](#requires) | [Install](#install) | [Usage](#usage) | [Output](#output) | [SCTE-35](#scte-35) | [AES Decrypt](#automatic-aes-decryption) | [Super Kabuki](https://github.com/futzu/threefive/blob/master/superkabuki.md)
 
-<details> <summary>Phase One: Expose the Pep Deep State. </h4> 
-</summary>
-
-  * [Phase One has begun!](https://github.com/python/peps/compare/main...futzu:peps:main)
-  * [PEP 668.... boo hiss! *(throws a tomato)*](https://peps.python.org/pep-0668/)
-     * Pep 668 inhibits installing packages with pip and pypy3.9,  at least on Debian. 
-     * Quick fix *(notice the use of unlink for dramatic effect)*
-   ```js
-   
-   root@debian:~# unlink /usr/lib/pypy3.9/EXTERNALLY-MANAGED
-   
-   ```
-</details>
-
 
 # M3uFu
 The Most Advanced M3U8 Parser Available.
-### Latest Version `0.0.63`
+### Latest Version `0.0.69`
  > Q. Why is m3ufu better than other m3u8 parsers?
 
 > A. Because most parsers parse for each individual tag differently, this results in a lot of extra code,and each new tag must be specifically supported. M3ufu, in contrast, parses all tags based on the format criteria specified in the RFC. This results in a lot less code, and all HLS tags are automatically supported. 
 
 ### `Features:`
 * All HLS Tags are Supported.
 * Private / Custom Tags are Supported.
```

### Comparing `m3ufu-0.0.67/README.md` & `m3ufu-0.0.69/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
-[Requires](#requires) | [Install](#install) | [Usage](#usage) | [Output](#output) | [SCTE-35](#scte-35) | [AES Decrypt](#automatic-aes-decryption) | [Super Kabuki](https://github.com/futzu/threefive/blob/master/superkabuki.md)
-
-<details> <summary>Phase One: Expose the Pep Deep State. </h4> 
-</summary>
+Metadata-Version: 2.1
+Name: m3ufu
+Version: 0.0.69
+Summary: M3U8 Parser with SCTE-35 Support
+Home-page: https://github.com/futzu/m3u8fu
+Author: Adrian
+Author-email: spam@iodisco.com
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 
-  * [Phase One has begun!](https://github.com/python/peps/compare/main...futzu:peps:main)
-  * [PEP 668.... boo hiss! *(throws a tomato)*](https://peps.python.org/pep-0668/)
-     * Pep 668 inhibits installing packages with pip and pypy3.9,  at least on Debian. 
-     * Quick fix *(notice the use of unlink for dramatic effect)*
-   ```js
-   
-   root@debian:~# unlink /usr/lib/pypy3.9/EXTERNALLY-MANAGED
-   
-   ```
-</details>
+[Requires](#requires) | [Install](#install) | [Usage](#usage) | [Output](#output) | [SCTE-35](#scte-35) | [AES Decrypt](#automatic-aes-decryption) | [Super Kabuki](https://github.com/futzu/threefive/blob/master/superkabuki.md)
 
 
 # M3uFu
 The Most Advanced M3U8 Parser Available.
-### Latest Version `0.0.63`
+### Latest Version `0.0.69`
  > Q. Why is m3ufu better than other m3u8 parsers?
 
 > A. Because most parsers parse for each individual tag differently, this results in a lot of extra code,and each new tag must be specifically supported. M3ufu, in contrast, parses all tags based on the format criteria specified in the RFC. This results in a lot less code, and all HLS tags are automatically supported. 
 
 ### `Features:`
 * All HLS Tags are Supported.
 * Private / Custom Tags are Supported.
```

### Comparing `m3ufu-0.0.67/m3ufu.egg-info/PKG-INFO` & `m3ufu-0.0.69/m3ufu.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,28 @@
 Metadata-Version: 2.1
 Name: m3ufu
-Version: 0.0.67
+Version: 0.0.69
 Summary: M3U8 Parser with SCTE-35 Support
 Home-page: https://github.com/futzu/m3u8fu
 Author: Adrian
 Author-email: spam@iodisco.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 [Requires](#requires) | [Install](#install) | [Usage](#usage) | [Output](#output) | [SCTE-35](#scte-35) | [AES Decrypt](#automatic-aes-decryption) | [Super Kabuki](https://github.com/futzu/threefive/blob/master/superkabuki.md)
 
-<details> <summary>Phase One: Expose the Pep Deep State. </h4> 
-</summary>
-
-  * [Phase One has begun!](https://github.com/python/peps/compare/main...futzu:peps:main)
-  * [PEP 668.... boo hiss! *(throws a tomato)*](https://peps.python.org/pep-0668/)
-     * Pep 668 inhibits installing packages with pip and pypy3.9,  at least on Debian. 
-     * Quick fix *(notice the use of unlink for dramatic effect)*
-   ```js
-   
-   root@debian:~# unlink /usr/lib/pypy3.9/EXTERNALLY-MANAGED
-   
-   ```
-</details>
-
 
 # M3uFu
 The Most Advanced M3U8 Parser Available.
-### Latest Version `0.0.63`
+### Latest Version `0.0.69`
  > Q. Why is m3ufu better than other m3u8 parsers?
 
 > A. Because most parsers parse for each individual tag differently, this results in a lot of extra code,and each new tag must be specifically supported. M3ufu, in contrast, parses all tags based on the format criteria specified in the RFC. This results in a lot less code, and all HLS tags are automatically supported. 
 
 ### `Features:`
 * All HLS Tags are Supported.
 * Private / Custom Tags are Supported.
```

### Comparing `m3ufu-0.0.67/m3ufu.py` & `m3ufu-0.0.69/m3ufu.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 Used to set version in setup.py
 and as an easy way to check which
 version you have installed.
 """
 
 MAJOR = "0"
 MINOR = "0"
-MAINTAINENCE = "67"
+MAINTAINENCE = "69"
 
 
 def version():
     """
     version prints the m3ufu version as a string
     """
     return f"{MAJOR}.{MINOR}.{MAINTAINENCE}"
@@ -110,26 +110,32 @@
 
 class TagParser:
     """
     TagParser parses all HLS Tags as of the latest RFC.
     Custom tags will also be parsed if possible.
     Parsed tags are stored in the Dict TagParser.tags.
     TagParser is used by the Segment class.
+
+
     Example 1:
-        #EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=2030321,BANDWIDTH=2127786,CODECS="avc1.4D401F,mp4a.40.2",RESOLUTION=768x432,CLOSED-CAPTIONS="text"
-                TagParser.tags["#EXT-X-STREAM-INF"]= {"CLOSED-CAPTIONS": "text",
-                                                        "RESOLUTION": "768x432",
-                                                        "CODECS": "avc1.4D401F,mp4a.40.2",
-                                                        "BANDWIDTH": 2127786,
-                                                        "AVERAGE-BANDWIDTH": 2030321}
+
+      #EXT-X-STREAM-INF:AVERAGE-BANDWIDTH=2030321,BANDWIDTH=2127786,CODECS="avc1.4D401F,mp4a.40.2",RESOLUTION=768x432,CLOSED-CAPTIONS="text"
+
+      TagParser.tags["#EXT-X-STREAM-INF"]= { "CLOSED-CAPTIONS": "text",
+                                             "RESOLUTION": "768x432",
+                                             "CODECS": "avc1.4D401F,mp4a.40.2",
+                                             "BANDWIDTH": 2127786,
+                                             "AVERAGE-BANDWIDTH": 2030321}
     Example 2:
-        #EXT-X-CUE-OUT-CONT:ElapsedTime=21.000,Duration=30,SCTE35=/DAnAAAAAAAAAP/wBQb+AGb/MAARAg9DVUVJAAAAAn+HCQA0AALMua1L
-                TagParser.tags["#EXT-X-CUE-OUT-CONT"] = {"SCTE35": "/DAnAAAAAAAAAP/wBQb+AGb/MAARAg9DVUVJAAAAAn+HCQA0AALMua1L",
-                                                        "Duration": 30,
-                                                        "ElapsedTime": 21.0}
+
+      #EXT-X-CUE-OUT-CONT:ElapsedTime=21.000,Duration=30,SCTE35=/DAnAAAAAAAAAP/wBQb+AGb/MAARAg9DVUVJAAAAAn+HCQA0AALMua1L
+
+      TagParser.tags["#EXT-X-CUE-OUT-CONT"] = { "SCTE35": "/DAnAAAAAAAAAP/wBQb+AGb/MAARAg9DVUVJAAAAAn+HCQA0AALMua1L",
+                                                "Duration": 30,
+                                                "ElapsedTime": 21.0}
     """
 
     def __init__(self, lines=None):
         self.tags = {}
         for line in lines:
             self._parse_tags(line)
 
@@ -179,14 +185,16 @@
             return
         splitup = tail.rsplit(",", 1)
         if len(splitup) == 2:
             tail, key = splitup
         else:
             key = splitup[0]
             tail = None
+        if "=" in key:
+            key,value = key.split("=",1)
         self.tags[tag][key] = value
         return tail
 
     def _split_value(self, tag, tail):
         """
         _split_value does a right split
         off tail for the value in a key=value pair.
@@ -212,14 +220,15 @@
 
     def _unquoted(self, tag, tail):
         """
         _unquoted handles unquoted attributes
         """
         value = None
         hold = ""
+        # = is only allowed as a suffix in base64
         while tail.endswith("="):
             hold += tail[-1]
             tail = tail[:-1]
         try:
             tail, value = tail.rsplit("=", 1)
             value += hold
             value = atoif(value)
@@ -242,14 +251,15 @@
         self.end = None
         self.duration = 0
         self.cue = False
         self.cue_data = None
         self.tags = {}
         self.tmp = None
         self.base_uri = base_uri
+        self.relative_uri = media_uri.removeprefix(base_uri)
         self.last_iv = None
         self.last_key_uri = None
         self.debug = False
 
     def __repr__(self):
         return str(self.__dict__)
 
@@ -542,15 +552,15 @@
     def _do_media(self, line):
         playlist = self._is_master(line)
         if playlist:
             media = playlist
         else:
             media = line
             if self.base_uri not in line:
-               media = self.base_uri + media
+                media = self.base_uri + media
         self._add_media(media)
         self.chunk = []
 
     def _parse_header(self, line):
         splitline = line.split(":", 1)
         if splitline[0] in HEADER_TAGS:
             val = ""
```

### Comparing `m3ufu-0.0.67/setup.py` & `m3ufu-0.0.69/setup.py`

 * *Files identical despite different names*

