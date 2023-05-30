# Comparing `tmp/fossiler-0.0.4.2.tar.gz` & `tmp/fossiler-0.0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fossiler-0.0.4.2.tar", last modified: Tue May 30 05:04:39 2023, max compression
+gzip compressed data, was "dist/fossiler-0.0.4.3.tar", last modified: Tue May 30 05:18:04 2023, max compression
```

## Comparing `fossiler-0.0.4.2.tar` & `fossiler-0.0.4.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-30 05:04:39.869857 fossiler-0.0.4.2/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    35149 2023-05-11 08:47:25.000000 fossiler-0.0.4.2/LICENSE
--rwxrwxrwx   0 heche     (1000) heche     (1000)    84889 2023-05-30 05:04:39.869857 fossiler-0.0.4.2/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)    77526 2023-05-30 05:03:57.000000 fossiler-0.0.4.2/README.md
--rwxrwxrwx   0 heche     (1000) heche     (1000)     2663 2023-05-29 21:11:35.000000 fossiler-0.0.4.2/command.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-30 05:04:39.869857 fossiler-0.0.4.2/fossiler/
--rwxrwxrwx   0 heche     (1000) heche     (1000)   145833 2023-05-30 05:00:39.000000 fossiler-0.0.4.2/fossiler/fossils.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-30 05:04:39.869857 fossiler-0.0.4.2/fossiler.egg-info/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    84889 2023-05-30 05:04:39.000000 fossiler-0.0.4.2/fossiler.egg-info/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)      261 2023-05-30 05:04:39.000000 fossiler-0.0.4.2/fossiler.egg-info/SOURCES.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-05-30 05:04:39.000000 fossiler-0.0.4.2/fossiler.egg-info/dependency_links.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)       60 2023-05-30 05:04:39.000000 fossiler-0.0.4.2/fossiler.egg-info/entry_points.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)       56 2023-05-30 05:04:39.000000 fossiler-0.0.4.2/fossiler.egg-info/requires.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)       17 2023-05-30 05:04:39.000000 fossiler-0.0.4.2/fossiler.egg-info/top_level.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-05-30 05:04:39.869857 fossiler-0.0.4.2/setup.cfg
--rwxrwxrwx   0 heche     (1000) heche     (1000)      803 2023-05-30 05:03:42.000000 fossiler-0.0.4.2/setup.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-30 05:18:04.475927 fossiler-0.0.4.3/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    35149 2023-05-11 08:47:25.000000 fossiler-0.0.4.3/LICENSE
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    84889 2023-05-30 05:18:04.475927 fossiler-0.0.4.3/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    77526 2023-05-30 05:03:57.000000 fossiler-0.0.4.3/README.md
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     2663 2023-05-29 21:11:35.000000 fossiler-0.0.4.3/command.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-30 05:18:04.475927 fossiler-0.0.4.3/fossiler/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   146036 2023-05-30 05:16:45.000000 fossiler-0.0.4.3/fossiler/fossils.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-30 05:18:04.475927 fossiler-0.0.4.3/fossiler.egg-info/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    84889 2023-05-30 05:18:04.000000 fossiler-0.0.4.3/fossiler.egg-info/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      261 2023-05-30 05:18:04.000000 fossiler-0.0.4.3/fossiler.egg-info/SOURCES.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-05-30 05:18:04.000000 fossiler-0.0.4.3/fossiler.egg-info/dependency_links.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)       60 2023-05-30 05:18:04.000000 fossiler-0.0.4.3/fossiler.egg-info/entry_points.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)       56 2023-05-30 05:18:04.000000 fossiler-0.0.4.3/fossiler.egg-info/requires.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)       17 2023-05-30 05:18:04.000000 fossiler-0.0.4.3/fossiler.egg-info/top_level.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-05-30 05:18:04.475927 fossiler-0.0.4.3/setup.cfg
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      803 2023-05-30 05:14:32.000000 fossiler-0.0.4.3/setup.py
```

### Comparing `fossiler-0.0.4.2/LICENSE` & `fossiler-0.0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fossiler-0.0.4.2/PKG-INFO` & `fossiler-0.0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fossiler
-Version: 0.0.4.2
+Version: 0.0.4.3
 Summary: Python package and CLI for finding available fossils
 Home-page: http://github.com/heche-psb/fossiler
 Author: Hengchi Chen
 Author-email: heche@psb.vib-ugent.be
 License: GPL
 Description: <div align="center">
```

### Comparing `fossiler-0.0.4.2/README.md` & `fossiler-0.0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `fossiler-0.0.4.2/command.py` & `fossiler-0.0.4.3/command.py`

 * *Files identical despite different names*

### Comparing `fossiler-0.0.4.2/fossiler/fossils.py` & `fossiler-0.0.4.3/fossiler/fossils.py`

 * *Files 0% similar despite different names*

```diff
@@ -242,15 +242,21 @@
         #added_num = len(Orders_replace_Species[i].split(',')) - 1
         #final_sp_num = original_sp_num + added_num
         content = content.replace(i,Orders_replace_Species[i])
     handle = StringIO(content.split("\n")[1])
     Tree = Phylo.read(handle,"newick")
     spnum = len(Tree.get_terminals())
     with open("sp{}_species_list".format(spnum),"w") as f:
-        for i in Tree.get_terminals(): f.write("{}\n".format(i.name))
+        focussp = ''
+        for i in Tree.get_terminals():
+            if i.name.endswith("_ap2") or i.name.endswith("_ap1"):
+                focussp = i.name[:-4]
+                continue
+            f.write("{}\n".format(i.name))
+        f.write("{}\n".format(focussp))
     content = content.replace(str(original_sp_num)+" ",str(spnum)+" ")
     return content, spnum
 
 def getproperstartingtree(treef,number,outdir):
     # Only works for order-level/or more recent WGDs
     Tree = Phylo.read(treef,"newick")
     Clade_names = [i.name for i in Tree.get_terminals()]
```

### Comparing `fossiler-0.0.4.2/fossiler.egg-info/PKG-INFO` & `fossiler-0.0.4.3/fossiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fossiler
-Version: 0.0.4.2
+Version: 0.0.4.3
 Summary: Python package and CLI for finding available fossils
 Home-page: http://github.com/heche-psb/fossiler
 Author: Hengchi Chen
 Author-email: heche@psb.vib-ugent.be
 License: GPL
 Description: <div align="center">
```

### Comparing `fossiler-0.0.4.2/setup.py` & `fossiler-0.0.4.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='fossiler',
-    version='0.0.4.2',
+    version='0.0.4.3',
     packages=['fossiler'],
     url='http://github.com/heche-psb/fossiler',
     license='GPL',
     author='Hengchi Chen',
     author_email='heche@psb.vib-ugent.be',
     description='Python package and CLI for finding available fossils',
     long_description=long_description,
```

