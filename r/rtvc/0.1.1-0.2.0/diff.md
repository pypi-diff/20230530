# Comparing `tmp/rtvc-0.1.1.tar.gz` & `tmp/rtvc-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rtvc-0.1.1.tar", last modified: Sat May 27 01:13:14 2023, max compression
+gzip compressed data, was "rtvc-0.2.0.tar", last modified: Tue May 30 04:52:43 2023, max compression
```

## Comparing `rtvc-0.1.1.tar` & `rtvc-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,19 @@
--rw-r--r--   0        0        0     1064 2023-05-26 07:34:56.775946 rtvc-0.1.1/LICENSE
--rw-r--r--   0        0        0      562 2023-05-26 23:59:00.302765 rtvc-0.1.1/README.md
--rw-r--r--   0        0        0     1437 2023-05-27 01:13:14.865999 rtvc-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-26 04:45:22.845379 rtvc-0.1.1/rtvc/__init__.py
--rw-r--r--   0        0        0      437 2023-05-26 06:43:47.085759 rtvc-0.1.1/rtvc/__main__.py
--rw-r--r--   0        0        0   156997 2023-05-27 00:05:53.762257 rtvc-0.1.1/rtvc/assets/icon.png
--rw-r--r--   0        0        0      734 2023-05-26 23:42:03.016172 rtvc-0.1.1/rtvc/audio.py
--rw-r--r--   0        0        0     1950 2023-05-27 00:37:54.402972 rtvc-0.1.1/rtvc/config.py
--rw-r--r--   0        0        0    18721 2023-05-27 00:37:54.410808 rtvc-0.1.1/rtvc/gui.py
--rw-r--r--   0        0        0      907 2023-05-27 00:37:54.405152 rtvc-0.1.1/rtvc/i18n.py
--rw-r--r--   0        0        0      977 2023-05-26 23:46:36.062919 rtvc-0.1.1/rtvc/locales/en_US.yaml
--rw-r--r--   0        0        0      941 2023-05-26 23:46:45.823224 rtvc-0.1.1/rtvc/locales/zh_CN.yaml
--rw-r--r--   0        0        0     1249 2023-05-26 23:41:55.884670 rtvc-0.1.1/tests/test_sola.py
--rw-r--r--   0        0        0     1164 1970-01-01 00:00:00.000000 rtvc-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-30 04:51:27.646554 rtvc-0.2.0/LICENSE
+-rw-r--r--   0        0        0      562 2023-05-30 04:51:27.646554 rtvc-0.2.0/README.md
+-rw-r--r--   0        0        0     1459 2023-05-30 04:52:43.251318 rtvc-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-30 04:51:27.646554 rtvc-0.2.0/rtvc/__init__.py
+-rw-r--r--   0        0        0      437 2023-05-30 04:51:27.646554 rtvc-0.2.0/rtvc/__main__.py
+-rw-r--r--   0        0        0   156997 2023-05-30 04:51:27.646554 rtvc-0.2.0/rtvc/assets/icon.png
+-rw-r--r--   0        0        0      734 2023-05-30 04:51:27.646554 rtvc-0.2.0/rtvc/audio.py
+-rw-r--r--   0        0        0     2354 2023-05-30 04:51:27.646554 rtvc-0.2.0/rtvc/config.py
+-rw-r--r--   0        0        0    23997 2023-05-30 04:51:27.646554 rtvc-0.2.0/rtvc/gui.py
+-rw-r--r--   0        0        0      907 2023-05-30 04:51:27.646554 rtvc-0.2.0/rtvc/i18n.py
+-rw-r--r--   0        0        0     2396 2023-05-30 04:51:27.646554 rtvc-0.2.0/rtvc/locales/en_US.yaml
+-rw-r--r--   0        0        0     2191 2023-05-30 04:51:27.646554 rtvc-0.2.0/rtvc/locales/zh_CN.yaml
+-rw-r--r--   0        0        0      220 2023-05-30 04:51:27.646554 rtvc-0.2.0/rtvc/plugins/__init__.py
+-rw-r--r--   0        0        0     4431 2023-05-30 04:51:27.646554 rtvc-0.2.0/rtvc/plugins/base.py
+-rw-r--r--   0        0        0      417 2023-05-30 04:51:27.646554 rtvc-0.2.0/rtvc/plugins/diffusion.py
+-rw-r--r--   0        0        0      200 2023-05-30 04:51:27.646554 rtvc-0.2.0/rtvc/plugins/hifisinger.py
+-rw-r--r--   0        0        0      237 2023-05-30 04:51:27.646554 rtvc-0.2.0/rtvc/plugins/rvc.py
+-rw-r--r--   0        0        0     1249 2023-05-30 04:51:27.646554 rtvc-0.2.0/tests/test_sola.py
+-rw-r--r--   0        0        0     1194 1970-01-01 00:00:00.000000 rtvc-0.2.0/PKG-INFO
```

### Comparing `rtvc-0.1.1/LICENSE` & `rtvc-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rtvc-0.1.1/README.md` & `rtvc-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `rtvc-0.1.1/pyproject.toml` & `rtvc-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "rtvc"
-version = "0.1.1"
+version = "0.2.0"
 description = "Real-Time Voice Conversion GUI"
 readme = "README.md"
 requires-python = ">=3.10,<3.12"
 keywords = [
     "voice-conversion",
     "svc",
 ]
@@ -18,14 +18,15 @@
 dependencies = [
     "noisereduce>=2.0.1",
     "sounddevice>=0.4.6",
     "pyyaml>=6.0",
     "PyQt6>=6.5.0",
     "pyqtdarktheme==2.1.0",
     "requests>=2.31.0",
+    "librosa==0.9.2",
 ]
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 repository = "https://github.com/fishaudio/realtime-vc-gui"
```

