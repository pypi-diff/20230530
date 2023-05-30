# Comparing `tmp/yafti-0.6.1.tar.gz` & `tmp/yafti-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yafti-0.6.1.tar", max compression
+gzip compressed data, was "yafti-0.6.2.tar", max compression
```

## Comparing `yafti-0.6.1.tar` & `yafti-0.6.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11358 2023-04-17 01:36:39.158258 yafti-0.6.1/LICENSE
--rw-r--r--   0        0        0    10052 2023-04-17 01:36:39.158258 yafti-0.6.1/README.md
--rw-r--r--   0        0        0     1528 2023-04-17 01:36:39.158258 yafti-0.6.1/pyproject.toml
--rw-r--r--   0        0        0      560 2023-04-17 01:36:39.158258 yafti-0.6.1/yafti/__init__.py
--rw-r--r--   0        0        0     1087 2023-04-17 01:36:39.158258 yafti-0.6.1/yafti/__main__.py
--rw-r--r--   0        0        0     2081 2023-04-17 01:36:39.158258 yafti-0.6.1/yafti/abc.py
--rw-r--r--   0        0        0     1901 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/app.py
--rw-r--r--   0        0        0     1813 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/events.py
--rw-r--r--   0        0        0      532 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/log.py
--rw-r--r--   0        0        0     1571 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/parser.py
--rw-r--r--   0        0        0     6823 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/plugin/flatpak.py
--rw-r--r--   0        0        0     2760 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/plugin/run.py
--rw-r--r--   0        0        0      302 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/registry.py
--rw-r--r--   0        0        0     3278 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/consent.py
--rw-r--r--   0        0        0     2227 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/console.py
--rw-r--r--   0        0        0     1817 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/dialog.py
--rw-r--r--   0        0        0       50 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/package/__init__.py
--rw-r--r--   0        0        0      317 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/package/models.py
--rw-r--r--   0        0        0       98 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/package/screen/__init__.py
--rw-r--r--   0        0        0     5232 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/package/screen/install.py
--rw-r--r--   0        0        0     4021 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/package/screen/package.py
--rw-r--r--   0        0        0     5522 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/package/screen/picker.py
--rw-r--r--   0        0        0     1368 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/package/state.py
--rw-r--r--   0        0        0      509 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/package/utils.py
--rw-r--r--   0        0        0     3413 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/title.py
--rw-r--r--   0        0        0     1214 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/utils.py
--rw-r--r--   0        0        0     5216 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/screen/window.py
--rw-r--r--   0        0        0      448 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/setup.py
--rw-r--r--   0        0        0       32 2023-04-17 01:36:39.162258 yafti-0.6.1/yafti/share.py
--rw-r--r--   0        0        0    10952 1970-01-01 00:00:00.000000 yafti-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-30 13:34:16.949961 yafti-0.6.2/LICENSE
+-rw-r--r--   0        0        0    10051 2023-05-30 13:34:16.949961 yafti-0.6.2/README.md
+-rw-r--r--   0        0        0     1533 2023-05-30 13:34:16.949961 yafti-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0      560 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/__init__.py
+-rw-r--r--   0        0        0     1087 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/__main__.py
+-rw-r--r--   0        0        0     2081 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/abc.py
+-rw-r--r--   0        0        0     2455 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/app.py
+-rw-r--r--   0        0        0     1813 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/events.py
+-rw-r--r--   0        0        0      532 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/log.py
+-rw-r--r--   0        0        0     1571 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/parser.py
+-rw-r--r--   0        0        0     6823 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/plugin/flatpak.py
+-rw-r--r--   0        0        0     2760 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/plugin/run.py
+-rw-r--r--   0        0        0      302 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/registry.py
+-rw-r--r--   0        0        0     3278 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/consent.py
+-rw-r--r--   0        0        0     2227 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/console.py
+-rw-r--r--   0        0        0     1817 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/dialog.py
+-rw-r--r--   0        0        0       50 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/package/__init__.py
+-rw-r--r--   0        0        0      317 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/package/models.py
+-rw-r--r--   0        0        0       98 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/package/screen/__init__.py
+-rw-r--r--   0        0        0     5232 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/package/screen/install.py
+-rw-r--r--   0        0        0     4021 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/package/screen/package.py
+-rw-r--r--   0        0        0     5522 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/package/screen/picker.py
+-rw-r--r--   0        0        0     1368 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/package/state.py
+-rw-r--r--   0        0        0      509 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/package/utils.py
+-rw-r--r--   0        0        0     3413 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/title.py
+-rw-r--r--   0        0        0     1214 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/utils.py
+-rw-r--r--   0        0        0     5216 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/screen/window.py
+-rw-r--r--   0        0        0      448 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/setup.py
+-rw-r--r--   0        0        0       32 2023-05-30 13:34:16.949961 yafti-0.6.2/yafti/share.py
+-rw-r--r--   0        0        0    10948 1970-01-01 00:00:00.000000 yafti-0.6.2/PKG-INFO
```

### Comparing `yafti-0.6.1/LICENSE` & `yafti-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yafti-0.6.1/README.md` & `yafti-0.6.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
 
 ### Configuration
 
 ```yaml
 title: uBlue First Boot
 properties:
   mode: "run-on-change"
-  path: "~/.config/yafti-first-run"
+  path: "~/.config/yafti/last-run"
 actions:
   pre:
   - run: /full/path/to/bin --with --params
   - run: /another/command run
   - yafti.plugin.flatpak:
       install: org.gnome.Calculator
   post:
```

