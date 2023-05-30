# Comparing `tmp/weighted_tqdm-0.7.tar.gz` & `tmp/weighted_tqdm-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weighted_tqdm-0.7.tar", last modified: Mon May 22 14:15:13 2023, max compression
+gzip compressed data, was "weighted_tqdm-0.8.tar", last modified: Tue May 30 15:46:16 2023, max compression
```

## Comparing `weighted_tqdm-0.7.tar` & `weighted_tqdm-0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-22 14:15:13.466488 weighted_tqdm-0.7/
--rw-rw-rw-   0        0        0     1096 2023-05-22 14:14:29.000000 weighted_tqdm-0.7/LICENSE
--rw-rw-rw-   0        0        0     2967 2023-05-22 14:15:13.467996 weighted_tqdm-0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2446 2023-05-22 14:14:29.000000 weighted_tqdm-0.7/README.md
--rw-rw-rw-   0        0        0      516 2023-05-22 14:15:13.470555 weighted_tqdm-0.7/setup.cfg
--rw-rw-rw-   0        0        0      866 2023-05-22 14:14:29.000000 weighted_tqdm-0.7/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:15:13.426646 weighted_tqdm-0.7/src/
-drwxrwxrwx   0        0        0        0 2023-05-22 14:15:13.437609 weighted_tqdm-0.7/src/weighted_tqdm/
--rw-rw-rw-   0        0        0       68 2023-04-26 13:34:55.000000 weighted_tqdm-0.7/src/weighted_tqdm/__init__.py
--rw-rw-rw-   0        0        0    16117 2023-05-22 12:47:17.000000 weighted_tqdm-0.7/src/weighted_tqdm/weighted_tqdm.py
-drwxrwxrwx   0        0        0        0 2023-05-22 14:15:13.465489 weighted_tqdm-0.7/src/weighted_tqdm.egg-info/
--rw-rw-rw-   0        0        0     2967 2023-05-22 14:15:13.000000 weighted_tqdm-0.7/src/weighted_tqdm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      305 2023-05-22 14:15:13.000000 weighted_tqdm-0.7/src/weighted_tqdm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-22 14:15:13.000000 weighted_tqdm-0.7/src/weighted_tqdm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-22 14:15:13.000000 weighted_tqdm-0.7/src/weighted_tqdm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-22 14:15:13.000000 weighted_tqdm-0.7/src/weighted_tqdm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-30 15:46:16.890186 weighted_tqdm-0.8/
+-rw-rw-rw-   0        0        0     1096 2023-05-30 15:42:25.000000 weighted_tqdm-0.8/LICENSE
+-rw-rw-rw-   0        0        0     3110 2023-05-30 15:46:16.891187 weighted_tqdm-0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2589 2023-05-30 15:45:46.000000 weighted_tqdm-0.8/README.md
+-rw-rw-rw-   0        0        0      516 2023-05-30 15:46:16.894183 weighted_tqdm-0.8/setup.cfg
+-rw-rw-rw-   0        0        0      867 2023-05-30 15:42:25.000000 weighted_tqdm-0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:46:16.851792 weighted_tqdm-0.8/src/
+drwxrwxrwx   0        0        0        0 2023-05-30 15:46:16.862962 weighted_tqdm-0.8/src/weighted_tqdm/
+-rw-rw-rw-   0        0        0       68 2023-04-26 13:34:55.000000 weighted_tqdm-0.8/src/weighted_tqdm/__init__.py
+-rw-rw-rw-   0        0        0    18996 2023-05-30 15:29:27.000000 weighted_tqdm-0.8/src/weighted_tqdm/weighted_tqdm.py
+drwxrwxrwx   0        0        0        0 2023-05-30 15:46:16.888021 weighted_tqdm-0.8/src/weighted_tqdm.egg-info/
+-rw-rw-rw-   0        0        0     3110 2023-05-30 15:46:16.000000 weighted_tqdm-0.8/src/weighted_tqdm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      305 2023-05-30 15:46:16.000000 weighted_tqdm-0.8/src/weighted_tqdm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 15:46:16.000000 weighted_tqdm-0.8/src/weighted_tqdm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-30 15:46:16.000000 weighted_tqdm-0.8/src/weighted_tqdm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-30 15:46:16.000000 weighted_tqdm-0.8/src/weighted_tqdm.egg-info/top_level.txt
```

### Comparing `weighted_tqdm-0.7/LICENSE` & `weighted_tqdm-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `weighted_tqdm-0.7/PKG-INFO` & `weighted_tqdm-0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: weighted_tqdm
-Version: 0.7
+Version: 0.8
 Summary: weighted_tqdm allows for weighted iterations in tqdm progress bars.
-Home-page: https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.7.tar.gz
+Home-page: https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.8.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -24,14 +24,15 @@
 **weighted_tqdm** works equivalently to tqdm, accepting all the same arguments, but also accepts a `weights` argument. This argument specifies the weights of each item in the iterable and can be given as a function of the iterable or be any iterable (list, array, tuple...). The progress bar will then take into account the weights of each item in it's prediciton of the time, and it's progress bar will be weighted accordingly. To the left of the progress bar an iteration counter is shown.
 ```
 how_many_qubits = [1,2,3,4,5]
 qubits weights = lambda x: (2**x)**3
 for i in weighted_tqdm(how_many_qubits, weights=weights):
     # do something
 ```
+New: Now supports `p_tqdm` with an additionally passed function handle for parallel execution. This functionality extends to the generators. 
 
 **qudit_tqdm** is a special variant of tqdm, that predicts the remaining time for calculations in quantum mechanics, with the added arguments `dit` specifying whether its a calculation of qubits (default `dit=2` or `dit=3` for qutrits), and the argument `exp` specifying the scaling of computational time with the dimension of a hilbert space. 
 ```
 for i in qudit_tqdm(how_many_qubits, dim=2, exp=3):
     time.sleep((2**i)**3)
 ```
```

