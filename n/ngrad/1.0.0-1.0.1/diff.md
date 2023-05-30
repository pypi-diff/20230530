# Comparing `tmp/ngrad-1.0.0.tar.gz` & `tmp/ngrad-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngrad-1.0.0.tar", last modified: Mon May 29 09:34:23 2023, max compression
+gzip compressed data, was "ngrad-1.0.1.tar", last modified: Tue May 30 18:37:22 2023, max compression
```

## Comparing `ngrad-1.0.0.tar` & `ngrad-1.0.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-05-29 09:34:23.850636 ngrad-1.0.0/
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     3757 2023-05-29 09:34:23.850636 ngrad-1.0.0/PKG-INFO
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     3278 2023-05-29 09:31:19.000000 ngrad-1.0.0/README.md
-drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-05-29 09:34:23.846636 ngrad-1.0.0/ngrad/
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        0 2023-05-29 09:04:57.000000 ngrad-1.0.0/ngrad/__init__.py
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     5211 2023-05-28 18:23:58.000000 ngrad-1.0.0/ngrad/engine.py
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     1896 2023-05-29 09:29:42.000000 ngrad-1.0.0/ngrad/library.py
-drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-05-29 09:34:23.850636 ngrad-1.0.0/ngrad.egg-info/
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     3757 2023-05-29 09:34:23.000000 ngrad-1.0.0/ngrad.egg-info/PKG-INFO
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)      213 2023-05-29 09:34:23.000000 ngrad-1.0.0/ngrad.egg-info/SOURCES.txt
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        1 2023-05-29 09:34:23.000000 ngrad-1.0.0/ngrad.egg-info/dependency_links.txt
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        6 2023-05-29 09:34:23.000000 ngrad-1.0.0/ngrad.egg-info/requires.txt
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        6 2023-05-29 09:34:23.000000 ngrad-1.0.0/ngrad.egg-info/top_level.txt
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)       38 2023-05-29 09:34:23.850636 ngrad-1.0.0/setup.cfg
--rw-rw-r--   0 x0axz     (1000) x0axz     (1000)      727 2023-05-29 09:27:49.000000 ngrad-1.0.0/setup.py
+drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-05-30 18:37:22.201923 ngrad-1.0.1/
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     1061 2023-05-30 18:26:38.000000 ngrad-1.0.1/LICENSE
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     3933 2023-05-30 18:37:22.201923 ngrad-1.0.1/PKG-INFO
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     3432 2023-05-30 18:26:38.000000 ngrad-1.0.1/README.md
+drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-05-30 18:37:22.201923 ngrad-1.0.1/ngrad/
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        0 2023-05-29 09:04:57.000000 ngrad-1.0.1/ngrad/__init__.py
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     5211 2023-05-28 18:23:58.000000 ngrad-1.0.1/ngrad/engine.py
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     1896 2023-05-29 09:29:42.000000 ngrad-1.0.1/ngrad/library.py
+drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-05-30 18:37:22.201923 ngrad-1.0.1/ngrad.egg-info/
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     3933 2023-05-30 18:37:22.000000 ngrad-1.0.1/ngrad.egg-info/PKG-INFO
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)      241 2023-05-30 18:37:22.000000 ngrad-1.0.1/ngrad.egg-info/SOURCES.txt
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        1 2023-05-30 18:37:22.000000 ngrad-1.0.1/ngrad.egg-info/dependency_links.txt
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        6 2023-05-30 18:37:22.000000 ngrad-1.0.1/ngrad.egg-info/requires.txt
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)        6 2023-05-30 18:37:22.000000 ngrad-1.0.1/ngrad.egg-info/top_level.txt
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)       38 2023-05-30 18:37:22.201923 ngrad-1.0.1/setup.cfg
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)      727 2023-05-30 18:35:42.000000 ngrad-1.0.1/setup.py
+drwxrwxr-x   0 x0axz     (1000) x0axz     (1000)        0 2023-05-30 18:37:22.201923 ngrad-1.0.1/test/
+-rw-rw-r--   0 x0axz     (1000) x0axz     (1000)     5098 2023-05-30 18:04:58.000000 ngrad-1.0.1/test/test_engine.py
```

### Comparing `ngrad-1.0.0/PKG-INFO` & `ngrad-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ngrad
-Version: 1.0.0
+Version: 1.0.1
 Summary: An Autograd engine and a neural network library that handle an N-dimensional array.
 Home-page: https://github.com/x0axz/ngrad
 Author: Nooh
 Author-email: x0axz@protonmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Autograd Engine
 
 The repository includes an Autograd engine and a neural network library that handle an N-dimensional array.
 
 Autograd is a tool used for derivative calculation. It tracks operations on values with enabled gradients and builds a dynamic computational graph — a graph without cycles. Input values serve as the leaves of the graph, while output values act as its roots. Gradients are computed by traversing the graph from root to leaf, applying the chain rule to multiply gradients at each step.
 
