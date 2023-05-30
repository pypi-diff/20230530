# Comparing `tmp/assemblyai-0.3.3.tar.gz` & `tmp/assemblyai-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyai-0.3.3.tar", last modified: Tue May 30 13:33:35 2023, max compression
+gzip compressed data, was "assemblyai-0.4.0.tar", last modified: Tue May 30 18:31:57 2023, max compression
```

## Comparing `assemblyai-0.3.3.tar` & `assemblyai-0.4.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:33:35.333550 assemblyai-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-30 13:33:26.000000 assemblyai-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-30 13:33:35.333550 assemblyai-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-30 13:33:26.000000 assemblyai-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:33:35.329550 assemblyai-0.3.3/assemblyai/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-30 13:33:26.000000 assemblyai-0.3.3/assemblyai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-30 13:33:26.000000 assemblyai-0.3.3/assemblyai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-30 13:33:26.000000 assemblyai-0.3.3/assemblyai/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-30 13:33:26.000000 assemblyai-0.3.3/assemblyai/lemur.py
--rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-05-30 13:33:26.000000 assemblyai-0.3.3/assemblyai/transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)    44868 2023-05-30 13:33:26.000000 assemblyai-0.3.3/assemblyai/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:33:35.333550 assemblyai-0.3.3/assemblyai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-30 13:33:35.000000 assemblyai-0.3.3/assemblyai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-30 13:33:35.000000 assemblyai-0.3.3/assemblyai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:33:35.000000 assemblyai-0.3.3/assemblyai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-30 13:33:35.000000 assemblyai-0.3.3/assemblyai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 13:33:35.000000 assemblyai-0.3.3/assemblyai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:33:35.333550 assemblyai-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-30 13:33:26.000000 assemblyai-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:33:35.333550 assemblyai-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:33:26.000000 assemblyai-0.3.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:33:35.333550 assemblyai-0.3.3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:33:26.000000 assemblyai-0.3.3/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-30 13:33:26.000000 assemblyai-0.3.3/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-30 13:33:26.000000 assemblyai-0.3.3/tests/unit/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-30 13:33:26.000000 assemblyai-0.3.3/tests/unit/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-30 13:33:26.000000 assemblyai-0.3.3/tests/unit/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-05-30 13:33:26.000000 assemblyai-0.3.3/tests/unit/test_lemur.py
--rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-05-30 13:33:26.000000 assemblyai-0.3.3/tests/unit/test_transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-05-30 13:33:26.000000 assemblyai-0.3.3/tests/unit/test_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:31:57.952522 assemblyai-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-30 18:31:46.000000 assemblyai-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-05-30 18:31:57.952522 assemblyai-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8488 2023-05-30 18:31:46.000000 assemblyai-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:31:57.948522 assemblyai-0.4.0/assemblyai/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-30 18:31:46.000000 assemblyai-0.4.0/assemblyai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-30 18:31:46.000000 assemblyai-0.4.0/assemblyai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-30 18:31:46.000000 assemblyai-0.4.0/assemblyai/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-30 18:31:46.000000 assemblyai-0.4.0/assemblyai/lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20931 2023-05-30 18:31:46.000000 assemblyai-0.4.0/assemblyai/transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44868 2023-05-30 18:31:46.000000 assemblyai-0.4.0/assemblyai/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:31:57.952522 assemblyai-0.4.0/assemblyai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-05-30 18:31:57.000000 assemblyai-0.4.0/assemblyai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-30 18:31:57.000000 assemblyai-0.4.0/assemblyai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:31:57.000000 assemblyai-0.4.0/assemblyai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-30 18:31:57.000000 assemblyai-0.4.0/assemblyai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 18:31:57.000000 assemblyai-0.4.0/assemblyai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 18:31:57.952522 assemblyai-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-30 18:31:46.000000 assemblyai-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:31:57.952522 assemblyai-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:31:46.000000 assemblyai-0.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:31:57.952522 assemblyai-0.4.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 18:31:46.000000 assemblyai-0.4.0/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-30 18:31:46.000000 assemblyai-0.4.0/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-30 18:31:46.000000 assemblyai-0.4.0/tests/unit/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-30 18:31:46.000000 assemblyai-0.4.0/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-30 18:31:46.000000 assemblyai-0.4.0/tests/unit/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-05-30 18:31:46.000000 assemblyai-0.4.0/tests/unit/test_lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-05-30 18:31:46.000000 assemblyai-0.4.0/tests/unit/test_transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-05-30 18:31:46.000000 assemblyai-0.4.0/tests/unit/test_transcript.py
```

### Comparing `assemblyai-0.3.3/LICENSE` & `assemblyai-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `assemblyai-0.3.3/PKG-INFO` & `assemblyai-0.4.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyai
-Version: 0.3.3
+Version: 0.4.0
 Summary: AssemblyAI Python SDK
 Home-page: https://github.com/AssemblyAI/assemblyai-python-sdk
 Author: AssemblyAI
 Author-email: engineering.sdk@assemblyai.com
 License: MIT License
 Project-URL: Code, https://github.com/AssemblyAI/assemblyai-python-sdk
 Project-URL: Issues, https://github.com/AssemblyAI/assemblyai-python-sdk/issues
@@ -286,16 +286,59 @@
 
 Visit one of our Playgrounds:
 
 - [LeMUR Playground](https://www.assemblyai.com/playground/v2/source)
 - [Transcription Playground](https://www.assemblyai.com/playground)
 
 
-# Advanced (TODO)
+# Advanced
 
+## How the SDK handles Default Configurations
+
+### Defining Defaults
+
+When no `TranscriptionConfig` is being passed to the `Transcriber` or its methods, it will use a default instance of a `TranscriptionConfig`.
+
+If you would like to re-use the same `TranscriptionConfig` for all your transcriptions,
+you can set it on the `Transcriber` directly:
+
+```python
+config = aai.TranscriptionConfig(punctuate=False, format_text=False)
+
+transcriber = aai.Transcriber(config=config)
+
+# will use the same config for all `.transcribe*(...)` operations
+transcriber.transcribe("https://example.org/audio.wav")
+```
+
+### Overriding Defaults
+
+You can override the default configuration later via the `.config` property of the `Transcriber`:
+
+```python
+transcriber = aai.Transcriber()
+
+# override the `Transcriber`'s config with a new config
+transcriber.config = aai.TranscriptionConfig(punctuate=False, format_text=False)
+```
+
+
+In case you want to override the `Transcriber`'s configuration for a specific operation with a different one, you can do so via the `config` parameter of a `.transcribe*(...)` method:
+
+```python
+config = aai.TranscriptionConfig(punctuate=False, format_text=False)
+# set a default configuration
+transcriber = aai.Transcriber(config=config)
+
+transcriber.transcribe(
+    "https://example.com/audio.mp3",
+    # overrides the above configuration on the `Transcriber` with the following
+    config=aai.TranscriptionConfig(dual_channel=True, disfluencies=True)
+)
+```
 
 ## Synchronous vs Asynchronous
 
 Currently, the SDK provides two ways to transcribe audio files.
 
 The synchronous approach halts the application's flow until the transcription has been completed.
```

