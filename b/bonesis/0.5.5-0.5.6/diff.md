# Comparing `tmp/bonesis-0.5.5.tar.gz` & `tmp/bonesis-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bonesis-0.5.5.tar", last modified: Thu Apr 27 20:53:00 2023, max compression
+gzip compressed data, was "bonesis-0.5.6.tar", last modified: Tue May 30 08:05:12 2023, max compression
```

## Comparing `bonesis-0.5.5.tar` & `bonesis-0.5.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:53:00.750640 bonesis-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-04-27 20:52:49.000000 bonesis-0.5.5/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    22961 2023-04-27 20:52:49.000000 bonesis-0.5.5/Licence_CeCILL_V2.1-fr.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-27 20:52:49.000000 bonesis-0.5.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-27 20:53:00.750640 bonesis-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-27 20:52:49.000000 bonesis-0.5.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:53:00.746640 bonesis-0.5.5/bonesis/
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/aeon.py
--rw-r--r--   0 runner    (1001) docker     (123)    28356 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/asp_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     8235 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/domains.py
--rw-r--r--   0 runner    (1001) docker     (123)    18123 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/language.py
--rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/reprogramming.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/snippets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:53:00.746640 bonesis-0.5.5/bonesis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-27 20:53:00.000000 bonesis-0.5.5/bonesis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-04-27 20:53:00.000000 bonesis-0.5.5/bonesis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 20:53:00.000000 bonesis-0.5.5/bonesis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-27 20:53:00.000000 bonesis-0.5.5/bonesis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-27 20:53:00.000000 bonesis-0.5.5/bonesis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-27 20:53:00.000000 bonesis-0.5.5/bonesis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 20:53:00.746640 bonesis-0.5.5/bonesis0/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis0/asp_encoding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis0/clingo_solving.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis0/diversity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis0/gil_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis0/proxy_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-27 20:52:49.000000 bonesis-0.5.5/bonesis0/subset_portfolio.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 20:53:00.750640 bonesis-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-04-27 20:52:49.000000 bonesis-0.5.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:05:12.459718 bonesis-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-05-30 08:04:55.000000 bonesis-0.5.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    22961 2023-05-30 08:04:55.000000 bonesis-0.5.6/Licence_CeCILL_V2.1-fr.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-30 08:04:55.000000 bonesis-0.5.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-30 08:05:12.459718 bonesis-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-05-30 08:04:55.000000 bonesis-0.5.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:05:12.455718 bonesis-0.5.6/bonesis/
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-05-30 08:04:55.000000 bonesis-0.5.6/bonesis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9489 2023-05-30 08:04:55.000000 bonesis-0.5.6/bonesis/aeon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27435 2023-05-30 08:04:55.000000 bonesis-0.5.6/bonesis/asp_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6297 2023-05-30 08:04:55.000000 bonesis-0.5.6/bonesis/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-30 08:04:55.000000 bonesis-0.5.6/bonesis/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-05-30 08:04:55.000000 bonesis-0.5.6/bonesis/domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18123 2023-05-30 08:04:55.000000 bonesis-0.5.6/bonesis/language.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-05-30 08:04:55.000000 bonesis-0.5.6/bonesis/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-30 08:04:55.000000 bonesis-0.5.6/bonesis/reprogramming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-30 08:04:55.000000 bonesis-0.5.6/bonesis/snippets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-05-30 08:04:55.000000 bonesis-0.5.6/bonesis/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17829 2023-05-30 08:04:55.000000 bonesis-0.5.6/bonesis/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:05:12.459718 bonesis-0.5.6/bonesis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-30 08:05:12.000000 bonesis-0.5.6/bonesis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-30 08:05:12.000000 bonesis-0.5.6/bonesis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 08:05:12.000000 bonesis-0.5.6/bonesis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-30 08:05:12.000000 bonesis-0.5.6/bonesis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 08:05:12.000000 bonesis-0.5.6/bonesis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-30 08:05:12.000000 bonesis-0.5.6/bonesis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 08:05:12.459718 bonesis-0.5.6/bonesis0/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 08:04:55.000000 bonesis-0.5.6/bonesis0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-30 08:04:55.000000 bonesis-0.5.6/bonesis0/asp_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-30 08:04:55.000000 bonesis-0.5.6/bonesis0/clingo_solving.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-05-30 08:04:55.000000 bonesis-0.5.6/bonesis0/diversity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-30 08:04:55.000000 bonesis-0.5.6/bonesis0/gil_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3664 2023-05-30 08:04:55.000000 bonesis-0.5.6/bonesis0/proxy_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-05-30 08:04:55.000000 bonesis-0.5.6/bonesis0/subset_portfolio.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 08:05:12.459718 bonesis-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-30 08:04:55.000000 bonesis-0.5.6/setup.py
```

### Comparing `bonesis-0.5.5/LICENSE.txt` & `bonesis-0.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.5/Licence_CeCILL_V2.1-fr.txt` & `bonesis-0.5.6/Licence_CeCILL_V2.1-fr.txt`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.5/README.md` & `bonesis-0.5.6/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -2,17 +2,24 @@
 
 Synthesis of Most Permissive Boolean Networks from network architecture and dynamical properties
 
 This software is distributed under the [CeCILL v2.1](http://www.cecill.info/index.en.html) free software license (GNU GPL compatible).
 
 ## Main related publications
 
+### Synthesis
+
 * **Synthesis of Boolean Networks from Biological Dynamical Constraints using Answer-Set Programming** (S Chevalier, C Froidevaux, L Paulevé, A Zinovyev). *In 2019 IEEE 31st International Conference on Tools with Artificial Intelligence (ICTAI), 34–41. Portland, Oregon, United States, 2019. IEEE.* [doi:10.1109/ICTAI.2019.00014](https://doi.org/10.1109/ICTAI.2019.00014)
 *  **Synthesis and Simulation of Ensembles of Boolean Networks for Cell Fate Decision** (S Chevalier, V Noël, L Calzone, A Zinovyev, L Paulevé) *In 18th International Conference on Computational Methods in Systems Biology (CMSB). Online, Germany, 2020.* Preprint at https://hal.archives-ouvertes.fr/hal-02898849/file/cmsb2020.pdf
 
+### Control
+
+* **Marker and source-marker reprogramming of Most Permissive Boolean networks and ensembles with BoNesis** (L Paulevé), *Peer Community Journal*, 2023
+[doi:10.24072/pcjournal.255](https://doi.org/10.24072/pcjournal.255)
+
 ## Installation
 
 ### Using pip
 ```
 pip install bonesis
 ```
```

