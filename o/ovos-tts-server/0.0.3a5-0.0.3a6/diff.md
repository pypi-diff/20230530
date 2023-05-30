# Comparing `tmp/ovos-tts-server-0.0.3a5.tar.gz` & `tmp/ovos-tts-server-0.0.3a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-tts-server-0.0.3a5.tar", last modified: Fri May  5 17:06:07 2023, max compression
+gzip compressed data, was "ovos-tts-server-0.0.3a6.tar", last modified: Tue May 30 18:08:34 2023, max compression
```

## Comparing `ovos-tts-server-0.0.3a5.tar` & `ovos-tts-server-0.0.3a6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:07.815004 ovos-tts-server-0.0.3a5/
--rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-05 17:06:07.000000 ovos-tts-server-0.0.3a5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-05 17:06:07.815004 ovos-tts-server-0.0.3a5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:07.815004 ovos-tts-server-0.0.3a5/ovos_tts_server/
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-05 17:06:07.000000 ovos-tts-server-0.0.3a5/ovos_tts_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-05 17:06:07.000000 ovos-tts-server-0.0.3a5/ovos_tts_server/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:07.815004 ovos-tts-server-0.0.3a5/ovos_tts_server/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-05 17:06:07.000000 ovos-tts-server-0.0.3a5/ovos_tts_server/examples/rainbow.json
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-05 17:06:07.000000 ovos-tts-server-0.0.3a5/ovos_tts_server/gradio_app.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-05 17:06:07.000000 ovos-tts-server-0.0.3a5/ovos_tts_server/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:07.815004 ovos-tts-server-0.0.3a5/ovos_tts_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-05 17:06:07.000000 ovos-tts-server-0.0.3a5/ovos_tts_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-05 17:06:07.000000 ovos-tts-server-0.0.3a5/ovos_tts_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:06:07.000000 ovos-tts-server-0.0.3a5/ovos_tts_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-05 17:06:07.000000 ovos-tts-server-0.0.3a5/ovos_tts_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-05 17:06:07.000000 ovos-tts-server-0.0.3a5/ovos_tts_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:06:07.000000 ovos-tts-server-0.0.3a5/ovos_tts_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:06:07.000000 ovos-tts-server-0.0.3a5/ovos_tts_server.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:06:07.815004 ovos-tts-server-0.0.3a5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3054 2023-05-05 17:06:07.000000 ovos-tts-server-0.0.3a5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:08:34.602711 ovos-tts-server-0.0.3a6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11347 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-30 18:08:34.602711 ovos-tts-server-0.0.3a6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:08:34.602711 ovos-tts-server-0.0.3a6/ovos_tts_server/
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:08:34.602711 ovos-tts-server-0.0.3a6/ovos_tts_server/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server/examples/rainbow.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server/gradio_app.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 18:08:34.602711 ovos-tts-server-0.0.3a6/ovos_tts_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/ovos_tts_server.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 18:08:34.602711 ovos-tts-server-0.0.3a6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3054 2023-05-30 18:08:34.000000 ovos-tts-server-0.0.3a6/setup.py
```

### Comparing `ovos-tts-server-0.0.3a5/LICENSE.md` & `ovos-tts-server-0.0.3a6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ovos-tts-server-0.0.3a5/PKG-INFO` & `ovos-tts-server-0.0.3a6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-server
-Version: 0.0.3a5
+Version: 0.0.3a6
 Summary: simple FastAPI server to host TTS plugins as a service
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-server
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: plugin TTS OVOS OpenVoiceOS
 Platform: UNKNOWN
@@ -25,20 +25,37 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # OpenVoiceOS TTS Server
 
 Turn any OVOS TTS plugin into a micro service!
 
