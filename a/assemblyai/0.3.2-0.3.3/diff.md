# Comparing `tmp/assemblyai-0.3.2.tar.gz` & `tmp/assemblyai-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyai-0.3.2.tar", last modified: Wed May 17 20:22:12 2023, max compression
+gzip compressed data, was "assemblyai-0.3.3.tar", last modified: Tue May 30 13:33:35 2023, max compression
```

## Comparing `assemblyai-0.3.2.tar` & `assemblyai-0.3.3.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:22:12.961701 assemblyai-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-17 20:22:03.000000 assemblyai-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-05-17 20:22:12.957700 assemblyai-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-05-17 20:22:03.000000 assemblyai-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:22:12.957700 assemblyai-0.3.2/assemblyai/
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-17 20:22:03.000000 assemblyai-0.3.2/assemblyai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-17 20:22:03.000000 assemblyai-0.3.2/assemblyai/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-17 20:22:03.000000 assemblyai-0.3.2/assemblyai/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-17 20:22:03.000000 assemblyai-0.3.2/assemblyai/lemur.py
--rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-05-17 20:22:03.000000 assemblyai-0.3.2/assemblyai/transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)    44507 2023-05-17 20:22:03.000000 assemblyai-0.3.2/assemblyai/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:22:12.957700 assemblyai-0.3.2/assemblyai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-05-17 20:22:12.000000 assemblyai-0.3.2/assemblyai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-17 20:22:12.000000 assemblyai-0.3.2/assemblyai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 20:22:12.000000 assemblyai-0.3.2/assemblyai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-17 20:22:12.000000 assemblyai-0.3.2/assemblyai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-17 20:22:12.000000 assemblyai-0.3.2/assemblyai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 20:22:12.961701 assemblyai-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-17 20:22:03.000000 assemblyai-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:22:12.957700 assemblyai-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:22:03.000000 assemblyai-0.3.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 20:22:12.957700 assemblyai-0.3.2/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 20:22:03.000000 assemblyai-0.3.2/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-17 20:22:03.000000 assemblyai-0.3.2/tests/unit/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-17 20:22:03.000000 assemblyai-0.3.2/tests/unit/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-17 20:22:03.000000 assemblyai-0.3.2/tests/unit/test_domains.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-05-17 20:22:03.000000 assemblyai-0.3.2/tests/unit/test_lemur.py
--rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-05-17 20:22:03.000000 assemblyai-0.3.2/tests/unit/test_transcriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-05-17 20:22:03.000000 assemblyai-0.3.2/tests/unit/test_transcript.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:33:35.333550 assemblyai-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-30 13:33:26.000000 assemblyai-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-30 13:33:35.333550 assemblyai-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7024 2023-05-30 13:33:26.000000 assemblyai-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:33:35.329550 assemblyai-0.3.3/assemblyai/
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-05-30 13:33:26.000000 assemblyai-0.3.3/assemblyai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-05-30 13:33:26.000000 assemblyai-0.3.3/assemblyai/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-30 13:33:26.000000 assemblyai-0.3.3/assemblyai/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4353 2023-05-30 13:33:26.000000 assemblyai-0.3.3/assemblyai/lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19563 2023-05-30 13:33:26.000000 assemblyai-0.3.3/assemblyai/transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44868 2023-05-30 13:33:26.000000 assemblyai-0.3.3/assemblyai/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:33:35.333550 assemblyai-0.3.3/assemblyai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-05-30 13:33:35.000000 assemblyai-0.3.3/assemblyai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-30 13:33:35.000000 assemblyai-0.3.3/assemblyai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 13:33:35.000000 assemblyai-0.3.3/assemblyai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-30 13:33:35.000000 assemblyai-0.3.3/assemblyai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 13:33:35.000000 assemblyai-0.3.3/assemblyai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 13:33:35.333550 assemblyai-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1773 2023-05-30 13:33:26.000000 assemblyai-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:33:35.333550 assemblyai-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:33:26.000000 assemblyai-0.3.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 13:33:35.333550 assemblyai-0.3.3/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 13:33:26.000000 assemblyai-0.3.3/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-30 13:33:26.000000 assemblyai-0.3.3/tests/unit/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-30 13:33:26.000000 assemblyai-0.3.3/tests/unit/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-30 13:33:26.000000 assemblyai-0.3.3/tests/unit/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-05-30 13:33:26.000000 assemblyai-0.3.3/tests/unit/test_domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-05-30 13:33:26.000000 assemblyai-0.3.3/tests/unit/test_lemur.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-05-30 13:33:26.000000 assemblyai-0.3.3/tests/unit/test_transcriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9417 2023-05-30 13:33:26.000000 assemblyai-0.3.3/tests/unit/test_transcript.py
```

### Comparing `assemblyai-0.3.2/LICENSE` & `assemblyai-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `assemblyai-0.3.2/PKG-INFO` & `assemblyai-0.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyai
-Version: 0.3.2
+Version: 0.3.3
 Summary: AssemblyAI Python SDK
 Home-page: https://github.com/AssemblyAI/assemblyai-python-sdk
 Author: AssemblyAI
 Author-email: engineering.sdk@assemblyai.com
 License: MIT License
 Project-URL: Code, https://github.com/AssemblyAI/assemblyai-python-sdk
 Project-URL: Issues, https://github.com/AssemblyAI/assemblyai-python-sdk/issues
@@ -108,30 +108,14 @@
 transcript = transcriber.transcribe("https://example.org/audio.mp3")
 
 print(transcript.text)
 ```
 </details>
 
 <details>
