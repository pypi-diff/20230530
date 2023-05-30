# Comparing `tmp/geostat-0.8.3.tar.gz` & `tmp/geostat-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/whdc/git/geostat/dist/.tmp-q5pzns9y/geostat-0.8.3.tar", last modified: Fri Apr 21 18:09:19 2023, max compression
+gzip compressed data, was "geostat-0.9.0.tar", last modified: Tue May 30 04:31:41 2023, max compression
```

## Comparing `geostat-0.8.3.tar` & `geostat-0.9.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-21 18:09:19.382182 geostat-0.8.3/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    11357 2022-08-12 07:59:13.000000 geostat-0.8.3/LICENSE
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-04-21 18:09:19.382182 geostat-0.8.3/PKG-INFO
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      687 2022-08-12 07:59:13.000000 geostat-0.8.3/README.md
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      679 2023-04-21 15:52:57.000000 geostat-0.8.3/pyproject.toml
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      926 2023-04-21 18:09:19.382182 geostat-0.8.3/setup.cfg
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-21 18:09:19.378182 geostat-0.8.3/src/
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-21 18:09:19.382182 geostat-0.8.3/src/geostat/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      268 2023-04-21 15:51:28.000000 geostat-0.8.3/src/geostat/__init__.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    18354 2023-04-21 15:51:20.000000 geostat-0.8.3/src/geostat/kernel.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    25489 2023-03-05 02:04:42.000000 geostat-0.8.3/src/geostat/krige.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3658 2023-04-10 22:02:47.000000 geostat-0.8.3/src/geostat/mean.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2620 2022-08-16 21:11:34.000000 geostat-0.8.3/src/geostat/mesh.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2557 2023-03-05 02:04:42.000000 geostat-0.8.3/src/geostat/metric.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    22135 2023-04-10 22:15:32.000000 geostat-0.8.3/src/geostat/model.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3424 2023-04-10 21:29:01.000000 geostat-0.8.3/src/geostat/op.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3167 2023-04-12 00:49:25.000000 geostat-0.8.3/src/geostat/param.py
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-21 18:09:19.382182 geostat-0.8.3/src/geostat.egg-info/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-04-21 18:09:19.000000 geostat-0.8.3/src/geostat.egg-info/PKG-INFO
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      592 2023-04-21 18:09:19.000000 geostat-0.8.3/src/geostat.egg-info/SOURCES.txt
--rw-rw-r--   0 whdc      (1000) whdc      (1000)        1 2023-04-21 18:09:19.000000 geostat-0.8.3/src/geostat.egg-info/dependency_links.txt
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      143 2023-04-21 18:09:19.000000 geostat-0.8.3/src/geostat.egg-info/requires.txt
--rw-rw-r--   0 whdc      (1000) whdc      (1000)        8 2023-04-21 18:09:19.000000 geostat-0.8.3/src/geostat.egg-info/top_level.txt
-drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-04-21 18:09:19.382182 geostat-0.8.3/tests/
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     4635 2023-04-10 21:29:01.000000 geostat-0.8.3/tests/test_antiderivative.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3732 2023-04-10 22:36:21.000000 geostat-0.8.3/tests/test_delta.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     5731 2023-04-10 21:29:01.000000 geostat-0.8.3/tests/test_gp.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     1147 2022-08-12 07:59:13.000000 geostat-0.8.3/tests/test_krige.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3507 2023-04-10 22:36:43.000000 geostat-0.8.3/tests/test_mcmc.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)      768 2022-08-12 08:18:35.000000 geostat-0.8.3/tests/test_mesh.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2625 2023-04-10 21:50:09.000000 geostat-0.8.3/tests/test_metric.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     2582 2023-04-10 22:14:06.000000 geostat-0.8.3/tests/test_multigp.py
--rw-rw-r--   0 whdc      (1000) whdc      (1000)     3761 2023-04-10 21:52:59.000000 geostat-0.8.3/tests/test_trend.py
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-05-30 04:31:41.238866 geostat-0.9.0/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    11357 2023-04-25 00:54:47.000000 geostat-0.9.0/LICENSE
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-05-30 04:31:41.238866 geostat-0.9.0/PKG-INFO
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      687 2023-04-25 00:54:47.000000 geostat-0.9.0/README.md
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      679 2023-05-30 04:29:49.000000 geostat-0.9.0/pyproject.toml
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      926 2023-05-30 04:31:41.238866 geostat-0.9.0/setup.cfg
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-05-30 04:31:41.234866 geostat-0.9.0/src/
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-05-30 04:31:41.234866 geostat-0.9.0/src/geostat/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      268 2023-05-30 04:29:31.000000 geostat-0.9.0/src/geostat/__init__.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    20973 2023-05-30 00:23:01.000000 geostat-0.9.0/src/geostat/kernel.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    25489 2023-04-25 00:54:47.000000 geostat-0.9.0/src/geostat/krige.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3658 2023-04-25 05:30:44.000000 geostat-0.9.0/src/geostat/mean.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2620 2023-04-25 00:54:47.000000 geostat-0.9.0/src/geostat/mesh.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2557 2023-04-25 00:54:47.000000 geostat-0.9.0/src/geostat/metric.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    22135 2023-05-30 00:28:09.000000 geostat-0.9.0/src/geostat/model.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3081 2023-05-30 04:22:25.000000 geostat-0.9.0/src/geostat/op.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3163 2023-05-30 00:23:13.000000 geostat-0.9.0/src/geostat/param.py
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-05-30 04:31:41.234866 geostat-0.9.0/src/geostat.egg-info/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)    14298 2023-05-30 04:31:41.000000 geostat-0.9.0/src/geostat.egg-info/PKG-INFO
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      616 2023-05-30 04:31:41.000000 geostat-0.9.0/src/geostat.egg-info/SOURCES.txt
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)        1 2023-05-30 04:31:41.000000 geostat-0.9.0/src/geostat.egg-info/dependency_links.txt
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      143 2023-05-30 04:31:41.000000 geostat-0.9.0/src/geostat.egg-info/requires.txt
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)        8 2023-05-30 04:31:41.000000 geostat-0.9.0/src/geostat.egg-info/top_level.txt
+drwxrwxr-x   0 whdc      (1000) whdc      (1000)        0 2023-05-30 04:31:41.238866 geostat-0.9.0/tests/
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     4635 2023-04-25 05:30:44.000000 geostat-0.9.0/tests/test_antiderivative.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3732 2023-04-25 05:30:44.000000 geostat-0.9.0/tests/test_delta.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     5731 2023-04-25 05:30:44.000000 geostat-0.9.0/tests/test_gp.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     1147 2023-04-25 00:54:47.000000 geostat-0.9.0/tests/test_krige.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3507 2023-04-25 05:30:44.000000 geostat-0.9.0/tests/test_mcmc.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)      768 2023-04-25 00:54:47.000000 geostat-0.9.0/tests/test_mesh.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2625 2023-04-25 05:30:44.000000 geostat-0.9.0/tests/test_metric.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     2582 2023-04-25 05:30:44.000000 geostat-0.9.0/tests/test_multigp.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     1393 2023-05-30 00:23:01.000000 geostat-0.9.0/tests/test_quadstack.py
+-rw-rw-r--   0 whdc      (1000) whdc      (1000)     3761 2023-04-25 05:30:44.000000 geostat-0.9.0/tests/test_trend.py
```

### Comparing `geostat-0.8.3/LICENSE` & `geostat-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geostat-0.8.3/PKG-INFO` & `geostat-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geostat
-Version: 0.8.3
+Version: 0.9.0
 Summary: Model spatial data with Gaussian processes
 Home-page: https://code.usgs.gov/mjstephens/geostat
 Author: Michael J. Stephens, Will Chang
 Author-email: "Michael J. Stephens" <mjstephens@usgs.gov>, Will Chang <will@hypergradient.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `geostat-0.8.3/README.md` & `geostat-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `geostat-0.8.3/pyproject.toml` & `geostat-0.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "geostat"