### Comparing `rtvc-0.1.1/rtvc/assets/icon.png` & `rtvc-0.2.0/rtvc/assets/icon.png`

 * *Files identical despite different names*

### Comparing `rtvc-0.1.1/rtvc/audio.py` & `rtvc-0.2.0/rtvc/audio.py`

 * *Files identical despite different names*

### Comparing `rtvc-0.1.1/rtvc/config.py` & `rtvc-0.2.0/rtvc/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import locale
 import sys
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Literal
 
 import yaml
 
 if getattr(sys, "frozen", False):
     # If the application is run as a bundle, the PyInstaller bootloader
@@ -31,14 +31,18 @@
     extra_duration: int = 50
     input_denoise: bool = False
     output_denoise: bool = False
     sample_rate: int = 44100
     sola_search_duration: int = 12
     buffer_num: int = 4
 
+    # Plugins
+    current_plugin: str | None = None
+    plugins: dict[str, dict] = field(default_factory=dict)
+
     @property
     def sample_frames(self):
         return self.sample_duration * self.sample_rate // 1000
 
     @property
     def fade_frames(self):
         return self.fade_duration * self.sample_rate // 1000
@@ -48,32 +52,40 @@
         return self.extra_duration * self.sample_rate // 1000
 
     @property
     def sola_search_frames(self):
         return self.sola_search_duration * self.sample_rate // 1000
 
 
-config_path = Path.home() / ".rtvc" / "config.yaml"
+default_config_path = str((Path.home() / ".rtvc" / "config.yaml").absolute())
 config = Config()
 
 
-def load_config():
+def load_config(path: Path | str = default_config_path) -> Config:
     global config
 
-    if config_path.exists():
-        with open(config_path, "r", encoding="utf-8") as f:
-            config = Config(**yaml.safe_load(f.read()))
+    path = Path(path)
+
+    if path.exists():
+        try:
+            with open(path, "r", encoding="utf-8") as f:
+                config = Config(**yaml.safe_load(f.read()))
+        except Exception:
+            config = Config()
+            print("Failed to load config file, use default config instead.")
 
     return config
 
 
-def save_config():
-    if not config_path.parent.exists():
-        config_path.parent.mkdir(parents=True)
+def save_config(path: Path | str = default_config_path) -> None:
+    path = Path(path)
+
+    if not path.parent.exists():
+        path.parent.mkdir(parents=True)
 
-    with open(config_path, "w", encoding="utf-8") as f:
+    with open(path, "w", encoding="utf-8") as f:
         yaml.safe_dump(config.__dict__, f)
 
 
 # Auto load config
 load_config()
 save_config()
```

### Comparing `rtvc-0.1.1/rtvc/gui.py` & `rtvc-0.2.0/rtvc/gui.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,84 @@
 import os
 import queue
 import sys
 import threading
 import time
 from io import BytesIO
-from pathlib import Path
 
 import librosa
 import noisereduce as nr
 import numpy as np
 import pkg_resources
 import qdarktheme
 import requests
 import sounddevice as sd
 import soundfile as sf
 from PyQt6.QtCore import Qt
 from PyQt6.QtGui import QIcon
 from PyQt6.QtWidgets import (
     QCheckBox,
     QComboBox,
+    QFileDialog,
     QGridLayout,
     QGroupBox,
     QHBoxLayout,
     QLabel,
     QLineEdit,
     QMessageBox,
     QPushButton,
     QSlider,
     QVBoxLayout,
     QWidget,
 )
 from scipy.signal import convolve
 
 from rtvc.audio import get_devices