-  <summary>Add Punctuation, Casing, and Formatting to a Transcript</summary>
-
-```python
-import assemblyai as aai
-
-config = aai.TranscriptionConfig(
-  punctuate = True,
-  format_text = True,
-)
-
-transcriber = aai.Transcriber()
-transcript = transcriber.transcribe("https://example.org/audio.mp3", config)
-```
-</details>
-
-<details>
   <summary>Export Subtitles of an Audio File</summary>
 
 ```python
 import assemblyai as aai
 
 transcriber = aai.Transcriber()
 transcript = transcriber.transcribe("https://example.org/audio.mp3")
@@ -146,21 +130,16 @@
 
 <details>
   <summary>List all Sentences and Paragraphs</summary>
 
 ```python
 import assemblyai as aai
 
-config = aai.TranscriptionConfig(
-  punctuate = True,
-  format_text = True,
-)
-
 transcriber = aai.Transcriber()
-transcript = transcriber.transcribe("https://example.org/audio.mp3", config)
+transcript = transcriber.transcribe("https://example.org/audio.mp3")
 
 sentences = transcript.get_sentences()
 for sentence in sentences:
   print(sentence.text)
 
 paragraphs = transcript.get_paragraphs()
 for paragraph in paragraphs:
```

### Comparing `assemblyai-0.3.2/README.md` & `assemblyai-0.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -78,30 +78,14 @@
 transcript = transcriber.transcribe("https://example.org/audio.mp3")
 
 print(transcript.text)
 ```
 </details>
 
 <details>
-  <summary>Add Punctuation, Casing, and Formatting to a Transcript</summary>
-
-```python
-import assemblyai as aai
-
-config = aai.TranscriptionConfig(
-  punctuate = True,
-  format_text = True,
-)
-
-transcriber = aai.Transcriber()
-transcript = transcriber.transcribe("https://example.org/audio.mp3", config)
-```
-</details>
-
-<details>
   <summary>Export Subtitles of an Audio File</summary>
 
 ```python
 import assemblyai as aai
 
 transcriber = aai.Transcriber()
 transcript = transcriber.transcribe("https://example.org/audio.mp3")
@@ -116,21 +100,16 @@
 
 <details>
   <summary>List all Sentences and Paragraphs</summary>
 
 ```python
 import assemblyai as aai
 
-config = aai.TranscriptionConfig(
-  punctuate = True,
-  format_text = True,
-)
-
 transcriber = aai.Transcriber()
-transcript = transcriber.transcribe("https://example.org/audio.mp3", config)
+transcript = transcriber.transcribe("https://example.org/audio.mp3")
 
 sentences = transcript.get_sentences()
 for sentence in sentences:
   print(sentence.text)
 
 paragraphs = transcript.get_paragraphs()
 for paragraph in paragraphs:
```