-version = "0.8.3"
+version = "0.9.0"
 description = "Model spatial data with Gaussian processes"
 readme = "README.md"
 authors = [
   {name="Michael J. Stephens", email="mjstephens@usgs.gov"},
   {name="Will Chang", email="will@hypergradient.ai"}
 ]
 license = { file = "LICENSE" }
```

### Comparing `geostat-0.8.3/setup.cfg` & `geostat-0.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = geostat
-version = 0.8.3
+version = 0.9.0
 author = Michael J. Stephens, Will Chang
 author_email = mjstephens@usgs.gov, will@hypergradient.ai
 description = Python package for performing kriging and Gaussian processes with geoscience-oriented utilities.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://code.usgs.gov/mjstephens/geostat
 project_urls =
```

### Comparing `geostat-0.8.3/src/geostat/kernel.py` & `geostat-0.9.0/src/geostat/kernel.py`

 * *Files 8% similar despite different names*

```diff
@@ -206,35 +206,126 @@
 
         return rampstack(tf.sqrt(e['d2']), v['sill'], v['range'])
 
     def reg(self, p):
         v = get_parameter_values(self.fa, p)
         return v['range']
 
+@tf.recompute_grad
+def smooth_convex(x, sills, ranges):
+    """
+    `x` has arbitrary shape [...], but must be non-negative.
+    `sills` and `ranges` both have shape [K].
+    """
+    r2 = ranges
+    r1 = tf.pad(ranges[:-1], [[1, 0]])
+    ex = ed(x)
+    ax = tf.abs(ex)
+    rx = ax / r2 - 1.
+
+    c1 = 2. / (r1 + r2)
+    c2 = 1. / (1. - tf.square(r1/r2))
+
+    # i1 = tf.cast(ax <= r1, tf.float32) # Indicates x <= r1.
+    # i2 = tf.cast(ax <= r2, tf.float32) * (1. - i1) # Indicates r1 < x <= r2.
+    # v = i1 * (1. - c1 * ax) + i2 * c2 * tf.square(rx)
+
+    v = tf.where(ax <= r1, 1. - c1 * ax, c2 * tf.square(rx))
+    v = tf.where(ax <= r2, v, 0.)
+
+    y = tf.einsum('...k,k->...', v, sills)
+    return y
+
 @tf.custom_gradient
