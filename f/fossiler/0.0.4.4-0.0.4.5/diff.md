# Comparing `tmp/fossiler-0.0.4.4.tar.gz` & `tmp/fossiler-0.0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fossiler-0.0.4.4.tar", last modified: Tue May 30 05:25:17 2023, max compression
+gzip compressed data, was "dist/fossiler-0.0.4.5.tar", last modified: Tue May 30 05:39:27 2023, max compression
```

## Comparing `fossiler-0.0.4.4.tar` & `fossiler-0.0.4.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-30 05:25:17.051390 fossiler-0.0.4.4/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    35149 2023-05-11 08:47:25.000000 fossiler-0.0.4.4/LICENSE
--rwxrwxrwx   0 heche     (1000) heche     (1000)    84889 2023-05-30 05:25:17.051390 fossiler-0.0.4.4/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)    77526 2023-05-30 05:03:57.000000 fossiler-0.0.4.4/README.md
--rwxrwxrwx   0 heche     (1000) heche     (1000)     2663 2023-05-29 21:11:35.000000 fossiler-0.0.4.4/command.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-30 05:25:17.041182 fossiler-0.0.4.4/fossiler/
--rwxrwxrwx   0 heche     (1000) heche     (1000)   146034 2023-05-30 05:24:57.000000 fossiler-0.0.4.4/fossiler/fossils.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-30 05:25:17.051390 fossiler-0.0.4.4/fossiler.egg-info/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    84889 2023-05-30 05:25:16.000000 fossiler-0.0.4.4/fossiler.egg-info/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)      261 2023-05-30 05:25:17.000000 fossiler-0.0.4.4/fossiler.egg-info/SOURCES.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-05-30 05:25:16.000000 fossiler-0.0.4.4/fossiler.egg-info/dependency_links.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)       60 2023-05-30 05:25:16.000000 fossiler-0.0.4.4/fossiler.egg-info/entry_points.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)       56 2023-05-30 05:25:16.000000 fossiler-0.0.4.4/fossiler.egg-info/requires.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)       17 2023-05-30 05:25:16.000000 fossiler-0.0.4.4/fossiler.egg-info/top_level.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-05-30 05:25:17.051390 fossiler-0.0.4.4/setup.cfg
--rwxrwxrwx   0 heche     (1000) heche     (1000)      803 2023-05-30 05:25:14.000000 fossiler-0.0.4.4/setup.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-30 05:39:27.243105 fossiler-0.0.4.5/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    35149 2023-05-11 08:47:25.000000 fossiler-0.0.4.5/LICENSE
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    84889 2023-05-30 05:39:27.243105 fossiler-0.0.4.5/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    77526 2023-05-30 05:03:57.000000 fossiler-0.0.4.5/README.md
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     2663 2023-05-29 21:11:35.000000 fossiler-0.0.4.5/command.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-30 05:39:27.231939 fossiler-0.0.4.5/fossiler/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   146375 2023-05-30 05:38:16.000000 fossiler-0.0.4.5/fossiler/fossils.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-30 05:39:27.243105 fossiler-0.0.4.5/fossiler.egg-info/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    84889 2023-05-30 05:39:27.000000 fossiler-0.0.4.5/fossiler.egg-info/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      261 2023-05-30 05:39:27.000000 fossiler-0.0.4.5/fossiler.egg-info/SOURCES.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-05-30 05:39:27.000000 fossiler-0.0.4.5/fossiler.egg-info/dependency_links.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)       60 2023-05-30 05:39:27.000000 fossiler-0.0.4.5/fossiler.egg-info/entry_points.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)       56 2023-05-30 05:39:27.000000 fossiler-0.0.4.5/fossiler.egg-info/requires.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)       17 2023-05-30 05:39:27.000000 fossiler-0.0.4.5/fossiler.egg-info/top_level.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-05-30 05:39:27.247114 fossiler-0.0.4.5/setup.cfg
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      803 2023-05-30 05:38:58.000000 fossiler-0.0.4.5/setup.py
```

### Comparing `fossiler-0.0.4.4/LICENSE` & `fossiler-0.0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fossiler-0.0.4.4/PKG-INFO` & `fossiler-0.0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fossiler
-Version: 0.0.4.4
+Version: 0.0.4.5
 Summary: Python package and CLI for finding available fossils
 Home-page: http://github.com/heche-psb/fossiler
 Author: Hengchi Chen
 Author-email: heche@psb.vib-ugent.be
 License: GPL
 Description: <div align="center">
```

### Comparing `fossiler-0.0.4.4/README.md` & `fossiler-0.0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `fossiler-0.0.4.4/command.py` & `fossiler-0.0.4.5/command.py`

 * *Files identical despite different names*

### Comparing `fossiler-0.0.4.4/fossiler/fossils.py` & `fossiler-0.0.4.5/fossiler/fossils.py`

 * *Files 1% similar despite different names*

```diff
@@ -241,22 +241,30 @@
         if i.endswith("_ap1") or i.endswith("_ap2"): continue
         #added_num = len(Orders_replace_Species[i].split(',')) - 1
         #final_sp_num = original_sp_num + added_num
         content = content.replace(i,Orders_replace_Species[i])
     handle = StringIO(content.split("\n")[1])
     Tree = Phylo.read(handle,"newick")
     spnum = len(Tree.get_terminals())
-    with open("sp{}_species_list".format(spnum),"w") as f:
+    with open("sp{}_species_list_space".format(spnum),"w") as f:
         focussp = ''
         for i in Tree.get_terminals():
             if i.name.endswith("_ap2") or i.name.endswith("_ap1"):
                 focussp = i.name[:-4]
                 continue
             f.write("{} ".format(i.name))
-        f.write("{} ".format(focussp))
+        f.write("{}".format(focussp))
+    with open("sp{}_species_list_lines".format(spnum),"w") as f:
+        focussp = ''
+        for i in Tree.get_terminals():
+            if i.name.endswith("_ap2") or i.name.endswith("_ap1"):
+                focussp = i.name[:-4]
+                continue
+            f.write("{}\n".format(i.name))
+        f.write("{}".format(focussp))
     content = content.replace(str(original_sp_num)+" ",str(spnum)+" ")
     return content, spnum
 
 def getproperstartingtree(treef,number,outdir):
     # Only works for order-level/or more recent WGDs
     Tree = Phylo.read(treef,"newick")
     Clade_names = [i.name for i in Tree.get_terminals()]
```

### Comparing `fossiler-0.0.4.4/fossiler.egg-info/PKG-INFO` & `fossiler-0.0.4.5/fossiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fossiler
-Version: 0.0.4.4
+Version: 0.0.4.5
 Summary: Python package and CLI for finding available fossils
 Home-page: http://github.com/heche-psb/fossiler
 Author: Hengchi Chen
 Author-email: heche@psb.vib-ugent.be
 License: GPL
 Description: <div align="center">
```

### Comparing `fossiler-0.0.4.4/setup.py` & `fossiler-0.0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='fossiler',
-    version='0.0.4.4',
+    version='0.0.4.5',
     packages=['fossiler'],
     url='http://github.com/heche-psb/fossiler',
     license='GPL',
     author='Hengchi Chen',
     author_email='heche@psb.vib-ugent.be',
     description='Python package and CLI for finding available fossils',
     long_description=long_description,
```