-from rtvc.config import application_path, config, save_config
+from rtvc.config import application_path, config, load_config, save_config
 from rtvc.i18n import _t, language_map
+from rtvc.plugins import ALL_PLUGINS
+from rtvc.plugins.base import render_plugin
 
 
 class MainWindow(QWidget):
     def __init__(self):
         super().__init__()
 
         self.setWindowIcon(QIcon(str(application_path / "assets" / "icon.png")))
 
-        self.setMinimumWidth(800)
-
         version = pkg_resources.get_distribution("rtvc").version
+        # remove +editable if it exists
+        version = version.split("+")[0]
         self.setWindowTitle(_t("title").format(version=version))
 
         self.main_layout = QVBoxLayout()
         # Stick to the top
         self.main_layout.setAlignment(Qt.AlignmentFlag.AlignTop)
 
         self.setup_ui_settings()
+        self.setup_backend_settings()
         self.setup_device_settings()
         self.setup_audio_settings()
+        self.plugin_layout = QGroupBox()
+        self.main_layout.addWidget(self.plugin_layout)
+        self.setup_plugin_settings()
         self.setup_action_buttons()
-
         self.setLayout(self.main_layout)
 
+        # Use size hint to set a reasonable size
+        self.setMinimumWidth(900)
+
         # Voice Conversion Thread
         self.thread = None
         self.vc_status = threading.Event()
 
     def setup_ui_settings(self):
         # we have language and backend settings in the first row
         row = QHBoxLayout()
+        row.setAlignment(Qt.AlignmentFlag.AlignLeft)
 
         # set up a theme combo box
         row.addWidget(QLabel(_t("theme.name")))
         self.theme_combo = QComboBox()
         self.theme_combo.addItem(_t("theme.auto"), "auto")
         self.theme_combo.addItem(_t("theme.light"), "light")
         self.theme_combo.addItem(_t("theme.dark"), "dark")
@@ -86,23 +95,41 @@
             self.language_combo.addItem(v, k)
 
         self.language_combo.setCurrentText(language_map[config.locale])
         self.language_combo.currentIndexChanged.connect(self.change_language)
         self.language_combo.setMinimumWidth(150)
         row.addWidget(self.language_combo)
 
-        # set up backend (url) input, and a test button
-        row.addWidget(QLabel(_t("backend.name")))
-        self.backend_input = QLineEdit()
-        self.backend_input.setText(config.backend)
-        row.addWidget(self.backend_input)
+        # setup plugin combo box
+        row.addWidget(QLabel(_t("plugins.name")))
+        self.plugin_combo = QComboBox()
+        self.plugin_combo.addItem(_t("plugins.none.name"), "none")
+        for plugin in ALL_PLUGINS:
+            self.plugin_combo.addItem(_t(f"plugins.{plugin.id}.name"), plugin.id)
+
+        if config.current_plugin is not None:
+            self.plugin_combo.setCurrentText(
+                _t(f"plugins.{config.current_plugin}.name")
+            )
+        else:
+            self.plugin_combo.setCurrentText(_t("plugins.none.name"))
 
-        self.test_button = QPushButton(_t("backend.test"))
-        self.test_button.clicked.connect(self.test_backend)
-        row.addWidget(self.test_button)
+        self.plugin_combo.currentIndexChanged.connect(self.change_plugin)
+        self.plugin_combo.setMinimumWidth(150)
+        row.addWidget(self.plugin_combo)
+
+        # save button
+        self.save_button = QPushButton(_t("config.save"))
+        self.save_button.clicked.connect(self.save_config)
+        row.addWidget(self.save_button)
+
+        # load button
+        self.load_button = QPushButton(_t("config.load"))
+        self.load_button.clicked.connect(self.load_config)
+        row.addWidget(self.load_button)
 
         self.main_layout.addLayout(row)
 
     def setup_device_settings(self):
         # second row: a group box for audio device settings
         row = QGroupBox(_t("audio_device.name"))
         row_layout = QGridLayout()
@@ -248,19 +275,72 @@
         self.output_denoise_checkbox.setText(_t("audio.output_denoise"))
         self.output_denoise_checkbox.setChecked(config.output_denoise)
         row_layout.addWidget(self.output_denoise_checkbox, 2, 4)
 
         row.setLayout(row_layout)
         self.main_layout.addWidget(row)
 