-Use with OpenVoiceOS [companion plugin](https://github.com/OpenVoiceOS/ovos-tts-server-plugin)
 
 ## Install
 
 `pip install ovos-tts-server`
 
+## Companion plugin
+
+Use in your voice assistant with OpenVoiceOS [companion plugin](https://github.com/OpenVoiceOS/ovos-tts-server-plugin)
+
+## Configuration
+
+the plugin is configured just like if it was running in the assistant, under mycroft.conf
+
+eg
+```
+ "tts": {
+    "module": "ovos-tts-plugin-piper",
+    "ovos-tts-plugin-piper": {
+      "model": "alan-low"
+    }
+  }
+```
+
 ## Usage
 
 ```bash
 ovos-tts-server --help
 usage: ovos-tts-server [-h] [--engine ENGINE] [--port PORT] [--host HOST] [--cache]
 
 options:
@@ -49,17 +66,14 @@
   --cache          save every synth to disk
 ```
 
 eg, to use the [GladosTTS plugin](https://github.com/NeonGeckoCom/neon-tts-plugin-glados) `ovos-tts-server --engine neon-tts-plugin-glados --cache`
 
 then do a get request `http://192.168.1.112:9666/synthesize/hello`
 
-## Companion plugin
-
-coming soon - companion plugin to point to a ovos-tts-server instance
 
 ## Docker
 
 you can create easily crete a docker file to serve any plugin
 
 ```dockerfile
 FROM python:3.7
```

### Comparing `ovos-tts-server-0.0.3a5/ovos_tts_server/__init__.py` & `ovos-tts-server-0.0.3a6/ovos_tts_server/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,45 +5,46 @@
 #    http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-import uvicorn
-
 from fastapi import FastAPI
 from fastapi.responses import FileResponse
 from ovos_plugin_manager.tts import load_tts_plugin
 from ovos_utils.log import LOG
 from starlette.requests import Request
 
 TTS = None
 
 
-def create_app():
+def create_app(tts_plugin):
     app = FastAPI()
 
+    @app.get("/status")
+    def stats(request: Request):
+        return {"status": "ok", "plugin": tts_plugin}
+
     @app.get("/synthesize/{utterance}")
     def synth(utterance: str, request: Request):
         LOG.debug(f"{utterance}|{request.query_params}")
         utterance = TTS.validate_ssml(utterance)
         audio, phonemes = TTS.synth(utterance, **request.query_params)
         return FileResponse(audio.path)
 
     return app
 
 
-def start_tts_server(engine, cache=False):
+def start_tts_server(tts_plugin, cache=False):
     global TTS
 
     # load ovos TTS plugin
-    engine = load_tts_plugin(engine)
+    engine = load_tts_plugin(tts_plugin)
 
     TTS = engine(config={"persist_cache": cache})  # this will cache every synth even across reboots
     TTS.log_timestamps = True  # enable logging
 
-    app = create_app()
+    app = create_app(tts_plugin)
     return app, TTS
```

### Comparing `ovos-tts-server-0.0.3a5/ovos_tts_server/__main__.py` & `ovos-tts-server-0.0.3a6/ovos_tts_server/__main__.py`

 * *Files identical despite different names*

### Comparing `ovos-tts-server-0.0.3a5/ovos_tts_server/examples/rainbow.json` & `ovos-tts-server-0.0.3a6/ovos_tts_server/examples/rainbow.json`

 * *Files identical despite different names*

### Comparing `ovos-tts-server-0.0.3a5/ovos_tts_server/gradio_app.py` & `ovos-tts-server-0.0.3a6/ovos_tts_server/gradio_app.py`

 * *Files identical despite different names*

### Comparing `ovos-tts-server-0.0.3a5/ovos_tts_server.egg-info/PKG-INFO` & `ovos-tts-server-0.0.3a6/ovos_tts_server.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-tts-server
-Version: 0.0.3a5
+Version: 0.0.3a6
 Summary: simple FastAPI server to host TTS plugins as a service
 Home-page: https://github.com/OpenVoiceOS/ovos-tts-server
 Author: JarbasAi
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Keywords: plugin TTS OVOS OpenVoiceOS
 Platform: UNKNOWN
@@ -25,20 +25,37 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # OpenVoiceOS TTS Server
 
 Turn any OVOS TTS plugin into a micro service!
 
-Use with OpenVoiceOS [companion plugin](https://github.com/OpenVoiceOS/ovos-tts-server-plugin)
 
 ## Install
 
 `pip install ovos-tts-server`
 
+## Companion plugin
+
+Use in your voice assistant with OpenVoiceOS [companion plugin](https://github.com/OpenVoiceOS/ovos-tts-server-plugin)
+
+## Configuration
+
+the plugin is configured just like if it was running in the assistant, under mycroft.conf
+
+eg
+```
+ "tts": {
+    "module": "ovos-tts-plugin-piper",
+    "ovos-tts-plugin-piper": {
+      "model": "alan-low"
+    }
+  }
+```
+
 ## Usage
 
 ```bash
 ovos-tts-server --help
 usage: ovos-tts-server [-h] [--engine ENGINE] [--port PORT] [--host HOST] [--cache]
 
 options:
@@ -49,17 +66,14 @@
   --cache          save every synth to disk
 ```
 
 eg, to use the [GladosTTS plugin](https://github.com/NeonGeckoCom/neon-tts-plugin-glados) `ovos-tts-server --engine neon-tts-plugin-glados --cache`
 
 then do a get request `http://192.168.1.112:9666/synthesize/hello`
 
-## Companion plugin
-
-coming soon - companion plugin to point to a ovos-tts-server instance
 
 ## Docker
 
 you can create easily crete a docker file to serve any plugin
 
 ```dockerfile
 FROM python:3.7
```

### Comparing `ovos-tts-server-0.0.3a5/setup.py` & `ovos-tts-server-0.0.3a6/setup.py`

 * *Files identical despite different names*

