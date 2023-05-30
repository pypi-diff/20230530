# Comparing `tmp/modelfree-protein15n-0.0.5.tar.gz` & `tmp/modelfree-protein15n-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelfree-protein15n-0.0.5.tar", last modified: Wed May 17 21:12:43 2023, max compression
+gzip compressed data, was "modelfree-protein15n-0.0.6.tar", last modified: Sun May 28 16:06:51 2023, max compression
```

## Comparing `modelfree-protein15n-0.0.5.tar` & `modelfree-protein15n-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,27 @@
-drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-17 21:12:43.497717 modelfree-protein15n-0.0.5/
--rwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)     1066 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/LICENSE
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       15 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/MANIFEST.in
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3599 2023-05-17 21:12:43.494481 modelfree-protein15n-0.0.5/PKG-INFO
--rwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)     2698 2023-05-17 21:05:22.000000 modelfree-protein15n-0.0.5/README.md
-drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-17 21:12:43.460197 modelfree-protein15n-0.0.5/modelfree_protein15n.egg-info/
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3599 2023-05-17 21:12:43.000000 modelfree-protein15n-0.0.5/modelfree_protein15n.egg-info/PKG-INFO
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)      573 2023-05-17 21:12:43.000000 modelfree-protein15n-0.0.5/modelfree_protein15n.egg-info/SOURCES.txt
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        1 2023-05-17 21:12:43.000000 modelfree-protein15n-0.0.5/modelfree_protein15n.egg-info/dependency_links.txt
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       50 2023-05-17 21:12:43.000000 modelfree-protein15n-0.0.5/modelfree_protein15n.egg-info/entry_points.txt
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       48 2023-05-17 21:12:43.000000 modelfree-protein15n-0.0.5/modelfree_protein15n.egg-info/requires.txt
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        8 2023-05-17 21:12:43.000000 modelfree-protein15n-0.0.5/modelfree_protein15n.egg-info/top_level.txt
-drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-17 21:12:43.489258 modelfree-protein15n-0.0.5/modfree/
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/modfree/__init__.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       71 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/modfree/__main__.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1736 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/modfree/analysis.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)      719 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/modfree/constants_functions.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     8708 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/modfree/data_format.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     6555 2023-05-17 20:50:18.000000 modelfree-protein15n-0.0.5/modfree/generator.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     2327 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/modfree/inputs.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)    14130 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/modfree/mf_standard.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     5837 2023-05-17 21:04:33.000000 modelfree-protein15n-0.0.5/modfree/modfree.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3675 2023-05-17 19:59:19.000000 modelfree-protein15n-0.0.5/modfree/outputs.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     2481 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/modfree/parser.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     4488 2023-05-17 20:40:18.000000 modelfree-protein15n-0.0.5/modfree/ploter.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3389 2023-05-17 21:03:40.000000 modelfree-protein15n-0.0.5/modfree/run_fit.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       38 2023-05-17 21:12:43.497717 modelfree-protein15n-0.0.5/setup.cfg
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1094 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.5/setup.py
+drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-28 16:06:51.665835 modelfree-protein15n-0.0.6/
+-rwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)     1066 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.6/LICENSE
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       15 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.6/MANIFEST.in
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3599 2023-05-28 16:06:51.665835 modelfree-protein15n-0.0.6/PKG-INFO
+-rwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)     2698 2023-05-17 21:05:22.000000 modelfree-protein15n-0.0.6/README.md
+drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-28 16:06:51.639547 modelfree-protein15n-0.0.6/modelfree_protein15n.egg-info/
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3599 2023-05-28 16:06:51.000000 modelfree-protein15n-0.0.6/modelfree_protein15n.egg-info/PKG-INFO
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)      546 2023-05-28 16:06:51.000000 modelfree-protein15n-0.0.6/modelfree_protein15n.egg-info/SOURCES.txt
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        1 2023-05-28 16:06:51.000000 modelfree-protein15n-0.0.6/modelfree_protein15n.egg-info/dependency_links.txt
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       50 2023-05-28 16:06:51.000000 modelfree-protein15n-0.0.6/modelfree_protein15n.egg-info/entry_points.txt
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       48 2023-05-28 16:06:51.000000 modelfree-protein15n-0.0.6/modelfree_protein15n.egg-info/requires.txt
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        8 2023-05-28 16:06:51.000000 modelfree-protein15n-0.0.6/modelfree_protein15n.egg-info/top_level.txt
+drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-28 16:06:51.661398 modelfree-protein15n-0.0.6/modfree/
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.6/modfree/__init__.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       71 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.6/modfree/__main__.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1372 2023-05-28 15:54:27.000000 modelfree-protein15n-0.0.6/modfree/analysis.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)      699 2023-05-28 15:39:24.000000 modelfree-protein15n-0.0.6/modfree/constants_functions.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     8708 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.6/modfree/data_format.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     6438 2023-05-28 15:44:13.000000 modelfree-protein15n-0.0.6/modfree/generator.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1901 2023-05-28 15:34:09.000000 modelfree-protein15n-0.0.6/modfree/inputs.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)    14226 2023-05-28 15:39:13.000000 modelfree-protein15n-0.0.6/modfree/mf.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     5613 2023-05-28 15:53:09.000000 modelfree-protein15n-0.0.6/modfree/modfree.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3538 2023-05-28 15:30:20.000000 modelfree-protein15n-0.0.6/modfree/outputs.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     4472 2023-05-28 15:30:09.000000 modelfree-protein15n-0.0.6/modfree/ploter.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     2961 2023-05-28 15:43:26.000000 modelfree-protein15n-0.0.6/modfree/run_fit.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       38 2023-05-28 16:06:51.665835 modelfree-protein15n-0.0.6/setup.cfg
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1094 2023-05-17 13:06:07.000000 modelfree-protein15n-0.0.6/setup.py
```

### Comparing `modelfree-protein15n-0.0.5/LICENSE` & `modelfree-protein15n-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.5/PKG-INFO` & `modelfree-protein15n-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: modelfree-protein15n
-Version: 0.0.5
+Version: 0.0.6
 Summary: Model free analysis of protein backbone amide 15N spin relaxation rates.
 Home-page: https://github.com/VSchnapka/modelfree-protein15n.git
 Author: Vincent Schnapka
 Author-email: vincentschnapka@gmail.com
 License: UNKNOWN
 Description: # modelfree-protein15n
         Model-Free analysis framework for protein backbone amide 15N NMR spin relaxation rates.
