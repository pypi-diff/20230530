# Comparing `tmp/PyGRO-0.1.0.tar.gz` & `tmp/PyGRO-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyGRO-0.1.0.tar", last modified: Tue Apr 18 07:07:26 2023, max compression
+gzip compressed data, was "PyGRO-0.1.1.tar", last modified: Tue May 30 08:31:52 2023, max compression
```

## Comparing `PyGRO-0.1.0.tar` & `PyGRO-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 riccardodellamonica   (501) staff       (20)        0 2023-04-18 07:07:26.212633 PyGRO-0.1.0/
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)     1065 2021-01-29 22:40:37.000000 PyGRO-0.1.0/LICENSE.txt
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)     1466 2023-04-18 07:07:26.212458 PyGRO-0.1.0/PKG-INFO
-drwxr-xr-x   0 riccardodellamonica   (501) staff       (20)        0 2023-04-18 07:07:26.206441 PyGRO-0.1.0/PyGRO.egg-info/
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)     1466 2023-04-18 07:07:26.000000 PyGRO-0.1.0/PyGRO.egg-info/PKG-INFO
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)      452 2023-04-18 07:07:26.000000 PyGRO-0.1.0/PyGRO.egg-info/SOURCES.txt
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)        1 2023-04-18 07:07:26.000000 PyGRO-0.1.0/PyGRO.egg-info/dependency_links.txt
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)       25 2023-04-18 07:07:26.000000 PyGRO-0.1.0/PyGRO.egg-info/requires.txt
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)        6 2023-04-18 07:07:26.000000 PyGRO-0.1.0/PyGRO.egg-info/top_level.txt
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)      925 2022-02-10 10:18:41.000000 PyGRO-0.1.0/README.md
-drwxr-xr-x   0 riccardodellamonica   (501) staff       (20)        0 2023-04-18 07:07:26.209246 PyGRO-0.1.0/pygro/
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)      195 2022-03-11 17:21:23.000000 PyGRO-0.1.0/pygro/__init__.py
-drwxr-xr-x   0 riccardodellamonica   (501) staff       (20)        0 2023-04-18 07:07:26.212059 PyGRO-0.1.0/pygro/default_metrics/
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)    11199 2021-04-04 11:28:03.000000 PyGRO-0.1.0/pygro/default_metrics/KerrBL.py
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)    49866 2021-05-08 10:28:38.000000 PyGRO-0.1.0/pygro/default_metrics/KerrSTVG.py
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)     2657 2021-04-04 11:28:07.000000 PyGRO-0.1.0/pygro/default_metrics/Yukawa.py
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)      130 2021-05-08 10:28:55.000000 PyGRO-0.1.0/pygro/default_metrics/__init__.py
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)     3753 2023-04-18 06:57:57.000000 PyGRO-0.1.0/pygro/geodesic.py
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)     8386 2023-04-18 06:58:01.000000 PyGRO-0.1.0/pygro/geodesic_engine.py
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)    17450 2023-04-18 06:57:43.000000 PyGRO-0.1.0/pygro/integrators.py
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)        0 2021-02-08 17:04:03.000000 PyGRO-0.1.0/pygro/interpolators.py
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)    33634 2023-04-18 06:57:42.000000 PyGRO-0.1.0/pygro/metric_engine.py
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)     4228 2022-03-24 17:38:30.000000 PyGRO-0.1.0/pygro/observer.py
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)       38 2023-04-18 07:07:26.212672 PyGRO-0.1.0/setup.cfg
--rw-r--r--   0 riccardodellamonica   (501) staff       (20)      737 2023-04-18 07:06:41.000000 PyGRO-0.1.0/setup.py
+drwxr-xr-x   0 riccardodellamonica   (501) staff       (20)        0 2023-05-30 08:31:52.043746 PyGRO-0.1.1/
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)     1065 2021-01-29 22:40:37.000000 PyGRO-0.1.1/LICENSE.txt
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)     1466 2023-05-30 08:31:52.043451 PyGRO-0.1.1/PKG-INFO
+drwxr-xr-x   0 riccardodellamonica   (501) staff       (20)        0 2023-05-30 08:31:52.038643 PyGRO-0.1.1/PyGRO.egg-info/
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)     1466 2023-05-30 08:31:51.000000 PyGRO-0.1.1/PyGRO.egg-info/PKG-INFO
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)      452 2023-05-30 08:31:51.000000 PyGRO-0.1.1/PyGRO.egg-info/SOURCES.txt
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)        1 2023-05-30 08:31:51.000000 PyGRO-0.1.1/PyGRO.egg-info/dependency_links.txt
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)       25 2023-05-30 08:31:51.000000 PyGRO-0.1.1/PyGRO.egg-info/requires.txt
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)        6 2023-05-30 08:31:51.000000 PyGRO-0.1.1/PyGRO.egg-info/top_level.txt
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)      925 2022-02-10 10:18:41.000000 PyGRO-0.1.1/README.md
+drwxr-xr-x   0 riccardodellamonica   (501) staff       (20)        0 2023-05-30 08:31:52.041158 PyGRO-0.1.1/pygro/
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)      195 2022-03-11 17:21:23.000000 PyGRO-0.1.1/pygro/__init__.py
+drwxr-xr-x   0 riccardodellamonica   (501) staff       (20)        0 2023-05-30 08:31:52.043062 PyGRO-0.1.1/pygro/default_metrics/
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)    11199 2021-04-04 11:28:03.000000 PyGRO-0.1.1/pygro/default_metrics/KerrBL.py
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)    49866 2021-05-08 10:28:38.000000 PyGRO-0.1.1/pygro/default_metrics/KerrSTVG.py
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)     2657 2021-04-04 11:28:07.000000 PyGRO-0.1.1/pygro/default_metrics/Yukawa.py
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)      130 2021-05-08 10:28:55.000000 PyGRO-0.1.1/pygro/default_metrics/__init__.py
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)     3753 2023-04-18 06:57:57.000000 PyGRO-0.1.1/pygro/geodesic.py
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)     8386 2023-04-18 06:58:01.000000 PyGRO-0.1.1/pygro/geodesic_engine.py
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)    17450 2023-04-18 06:57:43.000000 PyGRO-0.1.1/pygro/integrators.py
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)        0 2021-02-08 17:04:03.000000 PyGRO-0.1.1/pygro/interpolators.py
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)    33672 2023-05-30 08:30:29.000000 PyGRO-0.1.1/pygro/metric_engine.py
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)     4228 2022-03-24 17:38:30.000000 PyGRO-0.1.1/pygro/observer.py
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)       38 2023-05-30 08:31:52.043790 PyGRO-0.1.1/setup.cfg
+-rw-r--r--   0 riccardodellamonica   (501) staff       (20)      737 2023-05-30 08:30:39.000000 PyGRO-0.1.1/setup.py
```

### Comparing `PyGRO-0.1.0/LICENSE.txt` & `PyGRO-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PyGRO-0.1.0/PKG-INFO` & `PyGRO-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGRO
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python Integrator for General Relativistic Orbits
 Author: Riccardo Della Monica
 Author-email: dellamonicariccardo@gmail.com
 License: LICENSE.txt
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `PyGRO-0.1.0/PyGRO.egg-info/PKG-INFO` & `PyGRO-0.1.1/PyGRO.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyGRO
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python Integrator for General Relativistic Orbits
 Author: Riccardo Della Monica
 Author-email: dellamonicariccardo@gmail.com
 License: LICENSE.txt
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
```