@@ -25,31 +26,47 @@
 
 [Building an Autograd Engine: An Illustrative and Interactive Guide](https://x0axz.com/blog/autograd.html)
 
 The article provides a comprehensive guide to building an autograd engine and a neural network library that handle an N-dimensional array. It assumes a basic understanding of Python programming, high school calculus, and neural networks but offers various teaching methods for beginners. It includes line-by-line code explanations, output visualizations, and an interactive area to explore derivatives. The guide covers the foundational concepts of neural networks, starting with derivatives and progressing to backpropagation. It explains how to perform backpropagation manually and programmatically, including implementation techniques. The article also demonstrates the building of an autograd class from scratch and its application to training a neural network on a dataset. It concludes by guiding readers through the development of a simple neural network library using the autograd class.
 
 ## Installation
 
+```
+pip install ngrad
+```
+
+## Development
+
 The only library required for this to work is Numpy, which is used to handle N-dimensional array.
 
 ```
 pip install -r requirements.txt
 ```
 
 ## Test
 
-To verify the accuracy of the [engine.py](https://github.com/x0axz/ngrad/blob/main/ngrad/engine.py) code and ensure that it produces the same output for the N-dimensional array, scalar value, and PyTorch APIs, execute the following command:
+To verify the accuracy of the [engine.py](https://github.com/x0axz/ngrad/blob/main/ngrad/engine.py) code and ensure that it produces the same output for the N-dimensional array, scalar value, and PyTorch APIs, execute the following command (make sure that PyTorch is installed):
 
 ```
 cd test/
-python engine_test.py
+pip install -r requirements.txt
+```
+
+Run the test:
+
+```
+python test_engine.py
 ```
 
 ## Train
 
 This [notebook](https://github.com/x0axz/ngrad/blob/main/notebook/Training_Neural_Network.ipynb) comprises the code required for training the neural network, encompassing the code for [engine.py](https://github.com/x0axz/ngrad/blob/main/ngrad/engine.py) and [library.py](https://github.com/x0axz/ngrad/blob/main/ngrad/library.py). Within this notebook, we first set the input values, construct an MLP with a predetermined architecture, and subsequently execute forward propagation to compute and acquire the output. Subsequently, we initiate the training procedure of the neural network by generating a small dataset, followed by training the MLP model to minimize loss and enhance its prediction abilities. Finally, we present a list of the predicted outputs.
 
 ## Notebook
 
 This [notebook](https://github.com/x0axz/ngrad/blob/main/notebook/Autograd_Engine_&_NN_Library.ipynb) contains a comprehensive collection of examples and code for building, testing, and training the autograd engine and neural network library. Play with it to experiment and explore its functionalities.
 
+## License
+
+MIT
+
```

### Comparing `ngrad-1.0.0/README.md` & `ngrad-1.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -10,29 +10,45 @@
 
 [Building an Autograd Engine: An Illustrative and Interactive Guide](https://x0axz.com/blog/autograd.html)
 
 The article provides a comprehensive guide to building an autograd engine and a neural network library that handle an N-dimensional array. It assumes a basic understanding of Python programming, high school calculus, and neural networks but offers various teaching methods for beginners. It includes line-by-line code explanations, output visualizations, and an interactive area to explore derivatives. The guide covers the foundational concepts of neural networks, starting with derivatives and progressing to backpropagation. It explains how to perform backpropagation manually and programmatically, including implementation techniques. The article also demonstrates the building of an autograd class from scratch and its application to training a neural network on a dataset. It concludes by guiding readers through the development of a simple neural network library using the autograd class.
 
 ## Installation
 
+```
+pip install ngrad
+```
+
+## Development
+
 The only library required for this to work is Numpy, which is used to handle N-dimensional array.
 
 ```
 pip install -r requirements.txt
 ```
 
 ## Test
 
-To verify the accuracy of the [engine.py](https://github.com/x0axz/ngrad/blob/main/ngrad/engine.py) code and ensure that it produces the same output for the N-dimensional array, scalar value, and PyTorch APIs, execute the following command:
+To verify the accuracy of the [engine.py](https://github.com/x0axz/ngrad/blob/main/ngrad/engine.py) code and ensure that it produces the same output for the N-dimensional array, scalar value, and PyTorch APIs, execute the following command (make sure that PyTorch is installed):
 
 ```
 cd test/
-python engine_test.py
+pip install -r requirements.txt
+```
+
+Run the test:
+
+```
+python test_engine.py
 ```
 
 ## Train
 
 This [notebook](https://github.com/x0axz/ngrad/blob/main/notebook/Training_Neural_Network.ipynb) comprises the code required for training the neural network, encompassing the code for [engine.py](https://github.com/x0axz/ngrad/blob/main/ngrad/engine.py) and [library.py](https://github.com/x0axz/ngrad/blob/main/ngrad/library.py). Within this notebook, we first set the input values, construct an MLP with a predetermined architecture, and subsequently execute forward propagation to compute and acquire the output. Subsequently, we initiate the training procedure of the neural network by generating a small dataset, followed by training the MLP model to minimize loss and enhance its prediction abilities. Finally, we present a list of the predicted outputs.
 
 ## Notebook
 
 This [notebook](https://github.com/x0axz/ngrad/blob/main/notebook/Autograd_Engine_&_NN_Library.ipynb) contains a comprehensive collection of examples and code for building, testing, and training the autograd engine and neural network library. Play with it to experiment and explore its functionalities.
+
+## License
+
+MIT
```

### Comparing `ngrad-1.0.0/ngrad/engine.py` & `ngrad-1.0.1/ngrad/engine.py`

 * *Files identical despite different names*

### Comparing `ngrad-1.0.0/ngrad/library.py` & `ngrad-1.0.1/ngrad/library.py`

 * *Files identical despite different names*

### Comparing `ngrad-1.0.0/ngrad.egg-info/PKG-INFO` & `ngrad-1.0.1/ngrad.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ngrad
-Version: 1.0.0
+Version: 1.0.1
 Summary: An Autograd engine and a neural network library that handle an N-dimensional array.
 Home-page: https://github.com/x0axz/ngrad
 Author: Nooh
 Author-email: x0axz@protonmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Autograd Engine
 
 The repository includes an Autograd engine and a neural network library that handle an N-dimensional array.
 
 Autograd is a tool used for derivative calculation. It tracks operations on values with enabled gradients and builds a dynamic computational graph — a graph without cycles. Input values serve as the leaves of the graph, while output values act as its roots. Gradients are computed by traversing the graph from root to leaf, applying the chain rule to multiply gradients at each step.
 
@@ -25,31 +26,47 @@
 
 [Building an Autograd Engine: An Illustrative and Interactive Guide](https://x0axz.com/blog/autograd.html)
 
 The article provides a comprehensive guide to building an autograd engine and a neural network library that handle an N-dimensional array. It assumes a basic understanding of Python programming, high school calculus, and neural networks but offers various teaching methods for beginners. It includes line-by-line code explanations, output visualizations, and an interactive area to explore derivatives. The guide covers the foundational concepts of neural networks, starting with derivatives and progressing to backpropagation. It explains how to perform backpropagation manually and programmatically, including implementation techniques. The article also demonstrates the building of an autograd class from scratch and its application to training a neural network on a dataset. It concludes by guiding readers through the development of a simple neural network library using the autograd class.
 
 ## Installation
 
+```
+pip install ngrad
+```
+
+## Development
+
 The only library required for this to work is Numpy, which is used to handle N-dimensional array.
 
 ```
 pip install -r requirements.txt
 ```
 
 ## Test
 
-To verify the accuracy of the [engine.py](https://github.com/x0axz/ngrad/blob/main/ngrad/engine.py) code and ensure that it produces the same output for the N-dimensional array, scalar value, and PyTorch APIs, execute the following command:
+To verify the accuracy of the [engine.py](https://github.com/x0axz/ngrad/blob/main/ngrad/engine.py) code and ensure that it produces the same output for the N-dimensional array, scalar value, and PyTorch APIs, execute the following command (make sure that PyTorch is installed):
 
 ```
 cd test/
-python engine_test.py
+pip install -r requirements.txt
+```
+
+Run the test:
+
+```
+python test_engine.py
 ```
 
 ## Train
 
 This [notebook](https://github.com/x0axz/ngrad/blob/main/notebook/Training_Neural_Network.ipynb) comprises the code required for training the neural network, encompassing the code for [engine.py](https://github.com/x0axz/ngrad/blob/main/ngrad/engine.py) and [library.py](https://github.com/x0axz/ngrad/blob/main/ngrad/library.py). Within this notebook, we first set the input values, construct an MLP with a predetermined architecture, and subsequently execute forward propagation to compute and acquire the output. Subsequently, we initiate the training procedure of the neural network by generating a small dataset, followed by training the MLP model to minimize loss and enhance its prediction abilities. Finally, we present a list of the predicted outputs.
 
 ## Notebook
 
 This [notebook](https://github.com/x0axz/ngrad/blob/main/notebook/Autograd_Engine_&_NN_Library.ipynb) contains a comprehensive collection of examples and code for building, testing, and training the autograd engine and neural network library. Play with it to experiment and explore its functionalities.
 
+## License
+
+MIT
+
```

### Comparing `ngrad-1.0.0/setup.py` & `ngrad-1.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ngrad",
-    version="1.0.0",
+    version="1.0.1",
     description="An Autograd engine and a neural network library that handle an N-dimensional array.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Nooh",
     author_email="x0axz@protonmail.com",
     url="https://github.com/x0axz/ngrad",
     packages=setuptools.find_packages(),
```