-def quadstack(x, sills, ranges):
+def smooth_convex_grad(x, sills, ranges):
     """
     `x` has arbitrary shape [...], but must be non-negative.
     `sills` and `ranges` both have shape [K].
     """
+    r2 = ranges
+    r1 = tf.pad(ranges[:-1], [[1, 0]])
     ex = ed(x)
-    ax = tf.maximum(0., 1. - tf.abs(ex) / ranges) # [..., 1]
-    y = sills * tf.square(ax) # [..., K]
+    ax = tf.abs(ex)
+    rx = ax / r2 - 1.
+
+    c1 = 2. / (r1 + r2)
+    c2 = 1. / (1. - tf.square(r1/r2))
+
+    v = tf.where(ax <= r1, 1. - c1 * ax, c2 * tf.square(rx))
+    v = tf.where(ax <= r2, v, 0.)
+
+    y = tf.einsum('...k,k->...', v, sills)
+
     def grad(upstream):
+        r2 = ranges
+        r1 = tf.pad(ranges[:-1], [[1, 0]])
         ex = ed(x)
-        ax = tf.maximum(0., 1. - tf.abs(ex) / ranges) # [..., 1]
-        y = sills * tf.square(ax) # [..., K]
+        ax = tf.abs(ex)
+        rx = ax / r2 - 1.
+        i1 = tf.cast(ax <= r1, tf.float32) # Indicates x <= r1.
+        i2 = tf.cast(ax <= r2, tf.float32) * (1. - i1) # Indicates r1 < x <= r2.
+
+        c1 = 2. / (r1 + r2)
+        c2 = 1. / (1. - tf.square(r1 / r2))
+        c3 = 1. / (r2 - tf.square(r1) / r2)
+
+        v = i1 * (1. - c1 * ax) + i2 * c2 * tf.square(rx)
+
         sx = tf.sign(ex)