### Comparing `PyGRO-0.1.0/README.md` & `PyGRO-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `PyGRO-0.1.0/pygro/default_metrics/KerrBL.py` & `PyGRO-0.1.1/pygro/default_metrics/KerrBL.py`

 * *Files identical despite different names*

### Comparing `PyGRO-0.1.0/pygro/default_metrics/KerrSTVG.py` & `PyGRO-0.1.1/pygro/default_metrics/KerrSTVG.py`

 * *Files identical despite different names*

### Comparing `PyGRO-0.1.0/pygro/default_metrics/Yukawa.py` & `PyGRO-0.1.1/pygro/default_metrics/Yukawa.py`

 * *Files identical despite different names*

### Comparing `PyGRO-0.1.0/pygro/geodesic.py` & `PyGRO-0.1.1/pygro/geodesic.py`

 * *Files identical despite different names*

### Comparing `PyGRO-0.1.0/pygro/geodesic_engine.py` & `PyGRO-0.1.1/pygro/geodesic_engine.py`

 * *Files identical despite different names*

### Comparing `PyGRO-0.1.0/pygro/integrators.py` & `PyGRO-0.1.1/pygro/integrators.py`

 * *Files identical despite different names*

### Comparing `PyGRO-0.1.0/pygro/metric_engine.py` & `PyGRO-0.1.1/pygro/metric_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,15 +370,16 @@
                     except:
                         raise ValueError(f"Insert a valid expression for transform function {x}")
                     else:
                         self.transform_s.append(x_symb)
                         self.transform_functions_str.append(x_inpt)
                         self.transform_functions.append(sp.lambdify([self.x], self.evaluate_parameters(x_symb), 'numpy'))
                     
-
+        self.g_ff = lambdify([*self.x, *self.get_parameters_symb()], self.subs_functions(self.g))
+        
         print("The metric_engine has been initialized.")
 
     def save_metric(self, filename):
         r"""Saves the metric into a *.metric* file which can later be loaded with the :py:func:`Metric.load_metric` method.
 
         :param filename: The name of the *.metric* file in which to save the metric.
         :type filename: str
@@ -774,15 +775,15 @@
         for mu in range(4):
             for nu in range(4):
                 norm += self.g_f(x)[mu, nu]*v[mu]*v[nu]
         
         return norm'''
     
     def g_f(self, x):
-        return lambdify([*self.x, *self.get_parameters_symb()], self.subs_functions(self.g))(*x, *self.get_parameters_val())
+        return self.g_ff(*x, *self.get_parameters_val())
 
     def Christoffel(self, mu, nu, rho):
         """The mu-nu-rho Christoffel symbol, :math:`\Gamma^{\mu}_{\nu\rho}` related to the metric tensor.
         """
         ch = 0
         for sigma in range(4):
             ch += self.g_inv[rho,sigma]*(self.g[sigma, nu].diff(self.x[mu])+self.g[mu, sigma].diff(self.x[nu])-self.g[mu, nu].diff(self.x[sigma]))/2
```

### Comparing `PyGRO-0.1.0/pygro/observer.py` & `PyGRO-0.1.1/pygro/observer.py`

 * *Files identical despite different names*

### Comparing `PyGRO-0.1.0/setup.py` & `PyGRO-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
   name='PyGRO',
-  version='0.1.0',
+  version='0.1.1',
   author='Riccardo Della Monica',
   author_email='dellamonicariccardo@gmail.com',
   packages=find_packages(),
   license='LICENSE.txt',
   description='A Python Integrator for General Relativistic Orbits',
   long_description=open('README.md').read(),
   long_description_content_type='text/markdown',
```