### Comparing `assemblyai-0.3.3/assemblyai/__init__.py` & `assemblyai-0.4.0/assemblyai/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.3.3/assemblyai/api.py` & `assemblyai-0.4.0/assemblyai/api.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.3.3/assemblyai/client.py` & `assemblyai-0.4.0/assemblyai/client.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.3.3/assemblyai/lemur.py` & `assemblyai-0.4.0/assemblyai/lemur.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.3.3/assemblyai/transcriber.py` & `assemblyai-0.4.0/assemblyai/transcriber.py`

 * *Files 14% similar despite different names*

```diff
@@ -438,16 +438,18 @@
     Implementation of the Transcriber class.
     """
 
     def __init__(
         self,
         *,
         client: _client.Client,
+        config: types.TranscriptionConfig,
     ) -> None:
         self._client = client
+        self.config = config
 
     def transcribe_url(
         self,
         *,
         url: str,
         config: types.TranscriptionConfig,
         poll: bool,
@@ -513,15 +515,15 @@
     def transcribe(
         self,
         data: str,
         config: Optional[types.TranscriptionConfig],
         poll: bool,
     ) -> Transcript:
         if config is None:
-            config = types.TranscriptionConfig()
+            config = self.config
 
         if urlparse(data).scheme in {"http", "https"}:
             return self.transcribe_url(
                 url=data,
                 config=config,
                 poll=poll,
             )
@@ -532,17 +534,20 @@
             poll=poll,
         )
 
     def transcribe_group(
         self,
         *,
         data: List[str],
-        config: types.TranscriptionConfig,
+        config: Optional[types.TranscriptionConfig],
         poll: bool,
     ) -> TranscriptGroup:
+        if config is None:
+            config = self.config
+
         executor = concurrent.futures.ThreadPoolExecutor(max_workers=8)
         future_transcripts: Dict[concurrent.futures.Future[Transcript], str] = {}
 
         for d in data:
             transcript_future = executor.submit(
                 self.transcribe,
                 data=d,
@@ -572,49 +577,84 @@
     A transcriber used for transcribing URLs or local audio files.
     """
 
     def __init__(
         self,
         *,
         client: Optional[_client.Client] = None,
+        config: Optional[types.TranscriptionConfig] = None,
         max_workers: Optional[int] = None,
     ) -> None:
         """
         Initializes the `Transcriber` with the given parameters.
 
         Args:
             `client`: The `Client` to use for the `Transcriber`. If `None` is given, the
                 default settings for the `Client` will be used.
+            `config`: The default configuration for the `Transcriber`. If `None` is given,
+                the default configuration of a `TranscriptionConfig` will be used.
             `max_workers`: The maximum number of parallel jobs when using the `_async`
                 methods on the `Transcriber`. By default it uses `os.cpu_count() - 1`
+
+        Example:
+            To use the `Transcriber` with the default settings, you can simply do:
+            ```
+            transcriber = aai.Transcriber()
+            ```
+
+            To use the `Transcriber` with a custom configuration, you can do:
+            ```
+            config = aai.TranscriptionConfig(punctuate=False, format_text=False)
+
+            transcriber = aai.Transcriber(config=config)
+            ```
         """
         self._client = client or _client.Client.get_default()
 
         self._impl = _TranscriberImpl(
             client=self._client,
+            config=config or types.TranscriptionConfig(),
         )
 
         if not max_workers:
             max_workers = max(1, os.cpu_count() - 1)
 
         self._executor = concurrent.futures.ThreadPoolExecutor(
             max_workers=max_workers,
         )
 
+    @property
+    def config(self) -> types.TranscriptionConfig:
+        """
+        Returns the default configuration of the `Transcriber`.
+        """
+        return self._impl.config
+
+    @config.setter
+    def config(self, config: types.TranscriptionConfig) -> None:
+        """
+        Sets the default configuration of the `Transcriber`.
+
+        Args:
+            `config`: The new default configuration.
+        """
+        self._impl.config = config
+
     def submit(
         self,
         data: str,
         config: Optional[types.TranscriptionConfig] = None,
     ) -> Transcript:
         """
         Submits a transcription job without waiting for its completion.
 
         Args:
             data: An URL or a local file (as path)
-            config: Transcription options and features.
+            config: Transcription options and features. If `None` is given, the Transcriber's
+                default configuration will be used.
         """
         return self._impl.transcribe(
             data=data,
             config=config,
             poll=False,
         )
 
@@ -624,16 +664,16 @@
         config: Optional[types.TranscriptionConfig] = None,
     ) -> Transcript:
         """
         Transcribes an audio file whose location can be specified via a URL or file path.
 
         Args:
             data: An URL or a local file (as path)
-            config: Transcription options and features.
-            poll: Whether the transcript should be polled for its completion.
+            config: Transcription options and features. If `None` is given, the Transcriber's
+                default configuration will be used.
         """
 
         return self._impl.transcribe(
             data=data,
             config=config,
             poll=True,
         )
@@ -644,16 +684,16 @@
         config: Optional[types.TranscriptionConfig] = None,
     ) -> concurrent.futures.Future[Transcript]:
         """
         Transcribes an audio file whose location can be specified via a URL or file path.
 
         Args:
             data: An URL or a local file (as path)
-            config: Transcription options and features.
-            poll: Whether the transcript should be polled for its completion.
+            config: Transcription options and features. If `None` is given, the Transcriber's
+                default configuration will be used.
         """
 
         return self._executor.submit(
             self._impl.transcribe,
             data=data,
             config=config,
             poll=True,
@@ -665,39 +705,37 @@
         config: Optional[types.TranscriptionConfig] = None,
     ) -> TranscriptGroup:
         """
         Transcribes a list of files (as paths) or URLs with the given configs.
 
         Args:
             data: A list of paths or URLs (can be mixed)
-            config: Transcription options and features.
-            poll: Whether the transcripts should be polled for their completion.
+            config: Transcription options and features. If `None` is given, the Transcriber's
+                default configuration will be used.
         """
-        if config is None:
-            config = types.TranscriptionConfig()
 
         return self._impl.transcribe_group(
             data=data,
             config=config,
             poll=True,
         )
 
     def transcribe_group_async(
         self,
-        data: str,
+        data: List[str],
         config: Optional[types.TranscriptionConfig] = None,
     ) -> concurrent.futures.Future[TranscriptGroup]:
         """
         Transcribes a list of files (as paths) or URLs with the given configs asynchronously
         by returning a `concurrent.futures.Future[TranscriptGroup]` object.
 
         Args:
             data: A list of paths or URLs (can be mixed)
-            config: Transcription options and features.
-            poll: Whether the transcripts should be polled for their completion.
+            config: Transcription options and features. If `None` is given, the Transcriber's
+                default configuration will be used.
         """
 
         return self._executor.submit(
             self._impl.transcribe_group,
             data=data,
             config=config,
             poll=True,
```

