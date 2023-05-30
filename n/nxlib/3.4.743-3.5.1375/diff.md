# Comparing `tmp/nxlib-3.4.743.tar.gz` & `tmp/nxlib-3.5.1375.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nxlib-3.4.743.tar", last modified: Wed Feb  8 14:52:25 2023, max compression
+gzip compressed data, was "nxlib-3.5.1375.tar", last modified: Tue May 30 09:57:21 2023, max compression
```

## Comparing `nxlib-3.4.743.tar` & `nxlib-3.5.1375.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        0 2023-02-08 14:52:25.213431 nxlib-3.4.743/
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     1511 2023-02-08 14:52:25.213431 nxlib-3.4.743/PKG-INFO
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)      898 2022-08-02 08:13:19.000000 nxlib-3.4.743/README.md
-drwxr-xr-x   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        0 2023-02-08 14:52:25.209431 nxlib-3.4.743/ensenso_nxlib/
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)      288 2022-08-02 08:13:19.000000 nxlib-3.4.743/ensenso_nxlib/__init__.py
-drwxr-xr-x   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        0 2023-02-08 14:52:25.209431 nxlib-3.4.743/nxlib/
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)      349 2022-08-02 08:13:19.000000 nxlib-3.4.743/nxlib/__init__.py
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     3173 2022-08-02 08:13:19.000000 nxlib-3.4.743/nxlib/_helper.py
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)    22315 2023-02-03 15:26:48.000000 nxlib-3.4.743/nxlib/api.py
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     5253 2023-02-03 15:26:48.000000 nxlib-3.4.743/nxlib/command.py
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)    31102 2023-02-08 14:52:24.000000 nxlib-3.4.743/nxlib/constants.py
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)    10523 2023-02-08 14:31:58.000000 nxlib-3.4.743/nxlib/context.py
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     3243 2022-08-02 08:13:19.000000 nxlib-3.4.743/nxlib/exception.py
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)    22914 2022-08-02 08:13:19.000000 nxlib-3.4.743/nxlib/item.py
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)    12234 2023-02-08 14:31:58.000000 nxlib-3.4.743/nxlib/log.py
-drwxr-xr-x   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        0 2023-02-08 14:52:25.213431 nxlib-3.4.743/nxlib.egg-info/
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     1511 2023-02-08 14:52:25.000000 nxlib-3.4.743/nxlib.egg-info/PKG-INFO
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)      373 2023-02-08 14:52:25.000000 nxlib-3.4.743/nxlib.egg-info/SOURCES.txt
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        1 2023-02-08 14:52:25.000000 nxlib-3.4.743/nxlib.egg-info/dependency_links.txt
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        1 2022-08-22 06:18:36.000000 nxlib-3.4.743/nxlib.egg-info/not-zip-safe
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        6 2023-02-08 14:52:25.000000 nxlib-3.4.743/nxlib.egg-info/requires.txt
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)       20 2023-02-08 14:52:25.000000 nxlib-3.4.743/nxlib.egg-info/top_level.txt
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)      198 2023-02-08 14:52:25.213431 nxlib-3.4.743/setup.cfg
--rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     2275 2023-01-09 09:24:20.000000 nxlib-3.4.743/setup.py
+drwxr-xr-x   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        0 2023-05-30 09:57:21.338131 nxlib-3.5.1375/
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     1512 2023-05-30 09:57:21.338131 nxlib-3.5.1375/PKG-INFO
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)      898 2022-08-02 08:13:19.000000 nxlib-3.5.1375/README.md
+drwxr-xr-x   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        0 2023-05-30 09:57:21.334131 nxlib-3.5.1375/ensenso_nxlib/
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)      288 2022-08-02 08:13:19.000000 nxlib-3.5.1375/ensenso_nxlib/__init__.py
+drwxr-xr-x   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        0 2023-05-30 09:57:21.334131 nxlib-3.5.1375/nxlib/
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)      349 2022-08-02 08:13:19.000000 nxlib-3.5.1375/nxlib/__init__.py
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     3173 2022-08-02 08:13:19.000000 nxlib-3.5.1375/nxlib/_helper.py
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)    22315 2023-05-25 12:50:28.000000 nxlib-3.5.1375/nxlib/api.py
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     5253 2023-05-26 12:02:39.000000 nxlib-3.5.1375/nxlib/command.py
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)    31417 2023-05-30 09:57:21.000000 nxlib-3.5.1375/nxlib/constants.py
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)    10603 2023-05-25 12:50:28.000000 nxlib-3.5.1375/nxlib/context.py
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     3243 2022-08-02 08:13:19.000000 nxlib-3.5.1375/nxlib/exception.py
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)    22914 2022-08-02 08:13:19.000000 nxlib-3.5.1375/nxlib/item.py
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)    12236 2023-05-25 12:50:28.000000 nxlib-3.5.1375/nxlib/log.py
+drwxr-xr-x   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        0 2023-05-30 09:57:21.338131 nxlib-3.5.1375/nxlib.egg-info/
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     1512 2023-05-30 09:57:21.000000 nxlib-3.5.1375/nxlib.egg-info/PKG-INFO
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)      373 2023-05-30 09:57:21.000000 nxlib-3.5.1375/nxlib.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        1 2023-05-30 09:57:21.000000 nxlib-3.5.1375/nxlib.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        1 2022-08-22 06:18:36.000000 nxlib-3.5.1375/nxlib.egg-info/not-zip-safe
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)        6 2023-05-30 09:57:21.000000 nxlib-3.5.1375/nxlib.egg-info/requires.txt
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)       20 2023-05-30 09:57:21.000000 nxlib-3.5.1375/nxlib.egg-info/top_level.txt
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)      198 2023-05-30 09:57:21.338131 nxlib-3.5.1375/setup.cfg
+-rw-r--r--   0 daniel.saier (1567401200) domänen-benutzer (1567400513)     2275 2023-05-25 12:50:28.000000 nxlib-3.5.1375/setup.py
```

### Comparing `nxlib-3.4.743/PKG-INFO` & `nxlib-3.5.1375/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nxlib
-Version: 3.4.743
+Version: 3.5.1375
 Summary: Python interface to interact with the Ensenso NxLib
 Home-page: https://www.ensenso.com/python-api
 Author: Optonic GmbH
 Author-email: support@optonic.com
 License: MIT
 Description: > **Announcement:**
         With Ensenso SDK version 3.3 we stop the maintenance of our
