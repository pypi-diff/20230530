# Comparing `tmp/VisageSnap-0.3.0.tar.gz` & `tmp/VisageSnap-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VisageSnap-0.3.0.tar", last modified: Mon May 29 09:39:46 2023, max compression
+gzip compressed data, was "VisageSnap-0.3.1.tar", last modified: Tue May 30 06:14:08 2023, max compression
```

## Comparing `VisageSnap-0.3.0.tar` & `VisageSnap-0.3.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:39:46.746438 VisageSnap-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-29 09:39:46.746438 VisageSnap-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:39:46.742438 VisageSnap-0.3.0/VisageSnap/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:39:46.742438 VisageSnap-0.3.0/VisageSnap/image/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/image/imageloader.py
--rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:39:46.746438 VisageSnap-0.3.0/VisageSnap/model/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/model/modelhandler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:39:46.746438 VisageSnap-0.3.0/VisageSnap/processor/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/processor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/processor/faceprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/processor/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/processor/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/VisageSnap/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:39:46.742438 VisageSnap-0.3.0/VisageSnap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-29 09:39:46.000000 VisageSnap-0.3.0/VisageSnap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-29 09:39:46.000000 VisageSnap-0.3.0/VisageSnap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 09:39:46.000000 VisageSnap-0.3.0/VisageSnap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-29 09:39:46.000000 VisageSnap-0.3.0/VisageSnap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-29 09:39:46.000000 VisageSnap-0.3.0/VisageSnap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 09:39:46.746438 VisageSnap-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 09:39:46.746438 VisageSnap-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-29 09:39:31.000000 VisageSnap-0.3.0/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:14:08.975130 VisageSnap-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-30 06:14:08.975130 VisageSnap-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:14:08.971130 VisageSnap-0.3.1/VisageSnap/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:14:08.971130 VisageSnap-0.3.1/VisageSnap/image/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/image/imageloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2530 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:14:08.971130 VisageSnap-0.3.1/VisageSnap/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/model/modelhandler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:14:08.975130 VisageSnap-0.3.1/VisageSnap/processor/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/processor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/processor/faceprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3979 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/processor/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/processor/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/VisageSnap/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:14:08.971130 VisageSnap-0.3.1/VisageSnap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-05-30 06:14:08.000000 VisageSnap-0.3.1/VisageSnap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-30 06:14:08.000000 VisageSnap-0.3.1/VisageSnap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 06:14:08.000000 VisageSnap-0.3.1/VisageSnap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-30 06:14:08.000000 VisageSnap-0.3.1/VisageSnap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-30 06:14:08.000000 VisageSnap-0.3.1/VisageSnap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 06:14:08.975130 VisageSnap-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 06:14:08.975130 VisageSnap-0.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-30 06:13:54.000000 VisageSnap-0.3.1/tests/test.py
```

### Comparing `VisageSnap-0.3.0/LICENSE` & `VisageSnap-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `VisageSnap-0.3.0/PKG-INFO` & `VisageSnap-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisageSnap
-Version: 0.3.0
+Version: 0.3.1
 Summary: Face Classification package
 Home-page: https://github.com/asheswook/VisageSnap
 Author: Jaewook Lee
 Author-email: me@jwlee.xyz
 Project-URL: Bug Tracker, https://github.com/asheswook/VisageSnap/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -85,21 +85,21 @@
 
 ```python
 vs.load_model()
 ```
 
 Train with the picture files in the directory.
 
-```
+```python
 vs.train_labeled_data()
 ```
 
 If you want to train with unlabeled data, you can also try to like this:
 
-```
+```python
 vs.train_unlabeled_data()
 ```
 
 **Identification predictions**
 
 Put the picture files you want to predict into the directory.
```

### Comparing `VisageSnap-0.3.0/README.md` & `VisageSnap-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -70,21 +70,21 @@
 
 ```python
 vs.load_model()
 ```
 
 Train with the picture files in the directory.
 
-```
+```python
 vs.train_labeled_data()
 ```
 
 If you want to train with unlabeled data, you can also try to like this:
 
-```
+```python
 vs.train_unlabeled_data()
 ```
 
 **Identification predictions**
 
 Put the picture files you want to predict into the directory.
```

### Comparing `VisageSnap-0.3.0/VisageSnap/classes.py` & `VisageSnap-0.3.1/VisageSnap/classes.py`

 * *Files identical despite different names*

### Comparing `VisageSnap-0.3.0/VisageSnap/image/imageloader.py` & `VisageSnap-0.3.1/VisageSnap/image/imageloader.py`

 * *Files identical despite different names*

### Comparing `VisageSnap-0.3.0/VisageSnap/main.py` & `VisageSnap-0.3.1/VisageSnap/main.py`

 * *Files identical despite different names*

### Comparing `VisageSnap-0.3.0/VisageSnap/model/modelhandler.py` & `VisageSnap-0.3.1/VisageSnap/model/modelhandler.py`

 * *Files identical despite different names*

### Comparing `VisageSnap-0.3.0/VisageSnap/processor/faceprocessor.py` & `VisageSnap-0.3.1/VisageSnap/processor/faceprocessor.py`

 * *Files identical despite different names*

### Comparing `VisageSnap-0.3.0/VisageSnap/processor/predictor.py` & `VisageSnap-0.3.1/VisageSnap/processor/predictor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from ..classes import Face, GlobalState, Directory, From, To, As
 from ..utils import isimage
 from .faceprocessor import FaceProcessor
 import numpy as np
 import face_recognition
 import os
