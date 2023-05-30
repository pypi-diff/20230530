# Comparing `tmp/rpi_reactive_gpio-0.1.0.tar.gz` & `tmp/rpi_reactive_gpio-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpi_reactive_gpio-0.1.0.tar", max compression
+gzip compressed data, was "rpi_reactive_gpio-0.1.1.tar", max compression
```

## Comparing `rpi_reactive_gpio-0.1.0.tar` & `rpi_reactive_gpio-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1068 2023-05-25 06:52:36.683819 rpi_reactive_gpio-0.1.0/LICENSE
--rw-r--r--   0        0        0       80 2023-05-25 06:52:36.683819 rpi_reactive_gpio-0.1.0/README.md
--rw-r--r--   0        0        0      766 2023-05-25 06:52:36.683819 rpi_reactive_gpio-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      202 2023-05-25 06:52:36.683819 rpi_reactive_gpio-0.1.0/rpi_reactive_gpio/__init__.py
--rw-r--r--   0        0        0     1510 2023-05-25 06:52:36.683819 rpi_reactive_gpio-0.1.0/rpi_reactive_gpio/buttons.py
--rw-r--r--   0        0        0     3509 2023-05-25 06:52:36.683819 rpi_reactive_gpio-0.1.0/rpi_reactive_gpio/leds.py
--rw-r--r--   0        0        0      477 2023-05-25 06:52:36.683819 rpi_reactive_gpio-0.1.0/rpi_reactive_gpio/main.py
--rw-r--r--   0        0        0      846 2023-05-25 06:52:36.683819 rpi_reactive_gpio-0.1.0/rpi_reactive_gpio/pin_manager.py
--rw-r--r--   0        0        0     1044 2023-05-25 06:52:36.683819 rpi_reactive_gpio-0.1.0/rpi_reactive_gpio/scene.py
--rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 rpi_reactive_gpio-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-30 11:45:11.656786 rpi_reactive_gpio-0.1.1/LICENSE
+-rw-r--r--   0        0        0       80 2023-05-30 11:45:11.656786 rpi_reactive_gpio-0.1.1/README.md
+-rw-r--r--   0        0        0      766 2023-05-30 11:45:28.953031 rpi_reactive_gpio-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      202 2023-05-30 11:45:11.656786 rpi_reactive_gpio-0.1.1/rpi_reactive_gpio/__init__.py
+-rw-r--r--   0        0        0     1504 2023-05-30 11:45:11.656786 rpi_reactive_gpio-0.1.1/rpi_reactive_gpio/buttons.py
+-rw-r--r--   0        0        0     3503 2023-05-30 11:45:11.656786 rpi_reactive_gpio-0.1.1/rpi_reactive_gpio/leds.py
+-rw-r--r--   0        0        0      477 2023-05-30 11:45:11.656786 rpi_reactive_gpio-0.1.1/rpi_reactive_gpio/main.py
+-rw-r--r--   0        0        0      840 2023-05-30 11:45:11.656786 rpi_reactive_gpio-0.1.1/rpi_reactive_gpio/pin_manager.py
+-rw-r--r--   0        0        0     1100 2023-05-30 11:45:11.656786 rpi_reactive_gpio-0.1.1/rpi_reactive_gpio/scene.py
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 rpi_reactive_gpio-0.1.1/PKG-INFO
```

### Comparing `rpi_reactive_gpio-0.1.0/LICENSE` & `rpi_reactive_gpio-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.0/pyproject.toml` & `rpi_reactive_gpio-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rpi-reactive-gpio"
-version = "0.1.0"
+version = "0.1.1"
 description = "Syntax sugar for controlling RPi.GPIO with reactive design."
 authors = ["MarkParker5 <markparker.it@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rpi_reactive_gpio"}]
 homepage = "https://pypi.org/project/rpi-reactive-gpio/"
 repository = "https://github.com/MarkParker5/rpi-reactive-gpio"
