# Comparing `tmp/rpi_reactive_gpio-0.1.1.tar.gz` & `tmp/rpi_reactive_gpio-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpi_reactive_gpio-0.1.1.tar", max compression
+gzip compressed data, was "rpi_reactive_gpio-0.1.2.tar", max compression
```

## Comparing `rpi_reactive_gpio-0.1.1.tar` & `rpi_reactive_gpio-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1068 2023-05-30 11:45:11.656786 rpi_reactive_gpio-0.1.1/LICENSE
--rw-r--r--   0        0        0       80 2023-05-30 11:45:11.656786 rpi_reactive_gpio-0.1.1/README.md
--rw-r--r--   0        0        0      766 2023-05-30 11:45:28.953031 rpi_reactive_gpio-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      202 2023-05-30 11:45:11.656786 rpi_reactive_gpio-0.1.1/rpi_reactive_gpio/__init__.py
--rw-r--r--   0        0        0     1504 2023-05-30 11:45:11.656786 rpi_reactive_gpio-0.1.1/rpi_reactive_gpio/buttons.py
--rw-r--r--   0        0        0     3503 2023-05-30 11:45:11.656786 rpi_reactive_gpio-0.1.1/rpi_reactive_gpio/leds.py
--rw-r--r--   0        0        0      477 2023-05-30 11:45:11.656786 rpi_reactive_gpio-0.1.1/rpi_reactive_gpio/main.py
--rw-r--r--   0        0        0      840 2023-05-30 11:45:11.656786 rpi_reactive_gpio-0.1.1/rpi_reactive_gpio/pin_manager.py
--rw-r--r--   0        0        0     1100 2023-05-30 11:45:11.656786 rpi_reactive_gpio-0.1.1/rpi_reactive_gpio/scene.py
--rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 rpi_reactive_gpio-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-30 11:54:05.027960 rpi_reactive_gpio-0.1.2/LICENSE
+-rw-r--r--   0        0        0       80 2023-05-30 11:54:05.027960 rpi_reactive_gpio-0.1.2/README.md
+-rw-r--r--   0        0        0      766 2023-05-30 11:54:27.980213 rpi_reactive_gpio-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      202 2023-05-30 11:54:05.027960 rpi_reactive_gpio-0.1.2/rpi_reactive_gpio/__init__.py
+-rw-r--r--   0        0        0     1504 2023-05-30 11:54:05.027960 rpi_reactive_gpio-0.1.2/rpi_reactive_gpio/buttons.py
+-rw-r--r--   0        0        0     3503 2023-05-30 11:54:05.027960 rpi_reactive_gpio-0.1.2/rpi_reactive_gpio/leds.py
+-rw-r--r--   0        0        0      477 2023-05-30 11:54:05.027960 rpi_reactive_gpio-0.1.2/rpi_reactive_gpio/main.py
+-rw-r--r--   0        0        0      840 2023-05-30 11:54:05.027960 rpi_reactive_gpio-0.1.2/rpi_reactive_gpio/pin_manager.py
+-rw-r--r--   0        0        0     1100 2023-05-30 11:54:05.027960 rpi_reactive_gpio-0.1.2/rpi_reactive_gpio/scene.py
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 rpi_reactive_gpio-0.1.2/PKG-INFO
```

### Comparing `rpi_reactive_gpio-0.1.1/LICENSE` & `rpi_reactive_gpio-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.1/pyproject.toml` & `rpi_reactive_gpio-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rpi-reactive-gpio"
-version = "0.1.1"
+version = "0.1.2"
 description = "Syntax sugar for controlling RPi.GPIO with reactive design."
 authors = ["MarkParker5 <markparker.it@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "rpi_reactive_gpio"}]
 homepage = "https://pypi.org/project/rpi-reactive-gpio/"
 repository = "https://github.com/MarkParker5/rpi-reactive-gpio"
```

### Comparing `rpi_reactive_gpio-0.1.1/rpi_reactive_gpio/buttons.py` & `rpi_reactive_gpio-0.1.2/rpi_reactive_gpio/buttons.py`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.1/rpi_reactive_gpio/leds.py` & `rpi_reactive_gpio-0.1.2/rpi_reactive_gpio/leds.py`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.1/rpi_reactive_gpio/pin_manager.py` & `rpi_reactive_gpio-0.1.2/rpi_reactive_gpio/pin_manager.py`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.1/rpi_reactive_gpio/scene.py` & `rpi_reactive_gpio-0.1.2/rpi_reactive_gpio/scene.py`

 * *Files identical despite different names*

### Comparing `rpi_reactive_gpio-0.1.1/PKG-INFO` & `rpi_reactive_gpio-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpi-reactive-gpio
-Version: 0.1.1
+Version: 0.1.2
 Summary: Syntax sugar for controlling RPi.GPIO with reactive design.
 Home-page: https://pypi.org/project/rpi-reactive-gpio/
 License: MIT
 Keywords: raspberry-pi,gpio,reactive,rxpy,rx,rpi,rpi-gpio,RPi.GPIO
 Author: MarkParker5
 Author-email: markparker.it@gmail.com
 Requires-Python: >=3.10,<4.0
```