```

### Comparing `modelfree-protein15n-0.0.5/README.md` & `modelfree-protein15n-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.5/modelfree_protein15n.egg-info/PKG-INFO` & `modelfree-protein15n-0.0.6/modelfree_protein15n.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: modelfree-protein15n
-Version: 0.0.5
+Version: 0.0.6
 Summary: Model free analysis of protein backbone amide 15N spin relaxation rates.
 Home-page: https://github.com/VSchnapka/modelfree-protein15n.git
 Author: Vincent Schnapka
 Author-email: vincentschnapka@gmail.com
 License: UNKNOWN
 Description: # modelfree-protein15n
         Model-Free analysis framework for protein backbone amide 15N NMR spin relaxation rates.
```

### Comparing `modelfree-protein15n-0.0.5/modelfree_protein15n.egg-info/SOURCES.txt` & `modelfree-protein15n-0.0.6/modelfree_protein15n.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,13 +11,12 @@
 modfree/__init__.py
 modfree/__main__.py
 modfree/analysis.py
 modfree/constants_functions.py
 modfree/data_format.py
 modfree/generator.py
 modfree/inputs.py
-modfree/mf_standard.py
+modfree/mf.py
 modfree/modfree.py
 modfree/outputs.py
-modfree/parser.py
 modfree/ploter.py
 modfree/run_fit.py
```

### Comparing `modelfree-protein15n-0.0.5/modfree/constants_functions.py` & `modelfree-protein15n-0.0.6/modfree/constants_functions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # file containing the used constants and useful functions:
 import numpy as np
 
