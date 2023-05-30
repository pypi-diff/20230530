# Comparing `tmp/bioumlsim-0.3.1.tar.gz` & `tmp/bioumlsim-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bioumlsim-0.3.1.tar", last modified: Mon May 29 19:40:08 2023, max compression
+gzip compressed data, was "bioumlsim-0.4.0.tar", last modified: Tue May 30 09:04:11 2023, max compression
```

## Comparing `bioumlsim-0.3.1.tar` & `bioumlsim-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 19:40:08.693357 bioumlsim-0.3.1/
--rw-rw-rw-   0        0        0     1088 2023-05-17 07:27:39.000000 bioumlsim-0.3.1/LICENSE
--rw-rw-rw-   0        0        0      771 2023-05-29 19:40:08.694349 bioumlsim-0.3.1/PKG-INFO
--rw-rw-rw-   0        0        0       60 2023-05-17 07:27:39.000000 bioumlsim-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 19:40:08.601287 bioumlsim-0.3.1/bioumlsim/
--rw-rw-rw-   0        0        0     2995 2023-05-29 18:25:05.000000 bioumlsim-0.3.1/bioumlsim/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 19:40:08.690824 bioumlsim-0.3.1/bioumlsim/jars/
--rw-rw-rw-   0        0        0   386547 2023-05-26 08:30:49.000000 bioumlsim-0.3.1/bioumlsim/jars/biouml.plugins.sbml_0.9.10.jar
--rw-rw-rw-   0        0        0   615951 2023-05-26 08:30:49.000000 bioumlsim-0.3.1/bioumlsim/jars/biouml.plugins.simulation_0.9.10.jar
--rw-rw-rw-   0        0        0  2085692 2023-05-26 08:30:49.000000 bioumlsim-0.3.1/bioumlsim/jars/biouml.workbench_0.9.10.jar
--rw-rw-rw-   0        0        0   581945 2023-05-26 08:30:49.000000 bioumlsim-0.3.1/bioumlsim/jars/colt.jar
--rw-rw-rw-   0        0        0   396595 2023-05-26 08:30:49.000000 bioumlsim-0.3.1/bioumlsim/jars/com.developmentontheedge.beans-3.0.4.jar
--rw-rw-rw-   0        0        0    94331 2023-05-26 08:30:48.000000 bioumlsim-0.3.1/bioumlsim/jars/com.developmentontheedge.util_0.9.10.jar
--rw-rw-rw-   0        0        0    31222 2023-05-26 08:30:49.000000 bioumlsim-0.3.1/bioumlsim/jars/com.eclipsesource.json_0.9.4.jar
--rw-rw-rw-   0        0        0   575606 2023-05-26 08:30:49.000000 bioumlsim-0.3.1/bioumlsim/jars/org.apache.commons.collections_3.2.1.jar
--rw-rw-rw-   0        0        0   262026 2023-05-26 08:30:48.000000 bioumlsim-0.3.1/bioumlsim/jars/org.apache.commons.lang_2.4.0.jar
--rw-rw-rw-   0        0        0   421287 2023-05-26 08:30:49.000000 bioumlsim-0.3.1/bioumlsim/jars/org.apache.velocity_1.6.2.jar
--rw-rw-rw-   0        0        0    58013 2023-05-26 08:30:48.000000 bioumlsim-0.3.1/bioumlsim/jars/org.json-20170516.jar
--rw-rw-rw-   0        0        0  1251757 2023-05-26 08:30:49.000000 bioumlsim-0.3.1/bioumlsim/jars/ru.biosoft.access_0.9.10.jar
--rw-rw-rw-   0        0        0    14541 2023-05-26 08:30:49.000000 bioumlsim-0.3.1/bioumlsim/jars/ru.biosoft.exception-1.0.0.jar
--rw-rw-rw-   0        0        0   231950 2023-05-26 08:30:48.000000 bioumlsim-0.3.1/bioumlsim/jars/ru.biosoft.graph_0.9.10.jar
--rw-rw-rw-   0        0        0   197773 2023-05-26 08:30:48.000000 bioumlsim-0.3.1/bioumlsim/jars/ru.biosoft.graphics_0.9.10.jar
--rw-rw-rw-   0        0        0    26578 2023-05-26 08:30:49.000000 bioumlsim-0.3.1/bioumlsim/jars/ru.biosoft.jobcontrol-2.0.0.jar
--rw-rw-rw-   0        0        0   163699 2023-05-26 08:30:48.000000 bioumlsim-0.3.1/bioumlsim/jars/ru.biosoft.math_0.9.10.jar
--rw-rw-rw-   0        0        0    20343 2023-05-26 08:30:49.000000 bioumlsim-0.3.1/bioumlsim/jars/src.jar
--rw-rw-rw-   0        0        0   299064 2023-05-26 08:30:49.000000 bioumlsim-0.3.1/bioumlsim/jars/streamex-0.7.0.jar
--rw-rw-rw-   0        0        0      390 2023-05-22 19:11:01.000000 bioumlsim-0.3.1/bioumlsim/test.py
-drwxrwxrwx   0        0        0        0 2023-05-29 19:40:08.636414 bioumlsim-0.3.1/bioumlsim.egg-info/
--rw-rw-rw-   0        0        0      771 2023-05-29 19:40:08.000000 bioumlsim-0.3.1/bioumlsim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1115 2023-05-29 19:40:08.000000 bioumlsim-0.3.1/bioumlsim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 19:40:08.000000 bioumlsim-0.3.1/bioumlsim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-29 19:40:07.000000 bioumlsim-0.3.1/bioumlsim.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       20 2023-05-29 19:40:08.000000 bioumlsim-0.3.1/bioumlsim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-29 19:40:08.000000 bioumlsim-0.3.1/bioumlsim.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      185 2023-05-27 18:48:00.000000 bioumlsim-0.3.1/pyproject.toml
--rw-rw-rw-   0        0        0      872 2023-05-29 19:40:08.697350 bioumlsim-0.3.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-30 09:04:11.285301 bioumlsim-0.4.0/
+-rw-rw-rw-   0        0        0     1088 2023-05-17 07:27:39.000000 bioumlsim-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0      771 2023-05-30 09:04:11.286314 bioumlsim-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0       60 2023-05-17 07:27:39.000000 bioumlsim-0.4.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-30 09:04:11.175872 bioumlsim-0.4.0/bioumlsim/
+-rw-rw-rw-   0        0        0     2350 2023-05-30 08:35:52.000000 bioumlsim-0.4.0/bioumlsim/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-30 09:04:11.282287 bioumlsim-0.4.0/bioumlsim/jars/
+-rw-rw-rw-   0        0        0   386547 2023-05-26 08:30:49.000000 bioumlsim-0.4.0/bioumlsim/jars/biouml.plugins.sbml_0.9.10.jar
+-rw-rw-rw-   0        0        0   615951 2023-05-26 08:30:49.000000 bioumlsim-0.4.0/bioumlsim/jars/biouml.plugins.simulation_0.9.10.jar
+-rw-rw-rw-   0        0        0  2085692 2023-05-26 08:30:49.000000 bioumlsim-0.4.0/bioumlsim/jars/biouml.workbench_0.9.10.jar
+-rw-rw-rw-   0        0        0   581945 2023-05-26 08:30:49.000000 bioumlsim-0.4.0/bioumlsim/jars/colt.jar
+-rw-rw-rw-   0        0        0   396595 2023-05-26 08:30:49.000000 bioumlsim-0.4.0/bioumlsim/jars/com.developmentontheedge.beans-3.0.4.jar
+-rw-rw-rw-   0        0        0    94331 2023-05-26 08:30:48.000000 bioumlsim-0.4.0/bioumlsim/jars/com.developmentontheedge.util_0.9.10.jar
+-rw-rw-rw-   0        0        0    31222 2023-05-26 08:30:49.000000 bioumlsim-0.4.0/bioumlsim/jars/com.eclipsesource.json_0.9.4.jar
+-rw-rw-rw-   0        0        0   575606 2023-05-26 08:30:49.000000 bioumlsim-0.4.0/bioumlsim/jars/org.apache.commons.collections_3.2.1.jar
+-rw-rw-rw-   0        0        0   262026 2023-05-26 08:30:48.000000 bioumlsim-0.4.0/bioumlsim/jars/org.apache.commons.lang_2.4.0.jar
+-rw-rw-rw-   0        0        0   421287 2023-05-26 08:30:49.000000 bioumlsim-0.4.0/bioumlsim/jars/org.apache.velocity_1.6.2.jar
+-rw-rw-rw-   0        0        0    58013 2023-05-26 08:30:48.000000 bioumlsim-0.4.0/bioumlsim/jars/org.json-20170516.jar
+-rw-rw-rw-   0        0        0  1251757 2023-05-26 08:30:49.000000 bioumlsim-0.4.0/bioumlsim/jars/ru.biosoft.access_0.9.10.jar
+-rw-rw-rw-   0        0        0    14541 2023-05-26 08:30:49.000000 bioumlsim-0.4.0/bioumlsim/jars/ru.biosoft.exception-1.0.0.jar
+-rw-rw-rw-   0        0        0   231950 2023-05-26 08:30:48.000000 bioumlsim-0.4.0/bioumlsim/jars/ru.biosoft.graph_0.9.10.jar
+-rw-rw-rw-   0        0        0   197773 2023-05-26 08:30:48.000000 bioumlsim-0.4.0/bioumlsim/jars/ru.biosoft.graphics_0.9.10.jar
+-rw-rw-rw-   0        0        0    26578 2023-05-26 08:30:49.000000 bioumlsim-0.4.0/bioumlsim/jars/ru.biosoft.jobcontrol-2.0.0.jar
+-rw-rw-rw-   0        0        0   163699 2023-05-26 08:30:48.000000 bioumlsim-0.4.0/bioumlsim/jars/ru.biosoft.math_0.9.10.jar
+-rw-rw-rw-   0        0        0    20343 2023-05-26 08:30:49.000000 bioumlsim-0.4.0/bioumlsim/jars/src.jar
+-rw-rw-rw-   0        0        0   299064 2023-05-26 08:30:49.000000 bioumlsim-0.4.0/bioumlsim/jars/streamex-0.7.0.jar
+-rw-rw-rw-   0        0        0      323 2023-05-30 05:53:42.000000 bioumlsim-0.4.0/bioumlsim/test.py
+-rw-rw-rw-   0        0        0     1496 2023-05-30 07:46:26.000000 bioumlsim-0.4.0/bioumlsim/test.xml
+drwxrwxrwx   0        0        0        0 2023-05-30 09:04:11.205043 bioumlsim-0.4.0/bioumlsim.egg-info/
+-rw-rw-rw-   0        0        0      771 2023-05-30 09:04:11.000000 bioumlsim-0.4.0/bioumlsim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1134 2023-05-30 09:04:11.000000 bioumlsim-0.4.0/bioumlsim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-30 09:04:11.000000 bioumlsim-0.4.0/bioumlsim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-30 08:26:07.000000 bioumlsim-0.4.0/bioumlsim.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       31 2023-05-30 09:04:11.000000 bioumlsim-0.4.0/bioumlsim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-30 09:04:11.000000 bioumlsim-0.4.0/bioumlsim.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      185 2023-05-27 18:48:00.000000 bioumlsim-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0      895 2023-05-30 09:04:11.289324 bioumlsim-0.4.0/setup.cfg
```

### Comparing `bioumlsim-0.3.1/LICENSE` & `bioumlsim-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.3.1/PKG-INFO` & `bioumlsim-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioumlsim
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python interface for simulation with BioUML
 Home-page: https://www.biouml.org/
 Author: Ilya Kiselev, Biosoft.ru
 Author-email: 4x3cut0r@gmail.com
 Project-URL: Bug Tracker, https://github.com/Biosoft-ru/bioumlsim/issues
 Project-URL: Source Code, https://github.com/Biosoft-ru/bioumlsim
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bioumlsim-0.3.1/bioumlsim/__init__.py` & `bioumlsim-0.4.0/bioumlsim/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -31,14 +31,23 @@
         self.engine.setDiagram(diagram)
         self.engine.setClassPath(self.bioUMLPath +'/src.jar')
         self.engine.disableLog()
         self.engine.setAbsTolerance(self.atol)
         self.engine.setRelTolerance(self.rtol)
         return Model(self.engine, self.engine.createModel())
     
