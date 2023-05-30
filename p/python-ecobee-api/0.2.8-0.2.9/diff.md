# Comparing `tmp/python-ecobee-api-0.2.8.tar.gz` & `tmp/python-ecobee-api-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-ecobee-api-0.2.8.tar", last modified: Tue Jan  5 17:47:54 2021, max compression
+gzip compressed data, was "dist/python-ecobee-api-0.2.9.tar", last modified: Wed Jan  6 03:41:29 2021, max compression
```

## Comparing `python-ecobee-api-0.2.8.tar` & `python-ecobee-api-0.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 nolan     (1001) nolan     (1001)        0 2021-01-05 17:47:54.482372 python-ecobee-api-0.2.8/
--rw-rw-r--   0 nolan     (1001) nolan     (1001)      278 2021-01-05 17:47:54.482372 python-ecobee-api-0.2.8/PKG-INFO
--rw-rw-r--   0 nolan     (1001) nolan     (1001)      153 2021-01-05 17:42:52.000000 python-ecobee-api-0.2.8/README.md
-drwxrwxr-x   0 nolan     (1001) nolan     (1001)        0 2021-01-05 17:47:54.478372 python-ecobee-api-0.2.8/pyecobee/
--rw-rw-r--   0 nolan     (1001) nolan     (1001)    22711 2021-01-05 17:42:52.000000 python-ecobee-api-0.2.8/pyecobee/__init__.py
--rw-rw-r--   0 nolan     (1001) nolan     (1001)     1195 2021-01-05 17:42:52.000000 python-ecobee-api-0.2.8/pyecobee/const.py
--rw-rw-r--   0 nolan     (1001) nolan     (1001)      375 2021-01-05 17:42:52.000000 python-ecobee-api-0.2.8/pyecobee/errors.py
--rw-rw-r--   0 nolan     (1001) nolan     (1001)     1047 2021-01-05 17:42:52.000000 python-ecobee-api-0.2.8/pyecobee/util.py
-drwxrwxr-x   0 nolan     (1001) nolan     (1001)        0 2021-01-05 17:47:54.482372 python-ecobee-api-0.2.8/python_ecobee_api.egg-info/
--rw-rw-r--   0 nolan     (1001) nolan     (1001)      278 2021-01-05 17:47:54.000000 python-ecobee-api-0.2.8/python_ecobee_api.egg-info/PKG-INFO
--rw-rw-r--   0 nolan     (1001) nolan     (1001)      343 2021-01-05 17:47:54.000000 python-ecobee-api-0.2.8/python_ecobee_api.egg-info/SOURCES.txt
--rw-rw-r--   0 nolan     (1001) nolan     (1001)        1 2021-01-05 17:47:54.000000 python-ecobee-api-0.2.8/python_ecobee_api.egg-info/dependency_links.txt
--rw-rw-r--   0 nolan     (1001) nolan     (1001)       14 2021-01-05 17:47:54.000000 python-ecobee-api-0.2.8/python_ecobee_api.egg-info/requires.txt
--rw-rw-r--   0 nolan     (1001) nolan     (1001)        9 2021-01-05 17:47:54.000000 python-ecobee-api-0.2.8/python_ecobee_api.egg-info/top_level.txt
--rw-rw-r--   0 nolan     (1001) nolan     (1001)        1 2021-01-05 17:47:54.000000 python-ecobee-api-0.2.8/python_ecobee_api.egg-info/zip-safe
--rw-rw-r--   0 nolan     (1001) nolan     (1001)       79 2021-01-05 17:47:54.482372 python-ecobee-api-0.2.8/setup.cfg
--rwxrwxr-x   0 nolan     (1001) nolan     (1001)     1680 2021-01-05 17:43:31.000000 python-ecobee-api-0.2.8/setup.py
+drwxrwxr-x   0 nolan     (1001) nolan     (1001)        0 2021-01-06 03:41:29.879696 python-ecobee-api-0.2.9/
+-rw-rw-r--   0 nolan     (1001) nolan     (1001)      278 2021-01-06 03:41:29.879696 python-ecobee-api-0.2.9/PKG-INFO
+-rw-rw-r--   0 nolan     (1001) nolan     (1001)      153 2021-01-05 17:42:52.000000 python-ecobee-api-0.2.9/README.md
+drwxrwxr-x   0 nolan     (1001) nolan     (1001)        0 2021-01-06 03:41:29.875696 python-ecobee-api-0.2.9/pyecobee/
+-rw-rw-r--   0 nolan     (1001) nolan     (1001)    23350 2021-01-06 03:40:49.000000 python-ecobee-api-0.2.9/pyecobee/__init__.py
+-rw-rw-r--   0 nolan     (1001) nolan     (1001)     1195 2021-01-05 17:42:52.000000 python-ecobee-api-0.2.9/pyecobee/const.py
+-rw-rw-r--   0 nolan     (1001) nolan     (1001)      375 2021-01-05 17:42:52.000000 python-ecobee-api-0.2.9/pyecobee/errors.py
+-rw-rw-r--   0 nolan     (1001) nolan     (1001)     1047 2021-01-05 17:42:52.000000 python-ecobee-api-0.2.9/pyecobee/util.py
+drwxrwxr-x   0 nolan     (1001) nolan     (1001)        0 2021-01-06 03:41:29.879696 python-ecobee-api-0.2.9/python_ecobee_api.egg-info/
+-rw-rw-r--   0 nolan     (1001) nolan     (1001)      278 2021-01-06 03:41:29.000000 python-ecobee-api-0.2.9/python_ecobee_api.egg-info/PKG-INFO
+-rw-rw-r--   0 nolan     (1001) nolan     (1001)      343 2021-01-06 03:41:29.000000 python-ecobee-api-0.2.9/python_ecobee_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 nolan     (1001) nolan     (1001)        1 2021-01-06 03:41:29.000000 python-ecobee-api-0.2.9/python_ecobee_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 nolan     (1001) nolan     (1001)       14 2021-01-06 03:41:29.000000 python-ecobee-api-0.2.9/python_ecobee_api.egg-info/requires.txt
+-rw-rw-r--   0 nolan     (1001) nolan     (1001)        9 2021-01-06 03:41:29.000000 python-ecobee-api-0.2.9/python_ecobee_api.egg-info/top_level.txt
+-rw-rw-r--   0 nolan     (1001) nolan     (1001)        1 2021-01-05 17:47:54.000000 python-ecobee-api-0.2.9/python_ecobee_api.egg-info/zip-safe
+-rw-rw-r--   0 nolan     (1001) nolan     (1001)       79 2021-01-06 03:41:29.879696 python-ecobee-api-0.2.9/setup.cfg
+-rwxrwxr-x   0 nolan     (1001) nolan     (1001)     1680 2021-01-06 03:40:41.000000 python-ecobee-api-0.2.9/setup.py
```

### Comparing `python-ecobee-api-0.2.8/pyecobee/__init__.py` & `python-ecobee-api-0.2.9/pyecobee/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -451,14 +451,30 @@
         log_msg_action = "send message"
 
         try:
             self._request("POST", ECOBEE_ENDPOINT_THERMOSTAT, log_msg_action, body=body)
         except (ExpiredTokenError, InvalidTokenError) as err:
             raise err
 
