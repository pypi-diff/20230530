# Comparing `tmp/rpi_reactive_gpio-0.1.3.tar.gz` & `tmp/rpi_reactive_gpio-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpi_reactive_gpio-0.1.3.tar", max compression
+gzip compressed data, was "rpi_reactive_gpio-0.1.4.tar", max compression
```

## Comparing `rpi_reactive_gpio-0.1.3.tar` & `rpi_reactive_gpio-0.1.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1068 2023-05-30 12:15:56.665676 rpi_reactive_gpio-0.1.3/LICENSE
--rw-r--r--   0        0        0       80 2023-05-30 12:15:56.665676 rpi_reactive_gpio-0.1.3/README.md
--rw-r--r--   0        0        0      766 2023-05-30 12:16:18.633638 rpi_reactive_gpio-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      202 2023-05-30 12:15:56.665676 rpi_reactive_gpio-0.1.3/rpi_reactive_gpio/__init__.py
--rw-r--r--   0        0        0     1504 2023-05-30 12:15:56.665676 rpi_reactive_gpio-0.1.3/rpi_reactive_gpio/buttons.py
--rw-r--r--   0        0        0     3503 2023-05-30 12:15:56.665676 rpi_reactive_gpio-0.1.3/rpi_reactive_gpio/leds.py
--rw-r--r--   0        0        0      477 2023-05-30 12:15:56.665676 rpi_reactive_gpio-0.1.3/rpi_reactive_gpio/main.py
--rw-r--r--   0        0        0      840 2023-05-30 12:15:56.665676 rpi_reactive_gpio-0.1.3/rpi_reactive_gpio/pin_manager.py
--rw-r--r--   0        0        0     1100 2023-05-30 12:15:56.665676 rpi_reactive_gpio-0.1.3/rpi_reactive_gpio/scene.py
--rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 rpi_reactive_gpio-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-30 13:33:22.197888 rpi_reactive_gpio-0.1.4/LICENSE
+-rw-r--r--   0        0        0       80 2023-05-30 13:33:22.197888 rpi_reactive_gpio-0.1.4/README.md
+-rw-r--r--   0        0        0      766 2023-05-30 13:33:45.678206 rpi_reactive_gpio-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      207 2023-05-30 13:33:22.197888 rpi_reactive_gpio-0.1.4/rpi_reactive_gpio/__init__.py
+-rw-r--r--   0        0        0     1603 2023-05-30 13:33:22.197888 rpi_reactive_gpio-0.1.4/rpi_reactive_gpio/buttons.py
+-rw-r--r--   0        0        0     3504 2023-05-30 13:33:22.197888 rpi_reactive_gpio-0.1.4/rpi_reactive_gpio/leds.py
+-rw-r--r--   0        0        0      478 2023-05-30 13:33:22.197888 rpi_reactive_gpio-0.1.4/rpi_reactive_gpio/main.py
+-rw-r--r--   0        0        0      850 2023-05-30 13:33:22.197888 rpi_reactive_gpio-0.1.4/rpi_reactive_gpio/pin_manager.py
+-rw-r--r--   0        0        0     1102 2023-05-30 13:33:22.197888 rpi_reactive_gpio-0.1.4/rpi_reactive_gpio/scene.py
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 rpi_reactive_gpio-0.1.4/PKG-INFO
```

### Comparing `rpi_reactive_gpio-0.1.3/LICENSE` & `rpi_reactive_gpio-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.3/pyproject.toml` & `rpi_reactive_gpio-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rpi-reactive-gpio"
-version = "0.1.3"
+version = "0.1.4"
 description = "Syntax sugar for controlling RPi.GPIO with reactive design."
 authors = ["MarkParker5 <markparker.it@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rpi_reactive_gpio"}]
 homepage = "https://pypi.org/project/rpi-reactive-gpio/"
 repository = "https://github.com/MarkParker5/rpi-reactive-gpio"
```

### Comparing `rpi_reactive_gpio-0.1.3/rpi_reactive_gpio/buttons.py` & `rpi_reactive_gpio-0.1.4/rpi_reactive_gpio/buttons.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from __future__ import annotations
-from typing import Callable, Any
+from typing import Callable, Any, TypeVar
 import time
 import RPi.GPIO as GPIO