### Comparing `assemblyai-0.3.2/assemblyai/__init__.py` & `assemblyai-0.3.3/assemblyai/__init__.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.3.2/assemblyai/api.py` & `assemblyai-0.3.3/assemblyai/api.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.3.2/assemblyai/client.py` & `assemblyai-0.3.3/assemblyai/client.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.3.2/assemblyai/lemur.py` & `assemblyai-0.3.3/assemblyai/lemur.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.3.2/assemblyai/transcriber.py` & `assemblyai-0.3.3/assemblyai/transcriber.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.3.2/assemblyai/types.py` & `assemblyai-0.3.3/assemblyai/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -292,89 +292,89 @@
     language_code: LanguageCode = LanguageCode.en_us
     """
     The language of your audio file. Possible values are found in Supported Languages.
 
     The default value is `en_us`.
     """
 
-    punctuate: bool = False
+    punctuate: Optional[bool]
     "Enable Automatic Punctuation"
 
-    format_text: bool = False
+    format_text: Optional[bool]
     "Enable Text Formatting"
 
-    dual_channel: bool = False
+    dual_channel: Optional[bool]
     "Enable Dual Channel transcription"
 
-    webhook_url: Optional[str] = None
+    webhook_url: Optional[str]
     "The URL we should send webhooks to when your transcript is complete."
-    webhook_auth_header_name: Optional[str] = None
+    webhook_auth_header_name: Optional[str]
     "The name of the header that is sent when the `webhook_url` is being called."
-    webhook_auth_header_value: Optional[str] = None
+    webhook_auth_header_value: Optional[str]
     "The value of the `webhook_auth_header_name` that is sent when the `webhook_url` is being called."
 
-    audio_start_from: Optional[int] = None
+    audio_start_from: Optional[int]
     "The point in time, in milliseconds, to begin transcription from in your media file."
-    audio_end_at: Optional[int] = None
+    audio_end_at: Optional[int]
     "The point in time, in milliseconds, to stop transcribing in your media file."
 
-    word_boost: Optional[List[str]] = None
+    word_boost: Optional[List[str]]
     "A list of custom vocabulary to boost accuracy for."
-    boost_param: Optional[WordBoost] = None
+    boost_param: Optional[WordBoost]
     "The weight to apply to words/phrases in the word_boost array."
 
-    filter_profanity: bool = False
+    filter_profanity: Optional[bool]
     "Filter profanity from the transcribed text."
 
-    redact_pii: bool = False
+    redact_pii: Optional[bool]
     "Redact PII from the transcribed text."
-    redact_pii_audio: bool = False
+    redact_pii_audio: Optional[bool]
     "Generate a copy of the original media file with spoken PII 'beeped' out."
-    redact_pii_policies: Optional[List[PIIRedactionPolicy]] = None
+    redact_pii_policies: Optional[List[PIIRedactionPolicy]]
     "The list of PII Redaction policies to enable."
-    redact_pii_sub: Optional[PIISubstitutionPolicy] = None
+    redact_pii_sub: Optional[PIISubstitutionPolicy]
     "The replacement logic for detected PII."
 
-    speaker_labels: bool = False
+    speaker_labels: Optional[bool]
     "Enable Speaker Diarization."
 
     # content_safety: bool = False
     # "Enable Content Safety Detection."
 
     # iab_categories: bool = False
     # "Enable Topic Detection."
 
-    custom_spelling: Optional[List[Dict[str, List[str]]]] = None
+    custom_spelling: Optional[List[Dict[str, List[str]]]]
     "Customize how words are spelled and formatted using to and from values"
 
-    disfluencies: bool = False
+    disfluencies: Optional[bool]
     "Transcribe Filler Words, like 'umm', in your media file."
 
     # sentiment_analysis: bool = False
     # "Enable Sentiment Analysis."
 
     # auto_chapters: bool = False
     # "Enable Auto Chapters."
 
     # entity_detection: bool = False
     # "Enable Entity Detection."
 
-    summarization: bool = False
+    summarization: Optional[bool]
     "Enable Summarization"
-    summary_model: Optional[SummarizationModel] = None
+    summary_model: Optional[SummarizationModel]
     "The summarization model to use in case `summarization` is enabled"
-    summary_type: Optional[SummarizationType] = None
+    summary_type: Optional[SummarizationType]
     "The summarization type to use in case `summarization` is enabled"
 
     # auto_highlights: bool = False
     # "Detect important phrases and words in your transcription text."
 
