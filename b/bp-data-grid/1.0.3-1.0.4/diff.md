# Comparing `tmp/bp_data_grid-1.0.3.tar.gz` & `tmp/bp_data_grid-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bp_data_grid-1.0.3.tar", last modified: Wed May 10 10:52:05 2023, max compression
+gzip compressed data, was "bp_data_grid-1.0.4.tar", last modified: Tue May 30 09:59:14 2023, max compression
```

## Comparing `bp_data_grid-1.0.3.tar` & `bp_data_grid-1.0.4.tar`

### file list

```diff
@@ -1,26 +1,16 @@
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-10 10:52:05.404358 bp_data_grid-1.0.3/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     1063 2023-04-10 18:26:13.000000 bp_data_grid-1.0.3/LICENSE
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       44 2023-04-10 18:26:13.000000 bp_data_grid-1.0.3/MANIFEST.in
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3907 2023-05-10 10:52:05.404038 bp_data_grid-1.0.3/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2805 2023-05-03 12:51:36.000000 bp_data_grid-1.0.3/README.md
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-10 10:52:05.394868 bp_data_grid-1.0.3/bp_data_grid.egg-info/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     3907 2023-05-10 10:52:05.000000 bp_data_grid-1.0.3/bp_data_grid.egg-info/PKG-INFO
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      619 2023-05-10 10:52:05.000000 bp_data_grid-1.0.3/bp_data_grid.egg-info/SOURCES.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)        1 2023-05-10 10:52:05.000000 bp_data_grid-1.0.3/bp_data_grid.egg-info/dependency_links.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       18 2023-05-10 10:52:05.000000 bp_data_grid-1.0.3/bp_data_grid.egg-info/requires.txt
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       10 2023-05-10 10:52:05.000000 bp_data_grid-1.0.3/bp_data_grid.egg-info/top_level.txt
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-10 10:52:05.396157 bp_data_grid-1.0.3/data_grid/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)     2096 2023-04-24 06:27:21.000000 bp_data_grid-1.0.3/data_grid/__init__.py
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-10 10:52:05.391016 bp_data_grid-1.0.3/data_grid/frontend/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-10 10:52:05.397580 bp_data_grid-1.0.3/data_grid/frontend/dist/
-drwxr-xr-x   0 menakapanchaksharam   (501) staff       (20)        0 2023-05-10 10:52:05.403207 bp_data_grid-1.0.3/data_grid/frontend/dist/assets/
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)   202328 2023-05-10 10:51:00.000000 bp_data_grid-1.0.3/data_grid/frontend/dist/assets/html2canvas.esm-7570f311-59a6f546.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)  1581973 2023-05-10 10:51:00.000000 bp_data_grid-1.0.3/data_grid/frontend/dist/assets/index-015db93e.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      300 2023-05-10 10:51:00.000000 bp_data_grid-1.0.3/data_grid/frontend/dist/assets/index-d081bea5.css
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)   149944 2023-05-10 10:51:00.000000 bp_data_grid-1.0.3/data_grid/frontend/dist/assets/index.es-f2cb0452-6fcc3449.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)    21573 2023-05-10 10:51:00.000000 bp_data_grid-1.0.3/data_grid/frontend/dist/assets/purify.es-958e7803-b3d8833e.js
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      555 2023-05-10 10:51:35.000000 bp_data_grid-1.0.3/data_grid/frontend/dist/index.html
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     1497 2023-05-10 10:50:59.000000 bp_data_grid-1.0.3/data_grid/frontend/dist/vite.svg
--rw-rw-r--   0 menakapanchaksharam   (501) staff       (20)     2153 2023-04-10 09:19:07.000000 bp_data_grid-1.0.3/data_grid/register.py
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)       38 2023-05-10 10:52:05.404467 bp_data_grid-1.0.3/setup.cfg
--rw-r--r--   0 menakapanchaksharam   (501) staff       (20)      767 2023-05-10 10:51:47.000000 bp_data_grid-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:59:14.167108 bp_data_grid-1.0.4/
+-rw-rw-rw-   0        0        0     1082 2023-04-27 12:37:21.000000 bp_data_grid-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0       45 2023-04-27 12:37:21.000000 bp_data_grid-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4018 2023-05-30 09:59:14.159588 bp_data_grid-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2907 2023-05-09 08:44:53.000000 bp_data_grid-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 09:59:14.144593 bp_data_grid-1.0.4/bp_data_grid.egg-info/
+-rw-rw-rw-   0        0        0     4018 2023-05-30 09:59:13.000000 bp_data_grid-1.0.4/bp_data_grid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      261 2023-05-30 09:59:14.000000 bp_data_grid-1.0.4/bp_data_grid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 09:59:13.000000 bp_data_grid-1.0.4/bp_data_grid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-05-30 09:59:13.000000 bp_data_grid-1.0.4/bp_data_grid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 09:59:13.000000 bp_data_grid-1.0.4/bp_data_grid.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 09:59:14.153971 bp_data_grid-1.0.4/data_grid/
+-rw-rw-rw-   0        0        0     2175 2023-04-27 12:37:21.000000 bp_data_grid-1.0.4/data_grid/__init__.py
+-rw-rw-rw-   0        0        0     2206 2023-04-27 12:37:21.000000 bp_data_grid-1.0.4/data_grid/register.py
+-rw-rw-rw-   0        0        0       42 2023-05-30 09:59:14.169614 bp_data_grid-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      789 2023-05-30 09:56:08.000000 bp_data_grid-1.0.4/setup.py
```

### Comparing `bp_data_grid-1.0.3/LICENSE` & `bp_data_grid-1.0.4/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-Copyright (c) 2018-2021 Streamlit Inc.
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+Copyright (c) 2018-2021 Streamlit Inc.
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `bp_data_grid-1.0.3/data_grid/register.py` & `bp_data_grid-1.0.4/data_grid/register.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-from streamlit import session_state as _state
-from streamlit.components.v1 import components as _components
-
-
-def _patch_register_widget(register_widget):
-    def wrapper_register_widget(*args, **kwargs):
-        user_key = kwargs.get("user_key", None)
-        callbacks = _state.get("_components_callbacks", None)
-
-        # Check if a callback was registered for that user_key.
-        if user_key and callbacks and user_key in callbacks:
-            callback = callbacks[user_key]
-
-            # Add callback-specific args for the real register_widget function.
-            kwargs["on_change_handler"] = callback[0]
-            kwargs["args"] = callback[1]
-            kwargs["kwargs"] = callback[2]
-
-        # Call the original function with updated kwargs.
-        result = register_widget(*args, **kwargs)
-        return result
-
-    return wrapper_register_widget
-
-
-# Patch function only once.
-def init():
-    if not hasattr(_components.register_widget, "__callbacks_patched__"):
-        setattr(_components.register_widget, "__callbacks_patched__", True)
-        _components.register_widget = _patch_register_widget(_components.register_widget)
-
-
-def register_callback(element_key, callback, *callback_args, **callback_kwargs):
-    # Initialize callbacks store.
-    if "_components_callbacks" not in _state:
-        _state._components_callbacks = {}
-
-    # Register a callback for a given element_key.
-    _state._components_callbacks[element_key] = (callback, callback_args, callback_kwargs)
-
-def get_component_rerender_count(element_key):
-    # This funtion will return the custom component render count
-    if "_component_render_count" not in _state:
-        _state["_component_render_count"] = {}
-
-    if element_key not in _state["_component_render_count"]:
-        _state["_component_render_count"][element_key] = 0
-    return _state["_component_render_count"][element_key]
-    
-def set_component_rerender_count(element_key):
-    # This funtion will record the rerendering count
-    _state["_component_render_count"][element_key] = get_component_rerender_count(element_key) + 1
-    
+from streamlit import session_state as _state
+from streamlit.components.v1 import components as _components
+
+
+def _patch_register_widget(register_widget):
+    def wrapper_register_widget(*args, **kwargs):
+        user_key = kwargs.get("user_key", None)
+        callbacks = _state.get("_components_callbacks", None)
+
+        # Check if a callback was registered for that user_key.
+        if user_key and callbacks and user_key in callbacks:
+            callback = callbacks[user_key]
+
+            # Add callback-specific args for the real register_widget function.
+            kwargs["on_change_handler"] = callback[0]
+            kwargs["args"] = callback[1]
+            kwargs["kwargs"] = callback[2]
+
+        # Call the original function with updated kwargs.
+        result = register_widget(*args, **kwargs)
+        return result
+
+    return wrapper_register_widget
+
+
+# Patch function only once.
+def init():
+    if not hasattr(_components.register_widget, "__callbacks_patched__"):
+        setattr(_components.register_widget, "__callbacks_patched__", True)
+        _components.register_widget = _patch_register_widget(_components.register_widget)
+
+
+def register_callback(element_key, callback, *callback_args, **callback_kwargs):
+    # Initialize callbacks store.
+    if "_components_callbacks" not in _state:
+        _state._components_callbacks = {}
+
+    # Register a callback for a given element_key.
+    _state._components_callbacks[element_key] = (callback, callback_args, callback_kwargs)
+
+def get_component_rerender_count(element_key):
+    # This funtion will return the custom component render count
+    if "_component_render_count" not in _state:
+        _state["_component_render_count"] = {}
+
+    if element_key not in _state["_component_render_count"]:
+        _state["_component_render_count"][element_key] = 0
+    return _state["_component_render_count"][element_key]
+    
+def set_component_rerender_count(element_key):
+    # This funtion will record the rerendering count
+    _state["_component_render_count"][element_key] = get_component_rerender_count(element_key) + 1
+    
     return _state["_component_render_count"][element_key]
```