### Comparing `weighted_tqdm-0.7/README.md` & `weighted_tqdm-0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 **weighted_tqdm** works equivalently to tqdm, accepting all the same arguments, but also accepts a `weights` argument. This argument specifies the weights of each item in the iterable and can be given as a function of the iterable or be any iterable (list, array, tuple...). The progress bar will then take into account the weights of each item in it's prediciton of the time, and it's progress bar will be weighted accordingly. To the left of the progress bar an iteration counter is shown.
 ```
 how_many_qubits = [1,2,3,4,5]
 qubits weights = lambda x: (2**x)**3
 for i in weighted_tqdm(how_many_qubits, weights=weights):
     # do something
 ```
+New: Now supports `p_tqdm` with an additionally passed function handle for parallel execution. This functionality extends to the generators. 
 
 **qudit_tqdm** is a special variant of tqdm, that predicts the remaining time for calculations in quantum mechanics, with the added arguments `dit` specifying whether its a calculation of qubits (default `dit=2` or `dit=3` for qutrits), and the argument `exp` specifying the scaling of computational time with the dimension of a hilbert space. 
 ```
 for i in qudit_tqdm(how_many_qubits, dim=2, exp=3):
     time.sleep((2**i)**3)
 ```
```

### Comparing `weighted_tqdm-0.7/setup.cfg` & `weighted_tqdm-0.8/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206b 726f 6e62 696e 6174 696f 6e73   = kronbinations
-00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 370d  ..version = 0.7.
+00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 380d  ..version = 0.8.
 00000030: 0a61 7574 686f 7220 3d20 4d69 6368 6165  .author = Michae
 00000040: 6c20 5363 6869 6c6c 696e 670d 0a61 7574  l Schilling..aut
 00000050: 686f 725f 656d 6169 6c20 3d20 6d69 6368  hor_email = mich
 00000060: 6165 6c40 6e74 726f 7069 632e 6465 0d0a  ael@ntropic.de..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 7765  description = we
 00000080: 6967 6874 6564 5f74 7164 6d20 616c 6c6f  ighted_tqdm allo
 00000090: 7773 2066 6f72 2077 6569 6768 7465 6420  ws for weighted 
@@ -15,15 +15,15 @@
 000000e0: 4d45 2e6d 640d 0a6c 6f6e 675f 6465 7363  ME.md..long_desc
 000000f0: 7269 7074 696f 6e5f 636f 6e74 656e 745f  ription_content_
 00000100: 7479 7065 203d 2074 6578 742f 6d61 726b  type = text/mark
 00000110: 646f 776e 0d0a 7572 6c20 3d20 6874 7470  down..url = http
 00000120: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4e  s://github.com/N
 00000130: 7472 6f70 6963 2f77 6569 6768 7465 645f  tropic/weighted_
 00000140: 7471 646d 2f61 7263 6869 7665 2f72 6566  tqdm/archive/ref
-00000150: 732f 7461 6773 2f76 302e 372e 7461 722e  s/tags/v0.7.tar.
+00000150: 732f 7461 6773 2f76 302e 382e 7461 722e  s/tags/v0.8.tar.
 00000160: 677a 0d0a 5072 6f67 7261 6d6d 696e 6720  gz..Programming 
 00000170: 4c61 6e67 7561 6765 203d 203a 2050 7974  Language = : Pyt
 00000180: 686f 6e20 3a3a 2033 0d0a 094c 6963 656e  hon :: 3...Licen
 00000190: 7365 203a 3a20 4f53 4920 4170 7072 6f76  se :: OSI Approv
 000001a0: 6564 203a 3a20 4d49 5420 4c69 6365 6e73  ed :: MIT Licens
 000001b0: 650d 0a09 4f70 6572 6174 696e 6720 5379  e...Operating Sy
 000001c0: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