-    language_detection: bool = False
+    language_detection: Optional[bool]
     """
-    Identify the dominant language that’s spoken in an audio file, and route the file to the appropriate model for the detected language.
+    Identify the dominant language that's spoken in an audio file, and route the file to the appropriate model for the detected language.
 
     Automatic Language Detection is supported for the following languages:
 
         - English
         - Spanish
         - French
         - German
@@ -387,42 +387,42 @@
         extra = Extra.allow
 
 
 class TranscriptionConfig:
     def __init__(
         self,
         language_code: LanguageCode = LanguageCode.en_us,
-        punctuate: bool = False,
-        format_text: bool = False,
-        dual_channel: bool = False,
+        punctuate: Optional[bool] = None,
+        format_text: Optional[bool] = None,
+        dual_channel: Optional[bool] = None,
         webhook_url: Optional[str] = None,
         webhook_auth_header_name: Optional[str] = None,
         webhook_auth_header_value: Optional[str] = None,
         audio_start_from: Optional[int] = None,
         audio_end_at: Optional[int] = None,
         word_boost: List[str] = [],
         boost_param: Optional[WordBoost] = None,
-        filter_profanity: bool = False,
-        redact_pii: bool = False,
-        redact_pii_audio: bool = False,
+        filter_profanity: Optional[bool] = None,
+        redact_pii: Optional[bool] = None,
+        redact_pii_audio: Optional[bool] = None,
         redact_pii_policies: Optional[PIIRedactionPolicy] = None,
         redact_pii_sub: Optional[PIISubstitutionPolicy] = None,
-        speaker_labels: bool = False,
+        speaker_labels: Optional[bool] = None,
         # content_safety: bool = False,
         # iab_categories: bool = False,
-        custom_spelling: Dict[str, Union[str, Sequence[str]]] = {},
-        disfluencies: bool = False,
+        custom_spelling: Optional[Dict[str, Union[str, Sequence[str]]]] = None,
+        disfluencies: Optional[bool] = None,
         # sentiment_analysis: bool = False,
         # auto_chapters: bool = False,
         # entity_detection: bool = False,
-        summarization: bool = False,
+        summarization: Optional[bool] = None,
         summary_model: Optional[SummarizationModel] = None,
         summary_type: Optional[SummarizationType] = None,
         # auto_highlights: bool = False,
-        language_detection: bool = False,
+        language_detection: Optional[bool] = None,
         raw_transcription_config: Optional[RawTranscriptionConfig] = None,
     ) -> None:
         """
         Args:
             language_code: The language of your audio file. Possible values are found in Supported Languages.
             punctuate: Enable Automatic Punctuation
             format_text: Enable Text Formatting
@@ -511,45 +511,45 @@
     @language_code.setter
     def language_code(self, language_code: LanguageCode) -> None:
         "Sets the language code of the audio file."
 
         self._raw_transcription_config.language_code = language_code
 
     @property
-    def punctuate(self) -> bool:
+    def punctuate(self) -> Optional[bool]:
         "Returns the status of the Automatic Punctuation feature."
 
         return self._raw_transcription_config.punctuate
 
     @punctuate.setter
-    def punctuate(self, enable: bool) -> None:
+    def punctuate(self, enable: Optional[bool]) -> None:
         "Enable Automatic Punctuation feature."
 
         self._raw_transcription_config.punctuate = enable
 
     @property
-    def format_text(self) -> bool:
+    def format_text(self) -> Optional[bool]:
         "Returns the status of the Text Formatting feature."
 
         return self._raw_transcription_config.format_text
 
     @format_text.setter
-    def format_text(self, enable: bool) -> None:
+    def format_text(self, enable: Optional[bool]) -> None:
         "Enables Formatting Text feature."
 
         self._raw_transcription_config.format_text = enable
 
     @property
-    def dual_channel(self) -> bool:
+    def dual_channel(self) -> Optional[bool]:
         "Returns the status of the Dual Channel transcription feature"
 
         return self._raw_transcription_config.dual_channel
 
     @dual_channel.setter
-    def dual_channel(self, enable: bool = True) -> None:
+    def dual_channel(self, enable: Optional[bool]) -> None:
         "Enable Dual Channel transcription"
 
         self._raw_transcription_config.dual_channel = enable
 
     @property
     def webhook_url(self) -> Optional[str]:
         "The URL we should send webhooks to when your transcript is complete."
