# Comparing `tmp/ovos-stt-http-server-0.0.2a5.tar.gz` & `tmp/ovos-stt-http-server-0.0.2a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-stt-http-server-0.0.2a5.tar", last modified: Fri May  5 23:20:06 2023, max compression
+gzip compressed data, was "ovos-stt-http-server-0.0.2a6.tar", last modified: Tue May 30 18:08:28 2023, max compression
```

## Comparing `ovos-stt-http-server-0.0.2a5.tar` & `ovos-stt-http-server-0.0.2a6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:20:06.118240 ovos-stt-http-server-0.0.2a5/
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-05 23:20:06.118240 ovos-stt-http-server-0.0.2a5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:20:06.114240 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/
--rw-r--r--   0 runner    (1001) docker     (123)     4931 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:20:06.118240 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/
--rw-r--r--   0 runner    (1001) docker     (123)    58605 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/ca.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    54765 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/de.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    50925 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/en.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    55341 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/es.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    57453 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/fr.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    62637 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/it.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    68781 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/nl.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    48813 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/pt.mp3
--rw-r--r--   0 runner    (1001) docker     (123)    67821 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/uk.mp3
--rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/gradio_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 23:20:06.114240 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-05-05 23:20:06.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-05 23:20:06.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 23:20:06.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-05 23:20:06.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-05 23:20:06.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 23:20:06.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 23:20:06.000000 ovos-stt-http-server-0.0.2a5/ovos_stt_http_server.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 23:20:06.118240 ovos-stt-http-server-0.0.2a5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3049 2023-05-05 23:20:05.000000 ovos-stt-http-server-0.0.2a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:08:28.150126 ovos-stt-http-server-0.0.2a6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-30 18:08:27.000000 ovos-stt-http-server-0.0.2a6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-30 18:08:28.150126 ovos-stt-http-server-0.0.2a6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:08:28.146126 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-05-30 18:08:27.000000 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-05-30 18:08:27.000000 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:08:28.150126 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)    58605 2023-05-30 18:08:27.000000 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/audio/ca.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    54765 2023-05-30 18:08:27.000000 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/audio/de.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    50925 2023-05-30 18:08:27.000000 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/audio/en.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    55341 2023-05-30 18:08:27.000000 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/audio/es.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    57453 2023-05-30 18:08:27.000000 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/audio/fr.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    62637 2023-05-30 18:08:27.000000 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/audio/it.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    68781 2023-05-30 18:08:27.000000 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/audio/nl.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    48813 2023-05-30 18:08:27.000000 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/audio/pt.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)    67821 2023-05-30 18:08:27.000000 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/audio/uk.mp3
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-05-30 18:08:27.000000 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/gradio_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-30 18:08:27.000000 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:08:28.146126 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-30 18:08:28.000000 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-30 18:08:28.000000 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:08:28.000000 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-30 18:08:28.000000 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-30 18:08:28.000000 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-30 18:08:28.000000 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:08:28.000000 ovos-stt-http-server-0.0.2a6/ovos_stt_http_server.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 18:08:28.150126 ovos-stt-http-server-0.0.2a6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3049 2023-05-30 18:08:27.000000 ovos-stt-http-server-0.0.2a6/setup.py
```

### Comparing `ovos-stt-http-server-0.0.2a5/LICENSE.md` & `ovos-stt-http-server-0.0.2a6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a5/PKG-INFO` & `ovos-stt-http-server-0.0.2a6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-stt-http-server
-Version: 0.0.2a5
+Version: 0.0.2a6
 Summary: simple aiohttp server to host OpenVoiceOS stt plugins as a service
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-http-server
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: plugin STT OVOS OpenVoiceOS
 Platform: UNKNOWN
@@ -29,14 +29,31 @@
 
 Turn any OVOS STT plugin into a micro service!
 
 ## Install
 
 `pip install ovos-stt-http-server`
 