### Comparing `yafti-0.6.1/pyproject.toml` & `yafti-0.6.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "yafti"
-version = "0.6.1"
+version = "0.6.2"
 description = "Yet another first time installer"
 authors = ["Marco Ceppi <marco@ceppi.net>"]
 license = "Apache 2.0"
 readme = "README.md"
 homepage = "https://github.com/ublue-os/yafti"
 repository = "https://github.com/ublue-os/yafti"
 classifiers = [
@@ -20,15 +20,15 @@
 [tool.poetry.dependencies]
 python = "^3.11"
 pydantic = "1.10.2"  # This needs to match the minimum supported version in Fedora
 pygobject = "^3.42.2"
 pyyaml = "^6.0"
 gbulb = "^0.6.4"
 rich = "^13.3.2"
-typer = "^0.7.0"
+typer = ">=0.7,<0.10"
 
 [tool.poetry.plugins."yafti.plugin"]
 "yafti.plugin.flatpak" = "yafti.plugin.flatpak:Flatpak"
 "yafti.plugin.run" = "yafti.plugin.run:Run"
 "run" = "yafti.plugin.run:Run"
 
 [tool.poetry.plugins."yafti.screen"]
@@ -37,15 +37,15 @@
 "yafti.screen.console" = "yafti.screen.console:ConsoleScreen"
 "yafti.screen.consent" = "yafti.screen.consent:ConsentScreen"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 isort = "^5.12.0"
 pytest = "^7.2.1"
-ruff = ">=0.0.254,<0.0.262"
+ruff = ">=0.0.254,<0.0.271"
 coverage = "^7.2.1"
 pytest-cov = "^4.0.0"
 pytest-asyncio = ">=0.20.3,<0.22.0"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
```

### Comparing `yafti-0.6.1/yafti/__init__.py` & `yafti-0.6.2/yafti/__init__.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.1/yafti/__main__.py` & `yafti-0.6.2/yafti/__main__.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.1/yafti/abc.py` & `yafti-0.6.2/yafti/abc.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.1/yafti/app.py` & `yafti-0.6.2/yafti/app.py`

 * *Files 13% similar despite different names*

```diff
@@ -15,28 +15,38 @@
 """
 
 import hashlib
 
 import gbulb
 import yaml
 from gi.repository import Adw
+from pathlib import Path
 
 from yafti.parser import Config, YaftiRunModes
 from yafti.screen.window import Window
 
 
 class Yafti(Adw.Application):
     def __init__(self, cfg: Config = None, loop=None):
         super().__init__(application_id="it.ublue.Yafti")
         self.config = cfg
         self.loop = loop or gbulb.get_event_loop()
 
     def run(self, *args, **kwargs):
         configured_mode = self.config.properties.mode
-        _p = self.config.properties.path.expanduser()
+        _p: Path = self.config.properties.path.expanduser()
+        # TODO(GH-#103): Remove this prior to 1.0 release. Start.
+        _old_p = Path("~/.config/yafti-last-run").expanduser()
+        if _old_p.exists() and _old_p.resolve() != _p.resolve():
+            if not _p.parent.is_dir():
+                _p.parent.mkdir(mode=0o755, parents=True, exist_ok=True)
+            if _p.is_file():
+                _p.unlink()
+            _old_p.rename(_p)
+        # TODO(GH-#103): End.
         if configured_mode == YaftiRunModes.disable:
             return
 
         if configured_mode == YaftiRunModes.changed:
             if _p.exists() and _p.read_text() == self.config_sha:
                 return
 
@@ -50,15 +60,17 @@
         win.present()
         self.loop.run()
 
     @property
     def config_sha(self):
         return hashlib.sha256(yaml.dump(self.config.dict()).encode()).hexdigest()
 
-    def sync_first_run(self):
+    def sync_last_run(self):
         p = self.config.properties.path.expanduser()
+        if not p.parent.is_dir():
+            p.parent.mkdir(mode=0o755, parents=True, exist_ok=True)
         p.write_text(self.config_sha)
 
     def quit(self, *args, **kwargs):
         self.loop.stop()
-        self.sync_first_run()
+        self.sync_last_run()
         super().quit()
```

### Comparing `yafti-0.6.1/yafti/events.py` & `yafti-0.6.2/yafti/events.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.1/yafti/log.py` & `yafti-0.6.2/yafti/log.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.1/yafti/parser.py` & `yafti-0.6.2/yafti/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 class YaftiRunModes(str, Enum):
     changed = "run-on-change"
     ignore = "run-once"
     disable = "disabled"
 
 
 class YaftiProperties(BaseModel):
-    path: Optional[Path] = Path("~/.config/yafti-last-run")
+    path: Optional[Path] = Path("~/.config/yafti/last-run")
     mode: YaftiRunModes = YaftiRunModes.changed
 
 
 class Config(BaseModel):
     title: str
     properties: YaftiProperties = YaftiProperties()
     actions: Optional[ActionConfig]
```

### Comparing `yafti-0.6.1/yafti/plugin/flatpak.py` & `yafti-0.6.2/yafti/plugin/flatpak.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.1/yafti/plugin/run.py` & `yafti-0.6.2/yafti/plugin/run.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.1/yafti/screen/consent.py` & `yafti-0.6.2/yafti/screen/consent.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.1/yafti/screen/console.py` & `yafti-0.6.2/yafti/screen/console.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.1/yafti/screen/dialog.py` & `yafti-0.6.2/yafti/screen/dialog.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.1/yafti/screen/package/screen/install.py` & `yafti-0.6.2/yafti/screen/package/screen/install.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.1/yafti/screen/package/screen/package.py` & `yafti-0.6.2/yafti/screen/package/screen/package.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.1/yafti/screen/package/screen/picker.py` & `yafti-0.6.2/yafti/screen/package/screen/picker.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.1/yafti/screen/package/state.py` & `yafti-0.6.2/yafti/screen/package/state.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.1/yafti/screen/title.py` & `yafti-0.6.2/yafti/screen/title.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.1/yafti/screen/utils.py` & `yafti-0.6.2/yafti/screen/utils.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.1/yafti/screen/window.py` & `yafti-0.6.2/yafti/screen/window.py`

 * *Files identical despite different names*

### Comparing `yafti-0.6.1/PKG-INFO` & `yafti-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yafti
-Version: 0.6.1
+Version: 0.6.2
 Summary: Yet another first time installer
 Home-page: https://github.com/ublue-os/yafti
 License: Apache 2.0
 Author: Marco Ceppi
 Author-email: marco@ceppi.net
 Requires-Python: >=3.11,<4.0
 Classifier: Environment :: X11 Applications :: GTK
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Software Distribution
 Requires-Dist: gbulb (>=0.6.4,<0.7.0)
 Requires-Dist: pydantic (==1.10.2)
 Requires-Dist: pygobject (>=3.42.2,<4.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: rich (>=13.3.2,<14.0.0)
-Requires-Dist: typer (>=0.7.0,<0.8.0)
+Requires-Dist: typer (>=0.7,<0.10)
 Project-URL: Repository, https://github.com/ublue-os/yafti
 Description-Content-Type: text/markdown
 
 # Yet Another First Time Installer
 
 This application is responsible for installing Flatpaks on first boot after a user finishes installation. 
 It is intended as a replacement for custom zenity dialogs. 
@@ -82,15 +82,15 @@
 
 ### Configuration
 
 ```yaml
 title: uBlue First Boot
 properties:
   mode: "run-on-change"
-  path: "~/.config/yafti-first-run"
+  path: "~/.config/yafti/last-run"
 actions:
   pre:
   - run: /full/path/to/bin --with --params
   - run: /another/command run
   - yafti.plugin.flatpak:
       install: org.gnome.Calculator
   post:
```