@@ -577,69 +577,69 @@
     @property
     def audio_end_at(self) -> Optional[int]:
         "Returns the point in time, in milliseconds, to stop transcribing in your media file."
 
         return self._raw_transcription_config.audio_end_at
 
     @property
-    def word_boost(self) -> List[str]:
+    def word_boost(self) -> Optional[List[str]]:
         "Returns the list of custom vocabulary to boost accuracy for."
 
         return self._raw_transcription_config.word_boost
 
     @property
     def boost_param(self) -> Optional[WordBoost]:
         "Returns how much weight is being applied when boosting custom vocabularies."
 
         return self._raw_transcription_config.boost_param
 
     @property
-    def filter_profanity(self) -> bool:
+    def filter_profanity(self) -> Optional[bool]:
         "Returns the status of whether filtering profanity is enabled or not."
 
         return self._raw_transcription_config.filter_profanity
 
     @filter_profanity.setter
-    def filter_profanity(self, enable: bool) -> None:
+    def filter_profanity(self, enable: Optional[bool]) -> None:
         "Filter profanity from the transcribed text."
 
         self._raw_transcription_config.filter_profanity = enable
 
     @property
-    def redact_pii(self) -> bool:
+    def redact_pii(self) -> Optional[bool]:
         "Returns the status of the PII Redaction feature."
 
         return self._raw_transcription_config.redact_pii
 
     @property
-    def redact_pii_audio(self) -> bool:
+    def redact_pii_audio(self) -> Optional[bool]:
         "Whether or not to generate a copy of the original media file with spoken PII 'beeped' out."
 
         return self._raw_transcription_config.redact_pii_audio
 
     @property
-    def redact_pii_policies(self) -> List[PIIRedactionPolicy]:
+    def redact_pii_policies(self) -> Optional[List[PIIRedactionPolicy]]:
         "Returns a list of set of defined PII redaction policies."
 
         return self._raw_transcription_config.redact_pii_policies
 
     @property
-    def redact_pii_sub(self) -> PIISubstitutionPolicy:
+    def redact_pii_sub(self) -> Optional[PIISubstitutionPolicy]:
         "Returns the replacement logic for detected PII."
 
         return self._raw_transcription_config.redact_pii_sub
 
     @property
-    def speaker_labels(self) -> bool:
+    def speaker_labels(self) -> Optional[bool]:
         "Returns the status of the Speaker Diarization feature."
 
         return self._raw_transcription_config.speaker_labels
 
     @speaker_labels.setter
-    def speaker_labels(self, enable: bool) -> None:
+    def speaker_labels(self, enable: Optional[bool]) -> None:
         "Enable Speaker Diarization feature."
 
         self._raw_transcription_config.speaker_labels = enable
 
     # @property
     # def content_safety(self) -> bool:
     #     "Returns the status of the Content Safety feature."
@@ -661,31 +661,34 @@
     # @iab_categories.setter
     # def iab_categories(self, enable: bool) -> None:
     #     "Enable Topic Detection feature."
 
     #     self._raw_transcription_config.iab_categories = enable
 
     @property
-    def custom_spelling(self) -> Dict[str, List[str]]:
+    def custom_spelling(self) -> Optional[Dict[str, List[str]]]:
         "Returns the current set custom spellings."
 
+        if self._raw_transcription_config.custom_spelling is None:
+            return None
+
         custom_spellings = {}
         for custom_spelling in self._raw_transcription_config.custom_spelling:
             custom_spellings[custom_spelling["from"]] = custom_spelling["to"]
 
         return custom_spellings
 
     @property
-    def disfluencies(self) -> bool:
+    def disfluencies(self) -> Optional[bool]:
         "Returns whether to transcribing filler words is enabled or not."
 
         return self._raw_transcription_config.disfluencies
 
     @disfluencies.setter
-    def disfluencies(self, enable: bool) -> None:
+    def disfluencies(self, enable: Optional[bool]) -> None:
         "Transcribe filler words, like 'umm', in your media file."
 
         self._raw_transcription_config.disfluencies = enable
 
         return self
 
     # @property
@@ -721,15 +724,15 @@
     # @entity_detection.setter
     # def entity_detection(self, enable: bool) -> None:
     #     "Enable Entity Detection."
 
     #     self._raw_transcription_config.entity_detection = enable
 
     @property