+## Companion plugin
+
+Use in your voice assistant with OpenVoiceOS [companion plugin](https://github.com/OpenVoiceOS/ovos-stt-server-plugin)
+
+## Configuration
+
+the plugin is configured just like if it was running in the assistant, under mycroft.conf
+
+eg
+```
+  "stt": {
+    "module": "ovos-stt-plugin-deepgram",
+    "ovos-stt-plugin-deepgram": {"key": "xtimes40"}
+  }
+```
+
+
 ## Usage
 
 ```bash
 ovos-stt-server --help
 usage: ovos-stt-server [-h] [--engine ENGINE] [--port PORT] [--host HOST]
 
 options:
@@ -49,17 +66,14 @@
   --cache                     flag to pre-cache examples in Gradio web UI
   --title TITLE               title for Gradio UI
   --description DESCRIPTION   Description for Gradio UI
   --info INFO                 Text to display in Gradio UI
   --badge BADGE               URL of badge to show in Gradio UI
 ```
 > Note: `ffmpeg` is required for Gradio
-## Companion plugin
-
-Use with OpenVoiceOS [companion plugin](https://github.com/OpenVoiceOS/ovos-stt-server-plugin)
 
 
 ## Docker
 
 you can create easily create a docker file to serve any plugin
 
 ```dockerfile
```

### Comparing `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/__init__.py` & `ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,14 +88,18 @@
     return audio
 
 
 def create_app(stt_plugin):
     app = FastAPI()
     model = ModelContainer(stt_plugin)
 
+    @app.get("/status")
+    def stats(request: Request):
+        return {"status": "ok", "plugin": stt_plugin}
+
     @app.post("/stt")
     async def get_stt(request: Request):
         LOG.debug(f"Handling STT Request: {request}")
         lang = str(request.query_params.get("lang", "en-us")).lower()
         audio_bytes = await request.body()
         LOG.debug(len(audio_bytes))
         audio = bytes2audiodata(audio_bytes)
```

### Comparing `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/__main__.py` & `ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/__main__.py`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/ca.mp3` & `ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/audio/ca.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/de.mp3` & `ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/audio/de.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/en.mp3` & `ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/audio/en.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/es.mp3` & `ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/audio/es.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/fr.mp3` & `ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/audio/fr.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/it.mp3` & `ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/audio/it.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/nl.mp3` & `ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/audio/nl.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/pt.mp3` & `ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/audio/pt.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/audio/uk.mp3` & `ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/audio/uk.mp3`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server/gradio_app.py` & `ovos-stt-http-server-0.0.2a6/ovos_stt_http_server/gradio_app.py`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server.egg-info/PKG-INFO` & `ovos-stt-http-server-0.0.2a6/ovos_stt_http_server.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-stt-http-server
-Version: 0.0.2a5
+Version: 0.0.2a6
 Summary: simple aiohttp server to host OpenVoiceOS stt plugins as a service
 Home-page: https://github.com/OpenVoiceOS/ovos-stt-http-server
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: plugin STT OVOS OpenVoiceOS
 Platform: UNKNOWN
@@ -29,14 +29,31 @@
 
 Turn any OVOS STT plugin into a micro service!
 
 ## Install
 
 `pip install ovos-stt-http-server`
 
+## Companion plugin
+
+Use in your voice assistant with OpenVoiceOS [companion plugin](https://github.com/OpenVoiceOS/ovos-stt-server-plugin)
+
+## Configuration
+
+the plugin is configured just like if it was running in the assistant, under mycroft.conf
+
+eg
+```
+  "stt": {
+    "module": "ovos-stt-plugin-deepgram",
+    "ovos-stt-plugin-deepgram": {"key": "xtimes40"}
+  }
+```
+
+
 ## Usage
 
 ```bash
 ovos-stt-server --help
 usage: ovos-stt-server [-h] [--engine ENGINE] [--port PORT] [--host HOST]
 
 options:
@@ -49,17 +66,14 @@
   --cache                     flag to pre-cache examples in Gradio web UI
   --title TITLE               title for Gradio UI
   --description DESCRIPTION   Description for Gradio UI
   --info INFO                 Text to display in Gradio UI
   --badge BADGE               URL of badge to show in Gradio UI
 ```
 > Note: `ffmpeg` is required for Gradio
-## Companion plugin
-
-Use with OpenVoiceOS [companion plugin](https://github.com/OpenVoiceOS/ovos-stt-server-plugin)
 
 
 ## Docker
 
 you can create easily create a docker file to serve any plugin
 
 ```dockerfile
```

### Comparing `ovos-stt-http-server-0.0.2a5/ovos_stt_http_server.egg-info/SOURCES.txt` & `ovos-stt-http-server-0.0.2a6/ovos_stt_http_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-stt-http-server-0.0.2a5/setup.py` & `ovos-stt-http-server-0.0.2a6/setup.py`

 * *Files identical despite different names*

