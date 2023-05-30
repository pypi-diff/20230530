# Comparing `tmp/fossiler-0.0.4.tar.gz` & `tmp/fossiler-0.0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fossiler-0.0.4.tar", last modified: Mon May 29 21:34:05 2023, max compression
+gzip compressed data, was "dist/fossiler-0.0.4.2.tar", last modified: Tue May 30 05:04:39 2023, max compression
```

## Comparing `fossiler-0.0.4.tar` & `fossiler-0.0.4.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-29 21:34:05.641070 fossiler-0.0.4/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    35149 2023-05-11 08:47:25.000000 fossiler-0.0.4/LICENSE
--rwxrwxrwx   0 heche     (1000) heche     (1000)    84885 2023-05-29 21:34:05.642065 fossiler-0.0.4/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)    77524 2023-05-29 21:33:20.000000 fossiler-0.0.4/README.md
--rwxrwxrwx   0 heche     (1000) heche     (1000)     2663 2023-05-29 21:11:35.000000 fossiler-0.0.4/command.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-29 21:34:05.634860 fossiler-0.0.4/fossiler/
--rwxrwxrwx   0 heche     (1000) heche     (1000)   145646 2023-05-29 21:31:01.000000 fossiler-0.0.4/fossiler/fossils.py
-drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-29 21:34:05.640067 fossiler-0.0.4/fossiler.egg-info/
--rwxrwxrwx   0 heche     (1000) heche     (1000)    84885 2023-05-29 21:34:05.000000 fossiler-0.0.4/fossiler.egg-info/PKG-INFO
--rwxrwxrwx   0 heche     (1000) heche     (1000)      261 2023-05-29 21:34:05.000000 fossiler-0.0.4/fossiler.egg-info/SOURCES.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-05-29 21:34:05.000000 fossiler-0.0.4/fossiler.egg-info/dependency_links.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)       60 2023-05-29 21:34:05.000000 fossiler-0.0.4/fossiler.egg-info/entry_points.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)       56 2023-05-29 21:34:05.000000 fossiler-0.0.4/fossiler.egg-info/requires.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)       17 2023-05-29 21:34:05.000000 fossiler-0.0.4/fossiler.egg-info/top_level.txt
--rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-05-29 21:34:05.643083 fossiler-0.0.4/setup.cfg
--rwxrwxrwx   0 heche     (1000) heche     (1000)      801 2023-05-29 21:33:09.000000 fossiler-0.0.4/setup.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-30 05:04:39.869857 fossiler-0.0.4.2/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    35149 2023-05-11 08:47:25.000000 fossiler-0.0.4.2/LICENSE
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    84889 2023-05-30 05:04:39.869857 fossiler-0.0.4.2/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    77526 2023-05-30 05:03:57.000000 fossiler-0.0.4.2/README.md
+-rwxrwxrwx   0 heche     (1000) heche     (1000)     2663 2023-05-29 21:11:35.000000 fossiler-0.0.4.2/command.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-30 05:04:39.869857 fossiler-0.0.4.2/fossiler/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)   145833 2023-05-30 05:00:39.000000 fossiler-0.0.4.2/fossiler/fossils.py
+drwxrwxrwx   0 heche     (1000) heche     (1000)        0 2023-05-30 05:04:39.869857 fossiler-0.0.4.2/fossiler.egg-info/
+-rwxrwxrwx   0 heche     (1000) heche     (1000)    84889 2023-05-30 05:04:39.000000 fossiler-0.0.4.2/fossiler.egg-info/PKG-INFO
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      261 2023-05-30 05:04:39.000000 fossiler-0.0.4.2/fossiler.egg-info/SOURCES.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)        1 2023-05-30 05:04:39.000000 fossiler-0.0.4.2/fossiler.egg-info/dependency_links.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)       60 2023-05-30 05:04:39.000000 fossiler-0.0.4.2/fossiler.egg-info/entry_points.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)       56 2023-05-30 05:04:39.000000 fossiler-0.0.4.2/fossiler.egg-info/requires.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)       17 2023-05-30 05:04:39.000000 fossiler-0.0.4.2/fossiler.egg-info/top_level.txt
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      103 2023-05-30 05:04:39.869857 fossiler-0.0.4.2/setup.cfg
+-rwxrwxrwx   0 heche     (1000) heche     (1000)      803 2023-05-30 05:03:42.000000 fossiler-0.0.4.2/setup.py
```

### Comparing `fossiler-0.0.4/LICENSE` & `fossiler-0.0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fossiler-0.0.4/PKG-INFO` & `fossiler-0.0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: fossiler
-Version: 0.0.4
+Version: 0.0.4.2
 Summary: Python package and CLI for finding available fossils
 Home-page: http://github.com/heche-psb/fossiler
 Author: Hengchi Chen
 Author-email: heche@psb.vib-ugent.be
 License: GPL
 Description: <div align="center">
         