-    def summarization(self) -> bool:
+    def summarization(self) -> Optional[bool]:
         "Returns whether the Summarization feature is enabled or not."
 
         return self._raw_transcription_config.summarization
 
     @property
     def summary_model(self) -> Optional[SummarizationModel]:
         "Returns the model of the Summarization feature."
@@ -751,21 +754,21 @@
     # @auto_highlights.setter
     # def auto_highlights(self, enable: bool) -> None:
     #     "Detect important phrases and words in your transcription text."
 
     #     self._raw_transcription_config.auto_highlights = enable
 
     @property
-    def language_detection(self) -> bool:
+    def language_detection(self) -> Optional[bool]:
         "Returns whether Automatic Language Detection is enabled or not."
 
         return self._raw_transcription_config.language_detection
 
     @language_detection.setter
-    def language_detection(self, enable: bool) -> None:
+    def language_detection(self, enable: Optional[bool]) -> None:
         """
         Identify the dominant language that's spoken in an audio file, and route the file to the appropriate model for the detected language.
 
         Automatic Language Detection is supported for the following languages:
 
             - English
             - Spanish
@@ -895,31 +898,31 @@
             enable: whether to enable or disable the PII Redaction feature.
             redact_audio: Generate a copy of the original media file with spoken PII 'beeped' out.
             policies: A list of PII redaction policies to enable.
             substitution: The replacement logic for detected PII (`PIISubstutionPolicy.hash` by default).
         """
 
         if not enable:
-            self._raw_transcription_config.redact_pii = False
-            self._raw_transcription_config.redact_pii_audio = False
+            self._raw_transcription_config.redact_pii = None
+            self._raw_transcription_config.redact_pii_audio = None
             self._raw_transcription_config.redact_pii_policies = None
             self._raw_transcription_config.redact_pii_sub = None
 
             return self
 
         self._raw_transcription_config.redact_pii = True
         self._raw_transcription_config.redact_pii_audio = redact_audio
         self._raw_transcription_config.redact_pii_policies = policies
         self._raw_transcription_config.redact_pii_sub = substitution
 
         return self
 
     def set_custom_spelling(
         self,
-        replacement: Dict[str, Union[str, Sequence[str]]],
+        replacement: Optional[Dict[str, Union[str, Sequence[str]]]],
         override: bool = True,
     ) -> Self:
         """
         Customize how given words are being spelled or formatted in the transcription's text.
 
         Args:
             replacement: A dictionary that contains the replacement object (see below example)
@@ -929,14 +932,17 @@
             ```
             config.custom_spelling({
                 "AssemblyAI": "AssemblyAI",
                 "Kubernetes": ["k8s", "kubernetes"]
             })
             ```
         """
+        if replacement is None:
+            self._raw_transcription_config.custom_spelling = None
+            return self
 
         if self._raw_transcription_config.custom_spelling is None or override:
             self._raw_transcription_config.custom_spelling = []
 
         for to, from_ in replacement.items():
             if isinstance(from_, str):
                 from_ = [from_]
@@ -948,29 +954,29 @@
                 }
             )
 
         return self
 
     def set_summarize(
         self,
-        enable: bool,
+        enable: bool = True,
         model: Optional[SummarizationModel] = None,
         type: Optional[SummarizationType] = None,
     ) -> Self:
         """
         Enable Summarization.
 
         Args:
             enable: whether to enable to disable the Summarization feature.
             model: The summarization model to use
             type: The type of summarization to return
         """
 
         if not enable:
-            self._raw_transcription_config.summarization = False
+            self._raw_transcription_config.summarization = None
             self._raw_transcription_config.summary_model = None
             self._raw_transcription_config.summary_type = None
 
             return self
 
         self._raw_transcription_config.summarization = True
         self._raw_transcription_config.summary_model = model
