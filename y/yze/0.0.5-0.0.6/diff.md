# Comparing `tmp/yze-0.0.5.tar.gz` & `tmp/yze-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yze-0.0.5.tar", last modified: Wed May 24 12:36:22 2023, max compression
+gzip compressed data, was "yze-0.0.6.tar", last modified: Tue May 30 20:56:10 2023, max compression
```

## Comparing `yze-0.0.5.tar` & `yze-0.0.6.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-24 12:36:22.517734 yze-0.0.5/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4584 2023-05-24 12:36:22.517734 yze-0.0.5/PKG-INFO
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4086 2023-05-24 12:33:26.000000 yze-0.0.5/README.md
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      735 2023-05-24 12:35:46.000000 yze-0.0.5/pyproject.toml
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)       38 2023-05-24 12:36:22.517734 yze-0.0.5/setup.cfg
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-24 12:36:22.509734 yze-0.0.5/src/
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-24 12:36:22.517734 yze-0.0.5/src/yze/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4193 2023-04-26 10:10:00.000000 yze-0.0.5/src/yze/benchmark_mutant.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)    17913 2023-05-24 12:08:52.000000 yze-0.0.5/src/yze/dice.py
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     5162 2023-05-24 11:38:28.000000 yze-0.0.5/src/yze/mutant_odds_of_pushing.py
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-24 12:36:22.517734 yze-0.0.5/src/yze.egg-info/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     4584 2023-05-24 12:36:22.000000 yze-0.0.5/src/yze.egg-info/PKG-INFO
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      283 2023-05-24 12:36:22.000000 yze-0.0.5/src/yze.egg-info/SOURCES.txt
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)        1 2023-05-24 12:36:22.000000 yze-0.0.5/src/yze.egg-info/dependency_links.txt
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)      120 2023-05-24 12:36:22.000000 yze-0.0.5/src/yze.egg-info/entry_points.txt
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)        4 2023-05-24 12:36:22.000000 yze-0.0.5/src/yze.egg-info/top_level.txt
-drwxr-xr-x   0 nicolas   (1000) nicolas   (1000)        0 2023-05-24 12:36:22.517734 yze-0.0.5/tests/
--rw-r--r--   0 nicolas   (1000) nicolas   (1000)     3611 2023-05-24 11:53:49.000000 yze-0.0.5/tests/test_yze_dice.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-05-30 20:56:10.199971 yze-0.0.6/
+-rw-r--r--   0 nicolas    (501) staff       (20)     4899 2023-05-30 20:56:10.199860 yze-0.0.6/PKG-INFO
+-rw-r--r--   0 nicolas    (501) staff       (20)     4401 2023-05-30 20:52:24.000000 yze-0.0.6/README.md
+-rw-r--r--   0 nicolas    (501) staff       (20)      735 2023-05-30 20:54:23.000000 yze-0.0.6/pyproject.toml
+-rw-r--r--   0 nicolas    (501) staff       (20)       38 2023-05-30 20:56:10.200002 yze-0.0.6/setup.cfg
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-05-30 20:56:10.198207 yze-0.0.6/src/
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-05-30 20:56:10.198982 yze-0.0.6/src/yze/
+-rw-r--r--   0 nicolas    (501) staff       (20)        0 2023-05-23 06:35:38.000000 yze-0.0.6/src/yze/__init__.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     5518 2023-05-30 20:53:35.000000 yze-0.0.6/src/yze/benchmark_mutant.py
+-rw-r--r--   0 nicolas    (501) staff       (20)    17913 2023-05-30 10:50:59.000000 yze-0.0.6/src/yze/dice.py
+-rw-r--r--   0 nicolas    (501) staff       (20)     5161 2023-05-30 20:51:44.000000 yze-0.0.6/src/yze/mutant_odds_of_pushing.py
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-05-30 20:56:10.199587 yze-0.0.6/src/yze.egg-info/
+-rw-r--r--   0 nicolas    (501) staff       (20)     4899 2023-05-30 20:56:10.000000 yze-0.0.6/src/yze.egg-info/PKG-INFO
+-rw-r--r--   0 nicolas    (501) staff       (20)      303 2023-05-30 20:56:10.000000 yze-0.0.6/src/yze.egg-info/SOURCES.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        1 2023-05-30 20:56:10.000000 yze-0.0.6/src/yze.egg-info/dependency_links.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)      120 2023-05-30 20:56:10.000000 yze-0.0.6/src/yze.egg-info/entry_points.txt
+-rw-r--r--   0 nicolas    (501) staff       (20)        4 2023-05-30 20:56:10.000000 yze-0.0.6/src/yze.egg-info/top_level.txt
+drwxr-xr-x   0 nicolas    (501) staff       (20)        0 2023-05-30 20:56:10.199710 yze-0.0.6/tests/
+-rw-r--r--   0 nicolas    (501) staff       (20)     3611 2023-05-30 10:50:59.000000 yze-0.0.6/tests/test_yze_dice.py
```

### Comparing `yze-0.0.5/pyproject.toml` & `yze-0.0.6/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "yze"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Nicolas Legrand", email="nicolas.legrand@gmail.com" },
 ]
 description = "A small package to handle YZE games mechanics"
 readme = "README.md"
 requires-python = ">=3.11"
 classifiers = [
```

### Comparing `yze-0.0.5/src/yze/benchmark_mutant.py` & `yze-0.0.6/src/yze/benchmark_mutant.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,14 +13,22 @@
 # WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 # ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 # OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 
 from yze.dice import MutantDicePool
 import argparse
 import pprint
+import logging, sys, os
+
+DEBUG=os.getenv('DEBUG')
+loglevel = logging.INFO
+if DEBUG:
+    loglevel = logging.DEBUG
+logging.basicConfig(stream=sys.stderr, level=loglevel)
+
 
 def multiple_throws(throws=10000, attribute=1, skill=0, gear=0):
     """Throw dice <throws> times, store results in <results>, return
     results.
     """
     results = {
         'atleast_one': 0,
@@ -29,15 +37,15 @@
         'atleast_one_gear_botch': 0,
         'successes': {},
         'pushed_successes': {},
         'attribute_botched': {},
         'gear_botched': {},
     }
     
-    print(f'Throwing dice {throws} times !')
+    print(f'Throwing dice pool (attribute: {attribute}, skill: {skill}, gear: {gear}) {throws} times !')
     for i in range(int(throws)):
         d = MutantDicePool(attr=int(attribute), skill=int(skill), gear=int(gear))
         res = d.throw()
         pushed_res = d.push()
         successes = [x for x in d.result['attr'] + d.result['skill'] + d.result['gear'] if x == 6]
         if len(successes) > 0:
             results['atleast_one'] += 1
@@ -64,35 +72,60 @@
             results['atleast_one_gear_botch'] += 1
             if len(gear_botched) not in results['gear_botched']:
                 results['gear_botched'][len(gear_botched)] = 1
             else:
                 results['gear_botched'][len(gear_botched)] += 1
     return results
 
+
+def complete_benchmark():
+    """In dev yet, will launch multiple multiple_throws so as to try
+    to have almost exhaustive benchmarks.
+
+    """
+    pass
+def print_result(result_name, result, throws):
+    """Pretty print result to terminal
+    """
+    print (f'{result_name}: {result * 100 / throws} %')
+
+def print_result_list(result_list_name, result_list, throws):
+    """Pretty print the full result list
+    """
+    print(f'{result_list_name}:')
+    for key in sorted(result_list):
+        print(f'    chances to get {key}: {result_list[key] * 100 / throws} %')
+
+
 def main():
     """Fetch args from the commandline and proceed.
     """
     parser = argparse.ArgumentParser(
                         prog='benchmark_mutant',
                         description='make a lot of YZE rolls so as to have an idea of chances of success',
                         epilog='')
 
-    parser.add_argument('-t', '--throws', default=10000)      # option that takes a value
+    parser.add_argument('-t', '--throws', default=100000)      # option that takes a value
     parser.add_argument('-a', '--attribute', default=1)
     parser.add_argument('-s', '--skill', default=0)
     parser.add_argument('-g', '--gear', default=0)
+    parser.add_argument('-c', '--complete', action='store_true')
 
     args = parser.parse_args()
+    throws = int(args.throws)
 
-    results = multiple_throws(args.throws, args.attribute, args.skill, args.gear)
-
-    print (f'    at least one success : {results["atleast_one"]}')
-    print (f'    at least one pushed success : {results["atleast_one_pushed"]}')
-    print (f'    at least one damage to attribute : {results["atleast_one_attr_botch"]}')
-    print (f'    at least one damage to gear : {results["atleast_one_gear_botch"]}')
-
-
-    pp = pprint.PrettyPrinter(indent=4)
-    pp.pprint(results)
+    if args.complete:
+        print("Complete benchmark not implemented yet, sorry!")
+    else:
+        results = multiple_throws(throws, args.attribute, args.skill, args.gear)
+        print_result('at least one success', results['atleast_one'], throws)
+        print_result('at least on pushed succes', results['atleast_one_pushed'], throws)
+        print_result('at least one damage to attribute', results['atleast_one_attr_botch'], throws)
+        print_result('at least one damage to gear', results['atleast_one_gear_botch'], throws)
+        print_result_list('Successes on first roll', results['successes'], throws)
+        print_result_list('Successes on pushed roll', results['pushed_successes'], throws)
+        print_result_list('Attribute damage', results['attribute_botched'], throws)
+        print_result_list('Gear damage', results['gear_botched'], throws)
+        logging.debug(results)
 
 if __name__ == "__main__":
     main()
```

### Comparing `yze-0.0.5/src/yze/dice.py` & `yze-0.0.6/src/yze/dice.py`

 * *Files identical despite different names*

### Comparing `yze-0.0.5/src/yze/mutant_odds_of_pushing.py` & `yze-0.0.6/src/yze/mutant_odds_of_pushing.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     """Fetch args from the commandline and proceed.
     """
     parser = argparse.ArgumentParser(
                         prog='mutant_odds_of_pushing',
                         description="""Once you get a result, what are your odds when pushing it?
                         feed this command your results and see what is likely or not to happen""",
                         epilog="""Experimental probabilities made with pseudo random numbers.
-                        Maybie it’s not the best you can get :).""")
+                        Maybe it’s not the best you can get :).""")
 
     parser.add_argument('-t', '--throws', default=100000)      # option that takes a value
     parser.add_argument('-a', '--attribute_dice',
                         help="List your dice results eg: 253",
                         required=True)
     parser.add_argument('-s', '--skill_dice',
                         default=0,
```

### Comparing `yze-0.0.5/tests/test_yze_dice.py` & `yze-0.0.6/tests/test_yze_dice.py`

 * *Files identical despite different names*