### Comparing `assemblyai-0.3.3/assemblyai/types.py` & `assemblyai-0.4.0/assemblyai/types.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.3.3/assemblyai.egg-info/PKG-INFO` & `assemblyai-0.4.0/assemblyai.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyai
-Version: 0.3.3
+Version: 0.4.0
 Summary: AssemblyAI Python SDK
 Home-page: https://github.com/AssemblyAI/assemblyai-python-sdk
 Author: AssemblyAI
 Author-email: engineering.sdk@assemblyai.com
 License: MIT License
 Project-URL: Code, https://github.com/AssemblyAI/assemblyai-python-sdk
 Project-URL: Issues, https://github.com/AssemblyAI/assemblyai-python-sdk/issues
@@ -286,16 +286,59 @@
 
 Visit one of our Playgrounds:
 
 - [LeMUR Playground](https://www.assemblyai.com/playground/v2/source)
 - [Transcription Playground](https://www.assemblyai.com/playground)
 
 
-# Advanced (TODO)
+# Advanced
 
+## How the SDK handles Default Configurations
+
+### Defining Defaults
+
+When no `TranscriptionConfig` is being passed to the `Transcriber` or its methods, it will use a default instance of a `TranscriptionConfig`.
+
+If you would like to re-use the same `TranscriptionConfig` for all your transcriptions,
+you can set it on the `Transcriber` directly:
+
+```python
+config = aai.TranscriptionConfig(punctuate=False, format_text=False)
+
+transcriber = aai.Transcriber(config=config)
+
+# will use the same config for all `.transcribe*(...)` operations
+transcriber.transcribe("https://example.org/audio.wav")
+```
+
+### Overriding Defaults
+
+You can override the default configuration later via the `.config` property of the `Transcriber`:
+
+```python
+transcriber = aai.Transcriber()
+
+# override the `Transcriber`'s config with a new config
+transcriber.config = aai.TranscriptionConfig(punctuate=False, format_text=False)
+```
+
+
+In case you want to override the `Transcriber`'s configuration for a specific operation with a different one, you can do so via the `config` parameter of a `.transcribe*(...)` method:
+
+```python
+config = aai.TranscriptionConfig(punctuate=False, format_text=False)
+# set a default configuration
+transcriber = aai.Transcriber(config=config)
+
+transcriber.transcribe(
+    "https://example.com/audio.mp3",
+    # overrides the above configuration on the `Transcriber` with the following
+    config=aai.TranscriptionConfig(dual_channel=True, disfluencies=True)
+)
+```
 
 ## Synchronous vs Asynchronous
 
 Currently, the SDK provides two ways to transcribe audio files.
 
 The synchronous approach halts the application's flow until the transcription has been completed.
```

### Comparing `assemblyai-0.3.3/assemblyai.egg-info/SOURCES.txt` & `assemblyai-0.4.0/assemblyai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assemblyai-0.3.3/setup.py` & `assemblyai-0.4.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="assemblyai",
-    version="0.3.3",
+    version="0.4.0",
     description="AssemblyAI Python SDK",
     author="AssemblyAI",
     author_email="engineering.sdk@assemblyai.com",
     packages=find_packages(),
     install_requires=[
         "httpx>=0.19.0",
         "pydantic>=1.7.0",
```

### Comparing `assemblyai-0.3.3/tests/unit/factories.py` & `assemblyai-0.4.0/tests/unit/factories.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.3.3/tests/unit/test_domains.py` & `assemblyai-0.4.0/tests/unit/test_domains.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.3.3/tests/unit/test_lemur.py` & `assemblyai-0.4.0/tests/unit/test_lemur.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.3.3/tests/unit/test_transcriber.py` & `assemblyai-0.4.0/tests/unit/test_transcriber.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.3.3/tests/unit/test_transcript.py` & `assemblyai-0.4.0/tests/unit/test_transcript.py`

 * *Files identical despite different names*