```

### Comparing `nxlib-3.4.743/README.md` & `nxlib-3.5.1375/README.md`

 * *Files identical despite different names*

### Comparing `nxlib-3.4.743/nxlib/_helper.py` & `nxlib-3.5.1375/nxlib/_helper.py`

 * *Files identical despite different names*

### Comparing `nxlib-3.4.743/nxlib/api.py` & `nxlib-3.5.1375/nxlib/api.py`

 * *Files identical despite different names*

### Comparing `nxlib-3.4.743/nxlib/command.py` & `nxlib-3.5.1375/nxlib/command.py`

 * *Files identical despite different names*

### Comparing `nxlib-3.4.743/nxlib/constants.py` & `nxlib-3.5.1375/nxlib/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,15 @@
 ITM_ANGLE = "Angle"
 ITM_ANGLES = "Angles"
 ITM_ANGULAR_RESOLUTION = "AngularResolution"
 ITM_APERTURE = "Aperture"
 ITM_API_ERRORS = "ApiErrors"
 ITM_APPLICATION = "Application"
 ITM_APPLY = "Apply"
+ITM_APPROVED = "Approved"
 ITM_ARCHITECTURE = "Architecture"
 ITM_AREA_OF_INTEREST = "AreaOfInterest"
 ITM_ASSEMBLY_CALIBRATION = "AssemblyCalibration"
 ITM_ASSEMBLY_PATTERN = "AssemblyPattern"
 ITM_ASYNCHRONOUSLY_TRIGGERED = "AsynchronouslyTriggered"
 ITM_AUTO_BLACK_LEVEL = "AutoBlackLevel"
 ITM_AUTO_EXPOSURE = "AutoExposure"
@@ -144,14 +145,15 @@
 ITM_AUTOMATIC = "Automatic"
 ITM_AVAILABLE = "Available"
 ITM_AVERAGE = "Average"
 ITM_AVERAGE_POSE_ERROR = "AveragePoseError"
 ITM_AVERAGE_TRIANGULATION_ERROR = "AverageTriangulationError"
 ITM_AXIS = "Axis"
 ITM_BACKGROUND = "Background"
+ITM_BACKLOG_SIZE = "BacklogSize"
 ITM_BANDWIDTH = "Bandwidth"
 ITM_BANDWIDTH_LIMIT = "BandwidthLimit"
 ITM_BASELINE = "Baseline"
 ITM_BETA = "Beta"
 ITM_BILLBOARD_SIZE = "BillboardSize"
 ITM_BINARY_INFO = "BinaryInfo"
 ITM_BINNING = "Binning"
