# Comparing `tmp/mltlk-0.1.5.tar.gz` & `tmp/mltlk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mltlk-0.1.5.tar", last modified: Tue May 30 12:02:58 2023, max compression
+gzip compressed data, was "dist/mltlk-0.1.6.tar", last modified: Tue May 30 13:14:13 2023, max compression
```

## Comparing `mltlk-0.1.5.tar` & `mltlk-0.1.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 12:02:58.722649 mltlk-0.1.5/
--rw-r--r--   0 johanhagelback   (503) staff       (20)       93 2023-05-26 08:29:02.000000 mltlk-0.1.5/.gitignore
--rw-r--r--   0 johanhagelback   (503) staff       (20)     1073 2023-05-25 10:25:18.000000 mltlk-0.1.5/LICENSE
--rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-30 12:02:58.721975 mltlk-0.1.5/PKG-INFO
--rw-r--r--   0 johanhagelback   (503) staff       (20)      311 2023-05-26 08:20:29.000000 mltlk-0.1.5/README.md
--rw-r--r--   0 johanhagelback   (503) staff       (20)    31369 2023-05-30 11:10:44.000000 mltlk-0.1.5/Spiral.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    40302 2023-05-30 11:10:10.000000 mltlk-0.1.5/Weather.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    48621 2023-05-30 11:09:12.000000 mltlk-0.1.5/Wikipedia.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    33244 2023-05-30 12:01:38.000000 mltlk-0.1.5/Wikipedia_exploration.ipynb
--rw-r--r--   0 johanhagelback   (503) staff       (20)    50000 2023-05-30 11:12:17.000000 mltlk-0.1.5/Wikipedia_word2vec.ipynb
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 12:02:58.703185 mltlk-0.1.5/data/
--rw-r--r--   0 johanhagelback   (503) staff       (20)     4505 2021-03-10 11:22:51.000000 mltlk-0.1.5/data/spiral.csv
--rw-r--r--   0 johanhagelback   (503) staff       (20)      414 2023-05-26 08:09:41.000000 mltlk-0.1.5/data/weather.csv
--rw-r--r--   0 johanhagelback   (503) staff       (20)  2061699 2019-12-13 13:20:58.000000 mltlk-0.1.5/data/wikipedia_300.csv.gz
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 12:02:58.715117 mltlk-0.1.5/mltlk/
--rwxr-xr-x   0 johanhagelback   (503) staff       (20)      109 2023-05-30 12:01:12.000000 mltlk-0.1.5/mltlk/__init__.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     8137 2023-05-30 11:59:52.000000 mltlk-0.1.5/mltlk/exploration_textdata.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)    32219 2023-05-30 10:44:16.000000 mltlk-0.1.5/mltlk/ml.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     3324 2023-05-25 12:08:40.000000 mltlk-0.1.5/mltlk/resampling.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     2606 2023-05-30 07:25:34.000000 mltlk-0.1.5/mltlk/utils.py
--rw-r--r--   0 johanhagelback   (503) staff       (20)     4854 2023-05-29 08:24:02.000000 mltlk-0.1.5/mltlk/word2vec.py
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 12:02:58.719463 mltlk-0.1.5/mltlk.egg-info/
--rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-30 12:02:58.000000 mltlk-0.1.5/mltlk.egg-info/PKG-INFO
--rw-r--r--   0 johanhagelback   (503) staff       (20)      470 2023-05-30 12:02:58.000000 mltlk-0.1.5/mltlk.egg-info/SOURCES.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)        1 2023-05-30 12:02:58.000000 mltlk-0.1.5/mltlk.egg-info/dependency_links.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)       74 2023-05-30 12:02:58.000000 mltlk-0.1.5/mltlk.egg-info/requires.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)        6 2023-05-30 12:02:58.000000 mltlk-0.1.5/mltlk.egg-info/top_level.txt
--rw-r--r--   0 johanhagelback   (503) staff       (20)       38 2023-05-30 12:02:58.722836 mltlk-0.1.5/setup.cfg
--rw-r--r--   0 johanhagelback   (503) staff       (20)      361 2023-05-30 12:01:05.000000 mltlk-0.1.5/setup.py
-drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 12:02:58.720635 mltlk-0.1.5/stopwords/
--rw-r--r--   0 johanhagelback   (503) staff       (20)        5 2023-05-29 06:34:12.000000 mltlk-0.1.5/stopwords/custom.csv
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 13:14:13.217481 mltlk-0.1.6/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       93 2023-05-26 08:29:02.000000 mltlk-0.1.6/.gitignore
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     1073 2023-05-25 10:25:18.000000 mltlk-0.1.6/LICENSE
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-30 13:14:13.216711 mltlk-0.1.6/PKG-INFO
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      311 2023-05-26 08:20:29.000000 mltlk-0.1.6/README.md
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    31369 2023-05-30 11:10:44.000000 mltlk-0.1.6/Spiral.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    40302 2023-05-30 11:10:10.000000 mltlk-0.1.6/Weather.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    48621 2023-05-30 11:09:12.000000 mltlk-0.1.6/Wikipedia.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    33244 2023-05-30 13:13:01.000000 mltlk-0.1.6/Wikipedia_exploration.ipynb
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    50000 2023-05-30 11:12:17.000000 mltlk-0.1.6/Wikipedia_word2vec.ipynb
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 13:14:13.182569 mltlk-0.1.6/data/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     4505 2021-03-10 11:22:51.000000 mltlk-0.1.6/data/spiral.csv
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      414 2023-05-26 08:09:41.000000 mltlk-0.1.6/data/weather.csv
+-rw-r--r--   0 johanhagelback   (503) staff       (20)  2061699 2019-12-13 13:20:58.000000 mltlk-0.1.6/data/wikipedia_300.csv.gz
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 13:14:13.206134 mltlk-0.1.6/mltlk/
+-rwxr-xr-x   0 johanhagelback   (503) staff       (20)      109 2023-05-30 13:12:34.000000 mltlk-0.1.6/mltlk/__init__.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     7897 2023-05-30 13:12:12.000000 mltlk-0.1.6/mltlk/exploration_textdata.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)    32219 2023-05-30 10:44:16.000000 mltlk-0.1.6/mltlk/ml.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     3324 2023-05-25 12:08:40.000000 mltlk-0.1.6/mltlk/resampling.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     2606 2023-05-30 07:25:34.000000 mltlk-0.1.6/mltlk/utils.py
+-rw-r--r--   0 johanhagelback   (503) staff       (20)     4854 2023-05-29 08:24:02.000000 mltlk-0.1.6/mltlk/word2vec.py
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 13:14:13.213591 mltlk-0.1.6/mltlk.egg-info/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      233 2023-05-30 13:14:12.000000 mltlk-0.1.6/mltlk.egg-info/PKG-INFO
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      470 2023-05-30 13:14:13.000000 mltlk-0.1.6/mltlk.egg-info/SOURCES.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        1 2023-05-30 13:14:12.000000 mltlk-0.1.6/mltlk.egg-info/dependency_links.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       74 2023-05-30 13:14:12.000000 mltlk-0.1.6/mltlk.egg-info/requires.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        6 2023-05-30 13:14:12.000000 mltlk-0.1.6/mltlk.egg-info/top_level.txt
+-rw-r--r--   0 johanhagelback   (503) staff       (20)       38 2023-05-30 13:14:13.217758 mltlk-0.1.6/setup.cfg
+-rw-r--r--   0 johanhagelback   (503) staff       (20)      361 2023-05-30 13:12:25.000000 mltlk-0.1.6/setup.py
+drwxr-xr-x   0 johanhagelback   (503) staff       (20)        0 2023-05-30 13:14:13.214912 mltlk-0.1.6/stopwords/
+-rw-r--r--   0 johanhagelback   (503) staff       (20)        5 2023-05-29 06:34:12.000000 mltlk-0.1.6/stopwords/custom.csv
```

### Comparing `mltlk-0.1.5/LICENSE` & `mltlk-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.5/Spiral.ipynb` & `mltlk-0.1.6/Spiral.ipynb`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.5/Weather.ipynb` & `mltlk-0.1.6/Weather.ipynb`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.5/Wikipedia.ipynb` & `mltlk-0.1.6/Wikipedia.ipynb`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.5/Wikipedia_exploration.ipynb` & `mltlk-0.1.6/Wikipedia_exploration.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999826388888889%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': ['0.1.6\\n']}}}}"}*

```diff
@@ -12,15 +12,15 @@
             "execution_count": 1,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "0.1.5\n"