+    def plot(self, df):
+        import matplotlib.pyplot as plt
+        plt.plot(df)
+        plt.show()
+    
+    def loadTest(self):
+        path = os.path.dirname(__file__)+'/test.xml'
+        return self.load(path)
+         
 class Model:
     
     def __init__(self, engine, model):
         self.engine = engine
         self.model = model
         
     def simulate(self, tend, numpoints):
@@ -49,43 +58,13 @@
             numpoints: number of time points
         Returns:
             simulation results
         """
         print(f"Simulating model: {self.engine.getDiagram().getName()}.")
         self.engine.setCompletionTime(tend)
         self.engine.setTimeIncrement(tend / numpoints)
-        return Result(self.engine.simulateSimple(self.model), self.engine) 
-    
-class Result:
-    
-    def __init__(self, sr, engine):
-        self.sr = sr
-        self.engine = engine
-        species = engine.getFloatingSpecies()
-        self.values = np.array(sr.getValuesTransposed(species))
-        self.names = np.array(species)
-        self.times = np.array(sr.getTimes());
-        self.df = pd.DataFrame(self.values, columns = self.names, index = pd.Index(self.times, name ="Time"))
-        
-    def toFile(self, file, precision=3, separator ='\t'):
-        f = open(file, 'w')
-        f.write(np.array2string(self.names, separator=separator)[1:-1])
-        f.write('\n')
-        for row in self.values:
-            f.write(np.array2string(row, precision=precision, separator=separator)[1:-1])
-            f.write('\n')
-        f.close()
-    
-    def __str__(self):
-        return str(self.df)
-    
-    def getTimes(self):
-        return self.times
-    
-    def getNames(self):
-        return self.names
-        
-    def getValues(self, variable=None):
-        if (variable!=None):
-            return np.array(self.sr.getValues(variable))
-        else:
-            return self.values
+        result = self.engine.simulateSimple(self.model)
+        species = self.engine.getFloatingSpecies()
+        values = np.array(result.getValuesTransposed(species))
+        names = np.array(species)
+        times = np.array(result.getTimes());
+        return pd.DataFrame(values, columns = names, index = pd.Index(times, name ="Time"))
```

### Comparing `bioumlsim-0.3.1/bioumlsim/jars/biouml.plugins.sbml_0.9.10.jar` & `bioumlsim-0.4.0/bioumlsim/jars/biouml.plugins.sbml_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.3.1/bioumlsim/jars/biouml.plugins.simulation_0.9.10.jar` & `bioumlsim-0.4.0/bioumlsim/jars/biouml.plugins.simulation_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.3.1/bioumlsim/jars/biouml.workbench_0.9.10.jar` & `bioumlsim-0.4.0/bioumlsim/jars/biouml.workbench_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.3.1/bioumlsim/jars/colt.jar` & `bioumlsim-0.4.0/bioumlsim/jars/colt.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.3.1/bioumlsim/jars/com.developmentontheedge.beans-3.0.4.jar` & `bioumlsim-0.4.0/bioumlsim/jars/com.developmentontheedge.beans-3.0.4.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.3.1/bioumlsim/jars/com.developmentontheedge.util_0.9.10.jar` & `bioumlsim-0.4.0/bioumlsim/jars/com.developmentontheedge.util_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.3.1/bioumlsim/jars/com.eclipsesource.json_0.9.4.jar` & `bioumlsim-0.4.0/bioumlsim/jars/com.eclipsesource.json_0.9.4.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.3.1/bioumlsim/jars/org.apache.commons.collections_3.2.1.jar` & `bioumlsim-0.4.0/bioumlsim/jars/org.apache.commons.collections_3.2.1.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.3.1/bioumlsim/jars/org.apache.commons.lang_2.4.0.jar` & `bioumlsim-0.4.0/bioumlsim/jars/org.apache.commons.lang_2.4.0.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.3.1/bioumlsim/jars/org.apache.velocity_1.6.2.jar` & `bioumlsim-0.4.0/bioumlsim/jars/org.apache.velocity_1.6.2.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.3.1/bioumlsim/jars/org.json-20170516.jar` & `bioumlsim-0.4.0/bioumlsim/jars/org.json-20170516.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.3.1/bioumlsim/jars/ru.biosoft.access_0.9.10.jar` & `bioumlsim-0.4.0/bioumlsim/jars/ru.biosoft.access_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.3.1/bioumlsim/jars/ru.biosoft.exception-1.0.0.jar` & `bioumlsim-0.4.0/bioumlsim/jars/ru.biosoft.exception-1.0.0.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.3.1/bioumlsim/jars/ru.biosoft.graph_0.9.10.jar` & `bioumlsim-0.4.0/bioumlsim/jars/ru.biosoft.graph_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.3.1/bioumlsim/jars/ru.biosoft.graphics_0.9.10.jar` & `bioumlsim-0.4.0/bioumlsim/jars/ru.biosoft.graphics_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.3.1/bioumlsim/jars/ru.biosoft.jobcontrol-2.0.0.jar` & `bioumlsim-0.4.0/bioumlsim/jars/ru.biosoft.jobcontrol-2.0.0.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.3.1/bioumlsim/jars/ru.biosoft.math_0.9.10.jar` & `bioumlsim-0.4.0/bioumlsim/jars/ru.biosoft.math_0.9.10.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.3.1/bioumlsim/jars/src.jar` & `bioumlsim-0.4.0/bioumlsim/jars/src.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.3.1/bioumlsim/jars/streamex-0.7.0.jar` & `bioumlsim-0.4.0/bioumlsim/jars/streamex-0.7.0.jar`

 * *Files identical despite different names*

### Comparing `bioumlsim-0.3.1/bioumlsim.egg-info/PKG-INFO` & `bioumlsim-0.4.0/bioumlsim.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bioumlsim
-Version: 0.3.1
+Version: 0.4.0
 Summary: Python interface for simulation with BioUML
 Home-page: https://www.biouml.org/
 Author: Ilya Kiselev, Biosoft.ru
 Author-email: 4x3cut0r@gmail.com
 Project-URL: Bug Tracker, https://github.com/Biosoft-ru/bioumlsim/issues
 Project-URL: Source Code, https://github.com/Biosoft-ru/bioumlsim
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bioumlsim-0.3.1/bioumlsim.egg-info/SOURCES.txt` & `bioumlsim-0.4.0/bioumlsim.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 bioumlsim/__init__.py
 bioumlsim/test.py
+bioumlsim/test.xml
 bioumlsim.egg-info/PKG-INFO
 bioumlsim.egg-info/SOURCES.txt
 bioumlsim.egg-info/dependency_links.txt
 bioumlsim.egg-info/not-zip-safe
 bioumlsim.egg-info/requires.txt
 bioumlsim.egg-info/top_level.txt
 bioumlsim/jars/biouml.plugins.sbml_0.9.10.jar
```

### Comparing `bioumlsim-0.3.1/setup.cfg` & `bioumlsim-0.4.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 696f 756d 6c73 696d 0d0a 7665   = bioumlsim..ve
-00000020: 7273 696f 6e20 3d20 302e 332e 310d 0a61  rsion = 0.3.1..a
+00000020: 7273 696f 6e20 3d20 302e 342e 300d 0a61  rsion = 0.4.0..a
 00000030: 7574 686f 7220 3d20 496c 7961 204b 6973  uthor = Ilya Kis
 00000040: 656c 6576 2c20 4269 6f73 6f66 742e 7275  elev, Biosoft.ru
 00000050: 0d0a 6175 7468 6f72 5f65 6d61 696c 203d  ..author_email =
 00000060: 2034 7833 6375 7430 7240 676d 6169 6c2e   4x3cut0r@gmail.
 00000070: 636f 6d0d 0a64 6573 6372 6970 7469 6f6e  com..description
 00000080: 203d 2050 7974 686f 6e20 696e 7465 7266   = Python interf
 00000090: 6163 6520 666f 7220 7369 6d75 6c61 7469  ace for simulati
@@ -42,14 +42,15 @@
 00000290: 6f70 7469 6f6e 735d 0d0a 7061 636b 6167  options]..packag
 000002a0: 6573 203d 2062 696f 756d 6c73 696d 0d0a  es = bioumlsim..
 000002b0: 7079 7468 6f6e 5f72 6571 7569 7265 7320  python_requires 
 000002c0: 3d20 3e3d 332e 360d 0a7a 6970 5f73 6166  = >=3.6..zip_saf
 000002d0: 6520 3d20 4661 6c73 650d 0a69 6e73 7461  e = False..insta
 000002e0: 6c6c 5f72 6571 7569 7265 7320 3d20 0d0a  ll_requires = ..
 000002f0: 096a 7079 7065 310d 0a09 6e75 6d70 790d  .jpype1...numpy.
-00000300: 0a09 7061 6e64 6173 0d0a 0d0a 5b6f 7074  ..pandas....[opt
-00000310: 696f 6e73 2e70 6163 6b61 6765 5f64 6174  ions.package_dat
-00000320: 615d 0d0a 6269 6f75 6d6c 7369 6d20 3d20  a]..bioumlsim = 
-00000330: 6a61 7273 2f2a 2e6a 6172 0d0a 0d0a 5b65  jars/*.jar....[e
-00000340: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-00000350: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-00000360: 203d 2030 0d0a 0d0a                       = 0....
+00000300: 0a09 7061 6e64 6173 0d0a 096d 6174 706c  ..pandas...matpl
+00000310: 6f74 6c69 620d 0a0d 0a5b 6f70 7469 6f6e  otlib....[option
+00000320: 732e 7061 636b 6167 655f 6461 7461 5d0d  s.package_data].
+00000330: 0a62 696f 756d 6c73 696d 203d 206a 6172  .bioumlsim = jar
+00000340: 732f 2a2e 6a61 722c 2074 6573 742e 786d  s/*.jar, test.xm
+00000350: 6c0d 0a0d 0a5b 6567 675f 696e 666f 5d0d  l....[egg_info].
+00000360: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
+00000370: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
```