-        gx = sx * ax * (-2. * sills / ranges) 
+
         K = tf.shape(sills)[0]
+        gx = sx * sills * (i1 * -c1 + i2 * rx * (2 * c3))
         grad_x = upstream * tf.reduce_sum(gx, -1) # [...]
-        grad_sills = tf.einsum('ak,a->k', tf.reshape(y, [-1, K]), tf.reshape(upstream, [-1]))
-        grad_ranges = tf.einsum('ak,a->k', tf.reshape(-gx / ranges, [-1, K]), tf.reshape(upstream, [-1]))
+
+        grad_sills = tf.einsum('ak,a->k', tf.reshape(v, [-1, K]), tf.reshape(upstream, [-1]))
+
+        u = 2 / tf.square(r1 + r2) * ax * i1
+        yr1 = u + i2 * tf.square(rx * c3) * 2 * r1
+        yr2 = u - 2 * i2 * (rx * c3 + tf.square(rx * c2) / r2)
+        yr1 = sills * tf.reshape(yr1, [-1, K])
+        yr2 = sills * tf.reshape(yr2, [-1, K])
+        yr = tf.pad(yr1[:, 1:], [[0, 0], [0, 1]]) + yr2
+        grad_ranges = tf.einsum('ak,a->k', yr, tf.reshape(upstream, [-1]))
+
         return grad_x, grad_sills, grad_ranges
-    return tf.reduce_sum(y, -1), grad
+
+    return y, grad
+
+class SmoothConvex(Kernel):
+    def __init__(self, range='range', sill='sill', scale=None, metric=None):
+        fa = dict(sill=sill, range=range, scale=scale)
+        autoinputs = scale_to_metric(scale, metric)
+        super().__init__(fa, dict(d2=autoinputs))
+
+    def vars(self):
+        return ppp_list(self.fa['sill']) + ppp_list(self.fa['range'])
+
+    def call(self, p, e):
+        v = get_parameter_values(self.fa, p)
+        if isinstance(v['sill'], (tuple, list)):
+            v['sill'] = tf.stack(v['sill'])
+        if isinstance(v['range'], (tuple, list)):
+            v['range'] = tf.stack(v['range'])
+
+        return smooth_convex(tf.sqrt(e['d2']), v['sill'], v['range'])
+
+    def reg(self, p):
+        v = get_parameter_values(self.fa, p)
+        return v['range']
+
+@tf.recompute_grad
+def quadstack(x, sills, ranges):
+    """
+    `x` has arbitrary shape [...], but must be non-negative.
+    `sills` and `ranges` both have shape [K].
+    """
+    ex = ed(x)
+    ax = tf.maximum(0., 1. - tf.abs(ex) / ranges) # [..., 1]
+    y = sills * tf.square(ax) # [..., K]
+    return tf.reduce_sum(y, -1)
 
 class QuadStack(Kernel):
     def __init__(self, range='range', sill='sill', scale=None, metric=None):
         fa = dict(sill=sill, range=range, scale=scale)
         autoinputs = scale_to_metric(scale, metric)
         super().__init__(fa, dict(d2=autoinputs))
```

### Comparing `geostat-0.8.3/src/geostat/krige.py` & `geostat-0.9.0/src/geostat/krige.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.3/src/geostat/mean.py` & `geostat-0.9.0/src/geostat/mean.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.3/src/geostat/mesh.py` & `geostat-0.9.0/src/geostat/mesh.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.3/src/geostat/metric.py` & `geostat-0.9.0/src/geostat/metric.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.3/src/geostat/model.py` & `geostat-0.9.0/src/geostat/model.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.3/src/geostat/op.py` & `geostat-0.9.0/src/geostat/op.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from dataclasses import dataclass
 from typing import Dict