+                        "0.1.6\n"
                     ]
                 }
             ],
             "source": [
                 "import mltlk\n",
                 "print(mltlk.__version__)\n",
                 "from mltlk import *"
```

### Comparing `mltlk-0.1.5/Wikipedia_word2vec.ipynb` & `mltlk-0.1.6/Wikipedia_word2vec.ipynb`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.5/data/spiral.csv` & `mltlk-0.1.6/data/spiral.csv`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.5/data/wikipedia_300.csv.gz` & `mltlk-0.1.6/data/wikipedia_300.csv.gz`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.5/mltlk/exploration_textdata.py` & `mltlk-0.1.6/mltlk/exploration_textdata.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 from collections import Counter
 from customized_table import *
 from .utils import *
 
 
 # Caches to speed up processing
 cache_topcats = {}
-cache_overlap_js = {}
-cache_overlap_oc = {}
+cache_overlap = {}
 
 
 #
 # Builds a corpus from text data
 #
 def build_corpus(session):
     if session is None:
@@ -177,50 +176,46 @@
     print()
     
 
 #
 # Check overlapping words between all categories
 #
 def overlap_all_categories(corpus, n=10, sidx=0, similarity="jaccard"):
-    global cache_overlap_js, cache_overlap_oc
+    global cache_overlap
     similarity = similarity.lower()
     
     # Check all combinations of categories
     cats = sorted(corpus["categories"])
     tab = []
     for i in range(0,len(cats)):
         for j in range(i,len(cats)):
             if i != j:
                 cat1 = cats[i]
                 cat2 = cats[j]
                 key = f"{cat1}-{cat2}"
                 
                 # Calculate similarity
-                if key in cache_overlap_js and key in cache_overlap_oc:
-                    res_js = cache_overlap_js[key]
-                    res_oc = cache_overlap_oc[key]
+                if key in cache_overlap:
+                    res = cache_overlap[key]
                 else:
                     wrds1 = set(corpus["words_per_category"][cat1])
                     wrds2 = set(corpus["words_per_category"][cat2])
                     tot = wrds1.union(wrds2)
                     overlap = wrds1.intersection(wrds2)
-                    res_js = [len(overlap)/len(tot), len(wrds1), len(wrds2)]
-                    res_oc = [len(overlap)/min(len(wrds2),len(wrds2)), len(wrds1), len(wrds2)]
-                    cache_overlap_js[key] = res_js
-                    cache_overlap_oc[key] = res_oc
+                    res = [len(overlap)/len(tot), len(overlap)/min(len(wrds1),len(wrds2)), len(wrds1), len(wrds2)]
+                    cache_overlap[key] = res
             
                 # Check similarity to use
                 if similarity in [2, "oc", "overlap coefficient", "overlap"]:
-                    res = res_oc
+                    tab.append([cat1, res[2], cat2, res[3], res[1]])
                 elif similarity in [1, "ji", "jaccard similarity", "jaccard"]:
-                    res = res_js
+                    tab.append([cat1, res[2], cat2, res[3], res[0]])
                 else:
                     error("Unknown similarity " + colored(similarity, "cyan"))
                     return
-                tab.append([cat1, res[1], cat2, res[2], res[0]])
     tab = sorted(tab, key=lambda x: x[4], reverse=True)
     
     # Start and end index
     si = sidx
     if sidx < 0:
         si = len(tab) + sidx
     
@@ -229,8 +224,8 @@
     t.column_style([1, 3], {"color": "name"})
     t.column_style([2, 4], {"color": "value"})
     t.column_style(5, {"color": "percent", "num-format": "pct-2"})
     for i,r in enumerate(tab[si:si+n]):
         t.add_row([si+i] + r)
     print()
     t.display()
-    print()
+    print()
```

### Comparing `mltlk-0.1.5/mltlk/ml.py` & `mltlk-0.1.6/mltlk/ml.py`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.5/mltlk/resampling.py` & `mltlk-0.1.6/mltlk/resampling.py`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.5/mltlk/utils.py` & `mltlk-0.1.6/mltlk/utils.py`

 * *Files identical despite different names*

### Comparing `mltlk-0.1.5/mltlk/word2vec.py` & `mltlk-0.1.6/mltlk/word2vec.py`

 * *Files identical despite different names*