-theta = 22 # angle between CSA and dd axis
+# By default, theta = 22 # angle between CSA and dd axis
 
 gamma15N = -2.7126 * 1e7 # rad s-1 T-1
 gamma1H = 2.6752219 * 1e8 # rad s-1 T-1
 rNH = 1.015 * 1e-10 # 1.023e-10 is Average NH bond length cf Yao et al JACS 2008, in m
 tCSA = -172.0 * 1e-6 # CSA cf Kroenke et al JACS 1999
 mu_0 = 1.2566370614359173 * 1e-6 # vacuum permeability
 h = 6.62607004e-34 # Planck constant
 R = 8.31446261815324 # J.mol-1.K-1
 
 d = mu_0*h*gamma1H*gamma15N/(8*(np.pi**2)*(rNH**3)) # NH dipolar coupling constant
-theta = theta*np.pi/180 # in rad.
 
 
 # Legendre 2
 def P2(x):
     return (3*x*x - 1)/2
```

### Comparing `modelfree-protein15n-0.0.5/modfree/data_format.py` & `modelfree-protein15n-0.0.6/modfree/data_format.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.5/modfree/generator.py` & `modelfree-protein15n-0.0.6/modfree/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import glob
 import re
 import random as rd
 import numpy as np
 import modfree.data_format as df
 import modfree.outputs as outputs
-from modfree.mf_standard import give_params, calc_rates
+from modfree.mf import give_params, calc_rates
 
 
 def random_amp1(length):
     output = [rd.uniform(0, 1)]
     for i in range(1, length):
         idx, dat = 0, 1000
         while (dat > 0.4 or dat < 0) and idx < 10000:
@@ -90,32 +90,31 @@
         idx, dat = 0, 1000
         while (dat > 20e-9 or dat < 2e-9) and idx < 10000:
             dat = rd.gauss(output[0], 0.4e-9)
         output.append(dat)
     return output
 
 
-def generate_directories_file_std(directory_with_the_directories):
+def generate_directories_file(directory_with_the_directories):
     current_path = os.path.abspath(".")
     dirs = glob.glob(directory_with_the_directories+"/*/")
     with open(directory_with_the_directories+"/directories.toml", "w") as f:
         for d in dirs:
             field = re.findall("\d+", re.findall("\d+MHz", d, re.IGNORECASE)[0])[0]
             f.write(f"[generated-{field}]\n")
             f.write(f"directory = \"{current_path}/{d}\"\n")
             f.write(f"magnetic_field_MHz = {field}\n")
             f.write("\n")
             
             
-def generate_parameter_file_std(directory_with_the_directories, fields, modes=2):
+def generate_parameter_file(directory_with_the_directories, fields, modes=2):
     with open(directory_with_the_directories+"/parameters.toml", "w") as f:
-        f.write("# model free analysis parameter file. model choice: standard only so far\n")
+        f.write("# model free analysis parameter file.\n")
         f.write(f"modes = {modes}\n")
         f.write(f"residues = \"all\"\n\n")
-        f.write(f"# model dependent input parameters\n")
         f.write(f"magnetic_fields_MHz = {fields}\n\n")
         f.write(f"# parameters to fix: (taux, ampx, (x an integer that has to be compatible with the number of dynamic modes. Starts from 1.))\n")
         f.write(f"#tau1 = 50e-12\n\n")
         f.write(f"# minimization parameters\n")
         f.write(f"mf_minimization_iterations = 3\n")
         f.write(f"monte_carlo_iterations = 50\n")
         f.write(f"monte_carlo_minimization_iterations = 3\n")
@@ -167,13 +166,13 @@
             os.mkdir(output_dir+"/"+str(int(f))+"MHz")
         for e in RATES[f].keys():
             x = RES
             y = [RATES[f][e][r] for r in x]
             dy = [ERROR[f][e][r] for r in x]
             outputs.save_param(x, y, dy=dy, outputname=output_dir+"/"+str(int(f))+"MHz/generated_"+str(e)+".txt")
     print("Data directory input generation...")
-    generate_directories_file_std(output_dir)
-    generate_parameter_file_std(output_dir, list(RATES.keys()), modes=modes)
+    generate_directories_file(output_dir)
+    generate_parameter_file(output_dir, list(RATES.keys()), modes=modes)
 
 
 if __name__ == "__main__":
     print("data generator module")
```

### Comparing `modelfree-protein15n-0.0.5/modfree/inputs.py` & `modelfree-protein15n-0.0.6/modfree/inputs.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,47 +9,39 @@
         dat = [el.rstrip("\n").split() for el in f.readlines()]
     x = [int(el[0]) for el in dat]
     y = [float(el[1]) for el in dat]
     dy = [float(el[2]) for el in dat]
     return x, y, dy
 
 
