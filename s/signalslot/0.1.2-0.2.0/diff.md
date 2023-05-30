# Comparing `tmp/signalslot-0.1.2.tar.gz` & `tmp/signalslot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/signalslot-0.1.2.tar", last modified: Thu May 16 13:04:10 2019, max compression
+gzip compressed data, was "signalslot-0.2.0.tar", last modified: Tue May 30 13:21:28 2023, max compression
```

## Comparing `signalslot-0.1.2.tar` & `signalslot-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 sliim     (1000) sliim     (1000)        0 2019-05-16 13:04:10.000000 signalslot-0.1.2/
--rw-r--r--   0 sliim     (1000) sliim     (1000)       71 2019-05-15 10:43:31.000000 signalslot-0.1.2/MANIFEST.in
--rw-r--r--   0 sliim     (1000) sliim     (1000)     1491 2019-05-15 10:43:31.000000 signalslot-0.1.2/README.rst
--rw-r--r--   0 sliim     (1000) sliim     (1000)      438 2019-05-16 13:04:10.000000 signalslot-0.1.2/setup.cfg
--rw-r--r--   0 sliim     (1000) sliim     (1000)     2544 2019-05-16 13:04:10.000000 signalslot-0.1.2/PKG-INFO
--rw-r--r--   0 sliim     (1000) sliim     (1000)     1008 2019-05-16 12:49:15.000000 signalslot-0.1.2/setup.py
--rw-r--r--   0 sliim     (1000) sliim     (1000)      109 2019-05-16 12:49:15.000000 signalslot-0.1.2/test_requirements.txt
-drwxr-xr-x   0 sliim     (1000) sliim     (1000)        0 2019-05-16 13:04:10.000000 signalslot-0.1.2/signalslot/
--rw-r--r--   0 sliim     (1000) sliim     (1000)     1862 2019-05-15 10:43:31.000000 signalslot-0.1.2/signalslot/slot.py
--rw-r--r--   0 sliim     (1000) sliim     (1000)     5314 2019-05-15 10:43:31.000000 signalslot-0.1.2/signalslot/tests.py
-drwxr-xr-x   0 sliim     (1000) sliim     (1000)        0 2019-05-16 13:04:10.000000 signalslot-0.1.2/signalslot/contrib/
-drwxr-xr-x   0 sliim     (1000) sliim     (1000)        0 2019-05-16 13:04:10.000000 signalslot-0.1.2/signalslot/contrib/task/
--rw-r--r--   0 sliim     (1000) sliim     (1000)     1955 2019-05-15 10:43:31.000000 signalslot-0.1.2/signalslot/contrib/task/task.py
--rw-r--r--   0 sliim     (1000) sliim     (1000)       23 2019-05-15 10:43:31.000000 signalslot-0.1.2/signalslot/contrib/task/__init__.py
--rw-r--r--   0 sliim     (1000) sliim     (1000)     5523 2019-05-15 10:43:31.000000 signalslot-0.1.2/signalslot/contrib/task/test.py
--rw-r--r--   0 sliim     (1000) sliim     (1000)        0 2019-05-15 10:43:31.000000 signalslot-0.1.2/signalslot/contrib/__init__.py
--rw-r--r--   0 sliim     (1000) sliim     (1000)      271 2019-05-16 12:48:13.000000 signalslot-0.1.2/signalslot/__init__.py
--rw-r--r--   0 sliim     (1000) sliim     (1000)      889 2019-05-15 10:43:31.000000 signalslot-0.1.2/signalslot/exceptions.py
--rw-r--r--   0 sliim     (1000) sliim     (1000)     4309 2019-05-15 10:43:31.000000 signalslot-0.1.2/signalslot/signal.py
-drwxr-xr-x   0 sliim     (1000) sliim     (1000)        0 2019-05-16 13:04:10.000000 signalslot-0.1.2/signalslot.egg-info/
--rw-r--r--   0 sliim     (1000) sliim     (1000)      488 2019-05-16 13:04:10.000000 signalslot-0.1.2/signalslot.egg-info/SOURCES.txt
--rw-r--r--   0 sliim     (1000) sliim     (1000)     2544 2019-05-16 13:04:10.000000 signalslot-0.1.2/signalslot.egg-info/PKG-INFO
--rw-r--r--   0 sliim     (1000) sliim     (1000)        1 2019-05-16 13:04:10.000000 signalslot-0.1.2/signalslot.egg-info/dependency_links.txt
--rw-r--r--   0 sliim     (1000) sliim     (1000)       28 2019-05-16 13:04:10.000000 signalslot-0.1.2/signalslot.egg-info/requires.txt
--rw-r--r--   0 sliim     (1000) sliim     (1000)       11 2019-05-16 13:04:10.000000 signalslot-0.1.2/signalslot.egg-info/top_level.txt
--rw-r--r--   0 sliim     (1000) sliim     (1000)     1491 2019-05-15 10:43:31.000000 signalslot-0.1.2/README
--rw-r--r--   0 sliim     (1000) sliim     (1000)      616 2019-05-16 12:48:58.000000 signalslot-0.1.2/CHANGELOG
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-30 13:21:28.852963 signalslot-0.2.0/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      616 2023-04-26 05:52:00.000000 signalslot-0.2.0/CHANGELOG
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1052 2023-04-26 05:52:00.000000 signalslot-0.2.0/LICENSE
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       71 2023-04-26 05:52:00.000000 signalslot-0.2.0/MANIFEST.in
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2139 2023-05-30 13:21:28.852963 signalslot-0.2.0/PKG-INFO
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1502 2023-04-26 05:52:00.000000 signalslot-0.2.0/README
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1502 2023-04-26 05:52:00.000000 signalslot-0.2.0/README.rst
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      438 2023-05-30 13:21:28.852963 signalslot-0.2.0/setup.cfg
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1011 2023-04-26 05:52:00.000000 signalslot-0.2.0/setup.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-30 13:21:28.849630 signalslot-0.2.0/signalslot/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      271 2023-04-26 05:52:35.000000 signalslot-0.2.0/signalslot/__init__.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-30 13:21:28.849630 signalslot-0.2.0/signalslot/contrib/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)        0 2023-04-26 05:52:00.000000 signalslot-0.2.0/signalslot/contrib/__init__.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-30 13:21:28.852963 signalslot-0.2.0/signalslot/contrib/task/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       23 2023-04-26 05:52:00.000000 signalslot-0.2.0/signalslot/contrib/task/__init__.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1955 2023-04-26 05:52:00.000000 signalslot-0.2.0/signalslot/contrib/task/task.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     5523 2023-04-26 05:52:00.000000 signalslot-0.2.0/signalslot/contrib/task/test.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      889 2023-04-26 05:52:00.000000 signalslot-0.2.0/signalslot/exceptions.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     4310 2023-04-26 05:52:00.000000 signalslot-0.2.0/signalslot/signal.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     1668 2023-04-26 05:52:00.000000 signalslot-0.2.0/signalslot/slot.py
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     5314 2023-04-26 05:52:00.000000 signalslot-0.2.0/signalslot/tests.py
+drwxr-xr-x   0 jpic      (1000) jpic      (1000)        0 2023-05-30 13:21:28.849630 signalslot-0.2.0/signalslot.egg-info/
+-rw-r--r--   0 jpic      (1000) jpic      (1000)     2139 2023-05-30 13:21:28.000000 signalslot-0.2.0/signalslot.egg-info/PKG-INFO
+-rw-r--r--   0 jpic      (1000) jpic      (1000)      496 2023-05-30 13:21:28.000000 signalslot-0.2.0/signalslot.egg-info/SOURCES.txt
+-rw-r--r--   0 jpic      (1000) jpic      (1000)        1 2023-05-30 13:21:28.000000 signalslot-0.2.0/signalslot.egg-info/dependency_links.txt
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       14 2023-05-30 13:21:28.000000 signalslot-0.2.0/signalslot.egg-info/requires.txt
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       11 2023-05-30 13:21:28.000000 signalslot-0.2.0/signalslot.egg-info/top_level.txt
+-rw-r--r--   0 jpic      (1000) jpic      (1000)       84 2023-04-26 05:52:00.000000 signalslot-0.2.0/test_requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `signalslot-0.1.2/README.rst` & `signalslot-0.2.0/README`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 .. image:: https://secure.travis-ci.org/Numergy/signalslot.png?branch=master
     :target: http://travis-ci.org/Numergy/signalslot