```

### Comparing `weighted_tqdm-0.7/setup.py` & `weighted_tqdm-0.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "weighted_tqdm",
-    version       = "0.7",
+    version        = "0.8",
     author = "Michael Schilling",
     author_email = "michael@ntropic.de",
     description  = "weighted_tqdm allows for weighted iterations in tqdm progress bars.",
     long_description = long_description,
     long_description_content_type = "text/markdown",
-    url = "https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.7.tar.gz",
+    url = "https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.8.tar.gz",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
     packages=setuptools.find_packages(where="src"),
```

### Comparing `weighted_tqdm-0.7/src/weighted_tqdm/weighted_tqdm.py` & `weighted_tqdm-0.8/src/weighted_tqdm/weighted_tqdm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 # A function that modifies tqdm progress bars to estimate the remaining time, by allowing the user to specify how much time a step takes with respect to the others
 # adds input weights=[1,2,4,8,16] for a progress bar that takes into account that iteration 2 takes twice as long as iteration 1, and iteration 3 takes 4 times as long as iteration 1, etc.
 import time
 from tqdm import tqdm
 import itertools
 import numpy as np
+from pathos.helpers import cpu_count
+from pathos.multiprocessing import ProcessingPool as Pool
 
 def determine_length_of_iterable(iterable, weights, **kwargs):
     # calulcate the total number of iterations
     if hasattr(iterable, '__len__'):
         total = len(iterable)
     elif 'total' in kwargs:
         total = kwargs['total']
@@ -68,21 +70,49 @@
     #pbar.set_description('(Done)')
     pbar.update(weights_var[-1])
     pbar.close()
 
 def qudit_tqdm(iterable, dit=2, exp=3, name='qubits', print_val=False, bar_format='{l_bar}{bar}| {elapsed}<{remaining}', **kwargs):
     #  calculates the increase in compute for qudit calculations (by default for qubits and considereng O(n**3) operations)
     return weighted_tqdm(iterable, weights=lambda i: (dit**i)**exp, name=name, print_val=print_val, bar_format=bar_format, **kwargs)
-        
+
+def _parallel(function, *iterables, **kwargs):
+    # Modified version of p_tqdm works with weighted_tqdm generators
+    # Extract num_cpus
+    num_cpus = kwargs.pop('num_cpus', None)
+
+    # Determine num_cpus
+    if num_cpus is None:
+        num_cpus = cpu_count()
+    elif type(num_cpus) == float:
+        num_cpus = int(round(num_cpus * cpu_count()))
+
+    # Determine length of tqdm (equal to length of shortest iterable or total kwarg), if possible
+    total = kwargs.pop('total', None)
+    lengths = [len(iterable) for iterable in iterables if hasattr(iterable, '__len__')]
+    length = total or (min(lengths) if lengths else None)
+
+    # Create parallel generator
+    pool = Pool(num_cpus)
+    for item in weighted_tqdm(pool.imap(function, *iterables), **kwargs, weights= np.ones(length)/length):
+        yield item
+    pool.clear()
+
+
+def weighted_p_tqdm(function, *iterables, **kwargs):
+    """Performs a parallel ordered map with a progress bar."""
+    generator = _parallel( function, *iterables, **kwargs)
+    result = list(generator)
+    return result        
 # A variant of tqdm, that creates a progress bar generator (via class called progress), 
 # which is then used to create progress bars, which can be split between different loops
 ## for example:
 # p = progress()# for i in p.tqdm(range(10)):
-#    for j in p.tqdm(range(10)):
-#       pass
+# for j in p.tqdm(range(10)):
+#     pass
 ## this will create a progress bar where every iteration of j is counted as 1/10th of an iteration of i
 class progress:
     def __init__(self, total=1000, print_val=False, bar_format='{l_bar}{bar}| {elapsed}<{remaining}', max_rate=30, **kwargs):
         self.total = total # separate these steps dynamically
         self.levels = 0
         self.weight_by_level = []
         self.ind_by_level = []
@@ -91,14 +121,35 @@
         self.pbar = None
         self.print_val = print_val
         self.bar_format = bar_format
         self.names = []
         self.min_time = 1/max_rate
         self.time = time.time()
         