+    def set_humidifier_mode(self, index: int, humidifier_mode: str) -> None:
+        """Sets the humidifier mode (auto, off, manual)."""
+        body = {
+            "selection": {
+                "selectionType": "thermostats",
+                "selectionMatch": self.thermostats[index]["identifier"],
+            },
+            "thermostat": {"settings": {"humidifierMode": humidifier_mode}},
+        }
+        log_msg_action = "set humidifier mode"
+
+        try:
+            self._request("POST", ECOBEE_ENDPOINT_THERMOSTAT, log_msg_action, body=body)
+        except (ExpiredTokenError, InvalidTokenError) as err:
+            raise err
+
     def set_humidity(self, index: int, humidity: str) -> None:
         """Sets target humidity level."""
         body = {
             "selection": {
                 "selectionType": "thermostats",
                 "selectionMatch": self.thermostats[index]["identifier"],
             },
```

### Comparing `python-ecobee-api-0.2.8/pyecobee/const.py` & `python-ecobee-api-0.2.9/pyecobee/const.py`

 * *Files identical despite different names*

### Comparing `python-ecobee-api-0.2.8/pyecobee/util.py` & `python-ecobee-api-0.2.9/pyecobee/util.py`

 * *Files identical despite different names*

### Comparing `python-ecobee-api-0.2.8/setup.py` & `python-ecobee-api-0.2.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 
 setup(name='python-ecobee-api',
-      version='0.2.8',
+      version='0.2.9',
       description='Python API for talking to Ecobee thermostats',
       url='https://github.com/nkgilley/python-ecobee-api',
       author='Nolan Gilley',
       author_email='nkgilley@gmail.com',
       license='MIT',
       install_requires=['requests>=2.0'],
       packages=['pyecobee'],
```