### Comparing `bp_data_grid-1.0.3/setup.py` & `bp_data_grid-1.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import setuptools
-from pathlib import Path
-this_directory = Path(__file__).parent
-long_description = (this_directory / "README.md").read_text()
-
-setuptools.setup(
-    name="bp_data_grid",
-    version="1.0.3",
-    author="Bluepinapple",
-    author_email="vivek.sthul@bluepinapple.com",
-    description="Show data in data grid",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
-    url="",
-    packages=setuptools.find_packages(),
-    include_package_data=True,
-    classifiers=[],
-    python_requires=">=3.8.10",
-    install_requires=[
-        # By definition, a Custom Component depends on Streamlit.
-        # If your component has other Python dependencies, list
-        # them here.
-        "streamlit >= 1.20.0",
-    ],
-)
+import setuptools
+from pathlib import Path
+this_directory = Path(__file__).parent
+long_description = (this_directory / "README.md").read_text()
+
+setuptools.setup(
+    name="bp_data_grid",
+    version="1.0.4",
+    author="Bluepineapple",
+    author_email="avinash@bluepineapple.io",
+    description="Show data in data grid",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    url="",
+    packages=setuptools.find_packages(),
+    include_package_data=True,
+    classifiers=[],
+    python_requires=">=3.8.10",
+    install_requires=[
+        # By definition, a Custom Component depends on Streamlit.
+        # If your component has other Python dependencies, list
+        # them here.
+        "streamlit >= 1.20.0",
+    ],
+)
```