+    def setup_backend_settings(self):
+        widget = QGroupBox()
+        widget.setTitle(_t("backend.title"))
+        row = QHBoxLayout()
+
+        # protocol
+        row.addWidget(QLabel(_t("backend.protocol_label")))
+        self.backend_protocol = QComboBox()
+        self.backend_protocol.setMinimumWidth(75)
+        self.backend_protocol.addItems(["v1"])
+        self.backend_protocol.setCurrentText("v1")
+        row.addWidget(self.backend_protocol)
+
+        # set up backend (url) input, and a test button
+        row.addWidget(QLabel(_t("backend.name")))
+        self.backend_input = QLineEdit()
+        self.backend_input.setText(config.backend)
+        row.addWidget(self.backend_input)
+
+        self.test_button = QPushButton(_t("backend.test"))
+        self.test_button.clicked.connect(self.test_backend)
+        row.addWidget(self.test_button)
+
+        widget.setLayout(row)
+        self.main_layout.addWidget(widget)
+
+    def setup_plugin_settings(self):
+        plugin_id = config.current_plugin
+
+        if plugin_id is None:
+            self.get_plugin_config = lambda: dict()
+            self.plugin_key_mapping = dict()
+            self.plugin_layout.hide()
+            return
+
+        self.plugin_layout.show()
+        self.plugin_layout.setTitle(_t(f"plugins.{plugin_id}.name"))
+
+        if self.plugin_layout.layout():
+            # remove the old layout
+            QWidget().setLayout(self.plugin_layout.layout())
+
+        # Find the plugin class from the config
+        for plugin_cls in ALL_PLUGINS:
+            if plugin_cls.id != plugin_id:
+                continue
+
+            layout, get_value_func, key_mappping = render_plugin(plugin_cls)
+            self.get_plugin_config = get_value_func
+            self.plugin_key_mapping = key_mappping
+            self.plugin_layout.setLayout(layout)
+
+        # resize the window to fit the new layout
+        self.resize(self.sizeHint())
+
     def setup_action_buttons(self):
         row = QWidget()
         row_layout = QHBoxLayout()
-        # row_layout.setAlignment(Qt.AlignmentFlag.Alig)
-        # stick to bottom
         row_layout.addStretch(1)
 
         self.start_button = QPushButton(_t("action.start"))
         self.start_button.clicked.connect(self.start_conversion)
         row_layout.addWidget(self.start_button)
 
         self.stop_button = QPushButton(_t("action.stop"))
@@ -293,14 +373,21 @@
         )
         msg_box.setDefaultButton(QMessageBox.StandardButton.No)
         ret = msg_box.exec()
 
         if ret == QMessageBox.StandardButton.Yes:
             os.execv(sys.argv[0], sys.argv)
 
+    def change_plugin(self, index):
+        config.current_plugin = self.plugin_combo.itemData(index)
+        if config.current_plugin == "none":
+            config.current_plugin = None
+
+        self.setup_plugin_settings()
+
     def test_backend(self):
         backend = self.backend_input.text()
 
         try:
             response = requests.options(backend, timeout=5)
         except:
             response = None
@@ -314,28 +401,78 @@
             save_config()
         else:
             message_box.setIcon(QMessageBox.Icon.Question)
             message_box.setText(_t("backend.test_failed"))
 
         message_box.exec()
 
-    def start_conversion(self):
+    def save_config(self, save_to_file=True):
         config.backend = self.backend_input.text()
         config.input_device = self.input_device_combo.currentData()
         config.output_device = self.output_device_combo.currentData()
         config.db_threshold = self.db_threshold_slider.value()
         config.pitch_shift = self.pitch_shift_slider.value()
         config.sample_duration = self.sample_duration_slider.value()
         config.fade_duration = self.fade_duration_slider.value()
         config.extra_duration = self.extra_duration_slider.value()
         config.input_denoise = self.input_denoise_checkbox.isChecked()
         config.output_denoise = self.output_denoise_checkbox.isChecked()
+        config.plugins[config.current_plugin] = self.get_plugin_config()
+
+        save_config()
+
+        # pop up a message box to tell user if they want to save the config to a file
+        if not save_to_file:
+            return
+
+        msg_box = QMessageBox()
+        msg_box.setIcon(QMessageBox.Icon.Question)
+        msg_box.setText(_t("config.save_msg"))
+        msg_box.setStandardButtons(
+            QMessageBox.StandardButton.Yes | QMessageBox.StandardButton.No
+        )
+        msg_box.setDefaultButton(QMessageBox.StandardButton.No)
+
+        ret = msg_box.exec()
+        if ret == QMessageBox.StandardButton.No:
+            return
+
+        file_name, _ = QFileDialog.getSaveFileName(
+            self, _t("config.save_title"), "", "YAML (*.yaml)"
+        )
 