-def read_directory_file(filename="directories.toml", model="std"):
+def read_directory_file(filename="directories.toml"):
     rates = "R1", "R2", "NOE", "etaXY", "etaZ"
-    if model != "std":
-        print("in read directory file function: models other than std not yet implemented")
-        return None
-    if model == "std":
-        with open(filename, "rb") as f:
-            toml_dict = tomli.load(f)
-        dirs = dict()
-        for k in toml_dict.keys():
-            files = glob.glob(toml_dict[k]['directory']+"/*")
-            for f in files:
-                rate = re.findall('r1|r2|noe|etaxy|etaz', f, re.IGNORECASE)
-                rate = '' if rate == [] else rate[0]
-                for e in rates:
-                    match = re.search(rate, e, re.IGNORECASE)
-                    if match and match.group(0) != '':
-                        if toml_dict[k]['magnetic_field_MHz'] not in dirs.keys():
-                            dirs[toml_dict[k]['magnetic_field_MHz']] = dict()
-                        dirs[toml_dict[k]['magnetic_field_MHz']][e] = f
+    with open(filename, "rb") as f:
+        toml_dict = tomli.load(f)
+    dirs = dict()
+    for k in toml_dict.keys():
+        files = glob.glob(toml_dict[k]['directory']+"/*")
+        for f in files:
+            rate = re.findall('r1|r2|noe|etaxy|etaz', f, re.IGNORECASE)
+            rate = '' if rate == [] else rate[0]
+            for e in rates:
+                match = re.search(rate, e, re.IGNORECASE)
+                if match and match.group(0) != '':
+                    if toml_dict[k]['magnetic_field_MHz'] not in dirs.keys():
+                        dirs[toml_dict[k]['magnetic_field_MHz']] = dict()
+                    dirs[toml_dict[k]['magnetic_field_MHz']][e] = f
     return dirs
 
 
-def read_parameter_file(param_file, model="std"):
-    if model != "std":
-        print("in read directory file function: models other than std not yet implemented")
-        return None
-    if model == "std":
-        with open(param_file, "rb") as f:
-            toml_dict = tomli.load(f)
-        parameters = {"modes": toml_dict["modes"], "mf_minimization_iterations": toml_dict["mf_minimization_iterations"], "monte_carlo_iterations": toml_dict["monte_carlo_iterations"],
-                      "monte_carlo_minimization_iterations": toml_dict["monte_carlo_minimization_iterations"],
-                      "magnetic_fields_MHz": toml_dict["magnetic_fields_MHz"], "residues": toml_dict["residues"]}
-        fix_regex_pattern = "tau\d+|amp\d+"
-        parameters["fix"] = {k: val for k, val in toml_dict.items() if k not in parameters.keys() and re.match(fix_regex_pattern, k)}
+def read_parameter_file(param_file):
+    with open(param_file, "rb") as f:
+        toml_dict = tomli.load(f)
+    parameters = {"modes": toml_dict["modes"], "mf_minimization_iterations": toml_dict["mf_minimization_iterations"], "monte_carlo_iterations": toml_dict["monte_carlo_iterations"],
+                  "monte_carlo_minimization_iterations": toml_dict["monte_carlo_minimization_iterations"],
+                  "magnetic_fields_MHz": toml_dict["magnetic_fields_MHz"], "residues": toml_dict["residues"]}
+    fix_regex_pattern = "tau\d+|amp\d+"
+    parameters["fix"] = {k: val for k, val in toml_dict.items() if k not in parameters.keys() and re.match(fix_regex_pattern, k)}
     return parameters
 
 
 if __name__ == "__main__":
     print(read_parameter_file("parameters.txt"))
```

### Comparing `modelfree-protein15n-0.0.5/modfree/mf_standard.py` & `modelfree-protein15n-0.0.6/modfree/mf.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,27 +54,29 @@
     omegaN = gamma15N * field
     omegaH = gamma1H * field
     omega_sum = omegaH + omegaN
     omega_diff = omegaH - omegaN
     return 1.0 + (d**2)/(10*R1(x, amps, taus)) * (gamma1H/gamma15N)*(6*J(omega_sum)-J(omega_diff))
 
 