-.. image:: https://pypip.in/d/signalslot/badge.png
+.. image:: https://img.shields.io/pypi/dm/signalslot.svg
     :target: https://crate.io/packages/signalslot
-.. image:: https://pypip.in/v/signalslot/badge.png   
+.. image:: https://img.shields.io/pypi/v/signalslot.svg   
     :target: https://crate.io/packages/signalslot
 .. image:: https://coveralls.io/repos/Numergy/signalslot/badge.png 
     :target: https://coveralls.io/r/Numergy/signalslot
 .. image:: https://readthedocs.org/projects/signalslot/badge/?version=latest
     :target: https://signalslot.readthedocs.org/en/latest
 
 signalslot: simple Signal/Slot implementation for Python
```

### Comparing `signalslot-0.1.2/PKG-INFO` & `signalslot-0.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,68 +1,67 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: signalslot
-Version: 0.1.2
+Version: 0.2.0
 Summary: Simple Signal/Slot implementation
 Home-page: https://github.com/numergy/signalslot
-Author: UNKNOWN
-Author-email: UNKNOWN
 License: MIT
-Description: .. image:: https://secure.travis-ci.org/Numergy/signalslot.png?branch=master
-            :target: http://travis-ci.org/Numergy/signalslot
-        .. image:: https://pypip.in/d/signalslot/badge.png
-            :target: https://crate.io/packages/signalslot
-        .. image:: https://pypip.in/v/signalslot/badge.png   
-            :target: https://crate.io/packages/signalslot
-        .. image:: https://coveralls.io/repos/Numergy/signalslot/badge.png 
-            :target: https://coveralls.io/r/Numergy/signalslot
-        .. image:: https://readthedocs.org/projects/signalslot/badge/?version=latest
-            :target: https://signalslot.readthedocs.org/en/latest
-        
-        signalslot: simple Signal/Slot implementation for Python
-        ========================================================
-        
-        This package provides a simple and stupid implementation of the `Signal/Slot
-        pattern <http://en.wikipedia.org/wiki/Signals_and_slots>`_ for Python.
-        Wikipedia has a nice introduction:
-        
-            Signals and slots is a language construct introduced in Qt for
-            communication between objects[1] which makes it easy to implement the
-            Observer pattern while avoiding boilerplate code. 
-        
-        Rationale against Signal/Slot is detailed in the "Pattern"
-        section of the documentation.
-        
-        Install
-        -------
-        
-        Install latest stable version::
-        
-            pip install signalslot
-        
-        Install development version::
-        
-            pip install -e git+https://github.com/Numergy/signalslot
-        
-        Upgrade
-        -------
-        
-        Upgrade to the last stable version::
-        
-            pip install -U signalslot
-        
-        Uninstall
-        ---------
-        
-        ::
-        
-            pip uninstall signalslot
-        
 Keywords: signal slot
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.4
+License-File: LICENSE
+
+.. image:: https://secure.travis-ci.org/Numergy/signalslot.png?branch=master
+    :target: http://travis-ci.org/Numergy/signalslot
+.. image:: https://img.shields.io/pypi/dm/signalslot.svg
+    :target: https://crate.io/packages/signalslot
+.. image:: https://img.shields.io/pypi/v/signalslot.svg   
+    :target: https://crate.io/packages/signalslot
+.. image:: https://coveralls.io/repos/Numergy/signalslot/badge.png 
+    :target: https://coveralls.io/r/Numergy/signalslot
+.. image:: https://readthedocs.org/projects/signalslot/badge/?version=latest
+    :target: https://signalslot.readthedocs.org/en/latest
+
+signalslot: simple Signal/Slot implementation for Python
+========================================================
+
+This package provides a simple and stupid implementation of the `Signal/Slot
+pattern <http://en.wikipedia.org/wiki/Signals_and_slots>`_ for Python.
+Wikipedia has a nice introduction:
+
+    Signals and slots is a language construct introduced in Qt for
+    communication between objects[1] which makes it easy to implement the
+    Observer pattern while avoiding boilerplate code. 
+
+Rationale against Signal/Slot is detailed in the "Pattern"
+section of the documentation.
+
+Install
+-------
+
+Install latest stable version::
+
+    pip install signalslot
+
+Install development version::
+
+    pip install -e git+https://github.com/Numergy/signalslot
+
+Upgrade
+-------
+
+Upgrade to the last stable version::
+
+    pip install -U signalslot
+
+Uninstall
+---------
+
+::
+
+    pip uninstall signalslot
```

### Comparing `signalslot-0.1.2/setup.py` & `signalslot-0.2.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,21 +17,20 @@
     packages=find_packages(),
     include_package_data=True,
     license='MIT',
     keywords='signal slot',
     install_requires=[
         'six',
         'contexter',
-        'weakrefmethod',
     ],