-from pin_manager import tickables
+from .pin_manager import tickables
 
+
+ButtonCallback = TypeVar('ButtonCallback', bound = Callable[[int], None] | Callable[['ButtonClick', int], None])
     
 class ButtonClick:
     
     pass_args: list[Any] = []
     
     def __init__(self, pin: int, event_type: int = GPIO.FALLING, debounce_time_ms: int = 50, multiple_clicks_duration_ms: int = 500) -> None:
         self.pin = pin
@@ -24,15 +26,15 @@
             time_elapsed = time.time() - self.last_click_time
 
             if time_elapsed > self.multiple_clicks_duration_ms / 1000:
                 self.callback(*self.pass_args, self.num_clicks)
                 self.num_clicks = 0
     
     # decorator
-    def __call__(self, callback: Callable[[int], None]) -> Callable[[int], None]:
+    def __call__(self, callback: ButtonCallback) -> ButtonClick:
         self.callback = callback
         
         def event_handler(_):
             self.num_clicks += 1
             self.last_click_time = time.time()
         
         GPIO.setup(self.pin, GPIO.IN, pull_up_down = GPIO.PUD_UP)
@@ -41,8 +43,8 @@
             self.pin,
             self.event_type,
             callback = event_handler,
             bouncetime = self.debounce_time_ms
         )
         
         tickables.append(self)
-        return event_handler
+        return self
```

### Comparing `rpi_reactive_gpio-0.1.3/rpi_reactive_gpio/leds.py` & `rpi_reactive_gpio-0.1.4/rpi_reactive_gpio/leds.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from enum import Enum
 from typing import Callable
 import RPi.GPIO as GPIO
-from pin_manager import tickables, managers
+from .pin_manager import tickables, managers
 
 
 class LedState(Enum):
     off = 0
     on = 1
     blink = 2
     fast_blink = 3
```

### Comparing `rpi_reactive_gpio-0.1.3/rpi_reactive_gpio/pin_manager.py` & `rpi_reactive_gpio-0.1.4/rpi_reactive_gpio/pin_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 @runtime_checkable
 class Tickable(Protocol):
     def tick(self, period: float = 1.0):
         '''period must be in range 0.0...1.0'''
         pass
     
 @runtime_checkable
-class PinManagerProtocol(Tickable):
+class PinManagerProtocol(Tickable, Protocol):
     
     def update(self, *args, **kwargs):
         pass
     
     def __call__(self, get_pin_state: Callable) -> PinManagerProtocol:
         '''decorator for setting get_pin_state function that updates led state'''
         pass
```

### Comparing `rpi_reactive_gpio-0.1.3/rpi_reactive_gpio/scene.py` & `rpi_reactive_gpio-0.1.4/rpi_reactive_gpio/scene.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import time
 from abc import ABC
-from pin_manager import PinManagerProtocol, Tickable
-from buttons import ButtonClick
+from .pin_manager import PinManagerProtocol, Tickable
+from .buttons import ButtonClick
 
 
 class Scene(ABC):
     def main_loop(self, update_interval: float = 1.0, ticks_count: int = 100):
         attributes = [getattr(self, a) for a in dir(self)]
         self.managers = filter(lambda a: isinstance(a, PinManagerProtocol), attributes)
         self.tickables = filter(lambda a: isinstance(a, Tickable), attributes)
```

### Comparing `rpi_reactive_gpio-0.1.3/PKG-INFO` & `rpi_reactive_gpio-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpi-reactive-gpio
-Version: 0.1.3
+Version: 0.1.4
 Summary: Syntax sugar for controlling RPi.GPIO with reactive design.
 Home-page: https://pypi.org/project/rpi-reactive-gpio/
 License: MIT
 Keywords: raspberry-pi,gpio,reactive,rxpy,rx,rpi,rpi-gpio,RPi.GPIO
 Author: MarkParker5
 Author-email: markparker.it@gmail.com
 Requires-Python: >=3.10,<4.0
```