-def etaXY(x, amps, taus):
+def etaXY(x, amps, taus, theta=22):
     def J(omega): return j(omega, amps, taus)
+    theta = theta*np.pi/180 # in rad.
     field = x * 1e6 / (gamma1H/(2*np.pi))
     omegaN = gamma15N * field
     omegaH = gamma1H * field
     omega_sum = omegaH + omegaN
     omega_diff = omegaH - omegaN
     c = tCSA * omegaN
     return -(1/15)*d*c*P2(np.cos(theta))*(3*J(omegaN) + 4*J(0))
 
 
-def etaZ(x, amps, taus):
+def etaZ(x, amps, taus, theta=22):
     def J(omega): return j(omega, amps, taus)
+    theta = theta*np.pi/180 # in rad.
     field = x * 1e6 / (gamma1H/(2*np.pi))
     omegaN = gamma15N * field
     omegaH = gamma1H * field
     omega_sum = omegaH + omegaN
     omega_diff = omegaH - omegaN
     c = tCSA * omegaN
     return -(1/15)*d*c*P2(np.cos(theta))*6*J(omegaN)
```

### Comparing `modelfree-protein15n-0.0.5/modfree/modfree.py` & `modelfree-protein15n-0.0.6/modfree/modfree.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import modfree.inputs as inputs
 import modfree.outputs as outputs
 import modfree.run_fit as run_fit
 import modfree.ploter as ploter
 import modfree.generator as generator
 
 
