# Comparing `tmp/openirt-0.1.4.tar.gz` & `tmp/openirt-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openirt-0.1.4.tar", last modified: Tue May 30 08:51:20 2023, max compression
+gzip compressed data, was "openirt-0.1.5.tar", last modified: Tue May 30 08:57:23 2023, max compression
```

## Comparing `openirt-0.1.4.tar` & `openirt-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:51:20.502569 openirt-0.1.4/
--rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-30 08:51:02.000000 openirt-0.1.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)      256 2023-05-30 08:51:20.502569 openirt-0.1.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-30 08:51:02.000000 openirt-0.1.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:51:20.501569 openirt-0.1.4/openirt/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 08:51:02.000000 openirt-0.1.4/openirt/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6938 2023-05-30 08:51:02.000000 openirt-0.1.4/openirt/bayes3PL.py
--rw-rw-rw-   0 root         (0) root         (0)     2081 2023-05-30 08:51:02.000000 openirt-0.1.4/openirt/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     3932 2023-05-30 08:51:02.000000 openirt-0.1.4/openirt/irt_instance.py
--rw-rw-rw-   0 root         (0) root         (0)     1488 2023-05-30 08:51:02.000000 openirt-0.1.4/openirt/item_model.py
--rw-rw-rw-   0 root         (0) root         (0)     3387 2023-05-30 08:51:02.000000 openirt-0.1.4/openirt/norm_model.py
--rw-rw-rw-   0 root         (0) root         (0)     2750 2023-05-30 08:51:02.000000 openirt-0.1.4/openirt/pl1.py
--rw-rw-rw-   0 root         (0) root         (0)     4524 2023-05-30 08:51:02.000000 openirt-0.1.4/openirt/pl2.py
--rw-rw-rw-   0 root         (0) root         (0)     5893 2023-05-30 08:51:02.000000 openirt-0.1.4/openirt/pl3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:51:20.502569 openirt-0.1.4/openirt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      256 2023-05-30 08:51:20.000000 openirt-0.1.4/openirt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      337 2023-05-30 08:51:20.000000 openirt-0.1.4/openirt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 08:51:20.000000 openirt-0.1.4/openirt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-05-30 08:51:20.000000 openirt-0.1.4/openirt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 08:51:20.502569 openirt-0.1.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      555 2023-05-30 08:51:02.000000 openirt-0.1.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:51:20.502569 openirt-0.1.4/tests/
--rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-30 08:51:02.000000 openirt-0.1.4/tests/test_func.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:57:23.740669 openirt-0.1.5/
+-rw-rw-rw-   0 root         (0) root         (0)     1069 2023-05-30 08:57:05.000000 openirt-0.1.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      256 2023-05-30 08:57:23.740669 openirt-0.1.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       30 2023-05-30 08:57:05.000000 openirt-0.1.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:57:23.738669 openirt-0.1.5/openirt/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-30 08:57:05.000000 openirt-0.1.5/openirt/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6938 2023-05-30 08:57:05.000000 openirt-0.1.5/openirt/bayes3PL.py
+-rw-rw-rw-   0 root         (0) root         (0)     2081 2023-05-30 08:57:05.000000 openirt-0.1.5/openirt/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     3932 2023-05-30 08:57:05.000000 openirt-0.1.5/openirt/irt_instance.py
+-rw-rw-rw-   0 root         (0) root         (0)     1488 2023-05-30 08:57:05.000000 openirt-0.1.5/openirt/item_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3387 2023-05-30 08:57:05.000000 openirt-0.1.5/openirt/norm_model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2742 2023-05-30 08:57:05.000000 openirt-0.1.5/openirt/pl1.py
+-rw-rw-rw-   0 root         (0) root         (0)     4524 2023-05-30 08:57:05.000000 openirt-0.1.5/openirt/pl2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5893 2023-05-30 08:57:05.000000 openirt-0.1.5/openirt/pl3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:57:23.739669 openirt-0.1.5/openirt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      256 2023-05-30 08:57:23.000000 openirt-0.1.5/openirt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      337 2023-05-30 08:57:23.000000 openirt-0.1.5/openirt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 08:57:23.000000 openirt-0.1.5/openirt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-05-30 08:57:23.000000 openirt-0.1.5/openirt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-30 08:57:23.740669 openirt-0.1.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      555 2023-05-30 08:57:05.000000 openirt-0.1.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 08:57:23.739669 openirt-0.1.5/tests/
+-rw-rw-rw-   0 root         (0) root         (0)       32 2023-05-30 08:57:05.000000 openirt-0.1.5/tests/test_func.py
```

### Comparing `openirt-0.1.4/LICENSE` & `openirt-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `openirt-0.1.4/openirt/bayes3PL.py` & `openirt-0.1.5/openirt/bayes3PL.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.4/openirt/cli.py` & `openirt-0.1.5/openirt/cli.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.4/openirt/irt_instance.py` & `openirt-0.1.5/openirt/irt_instance.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.4/openirt/item_model.py` & `openirt-0.1.5/openirt/item_model.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.4/openirt/norm_model.py` & `openirt-0.1.5/openirt/norm_model.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.4/openirt/pl1.py` & `openirt-0.1.5/openirt/pl1.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 import sys
 # sys.path.append('../openirt')
-sys.path.append(str(Path(__file__).parent.parent.parent))
-# print(sys.path)
-from item_model import ItemModel
+sys.path.append(str(Path(__file__).parent))
+print(sys.path)
+from openirt.item_model import ItemModel
 from typing import Union
 import numpy as np
 from pl2 import PL2
 
 class PL1(ItemModel):
     def prob(self, ability: Union[list, np.ndarray, float], params: Union[list, np.ndarray]) -> np.ndarray:
         """
```

### Comparing `openirt-0.1.4/openirt/pl2.py` & `openirt-0.1.5/openirt/pl2.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.4/openirt/pl3.py` & `openirt-0.1.5/openirt/pl3.py`

 * *Files identical despite different names*

### Comparing `openirt-0.1.4/setup.py` & `openirt-0.1.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,13 +10,13 @@
 
 setup(
     name='openirt',
     packages = find_packages(include=['openirt']),
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
     url='https://gitlab.com/pleased/...',
-    version='0.1.4',
+    version='0.1.5',
     description='Item response theory toolkit',
     author='Johan Hay',
     license='MIT',
 )
```