+from functools import cache
+
 
 class Predictor(FaceProcessor):
     def __init__(self, globalState: GlobalState = None, directory: Directory = None):
         super().__init__(globalState)
 
         self.__state = globalState
         self.__directory = directory
@@ -31,81 +33,86 @@
         This function returns the distance between two encodings.
 
         Parameters
         ----------
         encoding1 (np.array) : encoding1.
         encoding2 (np.array) : encoding2.
         """
-        assert isinstance(encoding1, np.ndarray), "parameter must be numpy array."
-        assert isinstance(encoding2, np.ndarray), "parameter must be numpy array."
+        assert isinstance(
+            encoding1, np.ndarray), "parameter must be numpy array."
+        assert isinstance(
+            encoding2, np.ndarray), "parameter must be numpy array."
 
         return np.linalg.norm(encoding1 - encoding2)
 
     def __isNotUnknown(self, encoding) -> bool:
         """
         This function checks whether the encoding is unknown.
 
         Parameters
         ----------
         encoding (np.array) : target encoding.
         """
-        assert isinstance(encoding, np.ndarray), "parameter must be numpy array."
+        assert isinstance(
+            encoding, np.ndarray), "parameter must be numpy array."
 
         min_distance = 1
         for face in self.gen_faces():
-            average = self.__get_average(face) # 저장된 얼굴 평균 구하고
-            distance = self.__get_distance(encoding, average) # 타겟과의 거리를 구한다
+            average = self.__get_average(face)  # 저장된 얼굴 평균 구하고
+            distance = self.__get_distance(encoding, average)  # 타겟과의 거리를 구한다
             if distance < min_distance:
                 min_distance = distance
 
         if min_distance < self.threshold:
-            return True # 모르는 사람이 아니다
-        return False # 모르는 사람이다
+            return True  # 모르는 사람이 아니다
+        return False  # 모르는 사람이다
 
     def __predict(self, image: np.ndarray) -> list:
         assert isinstance(image, np.ndarray), "parameter must be numpy array."
 
         target_encodings = face_recognition.face_encodings(image)
         if len(target_encodings) == 0:
             return None
 
         result = []
         for target_encoding in target_encodings:
-            if self.__isNotUnknown(target_encoding): # 모르는 사람이 아니면
+            if self.__isNotUnknown(target_encoding):  # 모르는 사람이 아니면
                 result.append(self.__state.model.predict([target_encoding])[0])
             else:
                 result.append(-1)
 
         return result
-    
+
     def predict_image(self, image: np.ndarray) -> list:
         assert isinstance(image, np.ndarray), "parameter must be numpy array."
 
         return self.__predict(image)
-    
+
     def predict_encoding(self, encoding: np.ndarray) -> int:
         assert isinstance(encoding, np.ndarray), "parameter must be numpy array."
 
-        prediction = self.__predict([encoding])
-
-        return -1 if -1 in prediction else prediction[0]
-    
+        if self.__isNotUnknown(encoding):
+            return self.__state.model.predict([encoding])[0]
+        else:
+            return -1
 
     def predict_all(self) -> dict:
         result = {}
         for filename in os.listdir(self.__directory.predict):
             if isimage(filename) == False:
                 return
 
-            image = face_recognition.load_image_file(os.path.join(self.__directory.predict, filename))
+            image = face_recognition.load_image_file(
+                os.path.join(self.__directory.predict, filename))
             prediction = self.__predict(image)
 
             if prediction == None:
-                raise("There is no face in the image.")
+                raise ("There is no face in the image.")
 
             if len(prediction) == 1:
-                result[filename] = self.convert_labelType(prediction[0], To.NAME)
+                result[filename] = self.convert_labelType(
+                    prediction[0], To.NAME)
             else:
                 result[filename] = []
                 for p in prediction:
                     result[filename].append(self.convert_labelType(p, To.NAME))
-        return result
+        return result
```

### Comparing `VisageSnap-0.3.0/VisageSnap/processor/trainer.py` & `VisageSnap-0.3.1/VisageSnap/processor/trainer.py`

 * *Files identical despite different names*

### Comparing `VisageSnap-0.3.0/VisageSnap/utils.py` & `VisageSnap-0.3.1/VisageSnap/utils.py`

 * *Files identical despite different names*

### Comparing `VisageSnap-0.3.0/VisageSnap.egg-info/PKG-INFO` & `VisageSnap-0.3.1/VisageSnap.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VisageSnap
-Version: 0.3.0
+Version: 0.3.1
 Summary: Face Classification package
 Home-page: https://github.com/asheswook/VisageSnap
 Author: Jaewook Lee
 Author-email: me@jwlee.xyz
 Project-URL: Bug Tracker, https://github.com/asheswook/VisageSnap/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -85,21 +85,21 @@
 
 ```python
 vs.load_model()
 ```
 
 Train with the picture files in the directory.
 
-```
+```python
 vs.train_labeled_data()
 ```
 
 If you want to train with unlabeled data, you can also try to like this:
 
-```
+```python
 vs.train_unlabeled_data()
 ```
 
 **Identification predictions**
 
 Put the picture files you want to predict into the directory.
```

### Comparing `VisageSnap-0.3.0/VisageSnap.egg-info/SOURCES.txt` & `VisageSnap-0.3.1/VisageSnap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `VisageSnap-0.3.0/setup.py` & `VisageSnap-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     'scikit-learn',
     'dlib',
     'face_recognition',
 ]
 
 setuptools.setup(
     name='VisageSnap',
-    version='0.3.0',
+    version='0.3.1',
     author='Jaewook Lee',
     author_email='me@jwlee.xyz',
     description='Face Classification package',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/asheswook/VisageSnap',
     project_urls={
```