-__version__ = "0.0.5"
+__version__ = "0.0.6"
 
 
 console = Console()
 
 
 header = "\n".join(
 [
@@ -41,34 +41,34 @@
     console.print(panel)
 
 
 def plot(args: Namespace):
     data_file = args.o
     what_to_plot = args.p
     if what_to_plot == "relaxation" or what_to_plot == "all":
-        ploter.plot_rates_std(output_dir=data_file, file_format=args.format, dpi=args.dpi)
+        ploter.plot_rates(output_dir=data_file, file_format=args.format, dpi=args.dpi)
     if what_to_plot == "parameters" or what_to_plot == "all":
-        ploter.plot_params_std(output_dir=data_file, plotname="parameters."+str(args.format), file_format=args.format, dpi=args.dpi)
+        ploter.plot_params(output_dir=data_file, plotname="parameters."+str(args.format), file_format=args.format, dpi=args.dpi)
     if what_to_plot == "statistics" or what_to_plot == "all":
-        ploter.plot_statistics_std(output_dir=data_file, plotname="statistics."+str(args.format), file_format=args.format, dpi=args.dpi)
+        ploter.plot_statistics(output_dir=data_file, plotname="statistics."+str(args.format), file_format=args.format, dpi=args.dpi)
     if what_to_plot == "correlation" or what_to_plot == "all":
-        ploter.plot_rates_corr_std(output_dir=data_file, plotname="correlation."+str(args.format), file_format=args.format, dpi=args.dpi)
+        ploter.plot_rates_corr(output_dir=data_file, plotname="correlation."+str(args.format), file_format=args.format, dpi=args.dpi)
 
 
 def fit(args: Namespace):
-    data_files = inputs.read_directory_file(args.d, args.m)
-    input_parameters = inputs.read_parameter_file(args.p, args.m)
-    result = run_fit.launch_fits(input_parameters, args.r, data_files, model=args.m)
+    data_files = inputs.read_directory_file(args.d)
+    input_parameters = inputs.read_parameter_file(args.p)
+    result = run_fit.launch_fits(input_parameters, args.r, data_files)
     outputs.save_params(result, directory=args.o)
     df.Save(result, args.o+"/rawoutput.txt")
     if args.plot:
-        ploter.plot_params_std(output_dir=data_file, plotname="parameters."+str(args.format), file_format=args.format, dpi=args.dpi)
-        ploter.plot_statistics_std(output_dir=data_file, plotname="statistics."+str(args.format), file_format=args.format, dpi=args.dpi)
-        ploter.plot_rates_corr_std(output_dir=data_file, plotname="correlation."+str(args.format), file_format=args.format, dpi=args.dpi)
-        ploter.plot_rates_std(output_dir=data_file, file_format=args.format, dpi=args.dpi)
+        ploter.plot_params(output_dir=data_file, plotname="parameters."+str(args.format), file_format=args.format, dpi=args.dpi)
+        ploter.plot_statistics(output_dir=data_file, plotname="statistics."+str(args.format), file_format=args.format, dpi=args.dpi)
+        ploter.plot_rates_corr(output_dir=data_file, plotname="correlation."+str(args.format), file_format=args.format, dpi=args.dpi)
+        ploter.plot_rates(output_dir=data_file, file_format=args.format, dpi=args.dpi)
 
 
 def generate(args: Namespace):
     generator.generate(args.n, args.o, fields=args.fields, rates=args.rates, modes=args.modes, noise_proportion=args.noise)
 
 
 def build_parser():
@@ -78,15 +78,14 @@
 
     fit_parser = subparsers.add_parser("fit", help="Fit the data")
     fit_parser.set_defaults(func=fit)
     fit_parser.add_argument('-o', type=str, help="output directory", default="Outputs")
     fit_parser.add_argument('-d', type=str, help="directory file. toml file. contains the directories and the corresponding conditions", default="directories.toml")
     fit_parser.add_argument('-p', type=str, help="parameter file. toml file", default="params.toml")
     fit_parser.add_argument('-r', type=int, nargs="+", help="Residue(s) to analyse. By default, the program reads the parameter file.", default=0)
-    fit_parser.add_argument('-m', type=str, help="fitting model: standard (std), arrhenius (arrh), viscosity (visc), arrhenius-viscosity (arvi).", default="std")
     fit_parser.add_argument('-plot', type=bool, help="plot the output", default=False)
     
     plot_parser = subparsers.add_parser("plot", help="Plot the data")
     plot_parser.set_defaults(func=plot)
     plot_parser.add_argument('-o', type=str, help="output directory", default="Outputs")
     plot_parser.add_argument('-p', type=str, help="what to plot: all, relaxation, parameters, statistics, correlation", default="all")
     plot_parser.add_argument('-format', type=str, help="file format: pdf, jpg, png, svg", default="pdf")
```

### Comparing `modelfree-protein15n-0.0.5/modfree/outputs.py` & `modelfree-protein15n-0.0.6/modfree/outputs.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,19 +12,16 @@
             for i, res in enumerate(x):
                 f.write(str(res)+"  "+str(y[i])+"\n")
         else:
             for i, res in enumerate(x):
                 f.write(str(res)+"  "+str(y[i])+"  "+str(dy[i])+"\n")
 
 
-def save_params(result_dic, directory, model="std"):
+def save_params(result_dic, directory):
     #print(result_dic)
-    if model != "std":
-        print("other models not implemented so far in save_params")
-        return None
     if not os.path.isdir(directory):
         os.mkdir(directory)
     if directory[-1] != "/":
         directory = directory + "/"
     values = df.swap(result_dic, 1, 2)['values']
     #values = df.swap(values, 2, 3) # values[res][amps/taus][0,1,2,...]
     errors = df.swap(result_dic, 1, 2)['error']
@@ -41,15 +38,15 @@
             save_param(result_dic[res]['mc_taus'][i], outputname=directory+"Monte_Carlo/"+str(res)+"/mc_tau"+str(i+1)+".out")
             save_param(result_dic[res]['mc_amps'][i], outputname=directory+"Monte_Carlo/"+str(res)+"/mc_amp"+str(i+1)+".out")
     # experimental and back calculated relaxation rates
     if not os.path.isdir(directory+"Relaxation_Rates/"):
         os.mkdir(directory+"Relaxation_Rates/")
     rates = {"fit": dict(), "exp": dict(), "err": dict(), "fiterr": dict()}
     for res in X:
-        exp_rates, err_rates, fit_rates, fit_error = analysis.calc_rates_result(result_dic[res], model=model)
+        exp_rates, err_rates, fit_rates, fit_error = analysis.calc_rates_result(result_dic[res])
         rates["fit"][res] = fit_rates
         rates["fiterr"][res] = fit_error
         rates["exp"][res] = exp_rates
         rates["err"][res] = err_rates
         # rates[exp/fit][res][e][f]
     rates = df.swap(rates, 2, 4)
     for f in rates["exp"].keys():
```

### Comparing `modelfree-protein15n-0.0.5/modfree/ploter.py` & `modelfree-protein15n-0.0.6/modfree/ploter.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,36 +42,36 @@
     if log:
         ax.set_yscale("log")
     ax.set_xlabel("Sequence")
     ax.set_ylabel(filename.split("/")[-1].replace(".out", ""))
     ax.set_ylim(0.8*np.min(y), 1.2*np.max(y))
 
 
-def plot_params_std(output_dir, file_format="pdf", dpi=600):
+def plot_params(output_dir, file_format="pdf", dpi=600):
     check_output_dir(output_dir)
     param_files = glob.glob(output_dir+"/*.out")
     for el in param_files:
         log = True if re.search("tau", el) else False
         fig, ax = plt.subplots(1, 1, figsize=(8, 5))
         plot_param(el, ax=ax, log=log, color="darkblue")
         plt.savefig(output_dir+"/Plots/"+el.split("/")[-1].replace(".out", "."+file_format), format=file_format, dpi=dpi)
         plt.close()
     
 
-def plot_statistics_std(output_dir, plotname, file_format="pdf", dpi=600):
+def plot_statistics(output_dir, plotname, file_format="pdf", dpi=600):
     check_output_dir(output_dir)
     fig, ax = plt.subplots(3, 1, figsize=(8, 10))
     plot_param(output_dir+"/redchi2.out", color="darkblue", ax=ax[0], log=True)
     plot_param(output_dir+"/aic.out", color="darkblue", ax=ax[1])
     plot_param(output_dir+"/bic.out", color="darkblue", ax=ax[2])
     plt.savefig(output_dir+"/Plots/"+plotname, format=file_format, dpi=dpi)
     plt.close()
     
     
-def plot_rates_corr_std(output_dir, plotname, file_format="pdf", dpi=600):
+def plot_rates_corr(output_dir, plotname, file_format="pdf", dpi=600):
     check_output_dir(output_dir)
     rates_fit_dirs = sorted(glob.glob(output_dir+"/Relaxation_Rates/*.fit"))
     rates_exp_dirs = sorted(glob.glob(output_dir+"/Relaxation_Rates/*.exp"))
     fig, ax = plt.subplots(1, 1, figsize=(10, 10))
     for i, rdir in enumerate(rates_exp_dirs):
         x, y1, dy1 = read_relaxation_data_file(rates_exp_dirs[i])
         x, y2, dy2 = read_relaxation_data_file(rates_fit_dirs[i])
@@ -79,15 +79,15 @@
         ax.errorbar(y1, y2, xerr=dy1, yerr=dy2, color="darkblue", ls="", marker="o")
     ax.set_ylabel("Calculated relaxation rates")
     ax.set_xlabel("Experimental relaxation rates")
     plt.savefig(output_dir+"/Plots/"+plotname, format=file_format, dpi=dpi)
     plt.close()
 
 
-def plot_rates_std(output_dir, file_format="pdf", dpi=600):
+def plot_rates(output_dir, file_format="pdf", dpi=600):
     check_output_dir(output_dir)
     rates_fit_dirs = sorted(glob.glob(output_dir+"/Relaxation_Rates/*.fit"))
     rates_exp_dirs = sorted(glob.glob(output_dir+"/Relaxation_Rates/*.exp"))
     for i, rdir in enumerate(rates_exp_dirs):
         fig, ax = plt.subplots(1, 1, figsize=(10, 10))
         x1, y1, dy1 = read_relaxation_data_file(rates_exp_dirs[i])
         x2, y2, dy2 = read_relaxation_data_file(rates_fit_dirs[i])
```

### Comparing `modelfree-protein15n-0.0.5/modfree/run_fit.py` & `modelfree-protein15n-0.0.6/modfree/run_fit.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,72 +1,64 @@
 #!/usr/bin/env python
 import modfree.data_format as df
 import modfree.inputs as inputs
-import modfree.mf_standard as mf_standard
+import modfree.mf as mf
 
 
-def format_data(input_parameters_dic, directories, model="std"):
-    # format the data for the mf programm corresponding to the specified model.
+def format_data(input_parameters_dic, directories):
+    # format the data for the mf programm
     # outputs the data to fit and error to fit dictionnaries, in a metadictionnnary with all the residues.
-    if model == "std":
-        data = {f: {e: {x: y for (x,y,dy) in list(zip(*inputs.read_relaxation_data_file(directories[f][e])))} for e in directories[f].keys()} for f in directories.keys()}
-        error = {f: {e: {x: dy for (x,y,dy) in list(zip(*inputs.read_relaxation_data_file(directories[f][e])))} for e in directories[f].keys()} for f in directories.keys()}
-        data = df.swap(data, 1, 3)
-        error = df.swap(error, 1, 3)
-    else:
-        print("model not implemented yet in function run_fit.format_data")
-        return None
+    data = {f: {e: {x: y for (x,y,dy) in list(zip(*inputs.read_relaxation_data_file(directories[f][e])))} for e in directories[f].keys()} for f in directories.keys()}
+    error = {f: {e: {x: dy for (x,y,dy) in list(zip(*inputs.read_relaxation_data_file(directories[f][e])))} for e in directories[f].keys()} for f in directories.keys()}
+    data = df.swap(data, 1, 3)
+    error = df.swap(error, 1, 3)
     return data, error
 
 
-def run_fit(data, error, input_params, model="std"):
-    if model == "std":
-        return mf_standard.model_free(data, error, modes=input_params["modes"], mf_iterations=input_params["mf_minimization_iterations"], 
+def run_fit(data, error, input_params):
+    return mf.model_free(data, error, modes=input_params["modes"], mf_iterations=input_params["mf_minimization_iterations"], 
                                mc_iterations=input_params["monte_carlo_iterations"], mcmf_iterations=input_params["monte_carlo_minimization_iterations"],
                                **input_params["fix"])
-    else:
-        print("model not implemented in run_fit.run_fit")
-        return None
 
 
-def launch_fits(input_parameters_dic, residue, directories, model="std"):
-    data_dic, error_dic = format_data(input_parameters_dic, directories, model=model)
+def launch_fits(input_parameters_dic, residue, directories):
+    data_dic, error_dic = format_data(input_parameters_dic, directories)
     if residue == 0:
         residue = input_parameters_dic["residues"]
     if residue == "all":
         results = dict()
         for res in sorted(list(data_dic.keys())):
             print("\nresidue", res)
             try:
-                results[res] = run_fit(data_dic[res], error_dic[res], input_parameters_dic, model=model)
+                results[res] = run_fit(data_dic[res], error_dic[res], input_parameters_dic)
             except TypeError:
                 print("TypeError exception, there is probably not enough data for this residue.")
     elif type(residue) == list or type(residue) == tuple:
         results = dict()
         for res in sorted(residue):
             if res not in data_dic.keys():
                 print("\nresidue", res, "not in data")
                 continue
             print("\nresidue", res)
             try:
-                results[res] = run_fit(data_dic[res], error_dic[res], input_parameters_dic, model=model)
+                results[res] = run_fit(data_dic[res], error_dic[res], input_parameters_dic)
             except TypeError:
                 print("TypeError exception, there is probably not enough data for this residue.")
     else:
         residue = int(residue)
         print("\nresidue", residue)
         try:
-            results = {int(residue): run_fit(data_dic[int(residue)], error_dic[int(residue)], input_parameters_dic, model=model)}
+            results = {int(residue): run_fit(data_dic[int(residue)], error_dic[int(residue)], input_parameters_dic)}
         except ValueError:
             print("something is wrong with the residues settings in the parameter file")
             return None
         except KeyError:
             print("\nresidue", residue, "is not in the data")
             return None
         except TypeError:
             print("TypeError exception, there is probably not enough data for this residue.")
             return None
     return results
 
 
 if __name__ == "__main__":
-    print(format_data(inputs.read_parameter_file("parameters.txt"), "../../relaxation-data/dilute/", model="std"))
+    print(format_data(inputs.read_parameter_file("parameters.txt"), "../../relaxation-data/dilute/"))
```

### Comparing `modelfree-protein15n-0.0.5/setup.py` & `modelfree-protein15n-0.0.6/setup.py`

 * *Files identical despite different names*