@@ -373,14 +375,15 @@
 ITM_INTERVAL = "Interval"
 ITM_INVALIDATION = "Invalidation"
 ITM_INVERSE = "Inverse"
 ITM_INVERT = "Invert"
 ITM_IP_ADDRESS = "IpAddress"
 ITM_IP_BROADCAST = "IpBroadcast"
 ITM_IP_SUBNET_MASK = "IpSubnetMask"
+ITM_IS_APPROVED_FIRMWARE_VERSION = "IsApprovedFirmwareVersion"
 ITM_IS_SUPPLIED_FIRMWARE_VERSION = "IsSuppliedFirmwareVersion"
 ITM_ITEM_TYPES = "ItemTypes"
 ITM_ITEMS = "Items"
 ITM_ITERATIONS = "Iterations"
 ITM_K1 = "K1"
 ITM_K2 = "K2"
 ITM_K3 = "K3"
@@ -482,14 +485,15 @@
 ITM_OPERATING_SYSTEM = "OperatingSystem"
 ITM_OPERATION = "Operation"
 ITM_OPTICAL_AXIS = "OpticalAxis"
 ITM_OPTIMAL_FILTER_SIZE = "OptimalFilterSize"
 ITM_OPTIMIZATION_PROFILE = "OptimizationProfile"
 ITM_OPTIONS = "Options"
 ITM_OR = "Or"
+ITM_ORDER = "Order"
 ITM_ORIGIN = "Origin"
 ITM_OUTER_SIZE = "OuterSize"
 ITM_OUTPUT = "Output"
 ITM_OUTPUT_ASSIGNMENTS = "OutputAssignments"
 ITM_OUTPUT_DETECTIONS = "OutputDetections"
 ITM_OVERFLOW_POLICY = "OverflowPolicy"
 ITM_OVERLAY = "Overlay"
@@ -627,14 +631,15 @@
 ITM_SOURCE = "Source"
 ITM_SPECKLE_REMOVAL = "SpeckleRemoval"
 ITM_SPECULAR = "Specular"
 ITM_SPLIT_ROTATION = "SplitRotation"
 ITM_SSID = "Ssid"
 ITM_START_DAEMON = "StartDaemon"
 ITM_STATIC_BUFFER_COUNT = "StaticBufferCount"
+ITM_STATIC_BUFFER_SIZE = "StaticBufferSize"
 ITM_STATIC_BUFFERS = "StaticBuffers"
 ITM_STATUS = "Status"
 ITM_STEREO = "Stereo"
 ITM_STEREO_CALIBRATION = "StereoCalibration"
 ITM_STEREO_CALIBRATION_ONLY = "StereoCalibrationOnly"
 ITM_STEREO_EXTRINSIC = "StereoExtrinsic"
 ITM_STEREO_INTRINSIC = "StereoIntrinsic"
@@ -642,14 +647,15 @@
 ITM_STEREO_PATTERN_COUNT = "StereoPatternCount"
 ITM_STOP_DAEMON = "StopDaemon"
 ITM_SUBSAMPLING = "Subsampling"
 ITM_SUBSET = "Subset"
 ITM_SUPPLEMENTARY = "Supplementary"
 ITM_SURFACE_CONNECTIVITY = "SurfaceConnectivity"
 ITM_SYMBOL = "Symbol"
+ITM_SYMMETRIES = "Symmetries"
 ITM_SYSTEM_INFO = "SystemInfo"
 ITM_T1 = "T1"
 ITM_T2 = "T2"
 ITM_TARGET = "Target"
 ITM_TARGET_BRIGHTNESS = "TargetBrightness"
 ITM_TEMPERATURE = "Temperature"
 ITM_TEMPLATE_COUNT = "TemplateCount"
@@ -766,22 +772,24 @@
 VAL_DISCARD_NEW = "DiscardNew"
 VAL_DISCARD_OLD = "DiscardOld"
 VAL_DISCONNECT = "Disconnect"
 VAL_DISCONNECTED = "Disconnected"
 VAL_DOWN = "Down"
 VAL_ENABLED = "Enabled"
 VAL_ENSENSO = "Ensenso"
+VAL_ERROR = "Error"
 VAL_ETHERNET = "Ethernet"
 VAL_EUCLIDEAN = "Euclidean"
 VAL_FACTORY_RESET = "FactoryReset"
 VAL_FALLING_EDGE = "FallingEdge"
 VAL_FILE = "File"
 VAL_FIND = "Find"
 VAL_FIXED = "Fixed"
 VAL_FLEX_VIEW2 = "FlexView2"