### Comparing `bonesis-0.5.5/bonesis/__init__.py` & `bonesis-0.5.6/bonesis/__init__.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.5/bonesis/aeon.py` & `bonesis-0.5.6/bonesis/aeon.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.5/bonesis/asp_encoding.py` & `bonesis-0.5.6/bonesis/asp_encoding.py`

 * *Files 3% similar despite different names*

```diff
@@ -150,43 +150,14 @@
             return self.encode_domain_BooleanNetworksEnsemble(domain)
         if isinstance(domain, BooleanNetwork):
             return self.encode_domain_BooleanNetwork(domain)
         if isinstance(domain, InfluenceGraph):
             return self.encode_domain_InfluenceGraph(domain)
         raise TypeError(f"I don't know what to do with {type(domain)}")
 
-    def encode_BooleanFunction(self, n, f, ensure_dnf=True):
-        def clauses_of_dnf(f):
-            if f == self.ba.FALSE:
-                return [False]
-            if f == self.ba.TRUE:
-                return [True]
-            if isinstance(f, boolean.OR):
-                return f.args
-            else:
-                return [f]
-        def literals_of_clause(c):
-            def make_literal(l):
-                if isinstance(l, boolean.NOT):
-                    return (l.args[0].obj, -1)
-                else:
-                    return (l.obj, 1)
-            lits = c.args if isinstance(c, boolean.AND) else [c]
-            return map(make_literal, lits)
-        facts = []
-        if ensure_dnf:
-            f = self.ba.dnf(f).simplify()
-        for cid, c in enumerate(clauses_of_dnf(f)):
-            if isinstance(c, bool):
-                facts.append(clingo.Function("constant", symbols(n, s2v(c))))
-            else:
-                for m, v in literals_of_clause(c):
-                    facts.append(clingo.Function("clause", symbols(n, cid+1, m, v)))
-        return facts
-
     def encode_domain_BooleanNetworksEnsemble(self, bns):
         preds = set()
         facts = []
         for i, bn in enumerate(bns):
             bn_asp = self.encode_domain_BooleanNetwork(bn)
             facts.extend([f"bn_ensemble({i},{f})" for f in bn_asp])
             preds.update([(f.name, len(f.arguments)) for f in bn_asp])
@@ -195,20 +166,16 @@
             args = [f"A{i}" for i in range(arity)]
             p = f"{pname}({','.join(args)})"
             facts.append(f"{p} :- which_bn(BN), bn_ensemble(BN,{p})")
         return facts
 
     def encode_domain_BooleanNetwork(self, bn):
         self.ba = bn.ba
-        facts = []
-        facts.append(asp.Function("nbnode", symbols(len(bn))))
-        for n, f in bn.items():
-            facts.append(clingo.Function("node", symbols(n)))
-            facts += self.encode_BooleanFunction(n, f, ensure_dnf=False)
-        return facts
+        return [bn.asp_of_bn() + "\n" +
+                str(asp.Function("nbnode", symbols(len(bn))))]
 
     def encode_domain_InfluenceGraph(self, pkn):
         self.load_template_domain()
         if pkn.canonic:
             self.load_template_canonic()
         facts = pkn_to_facts(pkn, pkn.maxclause, pkn.allow_skipping_nodes)
         if pkn.exact:
@@ -269,14 +236,21 @@
         rules = [
             "eval(X,N,C,-1) :- clause(N,C,L,-V), mcfg(X,L,V), not clamped(X,N,_)",
             "eval(X,N,C,1) :- mcfg(X,L,V): clause(N,C,L,V); clause(N,C,_,_), mcfg(X,_,_), not clamped(X,N,_)",
             "eval(X,N,1) :- eval(X,N,C,1), clause(N,C,_,_)",
             "eval(X,N,-1) :- eval(X,N,C,-1): clause(N,C,_,_); clause(N,_,_,_), mcfg(X,_,_)",
             "eval(X,N,V) :- clamped(X,N,V)",
             "eval(X,N,V) :- constant(N,V), mcfg(X,_,_), not clamped(X,N,_)",
+
+            "eval(X,N,V) :- evalbdd(X,N,V), node(N), not clamped(X,N,_)",
+            "evalbdd(X,V,V) :- mcfg(X,_,_), V=(-1;1)",
+            "evalbdd(X,B,V) :- bdd(B,N,_,HI), mcfg(X,N,1), evalbdd(X,HI,V)",
+            "evalbdd(X,B,V) :- bdd(B,N,LO,_), mcfg(X,N,-1), evalbdd(X,LO,V)",
+            "evalbdd(X,B,V) :- mcfg(X,_,_), bdd(B,V)",
+
             "mcfg(X,N,V) :- ext(X,N,V)",
         ]
         self.push(rules)
 
     @unique_usage
     def load_template_cfg(self):
         rules = [
```