+        if not file_name:
+            return
+
+        save_config(file_name)
+
+    def load_config(self):
+        # pop up a message box to select a config file
+        file_name, _ = QFileDialog.getOpenFileName(
+            self, _t("config.load_title"), "", "YAML (*.yaml)"
+        )
+
+        if not file_name:
+            return
+
+        load_config(file_name)
         save_config()
 
+        # pop up a message box to tell user app will restart
+        msg_box = QMessageBox()
+        msg_box.setIcon(QMessageBox.Icon.Information)
+        msg_box.setText(_t("config.load_msg"))
+        msg_box.setStandardButtons(QMessageBox.StandardButton.Ok)
+        msg_box.exec()
+
+        os.execv(sys.argv[0], sys.argv)
+
+    def start_conversion(self):
+        self.save_config(save_to_file=False)
+
         self.start_button.setEnabled(False)
         self.stop_button.setEnabled(True)
 
         # Create windows and buffers
         self.input_wav = np.zeros(
             (
                 config.sample_frames
@@ -437,25 +574,42 @@
             ]
         )
 
         buffer = BytesIO()
         sf.write(buffer, self.input_wav, config.sample_rate, format="wav")
         buffer.seek(0)
 
+        safe_pad_length = (
+            config.extra_frames - config.fade_frames
+        ) / config.sample_rate - 0.03
+        safe_pad_length = max(0, safe_pad_length)
+
+        data = {
+            "fSafePrefixPadLength": str(safe_pad_length),
+            "fPitchChange": str(config.pitch_shift),
+            "sampleRate": str(config.sample_rate),
+        }
+
+        # Override plugin settings, and apply key mapping
+        if (
+            config.current_plugin is not None
+            and config.current_plugin in config.plugins
+        ):
+            for k, v in config.plugins[config.current_plugin].items():
+                if k in self.plugin_key_mapping:
+                    k = self.plugin_key_mapping[k]
+
+                data[k] = str(v)
+
         response = requests.post(
             config.backend,
             files={
                 "sample": ("audio.wav", buffer, "audio/wav"),
             },
-            data={
-                "fSafePrefixPadLength": "0",
-                "fPitchChange": str(config.pitch_shift),
-                "sSpeakId": "0",
-                "sampleRate": str(config.sample_rate),
-            },
+            data=data,
         )
 
         assert response.status_code == 200, f"Failed to request"
 
         buffer.close()
 
         with BytesIO(response.content) as buffer:
```

### Comparing `rtvc-0.1.1/rtvc/i18n.py` & `rtvc-0.2.0/rtvc/i18n.py`

 * *Files identical despite different names*

### Comparing `rtvc-0.1.1/tests/test_sola.py` & `rtvc-0.2.0/tests/test_sola.py`

 * *Files identical despite different names*

### Comparing `rtvc-0.1.1/PKG-INFO` & `rtvc-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: rtvc
-Version: 0.1.1
+Version: 0.2.0
 Summary: Real-Time Voice Conversion GUI
 Keywords: voice-conversion svc
 Author-Email: lengyue <lengyue@lengyue.me>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Project-URL: Repository, https://github.com/fishaudio/realtime-vc-gui
 Requires-Python: <3.12,>=3.10
 Requires-Dist: noisereduce>=2.0.1
 Requires-Dist: sounddevice>=0.4.6
 Requires-Dist: pyyaml>=6.0
 Requires-Dist: PyQt6>=6.5.0
 Requires-Dist: pyqtdarktheme==2.1.0
 Requires-Dist: requests>=2.31.0
+Requires-Dist: librosa==0.9.2
 Description-Content-Type: text/markdown
 
 # RTVC: Real-Time Voice Conversion GUI
 [![PyPI Version](https://img.shields.io/pypi/v/rtvc.svg?style=flat-square)](https://pypi.python.org/pypi/rtvc)
 [![CI Status](https://img.shields.io/github/actions/workflow/status/fishaudio/realtime-vc-gui/ci.yml?style=flat-square&logo=GitHub)](https://github.com/fishaudio/realtime-vc-gui/actions)
 [![License](https://img.shields.io/github/license/fishaudio/realtime-vc-gui?style=flat-square)](https://github.com/fishaudio/realtime-vc-gui/blob/main/LICENSE)
```