+VAL_FLEX_VIEW3 = "FlexView3"
 VAL_FLEXIBLE = "Flexible"
 VAL_FLOAT = "Float"
 VAL_FORCE = "Force"
 VAL_GENERATE_MODEL = "GenerateModel"
 VAL_GET_MODEL_DISTANCE = "GetModelDistance"
 VAL_GRID_HEIGHT = "GridHeight"
 VAL_GRID_SPACING = "GridSpacing"
@@ -794,14 +802,15 @@
 VAL_IGNORE = "Ignore"
 VAL_IMAGE_POSITION = "ImagePosition"
 VAL_IMMEDIATE = "Immediate"
 VAL_IN_USE = "InUse"
 VAL_INDEX = "Index"
 VAL_INFO = "Info"
 VAL_INPUT = "Input"
+VAL_INTERNAL = "Internal"
 VAL_ITEM = "Item"
 VAL_LEFT = "Left"
 VAL_LEFT_TO_RIGHT = "LeftToRight"
 VAL_LINK = "Link"
 VAL_LINK_HIDDEN = "LinkHidden"
 VAL_LIST_MODELS = "ListModels"
 VAL_LOAD_MODEL = "LoadModel"
@@ -875,14 +884,15 @@
 VAL_UNKNOWN = "Unknown"
 VAL_UNTRIGGERED = "Untriggered"
 VAL_UP = "Up"
 VAL_UPDATE_ACCESS_POINT = "UpdateAccessPoint"
 VAL_USER_DATA = "UserData"
 VAL_VALIDATE = "Validate"
 VAL_VIRTUAL = "Virtual"
+VAL_WARNING = "Warning"
 VAL_WORKSPACE = "Workspace"
 VAL_WORLD_Z = "WorldZ"
 VAL_WPA2_PSK = "Wpa2Psk"
 VAL_X = "X"
 VAL_X_NEGATIVE = "XNegative"
 VAL_X_POSITIVE = "XPositive"
 VAL_X_ROTATION_SYMMETRIC = "XRotationSymmetric"
```

### Comparing `nxlib-3.4.743/nxlib/context.py` & `nxlib-3.5.1375/nxlib/context.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,23 @@
     ``with`` statement, which automatically initializes the NxLib and takes care
     of the exception handling.
 
     Args:
         path (str, optional): The path to the NxLib shared library.
             Defaults to None.
     """
-    def __enter__(self, path=None):
-        api.initialize(path=path)
+    def __init__(self, path=None):
+        self._path = path
+
+    def __enter__(self):
+        api.initialize(path=self._path)
         return api
 
     def __exit__(self, exc_type, exc_value, exc_tb):
+        api.finalize()
         return _handle_exception(exc_type, exc_value, exc_tb)
 
 
 class NxLibRemote:
     """
     This class offers a simple to use interface for interacting with a remote
     NxLib. It implements the context manager protocol and thus can be used
```

### Comparing `nxlib-3.4.743/nxlib/exception.py` & `nxlib-3.5.1375/nxlib/exception.py`

 * *Files identical despite different names*

### Comparing `nxlib-3.4.743/nxlib/item.py` & `nxlib-3.5.1375/nxlib/item.py`

 * *Files identical despite different names*

### Comparing `nxlib-3.4.743/nxlib/log.py` & `nxlib-3.5.1375/nxlib/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         bytes from the debug buffer. Therefore the API function is called twice,
         once to determine the number of bytes held by the debug buffer and a
         second time to actually read and clear the debug buffer.
 
         Note:
             A warning is printed if the debug buffer overflowed and warnings
             are enabled. In this case the debug buffer size should be increased
-            via the tree item :doc:`/Debug/BufferSize <tree:debug/buffersize>`.
+            via the tree item :doc:`/Debug/BacklogSize <tree:debug/backlogsize>`.
 
         Returns:
             bytes: The debug buffers content as bytes.
         """
         buffer_size = 0
         for clear_read in [np.int32(0), np.int32(1)]:
             buffer = np.zeros(buffer_size, dtype=np.uint8, order="C")
```

### Comparing `nxlib-3.4.743/nxlib.egg-info/PKG-INFO` & `nxlib-3.5.1375/nxlib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nxlib
-Version: 3.4.743
+Version: 3.5.1375
 Summary: Python interface to interact with the Ensenso NxLib
 Home-page: https://www.ensenso.com/python-api
 Author: Optonic GmbH
 Author-email: support@optonic.com
 License: MIT
 Description: > **Announcement:**
         With Ensenso SDK version 3.3 we stop the maintenance of our
```

### Comparing `nxlib-3.4.743/setup.py` & `nxlib-3.5.1375/setup.py`

 * *Files identical despite different names*