+    python_requires='>=3.4',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 3',
         'Topic :: Software Development :: Libraries :: Python Modules',
     ],
 )
-
```

### Comparing `signalslot-0.1.2/signalslot/slot.py` & `signalslot-0.2.0/signalslot/slot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 """
 Module defining the Slot class.
 """
 
 import types
 import weakref
-import sys
 
 from .signal import BaseSlot
-
-# We cannot test a branch for Python >= 3.4 in Python < 3.4.
-if sys.version_info < (3, 4):  # pragma: no cover
-    from weakrefmethod import WeakMethod
-else:  # pragma: no cover
-    from weakref import WeakMethod
+from weakref import WeakMethod
 
 
 class Slot(BaseSlot):
     """
     A slot is a callable object that manages a connection to a signal.
     If weak is true or the slot is a subclass of weakref.ref, the slot
     is automatically de-referenced to the called function.
```

### Comparing `signalslot-0.1.2/signalslot/tests.py` & `signalslot-0.2.0/signalslot/tests.py`

 * *Files identical despite different names*

### Comparing `signalslot-0.1.2/signalslot/contrib/task/task.py` & `signalslot-0.2.0/signalslot/contrib/task/task.py`

 * *Files identical despite different names*

### Comparing `signalslot-0.1.2/signalslot/contrib/task/test.py` & `signalslot-0.2.0/signalslot/contrib/task/test.py`

 * *Files identical despite different names*

### Comparing `signalslot-0.1.2/signalslot/exceptions.py` & `signalslot-0.2.0/signalslot/exceptions.py`

 * *Files identical despite different names*

### Comparing `signalslot-0.1.2/signalslot/signal.py` & `signalslot-0.2.0/signalslot/signal.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             return list(slots)
 
     def connect(self, slot):
         """
         Connect a callback ``slot`` to this signal.
         """
         if not isinstance(slot, BaseSlot) and \
-                inspect.getargspec(slot).keywords is None:
+                inspect.getfullargspec(slot).varkw is None:
             raise exceptions.SlotMustAcceptKeywords(self, slot)
 
         with self._slots_lk:
             if not self.is_connected(slot):
                 self._slots.append(slot)
 
     def is_connected(self, slot):
```

### Comparing `signalslot-0.1.2/signalslot.egg-info/PKG-INFO` & `signalslot-0.2.0/signalslot.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,68 +1,67 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: signalslot
-Version: 0.1.2
+Version: 0.2.0
 Summary: Simple Signal/Slot implementation
 Home-page: https://github.com/numergy/signalslot
-Author: UNKNOWN
-Author-email: UNKNOWN
 License: MIT
-Description: .. image:: https://secure.travis-ci.org/Numergy/signalslot.png?branch=master
-            :target: http://travis-ci.org/Numergy/signalslot
-        .. image:: https://pypip.in/d/signalslot/badge.png
-            :target: https://crate.io/packages/signalslot
-        .. image:: https://pypip.in/v/signalslot/badge.png   
-            :target: https://crate.io/packages/signalslot
-        .. image:: https://coveralls.io/repos/Numergy/signalslot/badge.png 
-            :target: https://coveralls.io/r/Numergy/signalslot
-        .. image:: https://readthedocs.org/projects/signalslot/badge/?version=latest
-            :target: https://signalslot.readthedocs.org/en/latest
-        
-        signalslot: simple Signal/Slot implementation for Python
-        ========================================================
-        
-        This package provides a simple and stupid implementation of the `Signal/Slot
-        pattern <http://en.wikipedia.org/wiki/Signals_and_slots>`_ for Python.
-        Wikipedia has a nice introduction:
-        
-            Signals and slots is a language construct introduced in Qt for
-            communication between objects[1] which makes it easy to implement the
-            Observer pattern while avoiding boilerplate code. 
-        
-        Rationale against Signal/Slot is detailed in the "Pattern"
-        section of the documentation.
-        
-        Install
-        -------
-        
-        Install latest stable version::
-        
-            pip install signalslot
-        
-        Install development version::
-        
-            pip install -e git+https://github.com/Numergy/signalslot
-        
-        Upgrade
-        -------
-        
-        Upgrade to the last stable version::
-        
-            pip install -U signalslot
-        
-        Uninstall
-        ---------
-        
-        ::
-        
-            pip uninstall signalslot
-        
 Keywords: signal slot
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.4
+License-File: LICENSE
+
+.. image:: https://secure.travis-ci.org/Numergy/signalslot.png?branch=master
+    :target: http://travis-ci.org/Numergy/signalslot
+.. image:: https://img.shields.io/pypi/dm/signalslot.svg
+    :target: https://crate.io/packages/signalslot
+.. image:: https://img.shields.io/pypi/v/signalslot.svg   
+    :target: https://crate.io/packages/signalslot
+.. image:: https://coveralls.io/repos/Numergy/signalslot/badge.png 
+    :target: https://coveralls.io/r/Numergy/signalslot
+.. image:: https://readthedocs.org/projects/signalslot/badge/?version=latest
+    :target: https://signalslot.readthedocs.org/en/latest
+
+signalslot: simple Signal/Slot implementation for Python
+========================================================
+
+This package provides a simple and stupid implementation of the `Signal/Slot
+pattern <http://en.wikipedia.org/wiki/Signals_and_slots>`_ for Python.
+Wikipedia has a nice introduction:
+
+    Signals and slots is a language construct introduced in Qt for
+    communication between objects[1] which makes it easy to implement the
+    Observer pattern while avoiding boilerplate code. 
+
+Rationale against Signal/Slot is detailed in the "Pattern"
+section of the documentation.
+
+Install
+-------
+
+Install latest stable version::
+
+    pip install signalslot
+
+Install development version::
+
+    pip install -e git+https://github.com/Numergy/signalslot
+
+Upgrade
+-------
+
+Upgrade to the last stable version::
+
+    pip install -U signalslot
+
+Uninstall
+---------
+
+::
+
+    pip uninstall signalslot
```

### Comparing `signalslot-0.1.2/README` & `signalslot-0.2.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 .. image:: https://secure.travis-ci.org/Numergy/signalslot.png?branch=master
     :target: http://travis-ci.org/Numergy/signalslot
-.. image:: https://pypip.in/d/signalslot/badge.png
+.. image:: https://img.shields.io/pypi/dm/signalslot.svg
     :target: https://crate.io/packages/signalslot
-.. image:: https://pypip.in/v/signalslot/badge.png   
+.. image:: https://img.shields.io/pypi/v/signalslot.svg   
     :target: https://crate.io/packages/signalslot
 .. image:: https://coveralls.io/repos/Numergy/signalslot/badge.png 
     :target: https://coveralls.io/r/Numergy/signalslot
 .. image:: https://readthedocs.org/projects/signalslot/badge/?version=latest
     :target: https://signalslot.readthedocs.org/en/latest
 
 signalslot: simple Signal/Slot implementation for Python
```

### Comparing `signalslot-0.1.2/CHANGELOG` & `signalslot-0.2.0/CHANGELOG`

 * *Files identical despite different names*