+    def _parallel(self, function, *iterables, num_cpus=None, **kwargs):
+        # Modified version of p_tqdm works with weighted_tqdm generators
+
+        # Determine num_cpus
+        if num_cpus is None:
+            num_cpus = cpu_count()
+        elif type(num_cpus) == float:
+            num_cpus = int(round(num_cpus * cpu_count()))
+
+        # Create parallel generator
+        pool = Pool(num_cpus)
+        for item in self.tqdm(pool.imap(function, *iterables), **kwargs):
+            yield item
+        pool.clear()
+        
+    def p_tqdm(self, function, *iterables, num_cpus=None, **kwargs):
+        """Performs a parallel ordered map with a progress bar."""
+        generator = self._parallel(function, *iterables, num_cpus=num_cpus, **kwargs)
+        result = list(generator)
+        return result
+        
     def weighted_tqdm(self, iterable, weights=None, name='', **kwargs):
         how_many = determine_length_of_iterable(iterable, weights, **kwargs)
         # add to total levels of the progress bar
         # add the weight of the new level to the weight_by_level list
         if len(name):
             name += ': '
         self.names.append(name)
@@ -172,15 +223,15 @@
             self.pbar.update(diff_count)
         # finished iterating through the iterable
         if my_level == 1:  # reset the object
             if self.print_val:
                 self.pbar.set_description(self.names[-1]+str(elem)+' (' +str(ind+1) + '/' + str(how_many) + ')')
             else:
                 self.pbar.set_description(self.names[-1]+'(' +str(ind+1) + '/' + str(how_many) + ')')
-            self.time = new_time
+            self.time = time.time()
             self.pbar.close()
             self.pbar = None
             self.current_count = 0
             self.current_count_float = 0.0
             self.weight_by_level = []
             self.names = []
             self.levels = 0   
@@ -244,14 +295,36 @@
         self.indexes = indexes
         self.len_indexes = len(indexes)
         self.curr_ind = 0 # tracks the current indexes index in indexes
         self.cumm_weight = 0.0
         self.curr_pbar_index = 0
         self.pbar = tqdm(total=self.total, bar_format=self.bar_format)
         
+                
+    def _parallel(self, function, *iterables, num_cpus=None, **kwargs):
+        # Modified version of p_tqdm works with weighted_tqdm generators
+
+        # Determine num_cpus
+        if num_cpus is None:
+            num_cpus = cpu_count()
+        elif type(num_cpus) == float:
+            num_cpus = int(round(num_cpus * cpu_count()))
+
+        # Create parallel generator
+        pool = Pool(num_cpus)
+        for item in self.sub_tqdm(pool.imap(function, *iterables), **kwargs):
+            yield item
+        pool.clear()
+        
+    def p_tqdm(self, function, *iterables, num_cpus=None, **kwargs):
+        """Performs a parallel ordered map with a progress bar."""
+        generator = self._parallel(function, *iterables, num_cpus=num_cpus, **kwargs)
+        result = list(generator)
+        return result
+        
     def sub_tqdm(self, iterable, weights=None, name='', **kwargs):
         how_many = determine_length_of_iterable(iterable, weights, **kwargs)
         self.levels += 1
         my_level = self.levels
         if len(name):
             name += ': '
         self.names.append(name)
```

### Comparing `weighted_tqdm-0.7/src/weighted_tqdm.egg-info/PKG-INFO` & `weighted_tqdm-0.8/src/weighted_tqdm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: weighted-tqdm
-Version: 0.7
+Version: 0.8
 Summary: weighted_tqdm allows for weighted iterations in tqdm progress bars.
-Home-page: https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.7.tar.gz
+Home-page: https://github.com/Ntropic/weighted_tqdm/archive/refs/tags/v0.8.tar.gz
 Author: Michael Schilling
 Author-email: michael@ntropic.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -24,14 +24,15 @@
 **weighted_tqdm** works equivalently to tqdm, accepting all the same arguments, but also accepts a `weights` argument. This argument specifies the weights of each item in the iterable and can be given as a function of the iterable or be any iterable (list, array, tuple...). The progress bar will then take into account the weights of each item in it's prediciton of the time, and it's progress bar will be weighted accordingly. To the left of the progress bar an iteration counter is shown.
 ```
 how_many_qubits = [1,2,3,4,5]
 qubits weights = lambda x: (2**x)**3
 for i in weighted_tqdm(how_many_qubits, weights=weights):
     # do something
 ```
+New: Now supports `p_tqdm` with an additionally passed function handle for parallel execution. This functionality extends to the generators. 
 
 **qudit_tqdm** is a special variant of tqdm, that predicts the remaining time for calculations in quantum mechanics, with the added arguments `dit` specifying whether its a calculation of qubits (default `dit=2` or `dit=3` for qutrits), and the argument `exp` specifying the scaling of computational time with the dimension of a hilbert space. 
 ```
 for i in qudit_tqdm(how_many_qubits, dim=2, exp=3):
     time.sleep((2**i)**3)
 ```
```