@@ -1216,87 +1222,87 @@
 
     The default value is `en_us`.
     """
 
     audio_url: str
     "The URL of your media file to transcribe."
 
-    punctuate: bool = False
+    punctuate: Optional[bool]
     "Enable Automatic Punctuation"
 
-    format_text: bool = False
+    format_text: Optional[bool]
     "Enable Text Formatting"
 
-    dual_channel: bool = False
+    dual_channel: Optional[bool]
     "Enable Dual Channel transcription"
 
-    webhook_url: Optional[str] = None
+    webhook_url: Optional[str]
     "The URL we should send webhooks to when your transcript is complete."
-    webhook_auth_header_name: Optional[str] = None
+    webhook_auth_header_name: Optional[str]
     "The name of the header that is sent when the `webhook_url` is being called."
 
-    audio_start_from: Optional[int] = None
+    audio_start_from: Optional[int]
     "The point in time, in milliseconds, to begin transcription from in your media file."
-    audio_end_at: Optional[int] = None
+    audio_end_at: Optional[int]
     "The point in time, in milliseconds, to stop transcribing in your media file."
 
-    word_boost: Optional[List[str]] = None
+    word_boost: Optional[List[str]]
     "A list of custom vocabulary to boost accuracy for."
-    boost_param: Optional[WordBoost] = None
+    boost_param: Optional[WordBoost]
     "The weight to apply to words/phrases in the word_boost array."
 
-    filter_profanity: bool = False
+    filter_profanity: Optional[bool]
     "Filter profanity from the transcribed text."
 
-    redact_pii: bool = False
+    redact_pii: Optional[bool]
     "Redact PII from the transcribed text."
-    redact_pii_audio: bool = False
+    redact_pii_audio: Optional[bool]
     "Generate a copy of the original media file with spoken PII 'beeped' out."
-    redact_pii_policies: Optional[List[PIIRedactionPolicy]] = None
+    redact_pii_policies: Optional[List[PIIRedactionPolicy]]
     "The list of PII Redaction policies to enable."
-    redact_pii_sub: Optional[PIISubstitutionPolicy] = None
+    redact_pii_sub: Optional[PIISubstitutionPolicy]
     "The replacement logic for detected PII."
 
-    speaker_labels: bool = False
+    speaker_labels: Optional[bool]
     "Enable Speaker Diarization."
 
     # content_safety: bool = False
     # "Enable Content Safety Detection."
 
     # iab_categories: bool = False
     # "Enable Topic Detection."
 
-    custom_spelling: Optional[List[dict]] = None
+    custom_spelling: Optional[List[dict]]
     "Customize how words are spelled and formatted using to and from values"
 
-    disfluencies: bool = False
+    disfluencies: Optional[bool]
     "Transcribe Filler Words, like 'umm', in your media file."
 
     # sentiment_analysis: bool = False
     # "Enable Sentiment Analysis."
 
     # auto_chapters: bool = False
     # "Enable Auto Chapters."
 
     # entity_detection: bool = False
     # "Enable Entity Detection."
 
-    summarization: bool = False
+    summarization: Optional[bool]
     "Enable Summarization"
-    summary_model: Optional[SummarizationModel] = None
+    summary_model: Optional[SummarizationModel]
     "The summarization model to use in case `summarization` is enabled"
-    summary_type: Optional[SummarizationType] = None
+    summary_type: Optional[SummarizationType]
     "The summarization type to use in case `summarization` is enabled"
 
     # auto_highlights: bool = False
     # "Detect important phrases and words in your transcription text."
 
-    language_detection: bool = False
+    language_detection: Optional[bool]
     """
-    Identify the dominant language that’s spoken in an audio file, and route the file to the appropriate model for the detected language.
+    Identify the dominant language that's spoken in an audio file, and route the file to the appropriate model for the detected language.
 
     Automatic Language Detection is supported for the following languages:
 
         - English
         - Spanish
         - French
         - German
@@ -1319,35 +1325,35 @@
 
     id: Optional[str]
     "The unique identifier of your transcription"
 
     status: TranscriptStatus
     "The status of your transcription. queued, processing, completed, or error"
 
-    error: Optional[str] = None
+    error: Optional[str]
     "The error message in case the transcription fails"
 
-    text: Optional[str] = None
+    text: Optional[str]
     "The text transcription of your media file"
 
-    words: Optional[List[Word]] = None
+    words: Optional[List[Word]]
     "A list of all the individual words transcribed"
 
-    utterances: Optional[List[Utterance]] = None
+    utterances: Optional[List[Utterance]]
     "When `dual_channel` or `speaker_labels` is enabled, a list of turn-by-turn utterances"
 
-    confidence: Optional[float] = None
+    confidence: Optional[float]
     "The confidence our model has in the transcribed text, between 0.0 and 1.0"
 
-    audio_duration: Optional[float] = None
+    audio_duration: Optional[float]
     "The duration of your media file, in seconds"
 