+from tensorflow.core.function.trace_type import default_types
 
 # Tensorflow is extraordinarily noisy. Catch warnings during import.
 import warnings
 with warnings.catch_warnings():
     warnings.filterwarnings("ignore", category=DeprecationWarning)
     import tensorflow as tf
 
@@ -75,29 +76,15 @@
             cache['__save__'].append(self)
 
         return cache[id(self)]
 
     def __tf_tracing_type__(self, context):
         return SingletonTraceType(self)
 
-class SingletonTraceType(tf.types.experimental.TraceType):
+class SingletonTraceType(default_types.Literal):
     """
     A trace type to override TF's default behavior, which is
     to treat dataclass-based onjects as dicts.
     """
-
     def __init__(self, thing):
-       self.thing = thing
-       pass
-
-    def is_subtype_of(self, other):
-       return type(other) is SingletonTraceType \
-           and self.thing is other.thing
-
-    def most_specific_common_supertype(self, others):
-       return self if all(self == other for other in others) else None
-
-    def __eq__(self, other):
-       return isinstance(other, SingletonTraceType) and self.thing == other.thing
-
-    def __hash__(self):
-       return hash(id(self.thing))
+        self.value = thing
+        self._value_hash = hash(id(thing))
```

### Comparing `geostat-0.8.3/src/geostat/param.py` & `geostat-0.9.0/src/geostat/param.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,15 +54,15 @@
         for name, v in parameters.items():
             v = self.bounds[name].get_surface_parameter(v)
             if numpy: v = v.numpy()
             sp[name] = v
         return sp
 
     def __tf_tracing_type__(self, context):
-            return SingletonTraceType(type(self))
+        return SingletonTraceType(type(self))
 
 @dataclass(frozen=True)
 class PaperParameter:
     name: str
     lo: float
     hi: float
```

### Comparing `geostat-0.8.3/src/geostat.egg-info/PKG-INFO` & `geostat-0.9.0/src/geostat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geostat
-Version: 0.8.3
+Version: 0.9.0
 Summary: Model spatial data with Gaussian processes
 Home-page: https://code.usgs.gov/mjstephens/geostat
 Author: Michael J. Stephens, Will Chang
 Author-email: "Michael J. Stephens" <mjstephens@usgs.gov>, Will Chang <will@hypergradient.ai>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `geostat-0.8.3/src/geostat.egg-info/SOURCES.txt` & `geostat-0.9.0/src/geostat.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -20,8 +20,9 @@
 tests/test_delta.py
 tests/test_gp.py
 tests/test_krige.py
 tests/test_mcmc.py
 tests/test_mesh.py
 tests/test_metric.py
 tests/test_multigp.py
+tests/test_quadstack.py
 tests/test_trend.py
```

### Comparing `geostat-0.8.3/tests/test_antiderivative.py` & `geostat-0.9.0/tests/test_antiderivative.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.3/tests/test_delta.py` & `geostat-0.9.0/tests/test_delta.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.3/tests/test_gp.py` & `geostat-0.9.0/tests/test_gp.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.3/tests/test_krige.py` & `geostat-0.9.0/tests/test_krige.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.3/tests/test_mcmc.py` & `geostat-0.9.0/tests/test_mcmc.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.3/tests/test_mesh.py` & `geostat-0.9.0/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.3/tests/test_metric.py` & `geostat-0.9.0/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.3/tests/test_multigp.py` & `geostat-0.9.0/tests/test_multigp.py`

 * *Files identical despite different names*

### Comparing `geostat-0.8.3/tests/test_trend.py` & `geostat-0.9.0/tests/test_trend.py`

 * *Files identical despite different names*