```

### Comparing `rpi_reactive_gpio-0.1.0/rpi_reactive_gpio/buttons.py` & `rpi_reactive_gpio-0.1.1/rpi_reactive_gpio/buttons.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from typing import Callable, Any
 import time
 import RPi.GPIO as GPIO
-from pin_manager import all_tickable
+from pin_manager import tickables
 
     
 class ButtonClick:
     
     pass_args: list[Any] = []
     
     def __init__(self, pin: int, event_type: int = GPIO.FALLING, debounce_time_ms: int = 50, multiple_clicks_duration_ms: int = 500) -> None:
@@ -40,9 +40,9 @@
         GPIO.add_event_detect(
             self.pin,
             self.event_type,
             callback = event_handler,
             bouncetime = self.debounce_time_ms
         )
         
-        all_tickable.append(self)
+        tickables.append(self)
         return event_handler
```

### Comparing `rpi_reactive_gpio-0.1.0/rpi_reactive_gpio/leds.py` & `rpi_reactive_gpio-0.1.1/rpi_reactive_gpio/leds.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from enum import Enum
 from typing import Callable
 import RPi.GPIO as GPIO
-from pin_manager import all_tickable, managers
+from pin_manager import tickables, managers
 
 
 class LedState(Enum):
     off = 0
     on = 1
     blink = 2
     fast_blink = 3
@@ -37,15 +37,15 @@
         self._last_led_state = self._get_pin_state(*args, **kwargs)
     
     # decorator
     def __call__(self, get_pin_state: Callable[..., LedState]) -> LedManager:
         global managers
         self._get_pin_state = get_pin_state
         managers.append(self)
-        all_tickable.append(self)
+        tickables.append(self)
         return self
     
 class RGBLedState(Enum):
     off = 0
     red = 1
     yellow = 2
     green = 3
```

### Comparing `rpi_reactive_gpio-0.1.0/rpi_reactive_gpio/scene.py` & `rpi_reactive_gpio-0.1.1/rpi_reactive_gpio/scene.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 import time
 from abc import ABC
-from pin_manager import PinManagerProtocol
+from pin_manager import PinManagerProtocol, Tickable
 from buttons import ButtonClick
 
 
 class Scene(ABC):
     def main_loop(self, update_interval: float = 1.0, ticks_count: int = 100):
         attributes = [getattr(self, a) for a in dir(self)]
         self.managers = filter(lambda a: isinstance(a, PinManagerProtocol), attributes)
+        self.tickables = filter(lambda a: isinstance(a, Tickable), attributes)
         self.events = filter(lambda a: isinstance(a, ButtonClick), attributes)
         
         for event in self.events:
             event.pass_args = [self]
         
         while True:
-            self.update_all_managers()
+            self.update_all()
             for i in range(ticks_count):
-                self.tick_all_managers(i / ticks_count)
+                self.tick_all(i / ticks_count)
                 time.sleep(update_interval / ticks_count)
                 
-    def update_all_managers(self):
+    def update_all(self):
         for manager in self.managers:
             manager.update(self)
             
-    def tick_all_managers(self, period: float = 1.0):
+    def tick_all(self, period: float = 1.0):
         '''period must be in range 0.0...1.0'''
-        for manager in self.managers:
-            manager.tick(period)
+        for tickable in self.tickables:
+            tickable.tick(period)
```

### Comparing `rpi_reactive_gpio-0.1.0/PKG-INFO` & `rpi_reactive_gpio-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpi-reactive-gpio
-Version: 0.1.0
+Version: 0.1.1
 Summary: Syntax sugar for controlling RPi.GPIO with reactive design.
 Home-page: https://pypi.org/project/rpi-reactive-gpio/
 License: MIT
 Keywords: raspberry-pi,gpio,reactive,rxpy,rx,rpi,rpi-gpio,RPi.GPIO
 Author: MarkParker5
 Author-email: markparker.it@gmail.com
 Requires-Python: >=3.10,<4.0
```