### Comparing `bonesis-0.5.5/bonesis/cli.py` & `bonesis-0.5.6/bonesis/cli.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.5/bonesis/debug.py` & `bonesis-0.5.6/bonesis/debug.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.5/bonesis/language.py` & `bonesis-0.5.6/bonesis/language.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.5/bonesis/manager.py` & `bonesis-0.5.6/bonesis/manager.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.5/bonesis/reprogramming.py` & `bonesis-0.5.6/bonesis/reprogramming.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.5/bonesis/snippets.py` & `bonesis-0.5.6/bonesis/snippets.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.5/bonesis/utils.py` & `bonesis-0.5.6/bonesis/utils.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.5/bonesis/views.py` & `bonesis-0.5.6/bonesis/views.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.5/bonesis.egg-info/SOURCES.txt` & `bonesis-0.5.6/bonesis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.5/bonesis0/asp_encoding.py` & `bonesis-0.5.6/bonesis0/asp_encoding.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.5/bonesis0/clingo_solving.py` & `bonesis-0.5.6/bonesis0/clingo_solving.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.5/bonesis0/diversity.py` & `bonesis-0.5.6/bonesis0/diversity.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.5/bonesis0/gil_utils.py` & `bonesis-0.5.6/bonesis0/gil_utils.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.5/bonesis0/proxy_control.py` & `bonesis-0.5.6/bonesis0/proxy_control.py`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.5/bonesis0/subset_portfolio.cfg` & `bonesis-0.5.6/bonesis0/subset_portfolio.cfg`

 * *Files identical despite different names*

### Comparing `bonesis-0.5.5/setup.py` & `bonesis-0.5.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 
 from setuptools import setup, find_packages
 
 NAME = 'bonesis'
-VERSION = '0.5.5'
+VERSION = '0.5.6'
 
 setup(name=NAME,
     version=VERSION,
     description = "Synthesis of Most Permissive Boolean Networks",
     license_files = ('LICENSE.txt', 'Licence_CeCILL_V2.1-fr.txt'),
     install_requires = [
         "boolean.py",
```