-        # `fossiler v0.0.4` : a suite tool of fossils finding
+        # `fossiler v0.0.4.2` : a suite tool of fossils finding
         **Hengchi Chen**
         
         [**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/people/heche)**, VIB-UGent Center for Plant Systems Biology**
         
         [**Upper Limits**](#Upper-Limits) |
         [**Fossil Justifications**](#Fossil-Justifications) |
         [**References**](#References)
```

### Comparing `fossiler-0.0.4/README.md` & `fossiler-0.0.4.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 <div align="center">
 
-# `fossiler v0.0.4` : a suite tool of fossils finding
+# `fossiler v0.0.4.2` : a suite tool of fossils finding
 **Hengchi Chen**
 
 [**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/people/heche)**, VIB-UGent Center for Plant Systems Biology**
 
 [**Upper Limits**](#Upper-Limits) |
 [**Fossil Justifications**](#Fossil-Justifications) |
 [**References**](#References)
```

### Comparing `fossiler-0.0.4/command.py` & `fossiler-0.0.4.2/command.py`

 * *Files identical despite different names*

### Comparing `fossiler-0.0.4/fossiler/fossils.py` & `fossiler-0.0.4.2/fossiler/fossils.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,23 +241,26 @@
         if i.endswith("_ap1") or i.endswith("_ap2"): continue
         #added_num = len(Orders_replace_Species[i].split(',')) - 1
         #final_sp_num = original_sp_num + added_num
         content = content.replace(i,Orders_replace_Species[i])
     handle = StringIO(content.split("\n")[1])
     Tree = Phylo.read(handle,"newick")
     spnum = len(Tree.get_terminals())
+    with open("sp{}_species_list".format(spnum),"w") as f:
+        for i in Tree.get_terminals(): f.write("{}\n".format(i.name))
     content = content.replace(str(original_sp_num)+" ",str(spnum)+" ")
-    return content
+    return content, spnum
 
 def getproperstartingtree(treef,number,outdir):
     # Only works for order-level/or more recent WGDs
     Tree = Phylo.read(treef,"newick")
     Clade_names = [i.name for i in Tree.get_terminals()]
     with open(treef,"r") as f: content = f.read()
-    with open(treef,"w") as f: f.write(replacespecies(content,Clade_names))
+    content, spnum = replacespecies(content,Clade_names)
+    with open(treef+'_{}sp'.format(spnum),"w") as f: f.write(content)
 
 def otherpaperestimate(data):
     maximum_other_paper = {'eudicots':0}
 
 def reshuffleMSA(fn_msa):
     msa = AlignIO.read(fn_msa,"fasta")
     # first select a random species
```

### Comparing `fossiler-0.0.4/fossiler.egg-info/PKG-INFO` & `fossiler-0.0.4.2/fossiler.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: fossiler
-Version: 0.0.4
+Version: 0.0.4.2
 Summary: Python package and CLI for finding available fossils
 Home-page: http://github.com/heche-psb/fossiler
 Author: Hengchi Chen
 Author-email: heche@psb.vib-ugent.be
 License: GPL
 Description: <div align="center">
         
-        # `fossiler v0.0.4` : a suite tool of fossils finding
+        # `fossiler v0.0.4.2` : a suite tool of fossils finding
         **Hengchi Chen**
         
         [**Bioinformatics & Evolutionary Genomics Group**](https://www.vandepeerlab.org/people/heche)**, VIB-UGent Center for Plant Systems Biology**
         
         [**Upper Limits**](#Upper-Limits) |
         [**Fossil Justifications**](#Fossil-Justifications) |
         [**References**](#References)
```

### Comparing `fossiler-0.0.4/setup.py` & `fossiler-0.0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='fossiler',
-    version='0.0.4',
+    version='0.0.4.2',
     packages=['fossiler'],
     url='http://github.com/heche-psb/fossiler',
     license='GPL',
     author='Hengchi Chen',
     author_email='heche@psb.vib-ugent.be',
     description='Python package and CLI for finding available fossils',
     long_description=long_description,
```