-    webhook_status_code: Optional[str] = None
+    webhook_status_code: Optional[str]
     "The status code we received from your server when delivering your webhook"
-    webhook_auth: bool = False
+    webhook_auth: Optional[bool]
     "Whether the webhook was sent with an HTTP authentication header"
 
     # auto_highlights_result: Optional[AutohighlightResponse] = None
     # "The list of results when enabling Automatic Transcript Highlights"
 
     # content_safety_labels: Optional[ContentSafetyResponse] = None
     # "The list of results when Content Safety is enabled"
```

### Comparing `assemblyai-0.3.2/assemblyai.egg-info/PKG-INFO` & `assemblyai-0.3.3/assemblyai.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyai
-Version: 0.3.2
+Version: 0.3.3
 Summary: AssemblyAI Python SDK
 Home-page: https://github.com/AssemblyAI/assemblyai-python-sdk
 Author: AssemblyAI
 Author-email: engineering.sdk@assemblyai.com
 License: MIT License
 Project-URL: Code, https://github.com/AssemblyAI/assemblyai-python-sdk
 Project-URL: Issues, https://github.com/AssemblyAI/assemblyai-python-sdk/issues
@@ -108,30 +108,14 @@
 transcript = transcriber.transcribe("https://example.org/audio.mp3")
 
 print(transcript.text)
 ```
 </details>
 
 <details>
-  <summary>Add Punctuation, Casing, and Formatting to a Transcript</summary>
-
-```python
-import assemblyai as aai
-
-config = aai.TranscriptionConfig(
-  punctuate = True,
-  format_text = True,
-)
-
-transcriber = aai.Transcriber()
-transcript = transcriber.transcribe("https://example.org/audio.mp3", config)
-```
-</details>
-
-<details>
   <summary>Export Subtitles of an Audio File</summary>
 
 ```python
 import assemblyai as aai
 
 transcriber = aai.Transcriber()
 transcript = transcriber.transcribe("https://example.org/audio.mp3")
@@ -146,21 +130,16 @@
 
 <details>
   <summary>List all Sentences and Paragraphs</summary>
 
 ```python
 import assemblyai as aai
 
-config = aai.TranscriptionConfig(
-  punctuate = True,
-  format_text = True,
-)
-
 transcriber = aai.Transcriber()
-transcript = transcriber.transcribe("https://example.org/audio.mp3", config)
+transcript = transcriber.transcribe("https://example.org/audio.mp3")
 
 sentences = transcript.get_sentences()
 for sentence in sentences:
   print(sentence.text)
 
 paragraphs = transcript.get_paragraphs()
 for paragraph in paragraphs:
```

### Comparing `assemblyai-0.3.2/assemblyai.egg-info/SOURCES.txt` & `assemblyai-0.3.3/assemblyai.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,11 +12,12 @@
 assemblyai.egg-info/dependency_links.txt
 assemblyai.egg-info/requires.txt
 assemblyai.egg-info/top_level.txt
 tests/__init__.py
 tests/unit/__init__.py
 tests/unit/conftest.py
 tests/unit/factories.py
+tests/unit/test_config.py
 tests/unit/test_domains.py
 tests/unit/test_lemur.py
 tests/unit/test_transcriber.py
 tests/unit/test_transcript.py
```

### Comparing `assemblyai-0.3.2/setup.py` & `assemblyai-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="assemblyai",
-    version="0.3.2",
+    version="0.3.3",
     description="AssemblyAI Python SDK",
     author="AssemblyAI",
     author_email="engineering.sdk@assemblyai.com",
     packages=find_packages(),
     install_requires=[
         "httpx>=0.19.0",
         "pydantic>=1.7.0",
```

### Comparing `assemblyai-0.3.2/tests/unit/factories.py` & `assemblyai-0.3.3/tests/unit/factories.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.3.2/tests/unit/test_domains.py` & `assemblyai-0.3.3/tests/unit/test_domains.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.3.2/tests/unit/test_lemur.py` & `assemblyai-0.3.3/tests/unit/test_lemur.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.3.2/tests/unit/test_transcriber.py` & `assemblyai-0.3.3/tests/unit/test_transcriber.py`

 * *Files identical despite different names*

### Comparing `assemblyai-0.3.2/tests/unit/test_transcript.py` & `assemblyai-0.3.3/tests/unit/test_transcript.py`

 * *Files identical despite different names*

