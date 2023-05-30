# Comparing `tmp/ovos-stt-plugin-fasterwhisper-0.0.1a4.tar.gz` & `tmp/ovos-stt-plugin-fasterwhisper-0.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-stt-plugin-fasterwhisper-0.0.1a4.tar", last modified: Sun May  7 02:48:59 2023, max compression
+gzip compressed data, was "ovos-stt-plugin-fasterwhisper-0.0.1a5.tar", last modified: Tue May 30 02:25:56 2023, max compression
```

## Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a4.tar` & `ovos-stt-plugin-fasterwhisper-0.0.1a5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:48:59.356932 ovos-stt-plugin-fasterwhisper-0.0.1a4/
--rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-07 02:48:49.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-07 02:48:49.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-07 02:48:59.356932 ovos-stt-plugin-fasterwhisper-0.0.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-07 02:48:49.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:48:59.352932 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper/
--rw-r--r--   0 runner    (1001) docker     (123)     8320 2023-05-07 02:48:49.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-07 02:48:55.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-07 02:48:59.356932 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-07 02:48:59.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-07 02:48:59.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:48:59.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-07 02:48:59.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-07 02:48:59.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-07 02:48:59.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-07 02:48:59.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-07 02:48:59.356932 ovos-stt-plugin-fasterwhisper-0.0.1a4/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3493 2023-05-07 02:48:49.000000 ovos-stt-plugin-fasterwhisper-0.0.1a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 02:25:56.589755 ovos-stt-plugin-fasterwhisper-0.0.1a5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11431 2023-05-30 02:25:45.000000 ovos-stt-plugin-fasterwhisper-0.0.1a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-30 02:25:45.000000 ovos-stt-plugin-fasterwhisper-0.0.1a5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-30 02:25:56.589755 ovos-stt-plugin-fasterwhisper-0.0.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-30 02:25:45.000000 ovos-stt-plugin-fasterwhisper-0.0.1a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 02:25:56.589755 ovos-stt-plugin-fasterwhisper-0.0.1a5/ovos_stt_plugin_fasterwhisper/
+-rw-r--r--   0 runner    (1001) docker     (123)     8472 2023-05-30 02:25:45.000000 ovos-stt-plugin-fasterwhisper-0.0.1a5/ovos_stt_plugin_fasterwhisper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-30 02:25:50.000000 ovos-stt-plugin-fasterwhisper-0.0.1a5/ovos_stt_plugin_fasterwhisper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 02:25:56.589755 ovos-stt-plugin-fasterwhisper-0.0.1a5/ovos_stt_plugin_fasterwhisper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-30 02:25:56.000000 ovos-stt-plugin-fasterwhisper-0.0.1a5/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-30 02:25:56.000000 ovos-stt-plugin-fasterwhisper-0.0.1a5/ovos_stt_plugin_fasterwhisper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 02:25:56.000000 ovos-stt-plugin-fasterwhisper-0.0.1a5/ovos_stt_plugin_fasterwhisper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-30 02:25:56.000000 ovos-stt-plugin-fasterwhisper-0.0.1a5/ovos_stt_plugin_fasterwhisper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-30 02:25:56.000000 ovos-stt-plugin-fasterwhisper-0.0.1a5/ovos_stt_plugin_fasterwhisper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-30 02:25:56.000000 ovos-stt-plugin-fasterwhisper-0.0.1a5/ovos_stt_plugin_fasterwhisper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 02:25:56.000000 ovos-stt-plugin-fasterwhisper-0.0.1a5/ovos_stt_plugin_fasterwhisper.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 02:25:56.589755 ovos-stt-plugin-fasterwhisper-0.0.1a5/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3493 2023-05-30 02:25:45.000000 ovos-stt-plugin-fasterwhisper-0.0.1a5/setup.py
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a4/LICENSE` & `ovos-stt-plugin-fasterwhisper-0.0.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a4/PKG-INFO` & `ovos-stt-plugin-fasterwhisper-0.0.1a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-stt-plugin-fasterwhisper
-Version: 0.0.1a4
+Version: 0.0.1a5
 Summary: A fasterwhisper stt plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-plugin-fasterwhisper
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft ovos plugin stt
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a4/README.md` & `ovos-stt-plugin-fasterwhisper-0.0.1a5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -20,31 +20,30 @@
 ```json
   "stt": {
     "module": "ovos-stt-plugin-fasterwhisper",
     "ovos-stt-plugin-fasterwhisper": {
         "model": "large-v2",
         "use_cuda": true,
         "compute_type": "float16",
-        "beam_size": 5
+        "beam_size": 5,
+        "cpu_threads": 4
     }
   }
- 
 ```
 
 To use Whisper for lang detection  (ovos-dinkum-listener only)
 
 
 ```json
   "listener": {
     "audio_transformers": {
         "ovos-audio-transformer-plugin-fasterwhisper": {
             "model": "small"
         }
     }
   }
-
 ```
 
 ## Models
 
 Models will be auto downloaded by faster whisper on plugin load
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper/__init__.py` & `ovos-stt-plugin-fasterwhisper-0.0.1a5/ovos_stt_plugin_fasterwhisper/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
             model = "small"
 
         assert model in FasterWhisperSTT.MODELS  # TODO - better error handling
 
         self.compute_type = self.config.get("compute_type", "int8")
         self.use_cuda = self.config.get("use_cuda", False)
         self.beam_size = self.config.get("beam_size", 5)
+        self.cpu_threads = self.config.get("cpu_threads", 4)
 
         if self.use_cuda:
             device = "cuda"
         else:
             device = "cpu"
         self.engine = WhisperModel(model, device=device, compute_type=self.compute_type)
 
@@ -183,20 +184,21 @@
         if not model:
             model = "small"
         assert model in self.MODELS  # TODO - better error handling
 
         self.beam_size = self.config.get("beam_size", 5)
         self.compute_type = self.config.get("compute_type", "int8")
         self.use_cuda = self.config.get("use_cuda", False)
+        self.cpu_threads = self.config.get("cpu_threads", 4)
 
         if self.use_cuda:
             device = "cuda"
         else:
             device = "cpu"
-        self.engine = WhisperModel(model, device=device, compute_type=self.compute_type)
+        self.engine = WhisperModel(model, device=device, compute_type=self.compute_type, cpu_threads=self.cpu_threads)
 
     @staticmethod
     def audiodata2array(audio_data):
         assert isinstance(audio_data, AudioData)
         return FasterWhisperLangClassifier.audiochunk2array(audio_data.get_wav_data())
 
     def execute(self, audio, language=None):
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a4/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO` & `ovos-stt-plugin-fasterwhisper-0.0.1a5/ovos_stt_plugin_fasterwhisper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: ovos-stt-plugin-fasterwhisper
-Version: 0.0.1a4
+Version: 0.0.1a5
 Summary: A fasterwhisper stt plugin for mycroft
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-plugin-fasterwhisper
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Description: UNKNOWN
 Keywords: mycroft ovos plugin stt
```

### Comparing `ovos-stt-plugin-fasterwhisper-0.0.1a4/setup.py` & `ovos-stt-plugin-fasterwhisper-0.0.1a5/setup.py`

 * *Files identical despite different names*

